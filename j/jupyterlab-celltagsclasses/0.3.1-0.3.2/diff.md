# Comparing `tmp/jupyterlab_celltagsclasses-0.3.1.tar.gz` & `tmp/jupyterlab_celltagsclasses-0.3.2.tar.gz`

## Comparing `jupyterlab_celltagsclasses-0.3.1.tar` & `jupyterlab_celltagsclasses-0.3.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.editorconfig
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.eslintignore
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.eslintrc.js
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.gitattributes
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.prettierignore
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.stylelintrc
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/RELEASE.md
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/install.json
--rw-r--r--   0        0        0   164226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/package-lock.json
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/package.json
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/package.json.version
--rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/release-to-pypi.sh
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/tsconfig.json
--rw-r--r--   0        0        0   208738 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/yarn.lock
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/examples/test.ipynb
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/_version.py
--rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/build_log.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/install.json
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/package.json
--rw-r--r--   0        0        0    25055 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js
--rw-r--r--   0        0        0    23941 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map
--rw-r--r--   0        0        0    27701 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js
--rw-r--r--   0        0        0    26608 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style.js
--rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js
--rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map
--rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/media/screenshot.png
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/apply_on_cells.ts
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/index.ts
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/metadata.ts
--rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/xpath-test.js
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/xpath-test.ts
--rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/xpath.js
--rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/src/xpath.ts
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/style/index.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/style/index.js
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/.gitignore
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/LICENSE
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/README.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/.editorconfig
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/.eslintignore
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/.eslintrc.js
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/.gitattributes
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/.prettierignore
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/.stylelintrc
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/.yarnrc.yml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/RELEASE.md
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/install.json
+-rw-r--r--   0        0        0   164226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/package-lock.json
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/package.json
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/package.json.version
+-rwxr-xr-x   0        0        0      813 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/release-to-pypi.sh
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/tsconfig.json
+-rw-r--r--   0        0        0   208738 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/yarn.lock
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/examples/test.ipynb
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/_version.py
+-rw-r--r--   0        0        0    21236 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/build_log.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/install.json
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/package.json
+-rw-r--r--   0        0        0    25055 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js
+-rw-r--r--   0        0        0    23941 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map
+-rw-r--r--   0        0        0    27701 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js
+-rw-r--r--   0        0        0    26608 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/style.js
+-rw-r--r--   0        0        0    20494 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js
+-rw-r--r--   0        0        0    16237 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map
+-rw-r--r--   0        0        0    54944 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/media/screenshot.png
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/src/apply_on_cells.ts
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/src/index.ts
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/src/metadata.ts
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/src/xpath-test.js
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/src/xpath-test.ts
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/src/xpath.js
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/src/xpath.ts
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/style/index.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/style/index.js
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/README.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 jupyterlab_celltagsclasses-0.3.2/PKG-INFO
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/.eslintrc.js` & `jupyterlab_celltagsclasses-0.3.2/.eslintrc.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,42 +1,42 @@
 module.exports = {
     extends: [
         'eslint:recommended',
         'plugin:@typescript-eslint/eslint-recommended',
         'plugin:@typescript-eslint/recommended',
-        'plugin:prettier/recommended'
+        'plugin:prettier/recommended',
     ],
     parser: '@typescript-eslint/parser',
     parserOptions: {
         project: 'tsconfig.json',
-        sourceType: 'module'
+        sourceType: 'module',
     },
     plugins: ['@typescript-eslint'],
     rules: {
         '@typescript-eslint/naming-convention': [
             'error', {
                 selector: 'interface',
                 format: ['PascalCase'],
                 custom: {
                     regex: '^I[A-Z]',
-                    match: true
-                }
-            }
+                    match: true,
+                },
+            },
         ],
         '@typescript-eslint/no-unused-vars': ['warn', {
             args: 'none'
         }],
         '@typescript-eslint/no-explicit-any': 'off',
         '@typescript-eslint/no-namespace': 'off',
         '@typescript-eslint/no-use-before-define': 'off',
         '@typescript-eslint/quotes': [
             'error',
             'single', {
                 avoidEscape: true,
                 allowTemplateLiterals: false
-            }
+            },
         ],
         curly: ['error', 'all'],
         eqeqeq: 'error',
