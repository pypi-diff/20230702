# Comparing `tmp/django_backblaze_b2-3.1.0.tar.gz` & `tmp/django_backblaze_b2-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_backblaze_b2-3.1.0.tar", max compression
+gzip compressed data, was "django_backblaze_b2-3.2.0.tar", max compression
```

## Comparing `django_backblaze_b2-3.1.0.tar` & `django_backblaze_b2-3.2.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-3.1.0/LICENSE
--rw-r--r--   0        0        0     8414 2022-11-07 04:19:10.508445 django_backblaze_b2-3.1.0/README.md
--rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-3.1.0/django_backblaze_b2/__init__.py
--rw-r--r--   0        0        0     1020 2020-09-18 05:11:19.000000 django_backblaze_b2-3.1.0/django_backblaze_b2/_decorators.py
--rw-r--r--   0        0        0     2675 2022-02-20 23:58:19.510901 django_backblaze_b2-3.1.0/django_backblaze_b2/b2_file.py
--rw-r--r--   0        0        0     6784 2022-02-20 23:58:19.511715 django_backblaze_b2-3.1.0/django_backblaze_b2/cache_account_info.py
--rw-r--r--   0        0        0     1957 2021-04-09 06:06:19.000000 django_backblaze_b2-3.1.0/django_backblaze_b2/options.py
--rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-3.1.0/django_backblaze_b2/py.typed
--rw-r--r--   0        0        0    12368 2022-02-20 23:58:19.512503 django_backblaze_b2-3.1.0/django_backblaze_b2/storage.py
--rw-r--r--   0        0        0     4301 2021-06-19 05:28:56.702998 django_backblaze_b2-3.1.0/django_backblaze_b2/storages.py
--rw-r--r--   0        0        0      351 2020-09-18 05:11:19.000000 django_backblaze_b2-3.1.0/django_backblaze_b2/urls.py
--rw-r--r--   0        0        0     2131 2021-06-19 05:28:56.703608 django_backblaze_b2-3.1.0/django_backblaze_b2/views.py
--rw-r--r--   0        0        0     1961 2022-11-07 04:27:20.996602 django_backblaze_b2-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     9396 1970-01-01 00:00:00.000000 django_backblaze_b2-3.1.0/setup.py
--rw-r--r--   0        0        0    10368 1970-01-01 00:00:00.000000 django_backblaze_b2-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-3.2.0/LICENSE
+-rw-r--r--   0        0        0     8414 2023-07-01 06:50:01.842721 django_backblaze_b2-3.2.0/README.md
+-rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-3.2.0/django_backblaze_b2/__init__.py
+-rw-r--r--   0        0        0     1020 2023-07-01 06:50:01.843719 django_backblaze_b2-3.2.0/django_backblaze_b2/_decorators.py
+-rw-r--r--   0        0        0     2675 2023-07-02 05:20:20.087704 django_backblaze_b2-3.2.0/django_backblaze_b2/b2_file.py
+-rw-r--r--   0        0        0     7883 2023-07-02 05:09:27.990342 django_backblaze_b2-3.2.0/django_backblaze_b2/cache_account_info.py
+-rw-r--r--   0        0        0     1957 2023-07-01 06:50:01.845216 django_backblaze_b2-3.2.0/django_backblaze_b2/options.py
+-rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-3.2.0/django_backblaze_b2/py.typed
+-rw-r--r--   0        0        0    12368 2023-07-01 06:50:01.846040 django_backblaze_b2-3.2.0/django_backblaze_b2/storage.py
+-rw-r--r--   0        0        0     4309 2023-07-01 06:50:01.846530 django_backblaze_b2-3.2.0/django_backblaze_b2/storages.py
+-rw-r--r--   0        0        0      351 2023-07-01 06:50:01.847100 django_backblaze_b2-3.2.0/django_backblaze_b2/urls.py
+-rw-r--r--   0        0        0     2131 2023-07-01 06:50:01.847484 django_backblaze_b2-3.2.0/django_backblaze_b2/views.py
+-rw-r--r--   0        0        0     1961 2023-07-02 05:23:16.521145 django_backblaze_b2-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10118 1970-01-01 00:00:00.000000 django_backblaze_b2-3.2.0/PKG-INFO
```

### Comparing `django_backblaze_b2-3.1.0/LICENSE` & `django_backblaze_b2-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.1.0/README.md` & `django_backblaze_b2-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.1.0/django_backblaze_b2/_decorators.py` & `django_backblaze_b2-3.2.0/django_backblaze_b2/_decorators.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.1.0/django_backblaze_b2/b2_file.py` & `django_backblaze_b2-3.2.0/django_backblaze_b2/b2_file.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.1.0/django_backblaze_b2/cache_account_info.py` & `django_backblaze_b2-3.2.0/django_backblaze_b2/cache_account_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
+import threading
 from functools import wraps
 from hashlib import sha3_224 as hash
