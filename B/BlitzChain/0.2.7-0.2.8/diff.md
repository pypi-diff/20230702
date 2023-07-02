# Comparing `tmp/BlitzChain-0.2.7.tar.gz` & `tmp/BlitzChain-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlitzChain-0.2.7.tar", last modified: Thu Jun 29 02:36:21 2023, max compression
+gzip compressed data, was "BlitzChain-0.2.8.tar", last modified: Sun Jul  2 07:43:14 2023, max compression
```

## Comparing `BlitzChain-0.2.7.tar` & `BlitzChain-0.2.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-29 02:36:21.125012 BlitzChain-0.2.7/
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-29 02:36:21.122890 BlitzChain-0.2.7/BlitzChain.egg-info/
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-29 02:36:21.000000 BlitzChain-0.2.7/BlitzChain.egg-info/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-06-29 02:36:21.000000 BlitzChain-0.2.7/BlitzChain.egg-info/SOURCES.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-06-29 02:36:21.000000 BlitzChain-0.2.7/BlitzChain.egg-info/dependency_links.txt
--rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-06-29 02:36:21.000000 BlitzChain-0.2.7/BlitzChain.egg-info/requires.txt
--rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-06-29 02:36:21.000000 BlitzChain-0.2.7/BlitzChain.egg-info/top_level.txt
--rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.2.7/LICENSE
--rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-06-29 02:36:21.124868 BlitzChain-0.2.7/PKG-INFO
--rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.2.7/README.md
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-29 02:36:21.123678 BlitzChain-0.2.7/blitzchain/
--rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-06-29 02:36:16.000000 BlitzChain-0.2.7/blitzchain/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)     5442 2023-06-29 02:35:41.000000 BlitzChain-0.2.7/blitzchain/api.py
--rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-06-28 05:25:25.000000 BlitzChain-0.2.7/blitzchain/splitter.py
--rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.2.7/blitzchain/utils.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-29 02:36:21.124097 BlitzChain-0.2.7/cli/
--rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.2.7/cli/__init__.py
--rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.2.7/cli/main.py
--rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-06-29 02:36:21.125057 BlitzChain-0.2.7/setup.cfg
--rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.2.7/setup.py
-drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-06-29 02:36:21.124635 BlitzChain-0.2.7/tests/
--rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.2.7/tests/test_crud.py
--rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.2.7/tests/test_pdf.py
--rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.2.7/tests/test_qa.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.634204 BlitzChain-0.2.8/
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.629951 BlitzChain-0.2.8/BlitzChain.egg-info/
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)      361 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/SOURCES.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        1 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/dependency_links.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)        9 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/requires.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)       15 2023-07-02 07:43:14.000000 BlitzChain-0.2.8/BlitzChain.egg-info/top_level.txt
+-rw-r--r--   0 jackywong   (501) staff       (20)    11357 2023-06-25 04:01:50.000000 BlitzChain-0.2.8/LICENSE
+-rw-r--r--   0 jackywong   (501) staff       (20)      189 2023-07-02 07:43:14.633931 BlitzChain-0.2.8/PKG-INFO
+-rw-r--r--   0 jackywong   (501) staff       (20)     3488 2023-06-25 07:25:46.000000 BlitzChain-0.2.8/README.md
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.631242 BlitzChain-0.2.8/blitzchain/
+-rw-r--r--   0 jackywong   (501) staff       (20)       42 2023-07-02 07:43:10.000000 BlitzChain-0.2.8/blitzchain/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     5546 2023-07-02 07:43:05.000000 BlitzChain-0.2.8/blitzchain/api.py
+-rw-r--r--   0 jackywong   (501) staff       (20)     2138 2023-06-28 05:25:25.000000 BlitzChain-0.2.8/blitzchain/splitter.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      763 2023-06-28 00:10:27.000000 BlitzChain-0.2.8/blitzchain/utils.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.631908 BlitzChain-0.2.8/cli/
+-rw-r--r--   0 jackywong   (501) staff       (20)        0 2023-06-28 03:39:00.000000 BlitzChain-0.2.8/cli/__init__.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      430 2023-06-28 13:19:06.000000 BlitzChain-0.2.8/cli/main.py
+-rw-r--r--   0 jackywong   (501) staff       (20)       38 2023-07-02 07:43:14.634285 BlitzChain-0.2.8/setup.cfg
+-rw-r--r--   0 jackywong   (501) staff       (20)      485 2023-06-28 05:27:42.000000 BlitzChain-0.2.8/setup.py
+drwxr-xr-x   0 jackywong   (501) staff       (20)        0 2023-07-02 07:43:14.633334 BlitzChain-0.2.8/tests/
+-rw-r--r--   0 jackywong   (501) staff       (20)      216 2023-06-25 05:27:46.000000 BlitzChain-0.2.8/tests/test_crud.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      715 2023-06-25 05:08:57.000000 BlitzChain-0.2.8/tests/test_pdf.py
+-rw-r--r--   0 jackywong   (501) staff       (20)      621 2023-06-25 07:10:23.000000 BlitzChain-0.2.8/tests/test_qa.py
```

### Comparing `BlitzChain-0.2.7/LICENSE` & `BlitzChain-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.2.7/README.md` & `BlitzChain-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.2.7/blitzchain/api.py` & `BlitzChain-0.2.8/blitzchain/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,56 +68,62 @@
             }
         )
         return get_json_response(response)
 
     
     def generative_qa(self, user_input: str, answer_fields: list,
         conversation_id: str=None, limit: int=5, fields: list=None,
-        include_rerank: bool=False, minimum_rerank_score: float=0.7):
+        include_rerank: bool=False, minimum_rerank_score: float=0.7,
+        include_moderation: bool=False
+    ):
         """Get an answer based on a question that you ask.
         """
         url =  self.base_url + "collection/generative-qa"
         print(url)
         data={
             "collection": self.collection_name,
             "userInput": user_input,
             "answerFields": answer_fields,
             "limit": limit,
             "fields": fields,
             "includeRerank": include_rerank,
-            "minimumRerankScore": minimum_rerank_score
+            "minimumRerankScore": minimum_rerank_score,
+            "include_moderation": include_moderation
         }
         if conversation_id:
             data["conversationID"] = conversation_id
         print(data)
         response = requests.post(
             url,
             headers={
                 "Content-Type": "application/json",
                 "Authorization": "Bearer " + self.api_key
             },
             json=data
         )
         return get_json_response(response)
 
