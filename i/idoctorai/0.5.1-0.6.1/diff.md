# Comparing `tmp/idoctorai-0.5.1.tar.gz` & `tmp/idoctorai-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.5.1.tar", max compression
+gzip compressed data, was "idoctorai-0.6.1.tar", max compression
```

## Comparing `idoctorai-0.5.1.tar` & `idoctorai-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.5.1/LICENSE
--rw-r--r--   0        0        0    20905 2023-06-29 10:03:27.224271 idoctorai-0.5.1/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.5.1/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.5.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.5.1/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.5.1/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.5.1/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.5.1/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.5.1/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.5.1/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.5.1/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.5.1/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.5.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.5.1/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11296 2023-06-29 09:52:57.848773 idoctorai-0.5.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.5.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.5.1/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.5.1/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3271 2023-06-17 01:00:10.732858 idoctorai-0.5.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.5.1/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.5.1/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.5.1/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.5.1/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.5.1/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1741 2023-06-19 11:42:53.032573 idoctorai-0.5.1/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.5.1/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1606 2023-06-19 11:43:16.346788 idoctorai-0.5.1/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1480 2023-06-29 10:04:47.973917 idoctorai-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.5.1/README.md
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 idoctorai-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.6.1/LICENSE
+-rw-r--r--   0        0        0    20905 2023-07-02 07:24:35.136407 idoctorai-0.6.1/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.6.1/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.6.1/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.6.1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.6.1/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.6.1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.6.1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.6.1/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.6.1/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.6.1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     3082 2023-07-02 07:24:07.017384 idoctorai-0.6.1/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.6.1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.6.1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11296 2023-06-29 09:52:57.848773 idoctorai-0.6.1/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.6.1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.6.1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     3466 2023-07-02 07:23:10.503593 idoctorai-0.6.1/pandasai/llm/model.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.6.1/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3275 2023-07-02 06:33:47.366335 idoctorai-0.6.1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.6.1/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.6.1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.6.1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.6.1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.6.1/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1741 2023-06-19 11:42:53.032573 idoctorai-0.6.1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.6.1/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1606 2023-06-19 11:43:16.346788 idoctorai-0.6.1/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1480 2023-07-02 07:44:37.474145 idoctorai-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.6.1/README.md
+-rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 idoctorai-0.6.1/PKG-INFO
```

### Comparing `idoctorai-0.5.1/LICENSE` & `idoctorai-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/__init__.py` & `idoctorai-0.6.1/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/constants.py` & `idoctorai-0.6.1/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/exceptions.py` & `idoctorai-0.6.1/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/helpers/_optional.py` & `idoctorai-0.6.1/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/helpers/anonymizer.py` & `idoctorai-0.6.1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/helpers/cache.py` & `idoctorai-0.6.1/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/helpers/from_excel.py` & `idoctorai-0.6.1/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/helpers/notebook.py` & `idoctorai-0.6.1/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/helpers/save_chart.py` & `idoctorai-0.6.1/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/langchain/__init__.py` & `idoctorai-0.6.1/pandasai/langchain/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 
 from langchain.memory import ConversationBufferMemory
 
 from langchain import OpenAI, ConversationChain, LLMChain, PromptTemplate
 from langchain.memory import ConversationBufferWindowMemory
 
 from typing import Any, Dict, Optional
+from langchain.llms import AzureOpenAI
+
 
 
 
 class LangChain:
 
     api_token: str
     conversation: ConversationChain
-    llm: OpenAI
+    llm: AzureOpenAI
     model_name: str = "gpt-3.5-turbo"
     k: int = 2
     max_tokens: int = 4097
 
     template = """Assistant is a large language model trained by OpenAI.
 
 Assistant is designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, Assistant is able to generate human-like text based on the input it receives, allowing it to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
@@ -33,17 +35,19 @@
 Assistant:"""
     
     template= """
 {history}
 Human: {human_input}
 Assistant:"""
 
-    def __init__(self, api_token: Optional[str] = None, **kwargs,):
-        self.api_token = api_token or None
-        self.llm = OpenAI(model_name=self.model_name, openai_api_key=self.api_token, temperature=0)
+    def __init__(self, llm: AzureOpenAI, **kwargs,):
+        # self.llm = OpenAI(model_name=self.model_name, openai_api_key=self.api_token, temperature=0)
+        if llm is None:
+            raise ValueError("llm is required")
+        self.llm = llm
         prompt = PromptTemplate(
             input_variables=["history","human_input"], 
             template=self.template
         )
 
         memory = ConversationBufferWindowMemory(k=self.k)
         # memory = ConversationBufferMemory(memory_key="history", memory_size=3)
```

### Comparing `idoctorai-0.5.1/pandasai/llm/azure_openai.py` & `idoctorai-0.6.1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/llm/base.py` & `idoctorai-0.6.1/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/llm/fake.py` & `idoctorai-0.6.1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/llm/google_palm.py` & `idoctorai-0.6.1/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/llm/open_assistant.py` & `idoctorai-0.6.1/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/llm/openai.py` & `idoctorai-0.6.1/pandasai/llm/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,16 @@
         """
 
         self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
         if self.api_token is None:
             raise APIKeyNotFoundError("OpenAI API key is required")
         openai.api_key = self.api_token
 
-        # langchain 
-        self.langchain = LangChain(api_token=self.api_token)
+        # # langchain 
+        # self.langchain = LangChain(api_token=self.api_token)
 
         self._set_params(**kwargs)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling OpenAI API"""
         return {
@@ -95,16 +95,16 @@
             str: Response
         """
         self.last_prompt = str(instruction) + str(value)
 
         if self.model in self._supported_completion_models:
             response = self.completion(str(instruction) + str(value) + suffix)
         elif self.model in self._supported_chat_models:
-            # response = self.chat_completion(str(instruction) + str(value) + suffix)
-            response = self.langchain_input(str(instruction) + str(value) + suffix, history)
+            response = self.chat_completion(str(instruction) + str(value) + suffix)
+            # response = self.langchain_input(str(instruction) + str(value) + suffix, history)
             # print(response)
         else:
             raise UnsupportedOpenAIModelError("Unsupported model")
 
         return response
 
     @property
```

### Comparing `idoctorai-0.5.1/pandasai/llm/starcoder.py` & `idoctorai-0.6.1/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/prompts/base.py` & `idoctorai-0.6.1/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.6.1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.6.1/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/prompts/generate_python_code.py` & `idoctorai-0.6.1/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/prompts/generate_response.py` & `idoctorai-0.6.1/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.6.1/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.5.1/pyproject.toml` & `idoctorai-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.5.1"
+version = "0.6.1"
 description = "idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"},{include="pyproject.toml"}]
```

### Comparing `idoctorai-0.5.1/PKG-INFO` & `idoctorai-0.6.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.5.1
+Version: 0.6.1
 Summary: idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

