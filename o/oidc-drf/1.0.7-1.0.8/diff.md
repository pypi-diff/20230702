# Comparing `tmp/oidc_drf-1.0.7.tar.gz` & `tmp/oidc_drf-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.0.7.tar", last modified: Sat Jul  1 00:49:44 2023, max compression
+gzip compressed data, was "oidc_drf-1.0.8.tar", last modified: Sun Jul  2 09:16:29 2023, max compression
```

## Comparing `oidc_drf-1.0.7.tar` & `oidc_drf-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-01 00:49:44.455019 oidc_drf-1.0.7/
--rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-07-01 00:49:44.454882 oidc_drf-1.0.7/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     3711 2023-07-01 00:46:32.000000 oidc_drf-1.0.7/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-01 00:49:44.453996 oidc_drf-1.0.7/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.0.7/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-06-21 20:00:07.000000 oidc_drf-1.0.7/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    15596 2023-06-30 19:37:05.000000 oidc_drf-1.0.7/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.0.7/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-01 00:49:44.454731 oidc_drf-1.0.7/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.0.7/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      332 2023-06-30 19:04:55.000000 oidc_drf-1.0.7/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.0.7/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.0.7/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     7714 2023-07-01 00:38:14.000000 oidc_drf-1.0.7/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-01 00:49:44.454612 oidc_drf-1.0.7/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-07-01 00:49:44.000000 oidc_drf-1.0.7/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-01 00:49:44.000000 oidc_drf-1.0.7/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-01 00:49:44.000000 oidc_drf-1.0.7/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       27 2023-07-01 00:49:44.000000 oidc_drf-1.0.7/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-01 00:49:44.000000 oidc_drf-1.0.7/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-01 00:49:44.455055 oidc_drf-1.0.7/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1101 2023-06-30 22:32:47.000000 oidc_drf-1.0.7/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:16:29.158974 oidc_drf-1.0.8/
+-rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-07-02 09:16:29.158822 oidc_drf-1.0.8/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4409 2023-07-02 09:16:18.000000 oidc_drf-1.0.8/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:16:29.157603 oidc_drf-1.0.8/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.0.8/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.0.8/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    15614 2023-07-02 09:00:12.000000 oidc_drf-1.0.8/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.0.8/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:16:29.158606 oidc_drf-1.0.8/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.0.8/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.0.8/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.0.8/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.0.8/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7684 2023-07-02 09:12:31.000000 oidc_drf-1.0.8/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:16:29.158312 oidc_drf-1.0.8/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       27 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-02 09:16:29.159015 oidc_drf-1.0.8/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1101 2023-07-02 09:14:21.000000 oidc_drf-1.0.8/setup.py
```

### Comparing `oidc_drf-1.0.7/PKG-INFO` & `oidc_drf-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc_drf
-Version: 1.0.7
+Version: 1.0.8
 Summary: Django DRF OIDC Auth library
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.0.7/oidc_drf/admin.py` & `oidc_drf-1.0.8/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.7/oidc_drf/backends.py` & `oidc_drf-1.0.8/oidc_drf/backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def __init__(self, *args, **kwargs):
         """Initialize settings."""
         self.OIDC_OP_TOKEN_ENDPOINT = import_from_settings("OIDC_OP_TOKEN_ENDPOINT")
         self.OIDC_OP_USER_ENDPOINT = import_from_settings("OIDC_OP_USER_ENDPOINT")
         self.OIDC_OP_JWKS_ENDPOINT = import_from_settings("OIDC_OP_JWKS_ENDPOINT", None)
         self.OIDC_RP_CLIENT_ID = import_from_settings("OIDC_RP_CLIENT_ID")
         self.OIDC_RP_CLIENT_SECRET = import_from_settings("OIDC_RP_CLIENT_SECRET","")
-        self.OIDC_RP_SIGN_ALGO = import_from_settings("OIDC_RP_SIGN_ALGO", "HS256")
+        self.OIDC_RP_SIGN_ALGO = import_from_settings("OIDC_RP_SIGN_ALGO", "RS256")
         self.OIDC_RP_IDP_SIGN_KEY = import_from_settings("OIDC_RP_IDP_SIGN_KEY", None)
 
         if self.OIDC_RP_SIGN_ALGO.startswith("RS") and (
             self.OIDC_RP_IDP_SIGN_KEY is None and self.OIDC_OP_JWKS_ENDPOINT is None
         ):
             msg = "{} alg requires OIDC_RP_IDP_SIGN_KEY or OIDC_OP_JWKS_ENDPOINT to be configured."
             raise ImproperlyConfigured(msg.format(self.OIDC_RP_SIGN_ALGO))
