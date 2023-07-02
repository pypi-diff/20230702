# Comparing `tmp/medit-0.0.3.tar.gz` & `tmp/medit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medit-0.0.3.tar", max compression
+gzip compressed data, was "medit-0.0.4.tar", max compression
```

## Comparing `medit-0.0.3.tar` & `medit-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1837 2023-07-02 11:33:38.540816 medit-0.0.3/Readme.md
--rw-r--r--   0        0        0        0 2023-06-18 13:03:52.329049 medit-0.0.3/medit/__init__.py
--rwxr-xr-x   0        0        0     2392 2023-07-02 11:33:38.540816 medit-0.0.3/medit/cli.py
--rw-r--r--   0        0        0     1862 2023-07-02 11:32:00.577590 medit-0.0.3/medit/medit.ui
--rw-r--r--   0        0        0     4732 2023-07-02 15:46:12.488227 medit-0.0.3/medit/meditor.py
--rw-r--r--   0        0        0     7055 2023-07-02 14:04:10.012757 medit-0.0.3/medit/mview.py
--rw-r--r--   0        0        0        0 2023-07-02 15:40:29.959990 medit-0.0.3/medit/styles/__init__.py
--rw-r--r--   0        0        0    18966 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/github-markdown-dark.css
--rw-r--r--   0        0        0    18979 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/github-markdown-light.css
--rw-r--r--   0        0        0     5061 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/pygments-solarized-style/solarized-dark.css
--rw-r--r--   0        0        0     5061 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/pygments-solarized-style/solarized-light.css
--rw-r--r--   0        0        0    36899 2023-07-02 11:33:38.541816 medit-0.0.3/medit/styles/external/solarized-dark-all-sites.css
--rw-r--r--   0        0        0    36890 2023-07-02 11:33:38.542816 medit-0.0.3/medit/styles/external/solarized-light-all-sites.css
--rw-r--r--   0        0        0     4282 2023-07-02 11:33:38.542816 medit-0.0.3/medit/styles/external/thomasf-solarized-css/solarized-dark.css
--rw-r--r--   0        0        0     4282 2023-07-02 11:33:38.542816 medit-0.0.3/medit/styles/external/thomasf-solarized-css/solarized-light.css
--rwxr-xr-x   0        0        0     6985 2023-07-02 15:43:07.140557 medit-0.0.3/medit/ui.py
--rw-r--r--   0        0        0     2389 2023-07-02 11:32:00.577590 medit-0.0.3/medit/utils.py
--rw-r--r--   0        0        0     2294 2023-07-02 15:46:49.941362 medit-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 medit-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2188 2023-07-02 16:12:39.541375 medit-0.0.4/Readme.md
+-rw-r--r--   0        0        0        0 2023-06-18 13:03:52.329049 medit-0.0.4/medit/__init__.py
+-rwxr-xr-x   0        0        0     2392 2023-07-02 11:33:38.540816 medit-0.0.4/medit/cli.py
+-rw-r--r--   0        0        0     2101 2023-07-02 15:49:58.797871 medit-0.0.4/medit/medit.ui
+-rw-r--r--   0        0        0     4732 2023-07-02 15:46:12.488227 medit-0.0.4/medit/meditor.py
+-rw-r--r--   0        0        0     7340 2023-07-02 16:11:41.761127 medit-0.0.4/medit/mview.py
+-rw-r--r--   0        0        0        0 2023-07-02 15:40:29.959990 medit-0.0.4/medit/styles/__init__.py
+-rw-r--r--   0        0        0    18966 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/github-markdown-dark.css
+-rw-r--r--   0        0        0    18979 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/github-markdown-light.css
+-rw-r--r--   0        0        0     5061 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/pygments-solarized-style/solarized-dark.css
+-rw-r--r--   0        0        0     5061 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/pygments-solarized-style/solarized-light.css
+-rw-r--r--   0        0        0    36899 2023-07-02 11:33:38.541816 medit-0.0.4/medit/styles/external/solarized-dark-all-sites.css
+-rw-r--r--   0        0        0    36890 2023-07-02 11:33:38.542816 medit-0.0.4/medit/styles/external/solarized-light-all-sites.css
+-rw-r--r--   0        0        0     4282 2023-07-02 11:33:38.542816 medit-0.0.4/medit/styles/external/thomasf-solarized-css/solarized-dark.css
+-rw-r--r--   0        0        0     4282 2023-07-02 11:33:38.542816 medit-0.0.4/medit/styles/external/thomasf-solarized-css/solarized-light.css
+-rwxr-xr-x   0        0        0     6985 2023-07-02 15:43:07.140557 medit-0.0.4/medit/ui.py
+-rw-r--r--   0        0        0     2389 2023-07-02 11:32:00.577590 medit-0.0.4/medit/utils.py
+-rw-r--r--   0        0        0     2315 2023-07-02 16:11:41.762127 medit-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3129 1970-01-01 00:00:00.000000 medit-0.0.4/PKG-INFO
```

### Comparing `medit-0.0.3/Readme.md` & `medit-0.0.4/Readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,49 +29,59 @@
 poetry build
 poetry run twine check dist/pocketrockit-0.0.25-py3-none-any.whl
 python3 -m pip install --user --upgrade dist/pocketrockit-0.0.25-py3-none-any.whl
 ```
 
 ## 1.0 TODO
 
+* [x] File to title
+* [x] File viewer for Plain, Python, YAML, JSON, ..
+* [x] Save
+* [ ] Preview for Markdown/.. only
+* [ ] Manage word wrap
+* [ ] Hightlight todo.txt
+* [ ] Notify external file changes
+* [ ] (Re-)store zoom and fullscreen
+* [ ] File ignore filter
+* [ ] Icon
+* [ ] Autoload
+* [ ] Proper Qt style
 * [ ] Show local images
 * [ ] Show remote images
-* [ ] File to title
-* [ ] proper Qt style
-* [ ] slim file / folder create / rename
-* [ ] proper View CSS selector
-* [ ] File viewer for Plain, Python, YAML, JSON, ..
-* [ ] Autoload
-* [ ] Save
+* [ ] Slim file / folder create / rename
+* [ ] Proper View CSS selector
 * [ ] View follows editor
 * [ ] Links clickable
 * [ ] Fix Links to support `(text)[url]` syntax
 
 
 ## Feature ideas
 
-* [ ] export to Pdf / Html / docx ..
-* [ ] copy / paste images
-* [ ] drag & drop images
-* [ ] spell checker
+* [ ] Export to Pdf / Html / docx ..
+* [ ] Copy / paste images
+* [ ] Drag & drop images
+* [ ] Spell checker
 
 
 ## Read
+* https://web.archive.org/web/20190604145031/https://qscintilla.com/prepare-image-hack/
+
+* https://github.com/sindresorhus/github-markdown-css
+* https://python-markdown.github.io/extensions/code_hilite/#step-1-download-and-install-pygments
+* https://github.com/richleland/pygments-css
+* https://github.com/OzakIOne/markdown-github-dark
+* https://github.com/jamiemcg/remarkable
+* https://github.com/sindresorhus/github-markdown-css
 
-https://github.com/sindresorhus/github-markdown-css
-https://python-markdown.github.io/extensions/code_hilite/#step-1-download-and-install-pygments
-https://github.com/richleland/pygments-css
-https://github.com/OzakIOne/markdown-github-dark
-https://github.com/jamiemcg/remarkable
-https://github.com/sindresorhus/github-markdown-css
+* https://thomasf.github.io/solarized-css/
+* https://thomasf.github.io/solarized-css/solarized-light.css
 
-https://thomasf.github.io/solarized-css/
-https://thomasf.github.io/solarized-css/solarized-light.css
+* https://markdowncss.github.io/
+* https://github.com/markdowncss/retro
 
-https://markdowncss.github.io/
-https://github.com/markdowncss/retro
+* https://mixu.net/markdown-styles/
 
-https://mixu.net/markdown-styles/
+* https://github.com/altercation/solarized
 
-https://github.com/altercation/solarized
+* https://www.jsdelivr.com/package/npm/@naokim03/markdown-theme-solarized
 
-https://www.jsdelivr.com/package/npm/@naokim03/markdown-theme-solarized
+* https://github.com/5yutan5/PyQtDarkTheme
```

