# Comparing `tmp/unigui-1.5.4.tar.gz` & `tmp/unigui-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.5.4.tar", last modified: Sat Jul  1 14:25:04 2023, max compression
+gzip compressed data, was "dist/unigui-1.6.0.tar", last modified: Sat Jul  1 19:40:56 2023, max compression
```

## Comparing `unigui-1.5.4.tar` & `unigui-1.6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13116 2023-07-01 14:21:18.000000 unigui-1.5.4/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     9068 2023-06-12 23:28:53.000000 unigui-1.5.4/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.5.4/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.5.4/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.5.4/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/css/vendor.49a52e8f.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/css/361.c9159919.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)    43129 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/361.78add75c.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/app.6ab35062.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-06-12 23:10:20.000000 unigui-1.5.4/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.5.4/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-01 14:22:35.000000 unigui-1.5.4/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19997 2023-07-01 14:25:04.000000 unigui-1.5.4/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-01 14:25:04.000000 unigui-1.5.4/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19692 2023-07-01 14:05:35.000000 unigui-1.5.4/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.5.4/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19997 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.5.4/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1205 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-01 14:25:04.000000 unigui-1.5.4/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 19:40:56.000000 unigui-1.6.0/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13149 2023-07-01 19:08:47.000000 unigui-1.6.0/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9068 2023-06-12 23:28:53.000000 unigui-1.6.0/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.6.0/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      102 2023-06-21 23:42:45.000000 unigui-1.6.0/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.6.0/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/css/622.13cee13e.css
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    44039 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/js/622.b0e2d91a.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/js/app.09b50726.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-01 19:35:20.000000 unigui-1.6.0/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.6.0/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-01 19:39:53.000000 unigui-1.6.0/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19988 2023-07-01 19:40:56.000000 unigui-1.6.0/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-01 19:40:56.000000 unigui-1.6.0/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19683 2023-07-01 14:44:31.000000 unigui-1.6.0/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.6.0/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19988 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.6.0/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1205 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-01 19:40:56.000000 unigui-1.6.0/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.5.4/unigui/manager.py` & `unigui-1.6.0/unigui/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,16 @@
     def load(self):   
         screen_vars = {
             'icon' : 'article',
             'prepare' : None,
             'dispatch' : None,
             'blocks' : [],
             'header' : utils.appname,                        
-            'toolbar' : None
+            'toolbar' : None, 
+            'order' : 0
         }     
          
         blocks_dir = 'blocks'        
         screens_dir =  'screens'
         modules = {}
         for file in os.listdir(screens_dir):
             if file.endswith(".py") and file != '__init__.py':
@@ -182,15 +183,15 @@
                 screen.handlers__ = utils.handlers__
                 
                 if not screen.toolbar:
                     screen.toolbar = self.tool_buttons
                                 
                 screen.check()                         
         
-        self.screens.sort(key=lambda s: s.order)
+        self.screens.sort(key=lambda s: s.screen.order)
         main = self.screens[0]
         if 'prepare' in dir(main):
             main.prepare()
         self.screen_module = main
         self.menu = [[s.name,getattr(s,'icon', None)] for s in self.screens]        
 
         #remove user modules from sys for repeating loading for new users
