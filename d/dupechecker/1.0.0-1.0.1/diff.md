# Comparing `tmp/dupechecker-1.0.0.tar.gz` & `tmp/dupechecker-1.0.1.tar.gz`

## Comparing `dupechecker-1.0.0.tar` & `dupechecker-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 dupechecker-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    34158 2020-02-02 00:00:00.000000 dupechecker-1.0.0/docs/dupechecker.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-1.0.0/docs/index.html
--rw-r--r--   0        0        0    24923 2020-02-02 00:00:00.000000 dupechecker-1.0.0/docs/search.js
--rw-r--r--   0        0        0   121350 2020-02-02 00:00:00.000000 dupechecker-1.0.0/docs/dupechecker/dupechecker.html
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dupechecker-1.0.0/src/dupechecker/__init__.py
--rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 dupechecker-1.0.0/src/dupechecker/dupechecker.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-1.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 dupechecker-1.0.0/README.md
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dupechecker-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 dupechecker-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 dupechecker-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0    34158 2020-02-02 00:00:00.000000 dupechecker-1.0.1/docs/dupechecker.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-1.0.1/docs/index.html
+-rw-r--r--   0        0        0    24923 2020-02-02 00:00:00.000000 dupechecker-1.0.1/docs/search.js
+-rw-r--r--   0        0        0   121302 2020-02-02 00:00:00.000000 dupechecker-1.0.1/docs/dupechecker/dupechecker.html
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dupechecker-1.0.1/src/dupechecker/__init__.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 dupechecker-1.0.1/src/dupechecker/dupechecker.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 dupechecker-1.0.1/README.md
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dupechecker-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 dupechecker-1.0.1/PKG-INFO
```

### Comparing `dupechecker-1.0.0/docs/dupechecker.html` & `dupechecker-1.0.1/docs/dupechecker.html`

 * *Files identical despite different names*

### Comparing `dupechecker-1.0.0/docs/search.js` & `dupechecker-1.0.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `dupechecker-1.0.0/docs/dupechecker/dupechecker.html` & `dupechecker-1.0.1/docs/dupechecker/dupechecker.html`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 </span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="k">return</span> <span class="n">matching_sets</span>
 </span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
 </span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
 </span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="k">def</span> <span class="nf">group_by_size</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
 </span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="sd">&quot;&quot;&quot;Returns a list of lists where each sublist is a list of files that have the same size.&quot;&quot;&quot;</span>
 </span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="n">sizes</span> <span class="o">=</span> <span class="p">{}</span>
 </span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">paths</span><span class="p">:</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">size</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">size</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span>
 </span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="k">if</span> <span class="n">size</span> <span class="ow">in</span> <span class="n">sizes</span><span class="p">:</span>
 </span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">size</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
 </span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="k">else</span><span class="p">:</span>
 </span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">size</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="p">]</span>
 </span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="n">sizes</span><span class="o">.</span><span class="n">values</span><span class="p">())</span>
 </span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>
 </span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>
@@ -237,15 +237,15 @@
 </span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>                <span class="p">)</span>
 </span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>            <span class="p">)</span>
 </span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
 </span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="k">lambda</span><span class="p">:</span> <span class="nb">sum</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>            <span class="n">start_size</span> <span class="o">=</span> <span class="n">size</span><span class="p">()</span>
 </span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
 </span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">start_size</span> <span class="o">-</span> <span class="n">size</span><span class="p">()</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 </span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">else</span><span class="p">:</span>
 </span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
 </span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
 </span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>
 </span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
 </span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
@@ -294,15 +294,15 @@
 
     </div>
     <a class="headerlink" href="#group_by_size"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="group_by_size-29"><a href="#group_by_size-29"><span class="linenos">29</span></a><span class="k">def</span> <span class="nf">group_by_size</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
 </span><span id="group_by_size-30"><a href="#group_by_size-30"><span class="linenos">30</span></a>    <span class="sd">&quot;&quot;&quot;Returns a list of lists where each sublist is a list of files that have the same size.&quot;&quot;&quot;</span>
 </span><span id="group_by_size-31"><a href="#group_by_size-31"><span class="linenos">31</span></a>    <span class="n">sizes</span> <span class="o">=</span> <span class="p">{}</span>
 </span><span id="group_by_size-32"><a href="#group_by_size-32"><span class="linenos">32</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">paths</span><span class="p">:</span>
