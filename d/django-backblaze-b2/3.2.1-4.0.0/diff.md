# Comparing `tmp/django_backblaze_b2-3.2.1.tar.gz` & `tmp/django_backblaze_b2-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_backblaze_b2-3.2.1.tar", max compression
+gzip compressed data, was "django_backblaze_b2-4.0.0.tar", max compression
```

## Comparing `django_backblaze_b2-3.2.1.tar` & `django_backblaze_b2-4.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-3.2.1/LICENSE
--rw-r--r--   0        0        0     8414 2023-07-01 06:50:01.842721 django_backblaze_b2-3.2.1/README.md
--rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-3.2.1/django_backblaze_b2/__init__.py
--rw-r--r--   0        0        0     1020 2023-07-01 06:50:01.843719 django_backblaze_b2-3.2.1/django_backblaze_b2/_decorators.py
--rw-r--r--   0        0        0     2668 2023-07-02 05:32:52.756591 django_backblaze_b2-3.2.1/django_backblaze_b2/b2_file.py
--rw-r--r--   0        0        0     7883 2023-07-02 05:09:27.990342 django_backblaze_b2-3.2.1/django_backblaze_b2/cache_account_info.py
--rw-r--r--   0        0        0     1957 2023-07-01 06:50:01.845216 django_backblaze_b2-3.2.1/django_backblaze_b2/options.py
--rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-3.2.1/django_backblaze_b2/py.typed
--rw-r--r--   0        0        0    12368 2023-07-01 06:50:01.846040 django_backblaze_b2-3.2.1/django_backblaze_b2/storage.py
--rw-r--r--   0        0        0     4309 2023-07-01 06:50:01.846530 django_backblaze_b2-3.2.1/django_backblaze_b2/storages.py
--rw-r--r--   0        0        0      351 2023-07-01 06:50:01.847100 django_backblaze_b2-3.2.1/django_backblaze_b2/urls.py
--rw-r--r--   0        0        0     2131 2023-07-01 06:50:01.847484 django_backblaze_b2-3.2.1/django_backblaze_b2/views.py
--rw-r--r--   0        0        0     1960 2023-07-02 05:34:38.637551 django_backblaze_b2-3.2.1/pyproject.toml
--rw-r--r--   0        0        0    10118 1970-01-01 00:00:00.000000 django_backblaze_b2-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1318 2020-08-25 16:03:37.000000 django_backblaze_b2-4.0.0/LICENSE
+-rw-r--r--   0        0        0     8556 2023-07-02 20:36:28.971655 django_backblaze_b2-4.0.0/README.md
+-rw-r--r--   0        0        0      264 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.0/django_backblaze_b2/__init__.py
+-rw-r--r--   0        0        0     1024 2023-07-02 20:36:25.735529 django_backblaze_b2-4.0.0/django_backblaze_b2/_decorators.py
+-rw-r--r--   0        0        0     2720 2023-07-02 20:36:25.735944 django_backblaze_b2-4.0.0/django_backblaze_b2/b2_file.py
+-rw-r--r--   0        0        0     7932 2023-07-02 20:36:25.736279 django_backblaze_b2-4.0.0/django_backblaze_b2/cache_account_info.py
+-rw-r--r--   0        0        0     2004 2023-07-02 20:36:25.736571 django_backblaze_b2-4.0.0/django_backblaze_b2/options.py
+-rw-r--r--   0        0        0        0 2020-09-18 05:30:12.000000 django_backblaze_b2-4.0.0/django_backblaze_b2/py.typed
+-rw-r--r--   0        0        0    12923 2023-07-02 20:36:25.736917 django_backblaze_b2-4.0.0/django_backblaze_b2/storage.py
+-rw-r--r--   0        0        0     4727 2023-07-02 20:36:25.737269 django_backblaze_b2-4.0.0/django_backblaze_b2/storages.py
+-rw-r--r--   0        0        0      358 2023-07-02 20:36:25.737573 django_backblaze_b2-4.0.0/django_backblaze_b2/urls.py
+-rw-r--r--   0        0        0     2167 2023-07-02 20:36:25.737820 django_backblaze_b2-4.0.0/django_backblaze_b2/views.py
+-rw-r--r--   0        0        0     2022 2023-07-02 20:36:37.394079 django_backblaze_b2-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    10260 1970-01-01 00:00:00.000000 django_backblaze_b2-4.0.0/PKG-INFO
```

### Comparing `django_backblaze_b2-3.2.1/LICENSE` & `django_backblaze_b2-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_backblaze_b2-3.2.1/README.md` & `django_backblaze_b2-4.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 [![python version](https://img.shields.io/pypi/pyversions/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)
 [![django version](https://img.shields.io/pypi/djversions/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)
 
 A storage backend for Django that uses [Backblaze's B2 APIs](https://www.backblaze.com/b2/cloud-storage.html).
 
 Implementation wraps [Official Python SDK](https://github.com/Backblaze/b2-sdk-python)
 
+## Changelog / Releases
+
+See [https://github.com/ehossack/django-backblaze-b2/releases](https://github.com/ehossack/django-backblaze-b2/releases)
+
 ## How to use
 
 1. Install from this repo, or install from PyPi: `pip install django-backblaze-b2`
 As tested, requires python 3.7 or greater but solely due to type annotations. PRs welcome :)
 1. Configure your django `settings`. A minimalistic config would be:
 ```python
 CACHES = {
@@ -32,15 +36,15 @@
 
 Theoretically you may now refer to the base storage class as a storage class (see the sample app for some usage: you can run with `make run-sample-proj` although you might want to configure the `SECONDS_TO_RUN_APP` variable in `settings.env` to be 0 for unlimited to try things out)
 e.g.
 ```python
 from django_backblaze_b2 import BackblazeB2Storage
 
 class MyModel(models.Model):
-    fileField = models.FileField(
+    file_field = models.FileField(
         upload_to="uploads",
         storage=BackblazeB2Storage
     )
 ```
 
 ### Public/Logged-In/Private storage
 
@@ -52,16 +56,16 @@
         path('', include('django_backblaze_b2.urls')),
     ]
 ```
 
 ### Caching
 
 To retrieve file metadata ("file info" as the b2 sdk names it), this library has to authorize and request data from b2 servers, even for just resolving the url for a file. Because these are network calls, and relatively expensive in comparison to a file-based storage, and because data is unlikely to change frequently, there is some caching done by this library.  
-By default, the account information (`accountInfo`) configuration of the settings uses a cache by the name of `django-backblaze-b2` which you must have in your `CACHES` section of your `settings.py`. This is to leverage django's thread-safe cache implementations, and if you are using a database cache table or memcached, (rather than LocMemCache) your cache can be shared by the multiple django processes that typically serve requests.  
-It is not recommended configure `accountInfo` with the `default` django cache, as the `clear()` method may be called during the backblaze lifecycle.  
+By default, the account information (`account_info`) configuration of the settings uses a cache by the name of `django-backblaze-b2` which you must have in your `CACHES` section of your `settings.py`. This is to leverage django's thread-safe cache implementations, and if you are using a database cache table or memcached, (rather than LocMemCache) your cache can be shared by the multiple django processes that typically serve requests.  
+It is not recommended configure `account_info` with the `default` django cache, as the `clear()` method may be called during the backblaze lifecycle.  
 If you do not wish to use a django cache, you can use a sqlite database on disk for caching, or use a non-thread-safe in-memory implementation. This is only recommended for single-threaded deployments (remember in most deployments a new thread serves each request).  
 For further discussion on this see https://github.com/ehossack/django-backblaze-b2/issues/16
 
 ### Configurations
 
 You may want to use your own bucket name, or set further configuration such as lazy authorization/validation, or specifying file metadata.  
 Refer to [the options](./django_backblaze_b2/options.py) for all options.  
@@ -153,12 +157,12 @@
 * You can run tests with `make test`
 * You can view test coverage with `make test-coverage`, then see in the terminal, 
 open `test/htmlcov/index.html`
 or use `cov.xml` in your favourite IDE like VSCode
 
 ### Releasing
 
-1. `make publish-to-pypi`
+1. `make release`
 
 ### Cleanup
 
 1. `make cleanup`
```

### Comparing `django_backblaze_b2-3.2.1/django_backblaze_b2/_decorators.py` & `django_backblaze_b2-4.0.0/django_backblaze_b2/_decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from functools import wraps
 
 from django.http import HttpRequest, HttpResponse
 from django.utils.translation import gettext_lazy as _
 
 
-def requiresLogin(requiresStaff=False):
+def _requires_login(requires_staff=False):
     """
     Decorator for views that checks that the user passes the given test,
     redirecting to the log-in page if necessary. The test should be a callable
     that takes the user object and returns True if the user passes.
     """
 
     def decorator(view_func):
         @wraps(view_func)
         def _wrapped_view(request: HttpRequest, *args, **kwargs):
             from django.contrib.auth.views import redirect_to_login  # delay import in case custom user model
 
             if request.user.is_anonymous:
                 return redirect_to_login(request.get_full_path())
-            if not request.user.is_active or (requiresStaff and not request.user.is_staff):
+            if not request.user.is_active or (requires_staff and not request.user.is_staff):
                 return HttpResponse(_("Unauthorized"), status=401)
             return view_func(request, *args, **kwargs)
 
         return _wrapped_view
 
     return decorator
```

### Comparing `django_backblaze_b2-3.2.1/django_backblaze_b2/b2_file.py` & `django_backblaze_b2-4.0.0/django_backblaze_b2/b2_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,74 +11,74 @@
 class B2File(File):
     """Read/Write as lazy as possible"""
 
     def __init__(
         self,
         name: str,
         bucket: Bucket,
-        sizeProvider: Callable[[str], int],
-        fileMetadata: Dict[str, Any],
+        size_provider: Callable[[str], int],
+        file_metadata: Dict[str, Any],
         mode: str,
     ):
         self.name: str = name
         self._bucket: Bucket = bucket
-        self._sizeProvider = sizeProvider
-        self._fileMetadata = fileMetadata
+        self._size_provider = size_provider
+        self._file_metadata = file_metadata
         self._mode: str = mode
-        self._hasUnwrittenData: bool = False
+        self._has_unwritted_data: bool = False
         self._contents: Optional[IO] = None
 
     # https://github.com/python/mypy/issues/4125 -- kinda makes you wonder why we like mypy?
     @property  # type: ignore
     def file(self) -> IO[Any]:  # type: ignore
         if self._contents is None:
-            self._contents = self._readFileContents()
+            self._contents = self._read_file_contents()
         return self._contents
 
     # https://github.com/python/mypy/issues/1465
     @file.setter  # type: ignore
     def file(self, value: IO[Any]) -> None:
         self._contents = value
 
-    def _readFileContents(self) -> BytesIO:
-        downloadingFile = self._bucket.download_file_by_name(file_name=self.name)
-        bytesIO = BytesIO()
-        downloadingFile.save(bytesIO)
-        contents = BytesIO(bytesIO.getvalue())
-        bytesIO.close()
+    def _read_file_contents(self) -> BytesIO:
+        currently_downloading_file = self._bucket.download_file_by_name(file_name=self.name)
+        bytes_io = BytesIO()
+        currently_downloading_file.save(bytes_io)
+        contents = BytesIO(bytes_io.getvalue())
+        bytes_io.close()
         return contents
 
     @property
     def size(self) -> int:
         if not hasattr(self, "_size"):
-            self._size = self._sizeProvider(self.name)
+            self._size = self._size_provider(self.name)
         return self._size
 
     def read(self, num_bytes: Optional[int] = None) -> bytes:
         return self.file.read(num_bytes if isinstance(num_bytes, int) else -1)
 
     def write(self, content) -> int:
         if "w" not in self._mode:
             raise AttributeError("File was not opened for write access.")
         self.file = BytesIO(content)
 
-        self._hasUnwrittenData = True
+        self._has_unwritted_data = True
         return len(content)
 
     def close(self) -> None:
-        if self._hasUnwrittenData:
-            self.saveAndRetrieveFile(self.file)
+        if self._has_unwritted_data:
+            self.save_and_retrieve_file(self.file)
         self.file.close()
 
-    def saveAndRetrieveFile(self, content: IO[Any]) -> str:
+    def save_and_retrieve_file(self, content: IO[Any]) -> str:
         """
         Save and retrieve the filename.
         If the file exists it will make another version of that file.
         """
         logger.debug(f"Saving {self.name} to b2 bucket ({self._bucket.get_id()})")
         self._bucket.upload_bytes(
             data_bytes=content.read(),
             file_name=self.name,
-            file_infos=self._fileMetadata,
+            file_infos=self._file_metadata,
         )
-        self._hasUnwrittenData = False
+        self._has_unwritted_data = False
         return self.name
```

### Comparing `django_backblaze_b2-3.2.1/django_backblaze_b2/cache_account_info.py` & `django_backblaze_b2-4.0.0/django_backblaze_b2/cache_account_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,36 +46,38 @@
 
     Threadsafe only in the context of its own runtime,
     i.e. it's possible (unlikely though, only in a highly concurrent scenario) that a
     wrapper of Django could launch 2+ different processes, which would not share threads,
     and within the 'locked' blocks, mutation of values between cache accesses
     """
 
-    def __init__(self, cacheName: str):
-        logger.debug(f"Initializing {self.__class__.__name__} with cache '{cacheName}'")
-        self._cacheName = cacheName
-        self._cacheLock = threading.Lock()
+    def __init__(self, cache_name: str):
+        logger.debug(f"Initializing {self.__class__.__name__} with cache '{cache_name}'")
+        self._cache_name = cache_name
+        self._cache_lock = threading.Lock()
         try:
-            self.cache = caches[cacheName]
+            self.cache = caches[cache_name]
             self.cache.set("bucket_names", [])
         except InvalidCacheBackendError:
             logger.exception("Cache assignment failed")
             from django.conf import settings
 
-            helpMessage = (
+            help_message = (
                 (
                     ". "
-                    "The default 'accountInfo' option of this library is with a django cache"
+                    "The default 'account_info' option of this library is with a django cache"
                     " by the name of 'django-backblaze-b2'"
                 )
-                if "accountInfo" not in settings.BACKBLAZE_CONFIG
+                if "account_info" not in settings.BACKBLAZE_CONFIG
                 else ""
             )
 
-            raise ImproperlyConfigured(f"Expected to find a cache with name '{cacheName}' as per options" + helpMessage)
+            raise ImproperlyConfigured(
+                f"Expected to find a cache with name '{cache_name}' as per options" + help_message
+            )
         super(DjangoCacheAccountInfo, self).__init__()
 
     def clear(self):
         """
         Remove all info about accounts and buckets.
         """
         self.cache.clear()
@@ -165,56 +167,56 @@
             return self.cache.get(_bucket_cachekey(bucket_name))
         except KeyError as e:
             logger.debug(f"cache miss {bucket_name}: {e}")
             return None
 
     def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
         try:
-            self._cacheLock.acquire()
+            self._cache_lock.acquire()
             for bucket_name in self.cache.get("bucket_names", []):
                 cached_id = self.cache.get(_bucket_cachekey(bucket_name))
                 if cached_id and cached_id == bucket_id:
                     return bucket_name
             logger.debug(f"cache miss {bucket_id}")
         except KeyError as e:
             logger.debug(f"cache miss {bucket_id}: {e}")
         finally:
-            self._cacheLock.release()
+            self._cache_lock.release()
         return None
 
     def refresh_entire_bucket_name_cache(self, name_id_iterable: Iterable[Tuple[str, str]]):
-        with self._cacheLock:
+        with self._cache_lock:
             new_bucket_names = set()
             for bucket_name, bucket_id in name_id_iterable:
                 self.cache.set(_bucket_cachekey(bucket_name), bucket_id)
                 new_bucket_names.add(bucket_name)
 
             buckets_to_remove = [n for n in self.cache.get("bucket_names", []) if n not in new_bucket_names]
             for bucket_name in buckets_to_remove:
                 self.cache.delete(_bucket_cachekey(bucket_name))
 
             self.cache.set("bucket_names", list(new_bucket_names))
 
     def save_bucket(self, bucket: StoredBucketInfo):
-        with self._cacheLock:
+        with self._cache_lock:
             self.cache.set(_bucket_cachekey(bucket.name), bucket.id_)
             self.cache.set("bucket_names", self.cache.get("bucket_names", []) + [bucket.name])
 
     def remove_bucket_name(self, bucket_name):
-        with self._cacheLock:
+        with self._cache_lock:
             self.cache.set("bucket_names", [n for n in self.cache.get("bucket_names", []) if n != bucket_name])
             self.cache.delete(_bucket_cachekey(bucket_name))
 
     def list_bucket_names_ids(self) -> List[Tuple[str, str]]:
         tuples = []
-        with self._cacheLock:
+        with self._cache_lock:
             for bucket_name in self.cache.get("bucket_names", []):
                 bucket_id = self.cache.get(_bucket_cachekey(bucket_name))
                 tuples.append((bucket_name, bucket_id))
         return tuples
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}{{cacheName={self._cacheName},cache={self.cache}}}"
+        return f"{self.__class__.__name__}{{cache_name={self._cache_name},cache={self.cache}}}"
 
 
 def _bucket_cachekey(bucket_name: str) -> str:
     return hash(f"bucket-name__{bucket_name}".encode()).hexdigest()
```

### Comparing `django_backblaze_b2-3.2.1/django_backblaze_b2/options.py` & `django_backblaze_b2-4.0.0/django_backblaze_b2/options.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 from typing import Any, Dict, Optional, Union
 
 from typing_extensions import Literal, TypedDict
 
 
 class ProxiedBucketNames(TypedDict):
     public: Optional[str]
-    loggedIn: Optional[str]
+    logged_in: Optional[str]
     staff: Optional[str]
 
 
 class DjangoCacheAccountInfoConfig(TypedDict):
     type: Literal["django-cache"]
     cache: str
 
 
 class InMemoryAccountInfoConfig(TypedDict):
     type: Literal["memory"]
 
 
 class SqliteAccountInfoConfig(TypedDict):
     type: Literal["sqlite"]
-    databasePath: str
+    database_path: str
 
 
 class CDNConfig(TypedDict):
-    baseUrl: str
-    includeBucketUrlSegments: bool
+    base_url: str
+    include_bucket_url_segments: bool
 
 
 class BackblazeB2StorageOptions(TypedDict):
     """Configuration options."""
 
     realm: str  # default "production"
     application_key_id: str
     application_key: str
     bucket: str
-    authorizeOnInit: bool
-    validateOnInit: bool
-    allowFileOverwrites: bool
-    accountInfo: Optional[Union[DjangoCacheAccountInfoConfig, InMemoryAccountInfoConfig, SqliteAccountInfoConfig]]
-    forbidFilePropertyCaching: bool
-    specificBucketNames: ProxiedBucketNames
-    cdnConfig: Optional[CDNConfig]
+    authorize_on_init: bool
+    validate_on_init: bool
+    allow_file_overwrites: bool
+    account_info: Optional[Union[DjangoCacheAccountInfoConfig, InMemoryAccountInfoConfig, SqliteAccountInfoConfig]]
+    forbid_file_property_caching: bool
+    specific_bucket_names: ProxiedBucketNames
+    cdn_config: Optional[CDNConfig]
     # see: https://b2-sdk-python.readthedocs.io/en/master/api/api.html#b2sdk.v1.B2Api.create_bucket
-    nonExistentBucketDetails: Optional[Dict[str, Union[str, Dict[str, Any]]]]
-    defaultFileInfo: Dict[str, Any]
+    non_existent_bucket_details: Optional[Dict[str, Union[str, Dict[str, Any]]]]
+    default_file_info: Dict[str, Any]
 
 
-def getDefaultB2StorageOptions() -> BackblazeB2StorageOptions:
+def get_default_b2_storage_options() -> BackblazeB2StorageOptions:
     return {
         "realm": "production",
         "application_key_id": "you must set this value yourself",
         "application_key": "you must set this value yourself",
         "bucket": "django",
-        "authorizeOnInit": True,
-        "validateOnInit": True,
-        "allowFileOverwrites": False,
-        "accountInfo": {"type": "django-cache", "cache": "django-backblaze-b2"},
-        "forbidFilePropertyCaching": False,
-        "specificBucketNames": {"public": None, "loggedIn": None, "staff": None},
-        "cdnConfig": None,
-        "nonExistentBucketDetails": None,
-        "defaultFileInfo": {},
+        "authorize_on_init": True,
+        "validate_on_init": True,
+        "allow_file_overwrites": False,
+        "account_info": {"type": "django-cache", "cache": "django-backblaze-b2"},
+        "forbid_file_property_caching": False,
+        "specific_bucket_names": {"public": None, "logged_in": None, "staff": None},
+        "cdn_config": None,
+        "non_existent_bucket_details": None,
+        "default_file_info": {},
     }
```

### Comparing `django_backblaze_b2-3.2.1/django_backblaze_b2/storage.py` & `django_backblaze_b2-4.0.0/django_backblaze_b2/storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,230 +18,234 @@
 
 from django_backblaze_b2.b2_file import B2File
 from django_backblaze_b2.cache_account_info import DjangoCacheAccountInfo
 from django_backblaze_b2.options import (
     BackblazeB2StorageOptions,
     DjangoCacheAccountInfoConfig,
     SqliteAccountInfoConfig,
-    getDefaultB2StorageOptions,
+    get_default_b2_storage_options,
 )
 
 logger = getLogger("django-backblaze-b2")
 
 
-class _BaseFileInfoDict(TypedDict):
-    fileId: str
-    fileName: str
-    fileInfo: dict
+class _SdkBaseFileInfoDict(TypedDict):
+    """See https://github.com/Backblaze/b2-sdk-python/blob/2c85182c82ee09b7db7216d70567aafb87f31536/b2sdk/file_version.py"""  # noqa: E501
 
+    fileId: str  # noqa: N815
+    fileName: str  # noqa: N815
+    fileInfo: dict  # noqa: N815
+
+
+class _SdkFileInfoDict(_SdkBaseFileInfoDict, total=False):
+    """See https://github.com/Backblaze/b2-sdk-python/blob/2c85182c82ee09b7db7216d70567aafb87f31536/b2sdk/file_version.py#L143"""  # noqa: E501
 
-class _FileInfoDict(_BaseFileInfoDict, total=False):
     size: int
-    uploadTimestamp: int
-    contentType: str
+    uploadTimestamp: int  # noqa: N815
+    contentType: str  # noqa: N815
 
 
-class B2FileInformationNotAvailableException(Exception):
+class B2FileInformationNotAvailableException(Exception):  # noqa: N818
     ...
 
 
 @deconstructible
 class BackblazeB2Storage(Storage):
     """Storage class which fulfills the Django Storage contract through b2 apis"""
 
     def __init__(self, **kwargs):
-        opts = self._getDjangoSettingsOptions(kwargs.get("opts", {}))
+        opts = self._get_django_settings_options(kwargs.get("opts", {}))
         if "opts" in kwargs:
-            self._validateOptions(kwargs.get("opts"))
+            self._validate_options(kwargs.get("opts"))
         _merge(opts, kwargs.get("opts", {}))
-        logOpts = opts.copy()
-        logOpts.update({"application_key_id": "<redacted>", "application_key": "<redacted>"})
-        logger.debug(f"Initializing {self.__class__.__name__} with options {logOpts}")
-
-        self._bucketName = opts["bucket"]
-        self._defaultFileMetadata = opts["defaultFileInfo"]
-        self._forbidFilePropertyCaching = opts["forbidFilePropertyCaching"]
+        log_opts = opts.copy()
+        log_opts.update({"application_key_id": "<redacted>", "application_key": "<redacted>"})
+        logger.debug(f"Initializing {self.__class__.__name__} with options {log_opts}")
+
+        self._bucket_name = opts["bucket"]
+        self._default_file_metadata = opts["default_file_info"]
+        self._forbid_file_property_caching = opts["forbid_file_property_caching"]
         self._authInfo = dict(
             [(k, v) for k, v in opts.items() if k in ["realm", "application_key_id", "application_key"]]
         )
-        self._allowFileOverwrites = opts["allowFileOverwrites"]
+        self._allow_file_overwrites = opts["allow_file_overwrites"]
 
-        self._getAccountInfo = self._createAccountInfoCallable(opts)
+        self._get_account_info = self._create_account_info_callable(opts)
 
-        logger.info(f"{self.__class__.__name__} instantiated to use bucket {self._bucketName}")
-        if opts["authorizeOnInit"]:
+        logger.info(f"{self.__class__.__name__} instantiated to use bucket {self._bucket_name}")
+        if opts["authorize_on_init"]:
             logger.debug(f"{self.__class__.__name__} authorizing")
-            self.b2Api
-            if opts["validateOnInit"]:
-                self._getOrCreateBucket(opts["nonExistentBucketDetails"])
+            self.b2_api
+            if opts["validate_on_init"]:
+                self._get_or_create_bucket(opts["non_existent_bucket_details"])
 
-    def _getDjangoSettingsOptions(self, kwargOpts: Dict) -> BackblazeB2StorageOptions:
+    def _get_django_settings_options(self, kwarg_opts: Dict) -> BackblazeB2StorageOptions:
         """Setting terminology taken from:
         https://b2-sdk-python.readthedocs.io/en/master/glossary.html#term-application-key-ID
         kwargOpts available for subclasses
         """
         from django.conf import settings
 
         if not hasattr(settings, "BACKBLAZE_CONFIG"):
             raise ImproperlyConfigured("add BACKBLAZE_CONFIG dict to django settings")
         if "application_key_id" not in settings.BACKBLAZE_CONFIG or "application_key" not in settings.BACKBLAZE_CONFIG:
             raise ImproperlyConfigured(
                 "At minimum BACKBLAZE_CONFIG must contain auth 'application_key' and 'application_key_id'"
                 f"\nfound: {settings.BACKBLAZE_CONFIG}"
             )
-        self._validateOptions(settings.BACKBLAZE_CONFIG)
-        opts = getDefaultB2StorageOptions()
+        self._validate_options(settings.BACKBLAZE_CONFIG)
+        opts = get_default_b2_storage_options()
         opts.update(settings.BACKBLAZE_CONFIG)  # type: ignore
         return opts
 
-    def _validateOptions(self, options: Dict) -> None:
-        unrecognizedOptions = [k for k in options.keys() if k not in getDefaultB2StorageOptions().keys()]
-        if unrecognizedOptions:
-            raise ImproperlyConfigured(f"Unrecognized options: {unrecognizedOptions}")
+    def _validate_options(self, options: Dict) -> None:
+        unrecognized_options = [k for k in options.keys() if k not in get_default_b2_storage_options().keys()]
+        if unrecognized_options:
+            raise ImproperlyConfigured(f"Unrecognized options: {unrecognized_options}")
 
-    def _createAccountInfoCallable(self, opts: BackblazeB2StorageOptions) -> Callable[[], AbstractAccountInfo]:
+    def _create_account_info_callable(self, opts: BackblazeB2StorageOptions) -> Callable[[], AbstractAccountInfo]:
         if (
-            not isinstance(opts["accountInfo"], dict)
-            or "type" not in opts["accountInfo"]
-            or opts["accountInfo"]["type"] not in ["memory", "sqlite", "django-cache"]
+            not isinstance(opts["account_info"], dict)
+            or "type" not in opts["account_info"]
+            or opts["account_info"]["type"] not in ["memory", "sqlite", "django-cache"]
         ):
             raise ImproperlyConfigured(
-                (f"accountInfo property must be a dict with type found in options.py, was {opts['accountInfo']}")
+                (f"'account_info' property must be a dict with type found in options.py, was {opts['account_info']}")
             )
-        if opts["accountInfo"]["type"] == "django-cache":
+        if opts["account_info"]["type"] == "django-cache":
             logger.debug(f"{self.__class__.__name__} will use {DjangoCacheAccountInfo.__name__}")
             return lambda: DjangoCacheAccountInfo(
-                cacheName=cast(DjangoCacheAccountInfoConfig, opts["accountInfo"]).get("cache", "django-backblaze-b2")
+                cache_name=cast(DjangoCacheAccountInfoConfig, opts["account_info"]).get("cache", "django-backblaze-b2")
             )
-        elif opts["accountInfo"]["type"] == "memory":
+        elif opts["account_info"]["type"] == "memory":
             logger.debug(f"{self.__class__.__name__} will use {InMemoryAccountInfo.__name__}")
             return lambda: InMemoryAccountInfo()
-        elif opts["accountInfo"]["type"] == "sqlite":
+        elif opts["account_info"]["type"] == "sqlite":
             logger.debug(f"{self.__class__.__name__} will use {SqliteAccountInfo.__name__}")
             return lambda: SqliteAccountInfo(
-                file_name=cast(SqliteAccountInfoConfig, opts["accountInfo"])["databasePath"]
+                file_name=cast(SqliteAccountInfoConfig, opts["account_info"])["database_path"]
             )
         raise ImproperlyConfigured()
 
     @property
-    def b2Api(self) -> B2Api:
-        if not hasattr(self, "_b2Api"):
-            self._accountInfo = self._getAccountInfo()
-            self._b2Api = B2Api(account_info=self._accountInfo, cache=AuthInfoCache(self._accountInfo))
-            self._b2Api.authorize_account(**self._authInfo)
-        return self._b2Api
+    def b2_api(self) -> B2Api:
+        if not hasattr(self, "_b2_api"):
+            self._account_info = self._get_account_info()
+            self._b2_api = B2Api(account_info=self._account_info, cache=AuthInfoCache(self._account_info))
+            self._b2_api.authorize_account(**self._authInfo)
+        return self._b2_api
 
     @property
     def bucket(self) -> Bucket:
         if not hasattr(self, "_bucket"):
-            self._getOrCreateBucket()
+            self._get_or_create_bucket()
         return self._bucket
 
-    def _getOrCreateBucket(self, newBucketDetails=None) -> None:
+    def _get_or_create_bucket(self, new_bucket_details=None) -> None:
         try:
-            self._bucket = self.b2Api.get_bucket_by_name(self._bucketName)
+            self._bucket = self.b2_api.get_bucket_by_name(self._bucket_name)
         except NonExistentBucket as e:
-            if newBucketDetails is not None:
-                logger.debug(f"Bucket {self._bucketName} not found. Creating with details: {newBucketDetails}")
-                if "bucket_type" not in newBucketDetails:
-                    newBucketDetails["bucket_type"] = "allPrivate"
-                self._bucket = self.b2Api.create_bucket(name=self._bucketName, **newBucketDetails)
+            if new_bucket_details is not None:
+                logger.debug(f"Bucket {self._bucket_name} not found. Creating with details: {new_bucket_details}")
+                if "bucket_type" not in new_bucket_details:
+                    new_bucket_details["bucket_type"] = "allPrivate"
+                self._bucket = self.b2_api.create_bucket(name=self._bucket_name, **new_bucket_details)
             else:
                 raise e
         logger.debug(f"Connected to bucket {self._bucket.as_dict()}")
 
-    def _refreshBucket(self) -> Bucket:
+    def _refresh_bucket(self) -> Bucket:
         if self._bucket:
             return self._bucket.get_fresh_state()
         return self.bucket
 
     def _open(self, name: str, mode: str) -> File:
         return B2File(
             name=name,
             bucket=self.bucket,
-            fileMetadata=self._defaultFileMetadata,
+            file_metadata=self._default_file_metadata,
             mode=mode,
-            sizeProvider=self.size,
+            size_provider=self.size,
         )
 
     def _save(self, name: str, content: IO[Any]) -> str:
         """
         Save and retrieve the filename.
         If the file exists it will make another version of that file.
         """
         return B2File(
             name=name,
             bucket=self.bucket,
-            fileMetadata=self._defaultFileMetadata,
+            file_metadata=self._default_file_metadata,
             mode="w",
-            sizeProvider=self.size,
-        ).saveAndRetrieveFile(content)
+            size_provider=self.size,
+        ).save_and_retrieve_file(content)
 
     def path(self, name: str) -> str:
         return name
 
     def delete(self, name: str) -> None:
-        fileInfo = self._fileInfo(name)
-        if fileInfo:
-            logger.debug(f"Deleting file {name} id=({fileInfo['fileId']})")
-            self.b2Api.delete_file_version(file_id=fileInfo["fileId"], file_name=name)
+        file_info = self._file_info(name)
+        if file_info:
+            logger.debug(f"Deleting file {name} id=({file_info['fileId']})")
+            self.b2_api.delete_file_version(file_id=file_info["fileId"], file_name=name)
             if self._cache:
-                self._cache.delete(self._fileCacheKey(name))
+                self._cache.delete(self._file_cache_key(name))
         else:
             logger.debug("Not found")
 
-    def _fileInfo(self, name: str) -> Optional[_FileInfoDict]:
+    def _file_info(self, name: str) -> Optional[_SdkFileInfoDict]:
         try:
             if self._cache:
-                cacheKey = self._fileCacheKey(name)
-                timeoutInSeconds = 60
+                cache_key = self._file_cache_key(name)
+                timeout_in_seconds = 60
 
-                def loadInfo():
+                def load_info():
                     logger.debug(f"file info cache miss for {name}")
                     return self.bucket.get_file_info_by_name(name).as_dict()
 
-                return self._cache.get_or_set(key=cacheKey, default=loadInfo, timeout=timeoutInSeconds)
+                return self._cache.get_or_set(key=cache_key, default=load_info, timeout=timeout_in_seconds)
             return self.bucket.get_file_info_by_name(name).as_dict()
         except FileOrBucketNotFound:
             return None
 
-    def _fileCacheKey(self, name: str) -> str:
+    def _file_cache_key(self, name: str) -> str:
         return hash(f"{self.bucket.name}__{name}".encode()).hexdigest()
 
     @property
     def _cache(self) -> Optional[BaseCache]:
         if (
-            not self._forbidFilePropertyCaching
-            and self.b2Api  # force init
-            and self._accountInfo
-            and isinstance(self._accountInfo, DjangoCacheAccountInfo)
+            not self._forbid_file_property_caching
+            and self.b2_api  # force init
+            and self._account_info
+            and isinstance(self._account_info, DjangoCacheAccountInfo)
         ):
-            return self._accountInfo.cache
+            return self._account_info.cache
         return None
 
     def exists(self, name: str) -> bool:
-        return bool(self._fileInfo(name))
+        return bool(self._file_info(name))
 
     def size(self, name: str) -> int:
-        fileInfo = self._fileInfo(name)
-        return fileInfo.get("size", 0) if fileInfo else 0
+        file_info = self._file_info(name)
+        return file_info.get("size", 0) if file_info else 0
 
     def url(self, name: Optional[str]) -> str:
         if not name:
             raise Exception("Name must be defined")
-        return self._getFileUrl(name)
+        return self._get_file_url(name)
 
-    def _getFileUrl(self, name: str) -> str:
-        return self.getBackblazeUrl(name)
+    def _get_file_url(self, name: str) -> str:
+        return self.get_backblaze_url(name)
 
-    def getBackblazeUrl(self, filename: str) -> str:
-        return self.b2Api.get_download_url_for_file_name(bucket_name=self._bucketName, file_name=filename)
+    def get_backblaze_url(self, filename: str) -> str:
+        return self.b2_api.get_download_url_for_file_name(bucket_name=self._bucket_name, file_name=filename)
 
     def get_available_name(self, name: str, max_length: Optional[int] = None) -> str:
-        if self._allowFileOverwrites:
+        if self._allow_file_overwrites:
             return name
         return super().get_available_name(name, max_length)
 
     def listdir(self, path: str) -> Tuple[List[str], List[str]]:
         """
         List the contents of the specified path. Return a 2-tuple of lists:
         the first item being directories, the second item being files.
@@ -260,18 +264,18 @@
         Return the creation time (as a datetime) of the file specified by name.
         The datetime will be timezone-aware if USE_TZ=True.
         """
         from datetime import timezone
 
         from django.conf import settings
 
-        fileInfo = self._fileInfo(name)
+        file_info = self._file_info(name)
         try:
-            if fileInfo and float(fileInfo.get("uploadTimestamp", 0)) > 0:
-                timestamp = float(fileInfo["uploadTimestamp"]) / 1000.0
+            if file_info and float(file_info.get("uploadTimestamp", 0)) > 0:
+                timestamp = float(file_info["uploadTimestamp"]) / 1000.0
                 if settings.USE_TZ:
                     # Safe to use .replace() because UTC doesn't have DST
                     return datetime.utcfromtimestamp(timestamp).replace(tzinfo=timezone.utc)
                 return datetime.fromtimestamp(timestamp)
         except ValueError as e:
             raise B2FileInformationNotAvailableException(f"'uploadTimestamp' from API not valid for {name}: {e}")
         raise B2FileInformationNotAvailableException(f"'uploadTimestamp' not available for {name}")
@@ -288,16 +292,16 @@
     """merges b into a
     https://stackoverflow.com/a/7205107/11076240
     """
     if path is None:
         path = []
     for key in source:
         if key in target:
-            printablePath = ".".join(path + [str(key)])
+            printable_path = ".".join(path + [str(key)])
             if isinstance(target[key], dict) and isinstance(source[key], dict):
                 _merge(target[key], source[key], path + [str(key)])
             elif target[key] != source[key]:
-                logger.debug(f"Overriding setting {printablePath} with value {source[key]}")
+                logger.debug(f"Overriding setting {printable_path} with value {source[key]}")
                 target[key] = source[key]
         else:
             target[key] = source[key]
     return target
```

### Comparing `django_backblaze_b2-3.2.1/django_backblaze_b2/views.py` & `django_backblaze_b2-4.0.0/django_backblaze_b2/views.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,47 +5,49 @@
 from b2sdk.v1.exception import FileNotPresent
 from django.http import FileResponse, HttpRequest, HttpResponse, HttpResponseNotFound
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 
 from django_backblaze_b2 import storage, storages
 
-from ._decorators import requiresLogin
+from ._decorators import _requires_login
 
 logger = logging.getLogger("django-backblaze-b2")
 
 
 @xframe_options_sameorigin
-def downloadPublicFile(request: HttpRequest, filename: str) -> Union[HttpResponse, FileResponse]:
+def download_public_file(request: HttpRequest, filename: str) -> Union[HttpResponse, FileResponse]:
     """Serves the specified 'filename' without validating any authentication"""
-    return _downloadFileFromStorage(storages.PublicStorage(), filename)
+    return _download_file_from_storage(storages.PublicStorage(), filename)
 
 
-@requiresLogin()
+@_requires_login()
 @xframe_options_sameorigin
-def downloadLoggedInFile(request: HttpRequest, filename: str) -> Union[HttpResponse, FileResponse]:
+def download_logged_in_file(request: HttpRequest, filename: str) -> Union[HttpResponse, FileResponse]:
     """Serves the specified 'filename' validating the user is logged in"""
-    return _downloadFileFromStorage(storages.LoggedInStorage(), filename)
+    return _download_file_from_storage(storages.LoggedInStorage(), filename)
 
 
-@requiresLogin(requiresStaff=True)
+@_requires_login(requires_staff=True)
 @xframe_options_sameorigin
-def downloadStaffFile(request: HttpRequest, filename: str) -> Union[HttpResponse, FileResponse]:
+def download_staff_file(request: HttpRequest, filename: str) -> Union[HttpResponse, FileResponse]:
     """Serves the specified 'filename' validating the user is logged in and a staff user"""
-    return _downloadFileFromStorage(storages.StaffStorage(), filename)
+    return _download_file_from_storage(storages.StaffStorage(), filename)
 
 
-def _downloadFileFromStorage(storage: storage.BackblazeB2Storage, filename: str) -> Union[HttpResponse, FileResponse]:
+def _download_file_from_storage(
+    storage: storage.BackblazeB2Storage, filename: str
+) -> Union[HttpResponse, FileResponse]:
     if logger.isEnabledFor(logging.DEBUG):
         try:
-            logger.debug(f"Downloding file from {storage.getBackblazeUrl(filename)}")
+            logger.debug(f"Downloding file from {storage.get_backblaze_url(filename)}")
         except Exception:
             logger.exception(f"Debug log failed. Could not retrive b2 file url for {filename}")
 
     try:
         if storage.exists(filename):
-            contentType, _encoding = mimetypes.guess_type(filename)
-            return FileResponse(storage.open(filename, "r"), content_type=contentType)
+            content_type, _encoding = mimetypes.guess_type(filename)
+            return FileResponse(storage.open(filename, "r"), content_type=content_type)
     except (FileNotFoundError, FileNotPresent):
         logging.exception("Opening backblaze file failed")
 
     return HttpResponseNotFound(_("Could not find file") + f": {filename}")
```

### Comparing `django_backblaze_b2-3.2.1/pyproject.toml` & `django_backblaze_b2-4.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "django-backblaze-b2"
-version = "3.2.1"
+version = "4.0.0"
 description = "A Django app to use backblaze b2 as storage."
 authors = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 maintainers = ["Etienne H <django_backblaze_b2@internet-e-mail.com>"]
 license = "BSD-2-Clause"
 readme = "README.md"
 homepage = "https://github.com/ehossack/django-backblaze-b2/"
 repository = "https://github.com/ehossack/django-backblaze-b2/"
@@ -59,10 +59,13 @@
 flake8 = "^5.0"
 pytest-cov = "^4.0"
 pytest-django = "^4.5"
 pytest-pythonpath = "^0.7"
 docutils = "^0.19"
 toml = "^0.10.2"
 
+[tool.poetry.group.dev.dependencies]
+pep8-naming = "^0.13.3"
+
 [build-system]
 requires = ["poetry>=1.2.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `django_backblaze_b2-3.2.1/PKG-INFO` & `django_backblaze_b2-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-backblaze-b2
-Version: 3.2.1
+Version: 4.0.0
 Summary: A Django app to use backblaze b2 as storage.
 Home-page: https://github.com/ehossack/django-backblaze-b2/
 License: BSD-2-Clause
 Keywords: django,storage,backblaze,b2,cloud
 Author: Etienne H
 Author-email: django_backblaze_b2@internet-e-mail.com
 Maintainer: Etienne H
@@ -44,14 +44,18 @@
 [![python version](https://img.shields.io/pypi/pyversions/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)
 [![django version](https://img.shields.io/pypi/djversions/django-backblaze-b2)](https://pypi.org/project/django-backblaze-b2/)
 
 A storage backend for Django that uses [Backblaze's B2 APIs](https://www.backblaze.com/b2/cloud-storage.html).
 
 Implementation wraps [Official Python SDK](https://github.com/Backblaze/b2-sdk-python)
 
+## Changelog / Releases
+
+See [https://github.com/ehossack/django-backblaze-b2/releases](https://github.com/ehossack/django-backblaze-b2/releases)
+
 ## How to use
 
 1. Install from this repo, or install from PyPi: `pip install django-backblaze-b2`
 As tested, requires python 3.7 or greater but solely due to type annotations. PRs welcome :)
 1. Configure your django `settings`. A minimalistic config would be:
 ```python
 CACHES = {
@@ -72,15 +76,15 @@
 
 Theoretically you may now refer to the base storage class as a storage class (see the sample app for some usage: you can run with `make run-sample-proj` although you might want to configure the `SECONDS_TO_RUN_APP` variable in `settings.env` to be 0 for unlimited to try things out)
 e.g.
 ```python
 from django_backblaze_b2 import BackblazeB2Storage
 
 class MyModel(models.Model):
-    fileField = models.FileField(
+    file_field = models.FileField(
         upload_to="uploads",
         storage=BackblazeB2Storage
     )
 ```
 
 ### Public/Logged-In/Private storage
 
@@ -92,16 +96,16 @@
         path('', include('django_backblaze_b2.urls')),
     ]
 ```
 
 ### Caching
 
 To retrieve file metadata ("file info" as the b2 sdk names it), this library has to authorize and request data from b2 servers, even for just resolving the url for a file. Because these are network calls, and relatively expensive in comparison to a file-based storage, and because data is unlikely to change frequently, there is some caching done by this library.  
-By default, the account information (`accountInfo`) configuration of the settings uses a cache by the name of `django-backblaze-b2` which you must have in your `CACHES` section of your `settings.py`. This is to leverage django's thread-safe cache implementations, and if you are using a database cache table or memcached, (rather than LocMemCache) your cache can be shared by the multiple django processes that typically serve requests.  
-It is not recommended configure `accountInfo` with the `default` django cache, as the `clear()` method may be called during the backblaze lifecycle.  
+By default, the account information (`account_info`) configuration of the settings uses a cache by the name of `django-backblaze-b2` which you must have in your `CACHES` section of your `settings.py`. This is to leverage django's thread-safe cache implementations, and if you are using a database cache table or memcached, (rather than LocMemCache) your cache can be shared by the multiple django processes that typically serve requests.  
+It is not recommended configure `account_info` with the `default` django cache, as the `clear()` method may be called during the backblaze lifecycle.  
 If you do not wish to use a django cache, you can use a sqlite database on disk for caching, or use a non-thread-safe in-memory implementation. This is only recommended for single-threaded deployments (remember in most deployments a new thread serves each request).  
 For further discussion on this see https://github.com/ehossack/django-backblaze-b2/issues/16
 
 ### Configurations
 
 You may want to use your own bucket name, or set further configuration such as lazy authorization/validation, or specifying file metadata.  
 Refer to [the options](./django_backblaze_b2/options.py) for all options.  
@@ -193,13 +197,13 @@
 * You can run tests with `make test`
 * You can view test coverage with `make test-coverage`, then see in the terminal, 
 open `test/htmlcov/index.html`
 or use `cov.xml` in your favourite IDE like VSCode
 
 ### Releasing
 
-1. `make publish-to-pypi`
+1. `make release`
 
 ### Cleanup
 
 1. `make cleanup`
```

