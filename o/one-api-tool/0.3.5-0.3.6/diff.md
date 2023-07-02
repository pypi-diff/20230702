# Comparing `tmp/one-api-tool-0.3.5.tar.gz` & `tmp/one-api-tool-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "one-api-tool-0.3.5.tar", last modified: Mon Jun 26 09:40:52 2023, max compression
+gzip compressed data, was "one-api-tool-0.3.6.tar", last modified: Sun Jul  2 06:44:05 2023, max compression
```

## Comparing `one-api-tool-0.3.5.tar` & `one-api-tool-0.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:40:52.990080 one-api-tool-0.3.5/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.5/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)     4427 2023-06-26 09:40:52.989856 one-api-tool-0.3.5/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)     3871 2023-06-26 09:23:01.000000 one-api-tool-0.3.5/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:40:52.988751 one-api-tool-0.3.5/one_api_tool.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)     4427 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-06-26 09:40:52.000000 one-api-tool-0.3.5/one_api_tool.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:40:52.989168 one-api-tool-0.3.5/oneapi/
--rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.5/oneapi/__init__.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-06-26 09:40:52.989524 one-api-tool-0.3.5/oneapi/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.5/oneapi/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.3.5/oneapi/commands/one_api_requst.py
--rw-r--r--   0 zhangchong   (501) staff       (20)    11395 2023-06-26 09:40:17.000000 one-api-tool-0.3.5/oneapi/one_api.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-06-26 09:40:52.990131 one-api-tool-0.3.5/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-06-26 09:40:46.000000 one-api-tool-0.3.5/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-02 06:44:05.819392 one-api-tool-0.3.6/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1055 2023-04-17 11:33:07.000000 one-api-tool-0.3.6/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-02 06:44:05.819170 one-api-tool-0.3.6/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4172 2023-07-02 05:43:55.000000 one-api-tool-0.3.6/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-02 06:44:05.817923 one-api-tool-0.3.6/one_api_tool.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     4728 2023-07-02 06:44:05.000000 one-api-tool-0.3.6/one_api_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      343 2023-07-02 06:44:05.000000 one-api-tool-0.3.6/one_api_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-07-02 06:44:05.000000 one-api-tool-0.3.6/one_api_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       64 2023-07-02 06:44:05.000000 one-api-tool-0.3.6/one_api_tool.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       69 2023-07-02 06:44:05.000000 one-api-tool-0.3.6/one_api_tool.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        7 2023-07-02 06:44:05.000000 one-api-tool-0.3.6/one_api_tool.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-02 06:44:05.818417 one-api-tool-0.3.6/oneapi/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       37 2023-04-28 08:45:03.000000 one-api-tool-0.3.6/oneapi/__init__.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-07-02 06:44:05.818821 one-api-tool-0.3.6/oneapi/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-26 09:00:27.000000 one-api-tool-0.3.6/oneapi/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2168 2023-06-26 09:39:20.000000 one-api-tool-0.3.6/oneapi/commands/one_api_requst.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)    12552 2023-07-02 06:40:59.000000 one-api-tool-0.3.6/oneapi/one_api.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-07-02 06:44:05.819461 one-api-tool-0.3.6/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1051 2023-07-02 06:43:59.000000 one-api-tool-0.3.6/setup.py
```

### Comparing `one-api-tool-0.3.5/LICENSE` & `one-api-tool-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.5/PKG-INFO` & `one-api-tool-0.3.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-Metadata-Version: 2.1
-Name: one-api-tool
-Version: 0.3.5
-Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
-Home-page: https://github.com/muximus3/OneAPI
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # OneAPI
 Easily access multiple ChatGPT or similar APIs with just one line of code/command.
 
 Save a significant amount of ☕️ time by avoiding the need to read multiple API documents and test them individually.
 
 The currently supported APIs include:
  - [x] OpenAI Official API.
+    - [x] ChatGPT: GPT-3.5-turbo/GPT-4.
+    - [x] Token number counting.
+    - [x] Embedding generation.
+    - [x] Function call.
  - [x] Microsoft Azure OpenAI Resource endpoint API.
+    - [x] ChatGPT: GPT-3.5-turbo/GPT-4.
+    - [x] Token number counting.
+    - [x] Embedding generation.
  - [x] Anthropic Claude series model API.
