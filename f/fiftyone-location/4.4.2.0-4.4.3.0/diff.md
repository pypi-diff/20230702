# Comparing `tmp/fiftyone_location-4.4.2.0.tar.gz` & `tmp/fiftyone_location-4.4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_location-4.4.2.0.tar", last modified: Thu Jun 29 01:28:49 2023, max compression
+gzip compressed data, was "fiftyone_location-4.4.3.0.tar", last modified: Sun Jul  2 01:29:11 2023, max compression
```

## Comparing `fiftyone_location-4.4.2.0.tar` & `fiftyone_location-4.4.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:28:49.815375 fiftyone_location-4.4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-29 01:28:49.815375 fiftyone_location-4.4.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:28:49.815375 fiftyone_location-4.4.2.0/fiftyone_location/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:28:44.000000 fiftyone_location-4.4.2.0/fiftyone_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-29 01:28:44.000000 fiftyone_location-4.4.2.0/fiftyone_location/location_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-29 01:28:44.000000 fiftyone_location-4.4.2.0/fiftyone_location/location_pipelinebuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:28:49.815375 fiftyone_location-4.4.2.0/fiftyone_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-29 01:28:49.000000 fiftyone_location-4.4.2.0/fiftyone_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-29 01:28:49.000000 fiftyone_location-4.4.2.0/fiftyone_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:28:49.000000 fiftyone_location-4.4.2.0/fiftyone_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-29 01:28:49.000000 fiftyone_location-4.4.2.0/fiftyone_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 01:28:49.000000 fiftyone_location-4.4.2.0/fiftyone_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 01:28:49.815375 fiftyone_location-4.4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-29 01:28:44.000000 fiftyone_location-4.4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:29:11.225369 fiftyone_location-4.4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-02 01:29:11.225369 fiftyone_location-4.4.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:29:11.221369 fiftyone_location-4.4.3.0/fiftyone_location/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 01:29:01.000000 fiftyone_location-4.4.3.0/fiftyone_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-02 01:29:01.000000 fiftyone_location-4.4.3.0/fiftyone_location/location_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-02 01:29:01.000000 fiftyone_location-4.4.3.0/fiftyone_location/location_pipelinebuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:29:11.225369 fiftyone_location-4.4.3.0/fiftyone_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-02 01:29:11.000000 fiftyone_location-4.4.3.0/fiftyone_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-02 01:29:11.000000 fiftyone_location-4.4.3.0/fiftyone_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:29:11.000000 fiftyone_location-4.4.3.0/fiftyone_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-02 01:29:11.000000 fiftyone_location-4.4.3.0/fiftyone_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 01:29:11.000000 fiftyone_location-4.4.3.0/fiftyone_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:29:11.225369 fiftyone_location-4.4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-02 01:29:01.000000 fiftyone_location-4.4.3.0/setup.py
```

### Comparing `fiftyone_location-4.4.2.0/PKG-INFO` & `fiftyone_location-4.4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_location
-Version: 4.4.2.0
+Version: 4.4.3.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This repository contains the geo-location engines for the Python implementation of the Pipeline API.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_location-4.4.2.0/fiftyone_location/location_cloud.py` & `fiftyone_location-4.4.3.0/fiftyone_location/location_cloud.py`

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
 
 from fiftyone_pipeline_cloudrequestengine.cloudengine import CloudEngine
 
 class LocationCloud(CloudEngine):
     """!
     The location cloud engine requires the 51Degrees
```

### Comparing `fiftyone_location-4.4.2.0/fiftyone_location/location_pipelinebuilder.py` & `fiftyone_location-4.4.3.0/fiftyone_location/location_pipelinebuilder.py`

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
 
 from fiftyone_pipeline_core.pipelinebuilder import PipelineBuilder
 from fiftyone_pipeline_cloudrequestengine.cloudrequestengine import CloudRequestEngine
 from .location_cloud import LocationCloud
 
 class LocationPipelineBuilder(PipelineBuilder):
```

### Comparing `fiftyone_location-4.4.2.0/fiftyone_location.egg-info/PKG-INFO` & `fiftyone_location-4.4.3.0/fiftyone_location.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-location
-Version: 4.4.2.0
+Version: 4.4.3.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This repository contains the geo-location engines for the Python implementation of the Pipeline API.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_location-4.4.2.0/setup.py` & `fiftyone_location-4.4.3.0/setup.py`

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
 
 import setuptools
 import os
 import io
 
 # Read a text file and return the content as a string.
```

