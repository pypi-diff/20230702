# Comparing `tmp/omnivoreql-0.2.1.2.tar.gz` & `tmp/omnivoreql-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivoreql-0.2.1.2.tar", last modified: Sun Jul  2 00:18:11 2023, max compression
+gzip compressed data, was "omnivoreql-0.2.2.tar", last modified: Sun Jul  2 11:46:03 2023, max compression
```

## Comparing `omnivoreql-0.2.1.2.tar` & `omnivoreql-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.326193 omnivoreql-0.2.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/docs/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/docs/__init__,py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.326193 omnivoreql-0.2.1.2/omnivoreql/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/omnivoreql/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/omnivoreql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/test/test_omnivoreql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/docs/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/docs/__init__,py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/omnivoreql/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/omnivoreql/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/omnivoreql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/test/test_omnivoreql.py
```

### Comparing `omnivoreql-0.2.1.2/CONTRIBUTING.md` & `omnivoreql-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.1.2/LICENSE` & `omnivoreql-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.1.2/PKG-INFO` & `omnivoreql-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.2.1.2
+Version: 0.2.2
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Keywords: omnivore api readlater graphql gql client
 Platform: any
@@ -40,17 +40,16 @@
 ```python
 import omnivoreql
 ```
 
 Create a new instance of the client:
 
 ```python
-api_url = "https://api-prod.omnivore.app/api/graphql"
 api_token = "your_api_token_here"
-omnivoreql_client = omnivoreql.OmnivoreQL(api_url, api_token)
+omnivoreql_client = omnivoreql.OmnivoreQL(api_token)
 ```
 
 Use the methods of the OmnivoreQL class to interact with the Omnivore API. 
 
 ```python
 profile = omnivoreql_client.get_profile()
```

### Comparing `omnivoreql-0.2.1.2/README.md` & `omnivoreql-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,16 @@
 ```python
 import omnivoreql
 ```
 
 Create a new instance of the client:
 
 ```python
-api_url = "https://api-prod.omnivore.app/api/graphql"
 api_token = "your_api_token_here"
-omnivoreql_client = omnivoreql.OmnivoreQL(api_url, api_token)
+omnivoreql_client = omnivoreql.OmnivoreQL(api_token)
 ```
 
 Use the methods of the OmnivoreQL class to interact with the Omnivore API. 
 
 ```python
 profile = omnivoreql_client.get_profile()
```

### Comparing `omnivoreql-0.2.1.2/docs/PYPI.md` & `omnivoreql-0.2.2/docs/PYPI.md`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.1.2/omnivoreql.egg-info/PKG-INFO` & `omnivoreql-0.2.2/omnivoreql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.2.1.2
+Version: 0.2.2
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Keywords: omnivore api readlater graphql gql client
 Platform: any
@@ -40,17 +40,16 @@
 ```python
 import omnivoreql
 ```
 
 Create a new instance of the client:
 
 ```python
-api_url = "https://api-prod.omnivore.app/api/graphql"
 api_token = "your_api_token_here"
-omnivoreql_client = omnivoreql.OmnivoreQL(api_url, api_token)
+omnivoreql_client = omnivoreql.OmnivoreQL(api_token)
 ```
 
 Use the methods of the OmnivoreQL class to interact with the Omnivore API. 
 
 ```python
 profile = omnivoreql_client.get_profile()
```

### Comparing `omnivoreql-0.2.1.2/setup.py` & `omnivoreql-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.1.2/test/test_omnivoreql.py` & `omnivoreql-0.2.2/test/test_omnivoreql.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 import os
 import unittest
 import sys
 from dotenv import load_dotenv
 
 # Add the path to the folder containing the omnivoreql module to the Python path
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-import omnivoreql.omnivoreql as omnivoreql
+from omnivoreql.omnivoreql import OmnivoreQL
 
 class TestOmnivoreQL(unittest.TestCase):
-    omnivoreql = None
+    client = None
 
-    def setUp(self):
-        if self.omnivoreql is None:
+    @classmethod
+    def setUpClass(cls):
+        if cls.client is None:
             # Put in .env file or use 'python -m unittest test_omnivoreql.py OMNIVORE_API_TOKEN=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
-            self.api_token = self.getEnvVariable('OMNIVORE_API_TOKEN')
-            print("OMNIVORE_API_TOKEN: " + self.api_token[:4])
-            self.omnivoreql = omnivoreql.OmnivoreQL(
-                "https://api-prod.omnivore.app/api/graphql", self.api_token)
+            api_token = cls.getEnvVariable('OMNIVORE_API_TOKEN')
+            print("OMNIVORE_API_TOKEN: " + api_token[:4])
+            cls.client = OmnivoreQL(api_token)
 
-    def getEnvVariable(self, variable_name):
+    @staticmethod
+    def getEnvVariable(variable_name):
         for arg in sys.argv[1:]:
             if arg.startswith(variable_name + '='):
                 return arg.split('=')[1]
         dotenv_path = os.path.join(os.path.dirname(__file__), '.env')
         load_dotenv(dotenv_path)
         return os.environ.get(variable_name)
 
     def test_get_profile(self):
-        profile = self.omnivoreql.get_profile()
+        profile = self.client.get_profile()
         self.assertIsNotNone(profile)
 
     def test_save_url(self):
-        result = self.omnivoreql.save_url("https://www.google.com")
+        result = self.client.save_url("https://www.google.com")
         self.assertIsNotNone(result)
         self.assertFalse('errorCodes' in result['saveUrl'])
 
     def test_get_articles(self):
-        articles = self.omnivoreql.get_articles()
+        articles = self.client.get_articles()
         self.assertIsNotNone(articles)
         self.assertFalse('errorCodes' in articles['search'])
 
     def test_get_article(self):
-        username = self.omnivoreql.get_profile()['me']['profile']['username']
-        slug = self.omnivoreql.get_articles()['search']['edges'][0]['node']['slug']
-        articles = self.omnivoreql.get_article(
+        username = self.client.get_profile()['me']['profile']['username']
+        slug = self.client.get_articles()['search']['edges'][0]['node']['slug']
+        articles = self.client.get_article(
             username, slug
         )
         self.assertIsNotNone(articles)
         self.assertFalse('errorCodes' in articles['article'])
 
     def test_get_labels(self):
-        labels = self.omnivoreql.get_labels()
+        labels = self.client.get_labels()
         self.assertIsNotNone(labels)
         self.assertFalse('errorCodes' in labels['labels'])
 
     def test_get_subscriptions(self):
-        subscriptions = self.omnivoreql.get_subscriptions()
+        subscriptions = self.client.get_subscriptions()
         self.assertIsNotNone(subscriptions)
         self.assertFalse('errorCodes' in subscriptions['subscriptions'])
 
 
 if __name__ == '__main__':
     unittest.main()
```