-        'prefer-arrow-callback': 'error'
-    }
+        'prefer-arrow-callback': 'error',
+    },
 }
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/RELEASE.md` & `jupyterlab_celltagsclasses-0.3.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/package-lock.json` & `jupyterlab_celltagsclasses-0.3.2/package-lock.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/package.json` & `jupyterlab_celltagsclasses-0.3.2/package.json.version`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/package.json.version` & `jupyterlab_celltagsclasses-0.3.2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'0.3.2'"}*

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
+    "version": "0.3.2"
 }
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/release-to-pypi.sh` & `jupyterlab_celltagsclasses-0.3.2/release-to-pypi.sh`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/tsconfig.json` & `jupyterlab_celltagsclasses-0.3.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/yarn.lock` & `jupyterlab_celltagsclasses-0.3.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/examples/test.ipynb` & `jupyterlab_celltagsclasses-0.3.2/examples/test.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/build_log.json` & `jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/package.json` & `jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js` & `jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map` & `jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/lib_index_js.8b68da7de22fb270ee0f.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js` & `jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map` & `jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/remoteEntry.8de4dac15b9641f8640c.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js` & `jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map` & `jupyterlab_celltagsclasses-0.3.2/jupyterlab_celltagsclasses/labextension/static/style_index_js.4784725fff15b54ffe3d.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/media/screenshot.png` & `jupyterlab_celltagsclasses-0.3.2/media/screenshot.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/src/apply_on_cells.ts` & `jupyterlab_celltagsclasses-0.3.2/src/apply_on_cells.ts`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 /*
  * the logic of applying a function on a set of cells
  */
 
 /* eslint-disable prettier/prettier */
-import { INotebookTracker, } from '@jupyterlab/notebook'
-
-import { Cell, } from '@jupyterlab/cells'
+import { INotebookTracker } from '@jupyterlab/notebook'
 
+import { Cell } from '@jupyterlab/cells'
 
 export enum Scope {
-  All,        // run on all cells
-  Active,     // the active cell only
-  Multiple,   // the multiple selected if that is the case, the active cell otherwise
+  All, // run on all cells
+  Active, // the active cell only
+  Multiple, // the multiple selected if that is the case, the active cell otherwise
 }
 
 export const apply_on_cells = (
   notebookTracker: INotebookTracker,
   scope: Scope,
   to_apply: (cell: Cell) => void,
 ) => {
   const notebook = notebookTracker.currentWidget?.content
-  if (notebook === undefined) { return }
+  if (notebook === undefined) {
+    return
+  }
 
   let actionCells
   if (scope === Scope.All) {
     actionCells = notebook.widgets.slice()
   } else {
     const activeCell = notebook.activeCell
-    if (activeCell === null) { return }
+    if (activeCell === null) {
+      return
+    }
 
     if (scope === Scope.Active) {
       actionCells = [activeCell]
     } else {
       const { anchor, head } = notebook.getContiguousSelection()
       // when only one cell is selected/active, both are null
       if (anchor === null || head === null) {
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/src/index.ts` & `jupyterlab_celltagsclasses-0.3.2/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -33,28 +33,28 @@
         if (change.type !== 'add') {
           return
         }
         change.newValues.forEach(cellModel => {
           // compute widgets attached to cellModel
           const cellWidgets =
             notebookTracker.currentWidget?.content.widgets.filter(
-              (cell: Cell, index: number) => cell.model.id === cellModel.id
+              (cell: Cell, index: number) => cell.model.id === cellModel.id,
             )
           if (cellWidgets === undefined || cellWidgets?.length === 0) {
             // console.warn('could not find cell widget for cell model', cellModel)
             return
           }
           // console.debug( `found ${cellWidgets?.length} cell widgets`, cellWidgets[0] )
 
           // add classes for pre-existing tags
           cellModel.getMetadata('tags')?.forEach((tag: string) =>
             cellWidgets?.forEach(cellWidget => {
               // console.debug( `adding initial class for tag ${class_for_tag(tag)}` )
               cellWidget.addClass(class_for_tag(tag))
-            })
+            }),
           )
 
           // react to changes in tags
           cellModel.metadataChanged.connect((sender: ICellModel, change) => {
             // console.debug('metadata changed', sender, change)
             if (change.key !== 'tags') {
               // console.debug("ignoring non-tags metadata change")
@@ -100,16 +100,25 @@
                 }
               })
             }
           })
         })
       })
     })
-  }
+  },
 }
 
 export default plugin
 
 // re-export metadata helper functions
-export { md_get, md_set, md_unset, md_has, md_insert, md_remove, md_toggle, md_clean } from './metadata'
+export {
+  md_get,
+  md_set,
+  md_unset,
+  md_has,
+  md_insert,
+  md_remove,
+  md_toggle,
+  md_clean,
+} from './metadata'
 
 export { Scope, apply_on_cells } from './apply_on_cells'
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/src/metadata.ts` & `jupyterlab_celltagsclasses-0.3.2/src/metadata.ts`

 * *Files 3% similar despite different names*