```

### Comparing `unigui-1.5.4/unigui/guielements.py` & `unigui-1.6.0/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/server.py` & `unigui-1.6.0/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/utils.py` & `unigui-1.6.0/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/favicon.ico` & `unigui-1.6.0/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.6.0/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/css/361.c9159919.css` & `unigui-1.6.0/unigui/web/css/622.13cee13e.css`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-0593ed42]{display:flex;justify-content:center}.custom-caption[data-v-0593ed42]{padding:5px!important}.web-camera-container[data-v-0593ed42]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-0593ed42]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-0593ed42]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-0593ed42]{opacity:1}.web-camera-container .camera-shoot[data-v-0593ed42]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-0593ed42]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-0593ed42]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-0593ed42]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-0593ed42]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-0593ed42]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-0593ed42]{animation:preload-0593ed42 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-0593ed42]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-0593ed42]:nth-child(3){animation-delay:.4s}@keyframes preload-0593ed42{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-0593ed42]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-606d07c3]{display:flex;justify-content:center}.custom-caption[data-v-606d07c3]{padding:5px!important}.web-camera-container[data-v-606d07c3]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-606d07c3]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-606d07c3]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-606d07c3]{opacity:1}.web-camera-container .camera-shoot[data-v-606d07c3]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-606d07c3]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-606d07c3]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-606d07c3]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-606d07c3]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-606d07c3]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-606d07c3]{animation:preload-606d07c3 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-606d07c3]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-606d07c3]:nth-child(3){animation-delay:.4s}@keyframes preload-606d07c3{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-606d07c3]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.5.4/unigui/web/icons/favicon-96x96.png` & `unigui-1.6.0/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/icons/favicon-16x16.png` & `unigui-1.6.0/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/icons/favicon-32x32.png` & `unigui-1.6.0/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/icons/favicon-128x128.png` & `unigui-1.6.0/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.6.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.6.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.6.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.6.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.6.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.6.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.6.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.6.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/js/361.78add75c.js` & `unigui-1.6.0/unigui/web/js/622.b0e2d91a.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,82 +1,97 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [361], {
-        361: (e, t, a) => {
+    [622], {
+        6622: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Gt
+                default: () => Jt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
-                class: "q-pa-lg"
-            }, null, -1);
-
-            function o(e, t, a, o, n, d) {
-                const r = (0, l.up)("q-item-label"),
-                    c = (0, l.up)("q-tab"),
-                    h = (0, l.up)("q-tabs"),
-                    u = (0, l.up)("q-toolbar"),
-                    p = (0, l.up)("q-header"),
-                    g = (0, l.up)("zone"),
-                    m = (0, l.up)("q-page"),
-                    f = (0, l.up)("q-page-container"),
-                    y = (0, l.up)("q-layout");
-                return (0, l.wg)(), (0, l.j4)(y, {
+                    class: "q-pa-lg"
+                }, null, -1),
+                o = (0, l._)("div", {
+                    class: "q-pa-lg"
+                }, null, -1);
+
+            function n(e, t, a, n, d, r) {
+                const c = (0, l.up)("q-item-label"),
+                    h = (0, l.up)("element"),
+                    u = (0, l.up)("q-tab"),
+                    p = (0, l.up)("q-tabs"),
+                    g = (0, l.up)("q-toolbar"),
+                    m = (0, l.up)("q-header"),
+                    f = (0, l.up)("zone"),
+                    w = (0, l.up)("q-page"),
+                    y = (0, l.up)("q-page-container"),
+                    b = (0, l.up)("q-layout");
+                return (0, l.wg)(), (0, l.j4)(b, {
                     view: "lHh Lpr lFf"
                 }, {
-                    default: (0, l.w5)((() => [(0, l.Wm)(p, {
+                    default: (0, l.w5)((() => [(0, l.Wm)(m, {
                         elevated: ""
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(u, null, {
-                            default: (0, l.w5)((() => [(0, l.Wm)(r, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(g, null, {
+                            default: (0, l.w5)((() => [(0, l.Wm)(c, {
                                 class: "text-h5"
                             }, {
                                 default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.screen.header ? e.screen.header : ""), 1)])),
                                 _: 1
-                            }), i, (0, l.Wm)(h, {
+                            }), i, ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.screen.toolbar, (t => ((0, l.wg)(), (0, l.j4)(h, {
+                                class: "q-ma-xs",
+                                data: t,
+                                pdata: e.data
+                            }, null, 8, ["data", "pdata"])))), 256)), o, (0, l.Wm)(p, {
                                 class: "text-teal",
                                 align: "center",
                                 "inline-label": "",
                                 dense: "",
                                 modelValue: e.tab,
                                 "onUpdate:modelValue": t[0] || (t[0] = t => e.tab = t),
                                 style: {
                                     float: "center"
                                 }
                             }, {
-                                default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.menu, (t => ((0, l.wg)(), (0, l.j4)(c, {
+                                default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.menu, (t => ((0, l.wg)(), (0, l.iD)("div", null, [t.icon ? ((0, l.wg)(), (0, l.j4)(u, {
+                                    key: 0,
                                     class: "justify-center text-white shadow-2",
                                     name: t.name,
                                     icon: t.icon,
                                     label: t.name,
                                     onClick: a => e.tabclick(t.name)
-                                }, null, 8, ["name", "icon", "label", "onClick"])))), 256))])),
+                                }, null, 8, ["name", "icon", "label", "onClick"])) : (0, l.kq)("", !0), t.icon ? (0, l.kq)("", !0) : ((0, l.wg)(), (0, l.j4)(u, {
+                                    key: 1,
+                                    class: "justify-center text-white shadow-2",
+                                    name: t.name,
+                                    label: t.name,
+                                    onClick: a => e.tabclick(t.name)
+                                }, null, 8, ["name", "label", "onClick"]))])))), 256))])),
                                 _: 1
                             }, 8, ["modelValue"])])),
                             _: 1
                         })])),
                         _: 1
-                    }), (0, l.Wm)(f, null, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(m, {
+                    }), (0, l.Wm)(y, null, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(w, {
                             class: "flex justify-center centers"
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Wm)(g, {
+                            default: (0, l.w5)((() => [(0, l.Wm)(f, {
                                 data: e.screen.blocks
                             }, null, 8, ["data"])])),
                             _: 1
                         })])),
                         _: 1
                     })])),
                     _: 1
                 })
             }
             a(71);
 
-            function n(e, t, a, i, o, n) {
+            function d(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-item-section"),
                     c = (0, l.up)("q-item-label"),
                     h = (0, l.up)("q-item");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     clickable: "",
                     tag: "a",
@@ -96,164 +111,164 @@
                             _: 1
                         })])),
                         _: 1
                     })])),
                     _: 1
                 }, 8, ["onClick"])
             }
-            var d, r = a(698),
-                c = a(8603);
-            let h = null,
-                u = {},
-                p = !0;
-            const g = 136,
-                m = 400,
-                f = `height: ${g}px; width: ${m}px`;
+            var r, c = a(698),
+                h = a(8603);
+            let u = null,
+                p = {},
+                g = !0;
+            const m = 136,
+                f = 400,
+                w = `height: ${m}px; width: ${f}px`;
 
             function y(e) {
-                let t = e.minheight ? e.minheight : g,
-                    a = e.minwidth ? e.minwidth : m;
+                let t = e.minheight ? e.minheight : m,
+                    a = e.minwidth ? e.minwidth : f;
                 return `height: ${t}px; width: ${a}px`
             }
-            let w = {},
-                b = {};
-            const k = ["error", "progress", "warning", "info"];
-
-            function v(e) {
-                d = new WebSocket("ws://localhost:8000/ws"), d.onopen = () => e.statusConnect = !0, d.onmessage = t => {
-                    p && console.log("socket message", t.data), e.processMessage(JSON.parse(t.data))
-                }, d.onerror = t => e.error(t), d.onclose = t => {
-                    t.wasClean ? e.info("Connection closed and was clean.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, p && console.info("close code : " + t.code + " reason: " + t.reason)
-                }, h = e
-            }
+            let b = {},
+                k = {};
+            const v = ["error", "progress", "warning", "info"];
 
             function C(e) {
-                console.log("sended", e), d.send(JSON.stringify(e))
+                r = new WebSocket("ws://localhost:8000/ws"), r.onopen = () => e.statusConnect = !0, r.onmessage = t => {
+                    g && console.log("socket message", t.data), e.processMessage(JSON.parse(t.data))
+                }, r.onerror = t => e.error(t), r.onclose = t => {
+                    t.wasClean ? e.info("Connection closed and was clean.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
+                }, u = e
             }
-            let q, S = 0;
 
-            function j() {
-                for (let [e, t] of Object.entries(b)) t.styleSize = null
+            function q(e) {
+                console.log("sended", e), r.send(JSON.stringify(e))
             }
+            let j, S = 0;
 
-            function z(e, t, a, l = "?") {
+            function z() {
+                for (let [e, t] of Object.entries(k)) t.styleSize = null
+            }
+
+            function A(e, t, a, l = "?") {
                 let s = ++S,
                     i = [e.pdata.name, e.data.name, l, t, s];
-                C(i), u[s] = a
+                q(i), p[s] = a
             }
 
-            function A() {
-                w = {}, b = {}
+            function Z() {
+                b = {}, k = {}
             }
 
-            function Z(e, t) {
+            function M(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function M(e) {
+            function D(e) {
                 if (e.multi)
                     for (let [t, a] of e.update.entries())
                         if (a.length > 1) {
                             a.reverse();
                             let l = a.join("@"),
-                                s = b[l];
-                            Z(s, e.data[t])
+                                s = k[l];
+                            M(s, e.data[t])
                         } else {
-                            let l = w[a[0]];
+                            let l = b[a[0]];
                             Object.assign(l.data, e.data[t])
                         }
                 else {
                     let t, a = e.update;
                     if (a.length > 1) {
                         a.reverse();
                         let e = a.join("@");
-                        t = b[e]
-                    } else t = w[a[0]];
-                    Z(t, e.data), 1 == a.length && (0, c.delay)(W, 200, t)
+                        t = k[e]
+                    } else t = b[a[0]];
+                    M(t, e.data), 1 == a.length && (0, h.delay)(W, 200, t)
                 }
             }
 
             function $(e) {
-                typeof e.answer == String ? h.showError() : u[e.id](e.answer), delete u[e.id]
+                typeof e.answer == String ? u.showError() : p[e.id](e.answer), delete p[e.id]
             }
 
-            function D(e) {
+            function V(e) {
                 let t = [];
                 for (let l of e) l instanceof Array ? t.push(l) : t.push([l]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function V() {
-                for (let [e, t] of Object.entries(b)) t.expanding && (t.styleSize = y(t.data));
+            function O() {
+                for (let [e, t] of Object.entries(k)) t.expanding && (t.styleSize = y(t.data));
                 (0, l.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
                             W()
                         }))
                     }))
                 }))
             }
-            let O = _.debounce(V, 200);
+            let Q = _.debounce(O, 200);
 
             function W(e) {
-                Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), p && console.log("------------------recalc design");
-                const t = Q(e),
-                    a = H(e);
+                Array.isArray(e) && (e = null), j && (j.disconnect(), j = null), g && console.log("------------------recalc design");
+                const t = H(e),
+                    a = E(e);
                 for (let [l, s] of Object.entries(t)) {
-                    let e = b[l];
+                    let e = k[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
-                        r = w[d];
+                        r = b[d];
                     for (let a of r.data.childs)
                         if (Array.isArray(a)) {
                             if (a.find((t => t.name == e.data.name))) {
                                 let e = a[a.length - 1],
                                     t = `${e.name}@${d}`;
-                                o = b[t];
+                                o = k[t];
                                 break
                             }
                         } else if (a.name == e.data.name) {
                         o = e;
                         break
                     }
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
                     e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
-            function Q(e) {
-                const t = h.screen.blocks;
+            function H(e) {
+                const t = u.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
                     i = {};
-                for (let [d, r] of Object.entries(w)) i[r.name] = r.$el.getBoundingClientRect().height;
+                for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
                 let o = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
-                        n = t ? D(d) : [
+                        n = t ? V(d) : [
                             [d]
                         ];
                     for (let a of n) {
                         let e = 0;
                         for (let t of a) e += i[t.name] + 8;
                         o.push([e, a])
                     }
                     o.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
                     for (let l of o) {
                         let t = l[1];
-                        (0, r.hu)(Array.isArray(t));
+                        (0, c.hu)(Array.isArray(t));
                         const i = [];
-                        for (let [e, a] of Object.entries(b))
+                        for (let [e, a] of Object.entries(k))
                             if (a.expanding_height) {
                                 let [l, o] = e.split("@");
                                 if (t.find((e => e.name == o))) {
                                     let e = !0;
                                     const t = a.geom();
                                     for (let [l, o] of i.entries()) {
                                         let n = o.geom();
@@ -286,17 +301,17 @@
                 }
                 let n = Array.from(s.entries());
                 n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
                 for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
 
-            function H(e) {
+            function E(e) {
                 e = null;
-                const t = e ? [e] : h.screen.blocks;
+                const t = e ? [e] : u.screen.blocks;
                 let a = window.innerWidth - 30,
                     l = [],
                     s = {};
                 for (let n of t)
                     if (0 == l.length)
                         if (Array.isArray(n))
                             for (let e of n) l.push(Array.isArray(e) ? e : [e]);
@@ -313,20 +328,20 @@
                     l = e
                 }
                 l.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
                 const i = [];
                 let o = new Map;
                 for (let n of l) {
                     let e = Array.isArray(n) ? n[n.length - 1] : n,
-                        t = w[e.name].$el.getBoundingClientRect().right;
+                        t = b[e.name].$el.getBoundingClientRect().right;
                     e = Array.isArray(n) ? n[0] : n;
-                    let l = w[e.name].$el.getBoundingClientRect().left,
+                    let l = b[e.name].$el.getBoundingClientRect().left,
                         s = a - t + l - 10;
                     const d = [];
-                    for (let [a, i] of Object.entries(b))
+                    for (let [a, i] of Object.entries(k))
                         if (i.expanding_width) {
                             let e = a.split("@")[1];
                             if (n.find((t => t.name == e))) {
                                 let e = !0,
                                     t = i.geom().left;
                                 for (let [a, l] of d.entries())
                                     if (l !== i && l.geom().left == t) {
@@ -353,223 +368,224 @@
                             s[a.fullname] = [Math.floor(n / e), t[l]]
                         }
                     }
                 }
                 for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
                 return s
             }
-            const E = (0, l.aZ)({
+            const U = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
-                        C(["root", this.name])
+                        q(["root", this.name])
                     }
                 },
                 props: {
                     name: {
                         type: String,
                         required: !0
                     },
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
             var N = a(4260),
-                U = a(3414),
-                F = a(2035),
+                F = a(3414),
+                K = a(2035),
                 P = a(4554),
-                K = a(2350),
-                T = a(7518),
-                I = a.n(T);
-            const R = (0, N.Z)(E, [
-                    ["render", n]
+                T = a(2350),
+                I = a(7518),
+                R = a.n(I);
+            const B = (0, N.Z)(U, [
+                    ["render", d]
                 ]),
-                B = R;
-            I()(E, "components", {
-                QItem: U.Z,
-                QItemSection: F.Z,
+                L = B;
+            R()(U, "components", {
+                QItem: F.Z,
+                QItemSection: K.Z,
                 QIcon: P.Z,
-                QItemLabel: K.Z
+                QItemLabel: T.Z
             });
-            const L = {
+            const Y = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
-                Y = {
+                X = {
                     class: "q-col-gutter-sm"
                 },
-                X = {
+                G = {
                     key: 0,
                     class: "column q-col-gutter-sm"
                 };
 
-            function G(e, t, a, s, i, o) {
+            function J(e, t, a, s, i, o) {
                 const n = (0, l.up)("zone", !0),
                     d = (0, l.up)("block");
-                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", L, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", Y, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", X, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
+                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", Y, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", X, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", G, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
                     data: e
                 }, null, 8, ["data"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
-            const J = {
+            const ee = {
                     class: "row"
                 },
-                ee = {
+                te = {
                     key: 2,
                     class: "q-ma-sm",
                     style: {
                         "font-size": "18px"
                     }
                 },
-                te = ["data", "pdata"],
-                ae = {
+                ae = ["data", "pdata"],
+                le = {
                     key: 0,
                     class: "row"
                 },
-                le = ["data", "pdata"],
-                se = {
+                se = ["data", "pdata"],
+                ie = {
                     key: 0,
                     class: "row"
                 };
 
-            function ie(e, t, a, i, o, n) {
+            function oe(e, t, a, i, o, n) {
                 const d = (0, l.up)("element"),
                     r = (0, l.up)("q-icon"),
                     c = (0, l.up)("q-scroll-area"),
                     h = (0, l.up)("q-card");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     class: "my-card q-ma-xs"
                 }, {
-                    default: (0, l.w5)((() => [(0, l._)("div", J, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
+                    default: (0, l.w5)((() => [(0, l._)("div", ee, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 0,
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, l.wg)(), (0, l.j4)(r, {
                         key: 1,
                         size: "sm",
                         name: e.data.icon
-                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", ee, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.top_childs, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", te, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.top_childs, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))]), e.data.scroll ? ((0, l.wg)(), (0, l.j4)(c, {
                         key: 0,
                         style: (0, s.j5)(e.styleSize),
                         "thumb-style": e.thumbStyle,
                         "bar-style": e.barStyle
                     }, {
                         default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.childs, (t => ((0, l.wg)(), (0, l.iD)("div", {
                             class: "column",
                             data: t,
                             pdata: e.data
-                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ae, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", le, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
                         }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                             key: 1,
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
-                        }, null, 8, ["data", "pdata"]))], 8, te)))), 256))])),
+                        }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
                         _: 1
                     }, 8, ["style", "thumb-style", "bar-style"])) : ((0, l.wg)(!0), (0, l.iD)(l.HY, {
                         key: 1
                     }, (0, l.Ko)(e.data.childs, (t => ((0, l.wg)(), (0, l.iD)("div", {
                         class: "column",
                         data: t,
                         pdata: e.data
-                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", se, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ie, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
+                    }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
                     _: 1
                 })
             }
-            var oe = a(8880);
-            const ne = e => ((0, l.dD)("data-v-0593ed42"), e = e(), (0, l.Cn)(), e),
-                de = ["width", "height"],
-                re = ["src"],
-                ce = {
+            var ne = a(8880);
+            const de = e => ((0, l.dD)("data-v-606d07c3"), e = e(), (0, l.Cn)(), e),
+                re = ["width", "height"],
+                ce = ["src"],
+                he = {
                     key: 16,
                     class: "web-camera-container"
                 },
-                he = {
+                ue = {
                     class: "camera-button"
                 },
-                ue = {
+                pe = {
                     key: 0
                 },
-                pe = {
+                ge = {
                     key: 1
                 },
-                ge = {
+                me = {
                     class: "camera-loading"
                 },
-                me = ne((() => (0, l._)("ul", {
+                fe = de((() => (0, l._)("ul", {
                     class: "loader-circle"
                 }, [(0, l._)("li"), (0, l._)("li"), (0, l._)("li")], -1))),
-                fe = [me],
+                we = [fe],
                 ye = ["height"],
-                we = ["height"],
-                be = {
+                be = ["height"],
+                ke = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                ke = ne((() => (0, l._)("img", {
+                ve = de((() => (0, l._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                ve = [ke],
-                xe = {
+                xe = [ve],
+                Ce = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function Ce(e, t, a, i, o, n) {
+            function qe(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-img"),
                     c = (0, l.up)("q-badge"),
                     h = (0, l.up)("q-select"),
                     u = (0, l.up)("q-checkbox"),
                     p = (0, l.up)("q-toggle"),
                     g = (0, l.up)("q-btn-toggle"),
                     m = (0, l.up)("utable"),
                     f = (0, l.up)("linechart"),
-                    y = (0, l.up)("q-input"),
-                    w = (0, l.up)("q-tree"),
+                    w = (0, l.up)("q-input"),
+                    y = (0, l.up)("q-tree"),
                     b = (0, l.up)("q-scroll-area"),
                     k = (0, l.up)("q-separator"),
                     v = (0, l.up)("q-uploader"),
                     x = (0, l.up)("cgraph"),
-                    C = (0, l.up)("q-btn");
+                    C = (0, l.up)("q-btn"),
+                    q = (0, l.up)("q-tooltip");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
-                    onClick: (0, oe.iM)(e.switchValue, ["stop"]),
+                    onClick: (0, ne.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, s.j5)(e.elemSize)
                 }, {
                     default: (0, l.w5)((() => [e.data.header ? ((0, l.wg)(), (0, l.iD)("div", {
                         key: 0,
                         class: "absolute-bottom-right text-subtitle2 custom-caption",
-                        onClick: t[0] || (t[0] = (0, oe.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
+                        onClick: t[0] || (t[0] = (0, ne.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
                     }, (0, s.zw)(e.data.header), 1)) : (0, l.kq)("", !0), e.value ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "absolute all-pointer-events",
                         size: "32px",
                         name: "check_circle",
                         color: "gray",
                         style: {
@@ -639,23 +655,23 @@
                     pdata: e.pdata,
                     styleSize: e.styleSize
                 }, null, 8, ["data", "pdata", "styleSize"])) : "linechart" == e.type ? ((0, l.wg)(), (0, l.j4)(f, {
                     key: 6,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.styleSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, l.wg)(), (0, l.j4)(y, {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "edit" == e.type ? ((0, l.wg)(), (0, l.j4)(w, {
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
-                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, l.wg)(), (0, l.j4)(h, {
                     key: 8,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     "use-input": "",
@@ -664,22 +680,22 @@
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
-                    onKeyup: (0, oe.D2)(e.pressedEnter, ["enter"])
+                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"])
                 }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(b, {
                     key: 9,
                     style: (0, s.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
-                    default: (0, l.w5)((() => [(0, l.Wm)(w, {
+                    default: (0, l.w5)((() => [(0, l.Wm)(y, {
                         nodes: e.treeNodes,
                         selected: e.value,
                         "onUpdate:selected": t[7] || (t[7] = t => e.value = t),
                         expanded: e.expandedKeys,
                         "onUpdate:expanded": t[8] || (t[8] = t => e.expandedKeys = t),
                         "node-key": "label",
                         "default-expand-all": "",
@@ -690,27 +706,27 @@
                     key: 10,
                     class: "textarea",
                     "onUpdate:modelValue": t[9] || (t[9] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, s.j5)(e.elemSize)
                 }, null, 4)), [
-                    [oe.nr, e.value]
+                    [ne.nr, e.value]
                 ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
                     key: 11,
                     color: "green"
                 })) : "video" == e.type ? ((0, l.wg)(), (0, l.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, l._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, re)], 8, de)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
+                }, null, 8, ce)], 8, re)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
                     key: 13,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: "http://localhost:8000",
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
@@ -728,23 +744,23 @@
                     ref: "uploaderRef",
                     flat: ""
                 }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
                     key: 15,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ce, [(0, l._)("div", he, [(0, l._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", he, [(0, l._)("div", ue, [(0, l._)("button", {
                     class: (0, s.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[10] || (t[10] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", pe, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", ue, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", ge, fe, 512), [
-                    [oe.F8, e.isCameraOpen && e.isLoading]
+                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", ge, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", pe, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", me, we, 512), [
+                    [ne.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("div", {
                     key: 0,
                     class: (0, s.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, l._)("div", {
                     class: (0, s.C_)(["camera-shutter", {
@@ -752,65 +768,83 @@
                     }])
                 }, null, 2), (0, l.wy)((0, l._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
                 }, null, 8, ye), [
-                    [oe.F8, !e.isPhotoTaken]
+                    [ne.F8, !e.isPhotoTaken]
                 ]), (0, l.wy)((0, l._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, we), [
-                    [oe.F8, e.isPhotoTaken]
+                }, null, 8, be), [
+                    [ne.F8, e.isPhotoTaken]
                 ])], 2)), [
-                    [oe.F8, !e.isLoading]
-                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", be, [(0, l._)("button", {
+                    [ne.F8, !e.isLoading]
+                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", ke, [(0, l._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, ve)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", xe, [(0, l.Wm)(C, {
+                }, xe)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", Ce, [(0, l.Wm)(C, {
                     onClick: e.downloadImage,
                     label: "Send"
                 }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(C, {
                     key: 17,
                     "no-caps": "",
                     label: e.name,
                     icon: e.data.icon,
                     onClick: e.sendValue
-                }, null, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(C, {
+                }, {
+                    default: (0, l.w5)((() => [e.data.tooltip ? ((0, l.wg)(), (0, l.j4)(q, {
+                        key: 0,
+                        class: "text-body2"
+                    }, {
+                        default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
+                        _: 1
+                    })) : (0, l.kq)("", !0)])),
+                    _: 1
+                }, 8, ["label", "icon", "onClick"])) : ((0, l.wg)(), (0, l.j4)(C, {
                     key: 18,
                     "no-caps": "",
                     dense: "",
                     icon: e.data.icon,
                     onClick: e.sendValue
-                }, null, 8, ["icon", "onClick"]))
+                }, {
+                    default: (0, l.w5)((() => [e.data.tooltip ? ((0, l.wg)(), (0, l.j4)(q, {
+                        key: 0,
+                        class: "text-body2"
+                    }, {
+                        default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
+                        _: 1
+                    })) : (0, l.kq)("", !0)])),
+                    _: 1
+                }, 8, ["icon", "onClick"]))
             }
-            const qe = {
+            const _e = {
                     key: 0
                 },
-                _e = {
+                je = {
                     class: "row"
                 },
                 Se = ["onClick"];
 
-            function je(e, t, a, i, o, n) {
+            function ze(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-tooltip"),
                     c = (0, l.up)("q-input"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-th"),
                     p = (0, l.up)("q-tr"),
                     g = (0, l.up)("q-checkbox"),
                     m = (0, l.up)("q-select"),
                     f = (0, l.up)("q-td"),
-                    y = (0, l.up)("q-table");
-                return (0, l.wg)(), (0, l.j4)(y, {
+                    w = (0, l.up)("q-table");
+                return (0, l.wg)(), (0, l.j4)(w, {
                     class: "my-sticky-virtscroll-table",
                     "virtual-scroll": "",
                     dense: "",
                     style: (0, s.j5)(e.styleSize),
                     flat: "",
                     filter: e.search,
                     ref: "table",
@@ -821,15 +855,15 @@
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", qe, [(0, l._)("div", _e, [(0, l.Wm)(c, {
+                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", _e, [(0, l._)("div", je, [(0, l.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
                     }, (0, l.Nv)({
                         append: (0, l.w5)((() => ["" != e.search ? ((0, l.wg)(), (0, l.j4)(d, {
@@ -1018,26 +1052,26 @@
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var ze = a(1959);
+            var Ae = a(1959);
 
-            function Ae(e, t) {
+            function Ze(e, t) {
                 return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
             }
-            const Ze = (0, l.aZ)({
+            const Me = (0, l.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, ze.BK)(e);
+                    } = (0, Ae.BK)(e);
                     let s = (0, l.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const l = a.headers,
                                 s = l.length,
                                 i = a.rows,
                                 o = i.length;
@@ -1051,26 +1085,26 @@
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
                             return a
                         },
                         o = i(),
-                        n = (0, ze.iH)(o),
-                        d = (0, ze.iH)(o),
-                        r = (0, ze.iH)(!Array.isArray(t.value.value)),
+                        n = (0, Ae.iH)(o),
+                        d = (0, Ae.iH)(o),
+                        r = (0, Ae.iH)(!Array.isArray(t.value.value)),
                         c = (e, l) => {
-                            C([a.value.name, t.value.name, e, l])
+                            q([a.value.name, t.value.name, e, l])
                         },
                         h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
                         d.value = i(), n.value = d.value
                     })), (0, l.YP)(t, ((e, a) => {
-                        p && console.log("data update", a.name), d.value = i(), n.value = d.value, r.value = !Array.isArray(t.value.value)
+                        g && console.log("data update", a.name), d.value = i(), n.value = d.value, r.value = !Array.isArray(t.value.value)
                     })), {
                         rows: s,
                         value: h,
                         selected: d,
                         singleMode: r,
                         sendMessage: c,
                         datavalue: u,
@@ -1083,36 +1117,36 @@
                         editMode: !1,
                         options: [],
                         cedit: null
                     }
                 },
                 methods: {
                     select(e, t) {
-                        this.editMode && (this.cedit = t, p && console.log("selected", e, this.cedit))
+                        this.editMode && (this.cedit = t, g && console.log("selected", e, this.cedit))
                     },
                     change_switcher(e, t, a) {
                         if (console.log(e, t, a, e[t]), this.editMode) {
                             this.cedit = a;
                             const l = e.iiid;
                             let s = this.data.rows;
                             s[l][a] = e[t], this.sendMessage("#", [e[t],
                                 [l, a]
                             ])
                         }
                     },
                     change(e) {
-                        if (p && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
+                        if (g && console.log("changed", this.data.headers[this.cedit], e), this.editMode && this.selected.length) {
                             const t = this.selected[0].iiid;
                             let a = this.data.rows;
                             a[t][this.cedit] = e, this.sendMessage("#", [e, [t, this.cedit]])
                         }
                     },
                     keyInput(e) {
                         if ("Control" == e.key) return;
-                        p && console.log("keypress", e);
+                        g && console.log("keypress", e);
                         let t = !1;
                         switch (e.key) {
                             case "Enter":
                                 "update" in this.data && this.sendMessage("->", [this.rows[this.redit][this.data.headers[this.cedit]],
                                     [this.redit, this.cedit]
                                 ]), t = !0;
                             case "ArrowRight":
@@ -1153,25 +1187,25 @@
                                         a = typeof t.rows[e][this.cedit];
                                     "string" != a && "number" != a || (t.value = e), this.selected = [this.rows[e]]
                                 }
                                 break
                         }
                     },
                     complete(e, t, a) {
-                        z(this, [e, [this.redit, this.cedit]], (e => t((() => {
+                        A(this, [e, [this.redit, this.cedit]], (e => t((() => {
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        z(this, [t, this.search], (function(l) {
-                            if (!Array.isArray(l)) return h.error(l);
-                            p && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
+                        A(this, [t, this.search], (function(l) {
+                            if (!Array.isArray(l)) return u.error(l);
+                            g && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "+")
                     },
                     showSelected() {
                         let e = this.$refs.table;
@@ -1190,29 +1224,29 @@
                     switchMode() {
                         this.singleMode = !this.singleMode, this.singleMode && this.selected.length > 1 && this.selected.splice(1)
                     },
                     switchEdit() {
                         this.editMode = !this.editMode, this.sendMessage("!", this.editMode), this.editMode && !this.singleMode && this.switchMode()
                     },
                     delSelected() {
-                        if (!this.selected.length) return void h.error("Rows are not selected!");
+                        if (!this.selected.length) return void u.error("Rows are not selected!");
                         this.sendMessage("-", this.value);
                         let e = this.data.rows;
                         if (this.singleMode) e.splice(this.selected[0].iiid, 1);
                         else {
                             this.selected.length > 1 && this.selected.sort(((e, t) => t.iiid - e.iiid));
                             for (let t of this.selected) e.splice(t.iiid, 1)
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        Ae(this.updated, this.selected) || (this.sendMessage("=", this.selected.length ? this.selected[0].iiid : null), this.updated = this.selected), t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
+                        Ze(this.updated, this.selected) || (this.sendMessage("=", this.selected.length ? this.selected[0].iiid : null), this.updated = this.selected), t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
                     }
                 },
                 computed: {
                     redit() {
                         return console.log("redit", this.editMode && this.selected.length ? this.selected[0].iiid : null), this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
@@ -1233,52 +1267,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var Me = a(9267),
+            var De = a(9267),
                 $e = a(4842),
-                De = a(8870),
-                Ve = a(2165),
-                Oe = a(8186),
+                Ve = a(8870),
+                Oe = a(2165),
+                Qe = a(8186),
                 We = a(2414),
-                Qe = a(3884),
-                He = a(5735),
-                Ee = a(7208);
-            const Ne = (0, N.Z)(Ze, [
-                    ["render", je]
+                He = a(3884),
+                Ee = a(5735),
+                Ue = a(7208);
+            const Ne = (0, N.Z)(Me, [
+                    ["render", ze]
                 ]),
-                Ue = Ne;
-            I()(Ze, "components", {
-                QTable: Me.Z,
+                Fe = Ne;
+            R()(Me, "components", {
+                QTable: De.Z,
                 QInput: $e.Z,
                 QIcon: P.Z,
-                QTooltip: De.Z,
-                QBtn: Ve.Z,
-                QTr: Oe.Z,
+                QTooltip: Ve.Z,
+                QBtn: Oe.Z,
+                QTr: Qe.Z,
                 QTh: We.Z,
-                QTd: Qe.Z,
-                QCheckbox: He.Z,
-                QSelect: Ee.Z
+                QTd: He.Z,
+                QCheckbox: Ee.Z,
+                QSelect: Ue.Z
             });
-            const Fe = ["nodes", "edges"];
+            const Ke = ["nodes", "edges"];
 
             function Pe(e, t, a, i, o, n) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Fe)
+                }, null, 12, Ke)
             }
-            var Ke = a(2393),
-                Te = a.n(Ke);
-            const Ie = Te().stylesheet().selector("node").css({
+            var Te = a(2393),
+                Ie = a.n(Te);
+            const Re = Ie().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555"
                 }).selector("node[label]").css({
                     label: "data(label)",
@@ -1297,45 +1331,45 @@
                 }).selector("edge[label]").css({
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray"
                 }),
-                Re = {
+                Be = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Be(e, t) {
+            function Le(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id) return !0;
                 return !1
             }
-            const Le = (0, l.aZ)({
+            const Ye = (0, l.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Ie,
-                            layoutOptions: Re,
+                            style: Re,
+                            layoutOptions: Be,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: []
                         }
                     },
                     mounted() {
-                        let e = Te()({
+                        let e = Ie()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1383,15 +1417,15 @@
                         },
                         value() {
                             return this.data.value
                         }
                     },
                     methods: {
                         sendMessage(e, t) {
-                            C([this.pdata["name"], this.data["name"], e, t])
+                            q([this.pdata["name"], this.data["name"], e, t])
                         },
                         showClusterNode(e) {
                             const t = e.data("cluster"),
                                 a = this.cy.nodes(`[cluster='${t}']`),
                                 l = this.cy.nodes(`#${t}`);
                             l.data("isClusterNode", !0), l.animate({
                                 position: {
@@ -1450,15 +1484,15 @@
                             }
                         },
                         data: {
                             handler(e, t) {
                                 console.log("wa gr");
                                 let a = e.value,
                                     l = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Be(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Be(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Le(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Le(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1475,43 +1509,43 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Ye = (0, N.Z)(Le, [
+                Xe = (0, N.Z)(Ye, [
                     ["render", Pe]
                 ]),
-                Xe = Ye;
+                Ge = Xe;
 
-            function Ge(e, t, a, i, o, n) {
+            function Je(e, t, a, i, o, n) {
                 const d = (0, l.up)("v-chart");
                 return (0, l.wg)(), (0, l.j4)(d, {
                     ref: "chart",
                     option: o.options,
                     style: (0, s.j5)(a.styleSize),
                     autoresize: !0,
                     onClick: n.clicked
                 }, null, 8, ["option", "style", "onClick"])
             }
-            var Je = a(5512),
-                et = a(4447),
-                tt = a(1006),
-                at = a(3526),
-                lt = a(763),
-                st = a(546),
-                it = a(6902),
-                ot = a(2826),
-                nt = a(5256),
-                dt = a(3825),
-                rt = a(8825);
-            (0, lt.D)([et.N, tt.N, at.N]), (0, lt.D)([st.N, it.N, ot.N, nt.N, dt.N]);
-            let ct = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
-                ht = {
+            var et = a(5512),
+                tt = a(4447),
+                at = a(1006),
+                lt = a(3526),
+                st = a(763),
+                it = a(546),
+                ot = a(6902),
+                nt = a(2826),
+                dt = a(5256),
+                rt = a(3825),
+                ct = a(8825);
+            (0, st.D)([tt.N, at.N, lt.N]), (0, st.D)([it.N, ot.N, nt.N, dt.N, rt.N]);
+            let ht = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
+                ut = {
                     responsive: !0,
                     maintainAspectRatio: !1,
                     legend: {
                         data: [],
                         bottom: 10
                     },
                     tooltip: {
@@ -1546,26 +1580,26 @@
                         end: 10
                     }, {
                         start: 0,
                         end: 10
                     }],
                     series: []
                 };
-            const ut = {
+            const pt = {
                     name: "linechart",
                     components: {
-                        VChart: Je.ZP
+                        VChart: et.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, rt.Z)();
+                        const e = (0, ct.Z)();
                         return {
                             $q: e,
                             model: !1,
                             options: null
                         }
                     },
                     methods: {
@@ -1594,83 +1628,83 @@
                             let s = [];
                             for (let o = 0; o < l.length; o++) l[o] = "i" == l[o] ? -1 : parseInt(l[o]), s.push([]), o && (this.options.series.push({
                                 name: t[l[o]],
                                 type: "line",
                                 symbol: "none",
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: ct[o]
+                                    color: ht[o]
                                 },
                                 data: s[o]
                             }), this.options.legend.data.push(t[l[o]]));
                             this.options.xAxis.data = s[0];
                             let i = this.data.rows;
                             for (let o = 0; o < i.length; o++)
                                 for (let e = 0; e < l.length; e++) s[e].push(-1 == l[e] ? o : i[o][l[e]]);
                             this.$refs.chart.setOption(this.options)
                         }
                     },
                     mounted() {
-                        this.options = (0, c.cloneDeep)(ht), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
+                        this.options = (0, h.cloneDeep)(ut), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
                     },
                     watch: {}
                 },
-                pt = (0, N.Z)(ut, [
-                    ["render", Ge]
+                gt = (0, N.Z)(pt, [
+                    ["render", Je]
                 ]),
-                gt = pt;
+                mt = gt;
 
-            function mt(e) {
+            function ft(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const ft = (0, l.aZ)({
+            const wt = (0, l.aZ)({
                 name: "element",
                 components: {
-                    utable: Ue,
-                    cgraph: Xe,
-                    linechart: gt
+                    utable: Fe,
+                    cgraph: Ge,
+                    linechart: mt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
                     },
                     sendMessage(e, t) {
-                        C([this.pdata["name"], this.data["name"], e, t])
+                        q([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("->", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
-                        t && (this.sendMessage("=", e.files[t - 1].name), O())
+                        t && (this.sendMessage("=", e.files[t - 1].name), Q())
                     },
                     sendValue() {
                         this.sendMessage("=", this.value)
                     },
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
                         console.log(e), this.value = e
                     },
                     complete(e, t, a) {
-                        this.value = e, z(this, e, (e => t((() => {
+                        this.value = e, A(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
-                        h.lens(this.data)
+                        u.lens(this.data)
                     },
                     toggleCamera() {
                         this.isCameraOpen ? (this.isCameraOpen = !1, this.isPhotoTaken = !1, this.isShotPhoto = !1, this.stopCameraStream()) : (this.isCameraOpen = !0, this.createCameraElement())
                     },
                     createCameraElement() {
                         this.isLoading = !0;
                         const e = window.constraints = {
@@ -1698,15 +1732,15 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(mt, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(ft, "image/jpeg")
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
                         let t = this.type;
                         const a = "docviewer" == t || "graph" == t || "linechart" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
                             l = e.getBoundingClientRect();
@@ -1718,15 +1752,15 @@
                             top: l.top,
                             scrollHeight: a.scrollHeight,
                             scrollWidth: a.scrollWidth
                         }
                     }
                 },
                 mounted() {
-                    b[this.fullname] = this, p && console.log("mounted", this.fullname)
+                    k[this.fullname] = this, g && console.log("mounted", this.fullname)
                 },
                 data() {
                     return {
                         value: this.data.value,
                         styleSize: y(this.data),
                         options: [],
                         expandedKeys: [],
@@ -1827,64 +1861,65 @@
                     pdata: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     value(e, t) {
-                        "tree" == this.type && this.data.options[e] == t && this.expandedKeys.indexOf(t) < 0 && this.expandedKeys.push(t), e !== this.updated && (p && console.log("value changed", e, t), this.sendValue(), this.updated = e)
+                        "tree" == this.type && this.data.options[e] == t && this.expandedKeys.indexOf(t) < 0 && this.expandedKeys.push(t), e !== this.updated && (g && console.log("value changed", e, t), this.sendValue(), this.updated = e)
                     },
                     selection(e) {
-                        p && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
+                        g && console.log("selection changed", e, this.$refs.inputRef), Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        p && console.log("data update", this.fullname, t.name), this.styleSize || (this.styleSize = y(this.data), p && console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, b[this.fullname] = this
+                        g && console.log("data update", this.fullname, t.name), this.styleSize || (this.styleSize = y(this.data), g && console.log(`${this.name} size changed`)), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
                     }
                 }
             });
             var yt = a(4027),
-                wt = a(9721),
-                bt = a(8886),
-                kt = a(8761),
-                vt = a(1232),
-                xt = a(5551),
-                Ct = a(5869),
-                qt = a(1745);
-            const _t = (0, N.Z)(ft, [
-                    ["render", Ce],
-                    ["__scopeId", "data-v-0593ed42"]
+                bt = a(9721),
+                kt = a(8886),
+                vt = a(8761),
+                xt = a(1232),
+                Ct = a(5551),
+                qt = a(5869),
+                _t = a(1745);
+            const jt = (0, N.Z)(wt, [
+                    ["render", qe],
+                    ["__scopeId", "data-v-606d07c3"]
                 ]),
-                St = _t;
-            I()(ft, "components", {
+                St = jt;
+            R()(wt, "components", {
                 QImg: yt.Z,
                 QIcon: P.Z,
-                QSelect: Ee.Z,
-                QBadge: wt.Z,
-                QCheckbox: He.Z,
-                QToggle: bt.Z,
-                QBtnToggle: kt.Z,
+                QSelect: Ue.Z,
+                QBadge: bt.Z,
+                QCheckbox: Ee.Z,
+                QToggle: kt.Z,
+                QBtnToggle: vt.Z,
                 QInput: $e.Z,
-                QScrollArea: vt.Z,
-                QTree: xt.Z,
-                QSeparator: Ct.Z,
-                QUploader: qt.Z,
-                QBtn: Ve.Z
+                QScrollArea: xt.Z,
+                QTree: Ct.Z,
+                QSeparator: qt.Z,
+                QUploader: _t.Z,
+                QBtn: Oe.Z,
+                QTooltip: Ve.Z
             });
-            const jt = (0, l.aZ)({
+            const zt = (0, l.aZ)({
                 name: "block",
                 components: {
                     element: St
                 },
                 data() {
                     return {
-                        styleSize: f,
+                        styleSize: w,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
                             opacity: .75
                         },
@@ -1895,15 +1930,15 @@
                             width: "8px",
                             opacity: .2
                         }
                     }
                 },
                 methods: {
                     log() {
-                        console.log(Object.keys(w).length, this.name, this.$el.getBoundingClientRect())
+                        console.log(Object.keys(b).length, this.name, this.$el.getBoundingClientRect())
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         const t = e.querySelector(".q-scrollarea"),
                             a = e.getBoundingClientRect();
                         return {
                             el: e,
@@ -1913,15 +1948,15 @@
                             top: a.top,
                             scrollHeight: window.innerHeight,
                             scrollWidth: window.innerWidth
                         }
                     }
                 },
                 mounted() {
-                    w[this.name] = this, this.expanding && (b[this.fullname] = this)
+                    b[this.name] = this, this.expanding && (k[this.fullname] = this)
                 },
                 computed: {
                     name() {
                         return this.data.name
                     },
                     fullname() {
                         return `_scroll@${this.name}`
@@ -1943,55 +1978,55 @@
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        p && console.log("data update", this.name), this.styleSize = f, w[this.name] = this, this.expanding && (b[this.fullname] = this)
+                        g && console.log("data update", this.name), this.styleSize = w, b[this.name] = this, this.expanding && (k[this.fullname] = this)
                     }
                 }
             });
-            var zt = a(151);
-            const At = (0, N.Z)(jt, [
-                    ["render", ie]
+            var At = a(151);
+            const Zt = (0, N.Z)(zt, [
+                    ["render", oe]
                 ]),
-                Zt = At;
-            I()(jt, "components", {
-                QCard: zt.Z,
+                Mt = Zt;
+            R()(zt, "components", {
+                QCard: At.Z,
                 QIcon: P.Z,
-                QScrollArea: vt.Z
+                QScrollArea: xt.Z
             });
-            const Mt = (0, l.aZ)({
+            const Dt = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: Zt
+                        block: Mt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, l.Y3)((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
                                     W()
                                 }))
                             }))
                         }))
                     }
                 }),
-                $t = (0, N.Z)(Mt, [
-                    ["render", G]
+                $t = (0, N.Z)(Dt, [
+                    ["render", J]
                 ]),
-                Dt = $t,
-                Vt = {
+                Vt = $t,
+                Ot = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Ot(e, t, a, i, o, n) {
+            function Qt(e, t, a, i, o, n) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
@@ -2007,15 +2042,15 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", Vt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", Ot, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
@@ -2024,23 +2059,23 @@
             }
             const Wt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: Zt
+                    block: Mt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
-                        this.data.internal || C([this.data["name"], e]), this.hide()
+                        this.data.internal || q([this.data["name"], e]), this.hide()
                     },
                     hide() {
                         this.$refs.dialog.hide()
                     },
                     onDialogHide() {
                         this.$emit("hide")
                     },
@@ -2048,62 +2083,66 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Qt = a(5926),
-                Ht = a(2025);
-            const Et = (0, N.Z)(Wt, [
-                    ["render", Ot]
+            var Ht = a(5926),
+                Et = a(2025);
+            const Ut = (0, N.Z)(Wt, [
+                    ["render", Qt]
                 ]),
-                Nt = Et;
-            I()(Wt, "components", {
-                QDialog: Qt.Z,
-                QCard: zt.Z,
-                QItemLabel: K.Z,
-                QSpace: Ht.Z,
-                QBtn: Ve.Z
+                Nt = Ut;
+            R()(Wt, "components", {
+                QDialog: Ht.Z,
+                QCard: At.Z,
+                QItemLabel: T.Z,
+                QSpace: Et.Z,
+                QBtn: Oe.Z
             });
-            var Ut = !0;
-            let Ft = null;
+            var Ft = !0;
+            let Kt = null;
             const Pt = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
+                        data: {
+                            name: "toolbar"
+                        },
                         localServer: !0,
                         statusConnect: !1,
                         screen: {
                             blocks: []
                         }
                     }
                 },
                 components: {
-                    menubar: B,
-                    zone: Dt
+                    menubar: L,
+                    zone: Vt,
+                    element: St
                 },
                 created() {
-                    v(this)
+                    C(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
-                        C(["root", e])
+                        q(["root", e])
                     },
                     onResize(e) {
-                        p && console.log("window has been resized", window.innerHeight, window.innerWidth), O()
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), Q()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
@@ -2129,82 +2168,82 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Ft ? (l = {
+                        "progress" == t ? null == Kt ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Ft = this.$q.notify(l)) : null == e ? (Ft(), Ft = null) : (l = {
+                        }, Kt = this.$q.notify(l)) : null == e ? (Kt(), Kt = null) : (l = {
                             caption: e
-                        }, Ft(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, Kt(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if (Ut) Ut = !1, this.menu = e[0].map((e => ({
+                        if (Ft) Ft = !1, this.menu = e[0].map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
-                        }))), this.screen = e[1], this.tab = this.screen.name, p && console.log("init loading..");
-                        else if ("screen" == e.type) this.screen.name != e.name && j(), A(), this.screen = e;
+                        }))), this.screen = e[1], this.tab = this.screen.name, g && console.log("init loading..");
+                        else if ("screen" == e.type) this.screen.name != e.name && z(), Z(), this.screen = e;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
                             t.component = Nt, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
                         } else if (e.hasOwnProperty("answer")) $(e);
                         else {
-                            e.update && M(e);
+                            e.update && D(e);
                             let t = !1;
-                            for (let a of k) a in e && (this.notify(e[a], a), t = !0);
+                            for (let a of v) a in e && (this.notify(e[a], a), t = !0);
                             t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Ft && !e.progress && this.notify(null, "progress")
+                        Kt && !e.progress && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
-            var Kt = a(9214),
-                Tt = a(3812),
-                It = a(9570),
-                Rt = a(7547),
-                Bt = a(3269),
-                Lt = a(2652),
-                Yt = a(4379);
-            const Xt = (0, N.Z)(Pt, [
-                    ["render", o]
+            var Tt = a(9214),
+                It = a(3812),
+                Rt = a(9570),
+                Bt = a(7547),
+                Lt = a(3269),
+                Yt = a(2652),
+                Xt = a(4379);
+            const Gt = (0, N.Z)(Pt, [
+                    ["render", n]
                 ]),
-                Gt = Xt;
-            I()(Pt, "components", {
-                QLayout: Kt.Z,
-                QHeader: Tt.Z,
-                QToolbar: It.Z,
-                QBtn: Ve.Z,
-                QItemLabel: K.Z,
-                QTabs: Rt.Z,
-                QTab: Bt.Z,
-                QPageContainer: Lt.Z,
-                QPage: Yt.Z
+                Jt = Gt;
+            R()(Pt, "components", {
+                QLayout: Tt.Z,
+                QHeader: It.Z,
+                QToolbar: Rt.Z,
+                QBtn: Oe.Z,
+                QItemLabel: T.Z,
+                QTabs: Bt.Z,
+                QTab: Lt.Z,
+                QPageContainer: Yt.Z,
+                QPage: Xt.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.5.4/unigui/web/js/430.591e9a73.js` & `unigui-1.6.0/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/js/app.6ab35062.js` & `unigui-1.6.0/unigui/web/js/app.09b50726.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(361)]).then(r.bind(r, 361)),
+                        component: () => Promise.all([r.e(736), r.e(622)]).then(r.bind(r, 6622)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -44,30 +44,30 @@
                                     top: 0
                                 }),
                                 routes: v,
                                 history: e("")
                             });
                         return t
                     }));
-                async function g(e, t) {
+                async function b(e, t) {
                     const r = "function" === typeof m ? await m({}) : m,
                         n = e(d);
                     return n.use(o.Z, t), {
                         app: n,
                         router: r
                     }
                 }
-                var b = r(6417),
+                var g = r(6417),
                     y = r(5597);
                 const w = {
                         config: {
                             notify: {}
                         },
                         plugins: {
-                            Notify: b.Z,
+                            Notify: g.Z,
                             Dialog: y.Z
                         }
                     },
                     O = "";
                 async function k({
                     app: e,
                     router: t
@@ -94,15 +94,15 @@
                             urlPath: i,
                             publicPath: O
                         })
                     } catch (l) {
                         return l && l.url ? void a(l.url) : void console.error("[Quasar] boot error:", l)
                     }!0 !== n && (e.use(t), e.mount("#q-app"))
                 }
-                g(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
+                b(n.ri, w).then((e => Promise.all([Promise.resolve().then(r.bind(r, 2390))]).then((t => {
                     const r = t.map((e => e.default)).filter((e => "function" === typeof e));
                     k(e, r)
                 }))))
             },
             2390: (e, t, r) => {
                 r.r(t), r.d(t, {
                     default: () => o
@@ -159,24 +159,24 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            361: "78add75c",
-            430: "591e9a73"
+            430: "591e9a73",
+            622: "b0e2d91a"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            361: "c9159919",
+            622: "13cee13e",
             736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                361: 1
+                622: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.5.4/unigui/web/js/193.283445be.js` & `unigui-1.6.0/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.6.0/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/unigui/web/index.html` & `unigui-1.6.0/unigui/web/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.6ab35062.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.09b50726.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.5.4/LICENSE` & `unigui-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.5.4/setup.py` & `unigui-1.6.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.5.4',      
+      version='1.6.0',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.5.4/PKG-INFO` & `unigui-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.5.4
+Version: 1.6.0
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -51,19 +51,19 @@
         Select('Select', value='All', options=['All','Based','Group'])
     ], table, icon = 'api')
 ```
 
 | Screen global variables |	Status | Description |
 | :---: | :---: | :---: | 
 | name  | Has to be defined | Unique screen name |
-| order | Has to be defined | order in the program menu |
 | blocks | Has to be defined | which blocks to show on the screen |
 | user   | Always defined, read-only | Access to User(inherited) class which associated with a current user |
 | header | Optional | show it instead of app name |
 | toolbar | Optional | Gui elements to show in the screen toolbar |
+| order | Optional | order in the program menu |
 | icon  | Optional | MD icon of screen to show in screen menu |
 | dispatch | Optional | Screen handlers for catching gui signals. Has signature def dispatch(gui, signal) |
 | prepare | Optional | Syncronizes GUI elements one to another and with the program/system data. If defined then is called before screen appearing has a signature 'def prepare()' |
 
 
 ### Server start ###
 tests/run_hello.py
```

### Comparing `unigui-1.5.4/README.md` & `unigui-1.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -39,19 +39,19 @@
         Select('Select', value='All', options=['All','Based','Group'])
     ], table, icon = 'api')
 ```
 
 | Screen global variables |	Status | Description |
 | :---: | :---: | :---: | 
 | name  | Has to be defined | Unique screen name |
-| order | Has to be defined | order in the program menu |
 | blocks | Has to be defined | which blocks to show on the screen |
 | user   | Always defined, read-only | Access to User(inherited) class which associated with a current user |
 | header | Optional | show it instead of app name |
 | toolbar | Optional | Gui elements to show in the screen toolbar |
+| order | Optional | order in the program menu |
 | icon  | Optional | MD icon of screen to show in screen menu |
 | dispatch | Optional | Screen handlers for catching gui signals. Has signature def dispatch(gui, signal) |
 | prepare | Optional | Syncronizes GUI elements one to another and with the program/system data. If defined then is called before screen appearing has a signature 'def prepare()' |
 
 
 ### Server start ###
 tests/run_hello.py
```

### Comparing `unigui-1.5.4/unigui.egg-info/PKG-INFO` & `unigui-1.6.0/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.5.4
+Version: 1.6.0
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -51,19 +51,19 @@
         Select('Select', value='All', options=['All','Based','Group'])
     ], table, icon = 'api')
 ```
 
 | Screen global variables |	Status | Description |
 | :---: | :---: | :---: | 
 | name  | Has to be defined | Unique screen name |
-| order | Has to be defined | order in the program menu |
 | blocks | Has to be defined | which blocks to show on the screen |
 | user   | Always defined, read-only | Access to User(inherited) class which associated with a current user |
 | header | Optional | show it instead of app name |
 | toolbar | Optional | Gui elements to show in the screen toolbar |
+| order | Optional | order in the program menu |
 | icon  | Optional | MD icon of screen to show in screen menu |
 | dispatch | Optional | Screen handlers for catching gui signals. Has signature def dispatch(gui, signal) |
 | prepare | Optional | Syncronizes GUI elements one to another and with the program/system data. If defined then is called before screen appearing has a signature 'def prepare()' |
 
 
 ### Server start ###
 tests/run_hello.py
```

### Comparing `unigui-1.5.4/unigui.egg-info/SOURCES.txt` & `unigui-1.6.0/unigui.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/361.c9159919.css
+unigui/web/css/622.13cee13e.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -27,11 +27,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
-unigui/web/js/361.78add75c.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/app.6ab35062.js
+unigui/web/js/622.b0e2d91a.js
+unigui/web/js/app.09b50726.js
 unigui/web/js/vendor.3e8714c2.js
```

