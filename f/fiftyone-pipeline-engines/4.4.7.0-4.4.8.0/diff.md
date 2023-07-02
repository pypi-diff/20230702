# Comparing `tmp/fiftyone_pipeline_engines-4.4.7.0.tar.gz` & `tmp/fiftyone_pipeline_engines-4.4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_pipeline_engines-4.4.7.0.tar", last modified: Thu Jun 29 01:46:52 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_engines-4.4.8.0.tar", last modified: Sun Jul  2 01:56:21 2023, max compression
```

## Comparing `fiftyone_pipeline_engines-4.4.7.0.tar` & `fiftyone_pipeline_engines-4.4.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:52.147539 fiftyone_pipeline_engines-4.4.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-29 01:46:52.147539 fiftyone_pipeline_engines-4.4.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:52.147539 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2902 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/aspectdata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2494 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/aspectdata_dictionary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2111 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/basic_dictionary_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/datafile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/datafile_update_service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1938 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/datakeyed_cache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4548 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/missingproperty_service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2146 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:46:52.147539 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 01:46:52.000000 fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 01:46:52.147539 fiftyone_pipeline_engines-4.4.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-29 01:46:45.000000 fiftyone_pipeline_engines-4.4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/aspectdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/aspectdata_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/basic_dictionary_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datafile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datafile_update_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datakeyed_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/missingproperty_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 01:56:21.000000 fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:56:21.574805 fiftyone_pipeline_engines-4.4.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-02 01:56:16.000000 fiftyone_pipeline_engines-4.4.8.0/setup.py
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/PKG-INFO` & `fiftyone_pipeline_engines-4.4.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_pipeline_engines
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

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/aspectdata.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/aspectdata.py`

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
 
 from fiftyone_pipeline_core.elementdata import ElementData
 
 from fiftyone_pipeline_engines.missingproperty_service import MissingPropertyService
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/aspectdata_dictionary.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/aspectdata_dictionary.py`

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
 
 from .aspectdata import AspectData
 
 class AspectDataDictionary(AspectData):
 
     """!
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/basic_dictionary_cache.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/basic_dictionary_cache.py`

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
 
 from fiftyone_pipeline_engines.datakeyed_cache import DataKeyedCache
 
 class BasicDictionaryCache(DataKeyedCache):
 
     """!
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/datafile.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datafile.py`

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
 
 import tempfile
 import datetime
 
 class DataFile():
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/datafile_update_service.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datafile_update_service.py`

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
 
 from enum import Enum
 import gzip
 import shutil
 import os
 import random
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/datakeyed_cache.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/datakeyed_cache.py`

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
 
 
 class DataKeyedCache(object):
 
     """!
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/engine.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/engine.py`

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
 
 from fiftyone_pipeline_core.flowelement import FlowElement
 from fiftyone_pipeline_engines.datafile_update_service import DataFileUpdateService
 
 import json
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/lru_cache.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/lru_cache.py`

 * *Files 12% similar despite different names*

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
 
 from .datakeyed_cache import DataKeyedCache
 
 from cachetools import LRUCache
 
 class LRUEngineCache(DataKeyedCache):
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/missingproperty_service.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/missingproperty_service.py`

 * *Files 12% similar despite different names*

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
 
 
 class MissingPropertyService():
     
     """!
     A missing property service runs when a property is not available in the
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines/tracker.py` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines/tracker.py`

 * *Files 9% similar despite different names*

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
 
 from .datakeyed_cache import DataKeyedCache
 
 class Tracker(DataKeyedCache):
     
     """!
```

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines.egg-info/PKG-INFO` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone-pipeline-engines
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

### Comparing `fiftyone_pipeline_engines-4.4.7.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt` & `fiftyone_pipeline_engines-4.4.8.0/fiftyone_pipeline_engines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_engines-4.4.7.0/setup.py` & `fiftyone_pipeline_engines-4.4.8.0/setup.py`

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
 
 import setuptools
 import os
 import io
 
 # Read a text file and return the content as a string.
```

