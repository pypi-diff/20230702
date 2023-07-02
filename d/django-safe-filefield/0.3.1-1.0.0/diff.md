# Comparing `tmp/django-safe-filefield-0.3.1.tar.gz` & `tmp/django-safe-filefield-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-safe-filefield-0.3.1.tar", last modified: Sun Oct  8 23:30:18 2017, max compression
+gzip compressed data, was "django-safe-filefield-1.0.0.tar", last modified: Sun Jul  2 15:58:02 2023, max compression
```

## Comparing `django-safe-filefield-0.3.1.tar` & `django-safe-filefield-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 vbakin     (501) staff       (20)        0 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/
-drwxr-xr-x   0 vbakin     (501) staff       (20)        0 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/django_safe_filefield.egg-info/
--rw-r--r--   0 vbakin     (501) staff       (20)        1 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/django_safe_filefield.egg-info/dependency_links.txt
--rw-r--r--   0 vbakin     (501) staff       (20)     4681 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/django_safe_filefield.egg-info/PKG-INFO
--rw-r--r--   0 vbakin     (501) staff       (20)       26 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/django_safe_filefield.egg-info/requires.txt
--rw-r--r--   0 vbakin     (501) staff       (20)      442 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/django_safe_filefield.egg-info/SOURCES.txt
--rw-r--r--   0 vbakin     (501) staff       (20)       15 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/django_safe_filefield.egg-info/top_level.txt
--rw-r--r--   0 vbakin     (501) staff       (20)     4681 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/PKG-INFO
--rw-r--r--   0 vbakin     (501) staff       (20)     2862 2017-10-08 23:29:55.000000 django-safe-filefield-0.3.1/README.rst
-drwxr-xr-x   0 vbakin     (501) staff       (20)        0 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/safe_filefield/
--rw-r--r--   0 vbakin     (501) staff       (20)        0 2017-10-01 11:31:56.000000 django-safe-filefield-0.3.1/safe_filefield/__init__.py
--rw-r--r--   0 vbakin     (501) staff       (20)     1084 2017-10-08 23:27:26.000000 django-safe-filefield-0.3.1/safe_filefield/clamav.py
--rw-r--r--   0 vbakin     (501) staff       (20)       74 2017-10-08 23:27:26.000000 django-safe-filefield-0.3.1/safe_filefield/default_settings.py
--rw-r--r--   0 vbakin     (501) staff       (20)      904 2017-10-08 23:27:26.000000 django-safe-filefield-0.3.1/safe_filefield/forms.py
--rw-r--r--   0 vbakin     (501) staff       (20)     1165 2017-10-08 23:27:26.000000 django-safe-filefield-0.3.1/safe_filefield/models.py
--rw-r--r--   0 vbakin     (501) staff       (20)      132 2017-10-01 12:27:45.000000 django-safe-filefield-0.3.1/safe_filefield/utils.py
--rw-r--r--   0 vbakin     (501) staff       (20)     3044 2017-10-08 23:27:26.000000 django-safe-filefield-0.3.1/safe_filefield/validators.py
--rw-r--r--   0 vbakin     (501) staff       (20)      134 2017-10-08 23:30:18.000000 django-safe-filefield-0.3.1/setup.cfg
--rw-r--r--   0 vbakin     (501) staff       (20)     1268 2017-10-08 23:30:13.000000 django-safe-filefield-0.3.1/setup.py
+drwxr-xr-x   0 vbakin     (501) staff       (20)        0 2023-07-02 15:58:02.034254 django-safe-filefield-1.0.0/
+-rw-r--r--   0 vbakin     (501) staff       (20)     1071 2023-07-02 14:13:00.000000 django-safe-filefield-1.0.0/LICENSE
+-rw-r--r--   0 vbakin     (501) staff       (20)     4554 2023-07-02 15:58:02.034316 django-safe-filefield-1.0.0/PKG-INFO
+-rw-r--r--   0 vbakin     (501) staff       (20)     3230 2023-07-02 15:57:49.000000 django-safe-filefield-1.0.0/README.rst
+drwxr-xr-x   0 vbakin     (501) staff       (20)        0 2023-07-02 15:58:02.032260 django-safe-filefield-1.0.0/django_safe_filefield.egg-info/
+-rw-r--r--   0 vbakin     (501) staff       (20)     4554 2023-07-02 15:58:02.000000 django-safe-filefield-1.0.0/django_safe_filefield.egg-info/PKG-INFO
+-rw-r--r--   0 vbakin     (501) staff       (20)      450 2023-07-02 15:58:02.000000 django-safe-filefield-1.0.0/django_safe_filefield.egg-info/SOURCES.txt
+-rw-r--r--   0 vbakin     (501) staff       (20)        1 2023-07-02 15:58:02.000000 django-safe-filefield-1.0.0/django_safe_filefield.egg-info/dependency_links.txt
+-rw-r--r--   0 vbakin     (501) staff       (20)       26 2023-07-02 15:58:02.000000 django-safe-filefield-1.0.0/django_safe_filefield.egg-info/requires.txt
+-rw-r--r--   0 vbakin     (501) staff       (20)       15 2023-07-02 15:58:02.000000 django-safe-filefield-1.0.0/django_safe_filefield.egg-info/top_level.txt
+drwxr-xr-x   0 vbakin     (501) staff       (20)        0 2023-07-02 15:58:02.033991 django-safe-filefield-1.0.0/safe_filefield/
+-rw-r--r--   0 vbakin     (501) staff       (20)        0 2023-07-02 14:13:00.000000 django-safe-filefield-1.0.0/safe_filefield/__init__.py
+-rw-r--r--   0 vbakin     (501) staff       (20)     1084 2023-07-02 14:13:00.000000 django-safe-filefield-1.0.0/safe_filefield/clamav.py
+-rw-r--r--   0 vbakin     (501) staff       (20)       74 2023-07-02 14:13:00.000000 django-safe-filefield-1.0.0/safe_filefield/default_settings.py
+-rw-r--r--   0 vbakin     (501) staff       (20)      904 2023-07-02 14:13:00.000000 django-safe-filefield-1.0.0/safe_filefield/forms.py
+-rw-r--r--   0 vbakin     (501) staff       (20)     1165 2023-07-02 14:13:00.000000 django-safe-filefield-1.0.0/safe_filefield/models.py
+-rw-r--r--   0 vbakin     (501) staff       (20)      132 2023-07-02 14:13:00.000000 django-safe-filefield-1.0.0/safe_filefield/utils.py
+-rw-r--r--   0 vbakin     (501) staff       (20)     3666 2023-07-02 15:43:45.000000 django-safe-filefield-1.0.0/safe_filefield/validators.py
+-rw-r--r--   0 vbakin     (501) staff       (20)      134 2023-07-02 15:58:02.034495 django-safe-filefield-1.0.0/setup.cfg
+-rw-r--r--   0 vbakin     (501) staff       (20)     1650 2023-07-02 15:57:20.000000 django-safe-filefield-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-safe-filefield-0.3.1/README.rst` & `django-safe-filefield-1.0.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 django-safe-filefield
 =====================
