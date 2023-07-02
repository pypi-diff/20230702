# Comparing `tmp/fast-webflow-0.2.3.tar.gz` & `tmp/fast-webflow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-webflow-0.2.3.tar", last modified: Sun Jul  2 08:43:43 2023, max compression
+gzip compressed data, was "fast-webflow-0.3.0.tar", last modified: Sun Jul  2 14:54:21 2023, max compression
```

## Comparing `fast-webflow-0.2.3.tar` & `fast-webflow-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:43:43.973659 fast-webflow-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-02 08:43:43.973659 fast-webflow-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-02 08:43:43.973659 fast-webflow-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:43:43.969659 fast-webflow-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:43:43.969659 fast-webflow-0.2.3/src/fast_webflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-02 08:43:43.000000 fast-webflow-0.2.3/src/fast_webflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 08:43:43.000000 fast-webflow-0.2.3/src/fast_webflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:43:43.000000 fast-webflow-0.2.3/src/fast_webflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 08:43:43.000000 fast-webflow-0.2.3/src/fast_webflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:43:43.969659 fast-webflow-0.2.3/src/webflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/src/webflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:43:43.973659 fast-webflow-0.2.3/src/webflow/cms/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/src/webflow/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/src/webflow/cms/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/src/webflow/cms/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/src/webflow/cms/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/src/webflow/cms/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-02 08:43:33.000000 fast-webflow-0.2.3/src/webflow/cms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:54:21.362821 fast-webflow-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-02 14:54:21.362821 fast-webflow-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-02 14:54:21.362821 fast-webflow-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:54:21.362821 fast-webflow-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:54:21.362821 fast-webflow-0.3.0/src/fast_webflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-02 14:54:21.000000 fast-webflow-0.3.0/src/fast_webflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-02 14:54:21.000000 fast-webflow-0.3.0/src/fast_webflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 14:54:21.000000 fast-webflow-0.3.0/src/fast_webflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 14:54:21.000000 fast-webflow-0.3.0/src/fast_webflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:54:21.362821 fast-webflow-0.3.0/src/webflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/src/webflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:54:21.362821 fast-webflow-0.3.0/src/webflow/cms/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/src/webflow/cms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/src/webflow/cms/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/src/webflow/cms/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/src/webflow/cms/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/src/webflow/cms/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-02 14:54:10.000000 fast-webflow-0.3.0/src/webflow/cms/utils.py
```

### Comparing `fast-webflow-0.2.3/LICENSE` & `fast-webflow-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.2.3/PKG-INFO` & `fast-webflow-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.2.3
+Version: 0.3.0
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,16 +20,15 @@
 <!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
 [![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
 
 This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
 
 > Check out an example website built with the help of `fast-webflow`: [**liguriasegreta.com**](https://www.liguriasegreta.com)
 
-### DISCLAIMER
-This is an **unofficial** abstraction over WebFlow's API and I am not associated with the WebFlow team.
+**DISCLAIMER**  : This is an **unofficial** abstraction over WebFlow's API and I am not associated with the WebFlow team.
 
 
 ## Roadmap
 - [ ] Add *e-commerce* functionality
 - [ ] Add *membership* functionality
 - [ ] Add tests
 - [ ] Finish documentation
@@ -48,22 +47,22 @@
 pip install fast-webflow
 ```
 
 ## Getting Started
 1. Obtain an API key from WebFlow by following their [API Access Token](https://developers.webflow.com/docs/access-token).
 2. Import the `cms` module from the `fast-webflow` package automatically to interact with the WebFlow CMS API; then authenticate:
 ```python
-import cms
+import webflow.cms as cms
 api_key = 'YOUR_API_KEY'
 cms.authenticate(api_key)
 ```
 
 3. Start interacting with the WebFlow API using the provided methods. For example, to fetch all items from a collection:
 ```python
-from cms import Collection
+from webflow.cms import Collection
 
 collection_id = 'COLLECTION_ID'
 collection = Collection(collection_id)
 items = collection.get_all_items()
 
 for item in items:
     print(item["slug"])
@@ -72,15 +71,15 @@
 ## Examples
 If you are quickly searching for a particular code snippet, I hope you can find it here. These all
 assume that you *are already authenticated* (if not, see [the quickstart](#getting-started)).
 
 ### Create CMS Elements
 Elements from the CMS are handled via classes, with relevant methods for each. Classes also behave like dictionaries, holding by default some basic information (fetched from the CMS at creation time).
 ```python
-from cms import Site, Collection, Item
+from webflow.cms import Site, Collection, Item
 
 # connect to the Sites part of the API
 site_id = 'YOUR_SITE_ID'
 site = Site(site_id)
 
 # connect to the Collections part of the API
 collection_id = 'YOUR_COLLECTION_ID'
@@ -89,15 +88,15 @@
 # connect to the Items part of the API
 item_id = 'YOUR_ITEM_ID'
 item = Item(item_id)
 ```
 
 ### Fetch Data
 ```python
-from cms import Site, Collection, Item
+from webflow.cms import Site, Collection, Item
 
 # get list of available sites
 sites = cms.list_sites()
 site_id = sites[0]['_id']
 
 # connect to that site's CMS and get some data
 site = Site(site_id)
@@ -119,28 +118,28 @@
 item_id = 'YOUR_ITEM_ID'
 item = Item(item_id)
 item_data = item.get_data()
 ```
 
 ### Publish Website
 ```python
-from cms import Site
+from webflow.cms import Site
 
 # connect to that site's CMS and publish it
 site_id = 'YOUR_SITE_ID'
 site = Site(site_id)
 site.publish()
 
 # you may specify custom domains too
 site.publish(['www.first.domain.com', 'www.second.domain.com'])
 ```
 
 ### Upload Data
 ```python
-from cms import Site, Collection, Item
+from webflow.cms import Site, Collection, Item
 
 new_items = [
   {
     'name': 'first item,
     'slug': 'item1
   },
   {
```

### Comparing `fast-webflow-0.2.3/README.md` & `fast-webflow-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 <!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
 [![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
 
 This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
 
 > Check out an example website built with the help of `fast-webflow`: [**liguriasegreta.com**](https://www.liguriasegreta.com)
 
-### DISCLAIMER
-This is an **unofficial** abstraction over WebFlow's API and I am not associated with the WebFlow team.
+**DISCLAIMER**  : This is an **unofficial** abstraction over WebFlow's API and I am not associated with the WebFlow team.
 
 
 ## Roadmap
 - [ ] Add *e-commerce* functionality
 - [ ] Add *membership* functionality
 - [ ] Add tests
 - [ ] Finish documentation
@@ -33,22 +32,22 @@
 pip install fast-webflow
 ```
 
 ## Getting Started
 1. Obtain an API key from WebFlow by following their [API Access Token](https://developers.webflow.com/docs/access-token).
 2. Import the `cms` module from the `fast-webflow` package automatically to interact with the WebFlow CMS API; then authenticate:
 ```python
-import cms
+import webflow.cms as cms
 api_key = 'YOUR_API_KEY'
 cms.authenticate(api_key)
 ```
 
 3. Start interacting with the WebFlow API using the provided methods. For example, to fetch all items from a collection:
 ```python
-from cms import Collection
+from webflow.cms import Collection
 
 collection_id = 'COLLECTION_ID'
 collection = Collection(collection_id)
 items = collection.get_all_items()
 
 for item in items:
     print(item["slug"])
@@ -57,15 +56,15 @@
 ## Examples
 If you are quickly searching for a particular code snippet, I hope you can find it here. These all
 assume that you *are already authenticated* (if not, see [the quickstart](#getting-started)).
 
 ### Create CMS Elements
 Elements from the CMS are handled via classes, with relevant methods for each. Classes also behave like dictionaries, holding by default some basic information (fetched from the CMS at creation time).
 ```python
-from cms import Site, Collection, Item
+from webflow.cms import Site, Collection, Item
 
 # connect to the Sites part of the API
 site_id = 'YOUR_SITE_ID'
 site = Site(site_id)
 
 # connect to the Collections part of the API
 collection_id = 'YOUR_COLLECTION_ID'
@@ -74,15 +73,15 @@
 # connect to the Items part of the API
 item_id = 'YOUR_ITEM_ID'
 item = Item(item_id)
 ```
 
 ### Fetch Data
 ```python
-from cms import Site, Collection, Item
+from webflow.cms import Site, Collection, Item
 
 # get list of available sites
 sites = cms.list_sites()
 site_id = sites[0]['_id']
 
 # connect to that site's CMS and get some data
 site = Site(site_id)
@@ -104,28 +103,28 @@
 item_id = 'YOUR_ITEM_ID'
 item = Item(item_id)
 item_data = item.get_data()
 ```
 
 ### Publish Website
 ```python
-from cms import Site
+from webflow.cms import Site
 
 # connect to that site's CMS and publish it
 site_id = 'YOUR_SITE_ID'
 site = Site(site_id)
 site.publish()
 
 # you may specify custom domains too
 site.publish(['www.first.domain.com', 'www.second.domain.com'])
 ```
 
 ### Upload Data
 ```python
-from cms import Site, Collection, Item
+from webflow.cms import Site, Collection, Item
 
 new_items = [
   {
     'name': 'first item,
     'slug': 'item1
   },
   {
```

### Comparing `fast-webflow-0.2.3/setup.cfg` & `fast-webflow-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fast-webflow
-version = 0.2.3
+version = 0.3.0
 author = Thomas Cilloni
 author_email = tcilloni@outlook.com
 description = A client library to communicate with the WebFlow API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tcilloni/fast-webflow
 project_urls =
```

### Comparing `fast-webflow-0.2.3/src/fast_webflow.egg-info/PKG-INFO` & `fast-webflow-0.3.0/src/fast_webflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.2.3
+Version: 0.3.0
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -20,16 +20,15 @@
 <!--[![PyPI version](https://badge.fury.io/py/webflow-api.svg)](https://badge.fury.io/py/webflow-api)
 [![Python version](https://img.shields.io/pypi/pyversions/webflow-api.svg)](https://pypi.org/project/webflow-api)-->
 
 This Python library provides an **intuitive** and **fast** interface over WebFlow's API. It simplifies the process of integrating your Python applications with the WebFlow content management system (CMS), allowing you to create, read, update, and delete items within your WebFlow collections.
 
 > Check out an example website built with the help of `fast-webflow`: [**liguriasegreta.com**](https://www.liguriasegreta.com)
 
-### DISCLAIMER
-This is an **unofficial** abstraction over WebFlow's API and I am not associated with the WebFlow team.
+**DISCLAIMER**  : This is an **unofficial** abstraction over WebFlow's API and I am not associated with the WebFlow team.
 
 
 ## Roadmap
 - [ ] Add *e-commerce* functionality
 - [ ] Add *membership* functionality
 - [ ] Add tests
 - [ ] Finish documentation
@@ -48,22 +47,22 @@
 pip install fast-webflow
 ```
 
 ## Getting Started
 1. Obtain an API key from WebFlow by following their [API Access Token](https://developers.webflow.com/docs/access-token).
 2. Import the `cms` module from the `fast-webflow` package automatically to interact with the WebFlow CMS API; then authenticate:
 ```python
-import cms
+import webflow.cms as cms
 api_key = 'YOUR_API_KEY'
 cms.authenticate(api_key)
 ```
 
 3. Start interacting with the WebFlow API using the provided methods. For example, to fetch all items from a collection:
 ```python
-from cms import Collection
+from webflow.cms import Collection
 
 collection_id = 'COLLECTION_ID'
 collection = Collection(collection_id)
 items = collection.get_all_items()
 
 for item in items:
     print(item["slug"])
@@ -72,15 +71,15 @@
 ## Examples
 If you are quickly searching for a particular code snippet, I hope you can find it here. These all
 assume that you *are already authenticated* (if not, see [the quickstart](#getting-started)).
 
 ### Create CMS Elements
 Elements from the CMS are handled via classes, with relevant methods for each. Classes also behave like dictionaries, holding by default some basic information (fetched from the CMS at creation time).
 ```python
-from cms import Site, Collection, Item
+from webflow.cms import Site, Collection, Item
 
 # connect to the Sites part of the API
 site_id = 'YOUR_SITE_ID'
 site = Site(site_id)
 
 # connect to the Collections part of the API
 collection_id = 'YOUR_COLLECTION_ID'
@@ -89,15 +88,15 @@
 # connect to the Items part of the API
 item_id = 'YOUR_ITEM_ID'
 item = Item(item_id)
 ```
 
 ### Fetch Data
 ```python
-from cms import Site, Collection, Item
+from webflow.cms import Site, Collection, Item
 
 # get list of available sites
 sites = cms.list_sites()
 site_id = sites[0]['_id']
 
 # connect to that site's CMS and get some data
 site = Site(site_id)
@@ -119,28 +118,28 @@
 item_id = 'YOUR_ITEM_ID'
 item = Item(item_id)
 item_data = item.get_data()
 ```
 
 ### Publish Website
 ```python
-from cms import Site
+from webflow.cms import Site
 
 # connect to that site's CMS and publish it
 site_id = 'YOUR_SITE_ID'
 site = Site(site_id)
 site.publish()
 
 # you may specify custom domains too
 site.publish(['www.first.domain.com', 'www.second.domain.com'])
 ```
 
 ### Upload Data
 ```python
-from cms import Site, Collection, Item
+from webflow.cms import Site, Collection, Item
 
 new_items = [
   {
     'name': 'first item,
     'slug': 'item1
   },
   {
```

