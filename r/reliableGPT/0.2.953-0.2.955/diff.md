# Comparing `tmp/reliableGPT-0.2.953.tar.gz` & `tmp/reliableGPT-0.2.955.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.953.tar", last modified: Thu Jun 29 21:45:46 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.955.tar", last modified: Sun Jul  2 02:52:48 2023, max compression
```

## Comparing `reliableGPT-0.2.953.tar` & `reliableGPT-0.2.955.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-06-29 21:45:46.247001 reliableGPT-0.2.953/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.953/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-06-29 21:45:46.246870 reliableGPT-0.2.953/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     7112 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-06-29 21:45:46.245261 reliableGPT-0.2.953/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      450 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-06-29 21:45:46.246549 reliableGPT-0.2.953/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/reliablegpt/APICallHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3120 2023-06-29 21:36:46.000000 reliableGPT-0.2.953/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/reliablegpt/CustomQueue.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11224 2023-06-29 21:28:36.000000 reliableGPT-0.2.953/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-06-29 21:07:50.000000 reliableGPT-0.2.953/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5195 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      247 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3921 2023-06-29 21:41:17.000000 reliableGPT-0.2.953/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-06-29 21:45:46.247062 reliableGPT-0.2.953/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      398 2023-06-29 21:45:22.000000 reliableGPT-0.2.953/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-02 02:52:48.237419 reliableGPT-0.2.955/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.955/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-02 02:52:48.237318 reliableGPT-0.2.955/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     6254 2023-07-02 02:49:46.000000 reliableGPT-0.2.955/README.md
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.955/pyproject.toml
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-02 02:52:48.235777 reliableGPT-0.2.955/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-07-02 02:52:48.000000 reliableGPT-0.2.955/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      479 2023-07-02 02:52:48.000000 reliableGPT-0.2.955/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-07-02 02:52:48.000000 reliableGPT-0.2.955/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       54 2023-07-02 02:52:48.000000 reliableGPT-0.2.955/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-07-02 02:52:48.000000 reliableGPT-0.2.955/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-07-02 02:52:48.237175 reliableGPT-0.2.955/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4210 2023-06-28 20:45:06.000000 reliableGPT-0.2.955/reliablegpt/APICallHandler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3120 2023-06-28 23:12:14.000000 reliableGPT-0.2.955/reliablegpt/Alerting.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4407 2023-06-28 20:45:06.000000 reliableGPT-0.2.955/reliablegpt/CustomQueue.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    11549 2023-07-02 02:50:29.000000 reliableGPT-0.2.955/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1286 2023-07-02 02:49:46.000000 reliableGPT-0.2.955/reliablegpt/Model.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5170 2023-07-02 02:49:46.000000 reliableGPT-0.2.955/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      247 2023-06-28 23:12:17.000000 reliableGPT-0.2.955/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3953 2023-07-02 02:50:58.000000 reliableGPT-0.2.955/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2363 2023-07-02 02:50:58.000000 reliableGPT-0.2.955/reliablegpt/reliableQuery.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-07-02 02:52:48.237455 reliableGPT-0.2.955/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      398 2023-07-02 02:52:35.000000 reliableGPT-0.2.955/setup.py
```

### Comparing `reliableGPT-0.2.953/LICENSE` & `reliableGPT-0.2.955/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.953/README.md` & `reliableGPT-0.2.955/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -20,93 +20,58 @@
 * **Specify backup tokens**:
 Using your OpenAI keys across multiple servers - and just got one rotated? You can pass backup keys using `add_keys()`. We will store and go through these, in case any get keys get rotated by OpenAI. For security, we use special tokens, and enable you to delete all your keys (using `delete_keys()`) as well. 
 
 * **Context Window Errors**: 
 For context window errors it automatically retries your request with models with larger context windows
 
 * **Rate Limit Errors**: 
-We put your requests in a queue, and run parallel batches - while accounting for your OpenAI request + token limits (works with Langchain/LlamaIndex/Azure as well).
+Set `queue_requests=True` and We put your requests in a queue, and run parallel batches - while accounting for your OpenAI or Azure OpenAI request + token limits (works with Langchain/LlamaIndex/Azure as well).
 
 # Getting Started
 ## Step 1. pip install package
 ```
 pip install reliableGPT
 ```
 ## Step 2. The core package is 1 line of code
+Integrating with OpenAI, Azure OpenAI, Langchain, LlamaIndex
 ```python
 from reliablegpt import reliableGPT
 openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email='ishaan@berri.ai')
 ```
 
