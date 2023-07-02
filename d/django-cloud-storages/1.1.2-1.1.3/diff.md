# Comparing `tmp/django_cloud_storages-1.1.2.tar.gz` & `tmp/django_cloud_storages-1.1.3.tar.gz`

## Comparing `django_cloud_storages-1.1.2.tar` & `django_cloud_storages-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/manage.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/requirements.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/setup.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/Makefile
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/conf.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/make.bat
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/requirements.txt
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/backends/appwrite.rst
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/docs/backends/dropbox.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/__init__.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/settings.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/test_appwrite.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/test_dropbox.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/tests/test_folder/test_file.txt
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/LICENSE
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/README.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/manage.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/requirements.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/setup.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/cloud_storages/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0    14076 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/docs/Makefile
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/docs/conf.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/docs/index.rst
+-rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/docs/make.bat
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/docs/requirements.txt
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/docs/backends/appwrite.rst
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/docs/backends/dropbox.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/tests/settings.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/tests/test_appwrite.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/tests/test_dropbox.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/tests/test_folder/test_file.txt
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/README.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.3/PKG-INFO
```

### Comparing `django_cloud_storages-1.1.2/.readthedocs.yaml` & `django_cloud_storages-1.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/manage.py` & `django_cloud_storages-1.1.3/manage.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/requirements.txt` & `django_cloud_storages-1.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/cloud_storages/utils.py` & `django_cloud_storages-1.1.3/cloud_storages/utils.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/cloud_storages/backends/appwrite.py` & `django_cloud_storages-1.1.3/cloud_storages/backends/appwrite.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/cloud_storages/backends/dropbox.py` & `django_cloud_storages-1.1.3/cloud_storages/backends/dropbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
-
+import os
 from django.core.files.storage import Storage
 from django.core.files import File
 from django.utils.deconstruct import deconstructible
-from django.utils.deconstruct import deconstructible
+from django.utils._os import safe_join
 
 import dropbox
 from dropbox import sharing as dbx_sharing
 from dropbox.exceptions import ApiError
 from dropbox.files import *
 
 from cloud_storages.utils import *
@@ -29,14 +29,22 @@
         self.DROPBOX_ROOT_PATH = setting('DROPBOX_ROOT_PATH')
         self.MEDIA_URL = setting('MEDIA_URL')
         self.timeout = setting('DROPBOX_TIMEOUT', _DEFAULT_TIMEOUT)
         self.write_mode = setting('DROPBOX_WRITE_MODE', _DEFAULT_MODE)
         self.dbx = dropbox.Dropbox(app_key=self.DROPBOX_APP_KEY, app_secret=self.DROPBOX_APP_SECRET, oauth2_refresh_token=self.DROPBOX_OAUTH2_REFRESH_TOKEN)
         self.dbx.users_get_current_account()
 
+    def _full_path(self, name):
+        if name == '/':
+            name = ''
+        if name[0] in ["/", "\\"]:
+            name = name[1:]
+        joined_path = os.path.join(self.DROPBOX_ROOT_PATH, name).replace("\\", "/")
+        return joined_path
+    
     def open(self, name, mode="rb"):
         """Retrieve the specified file from storage."""
         return self._open(name, mode)
     def _open(self, name, mode='rb'):
         full_file_url = self.url(name)
         response = requests.get(full_file_url)
         if (response.status_code == 200):
@@ -56,19 +64,20 @@
         if not hasattr(content, "chunks"):
             content = File(content, name)
         path = self.get_available_name(name, content, max_length=max_length)
         if path[1] is None:
             self._save(path[0], content)
         return path[0]
     def _save(self, name, content):
+        full_name = self._full_path(name)
         content.open()
         if content.size <= self.CHUNK_SIZE:
-            self.dbx.files_upload(content.read(), name, mode=WriteMode(self.write_mode))
+            self.dbx.files_upload(content.read(), full_name, mode=WriteMode(self.write_mode))
         else:
-            self._chunked_upload(content, name)
+            self._chunked_upload(content, full_name)
         content.close()
         return name
 
     def get_available_name(self, name, content, max_length=None):
         """
         Return a filename that's free on the target storage system and
         available for new content to be written to.
@@ -105,40 +114,43 @@
 
     def get_valid_name(self, name):
         """
         Return a filename, based on the provided filename, that's suitable for
         use in the target storage system.
         """
         name = str(name).replace("\\", "/")
-        path = f"{self.DROPBOX_ROOT_PATH}/{name}"
-        return path
+        # name = self._full_path(name)
+        return name
     
     def get_alternative_name(self, file_root, file_ext=None, index=0):
         """
         Return an alternative filename if one exists to the filename.
         """
         res = file_root.rsplit('.', 1)  # Split on last occurrence of delimiter
         file_name = f"{res[0]}({index})"
         file_ext = res[1]
         updated_name =  f"{file_name}.{file_ext}"
+        # updated_name = self._full_path(updated_name)
         return updated_name
 
     def delete(self, name):
         """
         Delete the specified file from the storage system.
         """
-        self.dbx.files_delete_v2(name)
+        full_name = self._full_path(name)
+        self.dbx.files_delete_v2(full_name)
 
     def exists(self, name):
         """
         Return True if a file referenced by the given name already exists in the
         storage system, or False if the name is available for a new file.
         """
+        full_name = self._full_path(name)
         try:
-            return bool(self.dbx.files_get_metadata(name))
+            return bool(self.dbx.files_get_metadata(full_name))
         except ApiError:
             return False
     
     def listdir(self, path):
         """
         List the contents of the specified path. Return a 2-tuple of lists:
         the first item being directories, the second item being files.
