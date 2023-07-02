# Comparing `tmp/sphinxcontrib-django-2.3.tar.gz` & `tmp/sphinxcontrib-django-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-django-2.3.tar", last modified: Wed Apr 12 13:50:46 2023, max compression
+gzip compressed data, was "sphinxcontrib-django-2.4.tar", last modified: Sun Jul  2 20:51:31 2023, max compression
```

## Comparing `sphinxcontrib-django-2.3.tar` & `sphinxcontrib-django-2.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.556496 sphinxcontrib-django-2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-12 13:50:46.556496 sphinxcontrib-django-2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 13:50:46.556496 sphinxcontrib-django-2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.552496 sphinxcontrib-django-2.3/sphinxcontrib_django/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.552496 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/field_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/sphinxcontrib_django/roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.552496 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 13:50:46.000000 sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:50:46.556496 sphinxcontrib-django-2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_attribute_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_autodoc_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_class_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_data_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_django_configured.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_django_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_method_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-12 13:50:36.000000 sphinxcontrib-django-2.3/tests/test_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:31.711599 sphinxcontrib-django-2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-02 20:51:31.711599 sphinxcontrib-django-2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 20:51:31.711599 sphinxcontrib-django-2.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:31.707599 sphinxcontrib-django-2.4/sphinxcontrib_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:31.707599 sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/field_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/sphinxcontrib_django/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:31.707599 sphinxcontrib-django-2.4/sphinxcontrib_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-02 20:51:31.000000 sphinxcontrib-django-2.4/sphinxcontrib_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-02 20:51:31.000000 sphinxcontrib-django-2.4/sphinxcontrib_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:51:31.000000 sphinxcontrib-django-2.4/sphinxcontrib_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 20:51:31.000000 sphinxcontrib-django-2.4/sphinxcontrib_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-02 20:51:31.000000 sphinxcontrib-django-2.4/sphinxcontrib_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:31.711599 sphinxcontrib-django-2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12728 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/tests/test_attribute_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/tests/test_autodoc_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/tests/test_class_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/tests/test_data_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/tests/test_django_configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/tests/test_django_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/tests/test_method_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-02 20:51:18.000000 sphinxcontrib-django-2.4/tests/test_roles.py
```

### Comparing `sphinxcontrib-django-2.3/LICENSE` & `sphinxcontrib-django-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/PKG-INFO` & `sphinxcontrib-django-2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-django
-Version: 2.3
+Version: 2.4
 Summary: Improve the Sphinx autodoc for Django classes.
 Author-email: Diederik van der Boor <opensource@edoburu.nl>, Timo Ludwig <ti.ludwig@web.de>
 License: Apache2 2.0 License
 Project-URL: Bug Tracker, https://github.com/edoburu/sphinxcontrib-django/issues
 Project-URL: Documentation, https://sphinxcontrib-django.readthedocs.io/
 Project-URL: Release Notes, https://github.com/edoburu/sphinxcontrib-django/blob/main/CHANGES.rst
 Project-URL: Source Code, https://github.com/edoburu/sphinxcontrib-django
@@ -116,16 +116,24 @@
     django_settings = "myapp.settings"
 
 Optionally, you can include the table names of your models in their docstrings with:
 
 .. code-block:: python
 
     # Include the database table names of Django models
-    django_show_db_tables = True
+    django_show_db_tables = True                # Boolean, default: False
+    # Add abstract database tables names (only takes effect if django_show_db_tables is True)
+    django_show_db_tables_abstract = True       # Boolean, default: False
 
+Optionally, you can extend amount of displayed choices in model fields with them:
+
+.. code-block:: python
+
+    # Integer amount of model field choices to show, default 10
+    django_choices_to_show = 10
 
 Advanced Usage
 --------------
 
 If you want to run custom code which depends on Django, e.g. to monkeypatch your application during documentation build,
 you might run into an `ImproperlyConfigured <https://docs.djangoproject.com/en/stable/ref/exceptions/#improperlyconfigured>`_ exception:
```

### Comparing `sphinxcontrib-django-2.3/README.rst` & `sphinxcontrib-django-2.4/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -76,16 +76,24 @@
     django_settings = "myapp.settings"
 
 Optionally, you can include the table names of your models in their docstrings with:
 
 .. code-block:: python
 
     # Include the database table names of Django models
-    django_show_db_tables = True
+    django_show_db_tables = True                # Boolean, default: False
+    # Add abstract database tables names (only takes effect if django_show_db_tables is True)
+    django_show_db_tables_abstract = True       # Boolean, default: False
 
+Optionally, you can extend amount of displayed choices in model fields with them:
+
+.. code-block:: python
+
+    # Integer amount of model field choices to show, default 10
+    django_choices_to_show = 10
 
 Advanced Usage
 --------------
 
 If you want to run custom code which depends on Django, e.g. to monkeypatch your application during documentation build,
 you might run into an `ImproperlyConfigured <https://docs.djangoproject.com/en/stable/ref/exceptions/#improperlyconfigured>`_ exception:
```

### Comparing `sphinxcontrib-django-2.3/pyproject.toml` & `sphinxcontrib-django-2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/__init__.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This is a sphinx extension which improves the documentation of Django apps.
 """
-__version__ = "2.3"
+__version__ = "2.4"
 
 from . import docstrings, roles
 
 
 def setup(app):
     """
     Allow this module to be used as sphinx extension.
```

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/__init__.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import django
 from sphinx.errors import ConfigError
 
 from .. import __version__
 from .attributes import improve_attribute_docstring
 from .classes import improve_class_docstring
-from .config import EXCLUDE_MEMBERS, INCLUDE_MEMBERS
+from .config import CHOICES_LIMIT, EXCLUDE_MEMBERS, INCLUDE_MEMBERS
 from .data import improve_data_docstring
 from .methods import improve_method_docstring
 
 
 def setup(app):
     """
     Allow this package to be used as Sphinx extension.
@@ -55,16 +55,21 @@
     app.add_event("django-configured")
 
     # Set default to environment variable to enable backwards compatibility
     app.add_config_value(
         "django_settings", os.environ.get("DJANGO_SETTINGS_MODULE"), True
     )
 
+    # Django models tables names configuration.
     # Set default of django_show_db_tables to False
     app.add_config_value("django_show_db_tables", False, True)
+    # Set default of django_show_db_tables_abstract to False
+    app.add_config_value("django_show_db_tables_abstract", False, True)
+    # Integer amount of model field choices to show
+    app.add_config_value("django_choices_to_show", CHOICES_LIMIT, True)
     # Setup Django after config is initialized
     app.connect("config-inited", setup_django)
 
     # Load sphinx.ext.autodoc extension before registering events
     app.setup_extension("sphinx.ext.autodoc")
 
     # Generate docstrings for Django model fields
@@ -103,15 +108,15 @@
         )
     try:
         importlib.import_module(config.django_settings)
     except ModuleNotFoundError as e:
         raise ConfigError(
             "The module you specified in the configuration 'django_settings' in your"
             " conf.py cannot be imported. Make sure the module path is correct and the"
-            " source directoy is added to sys.path."
+            " source directory is added to sys.path."
         ) from e
     os.environ["DJANGO_SETTINGS_MODULE"] = config.django_settings
     django.setup()
 
     # Emit event to allow code which depends on Django to run
     app.emit("django-configured")
 
@@ -174,15 +179,15 @@
 
     :return: The modified list of lines
     :rtype: list [ str ]
     """
     if what == "class":
         improve_class_docstring(app, obj, lines)
     elif what == "attribute":
-        improve_attribute_docstring(obj, name, lines)
+        improve_attribute_docstring(app, obj, name, lines)
     elif what == "method":
         improve_method_docstring(name, lines)
     elif what == "data":
         improve_data_docstring(obj, lines)
 
     # Return the extended docstring
     return lines
```

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/attributes.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/attributes.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,34 +5,36 @@
 from django.db.models.fields import related_descriptors
 from django.db.models.fields.files import FileDescriptor
 from django.db.models.manager import ManagerDescriptor
 from django.db.models.query_utils import DeferredAttribute
 from django.utils.module_loading import import_string
 from sphinx.util.docstrings import prepare_docstring
 