### Comparing `medit-0.0.3/medit/cli.py` & `medit-0.0.4/medit/cli.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/medit.ui` & `medit-0.0.4/medit/medit.ui`

 * *Files 8% similar despite different names*

#### Comparing `medit-0.0.3/medit/medit.ui` & `medit-0.0.4/medit/medit.ui`

```diff
@@ -19,16 +19,25 @@
     <property name="windowTitle">
       <string>medit</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <layout class="QGridLayout" name="gridLayout">
         <item row="0" column="0" colspan="2">
           <layout class="QHBoxLayout" name="horizontalLayout">
+            <property name="leftMargin">
+              <number>0</number>
+            </property>
             <property name="topMargin">
-              <number>20</number>
+              <number>0</number>
+            </property>
+            <property name="rightMargin">
+              <number>0</number>
+            </property>
+            <property name="bottomMargin">
+              <number>0</number>
             </property>
             <item>
               <widget class="QSplitter" name="gb_splitter">
                 <property name="orientation">
                   <enum>Qt::Horizontal</enum>
                 </property>
                 <widget class="QTreeView" name="tv_files"/>
```

### Comparing `medit-0.0.3/medit/meditor.py` & `medit-0.0.4/medit/meditor.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/mview.py` & `medit-0.0.4/medit/mview.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,21 @@
         self.css_content_markdown = "".join(
             f"<style>{open(Path(__file__).parent / path).read()}</style>"
             for path in (
                 "styles/external/github-markdown-light.css",
                 "styles/external/thomasf-solarized-css/solarized-light.css",
                 "styles/external/solarized-light-all-sites.css",
                 "styles/external/pygments-solarized-style/solarized-light.css",
+
+                #"styles/external/github-markdown-dark.css",
+                #"styles/external/thomasf-solarized-css/solarized-dark.css",
+                #"styles/external/solarized-dark-all-sites.css",
+                #"styles/external/pygments-solarized-style/solarized-dark.css",
             ))