@@ -105,15 +105,15 @@
         access_token = token_info.get("access_token")
         
         
         # Validate the token
         payload = self.verify_token(id_token, nonce=nonce)
                 
         if payload:
-            self.store_tokens(access_token, refresh_token)
+            self.store_tokens(access_token, id_token, refresh_token)
             try:
                 return self.get_or_create_user(access_token, id_token, payload)
             except SuspiciousOperation as exc:
                 LOGGER.warning("failed to get or create user: %s", exc)
                 return None
         return None
         
@@ -402,14 +402,14 @@
             verify=import_from_settings("OIDC_VERIFY_SSL", True),
             timeout=import_from_settings("OIDC_TIMEOUT", None),
             proxies=import_from_settings("OIDC_PROXY", None),
         )
         response.raise_for_status()
         return response.json()
     
-    def store_tokens(self, access_token, refresh_token):
+    def store_tokens(self, access_token, id_token, refresh_token):
         """Store OIDC tokens."""
         session = self.request.session
         session["oidc_access_token"] = access_token
-        # session["oidc_id_token"] = id_token
+        session["oidc_id_token"] = id_token
         session["oidc_refresh_token"] = refresh_token
```

### Comparing `oidc_drf-1.0.7/oidc_drf/drf.py` & `oidc_drf-1.0.8/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.7/oidc_drf/utils.py` & `oidc_drf-1.0.8/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.7/oidc_drf/views.py` & `oidc_drf-1.0.8/oidc_drf/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,25 +79,25 @@
     def login_failure(self):
         return Response("login failure", status=status.HTTP_400_BAD_REQUEST)
 
 
     def login_success(self):        
 
         oidc_access_token = self.request.session["oidc_access_token"]
-        # oidc_id_token = self.request.session["oidc_id_token"]
+        oidc_id_token = self.request.session["oidc_id_token"]
         oidc_refresh_token = self.request.session["oidc_refresh_token"]
         
         data = {
             'access': str(oidc_access_token),
             'refresh': str(oidc_refresh_token),
-            # 'oidc_id_token': str(oidc_id_token),
+            'oidc_id_token': str(oidc_id_token),
         } 
         
         del self.request.session["oidc_access_token"]
-        # del self.request.session["oidc_id_token"]
+        del self.request.session["oidc_id_token"]
         del self.request.session["oidc_refresh_token"]
         self.request.session.save()
 
            
         return JsonResponse(data)
     
 
@@ -119,20 +119,20 @@
             
             if self.user and self.user.is_active:
                 return self.login_success()
         
         return self.login_failure()
 
 class OIDCLogoutView(APIView):
-    permission_classes = [IsAuthenticated]    
-    
-    def get(self, request):     
-        oidc_id_token = request.user.oidcextradata.id_token
+    permission_classes = [AllowAny]    
+
+    def post(self, request):     
+        oidc_id_token = request.data.get('oidc_id_token', '')
         if oidc_id_token:
-            
+
             logout_endpoint = import_from_settings("OIDC_OP_LOGOUT_ENDPOINT", "")
             post_logout_redirect_uri = import_from_settings("OIDC_LOGOUT_REDIRECT_URL", "http://localhost:3000")
             
             headers = {
                 'Content-Type': 'application/x-www-form-urlencoded',
             }
 
@@ -186,21 +186,21 @@
                 error_message = json_data.get('error', 'Request failed with status code: {}'.format(response.status_code))
                 error_data = {
                     'error': error_message
                 }
                 return JsonResponse(error_data, status=response.status_code)
             
             oidc_access_token = json_data.get("access_token")
-            # oidc_id_token = json_data.get("id_token")
+            oidc_id_token = json_data.get("id_token")
             oidc_refresh_token = json_data.get("refresh_token")
             
             data = {
                 'access': str(oidc_access_token),
                 'refresh': str(oidc_refresh_token),
-                # 'oidc_id_token': str(oidc_id_token),
+                'oidc_id_token': str(oidc_id_token),
             }       
     
             return JsonResponse(data)
         except requests.exceptions.RequestException as e:
             # Handle any request exceptions here
             error_message = str(e)
             error_data = {
```

### Comparing `oidc_drf-1.0.7/oidc_drf.egg-info/PKG-INFO` & `oidc_drf-1.0.8/oidc_drf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oidc-drf
-Version: 1.0.7
+Version: 1.0.8
 Summary: Django DRF OIDC Auth library
 Home-page: https://github.com/halmogbl/oidc_drf
 Author: Hamad Almogbl
 Author-email: hamad.almogbl@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `oidc_drf-1.0.7/setup.py` & `oidc_drf-1.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.0.7',
+    version='1.0.8',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
     description='Django DRF OIDC Auth library',
     long_description="Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.",
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
```