-from .config import CHOICES_LIMIT
 from .field_utils import get_field_type, get_field_verbose_name
 
 FIELD_DESCRIPTORS = (FileDescriptor, related_descriptors.ForwardManyToOneDescriptor)
 
 # Support for some common third party fields
 try:
     from phonenumber_field.modelfields import PhoneNumberDescriptor
 
     FIELD_DESCRIPTORS += (PhoneNumberDescriptor,)
 except ImportError:
     PhoneNumberDescriptor = None
 
 
-def improve_attribute_docstring(attribute, name, lines):
+def improve_attribute_docstring(app, attribute, name, lines):
     """
     Improve the documentation of various model fields.
 
     This improves the navigation between related objects.
 
+    :param app: The Sphinx application object
+    :type app: ~sphinx.application.Sphinx
+
     :param attribute: The instance of the object to document
     :type attribute: object
 
     :param name: The full dotted path to the object
     :type name: str
 
     :param lines: The docstring lines
@@ -52,29 +54,29 @@
             # with the postfix "_id" and contains the reference to the id of the related model
             # instance. These are usually undocumented, so they only are included in the docs
             # is sphinx is invoked with the undoc-members option.
             lines.append(
                 f"Internal field, use :class:`~{cls_path}.{field.name}` instead."
             )
         else:
-            lines.extend(get_field_details(field))
+            lines.extend(get_field_details(app, field))
     elif isinstance(attribute, FIELD_DESCRIPTORS):
         # Display a reasonable output for forward descriptors (foreign key and one to one fields).
-        lines.extend(get_field_details(attribute.field))
+        lines.extend(get_field_details(app, attribute.field))
     elif isinstance(attribute, related_descriptors.ManyToManyDescriptor):
         # Check this case first since ManyToManyDescriptor inherits from ReverseManyToOneDescriptor
         # This descriptor is used for both forward and reverse relationships
         if attribute.reverse:
-            lines.extend(get_field_details(attribute.rel))
+            lines.extend(get_field_details(app, attribute.rel))
         else:
-            lines.extend(get_field_details(attribute.field))
+            lines.extend(get_field_details(app, attribute.field))
     elif isinstance(attribute, related_descriptors.ReverseManyToOneDescriptor):
-        lines.extend(get_field_details(attribute.rel))
+        lines.extend(get_field_details(app, attribute.rel))
     elif isinstance(attribute, related_descriptors.ReverseOneToOneDescriptor):
-        lines.extend(get_field_details(attribute.related))
+        lines.extend(get_field_details(app, attribute.related))
     elif isinstance(attribute, (models.Manager, ManagerDescriptor)):
         # Somehow the 'objects' manager doesn't pass through the docstrings.
         module, model_name, field_name = name.rsplit(".", 2)
         lines.append("Django manager to access the ORM")
         lines.append(f"Use ``{model_name}.objects.all()`` to fetch all objects.")
     # Check if there are initial docstrings to be appended
     if docstring_lines:
@@ -88,36 +90,44 @@
             if lines:
                 # If lines are not empty, append a separating new line before docstring
                 lines.append("")
             # Remove last element because it's a newline
             lines.extend(docstring_lines[:-1])
 
 
-def get_field_details(field):
+def get_field_details(app, field):
     """
     This function returns the detail docstring of a model field.
     It includes the field type and the verbose name of the field.
 