-from typing import Iterable, Optional, Tuple
+from typing import Iterable, List, Optional, Tuple
 
 from b2sdk.account_info.exception import MissingAccountData
 from b2sdk.account_info.upload_url_pool import UrlPoolAccountInfo
 from django.core.cache import InvalidCacheBackendError, caches
 from django.core.exceptions import ImproperlyConfigured
 
 logger = logging.getLogger("django-backblaze-b2")
@@ -38,19 +39,25 @@
 
     return wrapper_factory
 
 
 class DjangoCacheAccountInfo(UrlPoolAccountInfo):
     """
     Store account information in django's cache: https://docs.djangoproject.com/en/3.1/topics/cache
+
+    Threadsafe only in the context of its own runtime,
+    i.e. it's possible (unlikely though, only in a highly concurrent scenario) that a
+    wrapper of Django could launch 2+ different processes, which would not share threads,
+    and within the 'locked' blocks, mutation of values between cache accesses
     """
 
     def __init__(self, cacheName: str):
         logger.debug(f"Initializing {self.__class__.__name__} with cache '{cacheName}'")
         self._cacheName = cacheName
+        self._cacheLock = threading.Lock()
         try:
             self.cache = caches[cacheName]
             self.cache.set("bucket_names", [])
         except InvalidCacheBackendError:
             logger.exception("Cache assignment failed")
             from django.conf import settings
 
@@ -158,37 +165,56 @@
             return self.cache.get(_bucket_cachekey(bucket_name))
         except KeyError as e:
             logger.debug(f"cache miss {bucket_name}: {e}")
             return None
 
     def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
         try:
+            self._cacheLock.acquire()
             for bucket_name in self.cache.get("bucket_names", []):
-                bucket_id = self.cache.get(_bucket_cachekey(bucket_name))
-                if bucket_id:
+                cached_id = self.cache.get(_bucket_cachekey(bucket_name))
+                if cached_id and cached_id == bucket_id:
                     return bucket_name
             logger.debug(f"cache miss {bucket_id}")
         except KeyError as e:
             logger.debug(f"cache miss {bucket_id}: {e}")
+        finally:
+            self._cacheLock.release()
         return None
 
     def refresh_entire_bucket_name_cache(self, name_id_iterable: Iterable[Tuple[str, str]]):
-        bucket_names_to_remove = set(self.cache.get("bucket_names", [])) - {name for name, id in name_id_iterable}
-        for (bucket_name, bucket_id) in name_id_iterable:
-            self.cache.set(_bucket_cachekey(bucket_name), bucket_id)
-        for bucket_name in bucket_names_to_remove:
-            self.remove_bucket_name(bucket_name)
+        with self._cacheLock:
+            new_bucket_names = set()
+            for bucket_name, bucket_id in name_id_iterable:
+                self.cache.set(_bucket_cachekey(bucket_name), bucket_id)
+                new_bucket_names.add(bucket_name)
+
+            buckets_to_remove = [n for n in self.cache.get("bucket_names", []) if n not in new_bucket_names]
+            for bucket_name in buckets_to_remove:
+                self.cache.delete(_bucket_cachekey(bucket_name))
+
+            self.cache.set("bucket_names", list(new_bucket_names))
 
     def save_bucket(self, bucket: StoredBucketInfo):