-# Advanced Usage 
-There's the default wrapper called `reliableGPT` - this handles errors thrown by individual queries. 
+## Advanced Usage - Queue Requests for Token & Request Limits 
+### Guaranteed responses from Azure + OpenAI GPT-4, GPT 3.5 Turbo - Handle Rate Limit Errors
+Use `queue_requests=True` and set your token limits as ` model_limits_dir = {"gpt-3.5-turbo": {"max_token_capacity": 1000000, "max_request_capacity": 10000}` You can find your account rate limits here: https://platform.openai.com/account/rate-limits
 
-There's another class `RequestHandler` - this handles the rate-limiting errors. 
+Here's an example request using queing to handle rate limits  
+```python
+openai.ChatCompletion.create = reliableGPT(
+  openai.ChatCompletion.create, 
+  user_email= ["ishaan@berri.ai", "krrish@berri.ai"], 
+  queue_requests=True,
+  model_limits_dir = {"gpt-3.5-turbo": {"max_token_capacity": 1000000, "max_request_capacity": 10000}},
+  fallback_strategy=['gpt-3.5-turbo', 'text-davinci-003', 'gpt-3.5-turbo']
+)
+```
 
 [👋 Give us feedback on how we could make this easier - Email us (krrish@berri.ai) or Text/Whatsapp us (+17708783106)].
 
 ### Breakdown of params
