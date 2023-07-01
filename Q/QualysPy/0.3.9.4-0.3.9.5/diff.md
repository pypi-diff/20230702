# Comparing `tmp/qualyspy-0.3.9.4.tar.gz` & `tmp/qualyspy-0.3.9.5.tar.gz`

## Comparing `qualyspy-0.3.9.4.tar` & `qualyspy-0.3.9.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/.readthedocs.yaml
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/config-example.ini
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/.vscode/launch.json
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/.vscode/settings.json
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/.vscode/tasks.json
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/debug/build.sh
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/debug/dtd.txt
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/debug/output.txt
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/debug/parse_dtd.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/debug/quickscan.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/debug/remove_cookies.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/debug/test.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/docs/Makefile
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/docs/conf.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/docs/make.bat
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/docs/modules.rst
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/docs/qualyspy.models.rst
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/docs/qualyspy.models.vmdr.rst
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/docs/qualyspy.rst
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/URLS.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/__init__.py
--rw-r--r--   0        0        0    15056 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/base.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/exceptions.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/gav.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/qutils.py
--rw-r--r--   0        0        0     9613 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/vmdr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/sa_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/gav/__init__.py
--rw-r--r--   0        0        0    22850 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/gav/asset_details_orm.py
--rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/gav/asset_details_output.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/vmdr/__init__.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/vmdr/converters.py
--rw-r--r--   0        0        0    12712 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/vmdr/host_list_orm.py
--rw-r--r--   0        0        0    20174 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/vmdr/host_list_output.py
--rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/vmdr/host_list_vm_detection_orm.py
--rw-r--r--   0        0        0    20975 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy/models/vmdr/host_list_vm_detection_output.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/exceptions.py
--rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/qualysapi.py
--rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/qutils.py
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/urls.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/asset_mgmt_tagging/__init__.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/asset_mgmt_tagging/api_input.py
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/asset_mgmt_tagging/asset.py
--rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/asset_mgmt_tagging/tag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/assets/__init__.py
--rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/assets/host_list.py
--rw-r--r--   0        0        0    40850 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/assets/host_list_detection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/certview/__init__.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/certview/certificate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/scan_configuration/__init__.py
--rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/qualyspy-legacy/scan_configuration/knowledgebase.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/requirements/deploy.txt
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/requirements/dev.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/requirements/docs.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/tests/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/tests/gav_test.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/tests/vmdr_test.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/LICENSE
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/README.md
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/pyproject.toml
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 qualyspy-0.3.9.4/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/config-example.ini
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/.vscode/launch.json
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/.vscode/settings.json
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/.vscode/tasks.json
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/debug/build.sh
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/debug/dtd.txt
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/debug/output.txt
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/debug/parse_dtd.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/debug/quickscan.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/debug/remove_cookies.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/debug/test.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/docs/Makefile
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/docs/conf.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/docs/make.bat
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/docs/modules.rst
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/docs/qualyspy.models.rst
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/docs/qualyspy.models.vmdr.rst
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/docs/qualyspy.rst
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/URLS.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/__init__.py
+-rw-r--r--   0        0        0    15042 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/base.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/exceptions.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/gav.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/qutils.py
+-rw-r--r--   0        0        0     9571 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/vmdr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/sa_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/gav/__init__.py
+-rw-r--r--   0        0        0    22850 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/gav/asset_details_orm.py
+-rw-r--r--   0        0        0     7776 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/gav/asset_details_output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/vmdr/__init__.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/vmdr/converters.py
+-rw-r--r--   0        0        0    12712 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/vmdr/host_list_orm.py
+-rw-r--r--   0        0        0    20174 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/vmdr/host_list_output.py
+-rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/vmdr/host_list_vm_detection_orm.py
+-rw-r--r--   0        0        0    20975 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy/models/vmdr/host_list_vm_detection_output.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/exceptions.py
+-rw-r--r--   0        0        0    15305 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/qualysapi.py
+-rw-r--r--   0        0        0    16537 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/qutils.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/urls.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/asset_mgmt_tagging/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/asset_mgmt_tagging/api_input.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/asset_mgmt_tagging/asset.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/asset_mgmt_tagging/tag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/assets/__init__.py
+-rw-r--r--   0        0        0    30142 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/assets/host_list.py
+-rw-r--r--   0        0        0    40850 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/assets/host_list_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/certview/__init__.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/certview/certificate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/scan_configuration/__init__.py
+-rw-r--r--   0        0        0    24210 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/qualyspy-legacy/scan_configuration/knowledgebase.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/requirements/deploy.txt
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/requirements/dev.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/requirements/docs.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/tests/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/tests/gav_test.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/tests/vmdr_test.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/LICENSE
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/README.md
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/pyproject.toml
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 qualyspy-0.3.9.5/PKG-INFO
```

### Comparing `qualyspy-0.3.9.4/.readthedocs.yaml` & `qualyspy-0.3.9.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/.vscode/launch.json` & `qualyspy-0.3.9.5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/.vscode/settings.json` & `qualyspy-0.3.9.5/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/.vscode/tasks.json` & `qualyspy-0.3.9.5/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/debug/dtd.txt` & `qualyspy-0.3.9.5/debug/dtd.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/debug/output.txt` & `qualyspy-0.3.9.5/debug/output.txt`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/debug/parse_dtd.py` & `qualyspy-0.3.9.5/debug/parse_dtd.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/debug/quickscan.py` & `qualyspy-0.3.9.5/debug/quickscan.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/debug/remove_cookies.py` & `qualyspy-0.3.9.5/debug/remove_cookies.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/debug/test.py` & `qualyspy-0.3.9.5/debug/test.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/docs/Makefile` & `qualyspy-0.3.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/docs/conf.py` & `qualyspy-0.3.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/docs/make.bat` & `qualyspy-0.3.9.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/docs/qualyspy.models.vmdr.rst` & `qualyspy-0.3.9.5/docs/qualyspy.models.vmdr.rst`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/docs/qualyspy.rst` & `qualyspy-0.3.9.5/docs/qualyspy.rst`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/base.py` & `qualyspy-0.3.9.5/qualyspy/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         config_file: str = str(os.path.join(os.path.expanduser("~"), ".qualyspy")),
         x_requested_with: str = "QualysPy Python Library",
     ) -> None:
         """Initializes an instance of the QualysAPIBase class.
 
         Args:
             config_file (str, optional): Path to the config file.  Defaults to
-                ~/etc/qualyspy/config.ini.
+                ~/.qualyspy.
             x_requested_with (str, optional): Value to send in the X-Requested-With header.
 
         Raises:
             exceptions.ConfigError: Raised if the config file is missing a required key.
         """
 
         # Read config file
```