-    def generative_code_qa(self, user_input: str, answer_fields: list,
+    def copilot(self, user_input: str, answer_fields: list,
         conversation_id: str=None, limit: int=5, fields: list=None,
-        include_rerank: bool=False, minimum_rerank_score: float=0.7):
+        include_rerank: bool=False, minimum_rerank_score: float=0.7,
+        include_moderation: bool=False
+    ):
         """Get an answer based on a question that you ask.
         """
         url =  self.base_url + "collection/generative-code-qa"
         print(url)
         data={
             "collection": self.collection_name,
             "userInput": user_input,
             "answerFields": answer_fields,
             "limit": limit,
             "fields": fields,
             "includeRerank": include_rerank,
-            "minimumRerankScore": minimum_rerank_score
+            "minimumRerankScore": minimum_rerank_score,
+            "includeModeration": include_moderation
         }
         if conversation_id:
             data["conversationID"] = conversation_id
         print(data)
         response = requests.post(
             url,
             headers={
@@ -143,24 +149,22 @@
                 "limit": limit,
                 "offset": offset,
                 "fields": fields,
                 "where": where,
                 "sort": sort
             }
         )
-        print(response.content.decode())
         return get_json_response(response)
     
     def count(self):
         api_url = self.base_url + "object/count"
         response = requests.get(
             api_url,
             headers={
                 "Content-Type": "application/json",
                 "Authorization": "Bearer " + self.api_key
             },
             params={
                 "collection": self.collection_name,
             }
         )
-        print(response.content.decode())
         return get_json_response(response)
```

### Comparing `BlitzChain-0.2.7/blitzchain/splitter.py` & `BlitzChain-0.2.8/blitzchain/splitter.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.2.7/blitzchain/utils.py` & `BlitzChain-0.2.8/blitzchain/utils.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.2.7/tests/test_pdf.py` & `BlitzChain-0.2.8/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `BlitzChain-0.2.7/tests/test_qa.py` & `BlitzChain-0.2.8/tests/test_qa.py`

 * *Files identical despite different names*

