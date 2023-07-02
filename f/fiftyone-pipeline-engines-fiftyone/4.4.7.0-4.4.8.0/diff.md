# Comparing `tmp/fiftyone_pipeline_engines_fiftyone-4.4.7.0.tar.gz` & `tmp/fiftyone_pipeline_engines_fiftyone-4.4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_pipeline_engines_fiftyone-4.4.7.0.tar", last modified: Thu Jun 29 01:46:52 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_engines_fiftyone-4.4.8.0.tar", last modified: Sun Jul  2 01:56:21 2023, max compression
```

## Comparing `fiftyone_pipeline_engines_fiftyone-4.4.7.0.tar` & `fiftyone_pipeline_engines_fiftyone-4.4.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:52.399546 fiftyone_pipeline_engines_fiftyone-4.4.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-29 01:46:52.399546 fiftyone_pipeline_engines_fiftyone-4.4.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:52.399546 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14874 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone/share_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:52.399546 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 01:46:52.399546 fiftyone_pipeline_engines_fiftyone-4.4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines_fiftyone-4.4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.770810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-02 01:56:21.770810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.766810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.770810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:56:21.770810 fiftyone_pipeline_engines_fiftyone-4.4.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines_fiftyone-4.4.8.0/setup.py
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.7.0/PKG-INFO` & `fiftyone_pipeline_engines_fiftyone-4.4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_pipeline_engines_fiftyone
-Version: 4.4.7.0
+Version: 4.4.8.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone/share_usage.py` & `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage.py`

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
 
 from __future__ import absolute_import
 import random
 import threading
 from fiftyone_pipeline_engines.engine import Engine
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py` & `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage_evidencekeyfilter.py`

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
 
 from fiftyone_pipeline_core.basiclist_evidence_keyfilter import BasicListEvidenceKeyFilter
 
 class ShareUsageEvidenceKeyFilter(BasicListEvidenceKeyFilter):
     """
     The ShareUsageEvidenceKeyFilter filters out all evidence
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py` & `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone/share_usage_tracker.py`

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
 
 from fiftyone_pipeline_engines.tracker import Tracker
 from cachetools import LRUCache
 
 import time
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO` & `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-pipeline-engines-fiftyone
-Version: 4.4.7.0
+Version: 4.4.8.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). It includes a ShareUsage engine that sends usage data to 51Degrees in zipped batches.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.7.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt` & `fiftyone_pipeline_engines_fiftyone-4.4.8.0/fiftyone_pipeline_engines_fiftyone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines_fiftyone-4.4.7.0/setup.py` & `fiftyone_pipeline_engines_fiftyone-4.4.8.0/setup.py`

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
 
 import setuptools
 import os
 import io
 
 def read(file_name):
```

