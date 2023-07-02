# Comparing `tmp/openai_api_call-0.5.3.tar.gz` & `tmp/openai_api_call-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_call-0.5.3.tar", last modified: Fri Jun 30 03:05:04 2023, max compression
+gzip compressed data, was "openai_api_call-0.6.0.tar", last modified: Sun Jul  2 09:15:34 2023, max compression
```

## Comparing `openai_api_call-0.5.3.tar` & `openai_api_call-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:05:04.860735 openai_api_call-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-30 03:05:04.860735 openai_api_call-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:05:04.856735 openai_api_call-0.5.3/openai_api_call/
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/chattool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/openai_api_call/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 03:05:04.860735 openai_api_call-0.5.3/openai_api_call.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 03:05:04.000000 openai_api_call-0.5.3/openai_api_call.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 03:05:04.860735 openai_api_call-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-30 03:04:49.000000 openai_api_call-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:15:34.364991 openai_api_call-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-07-02 09:15:34.364991 openai_api_call-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:15:34.364991 openai_api_call-0.6.0/openai_api_call/
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/openai_api_call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17100 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/openai_api_call/chattool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/openai_api_call/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/openai_api_call/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/openai_api_call/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/openai_api_call/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/openai_api_call/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:15:34.364991 openai_api_call-0.6.0/openai_api_call.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-07-02 09:15:34.000000 openai_api_call-0.6.0/openai_api_call.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-02 09:15:34.000000 openai_api_call-0.6.0/openai_api_call.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:15:34.000000 openai_api_call-0.6.0/openai_api_call.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-02 09:15:34.000000 openai_api_call-0.6.0/openai_api_call.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:15:34.000000 openai_api_call-0.6.0/openai_api_call.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-02 09:15:34.000000 openai_api_call-0.6.0/openai_api_call.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 09:15:34.000000 openai_api_call-0.6.0/openai_api_call.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 09:15:34.364991 openai_api_call-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-02 09:15:22.000000 openai_api_call-0.6.0/setup.py
```

### Comparing `openai_api_call-0.5.3/LICENSE` & `openai_api_call-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.3/PKG-INFO` & `openai_api_call-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_api_call
-Version: 0.5.3
+Version: 0.6.0
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -215,14 +215,15 @@
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
         - Since version `0.3.0`, you can use different API Key to send requests.
         - Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
         - Since version `0.5.0`, one can use `process_chats` to process the data, with a customized `msg2chat` function and a checkpoint file.
