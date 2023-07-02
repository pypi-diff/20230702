# Comparing `tmp/foursight-3.5.0.1b7.tar.gz` & `tmp/foursight-3.5.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-3.5.0.1b7.tar", max compression
+gzip compressed data, was "foursight-3.5.0.2b1.tar", max compression
```

## Comparing `foursight-3.5.0.1b7.tar` & `foursight-3.5.0.2b1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.5.0.1b7/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.5.0.1b7/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.5.0.1b7/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.5.0.1b7/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    54459 2023-06-08 17:18:53.343808 foursight-3.5.0.1b7/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.5.0.1b7/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    60950 2023-06-08 17:18:53.344867 foursight-3.5.0.1b7/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.5.0.1b7/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.5.0.1b7/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.5.0.1b7/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.5.0.1b7/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    15663 2023-06-09 17:46:33.623749 foursight-3.5.0.1b7/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.5.0.1b7/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.5.0.1b7/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.5.0.1b7/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.5.0.1b7/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.5.0.1b7/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.5.0.1b7/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.5.0.1b7/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45209 2023-04-27 02:48:56.047051 foursight-3.5.0.1b7/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.5.0.1b7/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.5.0.1b7/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   137874 2023-06-16 16:42:25.062533 foursight-3.5.0.1b7/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.5.0.1b7/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.5.0.1b7/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1269 2023-06-16 21:23:19.676865 foursight-3.5.0.1b7/pyproject.toml
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 foursight-3.5.0.1b7/setup.py
--rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 foursight-3.5.0.1b7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:59:14.705392 foursight-3.5.0.2b1/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-01-19 14:12:17.947754 foursight-3.5.0.2b1/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1055 2023-03-29 20:27:15.171164 foursight-3.5.0.2b1/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2023-01-19 14:12:17.952115 foursight-3.5.0.2b1/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    54459 2023-06-08 17:18:53.343808 foursight-3.5.0.2b1/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2023-01-19 14:12:17.956201 foursight-3.5.0.2b1/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    60950 2023-06-08 17:18:53.344867 foursight-3.5.0.2b1/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37766 2023-01-19 14:12:17.963001 foursight-3.5.0.2b1/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0    11548 2023-01-19 14:12:17.965655 foursight-3.5.0.2b1/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-01-25 11:36:46.617974 foursight-3.5.0.2b1/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 14:12:17.970674 foursight-3.5.0.2b1/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    15663 2023-06-09 17:46:33.623749 foursight-3.5.0.2b1/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2023-01-19 14:12:17.974848 foursight-3.5.0.2b1/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    44428 2023-01-19 14:12:17.975418 foursight-3.5.0.2b1/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95229 2023-01-19 14:12:17.978748 foursight-3.5.0.2b1/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17372 2023-01-19 14:12:17.979325 foursight-3.5.0.2b1/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2023-01-19 14:12:17.979607 foursight-3.5.0.2b1/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    97361 2023-01-19 14:12:17.983575 foursight-3.5.0.2b1/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 14:12:17.989004 foursight-3.5.0.2b1/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45209 2023-04-27 02:48:56.047051 foursight-3.5.0.2b1/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   127978 2023-01-26 16:17:00.941264 foursight-3.5.0.2b1/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    43470 2023-01-19 14:12:18.009971 foursight-3.5.0.2b1/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   137844 2023-06-29 20:53:05.170451 foursight-3.5.0.2b1/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      621 2023-03-29 20:27:15.171432 foursight-3.5.0.2b1/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      316 2023-03-29 19:16:47.518681 foursight-3.5.0.2b1/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1291 2023-07-01 18:14:04.697232 foursight-3.5.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 foursight-3.5.0.2b1/setup.py
+-rw-r--r--   0        0        0     1084 1970-01-01 00:00:00.000000 foursight-3.5.0.2b1/PKG-INFO
```

### Comparing `foursight-3.5.0.1b7/LICENSE.txt` & `foursight-3.5.0.2b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/app_utils.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/check_schedules.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/check_setup.json` & `foursight-3.5.0.2b1/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/audit_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/badge_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/es_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/header_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/system_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from dcicutils.boto_s3 import boto_s3_resource
 from dcicutils import ff_utils
 from dcicutils.env_utils import prod_bucket_env_for_app
