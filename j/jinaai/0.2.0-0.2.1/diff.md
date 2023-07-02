# Comparing `tmp/jinaai-0.2.0.tar.gz` & `tmp/jinaai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinaai-0.2.0.tar", last modified: Tue Jun 27 13:44:34 2023, max compression
+gzip compressed data, was "jinaai-0.2.1.tar", last modified: Sun Jul  2 06:39:42 2023, max compression
```

## Comparing `jinaai-0.2.0.tar` & `jinaai-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-27 13:44:34.098364 jinaai-0.2.0/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.2.0/LICENSE
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13476 2023-06-27 13:44:34.098042 jinaai-0.2.0/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13227 2023-06-27 13:38:12.000000 jinaai-0.2.0/README.md
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-27 13:44:34.096825 jinaai-0.2.0/jinaai/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2642 2023-06-27 13:33:29.000000 jinaai-0.2.0/jinaai/__init__.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-27 13:44:34.097886 jinaai-0.2.0/jinaai/clients/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.2.0/jinaai/clients/HTTPClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1867 2023-06-27 13:25:15.000000 jinaai-0.2.0/jinaai/clients/JinaChatClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2110 2023-06-19 04:25:56.000000 jinaai-0.2.0/jinaai/clients/PromptPerfectClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.2.0/jinaai/clients/RationaleClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1686 2023-06-19 03:26:43.000000 jinaai-0.2.0/jinaai/clients/SceneXClient.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.2.0/jinaai/clients/__init__.py
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.2.0/jinaai/utils.py
-drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-06-27 13:44:34.097234 jinaai-0.2.0/jinaai.egg-info/
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13476 2023-06-27 13:44:34.000000 jinaai-0.2.0/jinaai.egg-info/PKG-INFO
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      373 2023-06-27 13:44:34.000000 jinaai-0.2.0/jinaai.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-06-27 13:44:34.000000 jinaai-0.2.0/jinaai.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-06-27 13:44:34.000000 jinaai-0.2.0/jinaai.egg-info/top_level.txt
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-06-27 13:44:34.098409 jinaai-0.2.0/setup.cfg
--rw-r--r--   0 guillaumeroncari   (501) staff       (20)      483 2023-06-27 13:44:25.000000 jinaai-0.2.0/setup.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-02 06:39:42.558133 jinaai-0.2.1/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    11358 2023-06-12 03:23:49.000000 jinaai-0.2.1/LICENSE
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13564 2023-07-02 06:39:42.557948 jinaai-0.2.1/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13315 2023-07-02 05:30:22.000000 jinaai-0.2.1/README.md
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-02 06:39:42.555772 jinaai-0.2.1/jinaai/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2642 2023-06-27 13:33:29.000000 jinaai-0.2.1/jinaai/__init__.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-02 06:39:42.557780 jinaai-0.2.1/jinaai/clients/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1082 2023-06-19 03:53:55.000000 jinaai-0.2.1/jinaai/clients/HTTPClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1856 2023-07-02 05:36:25.000000 jinaai-0.2.1/jinaai/clients/JinaChatClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     2094 2023-07-02 05:51:36.000000 jinaai-0.2.1/jinaai/clients/PromptPerfectClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1934 2023-06-19 08:21:16.000000 jinaai-0.2.1/jinaai/clients/RationaleClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)     1686 2023-06-19 03:26:43.000000 jinaai-0.2.1/jinaai/clients/SceneXClient.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        0 2023-06-12 04:44:46.000000 jinaai-0.2.1/jinaai/clients/__init__.py
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      891 2023-06-16 08:41:29.000000 jinaai-0.2.1/jinaai/utils.py
+drwxr-xr-x   0 guillaumeroncari   (501) staff       (20)        0 2023-07-02 06:39:42.556528 jinaai-0.2.1/jinaai.egg-info/
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)    13564 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      402 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        1 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        9 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/requires.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)        7 2023-07-02 06:39:42.000000 jinaai-0.2.1/jinaai.egg-info/top_level.txt
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)       38 2023-07-02 06:39:42.558179 jinaai-0.2.1/setup.cfg
+-rw-r--r--   0 guillaumeroncari   (501) staff       (20)      508 2023-07-02 06:38:55.000000 jinaai-0.2.1/setup.py
```

### Comparing `jinaai-0.2.0/LICENSE` & `jinaai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.0/PKG-INFO` & `jinaai-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,100 +1,106 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.2.0
+Version: 0.2.1
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JinaAI Python SDK
 