+        - Since version `0.6.0`, the feature [function call](https://platform.openai.com/docs/guides/gpt/function-calling) is added.
 Keywords: openai_api_call
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `openai_api_call-0.5.3/README.md` & `openai_api_call-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -206,8 +206,9 @@
 This package is licensed under the MIT license. See the LICENSE file for more details.
 
 ## update log
 
 - Since version `0.2.0`, `Chat` type is used to handle data
 - Since version `0.3.0`, you can use different API Key to send requests.
 - Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
-- Since version `0.5.0`, one can use `process_chats` to process the data, with a customized `msg2chat` function and a checkpoint file.
+- Since version `0.5.0`, one can use `process_chats` to process the data, with a customized `msg2chat` function and a checkpoint file.
+- Since version `0.6.0`, the feature [function call](https://platform.openai.com/docs/guides/gpt/function-calling) is added.
```

### Comparing `openai_api_call-0.5.3/openai_api_call/__init__.py` & `openai_api_call-0.6.0/openai_api_call/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Openai API call."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '0.5.3'
+__version__ = '0.6.0'
 
 import os, requests
 from .chattool import Chat, Resp, chat_completion, usage_status
 from .checkpoint import load_chats, process_chats
 from .proxy import proxy_on, proxy_off, proxy_status
 from . import request
```

### Comparing `openai_api_call-0.5.3/openai_api_call/checkpoint.py` & `openai_api_call-0.6.0/openai_api_call/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,20 +75,20 @@
         # Warning: You are about to delete the checkpoint file
         os.system(f"rm {checkpoint}")
     ## load chats from the checkpoint file
     chats = load_chats(checkpoint, sep=sep)
     if len(chats) > len(data):
         warnings.warn(f"checkpoint file {checkpoint} has more chats than the messages")
         chats = chats[:len(data)]
-        return [chat[-1] for chat in chats] if last_message_only else chats
+        return [chat[-1]['content'] for chat in chats] if last_message_only else chats
         
     chats.extend([None] * (len(data) - len(chats)))
     ## process chats
     tq = tqdm.tqdm if not notebook else tqdm.notebook.tqdm
     for i in tq(range(len(data))):
         if chats[i] is not None: continue
         chat = data2chat(data[i])
         chat.save(checkpoint, mode='a', end=sep)
         chats[i] = chat
     if last_message_only:
-        return [chat[-1] for chat in chats]
+        return [chat[-1]['content'] for chat in chats]
     return chats
```

### Comparing `openai_api_call-0.5.3/openai_api_call/proxy.py` & `openai_api_call-0.6.0/openai_api_call/proxy.py`

 * *Files identical despite different names*

### Comparing `openai_api_call-0.5.3/openai_api_call/request.py` & `openai_api_call-0.6.0/openai_api_call/request.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,32 +50,40 @@
         parsed_url = parsed_url._replace(scheme="https")
     return urlunparse(parsed_url).replace("///", "//")
 
 def chat_completion( api_key:str
                    , messages:List[Dict]
                    , model:str
                    , chat_url:Union[str, None]=None
+                   , function_call:Union[str, None]=None
+                   , functions:Union[List[str], None]=None
                    , **options) -> Dict:
     """Chat completion API call
     
     Args:
         apikey (str): API key
         messages (List[Dict]): prompt message
         model (str): model to use
         chat_url (Union[str, None], optional): chat url. Defaults to None.
+        function_call (Union[str, None], optional): function call. Defaults to None.
+        functions (Union[List[str], None], optional): functions. Defaults to None.
         **options : options inherited from the `openai.ChatCompletion.create` function.
     
     Returns:
         Dict: API response
     """
     # request data
     payload = {
         "model": model,
         "messages": messages
     }
+    if function_call is not None:
+        payload.update({"function_call": function_call})
+    if functions is not None:
+        payload.update({"functions": functions})
     # inherit options
     payload.update(options)
     # request headers
     headers = {
         'Content-Type': 'application/json',
         'Authorization': 'Bearer ' + api_key
     }
@@ -131,18 +139,18 @@
         data = billing_response.json()
         total_usage = data.get("total_usage") / 100
         daily_costs = data.get("daily_costs")
         return total_storage, total_usage, daily_costs
     else:
         raise Exception(billing_response.text)
 
-# https://api.openai.com/v1/models
 def valid_models(api_key:str, gpt_only:bool=True, url:Union[str, None]=None):
     """Get valid models
-    
+    Request url: https://api.openai.com/v1/models
+
     Args:
         api_key (str): API key
         gpt_only (bool, optional): whether to return only GPT models. Defaults to True.
         url (Union[str, None], optional): base url. Defaults to None.
 
     Returns:
         List[str]: list of valid models
```

### Comparing `openai_api_call-0.5.3/openai_api_call/response.py` & `openai_api_call-0.6.0/openai_api_call/response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,123 @@
 # Response class for OpenAI API call
 
 from typing import Dict
+import json
 
 class Resp():
     
     def __init__(self, response:Dict, strip:bool=True) -> None:
         self.response = response
-        if strip and self.is_valid(): self._strip_content()
+        if strip and self.is_valid() and self.content is not None:
+            self._strip_content()
     
     def _strip_content(self):
         """Strip the content"""
         self.response['choices'][0]['message']['content'] = \
-            self.response['choices'][0]['message']['content'].strip()
+            self.content.strip()
     
     def __repr__(self) -> str:
-        return f"`Resp`: {self.content}"
+        if self.finish_reason == "function_call":
+            return f"`Resp(call)`: {self.function_call}"
+        else:
+            return f"`Resp`: {self.content}"
     
     def __str__(self) -> str:
         return self.content
 
     @property
+    def id(self):
+        return self.response['id']
+    
+    @property
+    def object(self):
+        return self.response['object']
+    
+    @property
+    def model(self):
+        return self.response['model']
+    
+    @property
+    def created(self):
+        return self.response['created']
+    
+    @property
+    def usage(self):
+        """Token usage"""
+        return self.response['usage']
+    
+    @property
     def total_tokens(self):
         """Total number of tokens"""
-        return self.response['usage']['total_tokens']
+        return self.usage['total_tokens']
     
     @property
     def prompt_tokens(self):
         """Number of tokens in the prompt"""
-        return self.response['usage']['prompt_tokens']
+        return self.usage['prompt_tokens']
     
     @property
     def completion_tokens(self):
         """Number of tokens of the response"""
-        return self.response['usage']['completion_tokens']
+        return self.usage['completion_tokens']
     
     @property
-    def content(self):
-        """Content of the response"""
-        return self.response['choices'][0]['message']['content']
+    def finish_reason(self):
+        """Finish reason"""
+        return self.response['choices'][0]['finish_reason']
     
     @property
-    def id(self):
-        return self.response['id']
+    def message(self):
+        """Message"""
+        return self.response['choices'][0]['message']
     
     @property
-    def model(self):
-        return self.response['model']
-    
+    def content(self):
+        """Content of the response"""
+        return self.message['content']
+
     @property
-    def created(self):
-        return self.response['created']
+    def function_call(self):
+        """Function call"""
+        if self.is_function_call:
+            args = {}
+            args['name'] = self.message['function_call']['name']
+            args['arguments'] = self.message['function_call']['arguments']
+            return args
+        else:
+            return None
+
+    def is_function_call(self):
+        """Check if the response is a function call"""
+        return self.finish_reason == 'function_call' and \
+            self.content is None
     
     def is_valid(self):
         """Check if the response is an error"""
         return 'error' not in self.response and 'choices' in self.response
     
     @property
+    def error(self):
+        """Error"""
+        return self.response['error']
+    
+    @property
     def error_message(self):
         """Error message"""
-        return self.response['error']['message']
+        return self.error['message']
     
     @property
     def error_type(self):
         """Error type"""
-        return self.response['error']['type']
+        return self.error['type']
     
     @property
     def error_param(self):
         """Error parameter"""
-        return self.response['error']['param']
+        return self.error['param']
     
     @property
     def error_code(self):
         """Error code"""
-        return self.response['error']['code']
+        return self.error['code']
 
+
```

### Comparing `openai_api_call-0.5.3/openai_api_call.egg-info/PKG-INFO` & `openai_api_call-0.6.0/openai_api_call.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-api-call
-Version: 0.5.3
+Version: 0.6.0
 Summary: A short wrapper of the OpenAI api call.
 Home-page: https://github.com/cubenlp/openai_api_call
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: > **中文文档移步[这里](README_zh_CN.md)。**
         
@@ -215,14 +215,15 @@
         
         ## update log
         
         - Since version `0.2.0`, `Chat` type is used to handle data
         - Since version `0.3.0`, you can use different API Key to send requests.
         - Since version `0.4.0`, this package is mantained by [cubenlp](https://github.com/cubenlp).
         - Since version `0.5.0`, one can use `process_chats` to process the data, with a customized `msg2chat` function and a checkpoint file.
+        - Since version `0.6.0`, the feature [function call](https://platform.openai.com/docs/guides/gpt/function-calling) is added.
 Keywords: openai_api_call
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `openai_api_call-0.5.3/setup.py` & `openai_api_call-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '0.5.3'
+VERSION = '0.6.0'
 
-requirements = ['Click>=7.0', 'requests>=2.20', 'tqdm>=4.60']
+requirements = ['Click>=7.0', 'requests>=2.20', 'tqdm>=4.60', 'docstring_parser>=0.10']
 
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
     author="Rex Wang",
     author_email='1073853456@qq.com',
     python_requires='>=3.8',
```

