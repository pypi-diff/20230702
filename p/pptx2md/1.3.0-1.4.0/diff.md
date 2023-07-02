# Comparing `tmp/pptx2md-1.3.0.tar.gz` & `tmp/pptx2md-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx2md-1.3.0.tar", max compression
+gzip compressed data, was "pptx2md-1.4.0.tar", max compression
```

## Comparing `pptx2md-1.3.0.tar` & `pptx2md-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     3287 2023-03-16 15:51:00.353572 pptx2md-1.3.0/pptx2md/__init__.py
--rw-r--r--   0        0        0     4425 2023-03-16 15:51:00.353572 pptx2md-1.3.0/pptx2md/__main__.py
--rw-r--r--   0        0        0      794 2022-02-28 16:22:16.322722 pptx2md-1.3.0/pptx2md/global_var.py
--rw-r--r--   0        0        0     5609 2022-02-28 16:22:17.723400 pptx2md-1.3.0/pptx2md/outputter.py
--rw-r--r--   0        0        0     6653 2023-03-16 15:51:00.354574 pptx2md-1.3.0/pptx2md/parser.py
--rw-r--r--   0        0        0      846 2022-02-28 16:22:21.552969 pptx2md-1.3.0/pptx2md/tools.py
--rw-r--r--   0        0        0      602 2023-03-16 15:51:17.174197 pptx2md-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 pptx2md-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3287 2023-03-16 15:51:00.353572 pptx2md-1.4.0/pptx2md/__init__.py
+-rw-r--r--   0        0        0     4569 2023-07-01 23:59:27.523065 pptx2md-1.4.0/pptx2md/__main__.py
+-rw-r--r--   0        0        0      809 2023-07-01 23:59:27.524066 pptx2md-1.4.0/pptx2md/global_var.py
+-rw-r--r--   0        0        0     5609 2022-02-28 16:22:17.723400 pptx2md-1.4.0/pptx2md/outputter.py
+-rw-r--r--   0        0        0     6721 2023-07-01 23:59:27.525152 pptx2md-1.4.0/pptx2md/parser.py
+-rw-r--r--   0        0        0      846 2022-02-28 16:22:21.552969 pptx2md-1.4.0/pptx2md/tools.py
+-rw-r--r--   0        0        0      602 2023-07-01 23:59:33.218348 pptx2md-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      797 2023-07-02 00:01:49.617844 pptx2md-1.4.0/setup.py
+-rw-r--r--   0        0        0      724 2023-07-02 00:01:49.617844 pptx2md-1.4.0/PKG-INFO
```

### Comparing `pptx2md-1.3.0/pptx2md/__init__.py` & `pptx2md-1.4.0/pptx2md/__init__.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.3.0/pptx2md/__main__.py` & `pptx2md-1.4.0/pptx2md/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
   arg_parser.add_argument('--disable-escaping', help='do not attempt to escape special characters', action="store_true")
   arg_parser.add_argument('--wiki', help='generate output as wikitext(TiddlyWiki)', action="store_true")
   arg_parser.add_argument('--mdk', help='generate output as madoko markdown', action="store_true")
   arg_parser.add_argument('--min-block-size',
                           help='the minimum character number of a text block to be converted',
                           type=int,
                           default=15)
+  arg_parser.add_argument("--page", help="only convert the specified page", type=int, default=None)
   return arg_parser.parse_args()
 
 
 def main():
   args = parse_args()
 
   file_path = args.pptx_path
@@ -99,14 +100,17 @@
     g.disable_color = False
 
   if args.disable_escaping:
     g.disable_escaping = True
   else:
     g.disable_escaping = False
 
+  if args.page:
+    g.page = args.page
+
   if not os.path.exists(file_path):
     print(f'source file {file_path} not exist!')
     print(f'absolute path: {os.path.abspath(file_path)}')
     exit(0)
   try:
     prs = Presentation(file_path)
   except KeyError as err:
```

### Comparing `pptx2md-1.3.0/pptx2md/global_var.py` & `pptx2md-1.4.0/pptx2md/global_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,7 +30,9 @@
 
 # global variables
 g.titles = {}
 g.file_prefix = '1'
 
 g.last_title = {}
 g.max_custom_title = 1
+
+g.page = None
```

### Comparing `pptx2md-1.3.0/pptx2md/outputter.py` & `pptx2md-1.4.0/pptx2md/outputter.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.3.0/pptx2md/parser.py` & `pptx2md-1.4.0/pptx2md/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,16 @@
 
 # main
 def parse(prs, outputer):
   global out
   out = outputer
   notes = []
   for idx, slide in enumerate(tqdm(prs.slides, desc='Converting slides')):
+    if g.page is not None and idx + 1 != g.page:
+        continue
     shapes = []
     try:
       shapes = sorted(ungroup_shapes(slide.shapes), key=attrgetter('top', 'left'))
     except:
       print('Bad shapes encountered in this slide. Please check or move them and try again.')
       print('shapes:')
       for sp in slide.shapes:
```

### Comparing `pptx2md-1.3.0/pptx2md/tools.py` & `pptx2md-1.4.0/pptx2md/tools.py`

 * *Files identical despite different names*

### Comparing `pptx2md-1.3.0/pyproject.toml` & `pptx2md-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pptx2md"
-version = "1.3.0"
+version = "1.4.0"
 description = "This package converts pptx to markdown"
 repository = "https://github.com/ssine/pptx2md"
 authors = ["Liu Siyao <liu.siyao@qq.com>"]
 license = "MIT Licence"
 
 [tool.poetry.scripts]
 pptx2md = "pptx2md.__main__:main"
```

### Comparing `pptx2md-1.3.0/PKG-INFO` & `pptx2md-1.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pptx2md
-Version: 1.3.0
+Version: 1.4.0
 Summary: This package converts pptx to markdown
 Home-page: https://github.com/ssine/pptx2md
 License: MIT Licence
 Author: Liu Siyao
 Author-email: liu.siyao@qq.com
 Requires-Python: >=3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=6.0.0)
 Requires-Dist: python-pptx (>=0.6.18)
 Requires-Dist: rapidfuzz (>=0.10.0)
 Requires-Dist: tqdm (>=4)
 Project-URL: Repository, https://github.com/ssine/pptx2md
```