+
         self.css_content = "".join(
             f"<style>{open(Path(__file__).parent / path).read()}</style>"
             for path in (
                 "styles/external/pygments-solarized-style/solarized-light.css",
             ))
 
         self.css_content_unused = "".join(
```

### Comparing `medit-0.0.3/medit/styles/external/github-markdown-dark.css` & `medit-0.0.4/medit/styles/external/github-markdown-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/styles/external/github-markdown-light.css` & `medit-0.0.4/medit/styles/external/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/styles/external/pygments-solarized-style/solarized-dark.css` & `medit-0.0.4/medit/styles/external/pygments-solarized-style/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/styles/external/pygments-solarized-style/solarized-light.css` & `medit-0.0.4/medit/styles/external/pygments-solarized-style/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/styles/external/solarized-dark-all-sites.css` & `medit-0.0.4/medit/styles/external/solarized-dark-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/styles/external/solarized-light-all-sites.css` & `medit-0.0.4/medit/styles/external/solarized-light-all-sites.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/styles/external/thomasf-solarized-css/solarized-dark.css` & `medit-0.0.4/medit/styles/external/thomasf-solarized-css/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/styles/external/thomasf-solarized-css/solarized-light.css` & `medit-0.0.4/medit/styles/external/thomasf-solarized-css/solarized-light.css`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/ui.py` & `medit-0.0.4/medit/ui.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/medit/utils.py` & `medit-0.0.4/medit/utils.py`

 * *Files identical despite different names*

### Comparing `medit-0.0.3/pyproject.toml` & `medit-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "medit"
-version = "0.0.3"
+version = "0.0.4"
 description = "Markup Editor"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/medit.git"
 readme = "Readme.md"
 packages = [
   {include = "medit/**/*.py"},
   {include = "medit/**/*.ui"},
@@ -21,14 +21,15 @@
 pyqt6 = "^6.5.1"
 pyqt6-qscintilla = "^2.14.0"
 pyqt6-webengine = "^6.5.0"
 markdown = "^3.4.3"
 markdown-checklist = "^0.4.4"
 # pygments-solarized-style = "^0.1"
 pyqtdarktheme = "^2.1.0"
+pygments = "^2.15.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
```

### Comparing `medit-0.0.3/PKG-INFO` & `medit-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: medit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Markup Editor
 Home-page: https://projects.om-office.de/frans/medit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncinotify (>=4.0.1,<5.0.0)
 Requires-Dist: markdown (>=3.4.3,<4.0.0)
 Requires-Dist: markdown-checklist (>=0.4.4,<0.5.0)
+Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: pyqt6 (>=6.5.1,<7.0.0)
 Requires-Dist: pyqt6-qscintilla (>=2.14.0,<3.0.0)
 Requires-Dist: pyqt6-webengine (>=6.5.0,<7.0.0)
 Requires-Dist: pyqtdarktheme (>=2.1.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://projects.om-office.de/frans/medit.git
 Description-Content-Type: text/markdown
@@ -52,49 +53,60 @@
 poetry build
 poetry run twine check dist/pocketrockit-0.0.25-py3-none-any.whl
 python3 -m pip install --user --upgrade dist/pocketrockit-0.0.25-py3-none-any.whl
 ```
 
 ## 1.0 TODO
 
+* [x] File to title
+* [x] File viewer for Plain, Python, YAML, JSON, ..
+* [x] Save
+* [ ] Preview for Markdown/.. only
+* [ ] Manage word wrap
+* [ ] Hightlight todo.txt
+* [ ] Notify external file changes
+* [ ] (Re-)store zoom and fullscreen
+* [ ] File ignore filter
+* [ ] Icon
+* [ ] Autoload
+* [ ] Proper Qt style
 * [ ] Show local images
 * [ ] Show remote images
-* [ ] File to title
-* [ ] proper Qt style
-* [ ] slim file / folder create / rename
-* [ ] proper View CSS selector
-* [ ] File viewer for Plain, Python, YAML, JSON, ..
-* [ ] Autoload
-* [ ] Save
+* [ ] Slim file / folder create / rename
+* [ ] Proper View CSS selector
 * [ ] View follows editor
 * [ ] Links clickable
 * [ ] Fix Links to support `(text)[url]` syntax
 
 
 ## Feature ideas
 
-* [ ] export to Pdf / Html / docx ..
-* [ ] copy / paste images
-* [ ] drag & drop images
-* [ ] spell checker
+* [ ] Export to Pdf / Html / docx ..
+* [ ] Copy / paste images
+* [ ] Drag & drop images
+* [ ] Spell checker
 
 
 ## Read
+* https://web.archive.org/web/20190604145031/https://qscintilla.com/prepare-image-hack/
+
+* https://github.com/sindresorhus/github-markdown-css
+* https://python-markdown.github.io/extensions/code_hilite/#step-1-download-and-install-pygments
+* https://github.com/richleland/pygments-css
+* https://github.com/OzakIOne/markdown-github-dark
+* https://github.com/jamiemcg/remarkable
+* https://github.com/sindresorhus/github-markdown-css
+
+* https://thomasf.github.io/solarized-css/
+* https://thomasf.github.io/solarized-css/solarized-light.css
 
-https://github.com/sindresorhus/github-markdown-css
-https://python-markdown.github.io/extensions/code_hilite/#step-1-download-and-install-pygments
-https://github.com/richleland/pygments-css
-https://github.com/OzakIOne/markdown-github-dark
-https://github.com/jamiemcg/remarkable
-https://github.com/sindresorhus/github-markdown-css
+* https://markdowncss.github.io/
+* https://github.com/markdowncss/retro
 
-https://thomasf.github.io/solarized-css/
-https://thomasf.github.io/solarized-css/solarized-light.css
+* https://mixu.net/markdown-styles/
 
-https://markdowncss.github.io/
-https://github.com/markdowncss/retro
+* https://github.com/altercation/solarized
 
-https://mixu.net/markdown-styles/
+* https://www.jsdelivr.com/package/npm/@naokim03/markdown-theme-solarized
 
-https://github.com/altercation/solarized
+* https://github.com/5yutan5/PyQtDarkTheme
 
-https://www.jsdelivr.com/package/npm/@naokim03/markdown-theme-solarized
```

