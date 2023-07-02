# Comparing `tmp/django_bootstrap_datepicker_plus-5.0.3.tar.gz` & `tmp/django_bootstrap_datepicker_plus-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_bootstrap_datepicker_plus-5.0.3.tar", max compression
+gzip compressed data, was "django_bootstrap_datepicker_plus-5.0.4.tar", max compression
```

## Comparing `django_bootstrap_datepicker_plus-5.0.3.tar` & `django_bootstrap_datepicker_plus-5.0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1068 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/LICENSE
--rw-r--r--   0        0        0     7987 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/README.rst
--rw-r--r--   0        0        0     3908 2023-01-12 04:15:12.661822 django_bootstrap_datepicker_plus-5.0.3/pyproject.toml
--rw-r--r--   0        0        0       60 2023-01-12 04:15:12.697822 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/__init__.py
--rw-r--r--   0        0        0     4584 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/_base.py
--rw-r--r--   0        0        0      754 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/_config.py
--rw-r--r--   0        0        0        0 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/py.typed
--rw-r--r--   0        0        0      419 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/schemas.py
--rw-r--r--   0        0        0     2739 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/settings.py
--rw-r--r--   0        0        0     1814 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/static/bootstrap_datepicker_plus/css/datepicker-widget.css
--rw-r--r--   0        0        0     9240 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/static/bootstrap_datepicker_plus/js/datepicker-widget.js
--rw-r--r--   0        0        0     1004 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/templates/bootstrap_datepicker_plus/input.html
--rw-r--r--   0        0        0     1261 2023-01-12 04:14:55.581838 django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/widgets.py
--rw-r--r--   0        0        0     9324 1970-01-01 00:00:00.000000 django_bootstrap_datepicker_plus-5.0.3/setup.py
--rw-r--r--   0        0        0     9549 1970-01-01 00:00:00.000000 django_bootstrap_datepicker_plus-5.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-02 18:58:29.497068 django_bootstrap_datepicker_plus-5.0.4/LICENSE
+-rw-r--r--   0        0        0     7987 2023-07-02 18:58:29.497068 django_bootstrap_datepicker_plus-5.0.4/README.rst
+-rw-r--r--   0        0        0     4058 2023-07-02 18:58:46.505822 django_bootstrap_datepicker_plus-5.0.4/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-07-02 18:58:46.549823 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/__init__.py
+-rw-r--r--   0        0        0     4584 2023-07-02 18:58:29.501068 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/_base.py
+-rw-r--r--   0        0        0      754 2023-07-02 18:58:29.501068 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/_config.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:58:29.501068 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/py.typed
+-rw-r--r--   0        0        0      419 2023-07-02 18:58:29.501068 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/schemas.py
+-rw-r--r--   0        0        0     2916 2023-07-02 18:58:29.501068 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/settings.py
+-rw-r--r--   0        0        0     1814 2023-07-02 18:58:29.501068 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/static/bootstrap_datepicker_plus/css/datepicker-widget.css
+-rw-r--r--   0        0        0     9240 2023-07-02 18:58:29.501068 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/static/bootstrap_datepicker_plus/js/datepicker-widget.js
+-rw-r--r--   0        0        0     1004 2023-07-02 18:58:29.501068 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/templates/bootstrap_datepicker_plus/input.html
+-rw-r--r--   0        0        0     1261 2023-07-02 18:58:29.501068 django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/widgets.py
+-rw-r--r--   0        0        0     9549 1970-01-01 00:00:00.000000 django_bootstrap_datepicker_plus-5.0.4/PKG-INFO
```

### Comparing `django_bootstrap_datepicker_plus-5.0.3/LICENSE` & `django_bootstrap_datepicker_plus-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bootstrap_datepicker_plus-5.0.3/README.rst` & `django_bootstrap_datepicker_plus-5.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `django_bootstrap_datepicker_plus-5.0.3/pyproject.toml` & `django_bootstrap_datepicker_plus-5.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "django-bootstrap-datepicker-plus"
-version = "5.0.3"
+version = "5.0.4"
 description = """\
     Bootstrap3/Bootstrap4/Bootstrap5 DatePickerInput, TimePickerInput, \
     DateTimePickerInput, MonthPickerInput, YearPickerInput\
     """
 readme = "README.rst"
 authors = ["Munim Munna <6266677+monim67@users.noreply.github.com>"]
 repository = "https://github.com/monim67/django-bootstrap-datepicker-plus"
 documentation = "https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/"
-packages = [{ include = "*", from = "src" }]
+packages = [{ include = "bootstrap_datepicker_plus", from = "src" }]
 license = "MIT"
 keywords = [
     "django",
     "bootstrap",
     "date-picker",
     "time-picker",
     "datetime-picker",
@@ -38,19 +38,20 @@
 pydantic = "*"
 typing-extensions = "*"
 
 [tool.poetry.group.build.dependencies]
 django-bootstrap3 = "^21.2"
 django-bootstrap4 = "^22.1"
 django-bootstrap5 = "^22.1"
+django-bootstrap-modal-forms = "^2.2.1"
 pytest-django = "^4.5.2"
 pytest-dotenv = "^0.5.2"
 black = "^22.6.0"
 isort = "^5.10.1"
-pydocstyle = {extras = ["toml"], version = "^6.1.1"}
+pydocstyle = { extras = ["toml"], version = "^6.1.1" }
 mypy = "*"
 django-stubs = "^1.12.0"
 coverage = { extras = ["toml"], version = "^6.5.0" }
 rstcheck = "^6.1.0"
 sphinx = "^4.3.2"
 poethepoet = "^0.15.0"
 django-crispy-forms = "^1.14.0"
@@ -80,26 +81,33 @@
 [tool.mypy]
 python_version = "3.7"
 namespace_packages = true
 strict = true
 plugins = ["mypy_django_plugin.main"]
 
 [[tool.mypy.overrides]]
-module = ["dev.myapp.migrations.*", "urllib3.*", "crispy_forms.*", "django_filters.*", "importlib_metadata.*"]
+module = [
+    "dev.myapp.migrations.*",
+    "urllib3.*",
+    "crispy_forms.*",
+    "django_filters.*",
+    "importlib_metadata.*",
+    "bootstrap_modal_forms.*",
+]
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = ["dev.myapp.migrations.*"]
 ignore_errors = true
 
 [tool.django-stubs]
 django_settings_module = "dev.mysite.settings"
 
 [tool.pytest.ini_options]
-pythonpath = "." # pytest-django needs it to find dev module
+pythonpath = "."                               # pytest-django needs it to find dev module
 django_find_project = false
 DJANGO_SETTINGS_MODULE = "dev.mysite.settings"
 addopts = "--reuse-db"
 testpaths = ["tests"]
 env_files = [".env", ".env.defaults"]
 
 [tool.coverage.run]
```