+    - [x] Claude-v1.3-100k, etc.
+    - [x] Token number counting.
 
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
 
 ## Usage
@@ -117,8 +114,8 @@
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
 - [ ] OpenAI function_call.
 - [x] Token number counting.
-- [ ] Custom token budget.
+- [ ] Custom token budget.
```

### Comparing `one-api-tool-0.3.5/README.md` & `one-api-tool-0.3.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,37 @@
+Metadata-Version: 2.1
+Name: one-api-tool
+Version: 0.3.6
+Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
+Home-page: https://github.com/muximus3/OneAPI
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # OneAPI
 Easily access multiple ChatGPT or similar APIs with just one line of code/command.
 
 Save a significant amount of ☕️ time by avoiding the need to read multiple API documents and test them individually.
 
 The currently supported APIs include:
  - [x] OpenAI Official API.
+    - [x] ChatGPT: GPT-3.5-turbo/GPT-4.
+    - [x] Token number counting.
+    - [x] Embedding generation.
+    - [x] Function call.
  - [x] Microsoft Azure OpenAI Resource endpoint API.
+    - [x] ChatGPT: GPT-3.5-turbo/GPT-4.
+    - [x] Token number counting.
+    - [x] Embedding generation.
  - [x] Anthropic Claude series model API.
+    - [x] Claude-v1.3-100k, etc.
+    - [x] Token number counting.
 
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
 
 ## Usage
@@ -105,8 +126,8 @@
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
 ## ToDo
 - [ ] Batch requests.
 - [ ] OpenAI function_call.
 - [x] Token number counting.
-- [ ] Custom token budget.
+- [ ] Custom token budget.
```

### Comparing `one-api-tool-0.3.5/one_api_tool.egg-info/PKG-INFO` & `one-api-tool-0.3.6/one_api_tool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: one-api-tool
-Version: 0.3.5
+Version: 0.3.6
 Summary: Use only one line of code to call multiple model APIs similar to ChatGPT. Currently supported: Azure OpenAI Resource endpoint API, OpenAI Official API, and Anthropic Claude series model API.
 Home-page: https://github.com/muximus3/OneAPI
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -13,16 +13,25 @@
 # OneAPI
 Easily access multiple ChatGPT or similar APIs with just one line of code/command.
 
 Save a significant amount of ☕️ time by avoiding the need to read multiple API documents and test them individually.
 
 The currently supported APIs include:
  - [x] OpenAI Official API.
+    - [x] ChatGPT: GPT-3.5-turbo/GPT-4.
+    - [x] Token number counting.
+    - [x] Embedding generation.
+    - [x] Function call.
  - [x] Microsoft Azure OpenAI Resource endpoint API.
+    - [x] ChatGPT: GPT-3.5-turbo/GPT-4.
+    - [x] Token number counting.
+    - [x] Embedding generation.
  - [x] Anthropic Claude series model API.
+    - [x] Claude-v1.3-100k, etc.
+    - [x] Token number counting.
 
 ## Installation
 ```sh
 pip install -U one-api-tool
 ```
 
 ## Usage
```

### Comparing `one-api-tool-0.3.5/oneapi/commands/one_api_requst.py` & `one-api-tool-0.3.6/oneapi/commands/one_api_requst.py`

 * *Files identical despite different names*

### Comparing `one-api-tool-0.3.5/oneapi/one_api.py` & `one-api-tool-0.3.6/oneapi/one_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,20 @@
     method_commpletions = "completions"
 
 class OpenAIDecodingArguments(BaseModel):
     messages: List[ChatGPTMessage] 
     model: str = "gpt-3.5-turbo"
     max_tokens: int = 2048
     temperature: float = 1
+    functions: Optional[list] = None
+    # Controls how the model responds to function calls. 
+    # "none" means the model does not call a function, and responds to the end-user. 
+    # "auto" means the model can pick between an end-user or calling a function. Specifying a particular function via {"name":\ "my_function"} forces the model to call that function. 
+    # "none" is the default when no functions are present. "auto" is the default if functions are present.
+    function_call : Optional[str] = None
     top_p: float = 1
     n: int = 1
     stream: bool = False
     stop: Optional[Sequence[str]] = None
     presence_penalty: float = 0
     frequency_penalty: float = 0
     user: Optional[str] = ""