-.. image:: https://travis-ci.org/mixkorshun/django-safe-filefield.svg?branch=master
-   :alt: build status
-   :target: https://travis-ci.org/mixkorshun/django-safe-filefield
-.. image:: https://codecov.io/gh/mixkorshun/django-safe-filefield/branch/master/graph/badge.svg
-   :alt: code coverage
-   :target: https://codecov.io/gh/mixkorshun/django-safe-filefield
+.. image:: https://github.com/mixkorshun/django-safe-filefield/actions/workflows/flake8.yml/badge.svg?branch=master
+   :alt: flake8
+   :target: https://github.com/mixkorshun/django-safe-filefield
+.. image:: https://github.com/mixkorshun/django-safe-filefield/actions/workflows/pytest.yml/badge.svg?branch=master
+   :alt: pytest
+   :target: https://github.com/mixkorshun/django-safe-filefield
 .. image:: https://badge.fury.io/py/django-safe-filefield.svg
    :alt: pypi
    :target: https://pypi.python.org/pypi/django-safe-filefield
 .. image:: https://img.shields.io/badge/code%20style-pep8-orange.svg
    :alt: pep8
    :target: https://www.python.org/dev/peps/pep-0008/
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
@@ -17,15 +17,15 @@
    :target: https://opensource.org/licenses/MIT
 
 Secure file field, which allows you to restrict uploaded file extensions.
 It may be useful for user-uploaded files (attachments).
 
 This package adds model and forms field. What this fields does:
 
- * restricts allowed file extensions (for example: only *.pdf files)
+ * restricts allowed file extensions (for example: only \*.pdf files)
  * checks file extensions is correct for sent content-type
  * checks sent content type is correct for file content (detects by `libmagic`)
  * checks uploaded file with anti-virus software
 
 Installation
 ------------
 
@@ -36,20 +36,20 @@
    pip install django-safe-filefield
 
 
 Add the following settings:
 
 .. code-block:: python
 
-   INSTALLED_APPS += (
+   INSTALLED_APPS += [
        'safe_filefield',
-   )
+   ]
 
 
-**django-safe-filefield** require `libmagic` to be installed.
+**django-safe-filefield** requires `libmagic` to be installed.
 
 Usage
 -----
 
 Simply add field to your model:
 
 .. code-block:: python
@@ -58,33 +58,46 @@
 
    class MyModel(models.Model):
 
        attachment = SafeFileField(
            allowed_extensions=('xls', 'xlsx', 'csv')
        )
 
-Or to directly to your form:
+Or directly to your form:
 
 .. code-block:: python
 
    from safe_filefield.forms import SafeFileField
 
    class MyForm(forms.Form):
 
        attachment = SafeFileField(
            allowed_extensions=('xls', 'xlsx', 'csv')
        )
 
