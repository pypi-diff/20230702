# Comparing `tmp/VeloWeb-1.0.1.tar.gz` & `tmp/VeloWeb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VeloWeb-1.0.1.tar", last modified: Sun Jul  2 13:35:57 2023, max compression
+gzip compressed data, was "VeloWeb-1.0.2.tar", last modified: Sun Jul  2 14:30:48 2023, max compression
```

## Comparing `VeloWeb-1.0.1.tar` & `VeloWeb-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 13:35:57.000382 VeloWeb-1.0.1/
--rw-rw-rw-   0        0        0      910 2023-07-02 13:35:57.000382 VeloWeb-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-02 13:35:56.968374 VeloWeb-1.0.1/VeloWeb.egg-info/
--rw-rw-rw-   0        0        0      910 2023-07-02 13:35:56.000000 VeloWeb-1.0.1/VeloWeb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-07-02 13:35:56.000000 VeloWeb-1.0.1/VeloWeb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 13:35:56.000000 VeloWeb-1.0.1/VeloWeb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-07-02 13:35:56.000000 VeloWeb-1.0.1/VeloWeb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-07-02 13:35:56.000000 VeloWeb-1.0.1/VeloWeb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-02 13:35:56.000000 VeloWeb-1.0.1/VeloWeb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 13:35:57.000382 VeloWeb-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-07-02 13:35:29.000000 VeloWeb-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 13:35:56.992378 VeloWeb-1.0.1/veloweb/
--rw-rw-rw-   0        0        0     3900 2023-07-02 13:06:35.000000 VeloWeb-1.0.1/veloweb/VeloHasher.py
--rw-rw-rw-   0        0        0     6403 2023-07-02 13:16:09.000000 VeloWeb-1.0.1/veloweb/VeloJWT.py
--rw-rw-rw-   0        0        0     2847 2023-07-01 16:49:03.000000 VeloWeb-1.0.1/veloweb/VeloMailer.py
--rw-rw-rw-   0        0        0     2594 2023-07-01 16:49:12.000000 VeloWeb-1.0.1/veloweb/VeloWTF.py
--rw-rw-rw-   0        0        0       27 2023-07-01 20:25:18.000000 VeloWeb-1.0.1/veloweb/__init__.py
--rw-rw-rw-   0        0        0      221 2023-07-02 12:55:02.000000 VeloWeb-1.0.1/veloweb/test.py
--rw-rw-rw-   0        0        0    11405 2023-07-02 12:34:50.000000 VeloWeb-1.0.1/veloweb/veloweb.py
+drwxrwxrwx   0        0        0        0 2023-07-02 14:30:48.602010 VeloWeb-1.0.2/
+-rw-rw-rw-   0        0        0      910 2023-07-02 14:30:48.600009 VeloWeb-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-02 14:30:48.554007 VeloWeb-1.0.2/VeloWeb.egg-info/
+-rw-rw-rw-   0        0        0      910 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-02 14:30:48.000000 VeloWeb-1.0.2/VeloWeb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 14:30:48.603010 VeloWeb-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2023-07-02 14:30:12.000000 VeloWeb-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 14:30:48.596008 VeloWeb-1.0.2/veloweb/
+-rw-rw-rw-   0        0        0     3900 2023-07-02 13:06:35.000000 VeloWeb-1.0.2/veloweb/VeloHasher.py
+-rw-rw-rw-   0        0        0     6403 2023-07-02 13:16:09.000000 VeloWeb-1.0.2/veloweb/VeloJWT.py
+-rw-rw-rw-   0        0        0     2847 2023-07-01 16:49:03.000000 VeloWeb-1.0.2/veloweb/VeloMailer.py
+-rw-rw-rw-   0        0        0     2594 2023-07-01 16:49:12.000000 VeloWeb-1.0.2/veloweb/VeloWTF.py
+-rw-rw-rw-   0        0        0       27 2023-07-01 20:25:18.000000 VeloWeb-1.0.2/veloweb/__init__.py
+-rw-rw-rw-   0        0        0      221 2023-07-02 12:55:02.000000 VeloWeb-1.0.2/veloweb/test.py
+-rw-rw-rw-   0        0        0    12889 2023-07-02 14:29:43.000000 VeloWeb-1.0.2/veloweb/veloweb.py
```

### Comparing `VeloWeb-1.0.1/PKG-INFO` & `VeloWeb-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeloWeb
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/veloweb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VeloWeb-1.0.1/VeloWeb.egg-info/PKG-INFO` & `VeloWeb-1.0.2/VeloWeb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeloWeb
-Version: 1.0.1
+Version: 1.0.2
 Summary: A lightweight and function rich web framework for python
 Home-page: https://github.com/E491K8/veloweb
 Author: Pawan kumar
 Author-email: control@vvfin.in
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VeloWeb-1.0.1/setup.py` & `VeloWeb-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="VeloWeb",
-    version="1.0.1",
+    version="1.0.2",
     author="Pawan kumar",
     author_email="control@vvfin.in",
     include_package_data=True,
     description="A lightweight and function rich web framework for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/E491K8/veloweb",
