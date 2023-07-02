# Comparing `tmp/django-python3-ldap-0.9.8.tar.gz` & `tmp/django-python3-ldap-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-python3-ldap-0.9.8.tar", last modified: Thu Dec 10 14:07:59 2015, max compression
+gzip compressed data, was "dist/django-python3-ldap-0.9.9.tar", last modified: Thu Feb 18 09:30:35 2016, max compression
```

## Comparing `django-python3-ldap-0.9.8.tar` & `django-python3-ldap-0.9.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/django_python3_ldap/
--rw-r--r--   0 dave       (501) staff       (20)       88 2015-12-10 14:07:29.000000 django-python3-ldap-0.9.8/django_python3_ldap/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)      496 2015-01-14 18:19:25.000000 django-python3-ldap-0.9.8/django_python3_ldap/auth.py
--rw-r--r--   0 dave       (501) staff       (20)     2895 2015-11-09 09:39:03.000000 django-python3-ldap-0.9.8/django_python3_ldap/conf.py
--rw-r--r--   0 dave       (501) staff       (20)     4680 2015-12-10 13:56:48.000000 django-python3-ldap-0.9.8/django_python3_ldap/ldap.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/django_python3_ldap/management/
--rw-r--r--   0 dave       (501) staff       (20)        0 2015-01-14 18:19:25.000000 django-python3-ldap-0.9.8/django_python3_ldap/management/__init__.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/django_python3_ldap/management/commands/
--rw-r--r--   0 dave       (501) staff       (20)        0 2015-01-14 18:19:25.000000 django-python3-ldap-0.9.8/django_python3_ldap/management/commands/__init__.py
--rw-rw-r--   0 dave       (501) staff       (20)     1025 2015-01-15 18:16:05.000000 django-python3-ldap-0.9.8/django_python3_ldap/management/commands/ldap_promote.py
--rw-r--r--   0 dave       (501) staff       (20)      772 2015-11-09 09:39:03.000000 django-python3-ldap-0.9.8/django_python3_ldap/management/commands/ldap_sync_users.py
--rw-r--r--   0 dave       (501) staff       (20)     7152 2015-11-09 09:39:03.000000 django-python3-ldap-0.9.8/django_python3_ldap/tests.py
--rw-r--r--   0 dave       (501) staff       (20)     3220 2015-11-25 10:33:14.000000 django-python3-ldap-0.9.8/django_python3_ldap/utils.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/django_python3_ldap.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)        1 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/django_python3_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)      788 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/django_python3_ldap.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)       37 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/django_python3_ldap.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)      637 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/django_python3_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)       20 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/django_python3_ldap.egg-info/top_level.txt
--rw-rw-r--   0 dave       (501) staff       (20)     1524 2015-01-14 18:00:09.000000 django-python3-ldap-0.9.8/LICENSE
--rw-rw-r--   0 dave       (501) staff       (20)       35 2015-01-14 17:59:51.000000 django-python3-ldap-0.9.8/MANIFEST.in
--rw-r--r--   0 dave       (501) staff       (20)      788 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)     6164 2015-11-09 09:39:03.000000 django-python3-ldap-0.9.8/README.rst
--rw-r--r--   0 dave       (501) staff       (20)       59 2015-12-10 14:07:59.000000 django-python3-ldap-0.9.8/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1078 2015-11-25 10:33:14.000000 django-python3-ldap-0.9.8/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-02-18 09:30:35.000000 django-python3-ldap-0.9.9/
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-02-18 09:30:35.000000 django-python3-ldap-0.9.9/django_python3_ldap/
+-rw-r--r--   0 dave       (501) staff       (20)       88 2016-02-18 09:29:40.000000 django-python3-ldap-0.9.9/django_python3_ldap/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)      496 2015-01-14 18:19:25.000000 django-python3-ldap-0.9.9/django_python3_ldap/auth.py
+-rw-r--r--   0 dave       (501) staff       (20)     2895 2015-11-09 09:39:03.000000 django-python3-ldap-0.9.9/django_python3_ldap/conf.py
+-rw-r--r--   0 dave       (501) staff       (20)     4786 2016-02-12 09:37:09.000000 django-python3-ldap-0.9.9/django_python3_ldap/ldap.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-02-18 09:30:35.000000 django-python3-ldap-0.9.9/django_python3_ldap/management/
+-rw-r--r--   0 dave       (501) staff       (20)        0 2015-01-14 18:19:25.000000 django-python3-ldap-0.9.9/django_python3_ldap/management/__init__.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-02-18 09:30:35.000000 django-python3-ldap-0.9.9/django_python3_ldap/management/commands/
+-rw-r--r--   0 dave       (501) staff       (20)        0 2015-01-14 18:19:25.000000 django-python3-ldap-0.9.9/django_python3_ldap/management/commands/__init__.py
+-rw-rw-r--   0 dave       (501) staff       (20)     1025 2015-01-15 18:16:05.000000 django-python3-ldap-0.9.9/django_python3_ldap/management/commands/ldap_promote.py
+-rw-r--r--   0 dave       (501) staff       (20)      772 2015-11-09 09:39:03.000000 django-python3-ldap-0.9.9/django_python3_ldap/management/commands/ldap_sync_users.py
+-rw-r--r--   0 dave       (501) staff       (20)     7152 2015-11-09 09:39:03.000000 django-python3-ldap-0.9.9/django_python3_ldap/tests.py
+-rw-r--r--   0 dave       (501) staff       (20)     3220 2015-11-25 10:33:14.000000 django-python3-ldap-0.9.9/django_python3_ldap/utils.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2016-02-18 09:30:35.000000 django-python3-ldap-0.9.9/django_python3_ldap.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)        1 2016-02-18 09:30:34.000000 django-python3-ldap-0.9.9/django_python3_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)      788 2016-02-18 09:30:34.000000 django-python3-ldap-0.9.9/django_python3_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)       37 2016-02-18 09:30:34.000000 django-python3-ldap-0.9.9/django_python3_ldap.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)      637 2016-02-18 09:30:35.000000 django-python3-ldap-0.9.9/django_python3_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)       20 2016-02-18 09:30:34.000000 django-python3-ldap-0.9.9/django_python3_ldap.egg-info/top_level.txt
+-rw-rw-r--   0 dave       (501) staff       (20)     1524 2015-01-14 18:00:09.000000 django-python3-ldap-0.9.9/LICENSE
+-rw-rw-r--   0 dave       (501) staff       (20)       35 2015-01-14 17:59:51.000000 django-python3-ldap-0.9.9/MANIFEST.in
+-rw-r--r--   0 dave       (501) staff       (20)      788 2016-02-18 09:30:35.000000 django-python3-ldap-0.9.9/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)     6164 2015-11-09 09:39:03.000000 django-python3-ldap-0.9.9/README.rst
+-rw-r--r--   0 dave       (501) staff       (20)       59 2016-02-18 09:30:35.000000 django-python3-ldap-0.9.9/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1078 2015-11-25 10:33:14.000000 django-python3-ldap-0.9.9/setup.py
```

### Comparing `django-python3-ldap-0.9.8/django_python3_ldap/conf.py` & `django-python3-ldap-0.9.9/django_python3_ldap/conf.py`

 * *Files identical despite different names*

### Comparing `django-python3-ldap-0.9.8/django_python3_ldap/ldap.py` & `django-python3-ldap-0.9.9/django_python3_ldap/ldap.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,20 @@
     """
     Creates and returns a connection to the LDAP server.
 
     The user identifier, if given, should be keyword arguments matching the fields
     in settings.LDAP_AUTH_USER_LOOKUP_FIELDS, plus a `password` argument.
     """
     # Format the DN for the username.