+import boto3
 import re
 import requests
 import json
 import datetime
 import time
 import itertools
 import random
@@ -1565,15 +1565,15 @@
 @action_function()
 def patch_states_files_higlass_defaults(connection, **kwargs):
     action = ActionResult(connection, 'patch_states_files_higlass_defaults')
     check_res = action.get_associated_check_result(kwargs)
     action_logs = {'patch_success': [], 'patch_failure': [], 'missing_ref_file': []}
     total_patches = check_res['full_output']['to_add']
 
-    s3 = boto_s3_resource()
+    s3 = boto3.resource('s3')
     bucket = s3.Bucket('elasticbeanstalk-%s-files' % prod_bucket_env_for_app())
 
     query = '/search/?type=FileReference'
     all_ref_files = ff_utils.search_metadata(query, key=connection.ff_keys)
     ref_files_tags = {}
     for ref_file in all_ref_files:
         if ref_file.get('tags'):
@@ -2397,15 +2397,15 @@
     action.output = action_logs
     return action
 
 
 def get_oh_google_sheet():
     # GET KEY FROM S3 To Access
     # TODO: encrypt the key same as foursight key and use same function to fetch it
-    s3 = boto_s3_resource()
+    s3 = boto3.resource('s3')
     obj = s3.Object('elasticbeanstalk-fourfront-webprod-system', 'DCICjupgoogle.json')
     cont = obj.get()['Body'].read().decode()
     key_dict = json.loads(cont)
     SCOPES = 'https://www.googleapis.com/auth/spreadsheets'
     creds = ServiceAccountCredentials.from_json_keyfile_dict(key_dict, SCOPES)
     gc = gspread.authorize(creds)
     # Get the google sheet information
```

### Comparing `foursight-3.5.0.1b7/chalicelib_fourfront/package.py` & `foursight-3.5.0.2b1/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-3.5.0.1b7/pyproject.toml` & `foursight-3.5.0.2b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "foursight"
-version = "3.5.0.1b7"
+version = "3.5.0.2b1"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.10"
-dcicutils = "7.5.1.1b1"
+#dcicutils = "^7.5.1"
+dcicutils = "7.6.0.1b4"
 click = "^7.1.2"
 PyJWT = "^2.5.0"
 Jinja2 = "2.10.1"
 MarkupSafe = "1.1.1"
 google-api-python-client = "^1.7.4"
 geocoder = "1.38.1"
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 tibanna_ff = ">=0.22.5"
 ## adding foursight-core
 # use below for deployment
-foursight-core = "4.3.0.1b8"
+foursight-core = "4.3.0.2b1"
 # use below for tests but not for deployment
 # foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="master" }
 pytest = "5.1.2"
 gspread = ">=3.6.0"
 oauth2client = ">=4.1.3"
 pandas = ">=1.1.4"
```

### Comparing `foursight-3.5.0.1b7/setup.py` & `foursight-3.5.0.2b1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 {'': ['*']}
 
 install_requires = \
 ['Jinja2==2.10.1',
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'click>=7.1.2,<8.0.0',
- 'dcicutils==7.5.1.1b1',
+ 'dcicutils==7.6.0.1b4',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
- 'foursight-core==4.3.0.1b8',
+ 'foursight-core==4.3.0.2b1',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.7.4,<2.0.0',
  'gspread>=3.6.0',
  'oauth2client>=4.1.3',
  'pandas>=1.1.4',
  'pytest==5.1.2',
@@ -34,15 +34,15 @@
                      'encrypt-accounts-file = '
                      'foursight_core.scripts.encrypt_accounts_file:main',
                      'publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight',
-    'version': '3.5.0.1b7',
+    'version': '3.5.0.2b1',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight-3.5.0.1b7/PKG-INFO` & `foursight-3.5.0.2b1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 3.5.0.1b7
+Version: 3.5.0.2b1
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (==2.10.1)
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: dcicutils (==7.5.1.1b1)
+Requires-Dist: dcicutils (==7.6.0.1b4)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==4.3.0.1b8)
+Requires-Dist: foursight-core (==4.3.0.2b1)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.7.4,<2.0.0)
 Requires-Dist: gspread (>=3.6.0)
 Requires-Dist: oauth2client (>=4.1.3)
 Requires-Dist: pandas (>=1.1.4)
 Requires-Dist: pytest (==5.1.2)
```

