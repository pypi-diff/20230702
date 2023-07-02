# Comparing `tmp/fiftyone_pipeline_core-4.4.7.0.tar.gz` & `tmp/fiftyone_pipeline_core-4.4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_pipeline_core-4.4.7.0.tar", last modified: Thu Jun 29 01:46:51 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_core-4.4.8.0.tar", last modified: Sun Jul  2 01:56:21 2023, max compression
```

## Comparing `fiftyone_pipeline_core-4.4.7.0.tar` & `fiftyone_pipeline_core-4.4.8.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:51.863531 fiftyone_pipeline_core-4.4.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-29 01:46:51.863531 fiftyone_pipeline_core-4.4.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:51.863531 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/JavaScriptResource.mustache
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/aspectproperty_value.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2078 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3433 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/elementdata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/elementdata_dictionary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3011 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/evidence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2427 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/evidence_keyfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8094 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/flowdata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4770 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/flowelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/flowerror.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/javascriptbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/jsonbundler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3046 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/messages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5057 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6440 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/pipelinebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/sequenceelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/setheaderelement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2934 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:51.863531 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-29 01:46:51.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-29 01:46:51.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:46:51.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 01:46:51.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 01:46:51.000000 fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 01:46:51.863531 fiftyone_pipeline_core-4.4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-29 01:46:45.000000 fiftyone_pipeline_core-4.4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/JavaScriptResource.mustache
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/aspectproperty_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/elementdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/elementdata_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/evidence_keyfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/javascriptbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/jsonbundler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/pipelinebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/sequenceelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/setheaderelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/setup.py
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/PKG-INFO` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fiftyone_pipeline_core
-Version: 4.4.7.0
+Name: fiftyone-pipeline-core
+Version: 4.4.8.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package definds the essential components of the Pipeline API such as flow elements, flow data and evidence. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/JavaScriptResource.mustache` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/JavaScriptResource.mustache`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/aspectproperty_value.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/aspectproperty_value.py`

 * *Files 4% similar despite different names*

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
 
 
 class AspectPropertyValue(object):
     
     """!
     An AspectPropertyValue is a wrapper for a value
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py`

 * *Files 7% similar despite different names*

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
 
 from .evidence_keyfilter import EvidenceKeyFilter
 
 
 class BasicListEvidenceKeyFilter(EvidenceKeyFilter):
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/elementdata.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/elementdata.py`

 * *Files 4% similar despite different names*

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
 
 
 class ElementData(object):
 
     """!
     Core ElementData class
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/elementdata_dictionary.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/elementdata_dictionary.py`

 * *Files 4% similar despite different names*

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
 
 from .elementdata import ElementData
 
 
 class ElementDataDictionary(ElementData):
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/evidence.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/evidence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # *********************************************************************
 # This Original Work is copyright of 51 Degrees Mobile Experts Limited.
-# Copyright 2022 51 Degrees Mobile Experts Limited, Davidson House,
+# Copyright 2023 51 Degrees Mobile Experts Limited, Davidson House,
 # Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
 #
 # This Original Work is licensed under the European Union Public Licence
 # (EUPL) v.1.2 and is subject to its terms as set out below.
 #
 # If a copy of the EUPL was not distributed with this file, You can obtain
 # one at https://opensource.org/licenses/EUPL-1.2.
 #
 # The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
 # amended by the European Commission) shall be deemed incompatible for
 # the purposes of the Work and the provisions of the compatibility
 # clause in Article 5 of the EUPL shall not apply.
-# 
-# If using the Work as, or as part of, a network application, by 
+#
+# If using the Work as, or as part of, a network application, by
 # including the attribution notice(s) required under Article 5 of the EUPL
-# in the end user terms of the application under an appropriate heading, 
+# in the end user terms of the application under an appropriate heading,
 # such notice(s) shall fulfill the requirements of that article.
 # ********************************************************************* 
 
 
 class Evidence:
 
     def __init__(self, flowdata):
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/evidence_keyfilter.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/evidence_keyfilter.py`

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
 
 
 class EvidenceKeyFilter:
 
     """!
     An EvidenceKeyFilter is attached to a FlowElement and is used to check
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/flowdata.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowdata.py`

 * *Files 1% similar despite different names*

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
 
 from .evidence import Evidence
 from .flowerror import FlowError
 from .messages import Messages	
 import traceback
 import sys
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/flowelement.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowelement.py`

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
 
 from .evidence_keyfilter import EvidenceKeyFilter
 
 
 class FlowElement(object):
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/flowerror.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowerror.py`

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
 
 class FlowError:
 
     """!
     An error that occurred during the processing of an element.
     """
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/javascriptbuilder.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/javascriptbuilder.py`

 * *Files 2% similar despite different names*

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
 
 
 from .flowelement import FlowElement
 from .evidence_keyfilter import EvidenceKeyFilter
 from .elementdata_dictionary import ElementDataDictionary
 import os
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/jsonbundler.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/jsonbundler.py`

 * *Files 2% similar despite different names*

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
 
 from .flowelement import FlowElement
 from .elementdata_dictionary import ElementDataDictionary
 
 class JSONBundlerElement(FlowElement):
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/logger.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/logger.py`

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
 
 from datetime import datetime
 import logging
 
 class Logger:
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/messages.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/messages.py`

 * *Files 11% similar despite different names*

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
 
  # Messages which may be reused for various property exceptions.
 
 class Messages():
 
     # Property does not start with SetHeader. This takes the name of a property
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/pipeline.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # *********************************************************************
 # This Original Work is copyright of 51 Degrees Mobile Experts Limited.
-# Copyright 2022 51 Degrees Mobile Experts Limited, Davidson House,
+# Copyright 2023 51 Degrees Mobile Experts Limited, Davidson House,
 # Forbury Square, Reading, Berkshire, United Kingdom RG1 3EU.
 #
 # This Original Work is licensed under the European Union Public Licence
 # (EUPL) v.1.2 and is subject to its terms as set out below.
 #
 # If a copy of the EUPL was not distributed with this file, You can obtain
 # one at https://opensource.org/licenses/EUPL-1.2.
 #
 # The 'Compatible Licences' set out in the Appendix to the EUPL (as may be
 # amended by the European Commission) shall be deemed incompatible for
 # the purposes of the Work and the provisions of the compatibility
 # clause in Article 5 of the EUPL shall not apply.
-# 
-# If using the Work as, or as part of, a network application, by 
+#
+# If using the Work as, or as part of, a network application, by
 # including the attribution notice(s) required under Article 5 of the EUPL
-# in the end user terms of the application under an appropriate heading, 
+# in the end user terms of the application under an appropriate heading,
 # such notice(s) shall fulfill the requirements of that article.
-# ********************************************************************* 
+# ********************************************************************* 
 
 from .flowdata import FlowData
 from .logger import Logger
 
 class Pipeline:
 
     """!
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/pipelinebuilder.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/pipelinebuilder.py`

 * *Files 2% similar despite different names*

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
 
 from .pipeline import Pipeline
 from .logger import Logger
 from .javascriptbuilder import JavascriptBuilderElement
 from .jsonbundler import JSONBundlerElement
 from .sequenceelement import SequenceElement
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/sequenceelement.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/sequenceelement.py`

 * *Files 15% similar despite different names*

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
 
 
 from .flowelement import FlowElement
 from .evidence_keyfilter import EvidenceKeyFilter
 import uuid
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/setheaderelement.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/setheaderelement.py`

 * *Files 1% similar despite different names*

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
 
 from .flowelement import FlowElement
 from .elementdata_dictionary import ElementDataDictionary
 from .messages import Messages
 import re
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core/web.py` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/web.py`

 * *Files 4% similar despite different names*

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
 
 from flask import request
 
 def webevidence(request):
 
     """!
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core.egg-info/PKG-INFO` & `fiftyone_pipeline_core-4.4.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fiftyone-pipeline-core
-Version: 4.4.7.0
+Name: fiftyone_pipeline_core
+Version: 4.4.8.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package definds the essential components of the Pipeline API such as flow elements, flow data and evidence. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_core-4.4.7.0/fiftyone_pipeline_core.egg-info/SOURCES.txt` & `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.7.0/setup.py` & `fiftyone_pipeline_core-4.4.8.0/setup.py`

 * *Files 4% similar despite different names*

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