```

### Comparing `VeloWeb-1.0.1/veloweb/VeloHasher.py` & `VeloWeb-1.0.2/veloweb/VeloHasher.py`

 * *Files identical despite different names*

### Comparing `VeloWeb-1.0.1/veloweb/VeloJWT.py` & `VeloWeb-1.0.2/veloweb/VeloJWT.py`

 * *Files identical despite different names*

### Comparing `VeloWeb-1.0.1/veloweb/VeloMailer.py` & `VeloWeb-1.0.2/veloweb/VeloMailer.py`

 * *Files identical despite different names*

### Comparing `VeloWeb-1.0.1/veloweb/VeloWTF.py` & `VeloWeb-1.0.2/veloweb/VeloWTF.py`

 * *Files identical despite different names*

### Comparing `VeloWeb-1.0.1/veloweb/veloweb.py` & `VeloWeb-1.0.2/veloweb/veloweb.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,20 +25,23 @@
         except ModuleNotFoundError:
             # If settings.py is not available, use default values
             self.config['HOST'] = '127.0.0.1'
             self.config['PORT'] = 8000
             self.config['DEBUG'] = True
             self.config['TEMPLATE_FOLDER'] = 'templates'
             self.config['STATIC_FOLDER'] = 'public'
+            self.config['ERROR_FOLDER'] = 'errors'  # Added error folder configuration
         else:
             self.config['HOST'] = getattr(settings, 'HOST', '127.0.0.1')
             self.config['PORT'] = getattr(settings, 'PORT', 8000)
             self.config['DEBUG'] = getattr(settings, 'DEBUG', True)
             self.config['TEMPLATE_FOLDER'] = getattr(settings, 'TEMPLATE_FOLDER', 'templates')
             self.config['STATIC_FOLDER'] = getattr(settings, 'STATIC_FOLDER', 'public')
+            self.config['ERROR_FOLDER'] = getattr(settings, 'ERROR_FOLDER', 'errors')  # Added error folder configuration
+
         self.jinja_env = Environment(loader=FileSystemLoader(self.config['TEMPLATE_FOLDER']))
 
     def add_route(self, path, methods, func):
         options = {"methods": methods}
         rule = Rule(path, endpoint=func, **options)
         self.url_map.add(rule)
         self.routes[func] = path
@@ -67,32 +70,62 @@
         self.session['flashes'].append({'message': message, 'category': category})
 
     def get_flashes(self):
         return self.session.pop('flashes', [])
 
     def handle_not_found(self):
         response = Response('Not Found', status=404)
-        return self.render_template('404.html', response=response)
+        error_file = os.path.join(self.config['ERROR_FOLDER'], '404.html')
+        if os.path.exists(error_file):
+            with open(error_file, 'r') as f:
+                file_content = f.read()
+            response.set_data(file_content)
+        response.headers['Content-Type'] = 'text/html'
+        return response
 
     def handle_method_not_allowed(self, allowed_methods):
         response = Response('Method Not Allowed', status=405)
+        error_file = os.path.join(self.config['ERROR_FOLDER'], '405.html')
+        if os.path.exists(error_file):
+            with open(error_file, 'r') as f:
+                file_content = f.read()
+            response.set_data(file_content)
         response.headers['Allow'] = ', '.join(allowed_methods)
-        return self.render_template('405.html', response=response)
+        response.headers['Content-Type'] = 'text/html'
+        return response
 
     def handle_bad_request(self):
-        response = self.make_response('Bad Request', status=400)
-        return self.render_template('400.html', response=response)
-    
+        response = Response('Bad Request', status=400)
+        error_file = os.path.join(self.config['ERROR_FOLDER'], '400.html')
+        if os.path.exists(error_file):
+            with open(error_file, 'r') as f:
+                file_content = f.read()
+            response.set_data(file_content)
+        response.headers['Content-Type'] = 'text/html'
+        return response
+
     def handle_unauthorized(self):
-        response = self.make_response('Unauthorized', status=401)
-        return self.render_template('401.html', response=response)
+        response = Response('Unauthorized', status=401)
+        error_file = os.path.join(self.config['ERROR_FOLDER'], '401.html')
+        if os.path.exists(error_file):
+            with open(error_file, 'r') as f:
+                file_content = f.read()
+            response.set_data(file_content)
+        response.headers['Content-Type'] = 'text/html'
+        return response
 
     def handle_forbidden(self):
-        response = self.make_response('Forbidden', status=403)
-        return self.render_template('403.html', response=response)
+        response = Response('Forbidden', status=403)
+        error_file = os.path.join(self.config['ERROR_FOLDER'], '403.html')
+        if os.path.exists(error_file):
+            with open(error_file, 'r') as f:
+                file_content = f.read()
+            response.set_data(file_content)
+        response.headers['Content-Type'] = 'text/html'
+        return response
 
     def make_response_from_template(self, template_name, context=None, status=None, headers=None):
         template = self.jinja_env.get_template(template_name)
         response_body = template.render(context or {})
         return self.make_response(response_body, status=status, headers=headers)
 
     def render_template_string(self, template_string, context=None):
```

