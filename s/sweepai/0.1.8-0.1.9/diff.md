# Comparing `tmp/sweepai-0.1.8.tar.gz` & `tmp/sweepai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.1.8.tar", max compression
+gzip compressed data, was "sweepai-0.1.9.tar", max compression
```

## Comparing `sweepai-0.1.8.tar` & `sweepai-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.1.8/LICENSE
--rw-r--r--   0        0        0     1044 2023-07-01 08:56:06.136408 sweepai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-15 06:30:41.945190 sweepai-0.1.8/sweepai/__init__.py
--rw-r--r--   0        0        0    10084 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/api.py
--rw-r--r--   0        0        0     3954 2023-07-01 08:44:12.065355 sweepai-0.1.8/sweepai/app/api_client.py
--rw-r--r--   0        0        0     8683 2023-07-01 08:41:26.515060 sweepai-0.1.8/sweepai/app/backend.py
--rw-r--r--   0        0        0      780 2023-07-01 08:36:57.091240 sweepai-0.1.8/sweepai/app/cli.py
--rw-r--r--   0        0        0     3311 2023-07-01 06:28:16.381542 sweepai-0.1.8/sweepai/app/config.py
--rw-r--r--   0        0        0     6345 2023-07-01 08:46:12.205568 sweepai-0.1.8/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.8/sweepai/core/__init__.py
--rw-r--r--   0        0        0    15868 2023-07-01 08:32:54.140792 sweepai-0.1.8/sweepai/core/chat.py
--rw-r--r--   0        0        0     2553 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     6803 2023-07-01 08:52:47.272877 sweepai-0.1.8/sweepai/core/entities.py
--rw-r--r--   0        0        0    12849 2023-07-01 08:48:08.915774 sweepai-0.1.8/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3509 2023-06-21 23:04:06.027667 sweepai-0.1.8/sweepai/core/react.py
--rw-r--r--   0        0        0    15487 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12335 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-06-16 23:50:11.723074 sweepai-0.1.8/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-03-21 00:50:54.566288 sweepai-0.1.8/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    11280 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-01 08:08:43.804621 sweepai-0.1.8/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-03-19 00:13:25.553442 sweepai-0.1.8/sweepai/utils/__init__.py
--rw-r--r--   0        0        0      385 2023-06-27 05:32:32.711633 sweepai-0.1.8/sweepai/utils/config.py
--rw-r--r--   0        0        0      670 2023-06-30 23:57:36.298069 sweepai-0.1.8/sweepai/utils/constants.py
--rw-r--r--   0        0        0     3633 2023-06-30 23:50:43.896566 sweepai-0.1.8/sweepai/utils/diff.py
--rw-r--r--   0        0        0      511 2023-06-15 23:48:37.899560 sweepai-0.1.8/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8099 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-06-15 23:48:37.899560 sweepai-0.1.8/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-06-15 23:48:37.899560 sweepai-0.1.8/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5339 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      748 2023-06-30 23:50:43.896566 sweepai-0.1.8/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11474 2023-07-01 08:08:27.324592 sweepai-0.1.8/sweepai/utils/utils.py
--rw-r--r--   0        0        0      998 2023-07-01 08:56:08.055470 sweepai-0.1.8/setup.py
--rw-r--r--   0        0        0      500 2023-07-01 08:56:08.055667 sweepai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1091 2023-07-01 23:37:51.703142 sweepai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/__init__.py
+-rw-r--r--   0        0        0    10664 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/api.py
+-rw-r--r--   0        0        0     3954 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/app/api_client.py
+-rw-r--r--   0        0        0     8683 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/app/backend.py
+-rw-r--r--   0        0        0      780 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/app/config.py
+-rw-r--r--   0        0        0     6342 2023-07-01 23:37:26.099727 sweepai-0.1.9/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    15871 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2553 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     6803 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/core/entities.py
+-rw-r--r--   0        0        0    13033 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3509 2023-07-01 23:29:41.701470 sweepai-0.1.9/sweepai/core/react.py
+-rw-r--r--   0        0        0    15487 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12185 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    11177 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/config.py
+-rw-r--r--   0        0        0      669 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     3633 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      511 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8105 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      748 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.1.9/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11266 2023-07-01 23:29:41.708137 sweepai-0.1.9/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     1028 2023-07-01 23:37:56.075299 sweepai-0.1.9/setup.py
+-rw-r--r--   0        0        0      544 2023-07-01 23:37:56.075499 sweepai-0.1.9/PKG-INFO
```

### Comparing `sweepai-0.1.8/LICENSE` & `sweepai-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/pyproject.toml` & `sweepai-0.1.9/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.1.8"
+version = "0.1.9"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [
     { include = "sweepai" }
 ]
 
 [tool.poetry.dependencies]