-The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products—SceneXplain, PromptPerfect, Rationale, and JinaChat—into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK enables users to effortlessly formulate and fine-tune prompts, thus streamlining application development.
-
+The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products — [SceneXplain](https://scenex.jina.ai), [PromptPerfect](https://promptperfect.jina.ai/), [Rationale](https://rationale.jina.ai/), and [JinaChat](https://chat.jina.ai/) — into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK lets you effortlessly formulate and fine-tune prompts, thus streamlining application development.
 
 ## Installing
 
-### Package Manager
+### Package manager
 
 Using pip:
 ```bash
 $ pip install jinaai
 ```
 
-## API Secrets
+## API secrets
 
-To generate an API secret, you need to authenticate on each respective platform and navigate to the API tab:
+To generate an API secret, you need to authenticate on each respective platform's API tab:
 
 - [SceneXplain API](https://scenex.jina.ai/api)
 - [PromptPerfect API](https://promptperfect.jina.ai/api)
 - [Rationale API](https://rationale.jina.ai/api)
 - [JinaChat API](https://chat.jina.ai/api)
 
 > **Note:** Each secret is product-specific and cannot be interchanged. If you're planning to use multiple products, you'll need to generate a separate secret for each.
 
-## Example Usage
+## Example usage
+
 
 Import the SDK and instantiate a new client with your authentication secrets:
+
 ```python
 from jinaai import JinaAI
 
-jinaai = new JinaAI(
+jinaai = JinaAI(
     secrets = {
         'promptperfect-secret': 'XXXXXX',
         'scenex-secret': 'XXXXXX',
         'rationale-secret': 'XXXXXX',
         'jinachat-secret': 'XXXXXX',
     }
 )
 ```
 
 Describe images:
+
 ```python
 descriptions = jinaai.describe(
     'https://picsum.photos/200'
 )
 ```
 
 Evaluate situations:
+
 ```python
 decisions = jinaai.decide(
     'Going to Paris this summer', 
     { 'analysis': 'proscons' }
 )
 ```
 
 Optimize prompts:
+
 ```python
 prompts = jinaai.optimize(
     'Write an Hello World function in Python'
 )
 ```
 
-Generate complex answer:
+Generate complex answers:
+
 ```python
 output = jinaai.generate(
     'Give me a recipe for a pizza with pineapple'
 )
 ```
 
-Use APIs together
+Use APIs together:
+
 ```python
 situations = [toBase64(img) for img in [
     'factory-1.png',
     'factory-2.png',
     'factory-3.png',
     'factory-4.png',
 ]]
 
 descriptions = jinaai.describe(situations)
 
 prompt1 = [
-    'Does any of those situations present a danger?',
+    'Do any of those situations present a danger?',
     'Reply with [YES] or [NO] and explain why',
     *['SITUATION:\n' + desc['output'] for i, desc in enumerate(descriptions['results'])]
 ]
 
 analysis = jinaai.generate('\n'.join(prompt1))
 
 prompt2 = [
@@ -122,16 +128,14 @@
 )
 
 print(descriptions['raw'])
 ```
 
 ## API Documentation
 
-<br/>
-
 ### JinaAi.describe
 
 ```python
 output = JinaAI.describe(input, options)
 ```
 
 - Input
```

### Comparing `jinaai-0.2.0/README.md` & `jinaai-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,90 +1,96 @@
 # JinaAI Python SDK
 
-The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products—SceneXplain, PromptPerfect, Rationale, and JinaChat—into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK enables users to effortlessly formulate and fine-tune prompts, thus streamlining application development.
-
+The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products — [SceneXplain](https://scenex.jina.ai), [PromptPerfect](https://promptperfect.jina.ai/), [Rationale](https://rationale.jina.ai/), and [JinaChat](https://chat.jina.ai/) — into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK lets you effortlessly formulate and fine-tune prompts, thus streamlining application development.
 
 ## Installing
 
-### Package Manager
+### Package manager
 
 Using pip:
 ```bash
 $ pip install jinaai
 ```
 
-## API Secrets
+## API secrets
 
-To generate an API secret, you need to authenticate on each respective platform and navigate to the API tab:
+To generate an API secret, you need to authenticate on each respective platform's API tab:
 
 - [SceneXplain API](https://scenex.jina.ai/api)
 - [PromptPerfect API](https://promptperfect.jina.ai/api)
 - [Rationale API](https://rationale.jina.ai/api)
 - [JinaChat API](https://chat.jina.ai/api)
 
 > **Note:** Each secret is product-specific and cannot be interchanged. If you're planning to use multiple products, you'll need to generate a separate secret for each.
 
-## Example Usage
+## Example usage
+
 
 Import the SDK and instantiate a new client with your authentication secrets:
+
 ```python
 from jinaai import JinaAI
 
-jinaai = new JinaAI(
+jinaai = JinaAI(
     secrets = {
         'promptperfect-secret': 'XXXXXX',
         'scenex-secret': 'XXXXXX',
         'rationale-secret': 'XXXXXX',
         'jinachat-secret': 'XXXXXX',
     }
 )
 ```
 
 Describe images:
+
 ```python
 descriptions = jinaai.describe(
     'https://picsum.photos/200'
 )
 ```
 
 Evaluate situations:
+
 ```python
 decisions = jinaai.decide(
     'Going to Paris this summer', 
     { 'analysis': 'proscons' }
 )
 ```
 
 Optimize prompts:
+
 ```python
 prompts = jinaai.optimize(
     'Write an Hello World function in Python'
 )
 ```
 
-Generate complex answer:
+Generate complex answers:
+
 ```python
 output = jinaai.generate(
     'Give me a recipe for a pizza with pineapple'
 )
 ```
 
-Use APIs together
+Use APIs together:
+
 ```python
 situations = [toBase64(img) for img in [
     'factory-1.png',
     'factory-2.png',
     'factory-3.png',
     'factory-4.png',
 ]]
 
 descriptions = jinaai.describe(situations)
 
 prompt1 = [
-    'Does any of those situations present a danger?',
+    'Do any of those situations present a danger?',
     'Reply with [YES] or [NO] and explain why',
     *['SITUATION:\n' + desc['output'] for i, desc in enumerate(descriptions['results'])]
 ]
 
 analysis = jinaai.generate('\n'.join(prompt1))
 
 prompt2 = [
@@ -112,16 +118,14 @@
 )
 
 print(descriptions['raw'])
 ```
 
 ## API Documentation
 
-<br/>
-
 ### JinaAi.describe
 
 ```python
 output = JinaAI.describe(input, options)
 ```
 
 - Input
```

### Comparing `jinaai-0.2.0/jinaai/__init__.py` & `jinaai-0.2.1/jinaai/__init__.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.0/jinaai/clients/HTTPClient.py` & `jinaai-0.2.1/jinaai/clients/HTTPClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.0/jinaai/clients/JinaChatClient.py` & `jinaai-0.2.1/jinaai/clients/JinaChatClient.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .HTTPClient import HTTPClient
 from ..utils import is_base64, is_url
 
 
 class JinaChatClient(HTTPClient):
     def __init__(self, headers=None):
-        baseUrl = 'https://api-dyzugixgtq-uc.a.run.app/v1/chat'
+        baseUrl = 'https://api.chat.jina.ai/v1/chat'
         defaultHeaders = { 
             'Content-Type': 'application/json',
         }
         mergedHeaders = defaultHeaders.update(headers)
         super().__init__(baseUrl=baseUrl, headers=defaultHeaders)
 
     def from_array(self, input, options=None):
```

### Comparing `jinaai-0.2.0/jinaai/clients/PromptPerfectClient.py` & `jinaai-0.2.1/jinaai/clients/PromptPerfectClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .HTTPClient import HTTPClient
 from ..utils import is_base64, is_url
 
 class PromptPerfectClient(HTTPClient):
     def __init__(self, headers=None):
-        baseUrl = 'https://us-central1-prompt-ops.cloudfunctions.net'
+        baseUrl = 'https://api.promptperfect.jina.ai'
         defaultHeaders = { 
             'Content-Type': 'application/json',
         }
         mergedHeaders = defaultHeaders.update(headers)
         super().__init__(baseUrl=baseUrl, headers=defaultHeaders)
 
     def from_array(self, input, options=None):
```

### Comparing `jinaai-0.2.0/jinaai/clients/RationaleClient.py` & `jinaai-0.2.1/jinaai/clients/RationaleClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.0/jinaai/clients/SceneXClient.py` & `jinaai-0.2.1/jinaai/clients/SceneXClient.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.0/jinaai/utils.py` & `jinaai-0.2.1/jinaai/utils.py`

 * *Files identical despite different names*

### Comparing `jinaai-0.2.0/jinaai.egg-info/PKG-INFO` & `jinaai-0.2.1/jinaai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,100 +1,106 @@
 Metadata-Version: 2.1
 Name: jinaai
-Version: 0.2.0
+Version: 0.2.1
 Summary: Jina AI Python SDK
 Home-page: https://github.com/jina-ai/jinaai-py.git
 Author: Jina AI
 Author-email: guillaume.roncari@jina.ai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JinaAI Python SDK
 
-The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products—SceneXplain, PromptPerfect, Rationale, and JinaChat—into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK enables users to effortlessly formulate and fine-tune prompts, thus streamlining application development.
-
+The JinaAI Python SDK is an efficient instrument that smoothly brings the power of JinaAI's products — [SceneXplain](https://scenex.jina.ai), [PromptPerfect](https://promptperfect.jina.ai/), [Rationale](https://rationale.jina.ai/), and [JinaChat](https://chat.jina.ai/) — into Python applications. Acting as a sturdy interface for JinaAI's APIs, this SDK lets you effortlessly formulate and fine-tune prompts, thus streamlining application development.
 
 ## Installing
 
-### Package Manager
+### Package manager
 
 Using pip:
 ```bash
 $ pip install jinaai
 ```
 
-## API Secrets
+## API secrets
 
-To generate an API secret, you need to authenticate on each respective platform and navigate to the API tab:
+To generate an API secret, you need to authenticate on each respective platform's API tab:
 
 - [SceneXplain API](https://scenex.jina.ai/api)
 - [PromptPerfect API](https://promptperfect.jina.ai/api)
 - [Rationale API](https://rationale.jina.ai/api)
 - [JinaChat API](https://chat.jina.ai/api)
 
 > **Note:** Each secret is product-specific and cannot be interchanged. If you're planning to use multiple products, you'll need to generate a separate secret for each.
 
-## Example Usage
+## Example usage
+
 
 Import the SDK and instantiate a new client with your authentication secrets:
+
 ```python
 from jinaai import JinaAI
 
-jinaai = new JinaAI(
+jinaai = JinaAI(
     secrets = {
         'promptperfect-secret': 'XXXXXX',
         'scenex-secret': 'XXXXXX',
         'rationale-secret': 'XXXXXX',
         'jinachat-secret': 'XXXXXX',
     }
 )
 ```
 
 Describe images:
+
 ```python
 descriptions = jinaai.describe(
     'https://picsum.photos/200'
 )
 ```
 
 Evaluate situations:
+
 ```python
 decisions = jinaai.decide(
     'Going to Paris this summer', 
     { 'analysis': 'proscons' }
 )
 ```
 
 Optimize prompts:
+
 ```python
 prompts = jinaai.optimize(
     'Write an Hello World function in Python'
 )
 ```
 
-Generate complex answer:
+Generate complex answers:
+
 ```python
 output = jinaai.generate(
     'Give me a recipe for a pizza with pineapple'
 )
 ```
 
-Use APIs together
+Use APIs together:
+
 ```python
 situations = [toBase64(img) for img in [
     'factory-1.png',
     'factory-2.png',
     'factory-3.png',
     'factory-4.png',
 ]]
 
 descriptions = jinaai.describe(situations)
 
 prompt1 = [
-    'Does any of those situations present a danger?',
+    'Do any of those situations present a danger?',
     'Reply with [YES] or [NO] and explain why',
     *['SITUATION:\n' + desc['output'] for i, desc in enumerate(descriptions['results'])]
 ]
 
 analysis = jinaai.generate('\n'.join(prompt1))
 
 prompt2 = [
@@ -122,16 +128,14 @@
 )
 
 print(descriptions['raw'])
 ```
 
 ## API Documentation
 
-<br/>
-
 ### JinaAi.describe
 
 ```python
 output = JinaAI.describe(input, options)
 ```
 
 - Input
```