-</span><span id="group_by_size-33"><a href="#group_by_size-33"><span class="linenos">33</span></a>        <span class="n">size</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="group_by_size-33"><a href="#group_by_size-33"><span class="linenos">33</span></a>        <span class="n">size</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span>
 </span><span id="group_by_size-34"><a href="#group_by_size-34"><span class="linenos">34</span></a>        <span class="k">if</span> <span class="n">size</span> <span class="ow">in</span> <span class="n">sizes</span><span class="p">:</span>
 </span><span id="group_by_size-35"><a href="#group_by_size-35"><span class="linenos">35</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">size</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
 </span><span id="group_by_size-36"><a href="#group_by_size-36"><span class="linenos">36</span></a>        <span class="k">else</span><span class="p">:</span>
 </span><span id="group_by_size-37"><a href="#group_by_size-37"><span class="linenos">37</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">size</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="p">]</span>
 </span><span id="group_by_size-38"><a href="#group_by_size-38"><span class="linenos">38</span></a>    <span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="n">sizes</span><span class="o">.</span><span class="n">values</span><span class="p">())</span>
 </span></pre></div>
 
@@ -513,15 +513,15 @@
 </span><span id="main-164"><a href="#main-164"><span class="linenos">164</span></a>                <span class="p">)</span>
 </span><span id="main-165"><a href="#main-165"><span class="linenos">165</span></a>            <span class="p">)</span>
 </span><span id="main-166"><a href="#main-166"><span class="linenos">166</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
 </span><span id="main-167"><a href="#main-167"><span class="linenos">167</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="k">lambda</span><span class="p">:</span> <span class="nb">sum</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="main-168"><a href="#main-168"><span class="linenos">168</span></a>            <span class="n">start_size</span> <span class="o">=</span> <span class="n">size</span><span class="p">()</span>
 </span><span id="main-169"><a href="#main-169"><span class="linenos">169</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
 </span><span id="main-170"><a href="#main-170"><span class="linenos">170</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">start_size</span> <span class="o">-</span> <span class="n">size</span><span class="p">()</span>
-</span><span id="main-171"><a href="#main-171"><span class="linenos">171</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="main-171"><a href="#main-171"><span class="linenos">171</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_bytes</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 </span><span id="main-172"><a href="#main-172"><span class="linenos">172</span></a>    <span class="k">else</span><span class="p">:</span>
 </span><span id="main-173"><a href="#main-173"><span class="linenos">173</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
 </span></pre></div>
```

#### html2text {}

```diff
@@ -43,15 +43,15 @@
 _26
 _27
 _28def group_by_size(paths: list[Pathier]) -> list[list[Pathier]]:
 _29    """Returns a list of lists where each sublist is a list of files that
 have the same size."""
 _30    sizes = {}
 _31    for path in paths:
-_32        size = path.size()
+_32        size = path.size
 _33        if size in sizes:
 _34            sizes[size].append(path)
 _35        else:
 _36            sizes[size] = [path]
 _37    return list(sizes.values())
 _38
 _39
@@ -194,15 +194,15 @@
 165        if args.delete_dupes or args.autodelete:
 166            size = lambda: sum(path.size() for path in args.paths)  # type:
 ignore
 167            start_size = size()
 168            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
 169            deleted_size = start_size - size()
-170            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+170            print(f"Deleted {Pathier.format_bytes(deleted_size)}.")
 171    else:
 172        print("No duplicates detected.")
 173
 174
 175if __name__ == "__main__":
 176    main(get_args())
   ⁰
@@ -228,15 +228,15 @@
 paths: list[pathier.pathier.Pathier]) -> list[list[pathier.pathier.Pathier]]:
 View Source
 29def group_by_size(paths: list[Pathier]) -> list[list[Pathier]]:
 30    """Returns a list of lists where each sublist is a list of files that
 have the same size."""
 31    sizes = {}
 32    for path in paths:
-33        size = path.size()
+33        size = path.size
 34        if size in sizes:
 35            sizes[size].append(path)
 36        else:
 37            sizes[size] = [path]
 38    return list(sizes.values())
 Returns a list of lists where each sublist is a list of files that have the
 same size.
@@ -385,11 +385,11 @@
 166        if args.delete_dupes or args.autodelete:
 167            size = lambda: sum(path.size() for path in args.paths)  # type:
 ignore
 168            start_size = size()
 169            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
 170            deleted_size = start_size - size()
