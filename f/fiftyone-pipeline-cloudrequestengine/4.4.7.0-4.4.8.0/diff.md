# Comparing `tmp/fiftyone_pipeline_cloudrequestengine-4.4.7.0.tar.gz` & `tmp/fiftyone_pipeline_cloudrequestengine-4.4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_pipeline_cloudrequestengine-4.4.7.0.tar", last modified: Thu Jun 29 01:46:52 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_cloudrequestengine-4.4.8.0.tar", last modified: Sun Jul  2 01:56:21 2023, max compression
```

## Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0.tar` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:52.647553 fiftyone_pipeline_cloudrequestengine-4.4.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-29 01:46:52.647553 fiftyone_pipeline_cloudrequestengine-4.4.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:52.647553 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:45.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-29 01:46:45.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/clouddata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-29 01:46:45.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14180 2023-06-29 01:46:45.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-29 01:46:45.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-29 01:46:45.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-29 01:46:45.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/requestclient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:52.647553 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-29 01:46:52.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-29 01:46:52.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:46:52.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 01:46:52.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-29 01:46:52.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 01:46:52.647553 fiftyone_pipeline_cloudrequestengine-4.4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-29 01:46:45.000000 fiftyone_pipeline_cloudrequestengine-4.4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.962814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-02 01:56:21.962814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.958814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/clouddata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/requestclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.962814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 01:56:21.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:56:21.962814 fiftyone_pipeline_cloudrequestengine-4.4.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-02 01:56:16.000000 fiftyone_pipeline_cloudrequestengine-4.4.8.0/setup.py
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/PKG-INFO` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_pipeline_cloudrequestengine
-Version: 4.4.7.0
+Version: 4.4.8.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package extends the flow element class created by the fiftyone-pipeline-core package into a specialized type of flow element called an engine.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/clouddata.py` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/clouddata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# *********************************************************************
-# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
-# Copyright 2022 51 Degrees Mobile Experts Limited, Davidson House,
-# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
-#
-# This Original Work is licensed under the European Union Public Licence
-# (EUPL) v.1.2 and is subject to its terms as set out below.
-#
-# If a copy of the EUPL was not distributed with this file, You can obtain
-# one at https://opensource.org/licenses/EUPL-1.2.
-#
-# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
-# amended by the European Commission) shall be deemed incompatible for
-# the purposes of the Work and the provisions of the compatibility
-# clause in Article 5 of the EUPL shall not apply.
-# 
-# If using the Work as, or as part of, a network application, by 
-# including the attribution notice(s) required under Article 5 of the EUPL
-# in the end user terms of the application under an appropriate heading, 
-# such notice(s) shall fulfill the requirements of that article.
+# *********************************************************************
+# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
+# Copyright 2023 51 Degrees Mobile Experts Limited, Davidson House,
+# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
+#
+# This Original Work is licensed under the European Union Public Licence
+# (EUPL) v.1.2 and is subject to its terms as set out below.
+#
+# If a copy of the EUPL was not distributed with this file, You can obtain
+# one at https://opensource.org/licenses/EUPL-1.2.
+#
+# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
+# amended by the European Commission) shall be deemed incompatible for
+# the purposes of the Work and the provisions of the compatibility
+# clause in Article 5 of the EUPL shall not apply.
+#
+# If using the Work as, or as part of, a network application, by
+# including the attribution notice(s) required under Article 5 of the EUPL
+# in the end user terms of the application under an appropriate heading,
+# such notice(s) shall fulfill the requirements of that article.
 # ********************************************************************* 
 
 from fiftyone_pipeline_engines.aspectdata_dictionary import AspectDataDictionary
 
 from fiftyone_pipeline_engines.missingproperty_service import MissingPropertyService
 
 class OnPremiseMissingPropertyService(MissingPropertyService):
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudengine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# *********************************************************************
-# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
-# Copyright 2022 51 Degrees Mobile Experts Limited, Davidson House,
-# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
-#
-# This Original Work is licensed under the European Union Public Licence
-# (EUPL) v.1.2 and is subject to its terms as set out below.
-#
-# If a copy of the EUPL was not distributed with this file, You can obtain
-# one at https://opensource.org/licenses/EUPL-1.2.
-#
-# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
-# amended by the European Commission) shall be deemed incompatible for
-# the purposes of the Work and the provisions of the compatibility
-# clause in Article 5 of the EUPL shall not apply.
-# 
-# If using the Work as, or as part of, a network application, by 
-# including the attribution notice(s) required under Article 5 of the EUPL
-# in the end user terms of the application under an appropriate heading, 
-# such notice(s) shall fulfill the requirements of that article.
+# *********************************************************************
+# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
+# Copyright 2023 51 Degrees Mobile Experts Limited, Davidson House,
+# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
+#
+# This Original Work is licensed under the European Union Public Licence
+# (EUPL) v.1.2 and is subject to its terms as set out below.
+#
+# If a copy of the EUPL was not distributed with this file, You can obtain
+# one at https://opensource.org/licenses/EUPL-1.2.
+#
+# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
+# amended by the European Commission) shall be deemed incompatible for
+# the purposes of the Work and the provisions of the compatibility
+# clause in Article 5 of the EUPL shall not apply.
+#
+# If using the Work as, or as part of, a network application, by
+# including the attribution notice(s) required under Article 5 of the EUPL
+# in the end user terms of the application under an appropriate heading,
+# such notice(s) shall fulfill the requirements of that article.
 # ********************************************************************* 
 
 from fiftyone_pipeline_engines.engine import Engine
 from fiftyone_pipeline_core.aspectproperty_value import AspectPropertyValue
 
 from .clouddata import CloudData
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudrequestengine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# *********************************************************************
-# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
-# Copyright 2022 51 Degrees Mobile Experts Limited, Davidson House,
-# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
-#
-# This Original Work is licensed under the European Union Public Licence
-# (EUPL) v.1.2 and is subject to its terms as set out below.
-#
-# If a copy of the EUPL was not distributed with this file, You can obtain
-# one at https://opensource.org/licenses/EUPL-1.2.
-#
-# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
-# amended by the European Commission) shall be deemed incompatible for
-# the purposes of the Work and the provisions of the compatibility
-# clause in Article 5 of the EUPL shall not apply.
-# 
-# If using the Work as, or as part of, a network application, by 
-# including the attribution notice(s) required under Article 5 of the EUPL
-# in the end user terms of the application under an appropriate heading, 
-# such notice(s) shall fulfill the requirements of that article.
+# *********************************************************************
+# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
+# Copyright 2023 51 Degrees Mobile Experts Limited, Davidson House,
+# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
+#
+# This Original Work is licensed under the European Union Public Licence
+# (EUPL) v.1.2 and is subject to its terms as set out below.
+#
+# If a copy of the EUPL was not distributed with this file, You can obtain
+# one at https://opensource.org/licenses/EUPL-1.2.
+#
+# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
+# amended by the European Commission) shall be deemed incompatible for
+# the purposes of the Work and the provisions of the compatibility
+# clause in Article 5 of the EUPL shall not apply.
+#
+# If using the Work as, or as part of, a network application, by
+# including the attribution notice(s) required under Article 5 of the EUPL
+# in the end user terms of the application under an appropriate heading,
+# such notice(s) shall fulfill the requirements of that article.
 # ********************************************************************* 
 
 from __future__ import absolute_import
 from fiftyone_pipeline_core.basiclist_evidence_keyfilter import BasicListEvidenceKeyFilter
 from fiftyone_pipeline_engines.engine import Engine
 from fiftyone_pipeline_engines.aspectdata_dictionary import AspectDataDictionary
 from .requestclient import RequestClient
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/cloudrequestexception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# *********************************************************************
-# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
-# Copyright 2022 51 Degrees Mobile Experts Limited, Davidson House,
-# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
-#
-# This Original Work is licensed under the European Union Public Licence
-# (EUPL) v.1.2 and is subject to its terms as set out below.
-#
-# If a copy of the EUPL was not distributed with this file, You can obtain
-# one at https://opensource.org/licenses/EUPL-1.2.
-#
-# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
-# amended by the European Commission) shall be deemed incompatible for
-# the purposes of the Work and the provisions of the compatibility
-# clause in Article 5 of the EUPL shall not apply.
-# 
-# If using the Work as, or as part of, a network application, by 
-# including the attribution notice(s) required under Article 5 of the EUPL
-# in the end user terms of the application under an appropriate heading, 
-# such notice(s) shall fulfill the requirements of that article.
+# *********************************************************************
+# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
+# Copyright 2023 51 Degrees Mobile Experts Limited, Davidson House,
+# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
+#
+# This Original Work is licensed under the European Union Public Licence
+# (EUPL) v.1.2 and is subject to its terms as set out below.
+#
+# If a copy of the EUPL was not distributed with this file, You can obtain
+# one at https://opensource.org/licenses/EUPL-1.2.
+#
+# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
+# amended by the European Commission) shall be deemed incompatible for
+# the purposes of the Work and the provisions of the compatibility
+# clause in Article 5 of the EUPL shall not apply.
+#
+# If using the Work as, or as part of, a network application, by
+# including the attribution notice(s) required under Article 5 of the EUPL
+# in the end user terms of the application under an appropriate heading,
+# such notice(s) shall fulfill the requirements of that article.
 # ********************************************************************* 
 
 """!
     Exception that can be thrown when the available data does not match that
     which is expected.
 """
 class CloudRequestException(Exception):
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/constants.py` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# *********************************************************************
-# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
-# Copyright 2022 51 Degrees Mobile Experts Limited, Davidson House,
-# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
-#
-# This Original Work is licensed under the European Union Public Licence
-# (EUPL) v.1.2 and is subject to its terms as set out below.
-#
-# If a copy of the EUPL was not distributed with this file, You can obtain
-# one at https://opensource.org/licenses/EUPL-1.2.
-#
-# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
-# amended by the European Commission) shall be deemed incompatible for
-# the purposes of the Work and the provisions of the compatibility
-# clause in Article 5 of the EUPL shall not apply.
-# 
-# If using the Work as, or as part of, a network application, by 
-# including the attribution notice(s) required under Article 5 of the EUPL
-# in the end user terms of the application under an appropriate heading, 
-# such notice(s) shall fulfill the requirements of that article.
+# *********************************************************************
+# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
+# Copyright 2023 51 Degrees Mobile Experts Limited, Davidson House,
+# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
+#
+# This Original Work is licensed under the European Union Public Licence
+# (EUPL) v.1.2 and is subject to its terms as set out below.
+#
+# If a copy of the EUPL was not distributed with this file, You can obtain
+# one at https://opensource.org/licenses/EUPL-1.2.
+#
+# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
+# amended by the European Commission) shall be deemed incompatible for
+# the purposes of the Work and the provisions of the compatibility
+# clause in Article 5 of the EUPL shall not apply.
+#
+# If using the Work as, or as part of, a network application, by
+# including the attribution notice(s) required under Article 5 of the EUPL
+# in the end user terms of the application under an appropriate heading,
+# such notice(s) shall fulfill the requirements of that article.
 # ********************************************************************* 
  
 class Constants:
     # Environment variable to set cloud end point
     FOD_CLOUD_API_URL = "FOD_CLOUD_API_URL"
     # Default cloud end point
     BASE_URL_DEFAULT = "https://cloud.51degrees.com/api/v4/"
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine/requestclient.py` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine/requestclient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# *********************************************************************
-# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
-# Copyright 2022 51 Degrees Mobile Experts Limited, Davidson House,
-# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
-#
-# This Original Work is licensed under the European Union Public Licence
-# (EUPL) v.1.2 and is subject to its terms as set out below.
-#
-# If a copy of the EUPL was not distributed with this file, You can obtain
-# one at https://opensource.org/licenses/EUPL-1.2.
-#
-# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
-# amended by the European Commission) shall be deemed incompatible for
-# the purposes of the Work and the provisions of the compatibility
-# clause in Article 5 of the EUPL shall not apply.
-# 
-# If using the Work as, or as part of, a network application, by 
-# including the attribution notice(s) required under Article 5 of the EUPL
-# in the end user terms of the application under an appropriate heading, 
-# such notice(s) shall fulfill the requirements of that article.
+# *********************************************************************
+# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
+# Copyright 2023 51 Degrees Mobile Experts Limited, Davidson House,
+# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
+#
+# This Original Work is licensed under the European Union Public Licence
+# (EUPL) v.1.2 and is subject to its terms as set out below.
+#
+# If a copy of the EUPL was not distributed with this file, You can obtain
+# one at https://opensource.org/licenses/EUPL-1.2.
+#
+# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
+# amended by the European Commission) shall be deemed incompatible for
+# the purposes of the Work and the provisions of the compatibility
+# clause in Article 5 of the EUPL shall not apply.
+#
+# If using the Work as, or as part of, a network application, by
+# including the attribution notice(s) required under Article 5 of the EUPL
+# in the end user terms of the application under an appropriate heading,
+# such notice(s) shall fulfill the requirements of that article.
 # ********************************************************************* 
 
 import requests
 
 class RequestClient:
     def request(self, type, url, content, originHeader):
         return requests.request(type, url, data=content, headers={"Origin":originHeader})
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-pipeline-cloudrequestengine
-Version: 4.4.7.0
+Version: 4.4.8.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package extends the flow element class created by the fiftyone-pipeline-core package into a specialized type of flow element called an engine.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/fiftyone_pipeline_cloudrequestengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_cloudrequestengine-4.4.7.0/setup.py` & `fiftyone_pipeline_cloudrequestengine-4.4.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# *********************************************************************
-# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
-# Copyright 2022 51 Degrees Mobile Experts Limited, Davidson House,
-# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
-#
-# This Original Work is licensed under the European Union Public Licence
-# (EUPL) v.1.2 and is subject to its terms as set out below.
-#
-# If a copy of the EUPL was not distributed with this file, You can obtain
-# one at https://opensource.org/licenses/EUPL-1.2.
-#
-# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
-# amended by the European Commission) shall be deemed incompatible for
-# the purposes of the Work and the provisions of the compatibility
-# clause in Article 5 of the EUPL shall not apply.
-# 
-# If using the Work as, or as part of, a network application, by 
-# including the attribution notice(s) required under Article 5 of the EUPL
-# in the end user terms of the application under an appropriate heading, 
-# such notice(s) shall fulfill the requirements of that article.
+# *********************************************************************
+# This Original Work is copyright of 51 Degrees Mobile Experts Limited.
+# Copyright 2023 51 Degrees Mobile Experts Limited, Davidson House,
+# Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
+#
+# This Original Work is licensed under the European Union Public Licence
+# (EUPL) v.1.2 and is subject to its terms as set out below.
+#
+# If a copy of the EUPL was not distributed with this file, You can obtain
+# one at https://opensource.org/licenses/EUPL-1.2.
+#
+# The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
+# amended by the European Commission) shall be deemed incompatible for
+# the purposes of the Work and the provisions of the compatibility
+# clause in Article 5 of the EUPL shall not apply.
+#
+# If using the Work as, or as part of, a network application, by
+# including the attribution notice(s) required under Article 5 of the EUPL
+# in the end user terms of the application under an appropriate heading,
+# such notice(s) shall fulfill the requirements of that article.
 # ********************************************************************* 
 
 import setuptools
 import os
 import io
 
 # Read a text file and return the content as a string.
```

