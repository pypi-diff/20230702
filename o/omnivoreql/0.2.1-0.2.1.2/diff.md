# Comparing `tmp/omnivoreql-0.2.1.tar.gz` & `tmp/omnivoreql-0.2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivoreql-0.2.1.tar", last modified: Sat Jul  1 17:12:55 2023, max compression
+gzip compressed data, was "omnivoreql-0.2.1.2.tar", last modified: Sun Jul  2 00:18:11 2023, max compression
```

## Comparing `omnivoreql-0.2.1.tar` & `omnivoreql-0.2.1.2.tar`

### file list

```diff
@@ -1,14 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 17:12:55.282087 omnivoreql-0.2.1/
--rw-rw-rw-   0        0        0     1086 2023-06-27 21:56:13.000000 omnivoreql-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2102 2023-07-01 17:12:55.282087 omnivoreql-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1492 2023-07-01 16:14:34.000000 omnivoreql-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 17:12:55.282087 omnivoreql-0.2.1/omnivoreql.egg-info/
--rw-rw-rw-   0        0        0     2102 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 17:12:55.000000 omnivoreql-0.2.1/omnivoreql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 17:12:55.290083 omnivoreql-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-07-01 17:12:22.000000 omnivoreql-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:12:55.282087 omnivoreql-0.2.1/test/
--rw-rw-rw-   0        0        0     2490 2023-07-01 15:33:30.000000 omnivoreql-0.2.1/test/test_omnivoreql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.326193 omnivoreql-0.2.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/docs/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/docs/__init__,py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.326193 omnivoreql-0.2.1.2/omnivoreql/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/omnivoreql/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/omnivoreql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:18:11.000000 omnivoreql-0.2.1.2/omnivoreql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:18:11.330193 omnivoreql-0.2.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-02 00:18:03.000000 omnivoreql-0.2.1.2/test/test_omnivoreql.py
```

### Comparing `omnivoreql-0.2.1/LICENSE` & `omnivoreql-0.2.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Shahriar
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Shahriar
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `omnivoreql-0.2.1/PKG-INFO` & `omnivoreql-0.2.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-Metadata-Version: 2.1
-Name: omnivoreql
-Version: 0.2.1
-Summary: Omnivore API Client for Python
-Home-page: https://github.com/yazdipour/OmnivoreQL
-Author: Shahriar Yazdipour
-Author-email: git@yazdipour.com
-License: MIT
-Keywords: omnivore api readlater graphql gql client
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# OmnivoreQL: Omnivore API client for Python
-
-This is a Python client for the [Omnivore API](https://omnivore.app).
-
-[![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
-[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
-<!-- [![Tests](https://github.com/yazdipour/omnivoreql/workflows/Tests/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/) -->
-
-## How to use
-
-To use omnivoreql in your Python project, you can follow these steps:
-
-Install the omnivoreql package using pip:
-
-```bash
-pip install omnivoreql
-```
-
-Import the package into your project:
-
-```python
-import omnivoreql
-```
-
-Create a new instance of the client:
-
-```python
-api_url = "https://api-prod.omnivore.app/api/graphql"
-api_token = "your_api_token_here"
-omnivoreql_client = omnivoreql.OmnivoreQL(api_url, api_token)
-```
-
-Use the methods of the OmnivoreQL class to interact with the Omnivore API. 
-
-```python
-profile = omnivoreql_client.get_profile()
-
-result = omnivoreql_client.save_url("https://www.google.com")
-
-articles = omnivoreql_client.get_articles()
-
-username = profile['me']['profile']['username']
-slug = articles['search']['edges'][0]['node']['slug']
-articles = omnivoreql_client.get_article(username, slug)
-
-labels = omnivoreql_client.get_labels()
-subscriptions = omnivoreql_client.get_subscriptions()
-```
-
-
+Metadata-Version: 2.1
+Name: omnivoreql
+Version: 0.2.1.2
+Summary: Omnivore API Client for Python
+Home-page: https://github.com/yazdipour/OmnivoreQL
+Author: Shahriar Yazdipour
+Author-email: git@yazdipour.com
+License: MIT
+Keywords: omnivore api readlater graphql gql client
+Platform: any
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# OmnivoreQL: Omnivore API client for Python
+
+This is a Python client for the [Omnivore API](https://omnivore.app).
+
+[![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
+[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
+<!-- [![Tests](https://github.com/yazdipour/omnivoreql/workflows/Tests/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/) -->
+[![Github Sponsor](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/yazdipour)
+
+## How to use
+
+To use omnivoreql in your Python project, you can follow these steps:
+
+Install the omnivoreql package using pip:
+
+```bash
+pip install omnivoreql
+```
+
+Import the package into your project:
+
+```python
+import omnivoreql
+```
+
+Create a new instance of the client:
+
+```python
+api_url = "https://api-prod.omnivore.app/api/graphql"
+api_token = "your_api_token_here"
+omnivoreql_client = omnivoreql.OmnivoreQL(api_url, api_token)
+```
+
+Use the methods of the OmnivoreQL class to interact with the Omnivore API. 
+
+```python
+profile = omnivoreql_client.get_profile()
+
+result = omnivoreql_client.save_url("https://www.google.com")
+
+articles = omnivoreql_client.get_articles()
+
+username = profile['me']['profile']['username']
+slug = articles['search']['edges'][0]['node']['slug']
+articles = omnivoreql_client.get_article(username, slug)
+
+labels = omnivoreql_client.get_labels()
+subscriptions = omnivoreql_client.get_subscriptions()
+```
```

