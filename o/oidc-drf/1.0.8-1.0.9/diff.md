# Comparing `tmp/oidc_drf-1.0.8.tar.gz` & `tmp/oidc_drf-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oidc_drf-1.0.8.tar", last modified: Sun Jul  2 09:16:29 2023, max compression
+gzip compressed data, was "oidc_drf-1.0.9.tar", last modified: Sun Jul  2 09:59:12 2023, max compression
```

## Comparing `oidc_drf-1.0.8.tar` & `oidc_drf-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:16:29.158974 oidc_drf-1.0.8/
--rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-07-02 09:16:29.158822 oidc_drf-1.0.8/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)     4409 2023-07-02 09:16:18.000000 oidc_drf-1.0.8/README.md
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:16:29.157603 oidc_drf-1.0.8/oidc_drf/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.0.8/oidc_drf/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.0.8/oidc_drf/admin.py
--rw-r--r--   0 hmogbl     (501) staff       (20)    15614 2023-07-02 09:00:12.000000 oidc_drf-1.0.8/oidc_drf/backends.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.0.8/oidc_drf/drf.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:16:29.158606 oidc_drf-1.0.8/oidc_drf/migrations/
--rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.0.8/oidc_drf/migrations/__init__.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.0.8/oidc_drf/models.py
--rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.0.8/oidc_drf/urls.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.0.8/oidc_drf/utils.py
--rw-r--r--   0 hmogbl     (501) staff       (20)     7684 2023-07-02 09:12:31.000000 oidc_drf-1.0.8/oidc_drf/views.py
-drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:16:29.158312 oidc_drf-1.0.8/oidc_drf.egg-info/
--rw-r--r--   0 hmogbl     (501) staff       (20)      768 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/PKG-INFO
--rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/SOURCES.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/dependency_links.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       27 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/requires.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-02 09:16:29.000000 oidc_drf-1.0.8/oidc_drf.egg-info/top_level.txt
--rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-02 09:16:29.159015 oidc_drf-1.0.8/setup.cfg
--rw-r--r--   0 hmogbl     (501) staff       (20)     1101 2023-07-02 09:14:21.000000 oidc_drf-1.0.8/setup.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:59:12.258880 oidc_drf-1.0.9/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5212 2023-07-02 09:59:12.258745 oidc_drf-1.0.9/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4473 2023-07-02 09:48:52.000000 oidc_drf-1.0.9/README.md
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:59:12.257455 oidc_drf-1.0.9/oidc_drf/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:35:48.000000 oidc_drf-1.0.9/oidc_drf/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      578 2023-07-02 09:08:57.000000 oidc_drf-1.0.9/oidc_drf/admin.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)    15520 2023-07-02 09:46:48.000000 oidc_drf-1.0.9/oidc_drf/backends.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     4583 2023-07-01 00:48:09.000000 oidc_drf-1.0.9/oidc_drf/drf.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:59:12.258588 oidc_drf-1.0.9/oidc_drf/migrations/
+-rw-r--r--   0 hmogbl     (501) staff       (20)        0 2023-06-21 18:47:16.000000 oidc_drf-1.0.9/oidc_drf/migrations/__init__.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      278 2023-07-02 09:08:51.000000 oidc_drf-1.0.9/oidc_drf/models.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)      507 2023-06-22 18:20:04.000000 oidc_drf-1.0.9/oidc_drf/urls.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     2081 2023-06-21 07:35:29.000000 oidc_drf-1.0.9/oidc_drf/utils.py
+-rw-r--r--   0 hmogbl     (501) staff       (20)     7684 2023-07-02 09:12:31.000000 oidc_drf-1.0.9/oidc_drf/views.py
+drwxr-xr-x   0 hmogbl     (501) staff       (20)        0 2023-07-02 09:59:12.258407 oidc_drf-1.0.9/oidc_drf.egg-info/
+-rw-r--r--   0 hmogbl     (501) staff       (20)     5212 2023-07-02 09:59:12.000000 oidc_drf-1.0.9/oidc_drf.egg-info/PKG-INFO
+-rw-r--r--   0 hmogbl     (501) staff       (20)      357 2023-07-02 09:59:12.000000 oidc_drf-1.0.9/oidc_drf.egg-info/SOURCES.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        1 2023-07-02 09:59:12.000000 oidc_drf-1.0.9/oidc_drf.egg-info/dependency_links.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       61 2023-07-02 09:59:12.000000 oidc_drf-1.0.9/oidc_drf.egg-info/requires.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)        9 2023-07-02 09:59:12.000000 oidc_drf-1.0.9/oidc_drf.egg-info/top_level.txt
+-rw-r--r--   0 hmogbl     (501) staff       (20)       38 2023-07-02 09:59:12.258917 oidc_drf-1.0.9/setup.cfg
+-rw-r--r--   0 hmogbl     (501) staff       (20)     1118 2023-07-02 09:58:43.000000 oidc_drf-1.0.9/setup.py
```

### Comparing `oidc_drf-1.0.8/README.md` & `oidc_drf-1.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,41 +27,14 @@
 OIDC_OP_TOKEN_ENDPOINT = ''# required
 OIDC_OP_USER_ENDPOINT = '' # required
 OIDC_OP_LOGOUT_ENDPOINT ='' # required
 
 OIDC_AUTHENTICATION_SSO_CALLBACK_URL = '' # required - identity provider will redirect you to this url after login
 OIDC_LOGOUT_REDIRECT_URL = '' # required - identity provider will redirect you to this url after logout
 
