# Comparing `tmp/falcon-api-browse-0.1.0.tar.gz` & `tmp/falcon_api_browse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon-api-browse-0.1.0.tar", max compression
+gzip compressed data, was "falcon_api_browse-0.1.1.tar", max compression
```

## Comparing `falcon-api-browse-0.1.0.tar` & `falcon_api_browse-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2022-03-13 23:10:12.170649 falcon-api-browse-0.1.0/LICENSE
--rw-r--r--   0        0        0      110 2022-03-13 23:52:14.768318 falcon-api-browse-0.1.0/falcon_api_browse/__init__.py
--rw-r--r--   0        0        0      821 2022-03-13 23:58:25.514996 falcon-api-browse-0.1.0/falcon_api_browse/middleware.py
--rw-r--r--   0        0        0      924 2022-03-13 23:36:39.983068 falcon-api-browse-0.1.0/falcon_api_browse/templates/base.html
--rw-r--r--   0        0        0     1648 2022-03-13 23:52:07.926280 falcon-api-browse-0.1.0/falcon_api_browse/views.py
--rw-r--r--   0        0        0      421 2022-03-13 23:52:51.695788 falcon-api-browse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      712 2022-03-14 03:35:00.147414 falcon-api-browse-0.1.0/setup.py
--rw-r--r--   0        0        0      611 2022-03-14 03:35:00.147556 falcon-api-browse-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-02 04:58:21.849240 falcon_api_browse-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1209 2023-07-02 04:58:21.849240 falcon_api_browse-0.1.1/README.rst
+-rw-r--r--   0        0        0      110 2023-07-02 04:58:21.849240 falcon_api_browse-0.1.1/falcon_api_browse/__init__.py
+-rw-r--r--   0        0        0     1247 2023-07-02 04:58:21.849240 falcon_api_browse-0.1.1/falcon_api_browse/middleware.py
+-rw-r--r--   0        0        0      933 2023-07-02 04:58:21.849240 falcon_api_browse-0.1.1/falcon_api_browse/templates/base.html
+-rw-r--r--   0        0        0     1648 2023-07-02 04:58:21.849240 falcon_api_browse-0.1.1/falcon_api_browse/views.py
+-rw-r--r--   0        0        0      614 2023-07-02 04:58:21.853240 falcon_api_browse-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 falcon_api_browse-0.1.1/PKG-INFO
```

### Comparing `falcon-api-browse-0.1.0/LICENSE` & `falcon_api_browse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon-api-browse-0.1.0/falcon_api_browse/middleware.py` & `falcon_api_browse-0.1.1/falcon_api_browse/middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,7 +16,16 @@
         :type response: :class:`falcon.Response`
         :type resource: Falcon resource object.
         :type params: Response parameters.
         """
         accept_html = "text/html" in request.accept.split(",")
         if accept_html:
             html_response(request, response, resource, params)
+
+    async def process_response_async(self, request, response, resource, params):
+        """Similar to :py:method:`process_response` but for ASGI.
+
+        Since there isn't any expensive I/O in process_response, use the same
+        method for ASGI too. The only I/O happening is reading the template
+        from Disk to render the HTML.
+        """
+        return self.process_request(request, response, resource, params)
```

### Comparing `falcon-api-browse-0.1.0/falcon_api_browse/templates/base.html` & `falcon_api_browse-0.1.1/falcon_api_browse/templates/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -28,10 +28,10 @@
 {% if resource.on_delete %}
     <pre>DELETE: {{ resource.on_delete.__doc__ }}</pre>
 {% endif %}
 
     <h2>Response</h2>
     <pre>Status: {{ response.status }}</pre>
     <pre>Body:</pre>
-    <pre>{{ response.text|ppjson }}</pre>
+    <pre>{{ response.render_body()|ppjson }}</pre>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -15,8 +15,8 @@
 PATCH: {{ resource.on_patch.__doc__ }}
 {% endif %} {% if resource.on_delete %}
 DELETE: {{ resource.on_delete.__doc__ }}
 {% endif %}
 ***** Response *****
 Status: {{ response.status }}
 Body:
-{{ response.text|ppjson }}
+{{ response.render_body()|ppjson }}
```

### Comparing `falcon-api-browse-0.1.0/falcon_api_browse/views.py` & `falcon_api_browse-0.1.1/falcon_api_browse/views.py`

 * *Files identical despite different names*