@@ -13,14 +13,15 @@
 uvicorn = "^0.21.0"
 PyGithub = "1.58.2"
 loguru = "^0.6.0"
 requests = "^2.28.2"
 urllib3 = "^2.0.3"
 gradio = "^3.35.2"
 config-path = "^1.0.3"
+typer = {extras = ["all"], version = "^0.9.0"}
 
 [tool.poetry.dev-dependencies]
 black = "^23.1.0"
 commit5 = "^0.1.1"
 jupyter = "^1.0.0"
 ipykernel = "^6.23.1"
 build = "^0.10.0"
```

### Comparing `sweepai-0.1.8/sweepai/api.py` & `sweepai-0.1.9/sweepai/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from loguru import logger
 import modal
 from pydantic import ValidationError
 from sweepai.handlers.create_pr import create_pr  # type: ignore
 
 from sweepai.handlers.on_ticket import on_ticket
 from sweepai.handlers.on_comment import on_comment
-from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, LABEL_COLOR, LABEL_DESCRIPTION, LABEL_NAME, SWEEP_LOGIN
+from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, DB_NAME, LABEL_COLOR, LABEL_DESCRIPTION, LABEL_NAME, SWEEP_LOGIN
 from sweepai.events import (
     CommentCreatedRequest,
     InstallationCreatedRequest,
     IssueCommentRequest,
     IssueRequest,
     PRRequest,
     ReposAddedRequest,
@@ -52,14 +52,15 @@
     "timeout": 30 * 60,
 }
 
 
 handle_ticket = stub.function(**FUNCTION_SETTINGS)(on_ticket)
 handle_comment = stub.function(**FUNCTION_SETTINGS)(on_comment)
 handle_pr = stub.function(**FUNCTION_SETTINGS)(create_pr)
+update_index = modal.Function.lookup(DB_NAME, "update_index")
 
 
 @stub.function(**FUNCTION_SETTINGS)
 @modal.web_endpoint(method="POST")
 async def webhook(raw_request: Request):
     """Handle a webhook request from GitHub."""
     try:
@@ -212,14 +213,24 @@
                         "merged_sweep_pr", 
                         properties={
                             "repo_name": repo_name,
                             "organization": organization,
                             "repo_full_name": pr_request.repository.full_name,
                             "username": merged_by
                     })
+                update_index.spawn(
+                    request_dict["repository"]["full_name"],
+                    installation_id=request_dict["installation"]["id"],
+                )
+            case ("push", None):
+                if event != "pull_request" or request_dict["base"]["merged"] == True:
+                    update_index.spawn(
+                        request_dict["repository"]["full_name"],
+                        installation_id=request_dict["installation"]["id"],
+                    )
             case "ping", None:
                 return {"message": "pong"}
             case _:
                 logger.info(
                     f"Unhandled event: {event} {request_dict.get('action', None)}"
                 )
     except ValidationError as e:
```

### Comparing `sweepai-0.1.8/sweepai/app/api_client.py` & `sweepai-0.1.9/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/app/backend.py` & `sweepai-0.1.9/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/app/cli.py` & `sweepai-0.1.9/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/app/config.py` & `sweepai-0.1.9/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/app/ui.py` & `sweepai-0.1.9/sweepai/app/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import json
 from github import Github
 import gradio as gr
 from loguru import logger
-import modal
+import webbrowser
 
 from sweepai.app.api_client import APIClient
 from sweepai.app.config import SweepChatConfig
 from sweepai.core.entities import Snippet
 from sweepai.utils.constants import DB_NAME
 
