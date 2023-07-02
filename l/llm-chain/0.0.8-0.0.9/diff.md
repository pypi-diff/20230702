# Comparing `tmp/llm-chain-0.0.8.tar.gz` & `tmp/llm-chain-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-chain-0.0.8.tar", last modified: Thu Jun 29 03:21:42 2023, max compression
+gzip compressed data, was "llm-chain-0.0.9.tar", last modified: Thu Jun 29 03:59:06 2023, max compression
```

## Comparing `llm-chain-0.0.8.tar` & `llm-chain-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 03:21:42.840030 llm-chain-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-02-25 17:02:25.000000 llm-chain-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10788 2023-06-29 03:21:42.840989 llm-chain-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10260 2023-06-28 15:14:20.000000 llm-chain-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 03:21:42.785839 llm-chain-0.0.8/llm_chain/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-09 17:08:19.000000 llm-chain-0.0.8/llm_chain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16384 2023-06-27 19:59:06.000000 llm-chain-0.0.8/llm_chain/base.py
--rw-r--r--   0 root         (0) root         (0)     2577 2023-06-26 01:19:40.000000 llm-chain-0.0.8/llm_chain/indexes.py
--rw-r--r--   0 root         (0) root         (0)     1253 2023-06-26 16:49:38.000000 llm-chain-0.0.8/llm_chain/memory.py
--rw-r--r--   0 root         (0) root         (0)     6458 2023-06-26 22:47:09.000000 llm-chain-0.0.8/llm_chain/models.py
--rw-r--r--   0 root         (0) root         (0)     2172 2023-06-26 23:23:59.000000 llm-chain-0.0.8/llm_chain/prompt_templates.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-14 02:06:25.000000 llm-chain-0.0.8/llm_chain/resources.py
--rw-r--r--   0 root         (0) root         (0)     6011 2023-06-29 03:17:13.000000 llm-chain-0.0.8/llm_chain/tools.py
--rw-r--r--   0 root         (0) root         (0)     4345 2023-06-28 05:09:19.000000 llm-chain-0.0.8/llm_chain/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 03:21:42.802796 llm-chain-0.0.8/llm_chain.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10788 2023-06-29 03:21:42.000000 llm-chain-0.0.8/llm_chain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      642 2023-06-29 03:21:42.000000 llm-chain-0.0.8/llm_chain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 03:21:42.000000 llm-chain-0.0.8/llm_chain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-06-29 03:21:42.000000 llm-chain-0.0.8/llm_chain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-29 03:21:42.000000 llm-chain-0.0.8/llm_chain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-25 17:02:25.000000 llm-chain-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      724 2023-06-29 03:21:42.842565 llm-chain-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 03:21:42.838130 llm-chain-0.0.8/tests/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-10 00:17:26.000000 llm-chain-0.0.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4281 2023-06-24 02:22:45.000000 llm-chain-0.0.8/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)    23562 2023-06-27 19:55:50.000000 llm-chain-0.0.8/tests/test_chains.py
--rw-r--r--   0 root         (0) root         (0)    11370 2023-06-26 17:14:59.000000 llm-chain-0.0.8/tests/test_indexes.py
--rw-r--r--   0 root         (0) root         (0)    13992 2023-06-28 05:01:38.000000 llm-chain-0.0.8/tests/test_memory.py
--rw-r--r--   0 root         (0) root         (0)    26878 2023-06-26 17:13:47.000000 llm-chain-0.0.8/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-06-23 05:43:22.000000 llm-chain-0.0.8/tests/test_prompt_templates.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-06-14 02:16:47.000000 llm-chain-0.0.8/tests/test_records.py
--rw-r--r--   0 root         (0) root         (0)     6227 2023-06-27 19:55:26.000000 llm-chain-0.0.8/tests/test_session.py
--rw-r--r--   0 root         (0) root         (0)    15653 2023-06-29 03:20:07.000000 llm-chain-0.0.8/tests/test_tools.py
--rw-r--r--   0 root         (0) root         (0)     3408 2023-06-26 17:18:37.000000 llm-chain-0.0.8/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 03:59:06.636717 llm-chain-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-02-25 17:02:25.000000 llm-chain-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10788 2023-06-29 03:59:06.637756 llm-chain-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10260 2023-06-28 15:14:20.000000 llm-chain-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 03:59:06.585686 llm-chain-0.0.9/llm_chain/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-09 17:08:19.000000 llm-chain-0.0.9/llm_chain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16384 2023-06-27 19:59:06.000000 llm-chain-0.0.9/llm_chain/base.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-06-26 01:19:40.000000 llm-chain-0.0.9/llm_chain/indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-06-26 16:49:38.000000 llm-chain-0.0.9/llm_chain/memory.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2023-06-26 22:47:09.000000 llm-chain-0.0.9/llm_chain/models.py
+-rw-r--r--   0 root         (0) root         (0)     2172 2023-06-26 23:23:59.000000 llm-chain-0.0.9/llm_chain/prompt_templates.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-14 02:06:25.000000 llm-chain-0.0.9/llm_chain/resources.py
+-rw-r--r--   0 root         (0) root         (0)     6018 2023-06-29 03:57:40.000000 llm-chain-0.0.9/llm_chain/tools.py
+-rw-r--r--   0 root         (0) root         (0)     4345 2023-06-28 05:09:19.000000 llm-chain-0.0.9/llm_chain/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 03:59:06.601849 llm-chain-0.0.9/llm_chain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10788 2023-06-29 03:59:06.000000 llm-chain-0.0.9/llm_chain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      642 2023-06-29 03:59:06.000000 llm-chain-0.0.9/llm_chain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 03:59:06.000000 llm-chain-0.0.9/llm_chain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-29 03:59:06.000000 llm-chain-0.0.9/llm_chain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-29 03:59:06.000000 llm-chain-0.0.9/llm_chain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-02-25 17:02:25.000000 llm-chain-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-29 03:59:06.639608 llm-chain-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 03:59:06.634495 llm-chain-0.0.9/tests/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-10 00:17:26.000000 llm-chain-0.0.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-06-24 02:22:45.000000 llm-chain-0.0.9/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    23562 2023-06-27 19:55:50.000000 llm-chain-0.0.9/tests/test_chains.py
+-rw-r--r--   0 root         (0) root         (0)    11370 2023-06-26 17:14:59.000000 llm-chain-0.0.9/tests/test_indexes.py
+-rw-r--r--   0 root         (0) root         (0)    13992 2023-06-28 05:01:38.000000 llm-chain-0.0.9/tests/test_memory.py
+-rw-r--r--   0 root         (0) root         (0)    26878 2023-06-26 17:13:47.000000 llm-chain-0.0.9/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-06-23 05:43:22.000000 llm-chain-0.0.9/tests/test_prompt_templates.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-06-14 02:16:47.000000 llm-chain-0.0.9/tests/test_records.py
+-rw-r--r--   0 root         (0) root         (0)     6227 2023-06-27 19:55:26.000000 llm-chain-0.0.9/tests/test_session.py
+-rw-r--r--   0 root         (0) root         (0)    15653 2023-06-29 03:20:07.000000 llm-chain-0.0.9/tests/test_tools.py
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-06-26 17:18:37.000000 llm-chain-0.0.9/tests/test_utilities.py
```

### Comparing `llm-chain-0.0.8/LICENSE` & `llm-chain-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/PKG-INFO` & `llm-chain-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-chain
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple and extensible LLM Chaining
 Home-page: https://github.com/shane-kercheval/llm-chain
 Author: Shane Kercheval
 Author-email: shane.kercheval@gmail.com
 Project-URL: Bug Tracker, https://github.com/shane-kercheval/llm-chain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llm-chain-0.0.8/README.md` & `llm-chain-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/llm_chain/base.py` & `llm-chain-0.0.9/llm_chain/base.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/llm_chain/indexes.py` & `llm-chain-0.0.9/llm_chain/indexes.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/llm_chain/memory.py` & `llm-chain-0.0.9/llm_chain/memory.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/llm_chain/models.py` & `llm-chain-0.0.9/llm_chain/models.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/llm_chain/prompt_templates.py` & `llm-chain-0.0.9/llm_chain/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/llm_chain/resources.py` & `llm-chain-0.0.9/llm_chain/resources.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/llm_chain/tools.py` & `llm-chain-0.0.9/llm_chain/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     creation_date: int
     answer_count: int
     title: str
     link: str
     body: str
     text: str | None
     markdown: str | None