@@ -114,15 +120,15 @@
             openai.api_base = self.method.api_base
 
     def simple_chat(self, args: OpenAIDecodingArguments):
         """
         https://learn.microsoft.com/en-us/azure/cognitive-services/openai/how-to/chatgpt?pivots=programming-language-chat-completions
         https://platform.openai.com/docs/api-reference/chat
         """
-
+        args.stream = False if args.functions is not None else args.stream 
         data = args.dict()
         completion = openai.ChatCompletion.create(**data)
         if data.get("stream", False):
             # create variables to collect the stream of chunks
             collected_chunks = []
             collected_messages = []
             # iterate through the stream of events
@@ -131,14 +137,16 @@
                 chunk_choice = chunk["choices"][0]
                 chunk_message = chunk_choice["delta"]  # extract the message
                 finish_reason = chunk_choice["finish_reason"]
                 collected_messages.append(chunk_message)  # save the message
             full_reply_content = "".join([m.get("content", "") for m in collected_messages])
             return full_reply_content
         else:
+            if args.functions is not None:
+                return completion.choices[0].message.get("function_call")
             return completion.choices[0].message.get("content", "")
 
 
     def get_embeddings(self, texts: List[str], engine="text-embedding-ada-002") -> List[List[float]]:
         assert len(texts) <= 2048, "The batch size should not be larger than 2048."
         # replace newlines, which can negatively affect performance.
         texts = [text.replace("\n", " ") for text in texts]
@@ -236,22 +244,29 @@
 
 
     @staticmethod
     def load_json(file_path):
         with open(file_path, "r") as f:
             return json.load(f)
 
-    def simple_chat(self, prompt, system="", model="", temperature=1, max_new_tokens=2048, stream=True, **kwargs):
+    def simple_chat(self, prompt, system="", functions=None, model="", temperature=1, max_new_tokens=2048, stream=True, **kwargs):
         if isinstance(self.tool, OpenAITool):
             msgs = [] if not system else [ChatGPTMessage(role="system", content=system)]
-            msgs.append(ChatGPTMessage(role="user", content=prompt))
+            if isinstance(prompt, str):
+                msgs.append(ChatGPTMessage(role="user", content=prompt))
+            elif isinstance(prompt, list):
+                msgs.extend(prompt)
+            elif isinstance(prompt, (dict, ChatGPTMessage)):
+                msgs.append(prompt)
+            else:
+                raise AssertionError(f"Prompt must be a string, list of strings, or ChatGPTMessage. Got {type(prompt)} instead.")
             if isinstance(self.tool.method, AzureMethod):
                 args = AzureDecodingArguments(messages=msgs, engine=model if model else "gpt-35-turbo", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
             elif isinstance(self.tool.method, OpenAIMethod):
-                args = OpenAIDecodingArguments(messages=msgs, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
+                args = OpenAIDecodingArguments(messages=msgs, functions=functions, function_call="auto" if functions else None, model=model if model else "gpt-3.5-turbo-0613", temperature=temperature, max_tokens=max_new_tokens, stream=stream, **kwargs)
         elif isinstance(self.tool, ClaudeAITool):
             args = ClaudeDecodingArguments(prompt=f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}", model=model if model else "claude-v1.3-100k", temperature=temperature, max_tokens_to_sample=max_new_tokens, stream=stream, **kwargs)
         else:
             raise AssertionError(f"Not supported api type: {type(self.tool)}")
 
         response = self.tool.simple_chat(args)
         return response
@@ -271,7 +286,9 @@
     def count_tokens(self, texts: List[str], encoding_name: str = 'cl100k_base') -> int:
         if isinstance(self.tool, OpenAITool):
             return self.tool.count_tokens(texts, encoding_name)
         elif isinstance(self.tool, ClaudeAITool):
             return sum([anthropic.count_tokens(text) for text in texts])
         else:
             raise AssertionError(f"Not supported api type for token counting: {type(self.tool)}")
+
+
```

### Comparing `one-api-tool-0.3.5/setup.py` & `one-api-tool-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="one-api-tool",
-    version="0.3.5",
+    version="0.3.6",
     packages=find_packages(),
     install_requires=[
         # Add your library's dependencies here
         "pydantic",
         "openai",
         "anthropic",
         "requests",
```