+Content type checking
++++++++++++++++++++++
+
+To check actual file content type, use `check_content_type` argument. This
+will prevent attacker from uploading malicious file just by changing its
+extension.
+
+.. code-block:: python
+
+   class MyForm(forms.Form):
+       attachment = SafeFileField(
+           check_content_type=True
+       )
 
 ClamAV support
---------------
+++++++++++++++
 
 .. note:: To use this functionality you should have `clamd` daemon.
 
-This package have ability to check uploaded file with ClamAV antivirus.
+This package has ability to check uploaded file with ClamAV antivirus.
 
 To use anti-virus protection simply enable it in your form or model definition:
 
 .. code-block:: python
 
    from safe_filefield.forms import SafeFileField
 
@@ -96,15 +109,15 @@
 
 You can configure some ClamAV settings:
 
 .. code-block:: python
 
    CLAMAV_SOCKET = 'unix://tmp/clamav.sock'  # or tcp://127.0.0.1:3310
 
-   CLAMAV_TIMEOUT = 30  # 30 seconds timeout, by default None which means infinite
+   CLAMAV_TIMEOUT = 30  # 30 seconds timeout, None by default which means infinite
 
 
 Contributing
 ------------
 
 If you have any valuable contribution, suggestion or idea,
 please let me know as well because I will look into it.
```

### Comparing `django-safe-filefield-0.3.1/safe_filefield/clamav.py` & `django-safe-filefield-1.0.0/safe_filefield/clamav.py`

 * *Files identical despite different names*

### Comparing `django-safe-filefield-0.3.1/safe_filefield/forms.py` & `django-safe-filefield-1.0.0/safe_filefield/forms.py`

 * *Files identical despite different names*

### Comparing `django-safe-filefield-0.3.1/safe_filefield/models.py` & `django-safe-filefield-1.0.0/safe_filefield/models.py`

 * *Files identical despite different names*

### Comparing `django-safe-filefield-0.3.1/safe_filefield/validators.py` & `django-safe-filefield-1.0.0/safe_filefield/validators.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import mimetypes
 import os
 
 from django.core.exceptions import ValidationError
 from django.utils.deconstruct import deconstructible
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from . import clamav
 from .utils import detect_content_type
 
 
 @deconstructible
 class FileExtensionValidator(object):
@@ -25,15 +25,16 @@
 
         if code is not None:
             self.code = code
 
     def __call__(self, value):
         extension = os.path.splitext(value.name)[1][1:].lower()
 
-        if self.allowed_extensions is not None and extension not in self.allowed_extensions:
+        if (self.allowed_extensions is not None) \
+                and (extension not in self.allowed_extensions):
             raise ValidationError(
                 self.message,
                 code=self.code,
                 params={
                     'extension': extension,
                     'allowed_extensions': ', '.join(
                         self.allowed_extensions)
@@ -53,38 +54,51 @@
         if message is not None:
             self.message = message
 
         if code is not None:
             self.code = code
 
     def __call__(self, file):
+        if hasattr(file, '_get_file'):
+            file = file._get_file()
+
         __, ext = os.path.splitext(file.name)
 
         detected_content_type = detect_content_type(file)
 
-        is_valid_content_type = bool(
-            (
-                ext in mimetypes.guess_all_extensions(file.content_type)
-            ) or (
-                detected_content_type == 'application/CDFV2-unknown'
-                and file.content_type == mimetypes.guess_type('.doc')
-            ) or (
-                detected_content_type == file.content_type
+        if getattr(file, 'content_type', None) is not None:
+            is_valid_content_type = bool(
+                (ext in mimetypes.guess_all_extensions(detected_content_type)
+                 and ext in mimetypes.guess_all_extensions(file.content_type)
+                 ) or (detected_content_type == 'application/CDFV2-unknown'
+                       and file.content_type == mimetypes.guess_type('.doc')
+                       and ext == "doc")
+            )
+            params = {
+                'extension': ext,
+                'content_type': file.content_type,
+                'detected_content_type': detected_content_type
+            }
+        else:
+            is_valid_content_type = bool(
+                (ext in mimetypes.guess_all_extensions(detected_content_type))
+                or (detected_content_type == 'application/CDFV2-unknown'
+                    and ext == "doc")
             )
-        )
+            params = {
+                'extension': ext,
+                'content_type': None,
+                'detected_content_type': detected_content_type
+            }
 
         if not is_valid_content_type:
             raise ValidationError(
                 self.message,
                 code=self.code,
-                params={
-                    'extension': ext,
-                    'content_type': file.content_type,
-                    'detected_content_type': detected_content_type
-                }
+                params=params
             )
 
 
 class AntiVirusValidator:
     message = _('File is infected with %(virus)s.')
 
     code = 'infected'
```