-    content_license: str
+    content_license: str | None
     answers: list[StackAnswer] = Field(default_factory=list)
 
     def __init__(self, **data):  # noqa
         super().__init__(**data)
         self.text = BeautifulSoup(self.body, 'html.parser').get_text(separator=' ')
         self.markdown = html_to_markdown(self.body)
```

### Comparing `llm-chain-0.0.8/llm_chain/utilities.py` & `llm-chain-0.0.9/llm_chain/utilities.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/llm_chain.egg-info/PKG-INFO` & `llm-chain-0.0.9/llm_chain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-chain
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple and extensible LLM Chaining
 Home-page: https://github.com/shane-kercheval/llm-chain
 Author: Shane Kercheval
 Author-email: shane.kercheval@gmail.com
 Project-URL: Bug Tracker, https://github.com/shane-kercheval/llm-chain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `llm-chain-0.0.8/llm_chain.egg-info/SOURCES.txt` & `llm-chain-0.0.9/llm_chain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/setup.cfg` & `llm-chain-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = llm-chain
-version = 0.0.8
+version = 0.0.9
 author = Shane Kercheval
 author_email = shane.kercheval@gmail.com
 description = Simple and extensible LLM Chaining
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shane-kercheval/llm-chain
 project_urls =
```

### Comparing `llm-chain-0.0.8/tests/conftest.py` & `llm-chain-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/tests/test_chains.py` & `llm-chain-0.0.9/tests/test_chains.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/tests/test_indexes.py` & `llm-chain-0.0.9/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/tests/test_memory.py` & `llm-chain-0.0.9/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/tests/test_models.py` & `llm-chain-0.0.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/tests/test_prompt_templates.py` & `llm-chain-0.0.9/tests/test_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/tests/test_records.py` & `llm-chain-0.0.9/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/tests/test_session.py` & `llm-chain-0.0.9/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/tests/test_tools.py` & `llm-chain-0.0.9/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `llm-chain-0.0.8/tests/test_utilities.py` & `llm-chain-0.0.9/tests/test_utilities.py`

 * *Files identical despite different names*