-
-# optional configrations
-OIDC_USE_NONCE = True # defalut true
-OIDC_USE_PKCE = True # defalut true
-
-OIDC_RP_SIGN_ALGO = 'RS256' # defalut RS256
-OIDC_RP_SCOPES = 'openid email' # defalut openid email
-OIDC_RP_IDP_SIGN_KEY = None # defalut None
-OIDC_VERIFY_SSL = True # defalut True
-OIDC_TIMEOUT = None # defalut None
-OIDC_PROXY = None # defalut None
-OIDC_USERNAME_CLAIM = 'preferred_username' # defalut 'preferred_username'
-OIDC_USERNAME_ALGO = None # defalut None
-OIDC_USE_ENCODED_USERNAME = None # defalut None
-OIDC_CREATE_USER = True # defalut True
-OIDC_VERIFY_KID = True # defalut True
-OIDC_ALLOW_UNSECURED_JWT = False # defalut False
-OIDC_TOKEN_USE_BASIC_AUTH = False # defalut False
-
-# you can map the info comming back from IDP to user model
-# defalut is {}
-OIDC_FIELD_MAPPING = {
-    'field_in_my_user_model': 'field_in_in_oidc',
-    'first_name': 'given_name',
-    'last_name': 'family_name',
-}
-
 # Django Rest Framework settings
 REST_FRAMEWORK = {
     'DEFAULT_AUTHENTICATION_CLASSES': [
         'oidc_drf.drf.OIDCAuthentication',  # This is important to be the first one 
     ],
 }
 
@@ -97,21 +70,48 @@
 
 ```
 
 That's it, we're done!
 
 
 
+# EXTRA SETTINGS
+those settings are optional and populated with default values.
 
+```python
 
+OIDC_USE_NONCE = True # defalut true
+OIDC_USE_PKCE = True # defalut true
 
+OIDC_USERNAME_CLAIM = 'preferred_username' # defalut 'preferred_username'
+OIDC_RP_SIGN_ALGO = 'RS256' # defalut RS256
+OIDC_RP_SCOPES = 'openid email' # defalut openid email
+OIDC_RP_IDP_SIGN_KEY = None # defalut None
+OIDC_VERIFY_SSL = True # defalut True
+OIDC_TIMEOUT = None # defalut None
+OIDC_PROXY = None # defalut None
+OIDC_USERNAME_ALGO = None # defalut None
+OIDC_USE_ENCODED_USERNAME = None # defalut None
+OIDC_CREATE_USER = True # defalut True
+OIDC_VERIFY_KID = True # defalut True
+OIDC_ALLOW_UNSECURED_JWT = False # defalut False
+OIDC_TOKEN_USE_BASIC_AUTH = False # defalut False
+
+# you can map the info comming back from IDP to user model
+# defalut is {}
+OIDC_FIELD_MAPPING = {
+    'field_in_my_user_model': 'field_in_in_oidc',
+    'first_name': 'given_name',
+    'last_name': 'family_name',
+}
 