-        self.cache.set(_bucket_cachekey(bucket.name), bucket.id_)
-        self.cache.set("bucket_names", list(self.cache.get("bucket_names", [])) + [bucket.name])
+        with self._cacheLock:
+            self.cache.set(_bucket_cachekey(bucket.name), bucket.id_)
+            self.cache.set("bucket_names", self.cache.get("bucket_names", []) + [bucket.name])
 
     def remove_bucket_name(self, bucket_name):
-        self.cache.set("bucket_names", [n for n in self.cache.get("bucket_names", []) if n != bucket_name])
-        self.cache.delete(_bucket_cachekey(bucket_name))
+        with self._cacheLock:
+            self.cache.set("bucket_names", [n for n in self.cache.get("bucket_names", []) if n != bucket_name])
+            self.cache.delete(_bucket_cachekey(bucket_name))
+
+    def list_bucket_names_ids(self) -> List[Tuple[str, str]]:
+        tuples = []
+        with self._cacheLock:
+            for bucket_name in self.cache.get("bucket_names", []):
+                bucket_id = self.cache.get(_bucket_cachekey(bucket_name))
+                tuples.append((bucket_name, bucket_id))
+        return tuples
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}{{cacheName={self._cacheName},cache={self.cache}}}"
 
 
 def _bucket_cachekey(bucket_name: str) -> str:
     return hash(f"bucket-name__{bucket_name}".encode()).hexdigest()