@@ -152,62 +164,65 @@
                 files.append(entry.name)
         return directories, files
     
     def size(self, name):
         """
         Return the total size, in bytes, of the file specified by name.
         """
-        metadata = self.dbx.files_get_metadata(name)
+        full_name = self._full_path(name)
+        metadata = self.dbx.files_get_metadata(full_name)
         return metadata.size
 
     def url(self, name, permanent_link=DROPBOX_PERMANENT_LINK):
         """
         Return an absolute URL where the file's contents can be accessed directly by a web browser.
         """
+        full_name = self._full_path(name)
         try:
             if not permanent_link:
-                media = self.dbx.files_get_temporary_link(name)
+                media = self.dbx.files_get_temporary_link(full_name)
                 file_url = media.link
             else:
                 dbx_share_settings = dbx_sharing.SharedLinkSettings(allow_download=True)
-                media = self.dbx.sharing_create_shared_link_with_settings(name, settings=dbx_share_settings)
+                media = self.dbx.sharing_create_shared_link_with_settings(full_name, settings=dbx_share_settings)
                 file_url = str(media.url)[:-1]+"1"
             return file_url
         except ApiError as e:
             raise e
 
     def get_accessed_time(self, name):
         """
         Return the last accessed time (as a datetime) of the file specified by name.
         The datetime will be timezone-aware if USE_TZ=True.
         """
-        last_accessed = self.dbx.files_get_metadata(name).client_modified
+        full_name = self._full_path(name)
+        last_accessed = self.dbx.files_get_metadata(full_name).client_modified
         return last_accessed
 
     def get_created_time(self, name):
         """
         Return the creation time (as a datetime) of the file specified by name.
         The datetime will be timezone-aware if USE_TZ=True.
         """
-        created_at = self.dbx.files_get_metadata(name).client_modified
+        full_name = self._full_path(name)
+        created_at = self.dbx.files_get_metadata(full_name).client_modified
         return created_at
 
     def get_modified_time(self, name):
         """
         Return the last modified time (as a datetime) of the file specified by
         name. The datetime will be timezone-aware if USE_TZ=True.
         """
-        last_modified = self.dbx.files_get_metadata(name).server_modified
+        full_name = self._full_path(name)
+        last_modified = self.dbx.files_get_metadata(full_name).server_modified
         return last_modified
                 
     def _chunked_upload(self, content, dest_path):
         upload_session = self.dbx.files_upload_session_start(content.read(self.CHUNK_SIZE))
         cursor = UploadSessionCursor(session_id=upload_session.session_id, offset=content.tell())
         commit = CommitInfo(path=dest_path, mode=WriteMode(self.write_mode))
         while content.tell() < content.size:
             if (content.size - content.tell()) <= self.CHUNK_SIZE:
                 self.dbx.files_upload_session_finish(content.read(self.CHUNK_SIZE), cursor, commit)
             else:
                 self.dbx.files_upload_session_append_v2(content.read(self.CHUNK_SIZE), cursor)
-                cursor.offset = content.tell()
-        
-
+                cursor.offset = content.tell()
```

### Comparing `django_cloud_storages-1.1.2/docs/Makefile` & `django_cloud_storages-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/docs/conf.py` & `django_cloud_storages-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/docs/index.rst` & `django_cloud_storages-1.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/docs/make.bat` & `django_cloud_storages-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/docs/backends/appwrite.rst` & `django_cloud_storages-1.1.3/docs/backends/appwrite.rst`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/docs/backends/dropbox.rst` & `django_cloud_storages-1.1.3/docs/backends/dropbox.rst`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/tests/settings.py` & `django_cloud_storages-1.1.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/tests/test_appwrite.py` & `django_cloud_storages-1.1.3/tests/test_appwrite.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/tests/test_dropbox.py` & `django_cloud_storages-1.1.3/tests/test_dropbox.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/.gitignore` & `django_cloud_storages-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/LICENSE` & `django_cloud_storages-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.2/README.md` & `django_cloud_storages-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Welcome to django-cloud-storages's
+# Welcome to django-cloud-storages
 
 django-cloud-storages is a package developed for django to work with cloud storages to store/upload media files.
 
 This package extends the [django Storage class](https://docs.djangoproject.com/en/4.2/ref/files/storage/#django.core.files.storage.Storage) to provide file storage in cloud.
 
 At the moment this package support the following cloud storage services -
```

### Comparing `django_cloud_storages-1.1.2/pyproject.toml` & `django_cloud_storages-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "django", "requests", "dropbox", "appwrite"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-cloud-storages"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="Samiddha Chakrabarti", email="samiddha99@protonmail.com" },
 ]
 description = "Cloud file storages for django."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `django_cloud_storages-1.1.2/PKG-INFO` & `django_cloud_storages-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-cloud-storages
-Version: 1.1.2
+Version: 1.1.3
 Summary: Cloud file storages for django.
 Project-URL: Homepage, https://github.com/Samiddha99/django-cloud-storages
 Project-URL: Documentation, https://django-cloud-storages.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Samiddha99/django-cloud-storages/issues
 Author-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
-# Welcome to django-cloud-storages's
+# Welcome to django-cloud-storages
 
 django-cloud-storages is a package developed for django to work with cloud storages to store/upload media files.
 
 This package extends the [django Storage class](https://docs.djangoproject.com/en/4.2/ref/files/storage/#django.core.files.storage.Storage) to provide file storage in cloud.
 
 At the moment this package support the following cloud storage services -
```

