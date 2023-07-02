# Comparing `tmp/dwave-ocean-sdk-6.4.0.tar.gz` & `tmp/dwave-ocean-sdk-6.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dwave-ocean-sdk-6.4.0.tar", last modified: Fri Jun  2 02:12:34 2023, max compression
+gzip compressed data, was "dist/dwave-ocean-sdk-6.4.1.tar", last modified: Sun Jul  2 01:21:28 2023, max compression
```

## Comparing `dwave-ocean-sdk-6.4.0.tar` & `dwave-ocean-sdk-6.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-02 02:12:02.000000 dwave-ocean-sdk-6.4.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5233 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4238 2023-06-02 02:12:02.000000 dwave-ocean-sdk-6.4.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/dwave_ocean_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5233 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/dwave_ocean_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/dwave_ocean_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/dwave_ocean_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/dwave_ocean_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/dwave_ocean_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/dwaveoceansdk/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2023-06-02 02:12:02.000000 dwave-ocean-sdk-6.4.0/dwaveoceansdk/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      883 2023-06-02 02:12:02.000000 dwave-ocean-sdk-6.4.0/dwaveoceansdk/package_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2023-06-02 02:12:02.000000 dwave-ocean-sdk-6.4.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1396 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-06-02 02:12:02.000000 dwave-ocean-sdk-6.4.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-02 02:12:34.000000 dwave-ocean-sdk-6.4.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3134 2023-06-02 02:12:02.000000 dwave-ocean-sdk-6.4.0/tests/test_individually.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-02 01:21:03.000000 dwave-ocean-sdk-6.4.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5233 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4238 2023-07-02 01:21:03.000000 dwave-ocean-sdk-6.4.1/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/dwave_ocean_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5233 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/dwave_ocean_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      329 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/dwave_ocean_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/dwave_ocean_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/dwave_ocean_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/dwave_ocean_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/dwaveoceansdk/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      604 2023-07-02 01:21:03.000000 dwave-ocean-sdk-6.4.1/dwaveoceansdk/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      883 2023-07-02 01:21:03.000000 dwave-ocean-sdk-6.4.1/dwaveoceansdk/package_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2023-07-02 01:21:03.000000 dwave-ocean-sdk-6.4.1/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1396 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2023-07-02 01:21:03.000000 dwave-ocean-sdk-6.4.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-02 01:21:28.000000 dwave-ocean-sdk-6.4.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3134 2023-07-02 01:21:03.000000 dwave-ocean-sdk-6.4.1/tests/test_individually.py
```

### Comparing `dwave-ocean-sdk-6.4.0/LICENSE` & `dwave-ocean-sdk-6.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-ocean-sdk-6.4.0/PKG-INFO` & `dwave-ocean-sdk-6.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-ocean-sdk
-Version: 6.4.0
+Version: 6.4.1
 Summary: Software development kit for open source D-Wave tools
 Home-page: https://github.com/dwavesystems/dwave-ocean-sdk
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: Apache 2.0
 Project-URL: Changes, https://github.com/dwavesystems/dwave-ocean-sdk/releases
 Project-URL: Documentation, https://docs.ocean.dwavesys.com
```

### Comparing `dwave-ocean-sdk-6.4.0/README.rst` & `dwave-ocean-sdk-6.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `dwave-ocean-sdk-6.4.0/dwave_ocean_sdk.egg-info/PKG-INFO` & `dwave-ocean-sdk-6.4.1/dwave_ocean_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-ocean-sdk
-Version: 6.4.0
+Version: 6.4.1
 Summary: Software development kit for open source D-Wave tools
 Home-page: https://github.com/dwavesystems/dwave-ocean-sdk
 Author: D-Wave Systems Inc.
 Author-email: tools@dwavesys.com
 License: Apache 2.0
 Project-URL: Changes, https://github.com/dwavesystems/dwave-ocean-sdk/releases
 Project-URL: Documentation, https://docs.ocean.dwavesys.com
```

### Comparing `dwave-ocean-sdk-6.4.0/dwaveoceansdk/__init__.py` & `dwave-ocean-sdk-6.4.1/dwaveoceansdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '6.4.0'
+__version__ = '6.4.1'
```

### Comparing `dwave-ocean-sdk-6.4.0/dwaveoceansdk/package_info.py` & `dwave-ocean-sdk-6.4.1/dwaveoceansdk/package_info.py`

 * *Files identical despite different names*

### Comparing `dwave-ocean-sdk-6.4.0/setup.cfg` & `dwave-ocean-sdk-6.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 author = D-Wave Systems Inc.
 author_email = tools@dwavesys.com
 description = Software development kit for open source D-Wave tools
 
 [options]
 install_requires = 
 	dimod==0.12.6
-	dwave-cloud-client==0.10.5
+	dwave-cloud-client==0.10.6
 	dwave-greedy==0.3.0
 	dwave-hybrid==0.6.10
 	dwave-inspector==0.4.2
 	dwave-neal==0.6.0
 	dwave-networkx==0.8.14
 	dwave-preprocessing==0.5.4
 	dwave-samplers==1.0.0
```

### Comparing `dwave-ocean-sdk-6.4.0/setup.py` & `dwave-ocean-sdk-6.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `dwave-ocean-sdk-6.4.0/tests/test_individually.py` & `dwave-ocean-sdk-6.4.1/tests/test_individually.py`

 * *Files identical despite different names*