```

### Comparing `django_backblaze_b2-3.1.0/django_backblaze_b2/options.py` & `django_backblaze_b2-3.2.0/django_backblaze_b2/options.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.1.0/django_backblaze_b2/storage.py` & `django_backblaze_b2-3.2.0/django_backblaze_b2/storage.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.1.0/django_backblaze_b2/storages.py` & `django_backblaze_b2-3.2.0/django_backblaze_b2/storages.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class PublicStorage(BackblazeB2Storage):
     """
     Storage that requires no authentication to view.
     If the bucket is public, returns the bucket's url, or CDN if configured
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self._bucketType: Optional[Literal["allPublic", "allPrivate"]] = None
         self._cdnConfig: Optional[CDNConfig] = kwargs.get("opts", {}).get("cdnConfig")
 
     def _isPublicBucket(self) -> bool:
         if self._bucketType is None:
             bucketDict = self.bucket.as_dict()
```

### Comparing `django_backblaze_b2-3.1.0/django_backblaze_b2/views.py` & `django_backblaze_b2-3.2.0/django_backblaze_b2/views.py`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.1.0/setup.py` & `django_backblaze_b2-3.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,205 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-backblaze-b2
+Version: 3.2.0
+Summary: A Django app to use backblaze b2 as storage.
+Home-page: https://github.com/ehossack/django-backblaze-b2/
+License: BSD-2-Clause
+Keywords: django,storage,backblaze,b2,cloud
+Author: Etienne H
+Author-email: django_backblaze_b2@internet-e-mail.com
+Maintainer: Etienne H
+Maintainer-email: django_backblaze_b2@internet-e-mail.com
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Dist: b2sdk (>=1.11.0)
+Requires-Dist: django (>=3.2)
+Requires-Dist: typing-extensions (>=4.0.1,<5.0.0)
+Project-URL: Repository, https://github.com/ehossack/django-backblaze-b2/
+Description-Content-Type: text/markdown
+
+# django-backblaze-b2
+
+[![pypi version](https://img.shields.io/pypi/v/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)
+[![python version](https://img.shields.io/pypi/pyversions/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)
+[![django version](https://img.shields.io/pypi/djversions/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)
+
+A storage backend for Django that uses [Backblaze's B2 APIs](https://www.backblaze.com/b2/cloud-storage.html).
+
+Implementation wraps [Official Python SDK](https://github.com/Backblaze/b2-sdk-python)
+
+## How to use
+
+1. Install from this repo, or install from PyPi: `pip install django-backblaze-b2`
+As tested, requires python 3.7 or greater but solely due to type annotations. PRs welcome :)
+1. Configure your django `settings`. A minimalistic config would be:
+```python
+CACHES = {
+    "default": .... ,
+    # add a cache via db table or memcached that can be accessed from multiple threads
+    "django-backblaze-b2": {
+        'BACKEND': 'django.core.cache.backends.db.DatabaseCache',
+        'LOCATION': 'django_backblaze_b2_cache_table',
+    }
+}
 
-packages = \
-['django_backblaze_b2']
+BACKBLAZE_CONFIG = {
+    # however you want to securely retrieve these values
+    "application_key_id": os.getenv("BACKBLAZE_KEY_ID"),
+    "application_key": os.getenv("BACKBLAZE_KEY"),
+}
+```
 
-package_data = \
-{'': ['*']}
+Theoretically you may now refer to the base storage class as a storage class (see the sample app for some usage: you can run with `make run-sample-proj` although you might want to configure the `SECONDS_TO_RUN_APP` variable in `settings.env` to be 0 for unlimited to try things out)
+e.g.
+```python
+from django_backblaze_b2 import BackblazeB2Storage
 
-install_requires = \
-['b2sdk>=1.11.0', 'django>=3.2', 'typing-extensions>=4.0.1,<5.0.0']
-
-setup_kwargs = {
-    'name': 'django-backblaze-b2',
-    'version': '3.1.0',
-    'description': 'A Django app to use backblaze b2 as storage.',
-    'long_description': '# django-backblaze-b2\n\n[![pypi version](https://img.shields.io/pypi/v/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)\n[![python version](https://img.shields.io/pypi/pyversions/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)\n[![django version](https://img.shields.io/pypi/djversions/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)\n\nA storage backend for Django that uses [Backblaze\'s B2 APIs](https://www.backblaze.com/b2/cloud-storage.html).\n\nImplementation wraps [Official Python SDK](https://github.com/Backblaze/b2-sdk-python)\n\n## How to use\n\n1. Install from this repo, or install from PyPi: `pip install django-backblaze-b2`\nAs tested, requires python 3.7 or greater but solely due to type annotations. PRs welcome :)\n1. Configure your django `settings`. A minimalistic config would be:\n```python\nCACHES = {\n    "default": .... ,\n    # add a cache via db table or memcached that can be accessed from multiple threads\n    "django-backblaze-b2": {\n        \'BACKEND\': \'django.core.cache.backends.db.DatabaseCache\',\n        \'LOCATION\': \'django_backblaze_b2_cache_table\',\n    }\n}\n\nBACKBLAZE_CONFIG = {\n    # however you want to securely retrieve these values\n    "application_key_id": os.getenv("BACKBLAZE_KEY_ID"),\n    "application_key": os.getenv("BACKBLAZE_KEY"),\n}\n```\n\nTheoretically you may now refer to the base storage class as a storage class (see the sample app for some usage: you can run with `make run-sample-proj` although you might want to configure the `SECONDS_TO_RUN_APP` variable in `settings.env` to be 0 for unlimited to try things out)\ne.g.\n```python\nfrom django_backblaze_b2 import BackblazeB2Storage\n\nclass MyModel(models.Model):\n    fileField = models.FileField(\n        upload_to="uploads",\n        storage=BackblazeB2Storage\n    )\n```\n\n### Public/Logged-In/Private storage\n\n1. Add `django_backblaze_b2` to your `INSTALLED_APPS`\n1. Add the urls to your `urlpatterns` in the root `urls.py`:\n```python\n    urlpatterns = [\n        ...\n        path(\'\', include(\'django_backblaze_b2.urls\')),\n    ]\n```\n\n### Caching\n\nTo retrieve file metadata ("file info" as the b2 sdk names it), this library has to authorize and request data from b2 servers, even for just resolving the url for a file. Because these are network calls, and relatively expensive in comparison to a file-based storage, and because data is unlikely to change frequently, there is some caching done by this library.  \nBy default, the account information (`accountInfo`) configuration of the settings uses a cache by the name of `django-backblaze-b2` which you must have in your `CACHES` section of your `settings.py`. This is to leverage django\'s thread-safe cache implementations, and if you are using a database cache table or memcached, (rather than LocMemCache) your cache can be shared by the multiple django processes that typically serve requests.  \nIt is not recommended configure `accountInfo` with the `default` django cache, as the `clear()` method may be called during the backblaze lifecycle.  \nIf you do not wish to use a django cache, you can use a sqlite database on disk for caching, or use a non-thread-safe in-memory implementation. This is only recommended for single-threaded deployments (remember in most deployments a new thread serves each request).  \nFor further discussion on this see https://github.com/ehossack/django-backblaze-b2/issues/16\n\n### Configurations\n\nYou may want to use your own bucket name, or set further configuration such as lazy authorization/validation, or specifying file metadata.  \nRefer to [the options](./django_backblaze_b2/options.py) for all options.  \nYou can modify the settings dict, but additionally override any setting with the `opts` keyword argument to the storage classes.\n\nTo specify different buckets to use for your public, logged-in, staff storage, you can set the \n`specificBucketNames` attribute of the settings dict.\n## Why\n\nThere are several Django storage packages out there already which support B2, but none met my needs. These are:\n\n* [django-storages](https://github.com/jschneier/django-storages)\n    * Large community engagement ✅\n    * Well-tested ✅\n    * [Second-class support](https://github.com/jschneier/django-storages/issues/765) via [Apache Libcloud](https://github.com/apache/libcloud) ❌\n    * Disconnect in configuration and actual use ❌\n    * PR list with low turnaround ❌\n* [django-b2](https://github.com/pyutil/django-b2)\n    * Similar aim to this project, around official backblaze SDK ✅\n    * Mixed goals (storage, scripts) ❌\n    * Tests?? ❌\n* [django-backblazeb2-storage](https://github.com/royendgel/django-backblazeb2-storage)\n    * Simple configuration ✅\n    * Not based around python SDK (potentially harder to keep up with version changes) ❌\n    * Tests?? ❌\n\n### S3 Compatible API\n\nBackblazed can be used with an [S3-compatible API](https://www.backblaze.com/b2/docs/s3_compatible_api.html)\nThis is great, but most packages use an older version of the S3 Api (v2). Backblaze uses v4.\n\n### What this package offers\n\n* Type Annotations\n* Tested\n* No hacks required to get up and running around API deficiencies (any hacks are not exposed in API)\n* Support for public/private files, restricted via Django user permissions\n* Support for CDN and cached url details\n\n## How it works\n\n* A simple implementation of the `django.core.files.storage.Storage` class provides handling for storage behaviour within your Django application\n* Three url routes are appended to the root of your application:  \n    1. `/b2/`\n    2. `/b2l/`\n    3. `/b2s/`\nThese routes act as a proxy/intermediary between the requester and backblaze b2 apis. The public `/b2/` allows exposing files from a private bucket, and the logged-in and staff routes will perform the known validations of a django app to prevent unauthorized access.\n* If you use a CDN config, you can specify the CDN options and then include the bucket url segments (`/file/<bucket-name>/`) if your CDN is proxying the classic b2 url (e.g. `f000.backblazeb2.com`) or not, if you are proxying the s3-compatible url.\n\n### Gotchas\n\n* The original filename + any upload paths is stored in the database. Thus your column name must be of sufficient length to hold that (unchanged behaviour from `FileSystemStorage`)\n*  When retrieving files from the `PublicStorage`, `LoggedInStorage` or `StaffStorage`, you may not override the `"bucket"` or authorization options, or else when the app proxies the file download, it will be unable to retrieve the file from the respective bucket.\n* Simply using `LoggedInStorage` or `StaffStorage` is not enough to protect your files if your bucket is not public. If any individual gains access to the file ids/urls for these files, there is no authentication around them. It is up to the implementer to ensure the security of their application.\n* Once the file is uploaded, and someone obtains a file url (e.g. http://djangodomain.com/b2l/uploads/image.png), the django model is no longer involved in file resolution. This means that if you share the bucket between multiple use-cases, you could in theory find files that don\'t belong to your django app (e.g. some image2.png), or similarly if you delete/change your models, the files could still be downloaded. Consider using an app like [django-cleanup](https://github.com/un1t/django-cleanup) if this is important to you\n\n## Contributing\n\nContributions welcome!\n\n* Please ensure test coverage does not decrease in a meaningful way.\n* Ensure formatting is compliant (`make lint`)\n* Use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)\n\n## Setting up for development\n\n### Requires\n\n* python\n* pyenv - align local version\n* GNU Make\n* (optional) docker - run sample app\n\n#### Version compatibility reminder\n\n| Ver  | Status   |  EOL       |\n| ---- | -------- | ---------- |\n| 3.11 | buffix   | 2027-10    |\n| 3.10 | bugfix   | 2026-10    |\n| 3.9  | bugfix   | 2025-10    |\n| 3.8  | bugfix   | 2024-10    |\n| 3.7  | security | 2023-06-27 |\n\n### Running\n\n1. `make setup`\n\n* You can run django with `make run-django` to test django app.\n* You can run tests with `make test`\n* You can view test coverage with `make test-coverage`, then see in the terminal, \nopen `test/htmlcov/index.html`\nor use `cov.xml` in your favourite IDE like VSCode\n\n### Releasing\n\n1. `make publish-to-pypi`\n\n### Cleanup\n\n1. `make cleanup`\n',
-    'author': 'Etienne H',
-    'author_email': 'django_backblaze_b2@internet-e-mail.com',
-    'maintainer': 'Etienne H',
-    'maintainer_email': 'django_backblaze_b2@internet-e-mail.com',
-    'url': 'https://github.com/ehossack/django-backblaze-b2/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
+class MyModel(models.Model):
+    fileField = models.FileField(
+        upload_to="uploads",
+        storage=BackblazeB2Storage
+    )
+```
+
+### Public/Logged-In/Private storage
+
+1. Add `django_backblaze_b2` to your `INSTALLED_APPS`
+1. Add the urls to your `urlpatterns` in the root `urls.py`:
+```python
+    urlpatterns = [
+        ...
+        path('', include('django_backblaze_b2.urls')),
+    ]
+```
+
+### Caching
+
+To retrieve file metadata ("file info" as the b2 sdk names it), this library has to authorize and request data from b2 servers, even for just resolving the url for a file. Because these are network calls, and relatively expensive in comparison to a file-based storage, and because data is unlikely to change frequently, there is some caching done by this library.  
+By default, the account information (`accountInfo`) configuration of the settings uses a cache by the name of `django-backblaze-b2` which you must have in your `CACHES` section of your `settings.py`. This is to leverage django's thread-safe cache implementations, and if you are using a database cache table or memcached, (rather than LocMemCache) your cache can be shared by the multiple django processes that typically serve requests.  
+It is not recommended configure `accountInfo` with the `default` django cache, as the `clear()` method may be called during the backblaze lifecycle.  
+If you do not wish to use a django cache, you can use a sqlite database on disk for caching, or use a non-thread-safe in-memory implementation. This is only recommended for single-threaded deployments (remember in most deployments a new thread serves each request).  
+For further discussion on this see https://github.com/ehossack/django-backblaze-b2/issues/16
+
+### Configurations
+
+You may want to use your own bucket name, or set further configuration such as lazy authorization/validation, or specifying file metadata.  
+Refer to [the options](./django_backblaze_b2/options.py) for all options.  
+You can modify the settings dict, but additionally override any setting with the `opts` keyword argument to the storage classes.
+
+To specify different buckets to use for your public, logged-in, staff storage, you can set the 
+`specificBucketNames` attribute of the settings dict.
+## Why
+
+There are several Django storage packages out there already which support B2, but none met my needs. These are:
+
+* [django-storages](https://github.com/jschneier/django-storages)
+    * Large community engagement ✅
+    * Well-tested ✅
+    * [Second-class support](https://github.com/jschneier/django-storages/issues/765) via [Apache Libcloud](https://github.com/apache/libcloud) ❌
+    * Disconnect in configuration and actual use ❌
+    * PR list with low turnaround ❌
+* [django-b2](https://github.com/pyutil/django-b2)
+    * Similar aim to this project, around official backblaze SDK ✅
+    * Mixed goals (storage, scripts) ❌
+    * Tests?? ❌
+* [django-backblazeb2-storage](https://github.com/royendgel/django-backblazeb2-storage)
+    * Simple configuration ✅
+    * Not based around python SDK (potentially harder to keep up with version changes) ❌
+    * Tests?? ❌
+
+### S3 Compatible API
+
+Backblazed can be used with an [S3-compatible API](https://www.backblaze.com/b2/docs/s3_compatible_api.html)
+This is great, but most packages use an older version of the S3 Api (v2). Backblaze uses v4.
+
+### What this package offers
+
+* Type Annotations
+* Tested
+* No hacks required to get up and running around API deficiencies (any hacks are not exposed in API)
+* Support for public/private files, restricted via Django user permissions
+* Support for CDN and cached url details
+
+## How it works
+
+* A simple implementation of the `django.core.files.storage.Storage` class provides handling for storage behaviour within your Django application
+* Three url routes are appended to the root of your application:  
+    1. `/b2/`
+    2. `/b2l/`
+    3. `/b2s/`
+These routes act as a proxy/intermediary between the requester and backblaze b2 apis. The public `/b2/` allows exposing files from a private bucket, and the logged-in and staff routes will perform the known validations of a django app to prevent unauthorized access.
+* If you use a CDN config, you can specify the CDN options and then include the bucket url segments (`/file/<bucket-name>/`) if your CDN is proxying the classic b2 url (e.g. `f000.backblazeb2.com`) or not, if you are proxying the s3-compatible url.
+
+### Gotchas
+
+* The original filename + any upload paths is stored in the database. Thus your column name must be of sufficient length to hold that (unchanged behaviour from `FileSystemStorage`)
+*  When retrieving files from the `PublicStorage`, `LoggedInStorage` or `StaffStorage`, you may not override the `"bucket"` or authorization options, or else when the app proxies the file download, it will be unable to retrieve the file from the respective bucket.
+* Simply using `LoggedInStorage` or `StaffStorage` is not enough to protect your files if your bucket is not public. If any individual gains access to the file ids/urls for these files, there is no authentication around them. It is up to the implementer to ensure the security of their application.
+* Once the file is uploaded, and someone obtains a file url (e.g. http://djangodomain.com/b2l/uploads/image.png), the django model is no longer involved in file resolution. This means that if you share the bucket between multiple use-cases, you could in theory find files that don't belong to your django app (e.g. some image2.png), or similarly if you delete/change your models, the files could still be downloaded. Consider using an app like [django-cleanup](https://github.com/un1t/django-cleanup) if this is important to you
+
+## Contributing
+
+Contributions welcome!
+
+* Please ensure test coverage does not decrease in a meaningful way.
+* Ensure formatting is compliant (`make lint`)
+* Use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
+
+## Setting up for development
+
+### Requires
+
+* python
+* pyenv - align local version
+* GNU Make
+* (optional) docker - run sample app
+
+#### Version compatibility reminder
+
+| Ver  | Status   |  EOL       |
+| ---- | -------- | ---------- |
+| 3.11 | buffix   | 2027-10    |
+| 3.10 | bugfix   | 2026-10    |
+| 3.9  | bugfix   | 2025-10    |
+| 3.8  | bugfix   | 2024-10    |
+| 3.7  | security | 2023-06-27 |
+
+### Running
+
+1. `make setup`
+
+* You can run django with `make run-django` to test django app.
+* You can run tests with `make test`
+* You can view test coverage with `make test-coverage`, then see in the terminal, 
+open `test/htmlcov/index.html`
+or use `cov.xml` in your favourite IDE like VSCode
+
+### Releasing
+
+1. `make publish-to-pypi`
+
+### Cleanup
 
+1. `make cleanup`
 
-setup(**setup_kwargs)
```