+    kwargs = {
+        key: value
+        for key, value
+        in kwargs.items()
+        if value
+    }
     username = None
     password = None
     if kwargs:
         password = kwargs.pop("password")
         username = import_func(settings.LDAP_AUTH_FORMAT_USERNAME)(kwargs)
     # Make the connection.
     if username or password:
```

### Comparing `django-python3-ldap-0.9.8/django_python3_ldap/management/commands/ldap_promote.py` & `django-python3-ldap-0.9.9/django_python3_ldap/management/commands/ldap_promote.py`

 * *Files identical despite different names*

### Comparing `django-python3-ldap-0.9.8/django_python3_ldap/management/commands/ldap_sync_users.py` & `django-python3-ldap-0.9.9/django_python3_ldap/management/commands/ldap_sync_users.py`

 * *Files identical despite different names*

### Comparing `django-python3-ldap-0.9.8/django_python3_ldap/tests.py` & `django-python3-ldap-0.9.9/django_python3_ldap/tests.py`

 * *Files identical despite different names*

### Comparing `django-python3-ldap-0.9.8/django_python3_ldap/utils.py` & `django-python3-ldap-0.9.9/django_python3_ldap/utils.py`

 * *Files identical despite different names*

### Comparing `django-python3-ldap-0.9.8/django_python3_ldap.egg-info/PKG-INFO` & `django-python3-ldap-0.9.9/django_python3_ldap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-python3-ldap
-Version: 0.9.8
+Version: 0.9.9
 Summary: Django LDAP user authentication backend for Python 3.
 Home-page: https://github.com/etianen/django-python3-ldap
 Author: Dave Hall
 Author-email: dave@etianen.com
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-python3-ldap-0.9.8/django_python3_ldap.egg-info/SOURCES.txt` & `django-python3-ldap-0.9.9/django_python3_ldap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-python3-ldap-0.9.8/LICENSE` & `django-python3-ldap-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-python3-ldap-0.9.8/PKG-INFO` & `django-python3-ldap-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-python3-ldap
-Version: 0.9.8
+Version: 0.9.9
 Summary: Django LDAP user authentication backend for Python 3.
 Home-page: https://github.com/etianen/django-python3-ldap
 Author: Dave Hall
 Author-email: dave@etianen.com
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `django-python3-ldap-0.9.8/README.rst` & `django-python3-ldap-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-python3-ldap-0.9.8/setup.py` & `django-python3-ldap-0.9.9/setup.py`

 * *Files identical despite different names*