-171            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+171            print(f"Deleted {Pathier.format_bytes(deleted_size)}.")
 172    else:
 173        print("No duplicates detected.")
```

### Comparing `dupechecker-1.0.0/src/dupechecker/dupechecker.py` & `dupechecker-1.0.1/src/dupechecker/dupechecker.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     return matching_sets
 
 
 def group_by_size(paths: list[Pathier]) -> list[list[Pathier]]:
     """Returns a list of lists where each sublist is a list of files that have the same size."""
     sizes = {}
     for path in paths:
-        size = path.size()
+        size = path.size
         if size in sizes:
             sizes[size].append(path)
         else:
             sizes[size] = [path]
     return list(sizes.values())
 
 
@@ -163,14 +163,14 @@
                 )
             )
         if args.delete_dupes or args.autodelete:
             size = lambda: sum(path.size() for path in args.paths)  # type: ignore
             start_size = size()
             delete_wizard(matches) if args.delete_dupes else autodelete(matches)
             deleted_size = start_size - size()
-            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+            print(f"Deleted {Pathier.format_bytes(deleted_size)}.")
     else:
         print("No duplicates detected.")
 
 
 if __name__ == "__main__":
     main(get_args())
```

### Comparing `dupechecker-1.0.0/LICENSE.txt` & `dupechecker-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dupechecker-1.0.0/README.md` & `dupechecker-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dupechecker-1.0.0/pyproject.toml` & `dupechecker-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,69 +6,65 @@
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6475 7065 6368 6563 6b65 7222 0d0a   "dupechecker"..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 2243  description = "C
 00000080: 6865 636b 2066 6f72 2061 6e64 2064 656c  heck for and del
 00000090: 6574 6520 6475 706c 6963 6174 6520 6669  ete duplicate fi
 000000a0: 6c65 7320 6672 6f6d 2074 6865 2063 6f6d  les from the com
 000000b0: 6d61 6e64 206c 696e 652e 220d 0a76 6572  mand line."..ver