```diff
@@ -29,26 +29,35 @@
 // clean up
 // (*) md_clean: remove empty metadata elements
 //         e.g. md_clean(cell, "path.to.subtree")
 //         or more typically
 //              md_clean(cell, "")
 //          will alter the cell's metadata so as to remove empty lists or empty keys
 
-
 import { ICellModel, Cell } from '@jupyterlab/cells'
 
 import {
-  XpathMap, Xpath, normalize,
-  xpath_get, xpath_set, xpath_unset, xpath_insert, xpath_remove, xpath_clean
+  XpathMap,
+  Xpath,
+  normalize,
+  xpath_get,
+  xpath_set,
+  xpath_unset,
+  xpath_insert,
+  xpath_remove,
+  xpath_clean,
 } from './xpath'
 
-
 // atomic values
 
-export const md_get = (cell: Cell | ICellModel, xpath: Xpath, if_missing?: any): any => {
+export const md_get = (
+  cell: Cell | ICellModel,
+  xpath: Xpath,
+  if_missing?: any,
+): any => {
   if (cell instanceof Cell) {
     cell = cell.model
   }
   xpath = normalize(xpath)
   const [first, ...tail] = xpath
 
   const start = cell.getMetadata(first)
@@ -86,15 +95,14 @@
   } else {
     const retcod = xpath_unset(start as XpathMap, tail)
     cell.model.setMetadata(first, start)
     return retcod
   }
 }
 
-
 // lists (e.g. tags)
 
 export const md_has = (cell: Cell, xpath: Xpath, key: string) => {
   xpath = normalize(xpath)
   const [first, ...tail] = xpath
   const start = cell.model.getMetadata(first)
   if (start === undefined) {
@@ -109,15 +117,15 @@
 
 export const md_insert = (cell: Cell, xpath: Xpath, key: string) => {
   xpath = normalize(xpath)
   const [first, ...tail] = xpath
 
   const start = cell.model.getMetadata(first)
   if (tail.length === 0) {
-    let sublist : Array<string>
+    let sublist: Array<string>
     if (start !== undefined) {
       sublist = start as Array<string>
       // use another object as otherwise .setMetadata() does not seem to propagate
       sublist = sublist.slice()
     } else {
       sublist = []
     }
@@ -132,15 +140,15 @@
     const subtree = start || {}
     const retcod = xpath_insert(subtree as XpathMap, tail, key)
     cell.model.setMetadata(first, subtree)
     return retcod
   }
 }
 
-export const md_remove = (cell: Cell, xpath: Xpath, key:string) => {
+export const md_remove = (cell: Cell, xpath: Xpath, key: string) => {
   xpath = normalize(xpath)
   const [first, ...tail] = xpath
   const start = cell.model.getMetadata(first)
   if (start === undefined) {
     return undefined
   }
   if (tail.length === 0) {
@@ -164,40 +172,39 @@
     cell.model.setMetadata(first, subtree)
     return retcod
   }
 }
 
 export const md_toggle = (cell: Cell, xpath: Xpath, key: string) => {
   xpath = normalize(xpath)
-  if ( ! md_has(cell, xpath, key)) {
+  if (!md_has(cell, xpath, key)) {
     return md_insert(cell, xpath, key)
   } else {
     return md_remove(cell, xpath, key)
   }
 }
 
-
-export const md_clean = (cell:Cell, xpath: Xpath) => {
+export const md_clean = (cell: Cell, xpath: Xpath) => {
   xpath = normalize(xpath)
   const [first, ...tail] = xpath
   if (first === undefined) {
     console.log(cell.model.metadata)
     // no xpath, clean the whole metadata
     for (const key of Object.entries(cell.model.metadata)) {
       const xpath = key as Xpath
-      const new_value = xpath_clean(md_get(cell, xpath), "")
-      if ((new_value === undefined) || (new_value.length === 0)) {
+      const new_value = xpath_clean(md_get(cell, xpath), '')
+      if (new_value === undefined || new_value.length === 0) {
         md_unset(cell, xpath)
       } else {
         md_set(cell, xpath, new_value)
       }
     }
   } else {
     const subtree = md_get(cell, first)
     const new_value = xpath_clean(subtree, tail)
-    if ((new_value === undefined) || (new_value.length === 0)) {
+    if (new_value === undefined || new_value.length === 0) {
       md_unset(cell, first)
     } else {
       md_set(cell, first, new_value)
     }
   }
 }
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/src/xpath-test.js` & `jupyterlab_celltagsclasses-0.3.2/src/xpath-test.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,100 +1,163 @@
-"use strict";
+'use strict'
 /* eslint-disable prettier/prettier */
-Object.defineProperty(exports, "__esModule", {
+Object.defineProperty(exports, '__esModule', {
     value: true
-});
-var xpath_1 = require("./xpath");
+})
+var xpath_1 = require('./xpath')
 /* not guaranteed to work by side-effects only */
-var md = {};
+var md = {}
 // uncomment to debug
 var checkpoint = function(md, message) {
     // console.log('------', message, '\n', JSON.stringify(md))
-    message;
-};
-console.assert((0, xpath_1.xpath_get)(md, 'simple') === undefined, '001');
-console.assert((0, xpath_1.xpath_set)(md, 'simple', 1) === 1, '002');
-console.assert((0, xpath_1.xpath_get)(md, 'simple') === 1, '003');
-checkpoint(md, "should have 'simple' set to 1");
+    message
+}
+console.assert((0, xpath_1.xpath_get)(md, 'simple') === undefined, '001')
+console.assert((0, xpath_1.xpath_set)(md, 'simple', 1) === 1, '002')
+console.assert((0, xpath_1.xpath_get)(md, 'simple') === 1, '003')
+checkpoint(md, "should have 'simple' set to 1")
 // first time OK
-console.assert((0, xpath_1.xpath_unset)(md, 'simple') === true, '011');
+console.assert((0, xpath_1.xpath_unset)(md, 'simple') === true, '011')
 // then KO
-console.assert((0, xpath_1.xpath_unset)(md, 'simple') === false, '012');
-console.assert((0, xpath_1.xpath_get)(md, 'simple') === undefined, '013');
-console.assert((0, xpath_1.xpath_set)(md, 'simple', 1) === 1, '014');
-checkpoint(md, 'same');
-console.assert((0, xpath_1.xpath_get)(md, 'nested.under') === undefined, '021');
-console.assert((0, xpath_1.xpath_set)(md, 'nested.under', 2) === 2, '022');
-console.assert((0, xpath_1.xpath_get)(md, 'nested.under') === 2, '023');
-console.assert((0, xpath_1.xpath_unset)(md, 'nested.under') === true, '024');
-console.assert((0, xpath_1.xpath_get)(md, 'nested.under') === undefined, '025');
-console.assert((0, xpath_1.xpath_unset)(md, 'nested.under') === false, '026');
-console.assert(JSON.stringify((0, xpath_1.xpath_get)(md, 'nested')) === '{}', '027');
-console.assert((0, xpath_1.xpath_set)(md, 'nested.under', 2) === 2, '028');
-checkpoint(md, "should have 'nested.under' set to 2");
-console.assert((0, xpath_1.xpath_get)(md, 'jupyter') === undefined, '031');
-console.assert((0, xpath_1.xpath_get)(md, 'jupyter.source_hidden') === undefined, '032');
-console.assert((0, xpath_1.xpath_get)(md, ['jupyter', 'source_hidden']) === undefined, '033');
-console.assert((0, xpath_1.xpath_set)(md, 'jupyter.source_hidden', true) === true, '034');
-console.assert((0, xpath_1.xpath_get)(md, ['jupyter', 'source_hidden']) === true, '035');
-console.assert((0, xpath_1.xpath_get)(md, 'jupyter.source_hidden') === true, '036');
-checkpoint(md, 'jupyter.source_hidden=true');
+console.assert((0, xpath_1.xpath_unset)(md, 'simple') === false, '012')
+console.assert((0, xpath_1.xpath_get)(md, 'simple') === undefined, '013')
+console.assert((0, xpath_1.xpath_set)(md, 'simple', 1) === 1, '014')
+checkpoint(md, 'same')
+console.assert((0, xpath_1.xpath_get)(md, 'nested.under') === undefined, '021')
+console.assert((0, xpath_1.xpath_set)(md, 'nested.under', 2) === 2, '022')
+console.assert((0, xpath_1.xpath_get)(md, 'nested.under') === 2, '023')
+console.assert((0, xpath_1.xpath_unset)(md, 'nested.under') === true, '024')
+console.assert((0, xpath_1.xpath_get)(md, 'nested.under') === undefined, '025')
+console.assert((0, xpath_1.xpath_unset)(md, 'nested.under') === false, '026')
+console.assert(
+    JSON.stringify((0, xpath_1.xpath_get)(md, 'nested')) === '{}',
+    '027',
+)
+console.assert((0, xpath_1.xpath_set)(md, 'nested.under', 2) === 2, '028')
+checkpoint(md, "should have 'nested.under' set to 2")
+console.assert((0, xpath_1.xpath_get)(md, 'jupyter') === undefined, '031')
+console.assert(
+    (0, xpath_1.xpath_get)(md, 'jupyter.source_hidden') === undefined,
+    '032',
+)
+console.assert(
+    (0, xpath_1.xpath_get)(md, ['jupyter', 'source_hidden']) === undefined,
+    '033',
+)
+console.assert(
+    (0, xpath_1.xpath_set)(md, 'jupyter.source_hidden', true) === true,
+    '034',
+)
+console.assert(
+    (0, xpath_1.xpath_get)(md, ['jupyter', 'source_hidden']) === true,
+    '035',
+)
+console.assert(
+    (0, xpath_1.xpath_get)(md, 'jupyter.source_hidden') === true,
+    '036',
+)
+checkpoint(md, 'jupyter.source_hidden=true')
 // cannot insert in pre-existing non-array
-console.assert((0, xpath_1.xpath_insert)(md, 'jupyter', 'anything') === undefined, '041');
-console.assert((0, xpath_1.xpath_insert)(md, 'jupyter.source_hidden', 'anything') === undefined, '042');
-checkpoint(md, 'same');
-console.assert((0, xpath_1.xpath_get)(md, 'tags.hide-input') === undefined, '051');
+console.assert(
+    (0, xpath_1.xpath_insert)(md, 'jupyter', 'anything') === undefined,
+    '041',
+)
+console.assert(
+    (0, xpath_1.xpath_insert)(md, 'jupyter.source_hidden', 'anything') ===
+    undefined,
+    '042',
+)
+checkpoint(md, 'same')
+console.assert(
+    (0, xpath_1.xpath_get)(md, 'tags.hide-input') === undefined,
+    '051',
+)
 // first time ok
-console.assert((0, xpath_1.xpath_insert)(md, 'tags', 'hide-input') === 'hide-input', '052');
+console.assert(
+    (0, xpath_1.xpath_insert)(md, 'tags', 'hide-input') === 'hide-input',
+    '052',
+)
 // then ko
-console.assert((0, xpath_1.xpath_insert)(md, 'tags', 'hide-input') === undefined, '053');
-console.assert((0, xpath_1.xpath_insert)(md, 'tags', 'foo') === 'foo', '054');
-var fetch = (0, xpath_1.xpath_get)(md, 'tags');
-console.assert(fetch instanceof Array, '055');
-console.assert(fetch.length === 2, '056');
-checkpoint(md, 'with 2 tags hide-input and foo');
-console.assert((0, xpath_1.xpath_remove)(md, 'tags', 'foo') === 'foo', '061');
-fetch = (0, xpath_1.xpath_get)(md, 'tags');
-console.assert(fetch instanceof Array, '062');
-console.assert(fetch.length === 1, '063');
-checkpoint(md, 'foo removed from the tags');
-console.assert((0, xpath_1.xpath_get)(md, 'hide_input') === undefined, '071');
-console.assert((0, xpath_1.xpath_set)(md, 'hide_input', true) === true, '072');
-console.assert((0, xpath_1.xpath_set)(md, 'hide_input', false) === false, '072-bis');
-console.assert((0, xpath_1.xpath_unset)(md, 'hide_input') === true, '073');
-console.assert((0, xpath_1.xpath_get)(md, 'hide_input') === undefined, '074');
-checkpoint(md, 'unchanged');
-var xpaths = ['empty-list', 'nested.empty-list'];
+console.assert(
+    (0, xpath_1.xpath_insert)(md, 'tags', 'hide-input') === undefined,
+    '053',
+)
+console.assert((0, xpath_1.xpath_insert)(md, 'tags', 'foo') === 'foo', '054')
+var fetch = (0, xpath_1.xpath_get)(md, 'tags')
+console.assert(fetch instanceof Array, '055')
+console.assert(fetch.length === 2, '056')
+checkpoint(md, 'with 2 tags hide-input and foo')
+console.assert((0, xpath_1.xpath_remove)(md, 'tags', 'foo') === 'foo', '061')
+fetch = (0, xpath_1.xpath_get)(md, 'tags')
+console.assert(fetch instanceof Array, '062')
+console.assert(fetch.length === 1, '063')
+checkpoint(md, 'foo removed from the tags')
+console.assert((0, xpath_1.xpath_get)(md, 'hide_input') === undefined, '071')
+console.assert((0, xpath_1.xpath_set)(md, 'hide_input', true) === true, '072')
+console.assert(
+    (0, xpath_1.xpath_set)(md, 'hide_input', false) === false,
+    '072-bis',
+)
+console.assert((0, xpath_1.xpath_unset)(md, 'hide_input') === true, '073')
+console.assert((0, xpath_1.xpath_get)(md, 'hide_input') === undefined, '074')
+checkpoint(md, 'unchanged')
+var xpaths = ['empty-list', 'nested.empty-list']
 for (var _i = 0, xpaths_1 = xpaths; _i < xpaths_1.length; _i++) {
-    var xpath = xpaths_1[_i];
-    console.assert((0, xpath_1.xpath_insert)(md, xpath, 'foo') === 'foo', '081');
-    console.assert((0, xpath_1.xpath_insert)(md, xpath, 'bar') === 'bar', '082');
-    console.assert((0, xpath_1.xpath_remove)(md, xpath, 'foo') === 'foo', '083');
-    console.assert((0, xpath_1.xpath_remove)(md, xpath, 'bar') === 'bar', '084');
-    md = (0, xpath_1.xpath_clean)(md, '');
-    console.assert((0, xpath_1.xpath_get)(md, xpath) === undefined, '085');
-    checkpoint(md, "unchanged after inserting/cleaning in ".concat(xpath));
+    var xpath = xpaths_1[_i]
+    console.assert((0, xpath_1.xpath_insert)(md, xpath, 'foo') === 'foo', '081')
+    console.assert((0, xpath_1.xpath_insert)(md, xpath, 'bar') === 'bar', '082')
+    console.assert((0, xpath_1.xpath_remove)(md, xpath, 'foo') === 'foo', '083')
+    console.assert((0, xpath_1.xpath_remove)(md, xpath, 'bar') === 'bar', '084')
+    md = (0, xpath_1.xpath_clean)(md, '')
+    console.assert((0, xpath_1.xpath_get)(md, xpath) === undefined, '085')
+    checkpoint(md, 'unchanged after inserting/cleaning in '.concat(xpath))
 }
 ////////////////////////////////////////
 var md2 = {
-    'cells': [],
-    'metadata': {
-        'kernelspec': {},
-        'language_info': [],
+    cells: [],
+    metadata: {
+        kernelspec: {},
+        language_info: [],
     },
-};
-console.assert(JSON.stringify((0, xpath_1.xpath_clean)(md2, '')) === "{}", '091');
-console.assert(JSON.stringify((0, xpath_1.xpath_clean)(md2, 'cells')) === "[]", '092');
-console.assert(JSON.stringify((0, xpath_1.xpath_clean)(md2, 'metadata')) === "{}", '093');
-console.assert(JSON.stringify((0, xpath_1.xpath_clean)(md2, 'metadata.kernelspec')) === '{"cells":[],"metadata":{}}', '094');
+}
+console.assert(
+    JSON.stringify((0, xpath_1.xpath_clean)(md2, '')) === '{}',
+    '091',
+)
+console.assert(
+    JSON.stringify((0, xpath_1.xpath_clean)(md2, 'cells')) === '[]',
+    '092',
+)
+console.assert(
+    JSON.stringify((0, xpath_1.xpath_clean)(md2, 'metadata')) === '{}',
+    '093',
+)
+console.assert(
+    JSON.stringify((0, xpath_1.xpath_clean)(md2, 'metadata.kernelspec')) ===
+    '{"cells":[],"metadata":{}}',
+    '094',
+)
 var md3 = {
     'empty-string': '',
-    'metadata': {
-        'kernelspec': {},
-        'language_info': [],
-        'empty-string': "",
+    metadata: {
+        kernelspec: {},
+        language_info: [],
+        'empty-string': '',
     },
-};
-console.assert(JSON.stringify((0, xpath_1.xpath_clean)(md3, '')) === "{}", '101');
-console.assert(JSON.stringify((0, xpath_1.xpath_clean)(md3, 'empty-string')) === '""', '102');
-console.assert(JSON.stringify((0, xpath_1.xpath_clean)(md3, 'metadata')) === "{}", '103');
-console.assert(JSON.stringify((0, xpath_1.xpath_clean)(md3, 'metadata.kernelspec')) === '{"empty-string":"","metadata":{}}', '104');
+}
+console.assert(
+    JSON.stringify((0, xpath_1.xpath_clean)(md3, '')) === '{}',
+    '101',
+)
+console.assert(
+    JSON.stringify((0, xpath_1.xpath_clean)(md3, 'empty-string')) === '""',
+    '102',
+)
+console.assert(
+    JSON.stringify((0, xpath_1.xpath_clean)(md3, 'metadata')) === '{}',
+    '103',
+)
+console.assert(
+    JSON.stringify((0, xpath_1.xpath_clean)(md3, 'metadata.kernelspec')) ===
+    '{"empty-string":"","metadata":{}}',
+    '104',
+)
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/src/xpath-test.ts` & `jupyterlab_celltagsclasses-0.3.2/src/xpath-test.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 /* eslint-disable prettier/prettier */
 
 import {
-    xpath_get, xpath_set, xpath_unset,  xpath_insert, xpath_remove, xpath_clean,
+  xpath_get,
+  xpath_set,
+  xpath_unset,
+  xpath_insert,
+  xpath_remove,
+  xpath_clean,
 } from './xpath'
 
 /* not guaranteed to work by side-effects only */
 let md = {}
 
 // uncomment to debug
 const checkpoint = (md: Record<string, any>, message: string) => {
-    // console.log('------', message, '\n', JSON.stringify(md))
-    message
+  // console.log('------', message, '\n', JSON.stringify(md))
+  message
 }
 
 console.assert(xpath_get(md, 'simple') === undefined, '001')
 console.assert(xpath_set(md, 'simple', 1) === 1, '002')
 console.assert(xpath_get(md, 'simple') === 1, '003')
 
 checkpoint(md, "should have 'simple' set to 1")
@@ -46,15 +51,18 @@
 console.assert(xpath_get(md, ['jupyter', 'source_hidden']) === true, '035')
 console.assert(xpath_get(md, 'jupyter.source_hidden') === true, '036')
 
 checkpoint(md, 'jupyter.source_hidden=true')
 
 // cannot insert in pre-existing non-array
 console.assert(xpath_insert(md, 'jupyter', 'anything') === undefined, '041')
-console.assert(xpath_insert(md, 'jupyter.source_hidden', 'anything') === undefined, '042')
+console.assert(
+  xpath_insert(md, 'jupyter.source_hidden', 'anything') === undefined,
+  '042',
+)
 
 checkpoint(md, 'same')
 
 console.assert(xpath_get(md, 'tags.hide-input') === undefined, '051')
 // first time ok
 console.assert(xpath_insert(md, 'tags', 'hide-input') === 'hide-input', '052')
 // then ko
@@ -77,48 +85,54 @@
 console.assert(xpath_set(md, 'hide_input', true) === true, '072')
 console.assert(xpath_set(md, 'hide_input', false) === false, '072-bis')
 console.assert(xpath_unset(md, 'hide_input') === true, '073')
 console.assert(xpath_get(md, 'hide_input') === undefined, '074')
 
 checkpoint(md, 'unchanged')
 
-const xpaths = [ 'empty-list', 'nested.empty-list' ]
+const xpaths = ['empty-list', 'nested.empty-list']
 for (const xpath of xpaths) {
-    console.assert(xpath_insert(md, xpath, 'foo') === 'foo', '081')
-    console.assert(xpath_insert(md, xpath, 'bar') === 'bar', '082')
-    console.assert(xpath_remove(md, xpath, 'foo') === 'foo', '083')
-    console.assert(xpath_remove(md, xpath, 'bar') === 'bar', '084')
-    md = xpath_clean(md, '')
-    console.assert(xpath_get(md, xpath) === undefined, '085')
-    checkpoint(md, `unchanged after inserting/cleaning in ${xpath}`)
+  console.assert(xpath_insert(md, xpath, 'foo') === 'foo', '081')
+  console.assert(xpath_insert(md, xpath, 'bar') === 'bar', '082')
+  console.assert(xpath_remove(md, xpath, 'foo') === 'foo', '083')
+  console.assert(xpath_remove(md, xpath, 'bar') === 'bar', '084')
+  md = xpath_clean(md, '')
+  console.assert(xpath_get(md, xpath) === undefined, '085')
+  checkpoint(md, `unchanged after inserting/cleaning in ${xpath}`)
 }
 
 ////////////////////////////////////////
 
 const md2 = {
-    'cells': [
-    ],
-    'metadata': {
-        'kernelspec': {},
-        'language_info': [],
-    },
+  cells: [],
+  metadata: {
+    kernelspec: {},
+    language_info: [],
+  },
 }
 
-console.assert(JSON.stringify(xpath_clean(md2, '')) === "{}", '091')
-console.assert(JSON.stringify(xpath_clean(md2, 'cells')) === "[]", '092')
-console.assert(JSON.stringify(xpath_clean(md2, 'metadata')) === "{}", '093')
-console.assert(JSON.stringify(xpath_clean(md2, 'metadata.kernelspec')) === '{"cells":[],"metadata":{}}', '094')
-
+console.assert(JSON.stringify(xpath_clean(md2, '')) === '{}', '091')
+console.assert(JSON.stringify(xpath_clean(md2, 'cells')) === '[]', '092')
+console.assert(JSON.stringify(xpath_clean(md2, 'metadata')) === '{}', '093')
+console.assert(
+  JSON.stringify(xpath_clean(md2, 'metadata.kernelspec')) ===
+    '{"cells":[],"metadata":{}}',
+  '094',
+)
 
 const md3 = {
+  'empty-string': '',
+  metadata: {
+    kernelspec: {},
+    language_info: [],
     'empty-string': '',
-    'metadata': {
-        'kernelspec': {},
-        'language_info': [],
-        'empty-string': "",
-    },
+  },
 }
 
-console.assert(JSON.stringify(xpath_clean(md3, '')) === "{}", '101')
+console.assert(JSON.stringify(xpath_clean(md3, '')) === '{}', '101')
 console.assert(JSON.stringify(xpath_clean(md3, 'empty-string')) === '""', '102')
-console.assert(JSON.stringify(xpath_clean(md3, 'metadata')) === "{}", '103')
-console.assert(JSON.stringify(xpath_clean(md3, 'metadata.kernelspec')) === '{"empty-string":"","metadata":{}}', '104')
+console.assert(JSON.stringify(xpath_clean(md3, 'metadata')) === '{}', '103')
+console.assert(
+  JSON.stringify(xpath_clean(md3, 'metadata.kernelspec')) ===
+    '{"empty-string":"","metadata":{}}',
+  '104',
+)
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/src/xpath.js` & `jupyterlab_celltagsclasses-0.3.2/src/xpath.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,207 +1,218 @@
-"use strict";
+'use strict'
 /* eslint-disable no-case-declarations */
 /* eslint-disable prettier/prettier */
-Object.defineProperty(exports, "__esModule", {
+Object.defineProperty(exports, '__esModule', {
     value: true
-});
-exports.xpath_clean = exports.xpath_remove = exports.xpath_insert = exports.xpath_unset = exports.xpath_set = exports.xpath_get = exports.normalize = void 0;
+})
+exports.xpath_clean =
+    exports.xpath_remove =
+    exports.xpath_insert =
+    exports.xpath_unset =
+    exports.xpath_set =
+    exports.xpath_get =
+    exports.normalize =
+    void 0
 // helpers to manage a JS object
 //
 // in this module we are only concerned about doing side effects
 // in a JavaScript object
 // what to do on the passed object
 var Action;
 (function(Action) {
-    Action[Action["Get"] = 0] = "Get";
-    Action[Action["Set"] = 1] = "Set";
-    Action[Action["Unset"] = 2] = "Unset";
-    Action[Action["Insert"] = 3] = "Insert";
-    Action[Action["Remove"] = 4] = "Remove";
-})(Action || (Action = {}));
+    Action[(Action['Get'] = 0)] = 'Get'
+    Action[(Action['Set'] = 1)] = 'Set'
+    Action[(Action['Unset'] = 2)] = 'Unset'
+    Action[(Action['Insert'] = 3)] = 'Insert'
+    Action[(Action['Remove'] = 4)] = 'Remove'
+})(Action || (Action = {}))
 var normalize = function(xpath) {
     if (typeof xpath === 'string') {
-        var string = xpath;
+        var string = xpath
         if (string.length === 0) {
-            return [];
+            return []
         }
-        return string.split('.');
+        return string.split('.')
     } else if (xpath instanceof Array) {
-        return xpath;
+        return xpath
     } else {
-        console.error("xpath must be string or array, got ".concat(xpath));
-        return [];
+        console.error('xpath must be string or array, got '.concat(xpath))
+        return []
     }
-};
-exports.normalize = normalize;
-var _manage_metadata = function(data, // intended to be cell.metadata
-    action, xpath, value) {
+}
+exports.normalize = normalize
+var _manage_metadata = function(
+    data, // intended to be cell.metadata
+    action,
+    xpath,
+    value,
+) {
     var Get = Action.Get,
         Set = Action.Set,
         Unset = Action.Unset,
         Insert = Action.Insert,
-        Remove = Action.Remove;
+        Remove = Action.Remove
     var recurse = function(scanner, action, xpath, value) {
         // console.log(`in recurse with xpath=${xpath}`)
         if (xpath.length === 0) {
             switch (action) {
                 case Get:
-                    return scanner;
+                    return scanner
                 default:
-                    return undefined;
+                    return undefined
             }
         } else if (xpath.length === 1) {
-            var step = xpath[0];
+            var step = xpath[0]
             //
             switch (action) {
                 case Get:
-                    return scanner[step];
+                    return scanner[step]
                 case Set:
-                    scanner[step] = value;
-                    return value;
+                    scanner[step] = value
+                    return value
                 case Unset:
                     if (step in scanner) {
-                        delete scanner[step];
-                        return true;
+                        delete scanner[step]
+                        return true
                     } else {
-                        return false;
+                        return false
                     }
                 case Insert:
                     // create list if needed
                     if (!(step in scanner)) {
-                        scanner[step] = [];
+                        scanner[step] = []
                     }
                     if (!(scanner[step] instanceof Array)) {
-                        return undefined;
+                        return undefined
                     }
                     // insert if not already present
                     {
-                        var list_1 = scanner[step];
+                        var list_1 = scanner[step]
                         if (list_1.indexOf(value) < 0) {
-                            list_1.push(value);
-                            return value;
+                            list_1.push(value)
+                            return value
                         } else {
-                            return undefined;
+                            return undefined
                         }
                     }
                 case Remove:
                     if (!(scanner[step] instanceof Array)) {
-                        return undefined;
+                        return undefined
                     }
-                    var list = (scanner[step]);
+                    var list = scanner[step]
                     // list.pop(value) is not accepted by ts ?!?
-                    var index = list.indexOf(value);
+                    var index = list.indexOf(value)
                     if (index >= 0) {
-                        list.splice(index, 1);
+                        list.splice(index, 1)
                     }
-                    return value;
+                    return value
             }
         } else {
             var first = xpath[0],
-                rest = xpath.slice(1);
+                rest = xpath.slice(1)
             if (first in scanner) {
                 if (!(scanner[first] instanceof Object)) {
-                    return undefined;
+                    return undefined
                 } else {
-                    var next = scanner[first];
-                    return recurse(next, action, rest, value);
+                    var next = scanner[first]
+                    return recurse(next, action, rest, value)
                 }
             } else {
                 switch (action) {
                     case Get:
-                        return undefined;
+                        return undefined
                     case Set:
-                        scanner[first] = {};
-                        var next = scanner[first];
-                        return recurse(next, action, rest, value);
+                        scanner[first] = {}
+                        var next = scanner[first]
+                        return recurse(next, action, rest, value)
                     case Unset:
-                        return undefined;
+                        return undefined
                     case Insert:
                         if (rest.length === 0) {
-                            scanner[first] = [];
-                            return recurse(scanner[first], action, rest, value);
+                            scanner[first] = []
+                            return recurse(scanner[first], action, rest, value)
                         } else {
-                            scanner[first] = {};
-                            return recurse(scanner[first], action, rest, value);
+                            scanner[first] = {}
+                            return recurse(scanner[first], action, rest, value)
                         }
                     case Remove:
-                        return undefined;
+                        return undefined
                 }
             }
         }
-    };
-    var xpath_list = (0, exports.normalize)(xpath);
-    return recurse(data, action, xpath_list, value);
-};
+    }
+    var xpath_list = (0, exports.normalize)(xpath)
+    return recurse(data, action, xpath_list, value)
+}
 var _clean_metadata = function(data, xpath) {
     var not_empty = function(x) {
         if (x instanceof Array) {
-            return x.length !== 0;
+            return x.length !== 0
         } else if (x instanceof Object) {
-            return Object.keys(x).length !== 0;
-        } else if ((typeof x) === 'string') {
-            return x.length !== 0;
+            return Object.keys(x).length !== 0
+        } else if (typeof x === 'string') {
+            return x.length !== 0
         } else {
-            return true;
+            return true
         }
-    };
+    }
     var clean_array = function(data) {
-        return data.map(clean).filter(not_empty);
-    };
+        return data.map(clean).filter(not_empty)
+    }
     var clean_object = function(data) {
-        var result = {};
+        var result = {}
         for (var key in data) {
-            var value = data[key];
-            var cleaned = clean(value);
+            var value = data[key]
+            var cleaned = clean(value)
             if (not_empty(cleaned)) {
-                result[key] = cleaned;
+                result[key] = cleaned
             }
         }
-        return result;
-    };
+        return result
+    }
     var clean = function(data) {
         if (data instanceof Array) {
-            return clean_array(data);
+            return clean_array(data)
         } else if (data instanceof Object) {
-            return clean_object(data);
+            return clean_object(data)
         } else {
-            return data;
+            return data
         }
-    };
-    var xpath_list = (0, exports.normalize)(xpath);
+    }
+    var xpath_list = (0, exports.normalize)(xpath)
     if (xpath_list.length === 0) {
-        return clean(data);
+        return clean(data)
     } else {
-        var start = (0, exports.xpath_get)(data, xpath_list);
+        var start = (0, exports.xpath_get)(data, xpath_list)
         if (start === undefined) {
             // nothing serious here, just a debug message
             //console.debug(`DBG: xpath_clean: nothing to clean at ${xpath} - from ${xpath_list}`)
-            return data;
+            return data
         } else {
-            return (0, exports.xpath_set)(data, xpath_list, clean(start));
+            return (0, exports.xpath_set)(data, xpath_list, clean(start))
         }
     }
-};
+}
 var xpath_get = function(metadata, xpath) {
-    return _manage_metadata(metadata, Action.Get, xpath, undefined);
-};
-exports.xpath_get = xpath_get;
+    return _manage_metadata(metadata, Action.Get, xpath, undefined)
+}
+exports.xpath_get = xpath_get
 var xpath_set = function(metadata, xpath, value) {
-    return _manage_metadata(metadata, Action.Set, xpath, value);
-};
-exports.xpath_set = xpath_set;
+    return _manage_metadata(metadata, Action.Set, xpath, value)
+}
+exports.xpath_set = xpath_set
 var xpath_unset = function(metadata, xpath) {
-    return _manage_metadata(metadata, Action.Unset, xpath, undefined);
-};
-exports.xpath_unset = xpath_unset;
+    return _manage_metadata(metadata, Action.Unset, xpath, undefined)
+}
+exports.xpath_unset = xpath_unset
 var xpath_insert = function(metadata, xpath, key) {
-    return _manage_metadata(metadata, Action.Insert, xpath, key);
-};
-exports.xpath_insert = xpath_insert;
+    return _manage_metadata(metadata, Action.Insert, xpath, key)
+}
+exports.xpath_insert = xpath_insert
 var xpath_remove = function(metadata, xpath, key) {
-    return _manage_metadata(metadata, Action.Remove, xpath, key);
-};
-exports.xpath_remove = xpath_remove;
+    return _manage_metadata(metadata, Action.Remove, xpath, key)
+}
+exports.xpath_remove = xpath_remove
 var xpath_clean = function(metadata, xpath) {
-    return _clean_metadata(metadata, xpath);
-};
-exports.xpath_clean = xpath_clean;
+    return _clean_metadata(metadata, xpath)
+}
+exports.xpath_clean = xpath_clean
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/src/xpath.ts` & `jupyterlab_celltagsclasses-0.3.2/src/xpath.ts`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 /* eslint-disable prettier/prettier */
 
 // helpers to manage a JS object
 //
 // in this module we are only concerned about doing side effects
 // in a JavaScript object
 