-get_relevant_snippets = modal.Function.lookup(DB_NAME, "get_relevant_snippets")
 config = SweepChatConfig.load()
 
 api_client = APIClient(config=config)
 
 pr_summary_template = """💡 I'll create the following PR:
 
 **{title}**
@@ -49,14 +48,15 @@
             installation_id = api_client.get_installation_id()
             assert installation_id
             config.installation_id = installation_id
             api_client.config = config
             config.save()
             return ""
         except Exception as e:
+            webbrowser.open_new_tab("https://github.com/apps/sweep-ai")
             config.repo_full_name = None
             config.installation_id = None
             config.save()
             api_client.config = config
             raise e
 
     repo_full_name.change(repo_name_change, [repo_full_name], [msg])
```

### Comparing `sweepai-0.1.8/sweepai/core/chat.py` & `sweepai-0.1.9/sweepai/core/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
                             messages=self.messages_dicts,
                             max_tokens=max_tokens - token_sub,
                             temperature=temperature,
                         ) \
                         .choices[0] \
                         .message["content"]
                 except Exception as e:
-                    logger.warn(e)
+                    logger.warning(e)
                     raise e
             result = fetch()
             logger.info(f"Output to call openai:\n{result}")
             return result
     
     def call_anthropic(self, model: ChatModel | None = None) -> str:
         if model is None:
```

### Comparing `sweepai-0.1.8/sweepai/core/code_repair.py` & `sweepai-0.1.9/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/core/entities.py` & `sweepai-0.1.9/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/core/prompts.py` & `sweepai-0.1.9/sweepai/core/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,20 +263,32 @@
 2. Provide complete functions with actual business logic. It is imperative that we do not leave any work to the user/future readers of this code.
 3. Do not write new "todo" comments.
 4. Do not write incomplete functions or line numbers.
 5. Make sure code follows programming language conventions in repo
 
 Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copied>0-25</copied>"). Make sure to use this exact format.
 Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copied>0-50</copied>".
+
+Example: New file:
+print("new file")
+</new_file>
+
+Example: Insert at end:
+<copied>0-100</copied>
+print("inserted at end")
+</new_file>
+
 Example: If you want to insert code after lines 50 and 75:
 <new_file>
 <copied>0-50</copied>
 def main():
      print("hello world")
-<copied>51-100</copied>
+<copied>51-75</copied>
+print("debug statement")
+<copied>76-100</copied>
 </new_file>
 """
 
 pr_code_prompt = ""  # TODO: deprecate this
 
 
 pull_request_prompt = """
```

### Comparing `sweepai-0.1.8/sweepai/core/react.py` & `sweepai-0.1.9/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/core/sweep_bot.py` & `sweepai-0.1.9/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/core/vector_db.py` & `sweepai-0.1.9/sweepai/core/vector_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,30 +251,25 @@
             cache_keys = [hash_sha256(doc) + SENTENCE_TRANSFORMERS_MODEL + sha for doc in documents_to_compute]
             cache.mset({key: json.dumps(value) for key, value in zip(cache_keys, computed_embeddings)})
         return deeplake_vs
     else:
         logger.error("No documents found in repository")
         return deeplake_vs
 
-@stub.function(image=image, secrets=secrets, shared_volumes={DISKCACHE_DIR: model_volume}, timeout=timeout)
-def init_index(
-    repo_name: str,
-    installation_id: int,
-    sweep_config: SweepConfig = SweepConfig(),
-):
-    pass
-
 
 @stub.function(image=image, secrets=secrets, shared_volumes={DISKCACHE_DIR: model_volume}, timeout=timeout)
 def update_index(
     repo_name,
     installation_id: int,
     sweep_config: SweepConfig = SweepConfig(),
-) -> int:
-    pass
+) -> int:    
+    get_deeplake_vs_from_repo(
+    repo_name,
+    sweep_config,
+    installation_id)
 
 
 @stub.function(image=image, secrets=secrets, shared_volumes={DEEPLAKE_DIR: model_volume}, timeout=timeout, keep_warm=1)
 def get_relevant_snippets(
     repo_name: str,
     query: str,
     n_results: int,
```

### Comparing `sweepai-0.1.8/sweepai/events.py` & `sweepai-0.1.9/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/handlers/create_pr.py` & `sweepai-0.1.9/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/handlers/on_comment.py` & `sweepai-0.1.9/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/handlers/on_review.py` & `sweepai-0.1.9/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/handlers/on_ticket.py` & `sweepai-0.1.9/sweepai/handlers/on_ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,19 +129,14 @@
                 error = e
                 continue
         posthog.capture(
             username, "fetching_failed", properties={"error": error, **metadata}
         )
         raise error
 
-    # update_index.call(
-    #     repo_full_name,
-    #     installation_id=installation_id,
-    # )
-
     logger.info("Fetching relevant files...")
     try:
         snippets, tree = fetch_file_contents_with_retry()
         assert len(snippets) > 0
     except Exception as e:
         logger.error(e)
         comment_reply(
```

### Comparing `sweepai-0.1.8/sweepai/slack.py` & `sweepai-0.1.9/sweepai/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/utils/constants.py` & `sweepai-0.1.9/sweepai/utils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This file should be split into environment and config files
 """
 