-# REST API
+```
 
-The REST API to the example app is described below.
+# REST APIs
+The REST API to the OIDC DRF is described below.
 
 ## AUTH ENDPOINT
 
 ### Request
 
 `GET /oidc/auth/`
```

### Comparing `oidc_drf-1.0.8/oidc_drf/admin.py` & `oidc_drf-1.0.9/oidc_drf/admin.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.8/oidc_drf/backends.py` & `oidc_drf-1.0.9/oidc_drf/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,27 +222,26 @@
         user_json = {**user_info_json, **decoded_access_token, **decoded_id_token}
         
         # Remove excluded fields from decoded id_token
         user_json = {key: value for key, value in user_json.items() if key not in excluded_fields}
         
         return user_json
     
-    def save_user_data(self,user, user_json,id_token):
+    def save_user_data(self,user, user_json):
         # Serialize the remaining user_json
         user_data = json.dumps(user_json)
 
         # Check if the user's OIDCExtraData already exists
         try:
             oidc_extra_data = user.oidcextradata
-            oidc_extra_data.id_token = id_token
             oidc_extra_data.data = user_data
             oidc_extra_data.save()
         except OIDCExtraData.DoesNotExist:
             # Create a new OIDCExtraData object for the user
-            oidc_extra_data = OIDCExtraData.objects.create(user=user, data=user_data, id_token=id_token)
+            oidc_extra_data = OIDCExtraData.objects.create(user=user, data=user_data)
 
 
     
     def get_or_create_user(self, access_token, id_token, payload):
         """Returns a User instance if 1 user is found. Creates a user if not found
         and configured to do so. Returns nothing if multiple users are matched."""
 
@@ -255,27 +254,27 @@
         users = self.filter_users_by_claims(user_info)
 
         if len(users) == 1:
             user = self.update_user(users[0], user_info)
             
             if user_info and access_token and id_token:
                 user_json = self.create_user_json(user_info, access_token, id_token)
-                self.save_user_data(user, user_json,id_token)
+                self.save_user_data(user, user_json)
             return user
 
         elif len(users) > 1:
             # In the rare case that two user accounts have the same email address,
             # bail. Randomly selecting one seems really wrong.
             msg = "Multiple users returned"
             raise SuspiciousOperation(msg)
         elif import_from_settings("OIDC_CREATE_USER", True):
             user = self.create_user(user_info)
             if user_info and access_token and id_token:
                 user_json = self.create_user_json(user_info, access_token, id_token)
-                self.save_user_data(user, user_json,id_token)
+                self.save_user_data(user, user_json)
 
 
             return user
         else:
             LOGGER.debug(
                 "Login failed: No user with %s found, and " "OIDC_CREATE_USER is False",
                 self.describe_user_by_claims(user_info),
```

### Comparing `oidc_drf-1.0.8/oidc_drf/drf.py` & `oidc_drf-1.0.9/oidc_drf/drf.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.8/oidc_drf/utils.py` & `oidc_drf-1.0.9/oidc_drf/utils.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.8/oidc_drf/views.py` & `oidc_drf-1.0.9/oidc_drf/views.py`

 * *Files identical despite different names*

### Comparing `oidc_drf-1.0.8/setup.py` & `oidc_drf-1.0.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='oidc_drf',
-    version='1.0.8',
+    version='1.0.9',
     author='Hamad Almogbl',
     author_email='hamad.almogbl@gmail.com',
-    description='Django DRF OIDC Auth library',
-    long_description="Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.",
+    description='Django DRF OIDC Auth library: Securely authenticate users using OIDC in Django DRF. Supports Code Flow and Code Flow With PKCE. Easy integration with React Js or any front-end framework.',
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/halmogbl/oidc_drf',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     install_requires=[
-        'Django',
+        "Django >= 3.2",
+        "josepy",
+        "requests",
+        "cryptography",
         'djangorestframework',
-        # Add other dependencies here
     ],
 )
```