+    :param app: The Sphinx application object
+    :type app: ~sphinx.application.Sphinx
+
     :param field: The field
     :type field: ~django.db.models.Field
 
     :return: The field details as list of strings
     :rtype: list [ str ]
     """
+    choices_limit = app.config.django_choices_to_show
+
     field_details = [
         f"Type: {get_field_type(field)}",
         "",
         f"{get_field_verbose_name(field)}",
     ]
     if hasattr(field, "choices") and field.choices:
         field_details.extend(["", "Choices:", ""])
         field_details.extend(
-            [f"* ``{key}``" for key, value in field.choices[:CHOICES_LIMIT]]
+            [
+                f"* ``{key}``" if key != "" else "* ``''`` (Empty string)"
+                for key, value in field.choices[:choices_limit]
+            ]
         )
         # Check if list has been truncated
-        if len(field.choices) > CHOICES_LIMIT:
+        if len(field.choices) > choices_limit:
             # If only one element has been truncated, just list it as well
-            if len(field.choices) == CHOICES_LIMIT + 1:
+            if len(field.choices) == choices_limit + 1:
                 field_details.append(f"* ``{field.choices[-1][0]}``")
             else:
-                field_details.append(f"* and {len(field.choices) - CHOICES_LIMIT} more")
+                field_details.append(f"* and {len(field.choices) - choices_limit} more")
     return field_details
```

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/classes.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,16 +42,15 @@
 
     :param lines: The docstring lines
     :type lines: list [ str ]
     """
 
     # Add database table name
     if app.config.django_show_db_tables:
-        lines.insert(0, "")
-        lines.insert(0, f"**Database table:** ``{model._meta.db_table}``")
+        add_db_table_name(app, model, lines)
 
     # Get predefined params to exclude them from the automatically inserted params
     param_offset = len(":param ")
     predefined_params = [
         line[param_offset : line.find(":", param_offset)]
         for line in lines
         if line.startswith(":param ") and ":" in line[param_offset:]
@@ -112,14 +111,35 @@
         "sphinx.ext.inheritance_diagram" in app.extensions
         and "sphinx.ext.graphviz" in app.extensions
         and not any("inheritance-diagram::" in line for line in lines)
     ):
         lines.append(".. inheritance-diagram::")  # pragma: no cover
 
 