### Comparing `qualyspy-0.3.9.4/qualyspy/gav.py` & `qualyspy-0.3.9.5/qualyspy/gav.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/qutils.py` & `qualyspy-0.3.9.5/qualyspy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/vmdr.py` & `qualyspy-0.3.9.5/qualyspy/vmdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,17 +26,15 @@
 
 
 class VmdrAPI(QualysAPIBase):
     """Qualys VMDR API Class.  Contains methods for interacting with the VMDR API."""
 
     def __init__(
         self,
-        config_file: str = str(
-            os.path.join(os.path.expanduser("~"), "etc", "qualyspy", "config.ini")
-        ),
+        config_file: str = str(os.path.join(os.path.expanduser("~"), ".qualyspy")),
         x_requested_with: str = "QualysPy Python Library",
     ) -> None:
         """Initialize the VMDR API Class.
 
         Args:
             config_file (str, optional): Path to config file. Defaults to ~/etc/qualysby/config.ini.
             x_requested_with (str, optional): Value for X-Requested-With header. Defaults to
```

### Comparing `qualyspy-0.3.9.4/qualyspy/models/sa_types.py` & `qualyspy-0.3.9.5/qualyspy/models/sa_types.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/models/gav/asset_details_orm.py` & `qualyspy-0.3.9.5/qualyspy/models/gav/asset_details_orm.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/models/gav/asset_details_output.py` & `qualyspy-0.3.9.5/qualyspy/models/gav/asset_details_output.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/models/vmdr/converters.py` & `qualyspy-0.3.9.5/qualyspy/models/vmdr/converters.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/models/vmdr/host_list_orm.py` & `qualyspy-0.3.9.5/qualyspy/models/vmdr/host_list_orm.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/models/vmdr/host_list_output.py` & `qualyspy-0.3.9.5/qualyspy/models/vmdr/host_list_output.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/models/vmdr/host_list_vm_detection_orm.py` & `qualyspy-0.3.9.5/qualyspy/models/vmdr/host_list_vm_detection_orm.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy/models/vmdr/host_list_vm_detection_output.py` & `qualyspy-0.3.9.5/qualyspy/models/vmdr/host_list_vm_detection_output.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/qualysapi.py` & `qualyspy-0.3.9.5/qualyspy-legacy/qualysapi.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/qutils.py` & `qualyspy-0.3.9.5/qualyspy-legacy/qutils.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/urls.json` & `qualyspy-0.3.9.5/qualyspy-legacy/urls.json`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/asset_mgmt_tagging/api_input.py` & `qualyspy-0.3.9.5/qualyspy-legacy/asset_mgmt_tagging/api_input.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/asset_mgmt_tagging/asset.py` & `qualyspy-0.3.9.5/qualyspy-legacy/asset_mgmt_tagging/asset.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/asset_mgmt_tagging/tag.py` & `qualyspy-0.3.9.5/qualyspy-legacy/asset_mgmt_tagging/tag.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/assets/host_list.py` & `qualyspy-0.3.9.5/qualyspy-legacy/assets/host_list.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/assets/host_list_detection.py` & `qualyspy-0.3.9.5/qualyspy-legacy/assets/host_list_detection.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/certview/certificate.py` & `qualyspy-0.3.9.5/qualyspy-legacy/certview/certificate.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/qualyspy-legacy/scan_configuration/knowledgebase.py` & `qualyspy-0.3.9.5/qualyspy-legacy/scan_configuration/knowledgebase.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/tests/gav_test.py` & `qualyspy-0.3.9.5/tests/gav_test.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/tests/vmdr_test.py` & `qualyspy-0.3.9.5/tests/vmdr_test.py`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/.gitignore` & `qualyspy-0.3.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/LICENSE` & `qualyspy-0.3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/README.md` & `qualyspy-0.3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `qualyspy-0.3.9.4/pyproject.toml` & `qualyspy-0.3.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "QualysPy"
-version = "0.3.9.4"
+version = "0.3.9.5"
 authors = [
   { name="Jordan Barnartt", email="jbarnart@uwaterloo.ca" },
 ]
 description = "A Python wrapper for the Qualys API."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `qualyspy-0.3.9.4/PKG-INFO` & `qualyspy-0.3.9.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QualysPy
-Version: 0.3.9.4
+Version: 0.3.9.5
 Summary: A Python wrapper for the Qualys API.
 Project-URL: Homepage, https://github.com/JordanBarnartt/qualyspy
 Project-URL: Bug Tracker, https://github.com/JordanBarnartt/qualyspy/issues
 Author-email: Jordan Barnartt <jbarnart@uwaterloo.ca>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
```