-#### reliableGPT
 Here's everything you can pass to reliableGPT 
 
 | Parameter | Type | Required/Optional | Description |
 | --------- | ---- | ----------------- | ----------- |
 | `openai.ChatCompletion.create`| OpenAI method| Required | This is a method from OpenAI, used for calling the OpenAI chat endpoints|
 | `user_email`| string/list | Required | Update you on spikes in errors. You can either set user_email to one email (as user_email = "ishaan@berri.ai") or multiple (as user_email = ["ishaan@berri.ai", "krrish@berri.ai"] if you want to send alerts to multiple emails |
 | `fallback_strategy` | list | Optional | You can define a custom fallback strategy of OpenAI models you want to try using. If you want to try one model several times, then just repeat that e.g. ['gpt-4', 'gpt-4', 'gpt-3.5-turbo'] will try gpt-4 twice before trying gpt-3.5-turbo | 
+| `queue_requests`| bool | Optional | Set to True if you want to handle rate limit errors using a request queuing mechanism |
+| `model_limits_dir`| dict | Optional | Note: Required if using `queue_requests = True`, For models you want to handle rate limits for set model_limits_dir = {"gpt-3.5-turbo": {"max_token_capacity": 1000000, "max_request_capacity": 10000}} You can find your account rate limits here: https://platform.openai.com/account/rate-limits |
 | `user_token`| string | Optional | Pass your user token if you want us to handle OpenAI Invalid Key Errors - we'll rotate through your stored keys (more on this below 👇) till we get one that works|
+| `backup_openai_key`| string | Optional | Pass your OpenAI API key if you're using Azure and want to switch to OpenAI in case your requests start failing |
 
-#### RequestHandler
-Here's everything you can pass to RequestHandler 👇
-
-🚀 [Example Code](https://colab.research.google.com/drive/1zFmhRbH46Blh7U1ymPSxUcstpMgT4ETX?usp=sharing)
-
-| Parameter | Type | Required/Optional | Description |
-| --------- | ---- | ----------------- | ----------- |
-| `process_func`| function | Required | Your method to call openai. We'll pass your prompt to this method.|
-| `max_token_capacity`| int | Required | Your OpenAI max token rate limit for whichever model you're using |
-| `max_request_capacity`| int | Required | Your OpenAI max request rate limit for whichever model you're using |
-| `user_email`| string | Required | Update you on spikes in errors |
-
-## Handle **rate limits**
-### Step 1. Set your Max Token Capacity, Max Request capacity
-```python
-request_handler = reliablegpt.RequestHandler(process_func=simple_openai_call,
-                              max_token_capacity=40000,
-                              max_request_capacity=200,
-                              verbose=True) # optional set verbose = True
-```
-### Step 2. Run your questions through the RequestHandler
-The `RequestHandler` can handle batches of questions as well as individual questions 
-
-**Example running 9 questions using reliablegpt.RequestHandler**
-```python
-list_questions = [
-  "What is the difference between a list and a tuple in Python?",
-  "How do you iterate over a dictionary in Python?",
-  "What is the purpose of the 'self' parameter in a class method?",
-  "What are lambda functions in Python?",
-  "How do you remove duplicates from a list in Python?",
-  "What is the difference between append() and extend() methods in Python lists?",
-  "How do you read a file in Python?", "How do you write to a file in Python?",
-  "What is the difference between a shallow copy and a deep copy in Python?",
-  "How do you convert a string to lowercase in Python?"
-]
-
-results = request_handler.batch_process(list_questions)
-
-print("\n\n\n")
-print(f"Results from reliableGPT {results}")
-```
-
-**Example running individual questions**
-```python
-print(request_handler.execute("Who is ishaan"))
-print(request_handler.execute("Why is he the best CTO of BerriAI 🍇"))
-```
 ## Handle **rotated keys** 
 ### Step 1. Add your keys 
 ```python
 from reliablegpt import add_keys, delete_keys, reliableGPT
 # Storing your keys 🔒
 user_email = "krrish@berri.ai" # 👈 Replace with your email
 token = add_keys(user_email, ["openai_key_1", "openai_key_2", "openai_key_3"])
```

### Comparing `reliableGPT-0.2.953/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.955/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.953/reliablegpt/Alerting.py` & `reliableGPT-0.2.955/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.953/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.955/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.953/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.955/reliablegpt/IndividualRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import copy
 import posthog
 import importlib
 import openai
 from openai import ChatCompletion
 import traceback
 
+
 class IndividualRequest:
   """A brief description of the class."""
 
   def __init__(self,
                model=None,
                fallback_strategy=[
                  'gpt-3.5-turbo', 'text-davinci-003', 'gpt-4',
@@ -42,14 +43,23 @@
 
   ## Code that handles / wraps openai calls
   def __call__(self, *args, **kwargs):
     try:
       self.print_verbose(f"calling model function: {self.model_function}")
       self.print_verbose(f"these are the kwargs: {kwargs}")
       self.print_verbose(f"this is the openai api base: {openai.api_base}")
+      try:
+        # this should never block running the openai call
+        self.save_request(
+            user_email=self.user_email,
+            graceful_string=self.graceful_string,
+            posthog_event='reliableGPT.request',
+        )
+      except:
+        print("ReliableGPT error occured during saving request")
       result = self.model_function(*args, **kwargs)
       self.print_verbose(f"This is the result: {str(result)[:500]}")
       return result
     except Exception as e:
       self.print_verbose("catches the error")
       return self.handle_exception(args, kwargs, e)
```

### Comparing `reliableGPT-0.2.953/reliablegpt/Model.py` & `reliableGPT-0.2.955/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.953/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.955/reliablegpt/RateLimitHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import uuid
 import time
 import traceback
 
 
 ## Dev Imports 
 # from IndividualRequest import IndividualRequest
-# from RateLimitHandler_helpers.APICallHandler import APICallHandler
+# from APICallHandler import APICallHandler
 
 ## Prod Imports
 from reliablegpt.IndividualRequest import IndividualRequest
 from reliablegpt.APICallHandler import APICallHandler
 
 
 class RateLimitHandler:
```

### Comparing `reliableGPT-0.2.953/reliablegpt/main.py` & `reliableGPT-0.2.955/reliablegpt/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # # Prod Imports
 from reliablegpt.IndividualRequest import IndividualRequest
 from reliablegpt.RateLimitHandler import RateLimitHandler
 from reliablegpt.Model import Model
-from reliablegpt.Alerting import Alerting
+from reliablegpt.alerting import Alerting
+from reliablegpt.reliableQuery import reliable_query
 
 # # Dev Imports
 # from IndividualRequest import IndividualRequest
 # from RateLimitHandler import RateLimitHandler
 # from Model import Model
-# from Alerting import Alerting
+# from alerting import Alerting
 
 from posthog import Posthog
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
@@ -22,15 +23,14 @@
 def save_request(user_email,
                  graceful_string,
                  posthog_event="",
                  result="",
                  posthog_metadata={},
                  errors=[]):
   try:
-    #metadata  = kwargs['metadata']
     if posthog_event != "":
       posthog.capture(user_email, posthog_event,
                       posthog_metadata)  # save posthog event
     if result == graceful_string or len(
         errors) == 2:  # returns a graceful string or got a 2nd exception
       # send an email and alert
       for error in errors:
@@ -80,17 +80,17 @@
                              backup_openai_key=backup_openai_key, 
                              verbose=verbose)
   elif queue_requests == True:
     max_token_capacity = 40000
     max_request_capacity = 200
     ## [TODO]: Allow handling multiple model types (gpt-3.5-turbo AND gpt-4)
     if model_limits_dir and isinstance(model_limits_dir, dict):
-      keys = model_limits_dir.keys()
+      keys = list(model_limits_dir.keys())
       max_token_capacity = model_limits_dir[keys[0]]["max_token_capacity"]
-      max_request_capacity = model_limits_dir["max_request_capacity"]
+      max_request_capacity = model_limits_dir[keys[0]]["max_request_capacity"]
 
     return RateLimitHandler(model,
                             fallback_strategy=fallback_strategy,
                             graceful_string=graceful_string,
                             user_email=primary_email,
                             user_token=user_token,
                             send_notification=send_notification,
```