+def add_db_table_name(app, model, lines):
+    """
+    Format and add table name by extension configuration.
+
+    :param app: The Sphinx application object
+    :type app: ~sphinx.application.Sphinx
+
+    :param model: The instance of the model to document
+    :type model: ~django.db.models.Model
+
+    :param lines: The docstring lines
+    :type lines: list [ str ]
+    """
+    if model._meta.abstract and not app.config.django_show_db_tables_abstract:
+        return
+
+    table_name = None if model._meta.abstract else model._meta.db_table
+    lines.insert(0, "")
+    lines.insert(0, f"**Database table:** ``{table_name}``")
+
+
 def add_model_parameters(fields, lines, field_docs):
     """
     Add the given fields as model parameter with the ``:param:`` directive
 
     :param fields: The list of fields
     :type fields: list [ ~django.db.models.Field ]
```

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/config.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,9 +18,10 @@
     "panels",
     "content_panels",
     # Polymorphic
     "polymorphic_primary_key_name",
     "polymorphic_super_sub_accessors_replaced",
 }
 
-#: How many choices should be shown for model fields
+#: How many choices should be shown for model fields by default,
+#: used as default for ``django_choices_to_show`` option
 CHOICES_LIMIT = 10
```

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/data.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/data.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/field_utils.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/field_utils.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/methods.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/methods.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/docstrings/patches.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/docstrings/patches.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django/roles.py` & `sphinxcontrib-django-2.4/sphinxcontrib_django/roles.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/PKG-INFO` & `sphinxcontrib-django-2.4/sphinxcontrib_django.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-django
-Version: 2.3
+Version: 2.4
 Summary: Improve the Sphinx autodoc for Django classes.
 Author-email: Diederik van der Boor <opensource@edoburu.nl>, Timo Ludwig <ti.ludwig@web.de>
 License: Apache2 2.0 License
 Project-URL: Bug Tracker, https://github.com/edoburu/sphinxcontrib-django/issues
 Project-URL: Documentation, https://sphinxcontrib-django.readthedocs.io/
 Project-URL: Release Notes, https://github.com/edoburu/sphinxcontrib-django/blob/main/CHANGES.rst
 Project-URL: Source Code, https://github.com/edoburu/sphinxcontrib-django
@@ -116,16 +116,24 @@
     django_settings = "myapp.settings"
 
 Optionally, you can include the table names of your models in their docstrings with:
 
 .. code-block:: python
 
     # Include the database table names of Django models
-    django_show_db_tables = True
+    django_show_db_tables = True                # Boolean, default: False
+    # Add abstract database tables names (only takes effect if django_show_db_tables is True)
+    django_show_db_tables_abstract = True       # Boolean, default: False
 
+Optionally, you can extend amount of displayed choices in model fields with them:
+
+.. code-block:: python
+
+    # Integer amount of model field choices to show, default 10
+    django_choices_to_show = 10
 
 Advanced Usage
 --------------
 
 If you want to run custom code which depends on Django, e.g. to monkeypatch your application during documentation build,
 you might run into an `ImproperlyConfigured <https://docs.djangoproject.com/en/stable/ref/exceptions/#improperlyconfigured>`_ exception:
```

### Comparing `sphinxcontrib-django-2.3/sphinxcontrib_django.egg-info/SOURCES.txt` & `sphinxcontrib-django-2.4/sphinxcontrib_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/tests/test_attribute_docstrings.py` & `sphinxcontrib-django-2.4/tests/test_attribute_docstrings.py`

 * *Files 15% similar despite different names*

```diff
@@ -367,14 +367,72 @@
         "   * ``8``",
         "   * ``9``",
         "   * and 2 more",
         "",
     ]
 
 
+@pytest.mark.sphinx(
+    "html", testroot="docstrings", confoverrides={"django_choices_to_show": 15}
+)
+def test_choice_field_custom_limit(app, do_autodoc):
+    actual = do_autodoc(
+        app, "attribute", "dummy_django_app.models.ChoiceModel.choice_limit_above"
+    )
+    print(actual)
+    assert list(actual) == [
+        "",
+        ".. py:attribute:: ChoiceModel.choice_limit_above",
+        "   :module: dummy_django_app.models",
+        "",
+        "   Type: :class:`~django.db.models.IntegerField`",
+        "",
+        "   Choice limit above",
+        "",
+        "   Choices:",
+        "",
+        "   * ``0``",
+        "   * ``1``",
+        "   * ``2``",
+        "   * ``3``",
+        "   * ``4``",
+        "   * ``5``",
+        "   * ``6``",
+        "   * ``7``",
+        "   * ``8``",
+        "   * ``9``",
+        "   * ``10``",
+        "   * ``11``",
+        "",
+    ]
+
+
+@pytest.mark.sphinx("html", testroot="docstrings")
+def test_choice_field_empty(app, do_autodoc):
+    actual = do_autodoc(
+        app, "attribute", "dummy_django_app.models.ChoiceModel.choice_with_empty"
+    )
+    print(actual)
+    assert list(actual) == [
+        "",
+        ".. py:attribute:: ChoiceModel.choice_with_empty",
+        "   :module: dummy_django_app.models",
+        "",
+        "   Type: :class:`~django.db.models.CharField`",
+        "",
+        "   Choice with empty",
+        "",
+        "   Choices:",
+        "",
+        "   * ``''`` (Empty string)",
+        "   * ``Something``",
+        "",
+    ]
+
+
 if PHONENUMBER:
 
     @pytest.mark.sphinx("html", testroot="docstrings")
     def test_phonenumber_field(app, do_autodoc):
         actual = do_autodoc(
             app, "attribute", "dummy_django_app.models.PhoneNumberModel.phone_number"
         )
```

### Comparing `sphinxcontrib-django-2.3/tests/test_autodoc_skip.py` & `sphinxcontrib-django-2.4/tests/test_autodoc_skip.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/tests/test_class_docstrings.py` & `sphinxcontrib-django-2.4/tests/test_class_docstrings.py`

 * *Files 8% similar despite different names*

```diff
@@ -198,14 +198,87 @@
             "   :type foreignkey_self: :class:`~django.db.models.ForeignKey` to"
             " :class:`~dummy_django_app.models.AbstractModel`"
         ),
         "",
     ]
 
 
+@pytest.mark.sphinx(
+    "html", testroot="docstrings", confoverrides={"django_show_db_tables": True}
+)
+def test_abstract_model_with_tables_names_and_ignore_abstract(app, do_autodoc):
+    actual = do_autodoc(app, "class", "dummy_django_app.models.AbstractModel")
+    print(actual)
+    assert list(actual) == [
+        "",
+        ".. py:class:: AbstractModel(*args, **kwargs)",
+        "   :module: dummy_django_app.models",
+        "",
+        "",
+        "   Relationship fields:",
+        "",
+        "   :param simple_model: Simple model",
+        (
+            "   :type simple_model: :class:`~django.db.models.ForeignKey` to"
+            " :class:`~dummy_django_app.models.SimpleModel`"
+        ),
+        "   :param user: User",
+        (
+            "   :type user: :class:`~django.db.models.ForeignKey` to"
+            " :class:`~django.contrib.auth.models.User`"
+        ),
+        "   :param foreignkey_self: Foreignkey self",
+        (
+            "   :type foreignkey_self: :class:`~django.db.models.ForeignKey` to"
+            " :class:`~dummy_django_app.models.AbstractModel`"
+        ),
+        "",
+    ]
+
+
+@pytest.mark.sphinx(
+    "html",
+    testroot="docstrings",
+    confoverrides={
+        "django_show_db_tables": True,
+        "django_show_db_tables_abstract": True,
+    },
+)
+def test_abstract_model_with_tables_names_and_abstract_show(app, do_autodoc):
+    actual = do_autodoc(app, "class", "dummy_django_app.models.AbstractModel")
+    print(actual)
+    assert list(actual) == [
+        "",
+        ".. py:class:: AbstractModel(*args, **kwargs)",
+        "   :module: dummy_django_app.models",
+        "",
+        "   **Database table:** ``None``",
+        "",
+        "",
+        "   Relationship fields:",
+        "",
+        "   :param simple_model: Simple model",
+        (
+            "   :type simple_model: :class:`~django.db.models.ForeignKey` to"
+            " :class:`~dummy_django_app.models.SimpleModel`"
+        ),
+        "   :param user: User",
+        (
+            "   :type user: :class:`~django.db.models.ForeignKey` to"
+            " :class:`~django.contrib.auth.models.User`"
+        ),
+        "   :param foreignkey_self: Foreignkey self",
+        (
+            "   :type foreignkey_self: :class:`~django.db.models.ForeignKey` to"
+            " :class:`~dummy_django_app.models.AbstractModel`"
+        ),
+        "",
+    ]
+
+
 @pytest.mark.sphinx("html", testroot="docstrings")
 def test_file_model(app, do_autodoc):
     actual = do_autodoc(app, "class", "dummy_django_app.models.FileModel")
     print(actual)
     assert list(actual) == [
         "",
         ".. py:class:: FileModel(id, upload)",
```

### Comparing `sphinxcontrib-django-2.3/tests/test_data_docstrings.py` & `sphinxcontrib-django-2.4/tests/test_data_docstrings.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/tests/test_django_configured.py` & `sphinxcontrib-django-2.4/tests/test_django_configured.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/tests/test_django_setup.py` & `sphinxcontrib-django-2.4/tests/test_django_setup.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-django-2.3/tests/test_method_docstrings.py` & `sphinxcontrib-django-2.4/tests/test_method_docstrings.py`

 * *Files identical despite different names*