-PREFIX = "prod"
+PREFIX = "dev"
 DB_NAME = PREFIX + "-db"
 API_NAME = PREFIX + "-api"
 UTILS_NAME = PREFIX + "-utils"
 SLACK_NAME = PREFIX + "-slack"
 BOT_TOKEN_NAME = PREFIX + "-bot-token"
 if PREFIX == "prod":
     BOT_TOKEN_NAME = "bot-token"
```

### Comparing `sweepai-0.1.8/sweepai/utils/diff.py` & `sweepai-0.1.9/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/utils/file_change_functions.py` & `sweepai-0.1.9/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/utils/github_utils.py` & `sweepai-0.1.9/sweepai/utils/github_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,16 +222,16 @@
 
 
 def index_full_repository(
     repo_name: str,
     installation_id: int = None,
     sweep_config: SweepConfig = SweepConfig(),
 ):
-    init_index = modal.Function.lookup(DB_NAME, "init_index")
-    num_indexed_docs = init_index.spawn(
+    update_index = modal.Function.lookup(DB_NAME, "update_index")
+    num_indexed_docs = update_index.spawn(
         repo_name=repo_name,
         installation_id=installation_id,
         sweep_config=sweep_config,
     )
     try:
         repo = get_github_client(installation_id).get_repo(repo_name)
         labels = repo.get_labels()
```

### Comparing `sweepai-0.1.8/sweepai/utils/huggingface.py` & `sweepai-0.1.9/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/utils/prompt_constructor.py` & `sweepai-0.1.9/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/utils/scorer.py` & `sweepai-0.1.9/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/utils/snippets.py` & `sweepai-0.1.9/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.1.8/sweepai/utils/utils.py` & `sweepai-0.1.9/sweepai/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,22 +23,18 @@
 class Tiktoken:
     openai_models = ["gpt-3.5-turbo", "gpt-4", "gpt-4-32k", "gpt-4-32k-0613"]
     anthropic_models = ["claude-v1", "claude-v1.3-100k", "claude-instant-v1.3-100k"]
     models = openai_models + anthropic_models
 
     def __enter__(self):
         import tiktoken
-        from anthropic import get_tokenizer
         self.openai_models = {model: tiktoken.encoding_for_model(model) for model in Tiktoken.openai_models}
-        self.anthropic_tokenizer = get_tokenizer()
 
     @method()
     def count(self, text: str, model: str = "gpt-4"):
-        if model in Tiktoken.anthropic_models:
-            return len(self.anthropic_tokenizer.encode(text).ids)
         return len(self.openai_models[model].encode(text))
 
 chunking_image = modal.Image.debian_slim() \
     .apt_install("git") \
     .pip_install("tree-sitter", "loguru")
 
 CHUNKING_CACHE_DIR = "/root/cache/"
```

### Comparing `sweepai-0.1.8/setup.py` & `sweepai-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 install_requires = \
 ['PyGithub==1.58.2',
  'config-path>=1.0.3,<2.0.0',
  'fastapi>=0.94.1,<0.95.0',
  'gradio>=3.35.2,<4.0.0',
  'loguru>=0.6.0,<0.7.0',
  'requests>=2.28.2,<3.0.0',
+ 'typer[all]>=0.9.0,<0.10.0',
  'urllib3>=2.0.3,<3.0.0',
  'uvicorn>=0.21.0,<0.22.0']
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Sweep software chores',
     'long_description': None,
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

