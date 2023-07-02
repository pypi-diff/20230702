# Comparing `tmp/reflex_ui-0.1.0.tar.gz` & `tmp/reflex_ui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_ui-0.1.0.tar", max compression
+gzip compressed data, was "reflex_ui-0.1.1.tar", max compression
```

## Comparing `reflex_ui-0.1.0.tar` & `reflex_ui-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1075 2023-05-27 11:53:20.000000 reflex_ui-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-05-27 11:53:20.000000 reflex_ui-0.1.0/README.md
--rw-r--r--   0        0        0      828 2023-07-01 11:26:55.436671 reflex_ui-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      110 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/__init__.py
--rw-r--r--   0        0        0     4932 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/app.py
--rw-r--r--   0        0        0    15247 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/app_server.py
--rw-r--r--   0        0        0     1530 2023-06-01 16:08:46.937561 reflex_ui-0.1.0/reflex/assets.py
--rw-r--r--   0        0        0     2480 2023-07-01 11:18:43.746669 reflex_ui-0.1.0/reflex/common.py
--rw-r--r--   0        0        0       47 2023-06-02 09:45:54.484185 reflex_ui-0.1.0/reflex/errors.py
--rw-r--r--   0        0        0    36711 2023-07-01 11:19:53.366669 reflex_ui-0.1.0/reflex/generated/app.js
--rw-r--r--   0        0        0    80467 2023-07-01 11:19:53.390002 reflex_ui-0.1.0/reflex/generated/app.js.map
--rw-r--r--   0        0        0      287 2023-07-01 11:19:51.620002 reflex_ui-0.1.0/reflex/generated/index.html
--rw-r--r--   0        0        0     4372 2023-07-01 11:19:52.343336 reflex_ui-0.1.0/reflex/generated/style.css
--rw-r--r--   0        0        0     7603 2023-07-01 11:19:52.346669 reflex_ui-0.1.0/reflex/generated/style.css.map
--rw-r--r--   0        0        0    75209 2022-04-21 09:32:25.000000 reflex_ui-0.1.0/reflex/hosted-assets/showdown.min.js
--rw-r--r--   0        0        0     2521 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/image_source.py
--rw-r--r--   0        0        0     1229 2023-06-02 09:31:52.003332 reflex_ui-0.1.0/reflex/messages.py
--rw-r--r--   0        0        0    38973 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/session.py
--rw-r--r--   0        0        0      121 2023-05-28 09:40:21.000000 reflex_ui-0.1.0/reflex/styling/__init__.py
--rw-r--r--   0        0        0     3648 2023-06-01 11:11:54.202507 reflex_ui-0.1.0/reflex/styling/box_style.py
--rw-r--r--   0        0        0     9391 2023-06-16 18:28:59.043338 reflex_ui-0.1.0/reflex/styling/color.py
--rw-r--r--   0        0        0     2874 2023-05-28 09:43:35.000000 reflex_ui-0.1.0/reflex/styling/fills.py
--rw-r--r--   0        0        0     2671 2023-05-28 16:11:56.000000 reflex_ui-0.1.0/reflex/styling/markdown_style.py
--rw-r--r--   0        0        0     1760 2023-05-28 16:11:33.000000 reflex_ui-0.1.0/reflex/styling/text_style.py
--rw-r--r--   0        0        0      274 2023-05-30 05:41:43.000000 reflex_ui-0.1.0/reflex/theme.py
--rw-r--r--   0        0        0    12670 2023-06-18 14:30:30.191229 reflex_ui-0.1.0/reflex/validator.py
--rw-r--r--   0        0        0      467 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/widgets/__init__.py
--rw-r--r--   0        0        0     2424 2023-07-01 11:10:37.780000 reflex_ui-0.1.0/reflex/widgets/auto_form.py
--rw-r--r--   0        0        0     8539 2023-06-19 07:57:40.933773 reflex_ui-0.1.0/reflex/widgets/button.py
--rw-r--r--   0        0        0     1630 2023-06-19 07:57:40.933773 reflex_ui-0.1.0/reflex/widgets/column.py
--rw-r--r--   0        0        0      226 2023-05-27 11:53:20.000000 reflex_ui-0.1.0/reflex/widgets/container.py
--rw-r--r--   0        0        0     1828 2023-06-10 18:22:34.826680 reflex_ui-0.1.0/reflex/widgets/dropdown.py
--rw-r--r--   0        0        0      507 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/widgets/image.py
--rw-r--r--   0        0        0     1175 2023-06-09 18:12:36.907709 reflex_ui-0.1.0/reflex/widgets/markdown_view.py
--rw-r--r--   0        0        0      552 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/widgets/media_player.py
--rw-r--r--   0        0        0      724 2023-06-18 14:35:53.924200 reflex_ui-0.1.0/reflex/widgets/metadata.py
--rw-r--r--   0        0        0     3524 2023-06-10 18:04:23.870009 reflex_ui-0.1.0/reflex/widgets/mouse_event_listener.py
--rw-r--r--   0        0        0      484 2023-06-14 20:50:37.701043 reflex_ui-0.1.0/reflex/widgets/plot.py
--rw-r--r--   0        0        0     1758 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/widgets/progress_circle.py
--rw-r--r--   0        0        0      533 2023-06-09 18:05:31.920936 reflex_ui-0.1.0/reflex/widgets/rectangle.py
--rw-r--r--   0        0        0     1648 2023-06-19 07:57:40.933773 reflex_ui-0.1.0/reflex/widgets/row.py
--rw-r--r--   0        0        0      242 2023-05-27 11:53:20.000000 reflex_ui-0.1.0/reflex/widgets/stack.py
--rw-r--r--   0        0        0     1567 2023-06-11 11:50:08.153416 reflex_ui-0.1.0/reflex/widgets/switch.py
--rw-r--r--   0        0        0      363 2023-05-28 16:37:28.000000 reflex_ui-0.1.0/reflex/widgets/text.py
--rw-r--r--   0        0        0     1895 2023-06-21 05:55:32.753397 reflex_ui-0.1.0/reflex/widgets/text_input.py
--rw-r--r--   0        0        0    20730 2023-07-01 11:08:44.473333 reflex_ui-0.1.0/reflex/widgets/widget_base.py
--rw-r--r--   0        0        0     3891 2023-06-11 10:23:10.760064 reflex_ui-0.1.0/reflex/world_units.py
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 reflex_ui-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-27 11:53:20.000000 reflex_ui-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-05-27 11:53:20.000000 reflex_ui-0.1.1/README.md
+-rw-r--r--   0        0        0      944 2023-07-02 17:23:41.010505 reflex_ui-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/__init__.py
+-rw-r--r--   0        0        0     4932 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/app.py
+-rw-r--r--   0        0        0    15243 2023-07-02 17:23:24.247163 reflex_ui-0.1.1/reflex/app_server.py
+-rw-r--r--   0        0        0     1530 2023-06-01 16:08:46.937561 reflex_ui-0.1.1/reflex/assets.py
+-rw-r--r--   0        0        0     2480 2023-07-02 17:23:24.247163 reflex_ui-0.1.1/reflex/common.py
+-rw-r--r--   0        0        0       47 2023-06-02 09:45:54.484185 reflex_ui-0.1.1/reflex/errors.py
+-rw-r--r--   0        0        0    36522 2023-07-02 17:49:31.901177 reflex_ui-0.1.1/reflex/generated/app.js
+-rw-r--r--   0        0        0    80229 2023-07-02 17:49:31.924510 reflex_ui-0.1.1/reflex/generated/app.js.map
+-rw-r--r--   0        0        0      287 2023-07-02 17:49:30.104509 reflex_ui-0.1.1/reflex/generated/index.html
+-rw-r--r--   0        0        0     4350 2023-07-02 17:49:30.834510 reflex_ui-0.1.1/reflex/generated/style.css
+-rw-r--r--   0        0        0     7562 2023-07-02 17:49:30.837843 reflex_ui-0.1.1/reflex/generated/style.css.map
+-rw-r--r--   0        0        0    75209 2022-04-21 09:32:25.000000 reflex_ui-0.1.1/reflex/hosted-assets/showdown.min.js
+-rw-r--r--   0        0        0     2521 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/image_source.py
+-rw-r--r--   0        0        0     1229 2023-06-02 09:31:52.003332 reflex_ui-0.1.1/reflex/messages.py
+-rw-r--r--   0        0        0    39029 2023-07-02 17:50:56.407878 reflex_ui-0.1.1/reflex/session.py
+-rw-r--r--   0        0        0      121 2023-05-28 09:40:21.000000 reflex_ui-0.1.1/reflex/styling/__init__.py
+-rw-r--r--   0        0        0     3648 2023-06-01 11:11:54.202507 reflex_ui-0.1.1/reflex/styling/box_style.py
+-rw-r--r--   0        0        0     9391 2023-06-16 18:28:59.043338 reflex_ui-0.1.1/reflex/styling/color.py
+-rw-r--r--   0        0        0     2874 2023-05-28 09:43:35.000000 reflex_ui-0.1.1/reflex/styling/fills.py
+-rw-r--r--   0        0        0     2671 2023-05-28 16:11:56.000000 reflex_ui-0.1.1/reflex/styling/markdown_style.py
+-rw-r--r--   0        0        0     1760 2023-05-28 16:11:33.000000 reflex_ui-0.1.1/reflex/styling/text_style.py
+-rw-r--r--   0        0        0      274 2023-05-30 05:41:43.000000 reflex_ui-0.1.1/reflex/theme.py
+-rw-r--r--   0        0        0    12670 2023-06-18 14:30:30.191229 reflex_ui-0.1.1/reflex/validator.py
+-rw-r--r--   0        0        0      467 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/widgets/__init__.py
+-rw-r--r--   0        0        0     2424 2023-07-01 11:10:37.780000 reflex_ui-0.1.1/reflex/widgets/auto_form.py
+-rw-r--r--   0        0        0     8439 2023-07-02 17:50:56.411212 reflex_ui-0.1.1/reflex/widgets/button.py
+-rw-r--r--   0        0        0     1577 2023-07-02 17:50:56.411212 reflex_ui-0.1.1/reflex/widgets/column.py
+-rw-r--r--   0        0        0      226 2023-05-27 11:53:20.000000 reflex_ui-0.1.1/reflex/widgets/container.py
+-rw-r--r--   0        0        0     1828 2023-06-10 18:22:34.826680 reflex_ui-0.1.1/reflex/widgets/dropdown.py
+-rw-r--r--   0        0        0      507 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/widgets/image.py
+-rw-r--r--   0        0        0     1175 2023-06-09 18:12:36.907709 reflex_ui-0.1.1/reflex/widgets/markdown_view.py
+-rw-r--r--   0        0        0      552 2023-07-01 11:08:44.473333 reflex_ui-0.1.1/reflex/widgets/media_player.py
+-rw-r--r--   0        0        0      724 2023-06-18 14:35:53.924200 reflex_ui-0.1.1/reflex/widgets/metadata.py
+-rw-r--r--   0        0        0     3524 2023-06-10 18:04:23.870009 reflex_ui-0.1.1/reflex/widgets/mouse_event_listener.py
+-rw-r--r--   0        0        0      484 2023-06-14 20:50:37.701043 reflex_ui-0.1.1/reflex/widgets/plot.py
+-rw-r--r--   0        0        0     1665 2023-07-02 17:50:56.411212 reflex_ui-0.1.1/reflex/widgets/progress_circle.py
+-rw-r--r--   0        0        0      533 2023-06-09 18:05:31.920936 reflex_ui-0.1.1/reflex/widgets/rectangle.py
+-rw-r--r--   0        0        0     1594 2023-07-02 17:44:56.264397 reflex_ui-0.1.1/reflex/widgets/row.py
+-rw-r--r--   0        0        0      242 2023-05-27 11:53:20.000000 reflex_ui-0.1.1/reflex/widgets/stack.py
+-rw-r--r--   0        0        0     1567 2023-06-11 11:50:08.153416 reflex_ui-0.1.1/reflex/widgets/switch.py
+-rw-r--r--   0        0        0      363 2023-05-28 16:37:28.000000 reflex_ui-0.1.1/reflex/widgets/text.py
+-rw-r--r--   0        0        0     1895 2023-06-21 05:55:32.753397 reflex_ui-0.1.1/reflex/widgets/text_input.py
+-rw-r--r--   0        0        0    20757 2023-07-02 17:50:56.414545 reflex_ui-0.1.1/reflex/widgets/widget_base.py
+-rw-r--r--   0        0        0     3891 2023-06-11 10:23:10.760064 reflex_ui-0.1.1/reflex/world_units.py
+-rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 reflex_ui-0.1.1/PKG-INFO
```

### Comparing `reflex_ui-0.1.0/LICENSE.txt` & `reflex_ui-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/pyproject.toml` & `reflex_ui-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex-ui"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>", "Paul Pinterits"]
 readme = "README.md"
 packages = [{ include = "reflex" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -13,19 +13,22 @@
 uvicorn = "^0.22.0"
 uniserde = "^0.2.5"
 pillow = "^9.5.0"
 websocket = "^0.2.1"
 websockets = "^11.0.3"
 timer-dict = "^1.0.0"
 introspection = "^1.5.2"
-pywebview = "^4.1"
 aiohttp = "^3.8.4"
 python-multipart = "^0.0.6"
 plotly = "^5.15.0"
 pytest = "^7.3.1"
+cefpython3 = { version = "^66.1", platform = "windows" }
+pygobject = { version = "^3.44.1", platform = "linux" }
+pywebview = "^4.2.2"
+
 
 [tool.poetry.group.dev.dependencies]
 alt-pytest-asyncio = "^0.7.0"
 black = "^23.1.0"
 coverage = "^7.2.2"
 isort = "^5.12.0"
 pre-commit = "^3.1.1"
```

### Comparing `reflex_ui-0.1.0/reflex/app.py` & `reflex_ui-0.1.1/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/app_server.py` & `reflex_ui-0.1.1/reflex/app_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
-import functools
 import asyncio
-import reflex.widgets.metadata
-import plotly
+import functools
 import io
-import reflex as rx
 import json
 import secrets
 import traceback
 import weakref
 from datetime import timedelta
 from pathlib import Path
 from typing import *  # type: ignore
 
 import fastapi
+import plotly
 import timer_dict
 import uniserde
 from PIL import Image
 
+import reflex as rx
+import reflex.widgets.metadata
+
 from . import app, assets, common, messages, session, validator
 from .common import Jsonable
 
 __all__ = [
     "AppServer",
 ]
 
@@ -36,15 +37,15 @@
 
 @functools.lru_cache(maxsize=None)
 def read_frontend_template(template_name: str) -> str:
     """
     Read a text file from the frontend directory and return its content. The
     results are cached to avoid repeated disk access.
     """
-    return (common.GENREATED_DIR / template_name).read_text(encoding="utf-8")
+    return (common.GENERATED_DIR / template_name).read_text(encoding="utf-8")
 
 
 class AppServer(fastapi.FastAPI):
     def __init__(
         self,
         app_: app.App,
         external_url: str,
@@ -150,15 +151,15 @@
 
         # Fill in all placeholders
         js = js.replace("{session_token}", session_token)
         js = js.replace(
             '"{initial_messages}"',
             json.dumps(initial_messages, indent=4),
         )
-        js = js.replace("{}; // {child_attribute_names}", CHILD_ATTRIBUTE_NAMES_JSON)
+        js = js.replace('"{child_attribute_names}"', CHILD_ATTRIBUTE_NAMES_JSON)
 
         html = html.replace("{title}", self.app.name)
         html = html.replace("/*{style}*/", css)
         html = html.replace("/*{script}*/", js)
 
         # Respond
         return fastapi.responses.HTMLResponse(html)
```

### Comparing `reflex_ui-0.1.0/reflex/assets.py` & `reflex_ui-0.1.1/reflex/assets.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/common.py` & `reflex_ui-0.1.1/reflex/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+import enum
 import hashlib
-from dataclasses import dataclass
-import fastapi
-import traceback
 import inspect
-import enum
 import secrets
+import traceback
+from dataclasses import dataclass
 from pathlib import Path
 from typing import *  # type: ignore
-import uniserde
 
+import fastapi
+import uniserde
 from typing_extensions import Annotated
 
 _SECURE_HASH_SEED: bytes = secrets.token_bytes(32)
 
 
 PACKAGE_ROOT_DIR = Path(__file__).resolve().parent
-GENREATED_DIR = PACKAGE_ROOT_DIR / "generated"
+GENERATED_DIR = PACKAGE_ROOT_DIR / "generated"
 HOSTED_ASSETS_DIR = PACKAGE_ROOT_DIR / "hosted-assets"
 
 
 Jsonable: TypeAlias = uniserde.Jsonable
 
 
 _READONLY = object()
```

### Comparing `reflex_ui-0.1.0/reflex/generated/app.js` & `reflex_ui-0.1.1/reflex/generated/app.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -902,15 +902,15 @@
         "./widgetBase": "DUgK"
     }],
     "EVxB": [function(require, module, exports) {
         "use strict";
         var __assign = this && this.__assign || function() {
             return (__assign = Object.assign || function(e) {
                 for (var t, n = 1, i = arguments.length; n < i; n++)
-                    for (var o in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, o) && (e[o] = t[o]);
+                    for (var r in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, r) && (e[r] = t[r]);
                 return e
             }).apply(this, arguments)
         };
         Object.defineProperty(exports, "__esModule", {
             value: !0
         }), exports.sendMessageOverWebsocket = exports.replaceChildren = exports.replaceOnlyChild = exports.getParentWidgetElementExcludingInjected = exports.getParentWidgetElementIncludingInjected = exports.getInstanceByWidgetId = exports.getElementByWidgetId = exports.fillToCss = exports.colorToCss = exports.pixelsPerEm = void 0;
         var text_1 = require("./text"),
@@ -926,44 +926,44 @@
             progressCircle_1 = require("./progressCircle"),
             plot_1 = require("./plot"),
             align_1 = require("./align"),
             margin_1 = require("./margin"),
             mediaPlayer_1 = require("./mediaPlayer"),
             sessionToken = "{session_token}",
             initialMessages = "{initial_messages}",
-            CHILD_ATTRIBUTE_NAMES = {},
+            CHILD_ATTRIBUTE_NAMES = "{child_attribute_names}",
             socket = null;
         exports.pixelsPerEm = 16;
         var elementsToInstances = new WeakMap;
 
         function colorToCss(e) {
             var t = e[0],
                 n = e[1],
                 i = e[2],
-                o = e[3];
-            return "rgba(".concat(255 * t, ", ").concat(255 * n, ", ").concat(255 * i, ", ").concat(o, ")")
+                r = e[3];
+            return "rgba(".concat(255 * t, ", ").concat(255 * n, ", ").concat(255 * i, ", ").concat(r, ")")
         }
 
         function fillToCss(e) {
             if ("solid" === e.type) return colorToCss(e.color);
             if ("linearGradient" === e.type) {
                 if (1 == e.stops.length) return colorToCss(e.stops[0][0]);
                 for (var t = [], n = 0; n < e.stops.length; n++) {
                     var i = e.stops[n][0],
-                        o = e.stops[n][1];
-                    t.push("".concat(colorToCss(i), " ").concat(100 * o, "%"))
+                        r = e.stops[n][1];
+                    t.push("".concat(colorToCss(i), " ").concat(100 * r, "%"))
                 }
                 return "linear-gradient(".concat(e.angleDegrees, "deg, ").concat(t.join(", "), ")")
             }
             if ("image" === e.type) {
-                var r = "url('".concat(e.imageUrl, "')");
-                if ("fit" == e.fillMode) return "".concat(r, " center/contain no-repeat");
-                if ("stretch" == e.fillMode) return "".concat(r, " top left / 100% 100%");
-                if ("tile" == e.fillMode) return "".concat(r, " left top repeat");
-                if ("zoom" == e.fillMode) return "".concat(r, " center/cover no-repeat");
+                var o = "url('".concat(e.imageUrl, "')");
+                if ("fit" == e.fillMode) return "".concat(o, " center/contain no-repeat");
+                if ("stretch" == e.fillMode) return "".concat(o, " top left / 100% 100%");
+                if ("tile" == e.fillMode) return "".concat(o, " left top repeat");
+                if ("zoom" == e.fillMode) return "".concat(o, " center/cover no-repeat");
                 throw "Invalid fill mode for image fill: ".concat(e.type)
             }
             throw "Invalid fill type: ".concat(e.type)
         }
 
         function getElementByWidgetId(e) {
             var t = document.getElementById("reflex-id-".concat(e));
@@ -1025,107 +1025,107 @@
             if (null === n) return t;
             var i = elementsToInstances.get(n);
             return void 0 === i ? t : __assign(__assign({}, i.state), t)
         }
 
         function createLayoutWidgetStates(e, t, n) {
             var i = getCurrentWidgetState(e, t),
-                o = e,
-                r = i._margin_;
-            if (0 !== r[0] || 0 !== r[1] || 0 !== r[2] || 0 !== r[3]) {
-                var s = "".concat(e, "-margin");
-                n[s] = {
+                r = e,
+                o = i._margin_;
+            if (0 !== o[0] || 0 !== o[1] || 0 !== o[2] || 0 !== o[3]) {
+                var l = "".concat(e, "-margin");
+                n[l] = {
                     _type_: "Margin-builtin",
                     _python_type_: "Margin (injected)",
                     _size_: i._size_,
                     _grow_: i._grow_,
-                    child: o,
-                    margin_left: r[0],
-                    margin_top: r[1],
-                    margin_right: r[2],
-                    margin_bottom: r[3]
-                }, o = s
+                    child: r,
+                    margin_left: o[0],
+                    margin_top: o[1],
+                    margin_right: o[2],
+                    margin_bottom: o[3]
+                }, r = l
             }
-            var l = i._align_;
-            if (null !== l[0] || null !== l[1]) {
+            var s = i._align_;
+            if (null !== s[0] || null !== s[1]) {
                 var a = "".concat(e, "-align");
                 n[a] = {
                     _type_: "Align-builtin",
                     _python_type_: "Align (injected)",
                     _size_: i._size_,
                     _grow_: i._grow_,
-                    child: o,
-                    align_x: l[0],
-                    align_y: l[1]
-                }, o = a
+                    child: r,
+                    align_x: s[0],
+                    align_y: s[1]
+                }, r = a
             }
-            return o
+            return r
         }
 
         function replaceChildrenWithLayoutWidgets(e, t, n) {
             function i(e) {
                 return e.split("-")[0]
             }
-            for (var o = 0, r = CHILD_ATTRIBUTE_NAMES[e._type_] || []; o < r.length; o++) {
-                var s = r[o],
-                    l = e[s];
-                if (Array.isArray(l)) e[s] = l.map(function(e) {
+            for (var r = 0, o = CHILD_ATTRIBUTE_NAMES[e._type_] || []; r < o.length; r++) {
+                var l = o[r],
+                    s = e[l];
+                if (Array.isArray(s)) e[l] = s.map(function(e) {
                     return e = i(e.toString()), t.add(e), createLayoutWidgetStates(e, n[e] || {}, n)
                 });
-                else if (null !== l) {
-                    var a = i(l.toString());
-                    e[s] = createLayoutWidgetStates(a, n[a] || {}, n), t.add(a)
+                else if (null !== s) {
+                    var a = i(s.toString());
+                    e[l] = createLayoutWidgetStates(a, n[a] || {}, n), t.add(a)
                 }
             }
         }
 
         function preprocessMessage(e, t) {
             "number" == typeof t && (t = t.toString());
-            for (var n = Object.keys(e), i = new Set, o = 0, r = n; o < r.length; o++) {
-                replaceChildrenWithLayoutWidgets(e[a = r[o]], i, e)
+            for (var n = Object.keys(e), i = new Set, r = 0, o = n; r < o.length; r++) {
+                replaceChildrenWithLayoutWidgets(e[a = o[r]], i, e)
             }
-            for (var s = 0, l = n; s < l.length; s++) {
-                var a = l[s];
-                if (i.has(a)) console.log("Discarding ".concat(a, " because it is a child"));
-                else if (a !== t) {
-                    var d = document.getElementById("reflex-id-".concat(a));
-                    if (null !== d) {
-                        var c = getParentWidgetElementExcludingInjected(d);
-                        if (null !== c) {
-                            var g = elementsToInstances.get(c);
-                            if (void 0 === g) throw "Parent widget with id ".concat(c, " not found");
-                            var u = c.id.slice("reflex-id-".length),
-                                p = __assign({}, g.state);
-                            replaceChildrenWithLayoutWidgets(p, i, e), e[u] = p, console.log("Parent of ".concat(a, " is ").concat(u))
-                        } else console.log("Discarding ".concat(a, " because it has no parent"))
-                    } else console.log("Discarding ".concat(a, " because it is not in the DOM"))
-                } else t = createLayoutWidgetStates(a, e[a], e)
+            for (var l = 0, s = n; l < s.length; l++) {
+                var a = s[l];
+                if (!i.has(a))
+                    if (a !== t) {
+                        var d = document.getElementById("reflex-id-".concat(a));
+                        if (null !== d) {
+                            var c = getParentWidgetElementExcludingInjected(d);
+                            if (null !== c) {
+                                var g = elementsToInstances.get(c);
+                                if (void 0 === g) throw "Parent widget with id ".concat(c, " not found");
+                                var u = c.id.slice("reflex-id-".length),
+                                    p = __assign({}, g.state);
+                                replaceChildrenWithLayoutWidgets(p, i, e), e[u] = p
+                            }
+                        }
+                    } else t = createLayoutWidgetStates(a, e[a], e)
             }
-            return t
+            return console.log("new message", e), console.log(CHILD_ATTRIBUTE_NAMES), t
         }
 
         function updateWidgetStates(e, t) {
-            t = preprocessMessage(e, t), console.log(e);
+            t = preprocessMessage(e, t);
             var n = document.createElement("div");
             for (var i in document.body.appendChild(n), n.id = "reflex-latent-widgets", n.style.display = "none", e) {
-                var o = e[i],
-                    r = "reflex-id-".concat(i);
-                if (!(c = document.getElementById(r))) {
-                    var s = widgetClasses[o._type_];
-                    if (!s) throw "Encountered unknown widget type: ".concat(o._type_);
-                    (c = (g = new s(r, o)).createElement()).id = r, c.classList.add("reflex-widget"), c.setAttribute("dbg-py-class", o._python_type_);
-                    var l = o.key;
-                    void 0 !== l && c.setAttribute("dbg-key", "".concat(l)), elementsToInstances.set(c, g), n.appendChild(c)
+                var r = e[i],
+                    o = "reflex-id-".concat(i);
+                if (!(c = document.getElementById(o))) {
+                    var l = widgetClasses[r._type_];
+                    if (!l) throw "Encountered unknown widget type: ".concat(r._type_);
+                    (c = (g = new l(o, r)).createElement()).id = o, c.classList.add("reflex-widget"), c.setAttribute("dbg-py-class", r._python_type_);
+                    var s = r.key;
+                    void 0 !== s && c.setAttribute("dbg-key", "".concat(s)), elementsToInstances.set(c, g), n.appendChild(c)
                 }
             }
             var a = new Set;
             for (var d in e) {
                 var c, g;
-                o = e[d];
-                commonUpdate(c = getElementByWidgetId(d), o), (g = elementsToInstances.get(c)).updateElement(c, o), g.state = __assign(__assign({}, g.state), o), a.add(g);
+                r = e[d];
+                commonUpdate(c = getElementByWidgetId(d), r), (g = elementsToInstances.get(c)).updateElement(c, r), g.state = __assign(__assign({}, g.state), r), a.add(g);
                 var u = getParentWidgetElementIncludingInjected(c);
                 if (u) {
                     var p = elementsToInstances.get(u);
                     if (!p) throw "Failed to find parent widget for ".concat(d);
                     a.add(p)
                 }
             }
@@ -1147,52 +1147,52 @@
                 if (null !== t) {
                     var n = e.firstElementChild;
                     if (null !== n) {
                         if (n.id === "reflex-id-".concat(t)) return;
                         var i = document.getElementById("reflex-latent-widgets");
                         null == i || i.appendChild(n)
                     }
-                    var o = getElementByWidgetId(t);
-                    null == e || e.appendChild(o)
+                    var r = getElementByWidgetId(t);
+                    null == e || e.appendChild(r)
                 } else e.innerHTML = ""
         }
 
         function replaceChildren(e, t) {
             if (void 0 !== t)
-                for (var n = document.getElementById("reflex-latent-widgets"), i = e.firstElementChild, o = 0;;) {
+                for (var n = document.getElementById("reflex-latent-widgets"), i = e.firstElementChild, r = 0;;) {
                     if (null === i) {
-                        for (; o < t.length;) {
-                            var r = getElementByWidgetId(t[o]);
-                            e.appendChild(r), o++
+                        for (; r < t.length;) {
+                            var o = getElementByWidgetId(t[r]);
+                            e.appendChild(o), r++
                         }
                         break
                     }
-                    if (o >= t.length) {
+                    if (r >= t.length) {
                         for (; null !== i;) {
-                            var s = i.nextElementSibling;
-                            n.appendChild(i), i = s
+                            var l = i.nextElementSibling;
+                            n.appendChild(i), i = l
                         }
                         break
                     }
-                    var l = t[o];
-                    if (i.id !== "reflex-id-".concat(l)) {
-                        var a = getElementByWidgetId(l);
-                        e.insertBefore(a, i), o++
-                    } else i = i.nextElementSibling, o++
+                    var s = t[r];
+                    if (i.id !== "reflex-id-".concat(s)) {
+                        var a = getElementByWidgetId(s);
+                        e.insertBefore(a, i), r++
+                    } else i = i.nextElementSibling, r++
                 }
         }
 
         function requestFileUpload(e) {
             var t = document.createElement("input");
 
             function n() {
                 if (null !== t.parentElement) {
-                    for (var n = new FormData, i = 0, o = t.files || []; i < o.length; i++) {
-                        var r = o[i];
-                        1, n.append("file_names", r.name), n.append("file_types", r.type), n.append("file_sizes", r.size.toString()), n.append("file_streams", r, r.name)
+                    for (var n = new FormData, i = 0, r = t.files || []; i < r.length; i++) {
+                        var o = r[i];
+                        1, n.append("file_names", o.name), n.append("file_types", o.type), n.append("file_sizes", o.size.toString()), n.append("file_streams", o, o.name)
                     }
                     n.append("dummy", "dummy"), fetch(e.uploadUrl, {
                         method: "PUT",
                         body: n
                     }), t.remove()
                 }
             }
```

### Comparing `reflex_ui-0.1.0/reflex/generated/app.js.map` & `reflex_ui-0.1.1/reflex/generated/app.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9206349206349207%*

 * *Differences: {"'mappings'": "';AAuHkC,aAAA,IAAA,EAAA,MAAA,KAAA,UAAA,WAAA,OAAA,EAAA,OAAA,QAAA,SAAA,GAAA,IAAA,IAAA,EAAA,EAAA,EAAA,EAAA,UAAA,OAAA,EAAA,EAAA,IAAA,IAAA,IAAA,KAAA,EAAA,UAAA,GAAA,OAAA,UAAA,eAAA,KAAA,EAAA,KAAA,EAAA,GAAA,EAAA,IAAA,OAAA,IAAA,MAAA,KAAA,YAAA,OAAA,eAAA,QAAA,aAAA,CAAA,OAAA,IAAA,QAAA,gBAAA,EAvHlC,IAAA,EAAA,QAAA,SAeA,EAAA,WAKI,SAAA,EACI,EACA,GAEA,KAAK,UAAY,EACjB,KAAK,MAAQ,EACb,KAAK,oBAAsB,GA2FnC,OAtFI,OAAA,eAAI,EAAA,UAAA,UAAO,CAAX,IAAA,WACI,IAAI,EAAU,SAAS,eAAe,KAAK,WAE3C,GAAgB,OAAZ,EACA,MAAM,IAAI,MACN,g […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "app.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "../../frontend",
     "sources": [
         "widgetBase.ts",
         "text.ts",
         "row.ts",
         "column.ts",
@@ -35,11 +35,11 @@
         "import { getInstanceByWidgetId, replaceOnlyChild } from './app';\nimport { WidgetBase, WidgetState } from './widgetBase';\n\nexport type PlaceholderState = WidgetState & {\n    _type_: 'Placeholder';\n    _child_?: number | string;\n};\n\nexport class PlaceholderWidget extends WidgetBase {\n    createElement(): HTMLElement {\n        let element = document.createElement('div');\n        element.classList.add('reflex-single-container');\n        return element;\n    }\n\n    updateElement(element: HTMLElement, deltaState: PlaceholderState): void {\n        replaceOnlyChild(element, deltaState._child_);\n    }\n\n    updateChildLayouts(): void {\n        getInstanceByWidgetId(this.state['_child_']).replaceLayoutCssProperties(\n            {}\n        );\n    }\n}\n",
         "import { colorToCss } from './app';\nimport { WidgetBase, WidgetState } from './widgetBase';\n\nexport type SwitchState = WidgetState & {\n    _type_: 'switch';\n    is_on?: boolean;\n    knobColorOn?: [number, number, number, number];\n    knobColorOff?: [number, number, number, number];\n    backgroundColorOn?: [number, number, number, number];\n    backgroundColorOff?: [number, number, number, number];\n};\n\nexport class SwitchWidget extends WidgetBase {\n    createElement(): HTMLElement {\n        let element = document.createElement('div');\n        element.classList.add('reflex-switch');\n\n        let containerElement = document.createElement('div');\n        containerElement.classList.add('container');\n        element.appendChild(containerElement);\n\n        let checkboxElement = document.createElement('input');\n        checkboxElement.type = 'checkbox';\n        containerElement.appendChild(checkboxElement);\n\n        let knobElement = document.createElement('div');\n        knobElement.classList.add('knob');\n        containerElement.appendChild(knobElement);\n\n        checkboxElement.addEventListener('change', () => {\n            this.setStateAndNotifyBackend({\n                is_on: checkboxElement.checked,\n            });\n        });\n\n        return element;\n    }\n\n    updateElement(element: HTMLElement, deltaState: SwitchState): void {\n        if (deltaState.is_on !== undefined) {\n            if (deltaState.is_on) {\n                element.classList.add('is-on');\n            } else {\n                element.classList.remove('is-on');\n            }\n\n            // Assign the new value to the checkbox element, but only if it\n            // differs from the current value, to avoid immediately triggering\n            // the event again.\n            let checkboxElement = element.querySelector('input');\n            if (checkboxElement?.checked !== deltaState.is_on) {\n                checkboxElement!.checked = deltaState.is_on;\n            }\n        }\n\n        if (deltaState.knobColorOff !== undefined) {\n            element.style.setProperty(\n                '--switch-knob-color-off',\n                colorToCss(deltaState.knobColorOff)\n            );\n        }\n\n        if (deltaState.knobColorOn !== undefined) {\n            element.style.setProperty(\n                '--switch-knob-color-on',\n                colorToCss(deltaState.knobColorOn)\n            );\n        }\n\n        if (deltaState.backgroundColorOff !== undefined) {\n            element.style.setProperty(\n                '--switch-background-color-off',\n                colorToCss(deltaState.backgroundColorOff)\n            );\n        }\n\n        if (deltaState.backgroundColorOn !== undefined) {\n            element.style.setProperty(\n                '--switch-background-color-on',\n                colorToCss(deltaState.backgroundColorOn)\n            );\n        }\n    }\n}\n",
         "import { colorToCss } from './app';\nimport { WidgetBase, WidgetState } from './widgetBase';\n\nexport type ProgressCircleState = WidgetState & {\n    _type_: 'progressCircle';\n    color?: [number, number, number, number];\n    background_color?: [number, number, number, number];\n    progress?: number | null;\n};\n\nexport class ProgressCircleWidget extends WidgetBase {\n    createElement(): HTMLElement {\n        let element = document.createElement('div');\n        element.innerHTML = `\n            <svg viewBox=\"25 25 50 50\">\n                <circle class=\"background\" cx=\"50\" cy=\"50\" r=\"20\"></circle>\n                <circle class=\"progress\" cx=\"50\" cy=\"50\" r=\"20\"></circle>\n            </svg>\n        `;\n        element.classList.add('reflex-progress-circle');\n        return element;\n    }\n\n    updateElement(element: HTMLElement, deltaState: ProgressCircleState): void {\n        if (deltaState.color !== undefined) {\n            element.style.stroke = colorToCss(deltaState.color);\n        }\n\n        if (deltaState.background_color !== undefined) {\n            element.style.setProperty(\n                '--background-color',\n                colorToCss(deltaState.background_color)\n            );\n        }\n\n        if (deltaState.progress !== undefined) {\n            if (deltaState.progress === null) {\n                element.classList.add('spinning');\n            } else {\n                element.classList.remove('spinning');\n\n                let fullCircle = 40 * Math.PI;\n                element.style.setProperty(\n                    '--dasharray',\n                    `${deltaState.progress * fullCircle}, ${\n                        (1 - deltaState.progress) * fullCircle\n                    }`\n                );\n            }\n        }\n    }\n}\n",
         "import { WidgetBase, WidgetState } from './widgetBase';\n\ntype PlotState = WidgetState & {\n    _type_: 'plot';\n    plotJson?: string;\n};\n\nfunction loadPlotly(callback) {\n    if (typeof Plotly === 'undefined') {\n        console.log('Fetching plotly.js');\n        let script = document.createElement('script');\n        script.src = '/reflex/asset/plotly.min.js';\n        script.onload = callback;\n        document.head.appendChild(script);\n    } else {\n        callback();\n    }\n}\n\nexport class PlotWidget extends WidgetBase {\n    createElement(): HTMLElement {\n        let element = document.createElement('div');\n        element.style.display = 'inline-block';\n        return element;\n    }\n\n    updateElement(element: HTMLElement, deltaState: PlotState): void {\n        if (deltaState.plotJson !== undefined) {\n            element.innerHTML = '';\n            loadPlotly(() => {\n                let plotJson = JSON.parse(deltaState.plotJson);\n                Plotly.newPlot(element, plotJson.data, plotJson.layout, {\n                    responsive: true,\n                });\n            });\n        }\n    }\n}\n",
         "import { getInstanceByWidgetId, replaceOnlyChild } from './app';\nimport { WidgetBase, WidgetState } from './widgetBase';\n\nexport type AlignState = WidgetState & {\n    _type_: 'Align-builtin';\n    child?: number | string;\n    align_x?: number | null;\n    align_y?: number | null;\n};\n\nexport class AlignWidget extends WidgetBase {\n    createElement(): HTMLElement {\n        let element = document.createElement('div');\n        element.classList.add('reflex-align');\n        return element;\n    }\n\n    updateElement(element: HTMLElement, deltaState: AlignState): void {\n        replaceOnlyChild(element, deltaState.child);\n    }\n\n    updateChildLayouts(): void {\n        // Prepare the list of CSS properties to apply to the child\n        let align_x: number = this.state['align_x']!;\n        let align_y: number = this.state['align_y']!;\n\n        let cssProperties = {};\n\n        let transform_x;\n        if (align_x === null) {\n            cssProperties['width'] = '100%';\n            transform_x = 0;\n        } else {\n            cssProperties['width'] = 'max-content';\n            cssProperties['left'] = `${align_x * 100}%`;\n            transform_x = align_x * -100;\n        }\n\n        let transform_y;\n        if (align_y === null) {\n            cssProperties['height'] = '100%';\n            transform_y = 0;\n        } else {\n            cssProperties['height'] = 'max-content';\n            cssProperties['top'] = `${align_y * 100}%`;\n            transform_y = align_y * -100;\n        }\n\n        if (transform_x !== 0 || transform_y !== 0) {\n            cssProperties[\n                'transform'\n            ] = `translate(${transform_x}%, ${transform_y}%)`;\n        }\n\n        // Apply the CSS properties to the child\n        getInstanceByWidgetId(this.state['child']).replaceLayoutCssProperties(\n            cssProperties\n        );\n    }\n}\n",
         "import { getInstanceByWidgetId, replaceOnlyChild } from './app';\nimport { WidgetBase, WidgetState } from './widgetBase';\n\nexport type MarginState = WidgetState & {\n    _type_: 'Margin-builtin';\n    child?: number | string;\n    margin_left?: number;\n    margin_top?: number;\n    margin_right?: number;\n    margin_bottom?: number;\n};\n\nexport class MarginWidget extends WidgetBase {\n    createElement(): HTMLElement {\n        let element = document.createElement('div');\n        element.classList.add('reflex-margin');\n        element.classList.add('reflex-single-container');\n        return element;\n    }\n\n    updateElement(element: HTMLElement, deltaState: MarginState): void {\n        replaceOnlyChild(element, deltaState.child);\n\n        if (deltaState.margin_left !== undefined) {\n            element.style.paddingLeft = `${deltaState.margin_left}em`;\n        }\n\n        if (deltaState.margin_top !== undefined) {\n            element.style.paddingTop = `${deltaState.margin_top}em`;\n        }\n\n        if (deltaState.margin_right !== undefined) {\n            element.style.paddingRight = `${deltaState.margin_right}em`;\n        }\n\n        if (deltaState.margin_bottom !== undefined) {\n            element.style.paddingBottom = `${deltaState.margin_bottom}em`;\n        }\n    }\n\n    updateChildLayouts(): void {\n        // let marginX = this.state['margin_left']! + this.state['margin_right']!;\n        // let marginY = this.state['margin_top']! + this.state['margin_bottom']!;\n\n        // getInstanceByWidgetId(this.state['child']).replaceLayoutCssProperties({\n        //     'margin-left': `${this.state['margin_left']}em`,\n        //     'margin-top': `${this.state['margin_top']}em`,\n        //     'margin-right': `${this.state['margin_right']}em`,\n        //     'margin-bottom': `${this.state['margin_bottom']}em`,\n        //     width: `calc(100% - ${marginX}em)`,\n        //     height: `calc(100% - ${marginY}em)`,\n        // });\n        getInstanceByWidgetId(this.state['child']).replaceLayoutCssProperties(\n            {}\n        );\n    }\n}\n",
         "import { WidgetBase, WidgetState } from './widgetBase';\n\nexport type MediaPlayerState = WidgetState & {\n    _type_: 'mediaPlayer';\n    media?: string;\n    loop?: boolean;\n    autoplay?: boolean;\n    controls?: boolean;\n    muted?: boolean;\n    volume?: number;\n};\n\nexport class MediaPlayerWidget extends WidgetBase {\n    createElement(): HTMLElement {\n        let element = document.createElement('video');\n        return element;\n    }\n\n    updateElement(element: HTMLMediaElement, deltaState: MediaPlayerState): void {\n        if (deltaState.media !== undefined) {\n            element.src = deltaState.media;\n        }\n\n        if (deltaState.loop !== undefined) {\n            element.loop = deltaState.loop;\n        }\n\n        if (deltaState.autoplay !== undefined) {\n            element.autoplay = deltaState.autoplay;\n        }\n\n        if (deltaState.controls !== undefined) {\n            element.controls = deltaState.controls;\n        }\n\n        if (deltaState.muted !== undefined) {\n            element.muted = deltaState.muted;\n        }\n\n        if (deltaState.volume !== undefined) {\n            element.volume = deltaState.volume;\n        }\n    }\n}\n",
-        "import { TextWidget } from './text';\nimport { RowWidget } from './row';\nimport { ColumnWidget } from './column';\nimport { DropdownWidget } from './dropdown';\nimport { RectangleWidget } from './rectangle';\nimport { StackWidget } from './stack';\nimport { Color, Fill } from './models';\nimport { MouseEventListenerWidget } from './mouseEventListener';\nimport { TextInputWidget } from './textInput';\nimport { PlaceholderWidget } from './placeholder';\nimport { SwitchWidget } from './switch';\nimport { WidgetBase, WidgetState } from './widgetBase';\nimport { ProgressCircleWidget } from './progressCircle';\nimport { PlotWidget } from './plot';\nimport { AlignWidget } from './align';\nimport { MarginWidget } from './margin';\nimport { MediaPlayerWidget } from './mediaPlayer';\n\nconst sessionToken = '{session_token}';\nconst initialMessages = '{initial_messages}';\nconst CHILD_ATTRIBUTE_NAMES = {}; // {child_attribute_names};\n\nlet socket: WebSocket | null = null;\nexport var pixelsPerEm = 16;\n\nconst elementsToInstances = new WeakMap<HTMLElement, WidgetBase>();\n\nexport function colorToCss(color: Color): string {\n    const [r, g, b, a] = color;\n    return `rgba(${r * 255}, ${g * 255}, ${b * 255}, ${a})`;\n}\n\nexport function fillToCss(fill: Fill): string {\n    // Solid Color\n    if (fill.type === 'solid') {\n        return colorToCss(fill.color);\n    }\n\n    // Linear Gradient\n    if (fill.type === 'linearGradient') {\n        if (fill.stops.length == 1) {\n            return colorToCss(fill.stops[0][0]);\n        }\n\n        let stopStrings: string[] = [];\n        for (let i = 0; i < fill.stops.length; i++) {\n            let color = fill.stops[i][0];\n            let position = fill.stops[i][1];\n            stopStrings.push(`${colorToCss(color)} ${position * 100}%`);\n        }\n\n        return `linear-gradient(${fill.angleDegrees}deg, ${stopStrings.join(\n            ', '\n        )})`;\n    }\n\n    // Image\n    if (fill.type === 'image') {\n        let cssUrl = `url('${fill.imageUrl}')`;\n\n        if (fill.fillMode == 'fit') {\n            return `${cssUrl} center/contain no-repeat`;\n        } else if (fill.fillMode == 'stretch') {\n            return `${cssUrl} top left / 100% 100%`;\n        } else if (fill.fillMode == 'tile') {\n            return `${cssUrl} left top repeat`;\n        } else if (fill.fillMode == 'zoom') {\n            return `${cssUrl} center/cover no-repeat`;\n        } else {\n            // Invalid fill mode\n            // @ts-ignore\n            throw `Invalid fill mode for image fill: ${fill.type}`;\n        }\n    }\n\n    // Invalid fill type\n    // @ts-ignore\n    throw `Invalid fill type: ${fill.type}`;\n}\n\nexport function getElementByWidgetId(id: number | string): HTMLElement {\n    let element = document.getElementById(`reflex-id-${id}`);\n\n    if (element === null) {\n        throw `Could not find widget with id ${id}`;\n    }\n\n    return element;\n}\n\nexport function getInstanceByWidgetId(id: number | string): WidgetBase {\n    let element = getElementByWidgetId(id);\n\n    let instance = elementsToInstances.get(element);\n\n    if (instance === undefined) {\n        throw `Could not find widget with id ${id}`;\n    }\n\n    return instance;\n}\n\nexport function getParentWidgetElementIncludingInjected(\n    element: HTMLElement\n): HTMLElement | null {\n    let curElement = element.parentElement;\n\n    while (curElement !== null) {\n        if (curElement.id.startsWith('reflex-id-')) {\n            return curElement;\n        }\n\n        curElement = curElement.parentElement;\n    }\n\n    return null;\n}\n\nexport function getParentWidgetElementExcludingInjected(\n    element: HTMLElement\n): HTMLElement | null {\n    let curElement: HTMLElement | null = element;\n\n    while (true) {\n        curElement = getParentWidgetElementIncludingInjected(curElement);\n\n        if (curElement === null) {\n            return null;\n        }\n\n        if (curElement.id.match(/reflex-id-\\d+$/)) {\n            return curElement;\n        }\n    }\n}\n\nconst widgetClasses = {\n    'Align-builtin': AlignWidget,\n    'Column-builtin': ColumnWidget,\n    'Dropdown-builtin': DropdownWidget,\n    'Margin-builtin': MarginWidget,\n    'MediaPlayer-builtin': MediaPlayerWidget,\n    'MouseEventListener-builtin': MouseEventListenerWidget,\n    'Plot-builtin': PlotWidget,\n    'ProgressCircle-builtin': ProgressCircleWidget,\n    'Rectangle-builtin': RectangleWidget,\n    'Row-builtin': RowWidget,\n    'Stack-builtin': StackWidget,\n    'Switch-builtin': SwitchWidget,\n    'Text-builtin': TextWidget,\n    'TextInput-builtin': TextInputWidget,\n    Placeholder: PlaceholderWidget,\n};\n\nglobalThis.widgetClasses = widgetClasses;\n\nfunction processMessage(message: any) {\n    console.log('Received message: ', message);\n\n    if (message.type == 'updateWidgetStates') {\n        updateWidgetStates(message.deltaStates, message.rootWidgetId);\n    } else if (message.type == 'evaluateJavascript') {\n        eval(message.javascriptSource);\n    } else if (message.type == 'requestFileUpload') {\n        requestFileUpload(message);\n    } else {\n        throw `Encountered unknown message type: ${message}`;\n    }\n}\n\nfunction getCurrentWidgetState(\n    id: number | string,\n    deltaState: WidgetState\n): WidgetState {\n    let parentElement = document.getElementById(`reflex-id-${id}`);\n\n    if (parentElement === null) {\n        return deltaState;\n    }\n\n    let parentInstance = elementsToInstances.get(parentElement);\n\n    if (parentInstance === undefined) {\n        return deltaState;\n    }\n\n    return {\n        ...parentInstance.state,\n        ...deltaState,\n    };\n}\n\nfunction createLayoutWidgetStates(\n    widgetId: number | string,\n    deltaState: WidgetState,\n    message: { [id: string]: WidgetState }\n): number | string {\n    let entireState = getCurrentWidgetState(widgetId, deltaState);\n    let resultId = widgetId;\n\n    // Margin\n    let margin = entireState['_margin_']!;\n    if (\n        margin[0] !== 0 ||\n        margin[1] !== 0 ||\n        margin[2] !== 0 ||\n        margin[3] !== 0\n    ) {\n        let marginId = `${widgetId}-margin`;\n        message[marginId] = {\n            _type_: 'Margin-builtin',\n            _python_type_: 'Margin (injected)',\n            _size_: entireState['_size_'],\n            _grow_: entireState['_grow_'],\n            // @ts-ignore\n            child: resultId,\n            margin_left: margin[0],\n            margin_top: margin[1],\n            margin_right: margin[2],\n            margin_bottom: margin[3],\n        };\n        resultId = marginId;\n    }\n\n    // Align\n    let align = entireState['_align_']!;\n    if (align[0] !== null || align[1] !== null) {\n        let alignId = `${widgetId}-align`;\n        message[alignId] = {\n            _type_: 'Align-builtin',\n            _python_type_: 'Align (injected)',\n            _size_: entireState['_size_'],\n            _grow_: entireState['_grow_'],\n            // @ts-ignore\n            child: resultId,\n            align_x: align[0],\n            align_y: align[1],\n        };\n        resultId = alignId;\n    }\n\n    return resultId;\n}\n\nfunction replaceChildrenWithLayoutWidgets(\n    deltaState: WidgetState,\n    childIds: Set<string>,\n    message: { [id: string]: WidgetState }\n): void {\n    let propertyNamesWithChildren =\n        CHILD_ATTRIBUTE_NAMES[deltaState['_type_']!] || [];\n\n    function cleanId(id: string): string {\n        return id.split('-')[0];\n    }\n\n    for (let propertyName of propertyNamesWithChildren) {\n        let propertyValue = deltaState[propertyName];\n\n        if (Array.isArray(propertyValue)) {\n            deltaState[propertyName] = propertyValue.map((childId) => {\n                childId = cleanId(childId.toString());\n                childIds.add(childId);\n                return createLayoutWidgetStates(\n                    childId,\n                    message[childId] || {},\n                    message\n                );\n            });\n        } else if (propertyValue !== null) {\n            let childId = cleanId(propertyValue.toString());\n            deltaState[propertyName] = createLayoutWidgetStates(\n                childId,\n                message[childId] || {},\n                message\n            );\n            childIds.add(childId);\n        }\n    }\n}\n\nfunction preprocessMessage(message: { [id: string]: WidgetState }, rootWidgetId: string | number | null): string | number | null {\n    // Make sure the rootWidgetId is not a number, but a string. This ensures\n    // that there are no false negatives when compared to an id in the message.\n    if (typeof rootWidgetId === 'number') {\n        rootWidgetId = rootWidgetId.toString();\n    }\n\n    let originalWidgetIds = Object.keys(message);\n\n    // Keep track of which widgets have their parents in the message\n    let childIds: Set<string> = new Set();\n\n    // Walk over all widgets in the message and inject layout widgets. The\n    // message is modified in-place, so take care to have a copy of all keys\n    for (let widgetId of originalWidgetIds) {\n        replaceChildrenWithLayoutWidgets(message[widgetId], childIds, message);\n    }\n\n    // Find all widgets which have had a layout widget injected, and make sure\n    // their parents are updated to point to the new widget.\n    for (let widgetId of originalWidgetIds) {\n        // Child of another widget in the message\n        if (childIds.has(widgetId)) {\n            console.log(`Discarding ${widgetId} because it is a child`);\n            continue;\n        }\n        \n        if (widgetId === rootWidgetId) {\n            rootWidgetId = createLayoutWidgetStates(widgetId, message[widgetId], message);\n            continue;\n        }\n\n        // The parent isn't contained in the message. Find and add it.\n        let childElement = document.getElementById(`reflex-id-${widgetId}`);\n        if (childElement === null) {\n            console.log(`Discarding ${widgetId} because it is not in the DOM`);\n            continue;\n        }\n\n        let parentElement =\n            getParentWidgetElementExcludingInjected(childElement);\n        if (parentElement === null) {\n            console.log(`Discarding ${widgetId} because it has no parent`);\n            continue;\n        }\n\n        let parentInstance = elementsToInstances.get(parentElement);\n        if (parentInstance === undefined) {\n            throw `Parent widget with id ${parentElement} not found`;\n        }\n\n        let parentId = parentElement.id.slice('reflex-id-'.length);\n        let newParentState = { ...parentInstance.state };\n        replaceChildrenWithLayoutWidgets(newParentState, childIds, message);\n        message[parentId] = newParentState;\n        console.log(`Parent of ${widgetId} is ${parentId}`);\n    }\n\n    return rootWidgetId;\n}\n\nfunction updateWidgetStates(\n    message: { [id: string]: WidgetState },\n    rootWidgetId: string | number | null\n): void {\n    // Preprocess the message. This converts `_align_` and `_margin_` properties\n    // into actual widgets, amongst other things.\n    rootWidgetId = preprocessMessage(message, rootWidgetId);\n    console.log(message);\n\n    // Create a HTML element to hold all latent widgets, so they aren't\n    // garbage collected while updating the DOM.\n    let latentWidgets = document.createElement('div');\n    document.body.appendChild(latentWidgets);\n    latentWidgets.id = 'reflex-latent-widgets';\n    latentWidgets.style.display = 'none';\n\n    // Make sure all widgets mentioned in the message have a corresponding HTML\n    // element\n    for (let widgetId in message) {\n        let deltaState = message[widgetId];\n        let elementId = `reflex-id-${widgetId}`;\n        let element = document.getElementById(elementId);\n\n        // This is a reused element, no need to instantiate a new one\n        if (element) {\n            continue;\n        }\n\n        // Get the class for this widget\n        const widgetClass = widgetClasses[deltaState._type_!];\n\n        // Make sure the widget type is valid (Just helpful for debugging)\n        if (!widgetClass) {\n            throw `Encountered unknown widget type: ${deltaState._type_}`;\n        }\n\n        // Create an instance for this widget\n        let instance: WidgetBase = new widgetClass(elementId, deltaState);\n\n        // Build the widget\n        element = instance.createElement();\n        element.id = elementId;\n        element.classList.add('reflex-widget');\n\n        // Store the widget's class name in the element. Used for debugging.\n        element.setAttribute('dbg-py-class', deltaState._python_type_!);\n\n        // Set the widget's key, if it has one. Used for debugging.\n        let key = deltaState['key'];\n        if (key !== undefined) {\n            element.setAttribute('dbg-key', `${key}`);\n        }\n\n        // Create a mapping from the element to the widget instance\n        elementsToInstances.set(element, instance);\n\n        // Keep the widget alive\n        latentWidgets.appendChild(element);\n    }\n\n    // Update all widgets mentioned in the message\n    let widgetsNeedingLayoutUpdate = new Set<WidgetBase>();\n\n    for (let id in message) {\n        let deltaState = message[id];\n        let element = getElementByWidgetId(id);\n\n        // Perform updates common to all widgets\n        commonUpdate(element, deltaState);\n\n        // Perform updates specific to this widget type\n        let instance = elementsToInstances.get(element!) as WidgetBase;\n        instance.updateElement(element, deltaState);\n\n        // Update the widget's state\n        instance.state = {\n            ...instance.state,\n            ...deltaState,\n        };\n\n        // Queue the widget and its parent for a layout update\n        widgetsNeedingLayoutUpdate.add(instance);\n\n        let parentElement = getParentWidgetElementIncludingInjected(element!);\n        if (parentElement) {\n            let parentInstance = elementsToInstances.get(parentElement);\n\n            if (!parentInstance) {\n                throw `Failed to find parent widget for ${id}`;\n            }\n\n            widgetsNeedingLayoutUpdate.add(parentInstance);\n        }\n    }\n\n    // Widgets that have changed, or had their parents changed need to have\n    // their layout updated\n    widgetsNeedingLayoutUpdate.forEach((widget) => {\n        widget.updateChildLayouts();\n    });\n\n    // Replace the root widget if requested\n    if (rootWidgetId !== null) {\n        let rootElement = getElementByWidgetId(rootWidgetId);\n        document.body.innerHTML = '';\n        document.body.appendChild(rootElement!);\n    }\n\n    // Remove the latent widgets\n    latentWidgets.remove();\n}\n\nfunction commonUpdate(element: HTMLElement, state: WidgetState) {\n    if (state._size_ !== undefined) {\n        if (state._size_[0] === null) {\n            element.style.removeProperty('min-width');\n        } else {\n            element.style.minWidth = `${state._size_[0]}em`;\n        }\n\n        if (state._size_[1] === null) {\n            element.style.removeProperty('min-height');\n        } else {\n            element.style.minHeight = `${state._size_[1]}em`;\n        }\n    }\n}\n\nexport function replaceOnlyChild(\n    parentElement: HTMLElement,\n    childId: null | undefined | number | string\n) {\n    // If undefined, do nothing\n    if (childId === undefined) {\n        return;\n    }\n\n    // If null, remove the child\n    if (childId === null) {\n        parentElement.innerHTML = '';\n        return;\n    }\n\n    const currentChildElement = parentElement.firstElementChild;\n\n    // If a child already exists, either move it to the latent container or\n    // leave it alone if it's already the correct element\n    if (currentChildElement !== null) {\n        // Don't reparent the child if not necessary. This way things like\n        // keyboard focus are preserved\n        if (currentChildElement.id === `reflex-id-${childId}`) {\n            return;\n        }\n\n        // Move the child element to a latent container, so it isn't garbage\n        // collected\n        let latentWidgets = document.getElementById('reflex-latent-widgets');\n        latentWidgets?.appendChild(currentChildElement);\n    }\n\n    // Add the replacement widget\n    let newElement = getElementByWidgetId(childId);\n    parentElement?.appendChild(newElement);\n}\n\nexport function replaceChildren(\n    parentElement: HTMLElement,\n    childIds: undefined | (number | string)[]\n) {\n    // If undefined, do nothing\n    if (childIds === undefined) {\n        return;\n    }\n    let latentWidgets = document.getElementById('reflex-latent-widgets')!;\n\n    let curElement = parentElement.firstElementChild;\n    let curIdIndex = 0;\n\n    while (true) {\n        // If there are no more children in the DOM element, add the remaining\n        // children\n        if (curElement === null) {\n            while (curIdIndex < childIds.length) {\n                let curId = childIds[curIdIndex];\n                let newElement = getElementByWidgetId(curId);\n                parentElement.appendChild(newElement!);\n                curIdIndex++;\n            }\n            break;\n        }\n\n        // If there are no more children in the message, remove the remaining\n        // DOM children\n        if (curIdIndex >= childIds.length) {\n            while (curElement !== null) {\n                let nextElement = curElement.nextElementSibling;\n                latentWidgets.appendChild(curElement);\n                curElement = nextElement;\n            }\n            break;\n        }\n\n        // This element is the correct element, move on\n        let curId = childIds[curIdIndex];\n        if (curElement.id === `reflex-id-${curId}`) {\n            curElement = curElement.nextElementSibling;\n            curIdIndex++;\n            continue;\n        }\n\n        // This element is not the correct element, insert the correct one\n        // instead\n        let newElement = getElementByWidgetId(curId);\n        parentElement.insertBefore(newElement!, curElement);\n        curIdIndex++;\n    }\n}\n\nfunction requestFileUpload(message: any) {\n    // Create a file upload input element\n    let input = document.createElement('input');\n    input.type = 'file';\n    input.multiple = message.multiple;\n\n    if (message.fileExtensions !== null) {\n        input.accept = message.fileExtensions.join(',');\n    }\n\n    input.style.display = 'none';\n\n    function finish() {\n        // Don't run twice\n        if (input.parentElement === null) {\n            return;\n        }\n\n        // Build a `FormData` object containing the files\n        const data = new FormData();\n\n        let ii = 0;\n        for (const file of input.files || []) {\n            ii += 1;\n            data.append('file_names', file.name);\n            data.append('file_types', file.type);\n            data.append('file_sizes', file.size.toString());\n            data.append('file_streams', file, file.name);\n        }\n\n        // FastAPI has trouble parsing empty form data. Append a dummy value so\n        // it's never empty\n        data.append('dummy', 'dummy');\n\n        // Upload the files\n        fetch(message.uploadUrl, {\n            method: 'PUT',\n            body: data,\n        });\n\n        // Remove the input element from the DOM. Removing this too early causes\n        // weird behavior in some browsers\n        input.remove();\n    }\n\n    // Listen for changes to the input\n    input.addEventListener('change', finish);\n\n    // Detect if the window gains focus. This means the file upload dialog was\n    // closed without selecting a file\n    window.addEventListener(\n        'focus',\n        function () {\n            // In some browsers `focus` fires before `change`. Give `change`\n            // time to run first.\n            this.window.setTimeout(finish, 500);\n        },\n        { once: true }\n    );\n\n    // Add the input element to the DOM\n    document.body.appendChild(input);\n\n    // Trigger the file upload\n    input.click();\n}\n\nfunction main() {\n    // Determine the browser's font size\n    var measure = document.createElement('div');\n    measure.style.height = '10em';\n    document.body.appendChild(measure);\n    pixelsPerEm = measure.offsetHeight / 10;\n    document.body.removeChild(measure);\n\n    // Process initial messages\n    console.log(`Processing ${initialMessages.length} initial message(s)`);\n    for (let message of initialMessages) {\n        processMessage(message);\n    }\n\n    // Connect to the websocket\n    var url = new URL(\n        `/reflex/ws?sessionToken=${sessionToken}`,\n        window.location.href\n    );\n    url.protocol = url.protocol.replace('http', 'ws');\n    console.log(`Connecting websocket to ${url.href}`);\n    socket = new WebSocket(url.href);\n\n    socket.addEventListener('open', onOpen);\n    socket.addEventListener('message', onMessage);\n    socket.addEventListener('error', onError);\n    socket.addEventListener('close', onClose);\n}\n\nfunction onOpen() {\n    console.log('Connection opened');\n}\n\nfunction onMessage(event: any) {\n    // Parse the message JSON\n    let message = JSON.parse(event.data);\n\n    // Handle it\n    processMessage(message);\n}\n\nfunction onError(event: any) {\n    console.log(`Error: ${event.message}`);\n}\n\nfunction onClose(event: any) {\n    console.log(`Connection closed: ${event.reason}`);\n}\n\nexport function sendMessageOverWebsocket(message: object) {\n    if (!socket) {\n        console.log(\n            `Attempted to send message, but the websocket is not connected: ${message}`\n        );\n        return;\n    }\n\n    console.log('Sending message: ', message);\n\n    socket.send(JSON.stringify(message));\n}\n\nmain();\n"
+        "import { TextWidget } from './text';\nimport { RowWidget } from './row';\nimport { ColumnWidget } from './column';\nimport { DropdownWidget } from './dropdown';\nimport { RectangleWidget } from './rectangle';\nimport { StackWidget } from './stack';\nimport { Color, Fill } from './models';\nimport { MouseEventListenerWidget } from './mouseEventListener';\nimport { TextInputWidget } from './textInput';\nimport { PlaceholderWidget } from './placeholder';\nimport { SwitchWidget } from './switch';\nimport { WidgetBase, WidgetState } from './widgetBase';\nimport { ProgressCircleWidget } from './progressCircle';\nimport { PlotWidget } from './plot';\nimport { AlignWidget } from './align';\nimport { MarginWidget } from './margin';\nimport { MediaPlayerWidget } from './mediaPlayer';\n\nconst sessionToken = '{session_token}';\nconst initialMessages = '{initial_messages}';\n\n// @ts-ignore\nconst CHILD_ATTRIBUTE_NAMES: { [id: string]: string[] } =\n    '{child_attribute_names}';\n\nlet socket: WebSocket | null = null;\nexport var pixelsPerEm = 16;\n\nconst elementsToInstances = new WeakMap<HTMLElement, WidgetBase>();\n\nexport function colorToCss(color: Color): string {\n    const [r, g, b, a] = color;\n    return `rgba(${r * 255}, ${g * 255}, ${b * 255}, ${a})`;\n}\n\nexport function fillToCss(fill: Fill): string {\n    // Solid Color\n    if (fill.type === 'solid') {\n        return colorToCss(fill.color);\n    }\n\n    // Linear Gradient\n    if (fill.type === 'linearGradient') {\n        if (fill.stops.length == 1) {\n            return colorToCss(fill.stops[0][0]);\n        }\n\n        let stopStrings: string[] = [];\n        for (let i = 0; i < fill.stops.length; i++) {\n            let color = fill.stops[i][0];\n            let position = fill.stops[i][1];\n            stopStrings.push(`${colorToCss(color)} ${position * 100}%`);\n        }\n\n        return `linear-gradient(${fill.angleDegrees}deg, ${stopStrings.join(\n            ', '\n        )})`;\n    }\n\n    // Image\n    if (fill.type === 'image') {\n        let cssUrl = `url('${fill.imageUrl}')`;\n\n        if (fill.fillMode == 'fit') {\n            return `${cssUrl} center/contain no-repeat`;\n        } else if (fill.fillMode == 'stretch') {\n            return `${cssUrl} top left / 100% 100%`;\n        } else if (fill.fillMode == 'tile') {\n            return `${cssUrl} left top repeat`;\n        } else if (fill.fillMode == 'zoom') {\n            return `${cssUrl} center/cover no-repeat`;\n        } else {\n            // Invalid fill mode\n            // @ts-ignore\n            throw `Invalid fill mode for image fill: ${fill.type}`;\n        }\n    }\n\n    // Invalid fill type\n    // @ts-ignore\n    throw `Invalid fill type: ${fill.type}`;\n}\n\nexport function getElementByWidgetId(id: number | string): HTMLElement {\n    let element = document.getElementById(`reflex-id-${id}`);\n\n    if (element === null) {\n        throw `Could not find widget with id ${id}`;\n    }\n\n    return element;\n}\n\nexport function getInstanceByWidgetId(id: number | string): WidgetBase {\n    let element = getElementByWidgetId(id);\n\n    let instance = elementsToInstances.get(element);\n\n    if (instance === undefined) {\n        throw `Could not find widget with id ${id}`;\n    }\n\n    return instance;\n}\n\nexport function getParentWidgetElementIncludingInjected(\n    element: HTMLElement\n): HTMLElement | null {\n    let curElement = element.parentElement;\n\n    while (curElement !== null) {\n        if (curElement.id.startsWith('reflex-id-')) {\n            return curElement;\n        }\n\n        curElement = curElement.parentElement;\n    }\n\n    return null;\n}\n\nexport function getParentWidgetElementExcludingInjected(\n    element: HTMLElement\n): HTMLElement | null {\n    let curElement: HTMLElement | null = element;\n\n    while (true) {\n        curElement = getParentWidgetElementIncludingInjected(curElement);\n\n        if (curElement === null) {\n            return null;\n        }\n\n        if (curElement.id.match(/reflex-id-\\d+$/)) {\n            return curElement;\n        }\n    }\n}\n\nconst widgetClasses = {\n    'Align-builtin': AlignWidget,\n    'Column-builtin': ColumnWidget,\n    'Dropdown-builtin': DropdownWidget,\n    'Margin-builtin': MarginWidget,\n    'MediaPlayer-builtin': MediaPlayerWidget,\n    'MouseEventListener-builtin': MouseEventListenerWidget,\n    'Plot-builtin': PlotWidget,\n    'ProgressCircle-builtin': ProgressCircleWidget,\n    'Rectangle-builtin': RectangleWidget,\n    'Row-builtin': RowWidget,\n    'Stack-builtin': StackWidget,\n    'Switch-builtin': SwitchWidget,\n    'Text-builtin': TextWidget,\n    'TextInput-builtin': TextInputWidget,\n    Placeholder: PlaceholderWidget,\n};\n\nglobalThis.widgetClasses = widgetClasses;\n\nfunction processMessage(message: any) {\n    console.log('Received message: ', message);\n\n    if (message.type == 'updateWidgetStates') {\n        updateWidgetStates(message.deltaStates, message.rootWidgetId);\n    } else if (message.type == 'evaluateJavascript') {\n        eval(message.javascriptSource);\n    } else if (message.type == 'requestFileUpload') {\n        requestFileUpload(message);\n    } else {\n        throw `Encountered unknown message type: ${message}`;\n    }\n}\n\nfunction getCurrentWidgetState(\n    id: number | string,\n    deltaState: WidgetState\n): WidgetState {\n    let parentElement = document.getElementById(`reflex-id-${id}`);\n\n    if (parentElement === null) {\n        return deltaState;\n    }\n\n    let parentInstance = elementsToInstances.get(parentElement);\n\n    if (parentInstance === undefined) {\n        return deltaState;\n    }\n\n    return {\n        ...parentInstance.state,\n        ...deltaState,\n    };\n}\n\nfunction createLayoutWidgetStates(\n    widgetId: number | string,\n    deltaState: WidgetState,\n    message: { [id: string]: WidgetState }\n): number | string {\n    let entireState = getCurrentWidgetState(widgetId, deltaState);\n    let resultId = widgetId;\n\n    // Margin\n    let margin = entireState['_margin_']!;\n    if (\n        margin[0] !== 0 ||\n        margin[1] !== 0 ||\n        margin[2] !== 0 ||\n        margin[3] !== 0\n    ) {\n        let marginId = `${widgetId}-margin`;\n        message[marginId] = {\n            _type_: 'Margin-builtin',\n            _python_type_: 'Margin (injected)',\n            _size_: entireState['_size_'],\n            _grow_: entireState['_grow_'],\n            // @ts-ignore\n            child: resultId,\n            margin_left: margin[0],\n            margin_top: margin[1],\n            margin_right: margin[2],\n            margin_bottom: margin[3],\n        };\n        resultId = marginId;\n    }\n\n    // Align\n    let align = entireState['_align_']!;\n    if (align[0] !== null || align[1] !== null) {\n        let alignId = `${widgetId}-align`;\n        message[alignId] = {\n            _type_: 'Align-builtin',\n            _python_type_: 'Align (injected)',\n            _size_: entireState['_size_'],\n            _grow_: entireState['_grow_'],\n            // @ts-ignore\n            child: resultId,\n            align_x: align[0],\n            align_y: align[1],\n        };\n        resultId = alignId;\n    }\n\n    return resultId;\n}\n\nfunction replaceChildrenWithLayoutWidgets(\n    deltaState: WidgetState,\n    childIds: Set<string>,\n    message: { [id: string]: WidgetState }\n): void {\n    let propertyNamesWithChildren =\n        CHILD_ATTRIBUTE_NAMES[deltaState['_type_']!] || [];\n\n    function cleanId(id: string): string {\n        return id.split('-')[0];\n    }\n\n    for (let propertyName of propertyNamesWithChildren) {\n        let propertyValue = deltaState[propertyName];\n\n        if (Array.isArray(propertyValue)) {\n            deltaState[propertyName] = propertyValue.map((childId) => {\n                childId = cleanId(childId.toString());\n                childIds.add(childId);\n                return createLayoutWidgetStates(\n                    childId,\n                    message[childId] || {},\n                    message\n                );\n            });\n        } else if (propertyValue !== null) {\n            let childId = cleanId(propertyValue.toString());\n            deltaState[propertyName] = createLayoutWidgetStates(\n                childId,\n                message[childId] || {},\n                message\n            );\n            childIds.add(childId);\n        }\n    }\n}\n\nfunction preprocessMessage(\n    message: { [id: string]: WidgetState },\n    rootWidgetId: string | number | null\n): string | number | null {\n    // Make sure the rootWidgetId is not a number, but a string. This ensures\n    // that there are no false negatives when compared to an id in the message.\n    if (typeof rootWidgetId === 'number') {\n        rootWidgetId = rootWidgetId.toString();\n    }\n\n    let originalWidgetIds = Object.keys(message);\n\n    // Keep track of which widgets have their parents in the message\n    let childIds: Set<string> = new Set();\n\n    // Walk over all widgets in the message and inject layout widgets. The\n    // message is modified in-place, so take care to have a copy of all keys\n    for (let widgetId of originalWidgetIds) {\n        replaceChildrenWithLayoutWidgets(message[widgetId], childIds, message);\n    }\n\n    // Find all widgets which have had a layout widget injected, and make sure\n    // their parents are updated to point to the new widget.\n    for (let widgetId of originalWidgetIds) {\n        // Child of another widget in the message\n        if (childIds.has(widgetId)) {\n            continue;\n        }\n\n        if (widgetId === rootWidgetId) {\n            rootWidgetId = createLayoutWidgetStates(\n                widgetId,\n                message[widgetId],\n                message\n            );\n            continue;\n        }\n\n        // The parent isn't contained in the message. Find and add it.\n        let childElement = document.getElementById(`reflex-id-${widgetId}`);\n        if (childElement === null) {\n            continue;\n        }\n\n        let parentElement =\n            getParentWidgetElementExcludingInjected(childElement);\n        if (parentElement === null) {\n            continue;\n        }\n\n        let parentInstance = elementsToInstances.get(parentElement);\n        if (parentInstance === undefined) {\n            throw `Parent widget with id ${parentElement} not found`;\n        }\n\n        let parentId = parentElement.id.slice('reflex-id-'.length);\n        let newParentState = { ...parentInstance.state };\n        replaceChildrenWithLayoutWidgets(newParentState, childIds, message);\n        message[parentId] = newParentState;\n    }\n\n    console.log('new message', message);\n    console.log(CHILD_ATTRIBUTE_NAMES);\n\n    return rootWidgetId;\n}\n\nfunction updateWidgetStates(\n    message: { [id: string]: WidgetState },\n    rootWidgetId: string | number | null\n): void {\n    // Preprocess the message. This converts `_align_` and `_margin_` properties\n    // into actual widgets, amongst other things.\n    rootWidgetId = preprocessMessage(message, rootWidgetId);\n\n    // Create a HTML element to hold all latent widgets, so they aren't\n    // garbage collected while updating the DOM.\n    let latentWidgets = document.createElement('div');\n    document.body.appendChild(latentWidgets);\n    latentWidgets.id = 'reflex-latent-widgets';\n    latentWidgets.style.display = 'none';\n\n    // Make sure all widgets mentioned in the message have a corresponding HTML\n    // element\n    for (let widgetId in message) {\n        let deltaState = message[widgetId];\n        let elementId = `reflex-id-${widgetId}`;\n        let element = document.getElementById(elementId);\n\n        // This is a reused element, no need to instantiate a new one\n        if (element) {\n            continue;\n        }\n\n        // Get the class for this widget\n        const widgetClass = widgetClasses[deltaState._type_!];\n\n        // Make sure the widget type is valid (Just helpful for debugging)\n        if (!widgetClass) {\n            throw `Encountered unknown widget type: ${deltaState._type_}`;\n        }\n\n        // Create an instance for this widget\n        let instance: WidgetBase = new widgetClass(elementId, deltaState);\n\n        // Build the widget\n        element = instance.createElement();\n        element.id = elementId;\n        element.classList.add('reflex-widget');\n\n        // Store the widget's class name in the element. Used for debugging.\n        element.setAttribute('dbg-py-class', deltaState._python_type_!);\n\n        // Set the widget's key, if it has one. Used for debugging.\n        let key = deltaState['key'];\n        if (key !== undefined) {\n            element.setAttribute('dbg-key', `${key}`);\n        }\n\n        // Create a mapping from the element to the widget instance\n        elementsToInstances.set(element, instance);\n\n        // Keep the widget alive\n        latentWidgets.appendChild(element);\n    }\n\n    // Update all widgets mentioned in the message\n    let widgetsNeedingLayoutUpdate = new Set<WidgetBase>();\n\n    for (let id in message) {\n        let deltaState = message[id];\n        let element = getElementByWidgetId(id);\n\n        // Perform updates common to all widgets\n        commonUpdate(element, deltaState);\n\n        // Perform updates specific to this widget type\n        let instance = elementsToInstances.get(element!) as WidgetBase;\n        instance.updateElement(element, deltaState);\n\n        // Update the widget's state\n        instance.state = {\n            ...instance.state,\n            ...deltaState,\n        };\n\n        // Queue the widget and its parent for a layout update\n        widgetsNeedingLayoutUpdate.add(instance);\n\n        let parentElement = getParentWidgetElementIncludingInjected(element!);\n        if (parentElement) {\n            let parentInstance = elementsToInstances.get(parentElement);\n\n            if (!parentInstance) {\n                throw `Failed to find parent widget for ${id}`;\n            }\n\n            widgetsNeedingLayoutUpdate.add(parentInstance);\n        }\n    }\n\n    // Widgets that have changed, or had their parents changed need to have\n    // their layout updated\n    widgetsNeedingLayoutUpdate.forEach((widget) => {\n        widget.updateChildLayouts();\n    });\n\n    // Replace the root widget if requested\n    if (rootWidgetId !== null) {\n        let rootElement = getElementByWidgetId(rootWidgetId);\n        document.body.innerHTML = '';\n        document.body.appendChild(rootElement!);\n    }\n\n    // Remove the latent widgets\n    latentWidgets.remove();\n}\n\nfunction commonUpdate(element: HTMLElement, state: WidgetState) {\n    if (state._size_ !== undefined) {\n        if (state._size_[0] === null) {\n            element.style.removeProperty('min-width');\n        } else {\n            element.style.minWidth = `${state._size_[0]}em`;\n        }\n\n        if (state._size_[1] === null) {\n            element.style.removeProperty('min-height');\n        } else {\n            element.style.minHeight = `${state._size_[1]}em`;\n        }\n    }\n}\n\nexport function replaceOnlyChild(\n    parentElement: HTMLElement,\n    childId: null | undefined | number | string\n) {\n    // If undefined, do nothing\n    if (childId === undefined) {\n        return;\n    }\n\n    // If null, remove the child\n    if (childId === null) {\n        parentElement.innerHTML = '';\n        return;\n    }\n\n    const currentChildElement = parentElement.firstElementChild;\n\n    // If a child already exists, either move it to the latent container or\n    // leave it alone if it's already the correct element\n    if (currentChildElement !== null) {\n        // Don't reparent the child if not necessary. This way things like\n        // keyboard focus are preserved\n        if (currentChildElement.id === `reflex-id-${childId}`) {\n            return;\n        }\n\n        // Move the child element to a latent container, so it isn't garbage\n        // collected\n        let latentWidgets = document.getElementById('reflex-latent-widgets');\n        latentWidgets?.appendChild(currentChildElement);\n    }\n\n    // Add the replacement widget\n    let newElement = getElementByWidgetId(childId);\n    parentElement?.appendChild(newElement);\n}\n\nexport function replaceChildren(\n    parentElement: HTMLElement,\n    childIds: undefined | (number | string)[]\n) {\n    // If undefined, do nothing\n    if (childIds === undefined) {\n        return;\n    }\n    let latentWidgets = document.getElementById('reflex-latent-widgets')!;\n\n    let curElement = parentElement.firstElementChild;\n    let curIdIndex = 0;\n\n    while (true) {\n        // If there are no more children in the DOM element, add the remaining\n        // children\n        if (curElement === null) {\n            while (curIdIndex < childIds.length) {\n                let curId = childIds[curIdIndex];\n                let newElement = getElementByWidgetId(curId);\n                parentElement.appendChild(newElement!);\n                curIdIndex++;\n            }\n            break;\n        }\n\n        // If there are no more children in the message, remove the remaining\n        // DOM children\n        if (curIdIndex >= childIds.length) {\n            while (curElement !== null) {\n                let nextElement = curElement.nextElementSibling;\n                latentWidgets.appendChild(curElement);\n                curElement = nextElement;\n            }\n            break;\n        }\n\n        // This element is the correct element, move on\n        let curId = childIds[curIdIndex];\n        if (curElement.id === `reflex-id-${curId}`) {\n            curElement = curElement.nextElementSibling;\n            curIdIndex++;\n            continue;\n        }\n\n        // This element is not the correct element, insert the correct one\n        // instead\n        let newElement = getElementByWidgetId(curId);\n        parentElement.insertBefore(newElement!, curElement);\n        curIdIndex++;\n    }\n}\n\nfunction requestFileUpload(message: any) {\n    // Create a file upload input element\n    let input = document.createElement('input');\n    input.type = 'file';\n    input.multiple = message.multiple;\n\n    if (message.fileExtensions !== null) {\n        input.accept = message.fileExtensions.join(',');\n    }\n\n    input.style.display = 'none';\n\n    function finish() {\n        // Don't run twice\n        if (input.parentElement === null) {\n            return;\n        }\n\n        // Build a `FormData` object containing the files\n        const data = new FormData();\n\n        let ii = 0;\n        for (const file of input.files || []) {\n            ii += 1;\n            data.append('file_names', file.name);\n            data.append('file_types', file.type);\n            data.append('file_sizes', file.size.toString());\n            data.append('file_streams', file, file.name);\n        }\n\n        // FastAPI has trouble parsing empty form data. Append a dummy value so\n        // it's never empty\n        data.append('dummy', 'dummy');\n\n        // Upload the files\n        fetch(message.uploadUrl, {\n            method: 'PUT',\n            body: data,\n        });\n\n        // Remove the input element from the DOM. Removing this too early causes\n        // weird behavior in some browsers\n        input.remove();\n    }\n\n    // Listen for changes to the input\n    input.addEventListener('change', finish);\n\n    // Detect if the window gains focus. This means the file upload dialog was\n    // closed without selecting a file\n    window.addEventListener(\n        'focus',\n        function () {\n            // In some browsers `focus` fires before `change`. Give `change`\n            // time to run first.\n            this.window.setTimeout(finish, 500);\n        },\n        { once: true }\n    );\n\n    // Add the input element to the DOM\n    document.body.appendChild(input);\n\n    // Trigger the file upload\n    input.click();\n}\n\nfunction main() {\n    // Determine the browser's font size\n    var measure = document.createElement('div');\n    measure.style.height = '10em';\n    document.body.appendChild(measure);\n    pixelsPerEm = measure.offsetHeight / 10;\n    document.body.removeChild(measure);\n\n    // Process initial messages\n    console.log(`Processing ${initialMessages.length} initial message(s)`);\n    for (let message of initialMessages) {\n        processMessage(message);\n    }\n\n    // Connect to the websocket\n    var url = new URL(\n        `/reflex/ws?sessionToken=${sessionToken}`,\n        window.location.href\n    );\n    url.protocol = url.protocol.replace('http', 'ws');\n    console.log(`Connecting websocket to ${url.href}`);\n    socket = new WebSocket(url.href);\n\n    socket.addEventListener('open', onOpen);\n    socket.addEventListener('message', onMessage);\n    socket.addEventListener('error', onError);\n    socket.addEventListener('close', onClose);\n}\n\nfunction onOpen() {\n    console.log('Connection opened');\n}\n\nfunction onMessage(event: any) {\n    // Parse the message JSON\n    let message = JSON.parse(event.data);\n\n    // Handle it\n    processMessage(message);\n}\n\nfunction onError(event: any) {\n    console.log(`Error: ${event.message}`);\n}\n\nfunction onClose(event: any) {\n    console.log(`Connection closed: ${event.reason}`);\n}\n\nexport function sendMessageOverWebsocket(message: object) {\n    if (!socket) {\n        console.log(\n            `Attempted to send message, but the websocket is not connected: ${message}`\n        );\n        return;\n    }\n\n    console.log('Sending message: ', message);\n\n    socket.send(JSON.stringify(message));\n}\n\nmain();\n"
     ],
     "version": 3
 }
```

### Comparing `reflex_ui-0.1.0/reflex/generated/style.css` & `reflex_ui-0.1.1/reflex/generated/style.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-:root{--color-dim:#ddd;--color-light:#eee;--color-font:#000;--color-accent:#e80265;--color-placeholder:#666;--corner-radius:0.4rem;--transition-slow:0.6s;--transition-med:0.2s;--transition-fast:0.1s}.reflex-single-container>*{width:100%;height:100%}body{width:100vw;height:100vh;margin:0;padding:0;font-family:Segoe UI,Tahoma,Geneva,Verdana,sans-serif;font-size:16px;background-color:#000}.reflex-widget{box-sizing:border-box}.reflex-align>*,.reflex-margin>*{position:relative}.reflex-column{flex-direction:column}.reflex-column,.reflex-row{display:flex;align-items:stretch}.reflex-row{flex-direction:row}.reflex-text{display:flex;align-items:center;justify-content:center}.reflex-rectangle{transition-timing-function:ease;background:var(--rectangle-background);border:var(--rectangle-stroke-width) solid var(--rectangle-stroke-color);border-radius:var(--rectangle-corner-radius-top-left) var(--rectangle-corner-radius-top-right) var(--rectangle-corner-radius-bottom-right) var(--rectangle-corner-radius-bottom-left);box-shadow:var(--rectangle-shadow-offset-x) var(--rectangle-shadow-offset-y) var(--rectangle-shadow-radius) var(--rectangle-shadow-color)}.reflex-rectangle-hover:hover{background:var(--rectangle-background-hover);border-color:var(--rectangle-stroke-color-hover);border-width:var(--rectangle-stroke-width-hover);border-radius:var(--rectangle-corner-radius-top-left-hover) var(--rectangle-corner-radius-top-right-hover) var(--rectangle-corner-radius-bottom-right-hover) var(--rectangle-corner-radius-bottom-left-hover);box-shadow:var(--rectangle-shadow-offset-x-hover) var(--rectangle-shadow-offset-y-hover) var(--rectangle-shadow-radius-hover) var(--rectangle-shadow-color-hover)}.reflex-stack>*{position:absolute;left:0;top:0;right:0;bottom:0}.reflex-text-input{min-height:1.2rem;background-color:var(--color-dim);color:#000;caret-color:var(--color-accent);border-radius:var(--corner-radius);border:1.5px solid transparent;padding:.7rem .5rem;text-align:center;outline:none;transition:background-color var(--transition-slow) ease-in-out;-moz-transition:background-color var(--transition-slow) ease-in-out;transition:border var(--transition-fast) ease-in-out;-moz-transition:border var(--transition-fast) ease-in-out}.reflex-text-input:focus,.reflex-text-input:hover{background-color:var(--color-light);border:1.5px solid var(--color-accent)}::placeholder{color:var(--color-placeholder)}.reflex-dropdown{min-height:2rem;background-color:var(--color-dim);color:#000;caret-color:var(--color-accent);border-radius:var(--corner-radius);border:1.5px solid transparent;padding:.3rem .5rem;text-align:center;outline:none}.reflex-dropdown:hover{background-color:var(--color-light);border:1.5px solid var(--color-accent)}.reflex-progress-circle{width:0;height:0}.reflex-progress-circle circle{fill:none;stroke-width:3.5}.spinning svg{transform-origin:center;animation:rotate 2s linear infinite}.spinning .progress{stroke-dasharray:1,200;stroke-dashoffset:0;stroke-linecap:round;animation:dash 1.5s ease-in-out infinite}.spinning .background{stroke:none}.reflex-progress-circle:not(.spinning) .progress{stroke-dashoffset:-94.25;stroke-dasharray:var(--dasharray);transition:stroke-dasharray .5s ease}.reflex-progress-circle:not(.spinning) .background{stroke:var(--background-color)}@keyframes rotate{to{transform:rotate(1turn)}}@keyframes dash{0%{stroke-dasharray:1,200;stroke-dashoffset:0}50%{stroke-dasharray:90,200;stroke-dashoffset:-35px}to{stroke-dashoffset:-125px}}.reflex-switch .container{position:relative;width:3.182em;height:1.548em;margin:auto;border-radius:4.3em;background-color:var(--switch-background-color-off);transition:all .3s ease;z-index:1}.reflex-switch.is-on .container{background-color:var(--switch-background-color-on)}.reflex-switch input{position:relative;width:100%;height:100%;padding:0;margin:0;opacity:0;cursor:pointer;z-index:3}.reflex-switch .knob{z-index:2;position:absolute;top:.172em;left:.172em;width:.86em;height:.43em;padding:.387em .172em;background-color:var(--switch-knob-color-off);border-radius:50%;transition:all .3s ease,left .3s cubic-bezier(.18,.89,.35,1.15)}.reflex-switch input:active+.knob{width:1.978em;border-radius:4.3em}.reflex-switch.is-on input:active+.knob{margin-left:-1.118em}.reflex-switch.is-on input+.knob{left:1.806em;background-color:var(--switch-knob-color-on)}
+:root{--color-dim:#ddd;--color-light:#eee;--color-font:#000;--color-accent:#e80265;--color-placeholder:#666;--corner-radius:0.4rem;--transition-slow:0.6s;--transition-med:0.2s;--transition-fast:0.1s}.reflex-single-container>*{width:100%;height:100%}body{width:100vw;height:100vh;margin:0;padding:0;font-family:Segoe UI,Tahoma,Geneva,Verdana,sans-serif;font-size:16px}.reflex-widget{box-sizing:border-box}.reflex-align>*,.reflex-margin>*{position:relative}.reflex-column{flex-direction:column}.reflex-column,.reflex-row{display:flex;align-items:stretch}.reflex-row{flex-direction:row}.reflex-text{display:flex;align-items:center;justify-content:center}.reflex-rectangle{transition-timing-function:ease;background:var(--rectangle-background);border:var(--rectangle-stroke-width) solid var(--rectangle-stroke-color);border-radius:var(--rectangle-corner-radius-top-left) var(--rectangle-corner-radius-top-right) var(--rectangle-corner-radius-bottom-right) var(--rectangle-corner-radius-bottom-left);box-shadow:var(--rectangle-shadow-offset-x) var(--rectangle-shadow-offset-y) var(--rectangle-shadow-radius) var(--rectangle-shadow-color)}.reflex-rectangle-hover:hover{background:var(--rectangle-background-hover);border-color:var(--rectangle-stroke-color-hover);border-width:var(--rectangle-stroke-width-hover);border-radius:var(--rectangle-corner-radius-top-left-hover) var(--rectangle-corner-radius-top-right-hover) var(--rectangle-corner-radius-bottom-right-hover) var(--rectangle-corner-radius-bottom-left-hover);box-shadow:var(--rectangle-shadow-offset-x-hover) var(--rectangle-shadow-offset-y-hover) var(--rectangle-shadow-radius-hover) var(--rectangle-shadow-color-hover)}.reflex-stack>*{position:absolute;left:0;top:0;right:0;bottom:0}.reflex-text-input{min-height:1.2rem;background-color:var(--color-dim);color:#000;caret-color:var(--color-accent);border-radius:var(--corner-radius);border:1.5px solid transparent;padding:.7rem .5rem;text-align:center;outline:none;transition:background-color var(--transition-slow) ease-in-out;-moz-transition:background-color var(--transition-slow) ease-in-out;transition:border var(--transition-fast) ease-in-out;-moz-transition:border var(--transition-fast) ease-in-out}.reflex-text-input:focus,.reflex-text-input:hover{background-color:var(--color-light);border:1.5px solid var(--color-accent)}::placeholder{color:var(--color-placeholder)}.reflex-dropdown{min-height:2rem;background-color:var(--color-dim);color:#000;caret-color:var(--color-accent);border-radius:var(--corner-radius);border:1.5px solid transparent;padding:.3rem .5rem;text-align:center;outline:none}.reflex-dropdown:hover{background-color:var(--color-light);border:1.5px solid var(--color-accent)}.reflex-progress-circle{width:0;height:0}.reflex-progress-circle circle{fill:none;stroke-width:3.5}.spinning svg{transform-origin:center;animation:rotate 2s linear infinite}.spinning .progress{stroke-dasharray:1,200;stroke-dashoffset:0;stroke-linecap:round;animation:dash 1.5s ease-in-out infinite}.spinning .background{stroke:none}.reflex-progress-circle:not(.spinning) .progress{stroke-dashoffset:-94.25;stroke-dasharray:var(--dasharray);transition:stroke-dasharray .5s ease}.reflex-progress-circle:not(.spinning) .background{stroke:var(--background-color)}@keyframes rotate{to{transform:rotate(1turn)}}@keyframes dash{0%{stroke-dasharray:1,200;stroke-dashoffset:0}50%{stroke-dasharray:90,200;stroke-dashoffset:-35px}to{stroke-dashoffset:-125px}}.reflex-switch .container{position:relative;width:3.182em;height:1.548em;margin:auto;border-radius:4.3em;background-color:var(--switch-background-color-off);transition:all .3s ease;z-index:1}.reflex-switch.is-on .container{background-color:var(--switch-background-color-on)}.reflex-switch input{position:relative;width:100%;height:100%;padding:0;margin:0;opacity:0;cursor:pointer;z-index:3}.reflex-switch .knob{z-index:2;position:absolute;top:.172em;left:.172em;width:.86em;height:.43em;padding:.387em .172em;background-color:var(--switch-knob-color-off);border-radius:50%;transition:all .3s ease,left .3s cubic-bezier(.18,.89,.35,1.15)}.reflex-switch input:active+.knob{width:1.978em;border-radius:4.3em}.reflex-switch.is-on input:active+.knob{margin-left:-1.118em}.reflex-switch.is-on input+.knob{left:1.806em;background-color:var(--switch-knob-color-on)}
 /*# sourceMappingURL=/style.css.map */
```

### Comparing `reflex_ui-0.1.0/reflex/generated/style.css.map` & `reflex_ui-0.1.1/reflex/generated/style.css.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'mappings'": "'AAAA,MACI,gBAAA,CACA,kBAAA,CACA,iBAAA,CACA,sBAAA,CACA,wBAAA,CAEA,sBAAA,CAEA,sBAAA,CACA,qBAAA,CACA,uBAGJ,2BACI,UAAA,CACA,YAGJ,KACI,WAAA,CACA,YAAA,CACA,QAAA,CACA,SAAA,CACA,qDAAA,CACA,eAGJ,eACI,sBAOJ,iCACI,kBAGJ,eAEI,sBAIJ,2BALI,YAAA,CAEA,oBAGJ,YAEI,mBAIJ,aACI,YAAA,CACA,kBAAA,CACA,uBAGJ,kBAGI,+BAAA,CAMA,sCAAA,CAEA,wEAAA,CACA,qLAAA,CAIA,0IAKJ,8BACI,4CAAA,CACA,gDAAA,CACA,gDAAA,CACA,6MAAA,CAIA,kKAKJ,gBACI,iBAAA,CAEA,MAAA,CACA,KAAA,CACA,OAAA,CACA,SAKJ,mBACI,iBAAA,CAEA,iCAAA,CACA,UAAA,CACA,+BAAA,CA […]*

```diff
@@ -1,13 +1,13 @@
 {
     "file": "style.css",
-    "mappings": "AAAA,MACI,gBAAA,CACA,kBAAA,CACA,iBAAA,CACA,sBAAA,CACA,wBAAA,CAEA,sBAAA,CAEA,sBAAA,CACA,qBAAA,CACA,uBAGJ,2BACI,UAAA,CACA,YAGJ,KACI,WAAA,CACA,YAAA,CACA,QAAA,CACA,SAAA,CACA,qDAAA,CACA,cAAA,CACA,sBAGJ,eACI,sBAOJ,iCACI,kBAGJ,eAEI,sBAIJ,2BALI,YAAA,CAEA,oBAGJ,YAEI,mBAIJ,aACI,YAAA,CACA,kBAAA,CACA,uBAGJ,kBAGI,+BAAA,CAMA,sCAAA,CAEA,wEAAA,CACA,qLAAA,CAIA,0IAKJ,8BACI,4CAAA,CACA,gDAAA,CACA,gDAAA,CACA,6MAAA,CAIA,kKAKJ,gBACI,iBAAA,CAEA,MAAA,CACA,KAAA,CACA,OAAA,CACA,SAKJ,mBACI,iBAAA,CAEA,iCAAA,CACA,UAAA,CACA,+BAAA,CAEA,kCAAA,CACA,8BAAA,CAEA,mBAAA,CACA,iBAAA,CACA,YAAA,CAEA,8DAAA,CACA,mEAAA,CAEA,oDAAA,CACA,0DAQJ,kDACI,mCAAA,CACA,uCAGJ,cACI,+BAIJ,iBACI,eAAA,CAEA,iCAAA,CACA,UAAA,CACA,+BAAA,CAEA,kCAAA,CACA,8BAAA,CAEA,mBAAA,CACA,iBAAA,CACA,aAGJ,uBACI,mCAAA,CACA,uCAIJ,wBACI,OAAA,CACA,SAGJ,+BACI,SAAA,CACA,iBAGJ,cACI,uBAAA,CACA,oCAGJ,oBACI,sBAAA,CACA,mBAAA,CACA,oBAAA,CACA,yCAGJ,sBACI,YAGJ,iDACI,wBAAA,CACA,iCAAA,CACA,qCAGJ,mDACI,+BAGJ,kBACI,GACI,yBAIR,gBACI,GACI,sBAAA,CACA,oBAEJ,IACI,uBAAA,CACA,wBAEJ,GACI,0BAIR,0BACI,iBAAA,CACA,aAAA,CACA,cAAA,CACA,WAAA,CACA,mBAAA,CACA,mDAAA,CACA,uBAAA,CACA,UAGJ,gCACI,mDAGJ,qBACI,iBAAA,CACA,UAAA,CACA,WAAA,CACA,SAAA,CACA,QAAA,CACA,SAAA,CACA,cAAA,CACA,UAGJ,qBACI,SAAA,CACA,iBAAA,CACA,UAAA,CACA,WAAA,CACA,WAAA,CACA,YAAA,CACA,qBAAA,CACA,6CAAA,CACA,iBAAA,CACA,gEAGJ,kCACI,aAAA,CACA,oBAGJ,wCACI,qBAGJ,iCACI,YAAA,CACA",
+    "mappings": "AAAA,MACI,gBAAA,CACA,kBAAA,CACA,iBAAA,CACA,sBAAA,CACA,wBAAA,CAEA,sBAAA,CAEA,sBAAA,CACA,qBAAA,CACA,uBAGJ,2BACI,UAAA,CACA,YAGJ,KACI,WAAA,CACA,YAAA,CACA,QAAA,CACA,SAAA,CACA,qDAAA,CACA,eAGJ,eACI,sBAOJ,iCACI,kBAGJ,eAEI,sBAIJ,2BALI,YAAA,CAEA,oBAGJ,YAEI,mBAIJ,aACI,YAAA,CACA,kBAAA,CACA,uBAGJ,kBAGI,+BAAA,CAMA,sCAAA,CAEA,wEAAA,CACA,qLAAA,CAIA,0IAKJ,8BACI,4CAAA,CACA,gDAAA,CACA,gDAAA,CACA,6MAAA,CAIA,kKAKJ,gBACI,iBAAA,CAEA,MAAA,CACA,KAAA,CACA,OAAA,CACA,SAKJ,mBACI,iBAAA,CAEA,iCAAA,CACA,UAAA,CACA,+BAAA,CAEA,kCAAA,CACA,8BAAA,CAEA,mBAAA,CACA,iBAAA,CACA,YAAA,CAEA,8DAAA,CACA,mEAAA,CAEA,oDAAA,CACA,0DAQJ,kDACI,mCAAA,CACA,uCAGJ,cACI,+BAIJ,iBACI,eAAA,CAEA,iCAAA,CACA,UAAA,CACA,+BAAA,CAEA,kCAAA,CACA,8BAAA,CAEA,mBAAA,CACA,iBAAA,CACA,aAGJ,uBACI,mCAAA,CACA,uCAIJ,wBACI,OAAA,CACA,SAGJ,+BACI,SAAA,CACA,iBAGJ,cACI,uBAAA,CACA,oCAGJ,oBACI,sBAAA,CACA,mBAAA,CACA,oBAAA,CACA,yCAGJ,sBACI,YAGJ,iDACI,wBAAA,CACA,iCAAA,CACA,qCAGJ,mDACI,+BAGJ,kBACI,GACI,yBAIR,gBACI,GACI,sBAAA,CACA,oBAEJ,IACI,uBAAA,CACA,wBAEJ,GACI,0BAIR,0BACI,iBAAA,CACA,aAAA,CACA,cAAA,CACA,WAAA,CACA,mBAAA,CACA,mDAAA,CACA,uBAAA,CACA,UAGJ,gCACI,mDAGJ,qBACI,iBAAA,CACA,UAAA,CACA,WAAA,CACA,SAAA,CACA,QAAA,CACA,SAAA,CACA,cAAA,CACA,UAGJ,qBACI,SAAA,CACA,iBAAA,CACA,UAAA,CACA,WAAA,CACA,WAAA,CACA,YAAA,CACA,qBAAA,CACA,6CAAA,CACA,iBAAA,CACA,gEAGJ,kCACI,aAAA,CACA,oBAGJ,wCACI,qBAGJ,iCACI,YAAA,CACA",
     "names": [],
     "sourceRoot": "../../frontend",
     "sources": [
         "style.scss"
     ],
     "sourcesContent": [
-        ":root {\n    --color-dim: #dddddd;\n    --color-light: #eeeeee;\n    --color-font: #000000;\n    --color-accent: #e80265;\n    --color-placeholder: #666666;\n\n    --corner-radius: 0.4rem;\n\n    --transition-slow: 0.6s;\n    --transition-med: 0.2s;\n    --transition-fast: 0.1s;\n}\n\n.reflex-single-container > * {\n    width: 100%;\n    height: 100%;\n}\n\nbody {\n    width: 100vw;\n    height: 100vh;\n    margin: 0;\n    padding: 0;\n    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;\n    font-size: 16px;\n    background-color: black;\n}\n\n.reflex-widget {\n    box-sizing: border-box;\n}\n\n.reflex-align > * {\n    position: relative;\n}\n\n.reflex-margin > * {\n    position: relative;\n}\n\n.reflex-column {\n    display: flex;\n    flex-direction: column;\n    align-items: stretch;\n}\n\n.reflex-row {\n    display: flex;\n    flex-direction: row;\n    align-items: stretch;\n}\n\n.reflex-text {\n    display: flex;\n    align-items: center;\n    justify-content: center;\n}\n\n.reflex-rectangle {\n    border-style: solid;\n\n    transition-timing-function: ease; /* The transition time is set via JS */\n\n    /*\n    The following attributes are controlled via variables, to allow JavaScript\n    to change them, even on pseudo-classes.\n    */\n    background: var(--rectangle-background);\n    border-color: var(--rectangle-stroke-color);\n    border-width: var(--rectangle-stroke-width);\n    border-radius: var(--rectangle-corner-radius-top-left)\n        var(--rectangle-corner-radius-top-right)\n        var(--rectangle-corner-radius-bottom-right)\n        var(--rectangle-corner-radius-bottom-left);\n    box-shadow: var(--rectangle-shadow-offset-x)\n        var(--rectangle-shadow-offset-y) var(--rectangle-shadow-radius)\n        var(--rectangle-shadow-color);\n}\n\n.reflex-rectangle-hover:hover {\n    background: var(--rectangle-background-hover);\n    border-color: var(--rectangle-stroke-color-hover);\n    border-width: var(--rectangle-stroke-width-hover);\n    border-radius: var(--rectangle-corner-radius-top-left-hover)\n        var(--rectangle-corner-radius-top-right-hover)\n        var(--rectangle-corner-radius-bottom-right-hover)\n        var(--rectangle-corner-radius-bottom-left-hover);\n    box-shadow: var(--rectangle-shadow-offset-x-hover)\n        var(--rectangle-shadow-offset-y-hover)\n        var(--rectangle-shadow-radius-hover) var(--rectangle-shadow-color-hover);\n}\n\n.reflex-stack > * {\n    position: absolute;\n\n    left: 0;\n    top: 0;\n    right: 0;\n    bottom: 0;\n}\n\n/* Text Input */\n\n.reflex-text-input {\n    min-height: 1.2rem;\n\n    background-color: var(--color-dim);\n    color: black;\n    caret-color: var(--color-accent);\n\n    border-radius: var(--corner-radius);\n    border: 1.5px solid transparent;\n\n    padding: 0.7rem 0.5rem;\n    text-align: center;\n    outline: none;\n\n    transition: background-color var(--transition-slow) ease-in-out;\n    -moz-transition: background-color var(--transition-slow) ease-in-out;\n\n    transition: border var(--transition-fast) ease-in-out;\n    -moz-transition: border var(--transition-fast) ease-in-out;\n}\n\n.reflex-text-input:hover {\n    background-color: var(--color-light);\n    border: 1.5px solid var(--color-accent);\n}\n\n.reflex-text-input:focus {\n    background-color: var(--color-light);\n    border: 1.5px solid var(--color-accent);\n}\n\n::placeholder {\n    color: var(--color-placeholder);\n}\n\n/* Dropdown */\n.reflex-dropdown {\n    min-height: 2rem;\n\n    background-color: var(--color-dim);\n    color: black;\n    caret-color: var(--color-accent);\n\n    border-radius: var(--corner-radius);\n    border: 1.5px solid transparent;\n\n    padding: 0.3rem 0.5rem;\n    text-align: center;\n    outline: none;\n}\n\n.reflex-dropdown:hover {\n    background-color: var(--color-light);\n    border: 1.5px solid var(--color-accent);\n}\n\n/* Loading Circle */\n.reflex-progress-circle {\n    width: 0;\n    height: 0;\n}\n\n.reflex-progress-circle circle {\n    fill: none;\n    stroke-width: 3.5;\n}\n\n.spinning svg {\n    transform-origin: center;\n    animation: rotate 2s linear infinite;\n}\n\n.spinning .progress {\n    stroke-dasharray: 1, 200;\n    stroke-dashoffset: 0;\n    stroke-linecap: round;\n    animation: dash 1.5s ease-in-out infinite;\n}\n\n.spinning .background {\n    stroke: none;\n}\n\n.reflex-progress-circle:not(.spinning) .progress {\n    stroke-dashoffset: -94.25;\n    stroke-dasharray: var(--dasharray);\n    transition: stroke-dasharray 0.5s ease;\n}\n\n.reflex-progress-circle:not(.spinning) .background {\n    stroke: var(--background-color);\n}\n\n@keyframes rotate {\n    100% {\n        transform: rotate(360deg);\n    }\n}\n\n@keyframes dash {\n    0% {\n        stroke-dasharray: 1, 200;\n        stroke-dashoffset: 0;\n    }\n    50% {\n        stroke-dasharray: 90, 200;\n        stroke-dashoffset: -35px;\n    }\n    100% {\n        stroke-dashoffset: -125px;\n    }\n}\n\n.reflex-switch .container {\n    position: relative;\n    width: 3.182em;\n    height: 1.548em;\n    margin: auto;\n    border-radius: 4.3em;\n    background-color: var(--switch-background-color-off);\n    transition: 0.3s ease all;\n    z-index: 1;\n}\n\n.reflex-switch.is-on .container {\n    background-color: var(--switch-background-color-on);\n}\n\n.reflex-switch input {\n    position: relative;\n    width: 100%;\n    height: 100%;\n    padding: 0;\n    margin: 0;\n    opacity: 0;\n    cursor: pointer;\n    z-index: 3;\n}\n\n.reflex-switch .knob {\n    z-index: 2;\n    position: absolute;\n    top: 0.172em;\n    left: 0.172em;\n    width: 0.86em;\n    height: 0.43em;\n    padding: 0.387em 0.172em;\n    background-color: var(--switch-knob-color-off);\n    border-radius: 50%;\n    transition: 0.3s ease all, left 0.3s cubic-bezier(0.18, 0.89, 0.35, 1.15);\n}\n\n.reflex-switch input:active + .knob {\n    width: 1.978em;\n    border-radius: 4.3em;\n}\n\n.reflex-switch.is-on input:active + .knob {\n    margin-left: -1.118em;\n}\n\n.reflex-switch.is-on input + .knob {\n    left: 1.806em;\n    background-color: var(--switch-knob-color-on);\n}\n"
+        ":root {\n    --color-dim: #dddddd;\n    --color-light: #eeeeee;\n    --color-font: #000000;\n    --color-accent: #e80265;\n    --color-placeholder: #666666;\n\n    --corner-radius: 0.4rem;\n\n    --transition-slow: 0.6s;\n    --transition-med: 0.2s;\n    --transition-fast: 0.1s;\n}\n\n.reflex-single-container > * {\n    width: 100%;\n    height: 100%;\n}\n\nbody {\n    width: 100vw;\n    height: 100vh;\n    margin: 0;\n    padding: 0;\n    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;\n    font-size: 16px;\n}\n\n.reflex-widget {\n    box-sizing: border-box;\n}\n\n.reflex-align > * {\n    position: relative;\n}\n\n.reflex-margin > * {\n    position: relative;\n}\n\n.reflex-column {\n    display: flex;\n    flex-direction: column;\n    align-items: stretch;\n}\n\n.reflex-row {\n    display: flex;\n    flex-direction: row;\n    align-items: stretch;\n}\n\n.reflex-text {\n    display: flex;\n    align-items: center;\n    justify-content: center;\n}\n\n.reflex-rectangle {\n    border-style: solid;\n\n    transition-timing-function: ease; /* The transition time is set via JS */\n\n    /*\n    The following attributes are controlled via variables, to allow JavaScript\n    to change them, even on pseudo-classes.\n    */\n    background: var(--rectangle-background);\n    border-color: var(--rectangle-stroke-color);\n    border-width: var(--rectangle-stroke-width);\n    border-radius: var(--rectangle-corner-radius-top-left)\n        var(--rectangle-corner-radius-top-right)\n        var(--rectangle-corner-radius-bottom-right)\n        var(--rectangle-corner-radius-bottom-left);\n    box-shadow: var(--rectangle-shadow-offset-x)\n        var(--rectangle-shadow-offset-y) var(--rectangle-shadow-radius)\n        var(--rectangle-shadow-color);\n}\n\n.reflex-rectangle-hover:hover {\n    background: var(--rectangle-background-hover);\n    border-color: var(--rectangle-stroke-color-hover);\n    border-width: var(--rectangle-stroke-width-hover);\n    border-radius: var(--rectangle-corner-radius-top-left-hover)\n        var(--rectangle-corner-radius-top-right-hover)\n        var(--rectangle-corner-radius-bottom-right-hover)\n        var(--rectangle-corner-radius-bottom-left-hover);\n    box-shadow: var(--rectangle-shadow-offset-x-hover)\n        var(--rectangle-shadow-offset-y-hover)\n        var(--rectangle-shadow-radius-hover) var(--rectangle-shadow-color-hover);\n}\n\n.reflex-stack > * {\n    position: absolute;\n\n    left: 0;\n    top: 0;\n    right: 0;\n    bottom: 0;\n}\n\n/* Text Input */\n\n.reflex-text-input {\n    min-height: 1.2rem;\n\n    background-color: var(--color-dim);\n    color: black;\n    caret-color: var(--color-accent);\n\n    border-radius: var(--corner-radius);\n    border: 1.5px solid transparent;\n\n    padding: 0.7rem 0.5rem;\n    text-align: center;\n    outline: none;\n\n    transition: background-color var(--transition-slow) ease-in-out;\n    -moz-transition: background-color var(--transition-slow) ease-in-out;\n\n    transition: border var(--transition-fast) ease-in-out;\n    -moz-transition: border var(--transition-fast) ease-in-out;\n}\n\n.reflex-text-input:hover {\n    background-color: var(--color-light);\n    border: 1.5px solid var(--color-accent);\n}\n\n.reflex-text-input:focus {\n    background-color: var(--color-light);\n    border: 1.5px solid var(--color-accent);\n}\n\n::placeholder {\n    color: var(--color-placeholder);\n}\n\n/* Dropdown */\n.reflex-dropdown {\n    min-height: 2rem;\n\n    background-color: var(--color-dim);\n    color: black;\n    caret-color: var(--color-accent);\n\n    border-radius: var(--corner-radius);\n    border: 1.5px solid transparent;\n\n    padding: 0.3rem 0.5rem;\n    text-align: center;\n    outline: none;\n}\n\n.reflex-dropdown:hover {\n    background-color: var(--color-light);\n    border: 1.5px solid var(--color-accent);\n}\n\n/* Loading Circle */\n.reflex-progress-circle {\n    width: 0;\n    height: 0;\n}\n\n.reflex-progress-circle circle {\n    fill: none;\n    stroke-width: 3.5;\n}\n\n.spinning svg {\n    transform-origin: center;\n    animation: rotate 2s linear infinite;\n}\n\n.spinning .progress {\n    stroke-dasharray: 1, 200;\n    stroke-dashoffset: 0;\n    stroke-linecap: round;\n    animation: dash 1.5s ease-in-out infinite;\n}\n\n.spinning .background {\n    stroke: none;\n}\n\n.reflex-progress-circle:not(.spinning) .progress {\n    stroke-dashoffset: -94.25;\n    stroke-dasharray: var(--dasharray);\n    transition: stroke-dasharray 0.5s ease;\n}\n\n.reflex-progress-circle:not(.spinning) .background {\n    stroke: var(--background-color);\n}\n\n@keyframes rotate {\n    100% {\n        transform: rotate(360deg);\n    }\n}\n\n@keyframes dash {\n    0% {\n        stroke-dasharray: 1, 200;\n        stroke-dashoffset: 0;\n    }\n    50% {\n        stroke-dasharray: 90, 200;\n        stroke-dashoffset: -35px;\n    }\n    100% {\n        stroke-dashoffset: -125px;\n    }\n}\n\n.reflex-switch .container {\n    position: relative;\n    width: 3.182em;\n    height: 1.548em;\n    margin: auto;\n    border-radius: 4.3em;\n    background-color: var(--switch-background-color-off);\n    transition: 0.3s ease all;\n    z-index: 1;\n}\n\n.reflex-switch.is-on .container {\n    background-color: var(--switch-background-color-on);\n}\n\n.reflex-switch input {\n    position: relative;\n    width: 100%;\n    height: 100%;\n    padding: 0;\n    margin: 0;\n    opacity: 0;\n    cursor: pointer;\n    z-index: 3;\n}\n\n.reflex-switch .knob {\n    z-index: 2;\n    position: absolute;\n    top: 0.172em;\n    left: 0.172em;\n    width: 0.86em;\n    height: 0.43em;\n    padding: 0.387em 0.172em;\n    background-color: var(--switch-knob-color-off);\n    border-radius: 50%;\n    transition: 0.3s ease all, left 0.3s cubic-bezier(0.18, 0.89, 0.35, 1.15);\n}\n\n.reflex-switch input:active + .knob {\n    width: 1.978em;\n    border-radius: 4.3em;\n}\n\n.reflex-switch.is-on input:active + .knob {\n    margin-left: -1.118em;\n}\n\n.reflex-switch.is-on input + .knob {\n    left: 1.806em;\n    background-color: var(--switch-knob-color-on);\n}\n"
     ],
     "version": 3
 }
```

### Comparing `reflex_ui-0.1.0/reflex/hosted-assets/showdown.min.js` & `reflex_ui-0.1.1/reflex/hosted-assets/showdown.min.js`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/image_source.py` & `reflex_ui-0.1.1/reflex/image_source.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/messages.py` & `reflex_ui-0.1.1/reflex/messages.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/session.py` & `reflex_ui-0.1.1/reflex/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 from __future__ import annotations
 
-import inspect
-import uniserde
+import asyncio
 import enum
-import logging
+import inspect
 import json
+import logging
 import secrets
 import sys
-import logging
-from . import errors
-import asyncio
-from . import common
 import typing
-from . import styling
 import weakref
 from dataclasses import dataclass
-from typing import *  #  type: ignore
-from . import assets
+from typing import *  # type: ignore
+
+import uniserde
 
 import reflex as rx
 
-from . import app_server, messages
+from . import app_server, assets, common, errors, messages, styling
 from .common import Jsonable
 from .widgets import widget_base
 
-
 __all__ = ["Session"]
 
 
 T = typing.TypeVar("T")
 
 
 def _get_type_hints(cls: type) -> Dict[str, type]:
     """
     Reimplementation of `typing.get_type_hints` because it has a stupid bug in
     python 3.10 where it dies if something is annotated as `dataclasses.KW_ONLY`.
     """
     type_hints = {}
 
     for cls in cls.__mro__:
-        for attr_name, annotation in vars(cls).get('__annotations__', {}).items():
+        for attr_name, annotation in vars(cls).get("__annotations__", {}).items():
             if attr_name in type_hints:
                 continue
 
             if isinstance(annotation, typing.ForwardRef):
                 annotation = annotation.__forward_code__
 
             if isinstance(annotation, str):
@@ -527,24 +522,24 @@
         result["_margin_"] = (
             widget.margin_left,
             widget.margin_top,
             widget.margin_right,
             widget.margin_bottom,
         )
         result["_size_"] = (
-            widget.width,
-            widget.height,
+            widget.width if isinstance(widget.width, (int, float)) else None,
+            widget.height if isinstance(widget.height, (int, float)) else None,
         )
         result["_align_"] = (
             widget.align_x,
             widget.align_y,
         )
         result["_grow_"] = (
-            widget.grow_x,
-            widget.grow_y,
+            widget.width == "grow",
+            widget.height == "grow",
         )
 
         # Add user-defined state
         for name, type_ in _get_type_hints(type(widget)).items():
             # Skip some values
             if name in (
                 "_",
```

### Comparing `reflex_ui-0.1.0/reflex/styling/box_style.py` & `reflex_ui-0.1.1/reflex/styling/box_style.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/styling/color.py` & `reflex_ui-0.1.1/reflex/styling/color.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/styling/fills.py` & `reflex_ui-0.1.1/reflex/styling/fills.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/styling/markdown_style.py` & `reflex_ui-0.1.1/reflex/styling/markdown_style.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/styling/text_style.py` & `reflex_ui-0.1.1/reflex/styling/text_style.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/validator.py` & `reflex_ui-0.1.1/reflex/validator.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/auto_form.py` & `reflex_ui-0.1.1/reflex/widgets/auto_form.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/button.py` & `reflex_ui-0.1.1/reflex/widgets/button.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import KW_ONLY
-from .. import common
-
-from .. import styling
+from typing import *  # type: ignore
 from typing import Optional
 
 import reflex as rx
 
-from .. import theme
+from .. import common, styling, theme
 from . import widget_base
 
 __all__ = [
     "Button",
     "ButtonPressedEvent",
 ]
 
@@ -53,20 +51,18 @@
         margin: Optional[float] = None,
         margin_x: Optional[float] = None,
         margin_y: Optional[float] = None,
         margin_left: Optional[float] = None,
         margin_top: Optional[float] = None,
         margin_right: Optional[float] = None,
         margin_bottom: Optional[float] = None,
-        width: Optional[float] = None,
-        height: Optional[float] = None,
+        width: Union[Literal["natural", "grow"], float] = "natural",
+        height: Union[Literal["natural", "grow"], float] = "natural",
         align_x: Optional[float] = None,
         align_y: Optional[float] = None,
-        grow_x: bool = False,
-        grow_y: bool = False,
     ):
         return cls(
             text,
             on_press,
             is_sensitive=is_sensitive,
             is_loading=is_loading,
             style=rx.BoxStyle(
@@ -109,16 +105,14 @@
             margin_top=margin_top,
             margin_right=margin_right,
             margin_bottom=margin_bottom,
             width=width,
             height=height,
             align_x=align_x,
             align_y=align_y,
-            grow_x=grow_x,
-            grow_y=grow_y,
         )
 
     @classmethod
     def minor(
         cls,
         text: str,
         on_press: rx.EventHandler[ButtonPressedEvent] = None,
@@ -130,20 +124,18 @@
         margin: Optional[float] = None,
         margin_x: Optional[float] = None,
         margin_y: Optional[float] = None,
         margin_left: Optional[float] = None,
         margin_top: Optional[float] = None,
         margin_right: Optional[float] = None,
         margin_bottom: Optional[float] = None,
-        width: Optional[float] = None,
-        height: Optional[float] = None,
+        width: Union[Literal["natural", "grow"], float] = "natural",
+        height: Union[Literal["natural", "grow"], float] = "natural",
         align_x: Optional[float] = None,
         align_y: Optional[float] = None,
-        grow_x: bool = False,
-        grow_y: bool = False,
     ):
         base_style = rx.BoxStyle(
             fill=styling.Color.TRANSPARENT,
             corner_radius=theme.CORNER_RADIUS,
             stroke_width=theme.OUTLINE_WIDTH,
             stroke_color=accent_color,
         )
@@ -186,16 +178,14 @@
             margin_top=margin_top,
             margin_right=margin_right,
             margin_bottom=margin_bottom,
             width=width,
             height=height,
             align_x=align_x,
             align_y=align_y,
-            grow_x=grow_x,
-            grow_y=grow_y,
         )
 
     def _on_mouse_enter(self, event: rx.MouseEnterEvent) -> None:
         self._is_entered = True
 
     def _on_mouse_leave(self, event: rx.MouseLeaveEvent) -> None:
         self._is_entered = False
```

### Comparing `reflex_ui-0.1.0/reflex/widgets/column.py` & `reflex_ui-0.1.1/reflex/widgets/column.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from typing import *  # type: ignore
+
 import reflex as rx
 
 from . import widget_base
 
 __all__ = [
     "Column",
 ]
@@ -22,20 +23,18 @@
         margin: Optional[float] = None,
         margin_x: Optional[float] = None,
         margin_y: Optional[float] = None,
         margin_left: Optional[float] = None,
         margin_top: Optional[float] = None,
         margin_right: Optional[float] = None,
         margin_bottom: Optional[float] = None,
-        width: Optional[float] = None,
-        height: Optional[float] = None,
+        width: Union[Literal["natural", "grow"], float] = "natural",
+        height: Union[Literal["natural", "grow"], float] = "natural",
         align_x: Optional[float] = None,
         align_y: Optional[float] = None,
-        grow_x: bool = False,
-        grow_y: bool = False,
     ):
         assert isinstance(children, tuple), children
         for child in children:
             assert isinstance(child, widget_base.Widget), child
 
         super().__init__(
             key=key,
@@ -46,16 +45,14 @@
             margin_top=margin_top,
             margin_right=margin_right,
             margin_bottom=margin_bottom,
             width=width,
             height=height,
             align_x=align_x,
             align_y=align_y,
-            grow_x=grow_x,
-            grow_y=grow_y,
         )
 
         self.children = list(children)
         self.spacing = spacing
 
 
 Column._unique_id = "Column-builtin"
```

### Comparing `reflex_ui-0.1.0/reflex/widgets/dropdown.py` & `reflex_ui-0.1.1/reflex/widgets/dropdown.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/markdown_view.py` & `reflex_ui-0.1.1/reflex/widgets/markdown_view.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/media_player.py` & `reflex_ui-0.1.1/reflex/widgets/media_player.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/metadata.py` & `reflex_ui-0.1.1/reflex/widgets/metadata.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/mouse_event_listener.py` & `reflex_ui-0.1.1/reflex/widgets/mouse_event_listener.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/progress_circle.py` & `reflex_ui-0.1.1/reflex/widgets/progress_circle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 from __future__ import annotations
 
-from typing import Optional
-from .. import theme
-import reflex as rx
 from dataclasses import KW_ONLY
+from typing import *  # type: ignore
+
+import reflex as rx
 
+from .. import styling, theme
 from . import widget_base
-from .. import styling
 
 __all__ = [
     "ProgressCircle",
 ]
 
+
 class ProgressCircle(widget_base.HtmlWidget):
     _: KW_ONLY
     color: styling.Color = theme.COLOR_ACCENT
     background_color: styling.Color = theme.COLOR_NEUTRAL
     progress: Optional[float] = None
 
     def __init__(
         self,
         *,
         color: rx.Color = theme.COLOR_ACCENT,
         background_color: rx.Color = theme.COLOR_NEUTRAL,
         progress: Optional[float] = None,
-        size: float = 3.5,
+        size: Union[Literal["grow"], float] = 3.5,
         key: Optional[str] = None,
         margin: Optional[float] = None,
         margin_x: Optional[float] = None,
         margin_y: Optional[float] = None,
         margin_left: Optional[float] = None,
         margin_top: Optional[float] = None,
         margin_right: Optional[float] = None,
         margin_bottom: Optional[float] = None,
         align_x: Optional[float] = None,
         align_y: Optional[float] = None,
-        grow_x: bool = False,
-        grow_y: bool = False,
     ):
         super().__init__(
             key=key,
             margin=margin,
             margin_x=margin_x,
             margin_y=margin_y,
             margin_left=margin_left,
             margin_top=margin_top,
             margin_right=margin_right,
             margin_bottom=margin_bottom,
             width=size,
             height=size,
             align_x=align_x,
             align_y=align_y,
-            grow_x=grow_x,
-            grow_y=grow_y,
         )
 
         self.color = color
         self.background_color = background_color
         self.progress = progress
```

### Comparing `reflex_ui-0.1.0/reflex/widgets/rectangle.py` & `reflex_ui-0.1.1/reflex/widgets/rectangle.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/row.py` & `reflex_ui-0.1.1/reflex/widgets/row.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,20 +24,18 @@
         margin: Optional[float] = None,
         margin_x: Optional[float] = None,
         margin_y: Optional[float] = None,
         margin_left: Optional[float] = None,
         margin_top: Optional[float] = None,
         margin_right: Optional[float] = None,
         margin_bottom: Optional[float] = None,
-        width: Optional[float] = None,
-        height: Optional[float] = None,
+        width: Union[Literal["natural", "grow"], float] = "natural",
+        height: Union[Literal["natural", "grow"], float] = "natural",
         align_x: Optional[float] = None,
         align_y: Optional[float] = None,
-        grow_x: bool = False,
-        grow_y: bool = False,
     ):
         assert isinstance(children, tuple), children
         for child in children:
             assert isinstance(child, widget_base.Widget), child
 
         super().__init__(
             key=key,
@@ -48,16 +46,14 @@
             margin_top=margin_top,
             margin_right=margin_right,
             margin_bottom=margin_bottom,
             width=width,
             height=height,
             align_x=align_x,
             align_y=align_y,
-            grow_x=grow_x,
-            grow_y=grow_y,
         )
 
         self.children = list(children)
         self.spacing = spacing
 
 
 Row._unique_id = "Row-builtin"
```

### Comparing `reflex_ui-0.1.0/reflex/widgets/switch.py` & `reflex_ui-0.1.1/reflex/widgets/switch.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/text_input.py` & `reflex_ui-0.1.1/reflex/widgets/text_input.py`

 * *Files identical despite different names*

### Comparing `reflex_ui-0.1.0/reflex/widgets/widget_base.py` & `reflex_ui-0.1.1/reflex/widgets/widget_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 import dataclasses
-import weakref
 import inspect
 import json
 import traceback
 import typing
+import weakref
 from abc import ABC, abstractmethod
 from dataclasses import KW_ONLY, dataclass
 from typing import *  # type: ignore
-from typing_extensions import dataclass_transform
 
 import introspection
 from typing_extensions import dataclass_transform
 
 from .. import common, messages, session
 from ..common import Jsonable
 
@@ -246,23 +245,20 @@
     margin_y: Optional[float] = None
 
     margin_left: Optional[float] = None
     margin_top: Optional[float] = None
     margin_right: Optional[float] = None
     margin_bottom: Optional[float] = None
 
-    width: Optional[float] = None
-    height: Optional[float] = None
+    width: Union[Literal["natural", "grow"], float] = "natural"
+    height: Union[Literal["natural", "grow"], float] = "natural"
 
     align_x: Optional[float] = None
     align_y: Optional[float] = None
 
-    grow_x: bool = False
-    grow_y: bool = False
-
     # Weak reference to the widget whose `build` method returned this widget.
     _weak_builder_: Callable[[], Optional[Widget]] = dataclasses.field(
         # Dataclasses seem to unintentionally turn this function into a method.
         # Make sure it works whether or not `self` is passed.
         default=lambda *args: None,
         init=False,
     )
@@ -292,30 +288,34 @@
         # instance doesn't have the attribute, but the class does, and
         # everything is fine, right? Wrong. We create a `StateProperty` for each
         # field, which overrides that default value. We absolutely need every
         # attribute to be an instance attribute, which we can achieve by
         # replacing every default value with a default factory.
         cls_vars = vars(cls)
 
-        for attr_name in cls_vars.get('__annotations__', {}):
+        for attr_name in cls_vars.get("__annotations__", {}):
             try:
                 field_or_default = cls_vars[attr_name]
             except KeyError:
                 continue
 
             if not isinstance(field_or_default, dataclasses.Field):
-                field = dataclasses.field(default_factory=make_default_factory_for_value(field_or_default))
+                field = dataclasses.field(
+                    default_factory=make_default_factory_for_value(field_or_default)
+                )
                 setattr(cls, attr_name, field)
                 continue
 
             # If it doesn't have a default value, we can ignore it
             if field_or_default.default is dataclasses.MISSING:
                 continue
 
-            field_or_default.default_factory = make_default_factory_for_value(field_or_default.default)
+            field_or_default.default_factory = make_default_factory_for_value(
+                field_or_default.default
+            )
             field_or_default.default = dataclasses.MISSING
 
     @staticmethod
     def _determine_explicitly_set_properties(
         original_init,
         self: "Widget",
         *args,
```

### Comparing `reflex_ui-0.1.0/reflex/world_units.py` & `reflex_ui-0.1.1/reflex/world_units.py`

 * *Files identical despite different names*