-000000c0: 7369 6f6e 203d 2022 312e 302e 3022 0d0a  sion = "1.0.0"..
+000000c0: 7369 6f6e 203d 2022 312e 302e 3122 0d0a  sion = "1.0.1"..
 000000d0: 7265 7175 6972 6573 2d70 7974 686f 6e20  requires-python 
 000000e0: 3d20 223e 3d33 2e31 3022 0d0a 6465 7065  = ">=3.10"..depe
 000000f0: 6e64 656e 6369 6573 203d 205b 2267 7269  ndencies = ["gri
 00000100: 6464 6c65 222c 2022 7061 7468 6965 7222  ddle", "pathier"
 00000110: 2c20 2270 7269 6e74 6275 6464 6965 7322  , "printbuddies"
 00000120: 2c20 2270 7974 6573 7422 2c20 2279 6f75  , "pytest", "you
 00000130: 6e6f 7479 6f75 222c 2022 6e6f 6966 7469  notyou", "noifti
 00000140: 6d65 7222 5d0d 0a72 6561 646d 6520 3d20  mer"]..readme = 
 00000150: 2252 4541 444d 452e 6d64 220d 0a6b 6579  "README.md"..key
 00000160: 776f 7264 7320 3d20 5b22 6669 6c65 636d  words = ["filecm
 00000170: 7022 2c20 2263 6c69 222c 2022 6669 6c65  p", "cli", "file
 00000180: 7379 7374 656d 225d 0d0a 636c 6173 7369  system"]..classi
-00000190: 6669 6572 7320 3d20 5b0d 0a20 2020 2022  fiers = [..    "
-000001a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001c0: 3a20 3322 2c0d 0a20 2020 2022 4c69 6365  : 3",..    "Lice
-000001d0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001e0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-000001f0: 7365 222c 0d0a 2020 2020 224f 7065 7261  se",..    "Opera
-00000200: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000210: 5320 496e 6465 7065 6e64 656e 7422 2c0d  S Independent",.
-00000220: 0a20 2020 205d 0d0a 0d0a 5b5b 7072 6f6a  .    ]....[[proj
-00000230: 6563 742e 6175 7468 6f72 735d 5d0d 0a6e  ect.authors]]..n
-00000240: 616d 6520 3d20 224d 6174 7420 4d61 6e65  ame = "Matt Mane
-00000250: 7322 0d0a 656d 6169 6c20 3d20 226d 6174  s"..email = "mat
-00000260: 746d 616e 6573 4070 6d2e 6d65 220d 0a0d  tmanes@pm.me"...
-00000270: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
-00000280: 0a22 486f 6d65 7061 6765 2220 3d20 2268  ."Homepage" = "h
-00000290: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000002a0: 6d2f 6d61 7474 2d6d 616e 6573 2f64 7570  m/matt-manes/dup
-000002b0: 6563 6865 636b 6572 220d 0a22 446f 6375  echecker".."Docu
-000002c0: 6d65 6e74 6174 696f 6e22 203d 2022 6874  mentation" = "ht
-000002d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000002e0: 2f6d 6174 742d 6d61 6e65 732f 6475 7065  /matt-manes/dupe
-000002f0: 6368 6563 6b65 722f 7472 6565 2f6d 6169  checker/tree/mai
-00000300: 6e2f 646f 6373 220d 0a22 536f 7572 6365  n/docs".."Source
-00000310: 2063 6f64 6522 203d 2022 6874 7470 733a   code" = "https:
-00000320: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
-00000330: 742d 6d61 6e65 732f 6475 7065 6368 6563  t-manes/dupechec
-00000340: 6b65 722f 7472 6565 2f6d 6169 6e2f 7372  ker/tree/main/sr
-00000350: 632f 6475 7065 6368 6563 6b65 7222 0d0a  c/dupechecker"..
-00000360: 0d0a 5b74 6f6f 6c2e 7079 7465 7374 2e69  ..[tool.pytest.i
-00000370: 6e69 5f6f 7074 696f 6e73 5d0d 0a61 6464  ni_options]..add
-00000380: 6f70 7473 203d 205b 0d0a 2020 2020 222d  opts = [..    "-
-00000390: 2d69 6d70 6f72 742d 6d6f 6465 3d69 6d70  -import-mode=imp
-000003a0: 6f72 746c 6962 222c 0d0a 2020 2020 5d0d  ortlib",..    ].
-000003b0: 0a70 7974 686f 6e70 6174 6820 3d20 2273  .pythonpath = "s
-000003c0: 7263 220d 0a0d 0a5b 746f 6f6c 2e68 6174  rc"....[tool.hat
-000003d0: 6368 2e62 7569 6c64 2e74 6172 6765 7473  ch.build.targets
-000003e0: 2e73 6469 7374 5d0d 0a65 7863 6c75 6465  .sdist]..exclude
-000003f0: 203d 205b 0d0a 2020 2020 222e 636f 7665   = [..    ".cove
-00000400: 7261 6765 222c 0d0a 2020 2020 222e 7079  rage",..    ".py
-00000410: 7465 7374 5f63 6163 6865 222c 0d0a 2020  test_cache",..  
-00000420: 2020 222e 7673 636f 6465 222c 0d0a 2020    ".vscode",..  
-00000430: 2020 2274 6573 7473 222c 0d0a 2020 2020    "tests",..    
-00000440: 222e 6769 7469 676e 6f72 6522 0d0a 2020  ".gitignore"..  
-00000450: 2020 5d0d 0a5b 7072 6f6a 6563 742e 7363    ]..[project.sc
-00000460: 7269 7074 735d 0d0a 6475 7065 6368 6563  ripts]..dupechec
-00000470: 6b65 7220 3d20 2264 7570 6563 6865 636b  ker = "dupecheck
-00000480: 6572 2e64 7570 6563 6865 636b 6572 3a6d  er.dupechecker:m
-00000490: 6169 6e22 0d0a                           ain"..
+00000190: 6669 6572 7320 3d20 5b22 5072 6f67 7261  fiers = ["Progra
+000001a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000001b0: 3a20 5079 7468 6f6e 203a 3a20 3322 2c20  : Python :: 3", 
+000001c0: 224c 6963 656e 7365 203a 3a20 4f53 4920  "License :: OSI 
+000001d0: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
+000001e0: 4c69 6365 6e73 6522 2c20 224f 7065 7261  License", "Opera
+000001f0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00000200: 5320 496e 6465 7065 6e64 656e 7422 5d0d  S Independent"].
+00000210: 0a0d 0a5b 5b70 726f 6a65 6374 2e61 7574  ...[[project.aut
+00000220: 686f 7273 5d5d 0d0a 6e61 6d65 203d 2022  hors]]..name = "
+00000230: 4d61 7474 204d 616e 6573 220d 0a65 6d61  Matt Manes"..ema
+00000240: 696c 203d 2022 6d61 7474 6d61 6e65 7340  il = "mattmanes@
+00000250: 706d 2e6d 6522 0d0a 0d0a 5b70 726f 6a65  pm.me"....[proje
+00000260: 6374 2e75 726c 735d 0d0a 486f 6d65 7061  ct.urls]..Homepa
+00000270: 6765 203d 2022 6874 7470 733a 2f2f 6769  ge = "https://gi
+00000280: 7468 7562 2e63 6f6d 2f6d 6174 742d 6d61  thub.com/matt-ma
+00000290: 6e65 732f 6475 7065 6368 6563 6b65 7222  nes/dupechecker"
+000002a0: 0d0a 446f 6375 6d65 6e74 6174 696f 6e20  ..Documentation 
+000002b0: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
+000002c0: 622e 636f 6d2f 6d61 7474 2d6d 616e 6573  b.com/matt-manes
+000002d0: 2f64 7570 6563 6865 636b 6572 2f74 7265  /dupechecker/tre
+000002e0: 652f 6d61 696e 2f64 6f63 7322 0d0a 2253  e/main/docs".."S
+000002f0: 6f75 7263 6520 636f 6465 2220 3d20 2268  ource code" = "h
+00000300: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000310: 6d2f 6d61 7474 2d6d 616e 6573 2f64 7570  m/matt-manes/dup
+00000320: 6563 6865 636b 6572 2f74 7265 652f 6d61  echecker/tree/ma
+00000330: 696e 2f73 7263 2f64 7570 6563 6865 636b  in/src/dupecheck
+00000340: 6572 220d 0a0d 0a5b 7072 6f6a 6563 742e  er"....[project.
+00000350: 7363 7269 7074 735d 0d0a 6475 7065 6368  scripts]..dupech
+00000360: 6563 6b65 7220 3d20 2264 7570 6563 6865  ecker = "dupeche
+00000370: 636b 6572 2e64 7570 6563 6865 636b 6572  cker.dupechecker
+00000380: 3a6d 6169 6e22 0d0a 0d0a 5b74 6f6f 6c5d  :main"....[tool]
+00000390: 0d0a 5b74 6f6f 6c2e 7079 7465 7374 2e69  ..[tool.pytest.i
+000003a0: 6e69 5f6f 7074 696f 6e73 5d0d 0a61 6464  ni_options]..add
+000003b0: 6f70 7473 203d 205b 222d 2d69 6d70 6f72  opts = ["--impor
+000003c0: 742d 6d6f 6465 3d69 6d70 6f72 746c 6962  t-mode=importlib
+000003d0: 225d 0d0a 7079 7468 6f6e 7061 7468 203d  "]..pythonpath =
+000003e0: 2022 7372 6322 0d0a 0d0a 5b74 6f6f 6c2e   "src"....[tool.
+000003f0: 6861 7463 682e 6275 696c 642e 7461 7267  hatch.build.targ
+00000400: 6574 732e 7364 6973 745d 0d0a 6578 636c  ets.sdist]..excl
+00000410: 7564 6520 3d20 5b22 2e63 6f76 6572 6167  ude = [".coverag
+00000420: 6522 2c20 222e 7079 7465 7374 5f63 6163  e", ".pytest_cac
+00000430: 6865 222c 2022 2e76 7363 6f64 6522 2c20  he", ".vscode", 
+00000440: 2274 6573 7473 222c 2022 2e67 6974 6967  "tests", ".gitig
+00000450: 6e6f 7265 225d 0d0a                      nore"]..
```

### Comparing `dupechecker-1.0.0/PKG-INFO` & `dupechecker-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dupechecker
-Version: 1.0.0
+Version: 1.0.1
 Summary: Check for and delete duplicate files from the command line.
 Project-URL: Homepage, https://github.com/matt-manes/dupechecker
 Project-URL: Documentation, https://github.com/matt-manes/dupechecker/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/dupechecker/tree/main/src/dupechecker
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,filecmp,filesystem
```

