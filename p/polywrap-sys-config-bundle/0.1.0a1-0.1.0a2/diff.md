# Comparing `tmp/polywrap_sys_config_bundle-0.1.0a1.tar.gz` & `tmp/polywrap_sys_config_bundle-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_sys_config_bundle-0.1.0a1.tar", max compression
+gzip compressed data, was "polywrap_sys_config_bundle-0.1.0a2.tar", max compression
```

## Comparing `polywrap_sys_config_bundle-0.1.0a1.tar` & `polywrap_sys_config_bundle-0.1.0a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       96 2023-06-24 15:32:46.425073 polywrap_sys_config_bundle-0.1.0a1/README.md
--rw-r--r--   0        0        0      161 2023-06-24 17:33:20.981278 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/__init__.py
--rw-r--r--   0        0        0     1987 2023-06-29 17:50:37.333727 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/bundle.py
--rw-r--r--   0        0        0      473 2023-06-25 07:12:15.268174 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/config.py
--rw-r--r--   0        0        0      481 2023-06-28 19:22:21.709498 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/embeds/__init__.py
--rw-r--r--   0        0        0     4785 2023-06-24 16:28:19.951607 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.info
--rw-r--r--   0        0        0   102231 2023-06-24 16:28:19.955373 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.wasm
--rw-r--r--   0        0        0     6217 2023-06-24 16:28:19.967475 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/embeds/http-resolver/wrap.info
--rw-r--r--   0        0        0   139741 2023-06-24 16:28:19.970782 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/embeds/http-resolver/wrap.wasm
--rw-r--r--   0        0        0        0 2023-06-24 15:32:46.430270 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/py.typed
--rw-r--r--   0        0        0      141 2023-06-24 17:13:09.170974 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/types/__init__.py
--rw-r--r--   0        0        0     1126 2023-06-28 19:21:52.049862 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/types/bundle_package.py
--rw-r--r--   0        0        0      607 2023-06-28 19:22:14.497896 polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/types/embedded_file_reader.py
--rw-r--r--   0        0        0     1419 2023-07-02 07:00:52.182007 polywrap_sys_config_bundle-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 polywrap_sys_config_bundle-0.1.0a1/setup.py
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 polywrap_sys_config_bundle-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0       96 2023-06-24 15:32:46.425073 polywrap_sys_config_bundle-0.1.0a2/README.md
+-rw-r--r--   0        0        0      161 2023-06-24 17:33:20.981278 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/__init__.py
+-rw-r--r--   0        0        0     1987 2023-06-29 17:50:37.333727 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/bundle.py
+-rw-r--r--   0        0        0      473 2023-06-25 07:12:15.268174 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/config.py
+-rw-r--r--   0        0        0      481 2023-06-28 19:22:21.709498 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/embeds/__init__.py
+-rw-r--r--   0        0        0     4785 2023-06-24 16:28:19.951607 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.info
+-rw-r--r--   0        0        0   102231 2023-06-24 16:28:19.955373 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.wasm
+-rw-r--r--   0        0        0     6217 2023-06-24 16:28:19.967475 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/embeds/http-resolver/wrap.info
+-rw-r--r--   0        0        0   139741 2023-06-24 16:28:19.970782 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/embeds/http-resolver/wrap.wasm
+-rw-r--r--   0        0        0        0 2023-06-24 15:32:46.430270 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/py.typed
+-rw-r--r--   0        0        0      141 2023-06-24 17:13:09.170974 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/types/__init__.py
+-rw-r--r--   0        0        0     1126 2023-06-28 19:21:52.049862 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/types/bundle_package.py
+-rw-r--r--   0        0        0      607 2023-06-28 19:22:14.497896 polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/types/embedded_file_reader.py
+-rw-r--r--   0        0        0     1419 2023-07-02 09:00:12.622413 polywrap_sys_config_bundle-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1208 1970-01-01 00:00:00.000000 polywrap_sys_config_bundle-0.1.0a2/setup.py
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 polywrap_sys_config_bundle-0.1.0a2/PKG-INFO
```

### Comparing `polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/bundle.py` & `polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.info` & `polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.info`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.wasm` & `polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.wasm`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/embeds/http-resolver/wrap.info` & `polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/embeds/http-resolver/wrap.info`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/embeds/http-resolver/wrap.wasm` & `polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/embeds/http-resolver/wrap.wasm`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/types/bundle_package.py` & `polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/types/bundle_package.py`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0a1/polywrap_sys_config_bundle/types/embedded_file_reader.py` & `polywrap_sys_config_bundle-0.1.0a2/polywrap_sys_config_bundle/types/embedded_file_reader.py`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0a1/pyproject.toml` & `polywrap_sys_config_bundle-0.1.0a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-sys-config-bundle"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "Polywrap System Client Config Bundle"
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [
     { include = "polywrap_sys_config_bundle" },
 ]
 include = ["**/wrap.info", "**/wrap.wasm"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-core = "^0.1.0a1"
-polywrap-client-config-builder = "^0.1.0a1"
-polywrap-http-plugin = "^0.1.0a1"
-polywrap-uri-resolvers = "^0.1.0a1"
-polywrap-manifest = "^0.1.0a1"
-polywrap-wasm = "^0.1.0a1"
-polywrap-fs-plugin = "^0.1.0a1"
+polywrap-core = "^0.1.0a2"
+polywrap-client-config-builder = "^0.1.0a2"
+polywrap-http-plugin = "^0.1.0a2"
+polywrap-uri-resolvers = "^0.1.0a2"
+polywrap-manifest = "^0.1.0a2"
+polywrap-wasm = "^0.1.0a2"
+polywrap-fs-plugin = "^0.1.0a2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
```

### Comparing `polywrap_sys_config_bundle-0.1.0a1/setup.py` & `polywrap_sys_config_bundle-0.1.0a2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 package_data = \
 {'': ['*'],
  'polywrap_sys_config_bundle.embeds': ['file-system-resolver/*',
                                        'http-resolver/*']}
 
 install_requires = \
-['polywrap-client-config-builder>=0.1.0a1,<0.2.0',
- 'polywrap-core>=0.1.0a1,<0.2.0',
- 'polywrap-fs-plugin>=0.1.0a1,<0.2.0',
- 'polywrap-http-plugin>=0.1.0a1,<0.2.0',
- 'polywrap-manifest>=0.1.0a1,<0.2.0',
- 'polywrap-uri-resolvers>=0.1.0a1,<0.2.0',
- 'polywrap-wasm>=0.1.0a1,<0.2.0']
+['polywrap-client-config-builder>=0.1.0a2,<0.2.0',
+ 'polywrap-core>=0.1.0a2,<0.2.0',
+ 'polywrap-fs-plugin>=0.1.0a2,<0.2.0',
+ 'polywrap-http-plugin>=0.1.0a2,<0.2.0',
+ 'polywrap-manifest>=0.1.0a2,<0.2.0',
+ 'polywrap-uri-resolvers>=0.1.0a2,<0.2.0',
+ 'polywrap-wasm>=0.1.0a2,<0.2.0']
 
 setup_kwargs = {
     'name': 'polywrap-sys-config-bundle',
-    'version': '0.1.0a1',
+    'version': '0.1.0a2',
     'description': 'Polywrap System Client Config Bundle',
     'long_description': '# polywrap-test-cases\n\nThis package allows fetching wrap test-cases from the wrap-test-harness.\n',
     'author': 'Niraj',
     'author_email': 'niraj@polywrap.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `polywrap_sys_config_bundle-0.1.0a1/PKG-INFO` & `polywrap_sys_config_bundle-0.1.0a2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: polywrap-sys-config-bundle
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Polywrap System Client Config Bundle
 Author: Niraj
 Author-email: niraj@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-client-config-builder (>=0.1.0a1,<0.2.0)
-Requires-Dist: polywrap-core (>=0.1.0a1,<0.2.0)
-Requires-Dist: polywrap-fs-plugin (>=0.1.0a1,<0.2.0)
-Requires-Dist: polywrap-http-plugin (>=0.1.0a1,<0.2.0)
-Requires-Dist: polywrap-manifest (>=0.1.0a1,<0.2.0)
-Requires-Dist: polywrap-uri-resolvers (>=0.1.0a1,<0.2.0)
-Requires-Dist: polywrap-wasm (>=0.1.0a1,<0.2.0)
+Requires-Dist: polywrap-client-config-builder (>=0.1.0a2,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0a2,<0.2.0)
+Requires-Dist: polywrap-fs-plugin (>=0.1.0a2,<0.2.0)
+Requires-Dist: polywrap-http-plugin (>=0.1.0a2,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0a2,<0.2.0)
+Requires-Dist: polywrap-uri-resolvers (>=0.1.0a2,<0.2.0)
+Requires-Dist: polywrap-wasm (>=0.1.0a2,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-test-cases
 
 This package allows fetching wrap test-cases from the wrap-test-harness.
```

