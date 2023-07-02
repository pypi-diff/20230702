# Comparing `tmp/flask-marshmallow-openapi-0.4.0.tar.gz` & `tmp/flask-marshmallow-openapi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.4.0.tar", last modified: Sat Jul  1 08:20:12 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.4.1.tar", last modified: Sun Jul  2 16:56:55 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.4.0.tar` & `flask-marshmallow-openapi-0.4.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:20:12.412895 flask-marshmallow-openapi-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-01 08:20:12.412895 flask-marshmallow-openapi-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 08:20:12.412895 flask-marshmallow-openapi-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:20:12.396895 flask-marshmallow-openapi-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:20:12.404895 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:20:12.404895 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/decorate_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/decorate_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/decorate_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/decorate_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/flask_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/schemas_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:20:12.404895 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/redoc_favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:20:12.408895 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 runner    (1001) docker     (123)  1045708 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   368781 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 runner    (1001) docker     (123)  1045498 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   322863 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)   145206 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)   256702 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:20:12.412895 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-01 08:19:58.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:20:12.404895 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-01 08:20:12.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-01 08:20:12.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:20:12.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:20:12.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-01 08:20:12.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-01 08:20:12.000000 flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.838029 flask-marshmallow-openapi-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.842029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.842029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/flask_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11436 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/schemas_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.842029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/redoc_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045708 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   368781 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045498 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   322863 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)   145206 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   256702 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.850029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-02 16:56:44.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:56:55.842029 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 16:56:55.000000 flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.4.0/.gitignore` & `flask-marshmallow-openapi-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/LICENSE` & `flask-marshmallow-openapi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/MANIFEST.in` & `flask-marshmallow-openapi-0.4.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/PKG-INFO` & `flask-marshmallow-openapi-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.4.0/README.md` & `flask-marshmallow-openapi-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/pyproject.toml` & `flask-marshmallow-openapi-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.4.0"
+version = "0.4.1"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
@@ -25,15 +25,15 @@
     "apispec[yaml,marshmallow]",
     "flask >= 2.3.0",
     "inflection",
     "marshmallow >= 3.18.0",
     "pyyaml",
     "requests",
     "wrapt",
-    "openapi-pydantic-models >= 1.0.0",
+    "openapi-pydantic-models >= 1.0.1",
 ]
 
 
 [project.urls]
 Source = "https://github.com/tadams42/flask-marshmallow-openapi"
```

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/decorate_delete.py` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_delete.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/decorate_get.py` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_get.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/decorate_patch.py` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_patch.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/decorate_post.py` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/decorate_post.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/decorators/helpers.py` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/decorators/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/flask_paths.py` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/flask_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             if not operation.operationId:
                 operation.operationId = f"{method}_{rule.endpoint}"
 
             docstring_data = self._docstring_data(view, method)
             if docstring_data:
                 operation_data = operation.model_dump()
                 operation_data.update(docstring_data)
-                operation = OperationObject.parse_obj(operation_data)
+                operation = OperationObject.model_validate(operation_data)
 
             self._register_operation_id(operation)
 
             if method.lower() == "delete":
                 setattr(retv, "delete_", operation)
             else:
                 setattr(retv, method.lower(), operation)
```

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/middleware.py` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/middleware.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/schemas_registry.py` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/schemas_registry.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/redoc_favicon.png` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/redoc_favicon.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.4.0
+Version: 0.4.1
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.4.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.4.1/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