### Comparing `omnivoreql-0.2.1/README.md` & `omnivoreql-0.2.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-# OmnivoreQL: Omnivore API client for Python
-
-This is a Python client for the [Omnivore API](https://omnivore.app).
-
-[![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
-[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
-<!-- [![Tests](https://github.com/yazdipour/omnivoreql/workflows/Tests/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/) -->
-
-## How to use
-
-To use omnivoreql in your Python project, you can follow these steps:
-
-Install the omnivoreql package using pip:
-
-```bash
-pip install omnivoreql
-```
-
-Import the package into your project:
-
-```python
-import omnivoreql
-```
-
-Create a new instance of the client:
-
-```python
-api_url = "https://api-prod.omnivore.app/api/graphql"
-api_token = "your_api_token_here"
-omnivoreql_client = omnivoreql.OmnivoreQL(api_url, api_token)
-```
-
-Use the methods of the OmnivoreQL class to interact with the Omnivore API. 
-
-```python
-profile = omnivoreql_client.get_profile()
-
-result = omnivoreql_client.save_url("https://www.google.com")
-
-articles = omnivoreql_client.get_articles()
-
-username = profile['me']['profile']['username']
-slug = articles['search']['edges'][0]['node']['slug']
-articles = omnivoreql_client.get_article(username, slug)
-
-labels = omnivoreql_client.get_labels()
-subscriptions = omnivoreql_client.get_subscriptions()
-```
+# OmnivoreQL: Omnivore API client for Python
+
+This is a Python client for the [Omnivore API](https://omnivore.app).
+
+[![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
+[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
+<!-- [![Tests](https://github.com/yazdipour/omnivoreql/workflows/Tests/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/) -->
+[![Github Sponsor](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/yazdipour)
+
+## How to use
+
+To use omnivoreql in your Python project, you can follow these steps:
+
+Install the omnivoreql package using pip:
+
+```bash
+pip install omnivoreql
+```
+
+Import the package into your project:
+
+```python
+import omnivoreql
+```
+
+Create a new instance of the client:
+
+```python
+api_url = "https://api-prod.omnivore.app/api/graphql"
+api_token = "your_api_token_here"
+omnivoreql_client = omnivoreql.OmnivoreQL(api_url, api_token)
+```
+
+Use the methods of the OmnivoreQL class to interact with the Omnivore API. 
+
+```python
+profile = omnivoreql_client.get_profile()
+
+result = omnivoreql_client.save_url("https://www.google.com")
+
+articles = omnivoreql_client.get_articles()
+
+username = profile['me']['profile']['username']
+slug = articles['search']['edges'][0]['node']['slug']
+articles = omnivoreql_client.get_article(username, slug)
+
+labels = omnivoreql_client.get_labels()
+subscriptions = omnivoreql_client.get_subscriptions()
+```
```

### Comparing `omnivoreql-0.2.1/omnivoreql.egg-info/PKG-INFO` & `omnivoreql-0.2.1.2/omnivoreql.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-Metadata-Version: 2.1
-Name: omnivoreql
-Version: 0.2.1
-Summary: Omnivore API Client for Python
-Home-page: https://github.com/yazdipour/OmnivoreQL
-Author: Shahriar Yazdipour
-Author-email: git@yazdipour.com
-License: MIT
-Keywords: omnivore api readlater graphql gql client
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# OmnivoreQL: Omnivore API client for Python
-
-This is a Python client for the [Omnivore API](https://omnivore.app).
-
-[![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
-[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
-<!-- [![Tests](https://github.com/yazdipour/omnivoreql/workflows/Tests/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/) -->
-
-## How to use
-
-To use omnivoreql in your Python project, you can follow these steps:
-
-Install the omnivoreql package using pip:
-
-```bash
-pip install omnivoreql
-```
-
-Import the package into your project:
-
-```python
-import omnivoreql
-```
-
-Create a new instance of the client:
-
-```python
-api_url = "https://api-prod.omnivore.app/api/graphql"
-api_token = "your_api_token_here"
-omnivoreql_client = omnivoreql.OmnivoreQL(api_url, api_token)
-```
-
-Use the methods of the OmnivoreQL class to interact with the Omnivore API. 
-
-```python
-profile = omnivoreql_client.get_profile()
-
-result = omnivoreql_client.save_url("https://www.google.com")
-
-articles = omnivoreql_client.get_articles()
-
-username = profile['me']['profile']['username']
-slug = articles['search']['edges'][0]['node']['slug']
-articles = omnivoreql_client.get_article(username, slug)
-
-labels = omnivoreql_client.get_labels()
-subscriptions = omnivoreql_client.get_subscriptions()
-```
-
-
+Metadata-Version: 2.1
+Name: omnivoreql
+Version: 0.2.1.2
+Summary: Omnivore API Client for Python
+Home-page: https://github.com/yazdipour/OmnivoreQL
+Author: Shahriar Yazdipour
+Author-email: git@yazdipour.com
+License: MIT
+Keywords: omnivore api readlater graphql gql client
+Platform: any
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# OmnivoreQL: Omnivore API client for Python
+
+This is a Python client for the [Omnivore API](https://omnivore.app).
+
+[![GitHub stars](https://img.shields.io/github/stars/yazdipour/omnivoreql.svg?style=social&label=Star)](https://github.com/yazdipour/omnivoreql/stargazers)
+[![PyPI version](https://badge.fury.io/py/omnivoreql.svg)](https://pypi.org/project/omnivoreql/)
+<!-- [![Tests](https://github.com/yazdipour/omnivoreql/workflows/Tests/badge.svg)](https://github.com/yazdipour/OmnivoreQL/actions/) -->
+[![Github Sponsor](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/yazdipour)
+
+## How to use
+
+To use omnivoreql in your Python project, you can follow these steps:
+
+Install the omnivoreql package using pip:
+
+```bash
+pip install omnivoreql
+```
+
+Import the package into your project:
+
+```python
+import omnivoreql
+```
+
+Create a new instance of the client:
+
+```python
+api_url = "https://api-prod.omnivore.app/api/graphql"
+api_token = "your_api_token_here"
+omnivoreql_client = omnivoreql.OmnivoreQL(api_url, api_token)
+```
+
+Use the methods of the OmnivoreQL class to interact with the Omnivore API. 
+
+```python
+profile = omnivoreql_client.get_profile()
+
+result = omnivoreql_client.save_url("https://www.google.com")
+
+articles = omnivoreql_client.get_articles()
+
+username = profile['me']['profile']['username']
+slug = articles['search']['edges'][0]['node']['slug']
+articles = omnivoreql_client.get_article(username, slug)
+
+labels = omnivoreql_client.get_labels()
+subscriptions = omnivoreql_client.get_subscriptions()
+```
```

### Comparing `omnivoreql-0.2.1/test/test_omnivoreql.py` & `omnivoreql-0.2.1.2/test/test_omnivoreql.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import os
-import unittest
-import sys
-from dotenv import load_dotenv
-
-# Add the path to the folder containing the omnivoreql module to the Python path
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-import omnivoreql.omnivoreql as omnivoreql
-
-class TestOmnivoreQL(unittest.TestCase):
-    omnivoreql = None
-
-    def setUp(self):
-        if self.omnivoreql is None:
-            # Put in .env file or use 'python -m unittest test_omnivoreql.py OMNIVORE_API_TOKEN=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
-            self.api_token = self.getEnvVariable('OMNIVORE_API_TOKEN')
-            print("OMNIVORE_API_TOKEN: " + self.api_token)
-            self.omnivoreql = omnivoreql.OmnivoreQL(
-                "https://api-prod.omnivore.app/api/graphql", self.api_token)
-
-    def getEnvVariable(self, variable_name):
-        for arg in sys.argv[1:]:
-            if arg.startswith(variable_name + '='):
-                return arg.split('=')[1]
-        dotenv_path = os.path.join(os.path.dirname(__file__), '.env')
-        load_dotenv(dotenv_path)
-        return os.environ.get(variable_name)
-
-    def test_get_profile(self):
-        profile = self.omnivoreql.get_profile()
-        self.assertIsNotNone(profile)
-
-    def test_save_url(self):
-        result = self.omnivoreql.save_url("https://www.google.com")
-        self.assertIsNotNone(result)
-        self.assertFalse('errorCodes' in result['saveUrl'])
-
-    def test_get_articles(self):
-        articles = self.omnivoreql.get_articles()
-        self.assertIsNotNone(articles)
-        self.assertFalse('errorCodes' in articles['search'])
-
-    def test_get_article(self):
-        username = self.omnivoreql.get_profile()['me']['profile']['username']
-        slug = self.omnivoreql.get_articles()['search']['edges'][0]['node']['slug']
-        articles = self.omnivoreql.get_article(
-            username, slug
-        )
-        self.assertIsNotNone(articles)
-        self.assertFalse('errorCodes' in articles['article'])
-
-    def test_get_labels(self):
-        labels = self.omnivoreql.get_labels()
-        self.assertIsNotNone(labels)
-        self.assertFalse('errorCodes' in labels['labels'])
-
-    def test_get_subscriptions(self):
-        subscriptions = self.omnivoreql.get_subscriptions()
-        self.assertIsNotNone(subscriptions)
-        self.assertFalse('errorCodes' in subscriptions['subscriptions'])
-
-
-if __name__ == '__main__':
-    unittest.main()
+import os
+import unittest
+import sys
+from dotenv import load_dotenv
+
+# Add the path to the folder containing the omnivoreql module to the Python path
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+import omnivoreql.omnivoreql as omnivoreql
+
+class TestOmnivoreQL(unittest.TestCase):
+    omnivoreql = None
+
+    def setUp(self):
+        if self.omnivoreql is None:
+            # Put in .env file or use 'python -m unittest test_omnivoreql.py OMNIVORE_API_TOKEN=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX'
+            self.api_token = self.getEnvVariable('OMNIVORE_API_TOKEN')
+            print("OMNIVORE_API_TOKEN: " + self.api_token[:4])
+            self.omnivoreql = omnivoreql.OmnivoreQL(
+                "https://api-prod.omnivore.app/api/graphql", self.api_token)
+
+    def getEnvVariable(self, variable_name):
+        for arg in sys.argv[1:]:
+            if arg.startswith(variable_name + '='):
+                return arg.split('=')[1]
+        dotenv_path = os.path.join(os.path.dirname(__file__), '.env')
+        load_dotenv(dotenv_path)
+        return os.environ.get(variable_name)
+
+    def test_get_profile(self):
+        profile = self.omnivoreql.get_profile()
+        self.assertIsNotNone(profile)
+
+    def test_save_url(self):
+        result = self.omnivoreql.save_url("https://www.google.com")
+        self.assertIsNotNone(result)
+        self.assertFalse('errorCodes' in result['saveUrl'])
+
+    def test_get_articles(self):
+        articles = self.omnivoreql.get_articles()
+        self.assertIsNotNone(articles)
+        self.assertFalse('errorCodes' in articles['search'])
+
+    def test_get_article(self):
+        username = self.omnivoreql.get_profile()['me']['profile']['username']
+        slug = self.omnivoreql.get_articles()['search']['edges'][0]['node']['slug']
+        articles = self.omnivoreql.get_article(
+            username, slug
+        )
+        self.assertIsNotNone(articles)
+        self.assertFalse('errorCodes' in articles['article'])
+
+    def test_get_labels(self):
+        labels = self.omnivoreql.get_labels()
+        self.assertIsNotNone(labels)
+        self.assertFalse('errorCodes' in labels['labels'])
+
+    def test_get_subscriptions(self):
+        subscriptions = self.omnivoreql.get_subscriptions()
+        self.assertIsNotNone(subscriptions)
+        self.assertFalse('errorCodes' in subscriptions['subscriptions'])
+
+
+if __name__ == '__main__':
+    unittest.main()
```