### Comparing `django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/_base.py` & `django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/_base.py`

 * *Files identical despite different names*

### Comparing `django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/_config.py` & `django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/_config.py`

 * *Files identical despite different names*

### Comparing `django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/settings.py` & `django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Package settings."""
 import functools
 from typing import Any, Dict, Optional, Tuple
 
 from django.conf import settings as django_settings
-from pydantic import Field, validator
-from pydantic.env_settings import BaseSettings, SettingsSourceCallable
+
+try:
+    from pydantic import Field, validator
+    from pydantic.env_settings import BaseSettings, SettingsSourceCallable
+except:
+    from pydantic.v1.env_settings import BaseSettings, SettingsSourceCallable  # type: ignore
+    from pydantic.v1 import Field, validator  # type: ignore
 
 from .schemas import WidgetOptions, WidgetVariant
 
 
 def _django_settings_source(settings: BaseSettings) -> Dict[str, Any]:
     return getattr(django_settings, "BOOTSTRAP_DATEPICKER_PLUS", {})
```

### Comparing `django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/static/bootstrap_datepicker_plus/css/datepicker-widget.css` & `django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/static/bootstrap_datepicker_plus/css/datepicker-widget.css`

 * *Files identical despite different names*

### Comparing `django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/static/bootstrap_datepicker_plus/js/datepicker-widget.js` & `django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/static/bootstrap_datepicker_plus/js/datepicker-widget.js`

 * *Files identical despite different names*

### Comparing `django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/templates/bootstrap_datepicker_plus/input.html` & `django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/templates/bootstrap_datepicker_plus/input.html`

 * *Files identical despite different names*

### Comparing `django_bootstrap_datepicker_plus-5.0.3/src/bootstrap_datepicker_plus/widgets.py` & `django_bootstrap_datepicker_plus-5.0.4/src/bootstrap_datepicker_plus/widgets.py`

 * *Files identical despite different names*

### Comparing `django_bootstrap_datepicker_plus-5.0.3/setup.py` & `django_bootstrap_datepicker_plus-5.0.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,242 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-bootstrap-datepicker-plus
+Version: 5.0.4
+Summary: Bootstrap3/Bootstrap4/Bootstrap5 DatePickerInput, TimePickerInput, DateTimePickerInput, MonthPickerInput, YearPickerInput
+Home-page: https://github.com/monim67/django-bootstrap-datepicker-plus
+License: MIT
+Keywords: django,bootstrap,date-picker,time-picker,datetime-picker,date-range-picker
+Author: Munim Munna
+Author-email: 6266677+monim67@users.noreply.github.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Requires-Dist: Django (>=2,<5)
+Requires-Dist: pydantic
+Requires-Dist: typing-extensions
+Project-URL: Documentation, https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/monim67/django-bootstrap-datepicker-plus
+Description-Content-Type: text/x-rst
+
+########################################
+django-bootstrap-datepicker-plus
+########################################
+
+This django widget contains Bootstrap 3, Bootstrap 4 and Bootstrap 5
+Date-Picker, Time-Picker, DateTime-Picker, Month-Picker and Year-Picker input
+with date-range-picker functionality for django version >= 2.0.
+The widget implements `bootstrap-datetimepicker v4 <https://getdatepicker.com/4/>`_
+to show bootstrap-datepicker in django model forms and custom forms
+which can be configured easily for date-range selection.
+
+If you are not using Bootstrap use `django-flatpickr <https://github.com/monim67/django-flatpickr>`_ instead.
+
+|  |build-status| |docs-status| |coverage|
+|  |pyversions| |djversions| |license|
+
+|  |date-picker-image| |datetime-picker-image| |time-picker-image|
+
+
+
+********************
+Demo
+********************
+
+- `With Bootstrap 3 <https://monim67.github.io/django-bootstrap-datepicker-plus/demo/bootstrap3/>`_
+- `With Bootstrap 4 <https://monim67.github.io/django-bootstrap-datepicker-plus/demo/bootstrap4/>`_
+- `With Bootstrap 5 <https://monim67.github.io/django-bootstrap-datepicker-plus/demo/bootstrap5/>`_
+
+
+
+********************
+Getting Started
+********************
+
+- Follow the `Getting Started doc <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Getting_Started.html>`_.
+- Head over to `Usage <#usage>`_ section to see how to use it in forms and views.
+- Read detailed `Documentation on ReadTheDocs <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/>`_
+- Looks complex to get started? Follow a `Quick Walkthrough Tutorial <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Walkthrough.html>`_
+- Getting errors? See `Troubleshoot instructions <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Troubleshooting.html>`_
+
+
+
+********************
+Usage
+********************
+
+
+++++++++++++++++++++++++++++++
+Usage in Generic View
+++++++++++++++++++++++++++++++
+
+.. code:: python
+
+    # File: views.py
+    from bootstrap_datepicker_plus.widgets import DateTimePickerInput
+    from django.views import generic
+    from .models import Question
+
+    class CreateView(generic.edit.CreateView):
+        model = Question
+        fields = ["question_text", "pub_date"]
+        def get_form(self):
+            form = super().get_form()
+            form.fields["pub_date"].widget = DateTimePickerInput()
+            return form
+
+
+++++++++++++++++++++++++++++++
+Advanced Usage
+++++++++++++++++++++++++++++++
+
+- `Usage in Custom Form <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Usage.html#custom-form-usage>`_
+- `Usage in Model Form <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Usage.html#model-form-usage>`_
+- `Usage doc <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Usage.html>`_
+
+
+++++++++++++++++++++++++++++++
+Types of DatePickers
+++++++++++++++++++++++++++++++
+
+The widget contains all types of date-picker you may ever need.
+
+.. code:: python
+
+    # File: forms.py
+    from bootstrap_datepicker_plus.widgets import DatePickerInput, TimePickerInput, DateTimePickerInput, MonthPickerInput, YearPickerInput
+    from django import forms
+
+    class EventForm(forms.ModelForm):
+        class Meta:
+            model = Event
+            fields = ["start_date", "start_time", "start_datetime", "start_month", "start_year"]
+            widgets = {
+                "start_date": DatePickerInput(),
+                "start_time": TimePickerInput(),
+                "start_datetime": DateTimePickerInput(),
+                "start_month": MonthPickerInput(),
+                "start_year": YearPickerInput(),
+            }
+
+
+++++++++++++++++++++++++++++++
+Implement date-range-picker
+++++++++++++++++++++++++++++++
+
+DatePickers can be linked to select a date-range or time-range.
+
+.. code:: python
+
+    # File: forms.py
+    from bootstrap_datepicker_plus.widgets import DatePickerInput, TimePickerInput
+    from django import forms
+
+    class EventForm(forms.ModelForm):
+        class Meta:
+            model = Event
+            fields = ["name", "start_date", "end_date", "start_time", "end_time"]
+            widgets = {
+                "start_date": DatePickerInput(),
+                "end_date": DatePickerInput(range_from="start_date"),
+                "start_time": TimePickerInput(),
+                "end_time": TimePickerInput(range_from="start_time"),
+            }
+
+
+++++++++++++++++++++++++++++++
+Customization
+++++++++++++++++++++++++++++++
+
+- `Customize date format, language <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/customization.html>`_
+- `Use custom template for widget input <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Template_Customizing.html>`_
+
+
+********************
+Contributing
+********************
+
+- `CONTRIBUTING.md <https://github.com/monim67/django-bootstrap-datepicker-plus/blob/master/.github/CONTRIBUTING.md>`_.
+- `CODE_OF_CONDUCT.md <https://github.com/monim67/django-bootstrap-datepicker-plus/blob/master/.github/CODE_OF_CONDUCT.md>`_.
+
+********************
+License
+********************
+
+This project is licensed under `MIT LICENSE <https://github.com/monim67/django-bootstrap-datepicker-plus/blob/master/LICENSE>`_ file for details.
+
+********************
+Acknowledgments
+********************
+
+This project implements `Eonasdan/bootstrap-datetimepicker <https://github.com/Eonasdan/bootstrap-datetimepicker>`_ to display date-pickers.
+The project was initially forked from `pbucher/django-bootstrap-datepicker <https://github.com/pbucher/django-bootstrap-datepicker>`_ and
+later reworked completely under MIT Licence.
+
+
+|buymeacoffee|
+
+
+.. |date-picker-image| image:: https://raw.githubusercontent.com/monim67/django-bootstrap-datepicker-plus/26d89a744d403a895422313a48c02885c4718251/images/date-picker.png
+    :alt: Date-picker
+    :width: 218px
+    :height: 280px
+
+.. |datetime-picker-image| image:: https://raw.githubusercontent.com/monim67/django-bootstrap-datepicker-plus/26d89a744d403a895422313a48c02885c4718251/images/datetime-picker.png
+    :alt: Datetime-picker
+    :width: 218px
+    :height: 280px
+
+.. |time-picker-image| image:: https://raw.githubusercontent.com/monim67/django-bootstrap-datepicker-plus/26d89a744d403a895422313a48c02885c4718251/images/time-picker.png
+    :alt: Time-picker
+    :width: 218px
+    :height: 280px
+
+.. |build-status| image:: https://github.com/monim67/django-bootstrap-datepicker-plus/actions/workflows/build.yml/badge.svg?event=push
+    :target: https://github.com/monim67/django-bootstrap-datepicker-plus/actions/workflows/build.yml
+    :alt: Build Status
+    :height: 20px
+
+.. |docs-status| image:: https://readthedocs.org/projects/django-bootstrap-datepicker-plus/badge/?version=latest
+    :target: https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+    :height: 20px
+
+.. |coverage| image:: https://coveralls.io/repos/github/monim67/django-bootstrap-datepicker-plus/badge.svg?branch=master
+    :target: https://coveralls.io/github/monim67/django-bootstrap-datepicker-plus?branch=master
+    :alt: Coverage Status
+    :height: 20px
+
+.. |pyversions| image:: https://img.shields.io/pypi/pyversions/django-bootstrap-datepicker-plus.svg
+    :target: https://pypi.python.org/pypi/django-bootstrap-datepicker-plus
+    :alt: Python Versions
+    :height: 20px
+
+.. |djversions| image:: https://img.shields.io/pypi/djversions/django-bootstrap-datepicker-plus.svg
+    :target: https://pypi.python.org/pypi/django-bootstrap-datepicker-plus
+    :alt: DJango Versions
+    :height: 20px
+
+.. |license| image:: https://img.shields.io/pypi/l/django-bootstrap-datepicker-plus.svg
+    :target: https://pypi.python.org/pypi/django-bootstrap-datepicker-plus
+    :alt: Licence
+    :height: 20px
+
+.. |buymeacoffee| image:: https://cdn.buymeacoffee.com/buttons/v2/default-orange.png
+   :target: https://www.buymeacoffee.com/monim67
+   :alt: Buy Me A Coffee
+   :height: 48px
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['bootstrap_datepicker_plus']
-
-package_data = \
-{'': ['*'],
- 'bootstrap_datepicker_plus': ['static/bootstrap_datepicker_plus/css/*',
-                               'static/bootstrap_datepicker_plus/js/*',
-                               'templates/bootstrap_datepicker_plus/*']}
-
-install_requires = \
-['Django>=2,<5', 'pydantic', 'typing-extensions']
-
-setup_kwargs = {
-    'name': 'django-bootstrap-datepicker-plus',
-    'version': '5.0.3',
-    'description': 'Bootstrap3/Bootstrap4/Bootstrap5 DatePickerInput, TimePickerInput, DateTimePickerInput, MonthPickerInput, YearPickerInput',
-    'long_description': '########################################\ndjango-bootstrap-datepicker-plus\n########################################\n\nThis django widget contains Bootstrap 3, Bootstrap 4 and Bootstrap 5\nDate-Picker, Time-Picker, DateTime-Picker, Month-Picker and Year-Picker input\nwith date-range-picker functionality for django version >= 2.0.\nThe widget implements `bootstrap-datetimepicker v4 <https://getdatepicker.com/4/>`_\nto show bootstrap-datepicker in django model forms and custom forms\nwhich can be configured easily for date-range selection.\n\nIf you are not using Bootstrap use `django-flatpickr <https://github.com/monim67/django-flatpickr>`_ instead.\n\n|  |build-status| |docs-status| |coverage|\n|  |pyversions| |djversions| |license|\n\n|  |date-picker-image| |datetime-picker-image| |time-picker-image|\n\n\n\n********************\nDemo\n********************\n\n- `With Bootstrap 3 <https://monim67.github.io/django-bootstrap-datepicker-plus/demo/bootstrap3/>`_\n- `With Bootstrap 4 <https://monim67.github.io/django-bootstrap-datepicker-plus/demo/bootstrap4/>`_\n- `With Bootstrap 5 <https://monim67.github.io/django-bootstrap-datepicker-plus/demo/bootstrap5/>`_\n\n\n\n********************\nGetting Started\n********************\n\n- Follow the `Getting Started doc <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Getting_Started.html>`_.\n- Head over to `Usage <#usage>`_ section to see how to use it in forms and views.\n- Read detailed `Documentation on ReadTheDocs <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/>`_\n- Looks complex to get started? Follow a `Quick Walkthrough Tutorial <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Walkthrough.html>`_\n- Getting errors? See `Troubleshoot instructions <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Troubleshooting.html>`_\n\n\n\n********************\nUsage\n********************\n\n\n++++++++++++++++++++++++++++++\nUsage in Generic View\n++++++++++++++++++++++++++++++\n\n.. code:: python\n\n    # File: views.py\n    from bootstrap_datepicker_plus.widgets import DateTimePickerInput\n    from django.views import generic\n    from .models import Question\n\n    class CreateView(generic.edit.CreateView):\n        model = Question\n        fields = ["question_text", "pub_date"]\n        def get_form(self):\n            form = super().get_form()\n            form.fields["pub_date"].widget = DateTimePickerInput()\n            return form\n\n\n++++++++++++++++++++++++++++++\nAdvanced Usage\n++++++++++++++++++++++++++++++\n\n- `Usage in Custom Form <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Usage.html#custom-form-usage>`_\n- `Usage in Model Form <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Usage.html#model-form-usage>`_\n- `Usage doc <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Usage.html>`_\n\n\n++++++++++++++++++++++++++++++\nTypes of DatePickers\n++++++++++++++++++++++++++++++\n\nThe widget contains all types of date-picker you may ever need.\n\n.. code:: python\n\n    # File: forms.py\n    from bootstrap_datepicker_plus.widgets import DatePickerInput, TimePickerInput, DateTimePickerInput, MonthPickerInput, YearPickerInput\n    from django import forms\n\n    class EventForm(forms.ModelForm):\n        class Meta:\n            model = Event\n            fields = ["start_date", "start_time", "start_datetime", "start_month", "start_year"]\n            widgets = {\n                "start_date": DatePickerInput(),\n                "start_time": TimePickerInput(),\n                "start_datetime": DateTimePickerInput(),\n                "start_month": MonthPickerInput(),\n                "start_year": YearPickerInput(),\n            }\n\n\n++++++++++++++++++++++++++++++\nImplement date-range-picker\n++++++++++++++++++++++++++++++\n\nDatePickers can be linked to select a date-range or time-range.\n\n.. code:: python\n\n    # File: forms.py\n    from bootstrap_datepicker_plus.widgets import DatePickerInput, TimePickerInput\n    from django import forms\n\n    class EventForm(forms.ModelForm):\n        class Meta:\n            model = Event\n            fields = ["name", "start_date", "end_date", "start_time", "end_time"]\n            widgets = {\n                "start_date": DatePickerInput(),\n                "end_date": DatePickerInput(range_from="start_date"),\n                "start_time": TimePickerInput(),\n                "end_time": TimePickerInput(range_from="start_time"),\n            }\n\n\n++++++++++++++++++++++++++++++\nCustomization\n++++++++++++++++++++++++++++++\n\n- `Customize date format, language <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/customization.html>`_\n- `Use custom template for widget input <https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/Template_Customizing.html>`_\n\n\n********************\nContributing\n********************\n\n- `CONTRIBUTING.md <https://github.com/monim67/django-bootstrap-datepicker-plus/blob/master/.github/CONTRIBUTING.md>`_.\n- `CODE_OF_CONDUCT.md <https://github.com/monim67/django-bootstrap-datepicker-plus/blob/master/.github/CODE_OF_CONDUCT.md>`_.\n\n********************\nLicense\n********************\n\nThis project is licensed under `MIT LICENSE <https://github.com/monim67/django-bootstrap-datepicker-plus/blob/master/LICENSE>`_ file for details.\n\n********************\nAcknowledgments\n********************\n\nThis project implements `Eonasdan/bootstrap-datetimepicker <https://github.com/Eonasdan/bootstrap-datetimepicker>`_ to display date-pickers.\nThe project was initially forked from `pbucher/django-bootstrap-datepicker <https://github.com/pbucher/django-bootstrap-datepicker>`_ and\nlater reworked completely under MIT Licence.\n\n\n|buymeacoffee|\n\n\n.. |date-picker-image| image:: https://raw.githubusercontent.com/monim67/django-bootstrap-datepicker-plus/26d89a744d403a895422313a48c02885c4718251/images/date-picker.png\n    :alt: Date-picker\n    :width: 218px\n    :height: 280px\n\n.. |datetime-picker-image| image:: https://raw.githubusercontent.com/monim67/django-bootstrap-datepicker-plus/26d89a744d403a895422313a48c02885c4718251/images/datetime-picker.png\n    :alt: Datetime-picker\n    :width: 218px\n    :height: 280px\n\n.. |time-picker-image| image:: https://raw.githubusercontent.com/monim67/django-bootstrap-datepicker-plus/26d89a744d403a895422313a48c02885c4718251/images/time-picker.png\n    :alt: Time-picker\n    :width: 218px\n    :height: 280px\n\n.. |build-status| image:: https://github.com/monim67/django-bootstrap-datepicker-plus/actions/workflows/build.yml/badge.svg?event=push\n    :target: https://github.com/monim67/django-bootstrap-datepicker-plus/actions/workflows/build.yml\n    :alt: Build Status\n    :height: 20px\n\n.. |docs-status| image:: https://readthedocs.org/projects/django-bootstrap-datepicker-plus/badge/?version=latest\n    :target: https://django-bootstrap-datepicker-plus.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n    :height: 20px\n\n.. |coverage| image:: https://coveralls.io/repos/github/monim67/django-bootstrap-datepicker-plus/badge.svg?branch=master\n    :target: https://coveralls.io/github/monim67/django-bootstrap-datepicker-plus?branch=master\n    :alt: Coverage Status\n    :height: 20px\n\n.. |pyversions| image:: https://img.shields.io/pypi/pyversions/django-bootstrap-datepicker-plus.svg\n    :target: https://pypi.python.org/pypi/django-bootstrap-datepicker-plus\n    :alt: Python Versions\n    :height: 20px\n\n.. |djversions| image:: https://img.shields.io/pypi/djversions/django-bootstrap-datepicker-plus.svg\n    :target: https://pypi.python.org/pypi/django-bootstrap-datepicker-plus\n    :alt: DJango Versions\n    :height: 20px\n\n.. |license| image:: https://img.shields.io/pypi/l/django-bootstrap-datepicker-plus.svg\n    :target: https://pypi.python.org/pypi/django-bootstrap-datepicker-plus\n    :alt: Licence\n    :height: 20px\n\n.. |buymeacoffee| image:: https://cdn.buymeacoffee.com/buttons/v2/default-orange.png\n   :target: https://www.buymeacoffee.com/monim67\n   :alt: Buy Me A Coffee\n   :height: 48px\n',
-    'author': 'Munim Munna',
-    'author_email': '6266677+monim67@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/monim67/django-bootstrap-datepicker-plus',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

