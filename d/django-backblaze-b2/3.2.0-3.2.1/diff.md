# Comparing `tmp/django_backblaze_b2-3.2.0.tar.gz` & `tmp/django_backblaze_b2-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_backblaze_b2-3.2.0.tar", max compression
+gzip compressed data, was "django_backblaze_b2-3.2.1.tar", max compression
```

## Comparing `django_backblaze_b2-3.2.0.tar` & `django_backblaze_b2-3.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-3.2.0/LICENSE
--rw-r--r--   0        0        0     8414 2023-07-01 06:50:01.842721 django_backblaze_b2-3.2.0/README.md
--rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-3.2.0/django_backblaze_b2/__init__.py
--rw-r--r--   0        0        0     1020 2023-07-01 06:50:01.843719 django_backblaze_b2-3.2.0/django_backblaze_b2/_decorators.py
--rw-r--r--   0        0        0     2675 2023-07-02 05:20:20.087704 django_backblaze_b2-3.2.0/django_backblaze_b2/b2_file.py
--rw-r--r--   0        0        0     7883 2023-07-02 05:09:27.990342 django_backblaze_b2-3.2.0/django_backblaze_b2/cache_account_info.py
--rw-r--r--   0        0        0     1957 2023-07-01 06:50:01.845216 django_backblaze_b2-3.2.0/django_backblaze_b2/options.py
--rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-3.2.0/django_backblaze_b2/py.typed
--rw-r--r--   0        0        0    12368 2023-07-01 06:50:01.846040 django_backblaze_b2-3.2.0/django_backblaze_b2/storage.py
--rw-r--r--   0        0        0     4309 2023-07-01 06:50:01.846530 django_backblaze_b2-3.2.0/django_backblaze_b2/storages.py
--rw-r--r--   0        0        0      351 2023-07-01 06:50:01.847100 django_backblaze_b2-3.2.0/django_backblaze_b2/urls.py
--rw-r--r--   0        0        0     2131 2023-07-01 06:50:01.847484 django_backblaze_b2-3.2.0/django_backblaze_b2/views.py
--rw-r--r--   0        0        0     1961 2023-07-02 05:23:16.521145 django_backblaze_b2-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    10118 1970-01-01 00:00:00.000000 django_backblaze_b2-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-3.2.1/LICENSE
+-rw-r--r--   0        0        0     8414 2023-07-01 06:50:01.842721 django_backblaze_b2-3.2.1/README.md
+-rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-3.2.1/django_backblaze_b2/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-01 06:50:01.843719 django_backblaze_b2-3.2.1/django_backblaze_b2/_decorators.py
+-rw-r--r--   0        0        0     2668 2023-07-02 05:32:52.756591 django_backblaze_b2-3.2.1/django_backblaze_b2/b2_file.py
+-rw-r--r--   0        0        0     7883 2023-07-02 05:09:27.990342 django_backblaze_b2-3.2.1/django_backblaze_b2/cache_account_info.py
+-rw-r--r--   0        0        0     1957 2023-07-01 06:50:01.845216 django_backblaze_b2-3.2.1/django_backblaze_b2/options.py
+-rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-3.2.1/django_backblaze_b2/py.typed
+-rw-r--r--   0        0        0    12368 2023-07-01 06:50:01.846040 django_backblaze_b2-3.2.1/django_backblaze_b2/storage.py
+-rw-r--r--   0        0        0     4309 2023-07-01 06:50:01.846530 django_backblaze_b2-3.2.1/django_backblaze_b2/storages.py
+-rw-r--r--   0        0        0      351 2023-07-01 06:50:01.847100 django_backblaze_b2-3.2.1/django_backblaze_b2/urls.py
+-rw-r--r--   0        0        0     2131 2023-07-01 06:50:01.847484 django_backblaze_b2-3.2.1/django_backblaze_b2/views.py
+-rw-r--r--   0        0        0     1960 2023-07-02 05:34:38.637551 django_backblaze_b2-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10118 1970-01-01 00:00:00.000000 django_backblaze_b2-3.2.1/PKG-INFO
```

### Comparing `django_backblaze_b2-3.2.0/LICENSE` & `django_backblaze_b2-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.2.0/README.md` & `django_backblaze_b2-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.2.0/django_backblaze_b2/_decorators.py` & `django_backblaze_b2-3.2.1/django_backblaze_b2/_decorators.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.2.0/django_backblaze_b2/b2_file.py` & `django_backblaze_b2-3.2.1/django_backblaze_b2/b2_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         if not hasattr(self, "_size"):
             self._size = self._sizeProvider(self.name)
         return self._size
 
     def read(self, num_bytes: Optional[int] = None) -> bytes:
         return self.file.read(num_bytes if isinstance(num_bytes, int) else -1)
 
-    def write(self, content: bytes) -> int:
+    def write(self, content) -> int:
         if "w" not in self._mode:
             raise AttributeError("File was not opened for write access.")
         self.file = BytesIO(content)
 
         self._hasUnwrittenData = True
         return len(content)
```

### Comparing `django_backblaze_b2-3.2.0/django_backblaze_b2/cache_account_info.py` & `django_backblaze_b2-3.2.1/django_backblaze_b2/cache_account_info.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.2.0/django_backblaze_b2/options.py` & `django_backblaze_b2-3.2.1/django_backblaze_b2/options.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.2.0/django_backblaze_b2/storage.py` & `django_backblaze_b2-3.2.1/django_backblaze_b2/storage.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.2.0/django_backblaze_b2/storages.py` & `django_backblaze_b2-3.2.1/django_backblaze_b2/storages.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.2.0/django_backblaze_b2/views.py` & `django_backblaze_b2-3.2.1/django_backblaze_b2/views.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.2.0/pyproject.toml` & `django_backblaze_b2-3.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "django-backblaze-b2"
-version = "3.2.0"
+version = "3.2.1"
 description = "A Django app to use backblaze b2 as storage."
 authors = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 maintainers = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 homepage = "https://github.com/ehossack/django-backblaze-b2/"
 repository = "https://github.com/ehossack/django-backblaze-b2/"
@@ -51,15 +51,15 @@
 typing-extensions = "^4.0.1"
 
 [tool.poetry.dev-dependencies]
 isort = "^5.11.5"
 pytest = "^7.3"
 mypy = ">=0.8"
 black = "^23.3"
-django-stubs = "^1.16.0"
+django-stubs = "^4.2.0"
 flake8 = "^5.0"
 pytest-cov = "^4.0"
 pytest-django = "^4.5"
 pytest-pythonpath = "^0.7"
 docutils = "^0.19"
 toml = "^0.10.2"
```

### Comparing `django_backblaze_b2-3.2.0/PKG-INFO` & `django_backblaze_b2-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-backblaze-b2
-Version: 3.2.0
+Version: 3.2.1
 Summary: A Django app to use backblaze b2 as storage.
 Home-page: https://github.com/ehossack/django-backblaze-b2/
 License: BSD-2-Clause
 Keywords: django,storage,backblaze,b2,cloud
 Author: Etienne H
 Author-email: django_backblaze_b2@internet-e-mail.com
 Maintainer: Etienne H
```

