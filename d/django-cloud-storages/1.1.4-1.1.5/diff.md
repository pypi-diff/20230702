# Comparing `tmp/django_cloud_storages-1.1.4.tar.gz` & `tmp/django_cloud_storages-1.1.5.tar.gz`

## Comparing `django_cloud_storages-1.1.4.tar` & `django_cloud_storages-1.1.5.tar`

### file list

```diff
@@ -1,27 +1,18 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/.readthedocs.yaml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/manage.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/requirements.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/setup.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/cloud_storages/__init__.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/docs/Makefile
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/docs/conf.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/docs/make.bat
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/docs/requirements.txt
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/docs/backends/appwrite.rst
--rw-r--r--   0        0        0     6578 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/docs/backends/dropbox.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/tests/__init__.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/tests/settings.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/tests/test_appwrite.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/tests/test_dropbox.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/tests/test_folder/test_file.txt
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/LICENSE
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/README.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/.readthedocs.yaml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/setup.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/cloud_storages/__init__.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/tests/settings.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/tests/test_appwrite.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/tests/test_dropbox.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/tests/test_folder/test_file.txt
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/LICENSE
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/README.md
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.5/PKG-INFO
```

### Comparing `django_cloud_storages-1.1.4/.readthedocs.yaml` & `django_cloud_storages-1.1.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.4/cloud_storages/utils.py` & `django_cloud_storages-1.1.5/cloud_storages/utils.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.4/cloud_storages/backends/appwrite.py` & `django_cloud_storages-1.1.5/cloud_storages/backends/appwrite.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.4/cloud_storages/backends/dropbox.py` & `django_cloud_storages-1.1.5/cloud_storages/backends/dropbox.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.4/docs/index.rst` & `django_cloud_storages-1.1.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,36 @@
-.. django-cloud-storages documentation master file, created by
-   sphinx-quickstart on Fri Jun 30 17:42:08 2023.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
-Welcome to django-cloud-storages's documentation!
-=================================================
+# Welcome to django-cloud-storages
 
 django-cloud-storages is a package developed for django to work with cloud storages to store/upload media files.
 
+This package extends the [django Storage class](https://docs.djangoproject.com/en/4.2/ref/files/storage/#django.core.files.storage.Storage) to provide file storage in cloud.
+
 At the moment this package support the following cloud storage services -
 
-.. toctree::
-   :maxdepth: 1
-   :glob:
+* AppWrite
+* DropBox
 
-   backends/*
+### **Installation**
 
-Installation
-************
+---
 
-Use pip to install from PyPI::
+Use pip to install from PyPI:
 
-   pip install django-cloud-storages
+   `pip install django-cloud-storages`
 
 It will install all the cloud storage backends (available in this package), you can choose any of the storage backend as per your requirement.
 
-Contributing
-************
+### **Documentation**
 
-To contribute to django-cloud-storages `create a fork`_ on GitHub. Clone your fork, make some changes, and submit a pull request.
+The documentation for the package *django-cloud-storage* is available at [https://django-cloud-storages.readthedocs.io](https://django-cloud-storages.readthedocs.io/).
 
-.. _create a fork: https://github.com/Samiddha99/django-cloud-storages
+### **Contributing**
 
-Issues
-******
+---
 
-Use the GitHub `issue tracker`_ for django-cloud-storages to submit bugs, issues, and feature requests.
+To contribute to django-cloud-storages [create a fork](https://github.com/Samiddha99/django-cloud-storages) on GitHub. Clone your fork, make some changes, and submit a pull request.
 
-.. _issue tracker: https://github.com/Samiddha99/django-cloud-storages/issues
+### **Issues**
 
-Indices and tables
-==================
+---
 
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+Use the GitHub [issue tracker](https://github.com/Samiddha99/django-cloud-storages/issues) for django-cloud-storages to submit bugs, issues, and feature requests.
```

### Comparing `django_cloud_storages-1.1.4/tests/settings.py` & `django_cloud_storages-1.1.5/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.4/tests/test_appwrite.py` & `django_cloud_storages-1.1.5/tests/test_appwrite.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.4/tests/test_dropbox.py` & `django_cloud_storages-1.1.5/tests/test_dropbox.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.4/.gitignore` & `django_cloud_storages-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.4/LICENSE` & `django_cloud_storages-1.1.5/LICENSE`

 * *Files identical despite different names*