-
 // what to do on the passed object
 enum Action {
-  Get,      // get the metadata at that xpath
-  Set,      // set the metadata at that xpath
-  Unset,    // undo the set operation
-  Insert,   // insert the value inside that xpath (should point to a list)
-  Remove,   // undo insert
+  Get, // get the metadata at that xpath
+  Set, // set the metadata at that xpath
+  Unset, // undo the set operation
+  Insert, // insert the value inside that xpath (should point to a list)
+  Remove, // undo insert
 }
 
-
 export type XpathMap = Record<string, any>
 export type Xpath = string | string[]
 
 export const normalize = (xpath: Xpath): string[] => {
   if (typeof xpath === 'string') {
     const string = xpath as string
     if (string.length === 0) {
@@ -31,31 +29,28 @@
     return xpath
   } else {
     console.error(`xpath must be string or array, got ${xpath}`)
     return []
   }
 }
 
-
 const _manage_metadata = (
-  data: XpathMap,      // intended to be cell.metadata
+  data: XpathMap, // intended to be cell.metadata
   action: Action,
   xpath: Xpath,
   value: any,
 ): any => {
-
-  const { Get, Set, Unset, Insert, Remove, } = Action
+  const { Get, Set, Unset, Insert, Remove } = Action
 
   const recurse = (
     scanner: XpathMap,
     action: Action,
     xpath: string[],
     value: any,
   ): any => {
-
     // console.log(`in recurse with xpath=${xpath}`)
 
     if (xpath.length === 0) {
       switch (action) {
         case Get:
           return scanner
         default:
@@ -95,15 +90,15 @@
               return undefined
             }
           }
         case Remove:
           if (!(scanner[step] instanceof Array)) {
             return undefined
           }
-          const list = (scanner[step]) as string[]
+          const list = scanner[step] as string[]
           // list.pop(value) is not accepted by ts ?!?
           const index = list.indexOf(value)
           if (index >= 0) {
             list.splice(index, 1)
           }
           return value
       }
@@ -143,28 +138,27 @@
 
   const xpath_list = normalize(xpath)
 
   return recurse(data, action, xpath_list, value)
 }
 
 const _clean_metadata = (data: XpathMap, xpath: Xpath): XpathMap => {
-
-  const not_empty = (x: any) : boolean => {
+  const not_empty = (x: any): boolean => {
     if (x instanceof Array) {
       return x.length !== 0
     } else if (x instanceof Object) {
       return Object.keys(x).length !== 0
-    } else if ((typeof x) === 'string') {
+    } else if (typeof x === 'string') {
       return x.length !== 0
     } else {
       return true
     }
   }
 
-  const clean_array = (data: any[]) : any[] => {
+  const clean_array = (data: any[]): any[] => {
     return data.map(clean).filter(not_empty)
   }
   const clean_object = (data: Record<string, any>): Record<string, any> => {
     const result = {} as Record<string, any>
     for (const key in data) {
       const value = data[key]
       const cleaned = clean(value)
@@ -172,15 +166,14 @@
         result[key] = cleaned
       }
     }
     return result
   }
 
   const clean = (data: any[] | Record<string, any>) => {
-
     if (data instanceof Array) {
       return clean_array(data)
     } else if (data instanceof Object) {
       return clean_object(data)
     } else {
       return data
     }
@@ -197,15 +190,14 @@
       return data
     } else {
       return xpath_set(data, xpath_list, clean(start))
     }
   }
 }
 
-
 export const xpath_get = (metadata: XpathMap, xpath: Xpath) =>
   _manage_metadata(metadata, Action.Get, xpath, undefined)
 export const xpath_set = (metadata: XpathMap, xpath: Xpath, value: any) =>
   _manage_metadata(metadata, Action.Set, xpath, value)
 export const xpath_unset = (metadata: XpathMap, xpath: Xpath) =>
   _manage_metadata(metadata, Action.Unset, xpath, undefined)
 export const xpath_insert = (metadata: XpathMap, xpath: Xpath, key: string) =>
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/style/base.css` & `jupyterlab_celltagsclasses-0.3.2/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/.gitignore` & `jupyterlab_celltagsclasses-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/LICENSE` & `jupyterlab_celltagsclasses-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/README.md` & `jupyterlab_celltagsclasses-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 
 ![](media/screenshot.png)
 
 ### metadata management helper functions
 
 it also exports utilities to manage a cell's metadata, specifically for
 
-* getting, setting or unsetting a key/value pair
-* adding, removing items in a list inside the metadata (e.g. tags)
-* cleaning the metadata for empty/useless items
+- getting, setting or unsetting a key/value pair
+- adding, removing items in a list inside the metadata (e.g. tags)
+- cleaning the metadata for empty/useless items
 
 to that effect, see the `md_get` and similar functions in `metadata.ts` (that can be imported right from the module)
 
 ### helper: apply function on cells
 
 the `apply_on_cells` function allows you to write a function that works on an individual cell, and then call it on either
 
-* the active cell only
-* all the selected cells if relevant, otherwise the active cell
-* all the cells in the notebook
+- the active cell only
+- all the selected cells if relevant, otherwise the active cell
+- all the cells in the notebook
 
 for that you can pass it a `Scope` value that can be either `Active`, `Multiple`, or `All`
 
 ## Development
 
 See the documentation on Jlab extensions for more details; the gist of it is
```

### Comparing `jupyterlab_celltagsclasses-0.3.1/pyproject.toml` & `jupyterlab_celltagsclasses-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_celltagsclasses-0.3.1/PKG-INFO` & `jupyterlab_celltagsclasses-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_celltagsclasses
-Version: 0.3.1
+Version: 0.3.2
 Summary: JLAB extension to add classes to cells based on their tags
 Project-URL: Homepage, https://github.com/parmentelat/jupyterlab-celltagsclasses
 Project-URL: Bug Tracker, https://github.com/parmentelat/jupyterlab-celltagsclasses/issues
 Project-URL: Repository, https://github.com/parmentelat/jupyterlab-celltagsclasses.git
 Author-email: Thierry Parmentelat <thierry.parmentelat@inria.fr>
 License: BSD 3-Clause License
         
@@ -88,27 +88,27 @@
 
 ![](media/screenshot.png)
 
 ### metadata management helper functions
 
 it also exports utilities to manage a cell's metadata, specifically for
 
-* getting, setting or unsetting a key/value pair
-* adding, removing items in a list inside the metadata (e.g. tags)
-* cleaning the metadata for empty/useless items
+- getting, setting or unsetting a key/value pair
+- adding, removing items in a list inside the metadata (e.g. tags)
+- cleaning the metadata for empty/useless items
 
 to that effect, see the `md_get` and similar functions in `metadata.ts` (that can be imported right from the module)
 
 ### helper: apply function on cells
 
 the `apply_on_cells` function allows you to write a function that works on an individual cell, and then call it on either
 
-* the active cell only
-* all the selected cells if relevant, otherwise the active cell
-* all the cells in the notebook
+- the active cell only
+- all the selected cells if relevant, otherwise the active cell
+- all the cells in the notebook
 
 for that you can pass it a `Scope` value that can be either `Active`, `Multiple`, or `All`
 
 ## Development
 
 See the documentation on Jlab extensions for more details; the gist of it is
```

