# Comparing `tmp/jupyterlab_celltagsclasses-0.3.0.tar.gz` & `tmp/jupyterlab_celltagsclasses-0.3.1.tar.gz`

## Comparing `jupyterlab_celltagsclasses-0.3.0.tar` & `jupyterlab_celltagsclasses-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.editorconfig
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.eslintignore
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.eslintrc.js
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.gitattributes
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.prettierignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/RELEASE.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/install.json
--rw-r--r--   0        0        0   164226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/package-lock.json
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/package.json
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/package.json.version
--rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/release-to-pypi.sh
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/tsconfig.json
--rw-r--r--   0        0        0   208738 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/yarn.lock
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/examples/test.ipynb
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/_version.py
--rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/build_log.json
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/package.json
--rw-r--r--   0        0        0    25055 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js
--rw-r--r--   0        0        0    23941 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map
--rw-r--r--   0        0        0    27701 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js
--rw-r--r--   0        0        0    26608 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style.js
--rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js
--rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map
--rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/media/screenshot.png
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/apply_on_cells.ts
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/index.ts
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/metadata.ts
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/xpath-test.js
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/xpath-test.ts
--rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/xpath.js
--rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/src/xpath.ts
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/style/index.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/style/index.js
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/LICENSE
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/README.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.editorconfig
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.eslintignore
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.eslintrc.js
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.gitattributes
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.prettierignore
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/RELEASE.md
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/install.json
+-rw-r--r--   0        0        0   164226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/package-lock.json
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/package.json
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/package.json.version
+-rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/release-to-pypi.sh
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/tsconfig.json
+-rw-r--r--   0        0        0   208738 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/yarn.lock
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/examples/test.ipynb
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/_version.py
+-rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/build_log.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/install.json
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/package.json
+-rw-r--r--   0        0        0    25055 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js
+-rw-r--r--   0        0        0    23941 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map
+-rw-r--r--   0        0        0    27701 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js
+-rw-r--r--   0        0        0    26608 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style.js
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js
+-rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map
+-rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/media/screenshot.png
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/apply_on_cells.ts
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/index.ts
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/metadata.ts
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/xpath-test.js
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/xpath-test.ts
+-rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/xpath.js
+-rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/xpath.ts
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/style/index.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/style/index.js
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/README.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/PKG-INFO
```

### Comparing `jupyterlab_celltagsclasses-0.3.0/.eslintrc.js` & `jupyterlab_celltagsclasses-0.3.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/RELEASE.md` & `jupyterlab_celltagsclasses-0.3.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/package-lock.json` & `jupyterlab_celltagsclasses-0.3.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/package.json` & `jupyterlab_celltagsclasses-0.3.1/package.json.version`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/package.json.version` & `jupyterlab_celltagsclasses-0.3.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.3.1'"}*

```diff
@@ -90,9 +90,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.3.0"
+    "version": "0.3.1"
 }
```

### Comparing `jupyterlab_celltagsclasses-0.3.0/release-to-pypi.sh` & `jupyterlab_celltagsclasses-0.3.1/release-to-pypi.sh`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/bin/bash
 
+echo "checking for required python packages"
+for pkg in build twine hatch; do
+    pip show $pkg >& /dev/null || pip install $pkg
+done
+
 echo "Current version is: $(hatch version)"
 
 # prompt user for version number
 echo "Enter new version number: "
 read version
 
-echo "checking for required python packages"
-for pkg in build twine hatch; do
-    pip show $pkg >& /dev/null || pip install $pkg
-done
-
 # hatch has the nasty effect of reformatting package.json
 #hatch version $version
 echo "bumping version to $version"
 sed -i.version -e 's/\("version": "\)[^"]*/\1'$version'/' package.json
 
 echo "diffing package.json"
 git diff package.json
```

### Comparing `jupyterlab_celltagsclasses-0.3.0/tsconfig.json` & `jupyterlab_celltagsclasses-0.3.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/yarn.lock` & `jupyterlab_celltagsclasses-0.3.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/examples/test.ipynb` & `jupyterlab_celltagsclasses-0.3.1/examples/test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/build_log.json` & `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/package.json` & `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js` & `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map` & `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js` & `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map` & `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js` & `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map` & `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/media/screenshot.png` & `jupyterlab_celltagsclasses-0.3.1/media/screenshot.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/src/apply_on_cells.ts` & `jupyterlab_celltagsclasses-0.3.1/src/apply_on_cells.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/src/index.ts` & `jupyterlab_celltagsclasses-0.3.1/src/index.ts`

 * *Files 3% similar despite different names*

```diff
@@ -80,23 +80,23 @@
                 })
                 removedTags.forEach(tag => {
                   console.debug(`removing class for tag ${class_for_tag(tag)}`)
                   cellWidget.removeClass(class_for_tag(tag))
                 })
               })
             } else if (change.type === 'add') {
-              console.log('add', change, change.newValue)
+              console.debug('celltagsclasses: add', change, change.newValue)
               cellWidgets.forEach(cellWidget => {
                 for (const tag of change.newValue) {
                   // console.debug(`adding class for tag ${class_for_tag(tag)}`)
                   cellWidget.addClass(class_for_tag(tag))
                 }
               })
             } else if (change.type === 'remove') {
-              console.log('remove', change, change.newValue)
+              console.debug('celltagsclasses: remove', change, change.newValue)
               cellWidgets.forEach(cellWidget => {
                 for (const tag of change.newValue) {
                   // console.debug(`removing class for tag ${class_for_tag(tag)}`)
                   cellWidget.removeClass(class_for_tag(tag))
                 }
               })
             }
```

### Comparing `jupyterlab_celltagsclasses-0.3.0/src/metadata.ts` & `jupyterlab_celltagsclasses-0.3.1/src/metadata.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/src/xpath-test.js` & `jupyterlab_celltagsclasses-0.3.1/src/xpath-test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/src/xpath-test.ts` & `jupyterlab_celltagsclasses-0.3.1/src/xpath-test.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/src/xpath.js` & `jupyterlab_celltagsclasses-0.3.1/src/xpath.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/src/xpath.ts` & `jupyterlab_celltagsclasses-0.3.1/src/xpath.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/style/base.css` & `jupyterlab_celltagsclasses-0.3.1/style/base.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 /*
     See the JupyterLab Developer Guide for useful CSS Patterns:
 
     https://jupyterlab.readthedocs.io/en/stable/developer/css.html
 */
 
-/* hide only the input of cells with the tag 'hide-input' */
 .cell-tag-celltagsclasses-test1 {
   padding: 10px;
   border: 2.5px black solid;
   border-radius: 10px;
 
   /* could be overridden if cell is active */
   background-color: yellow !important;
```

### Comparing `jupyterlab_celltagsclasses-0.3.0/.gitignore` & `jupyterlab_celltagsclasses-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/LICENSE` & `jupyterlab_celltagsclasses-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/README.md` & `jupyterlab_celltagsclasses-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/pyproject.toml` & `jupyterlab_celltagsclasses-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.0/PKG-INFO` & `jupyterlab_celltagsclasses-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_celltagsclasses
-Version: 0.3.0
+Version: 0.3.1
 Summary: JLAB extension to add classes to cells based on their tags
 Project-URL: Homepage, https://github.com/parmentelat/jupyterlab-celltagsclasses
 Project-URL: Bug Tracker, https://github.com/parmentelat/jupyterlab-celltagsclasses/issues
 Project-URL: Repository, https://github.com/parmentelat/jupyterlab-celltagsclasses.git
 Author-email: Thierry Parmentelat <thierry.parmentelat@inria.fr>
 License: BSD 3-Clause License
```

