# Comparing `tmp/sweepai-0.2.0.tar.gz` & `tmp/sweepai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.2.0.tar", max compression
+gzip compressed data, was "sweepai-0.2.1.tar", max compression
```

## Comparing `sweepai-0.2.0.tar` & `sweepai-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.0/LICENSE
--rw-r--r--   0        0        0     3595 2023-07-02 05:30:42.090895 sweepai-0.2.0/README.md
--rw-r--r--   0        0        0     1133 2023-07-02 07:30:30.847953 sweepai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.0/sweepai/__init__.py
--rw-r--r--   0        0        0    10664 2023-07-01 23:29:41.701470 sweepai-0.2.0/sweepai/api.py
--rw-r--r--   0        0        0     5893 2023-07-02 07:30:30.847953 sweepai-0.2.0/sweepai/app/api_client.py
--rw-r--r--   0        0        0     6995 2023-07-02 07:30:30.847953 sweepai-0.2.0/sweepai/app/backend.py
--rw-r--r--   0        0        0      741 2023-07-02 07:30:30.847953 sweepai-0.2.0/sweepai/app/cli.py
--rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.0/sweepai/app/config.py
--rw-r--r--   0        0        0     8941 2023-07-02 07:30:30.847953 sweepai-0.2.0/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.0/sweepai/core/__init__.py
--rw-r--r--   0        0        0    16077 2023-07-02 07:30:30.847953 sweepai-0.2.0/sweepai/core/chat.py
--rw-r--r--   0        0        0     2553 2023-07-01 23:29:41.701470 sweepai-0.2.0/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     7286 2023-07-02 07:30:30.847953 sweepai-0.2.0/sweepai/core/entities.py
--rw-r--r--   0        0        0    13033 2023-07-01 23:29:41.701470 sweepai-0.2.0/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3509 2023-07-01 23:29:41.701470 sweepai-0.2.0/sweepai/core/react.py
--rw-r--r--   0        0        0    15487 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12030 2023-07-02 07:30:30.847953 sweepai-0.2.0/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    11177 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0    19497 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/slack.py
--rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/utils/__init__.py
--rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/utils/config.py
--rw-r--r--   0        0        0      670 2023-07-02 07:30:30.847953 sweepai-0.2.0/sweepai/utils/constants.py
--rw-r--r--   0        0        0     3633 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/utils/diff.py
--rw-r--r--   0        0        0      511 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8984 2023-07-02 07:30:30.847953 sweepai-0.2.0/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      902 2023-07-02 07:30:30.851287 sweepai-0.2.0/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.0/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11266 2023-07-01 23:29:41.708137 sweepai-0.2.0/sweepai/utils/utils.py
--rw-r--r--   0        0        0     4651 2023-07-02 07:30:37.382656 sweepai-0.2.0/setup.py
--rw-r--r--   0        0        0     4143 2023-07-02 07:30:37.383226 sweepai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3682 2023-07-02 21:27:52.322803 sweepai-0.2.1/README.md
+-rw-r--r--   0        0        0     1133 2023-07-02 21:42:21.413411 sweepai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.1/sweepai/__init__.py
+-rw-r--r--   0        0        0    10664 2023-07-01 23:29:41.701470 sweepai-0.2.1/sweepai/api.py
+-rw-r--r--   0        0        0     5893 2023-07-02 07:30:30.847953 sweepai-0.2.1/sweepai/app/api_client.py
+-rw-r--r--   0        0        0     6995 2023-07-02 07:30:30.847953 sweepai-0.2.1/sweepai/app/backend.py
+-rw-r--r--   0        0        0      741 2023-07-02 07:30:30.847953 sweepai-0.2.1/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3311 2023-07-01 23:29:41.701470 sweepai-0.2.1/sweepai/app/config.py
+-rw-r--r--   0        0        0     9658 2023-07-02 21:45:04.116856 sweepai-0.2.1/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.701470 sweepai-0.2.1/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    16077 2023-07-02 07:30:30.847953 sweepai-0.2.1/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2553 2023-07-01 23:29:41.701470 sweepai-0.2.1/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     7286 2023-07-02 07:30:30.847953 sweepai-0.2.1/sweepai/core/entities.py
+-rw-r--r--   0        0        0    13033 2023-07-01 23:29:41.701470 sweepai-0.2.1/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3509 2023-07-01 23:29:41.701470 sweepai-0.2.1/sweepai/core/react.py
+-rw-r--r--   0        0        0    15487 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12030 2023-07-02 07:30:30.847953 sweepai-0.2.1/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     2536 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     5906 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     3423 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    11177 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0    19497 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/slack.py
+-rw-r--r--   0        0        0        0 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0      385 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/utils/config.py
+-rw-r--r--   0        0        0      670 2023-07-02 07:30:30.847953 sweepai-0.2.1/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     3633 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      507 2023-07-02 21:36:52.379851 sweepai-0.2.1/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8166 2023-07-02 21:45:23.803536 sweepai-0.2.1/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5339 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      902 2023-07-02 07:30:30.851287 sweepai-0.2.1/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-01 23:29:41.704803 sweepai-0.2.1/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11266 2023-07-01 23:29:41.708137 sweepai-0.2.1/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     4740 2023-07-02 21:45:38.055674 sweepai-0.2.1/setup.py
+-rw-r--r--   0        0        0     4230 2023-07-02 21:45:38.056548 sweepai-0.2.1/PKG-INFO
```

### Comparing `sweepai-0.2.0/LICENSE` & `sweepai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/README.md` & `sweepai-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
     <img src=".assets/sweep-banner-github.png">
 </p>
 <p align="center">
     <i>Spend time reviewing code generated by AI, not writing it.</i>
 </p>
 
 <p align="center">
+<a href="https://sweep.dev/">🌐 Website</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.sweep.dev/">📚 Docs</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://discord.gg/sweep-ai">📢 Discord</a>
 </p>
 
 <b>Sweep</b> allows you to create and review GitHub issues with easy.
 Simply describe any issue and Sweep will do the rest.
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                        [.assets/sweep-banner-github.png]
           Spend time reviewing code generated by AI, not writing it.
-                        ð_Docs   â¢   ð¢_Discord
+              ð_Website   â¢   ð_Docs   â¢   ð¢_Discord
 Sweep allows you to create and review GitHub issues with easy. Simply describe
 any issue and Sweep will do the rest. It will plan out what needs to be done,
 what changes to make, and write the changes to a PR. --- ## â¨ Demo For the
 best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of
 your repos and see the magic happen. [Demo](https://github.com/sweepai/sweep/
 assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47) ## ð Getting Started
 ### ð¥ï¸ Sweep Chat Sweep Chat allows you to interact with Sweep locally and
```

### Comparing `sweepai-0.2.0/pyproject.toml` & `sweepai-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.2.0"
+version = "0.2.1"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `sweepai-0.2.0/sweepai/api.py` & `sweepai-0.2.1/sweepai/api.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/app/api_client.py` & `sweepai-0.2.1/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/app/backend.py` & `sweepai-0.2.1/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/app/cli.py` & `sweepai-0.2.1/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/app/config.py` & `sweepai-0.2.1/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/app/ui.py` & `sweepai-0.2.1/sweepai/app/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import gradio as gr
 from loguru import logger
 import webbrowser
 
 from sweepai.app.api_client import APIClient, create_pr_function, create_pr_function_call
 from sweepai.app.config import SweepChatConfig
 from sweepai.core.entities import Snippet
-from sweepai.utils.constants import DB_NAME
-from sweepai.utils.github_utils import get_files_recursively
 
 config = SweepChatConfig.load()
 
 api_client = APIClient(config=config)
 
 pr_summary_template = """💡 I'll create the following PR:
 
@@ -37,14 +35,36 @@
 }
 #snippets {
     height: 750px;
     overflow-y: scroll;
 }
 """
 
+def get_files_recursively(repo, path=''):
+    path_to_contents = {}
+    try:
+        contents = repo.get_contents(path)
+        files = []
+        while contents:
+            file_content = contents.pop(0)
+            if file_content.type == 'dir':
+                contents.extend(repo.get_contents(file_content.path))
+            else:
+                try:
+                    decoded_contents = file_content.decoded_content.decode("utf-8")
+                except:
+                    continue
+                if decoded_contents:
+                    path_to_contents[file_content.path] = file_content.decoded_content.decode("utf-8")
+                    files.append(file_content.path)
+        return sorted(files), path_to_contents
+    except Exception as e:
+        logger.error(e)
+        return [], path_to_contents
+
 with gr.Blocks(theme=gr.themes.Soft(), title="Sweep Chat", css=css) as demo:
     with gr.Row():
         with gr.Column():
             repo_full_name = gr.Dropdown(choices=[repo.full_name for repo in repos], label="Repo full name", value=config.repo_full_name or "")
         with gr.Column(scale=2):
             repo = github_client.get_repo(config.repo_full_name)
             all_files, path_to_contents = get_files_recursively(repo)
```

### Comparing `sweepai-0.2.0/sweepai/core/chat.py` & `sweepai-0.2.1/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/core/code_repair.py` & `sweepai-0.2.1/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/core/entities.py` & `sweepai-0.2.1/sweepai/core/entities.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/core/prompts.py` & `sweepai-0.2.1/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/core/react.py` & `sweepai-0.2.1/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/core/sweep_bot.py` & `sweepai-0.2.1/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/core/vector_db.py` & `sweepai-0.2.1/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/events.py` & `sweepai-0.2.1/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/handlers/create_pr.py` & `sweepai-0.2.1/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/handlers/on_comment.py` & `sweepai-0.2.1/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/handlers/on_review.py` & `sweepai-0.2.1/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/handlers/on_ticket.py` & `sweepai-0.2.1/sweepai/handlers/on_ticket.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/slack.py` & `sweepai-0.2.1/sweepai/slack.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/utils/constants.py` & `sweepai-0.2.1/sweepai/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/utils/diff.py` & `sweepai-0.2.1/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/utils/file_change_functions.py` & `sweepai-0.2.1/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/utils/github_utils.py` & `sweepai-0.2.1/sweepai/utils/github_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 import os
 import time
 import re
 import github
 from github import Github
 from github.Repository import Repository
 from loguru import logger
-from git import Repo
 
 from jwt import encode
 import requests
 from tqdm import tqdm
 from sweepai.core.entities import Snippet
 from sweepai.utils.config import SweepConfig
 from sweepai.utils.constants import APP_ID, DB_NAME
 from sweepai.utils.event_logger import posthog
 
-
 def make_valid_string(string: str):
     pattern = r"[^\w./-]+"
     return re.sub(pattern, "_", string)
 
 
 def get_jwt():
     signing_key = os.environ["GITHUB_APP_PEM"]
@@ -126,14 +124,15 @@
 #     shutil.rmtree("repo")
 #     return tree
 def get_tree_and_file_list(
     repo_name: str, 
     installation_id: int, 
     snippet_paths: list[str]
 ) -> str:
+    from git import Repo
     token = get_token(installation_id)
     shutil.rmtree("repo", ignore_errors=True)
     repo_url = f"https://x-access-token:{token}@github.com/{repo_name}.git"
     Repo.clone_from(repo_url, "repo")
 
     prefixes = []
     for snippet_path in snippet_paths:
@@ -246,29 +245,7 @@
             )
     except Exception as e:
         posthog("index_full_repository", "failed", {"error": str(e)})
         logger.warning(
             "Adding label failed, probably because label already."
         )  # warn that the repo may already be indexed
     return num_indexed_docs
-
-def get_files_recursively(repo, path=''):
-    path_to_contents = {}
-    try:
-        contents = repo.get_contents(path)
-        files = []
-        while contents:
-            file_content = contents.pop(0)
-            if file_content.type == 'dir':
-                contents.extend(repo.get_contents(file_content.path))
-            else:
-                try:
-                    decoded_contents = file_content.decoded_content.decode("utf-8")
-                except:
-                    continue
-                if decoded_contents:
-                    path_to_contents[file_content.path] = file_content.decoded_content.decode("utf-8")
-                    files.append(file_content.path)
-        return sorted(files), path_to_contents
-    except Exception as e:
-        logger.error(e)
-        return [], path_to_contents
```

### Comparing `sweepai-0.2.0/sweepai/utils/huggingface.py` & `sweepai-0.2.1/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/utils/prompt_constructor.py` & `sweepai-0.2.1/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/utils/scorer.py` & `sweepai-0.2.1/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/utils/snippets.py` & `sweepai-0.2.1/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/sweepai/utils/utils.py` & `sweepai-0.2.1/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.2.0/setup.py` & `sweepai-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Sweep software chores',
-    'long_description': '<p align="center">\n    <img src=".assets/sweep-banner-github.png">\n</p>\n<p align="center">\n    <i>Spend time reviewing code generated by AI, not writing it.</i>\n</p>\n\n<p align="center">\n<a href="https://docs.sweep.dev/">📚 Docs</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://discord.gg/sweep-ai">📢 Discord</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with easy.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src=".assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n\n## 🌠 Features\n* Automatic feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
+    'long_description': '<p align="center">\n    <img src=".assets/sweep-banner-github.png">\n</p>\n<p align="center">\n    <i>Spend time reviewing code generated by AI, not writing it.</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev/">🌐 Website</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://docs.sweep.dev/">📚 Docs</a>\n<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>\n<a href="https://discord.gg/sweep-ai">📢 Discord</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with easy.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src=".assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n\n## 🌠 Features\n* Automatic feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created\n* Code snippets embedding-based search\n* Chain-of-Thought retrieval using GPT Functions\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n---\n\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['PyGithub==1.58.2', 'config-
 path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0', 'loguru>=0.6.0,<0.7.0',
 'requests>=2.28.2,<3.0.0', 'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0']
 entry_points = \ {'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai =
-sweepai.app.cli:app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.2.0',
+sweepai.app.cli:app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.2.1',
 'description': 'Sweep software chores', 'long_description': '
                     \n [.assets/sweep-banner-github.png]\n
 \n
         \n Spend time reviewing code generated by AI, not writing it.\n
 \n\n
-                     \nð_Docs\n  â¢  \nð¢_Discord\n
+          \nð_Website\n  â¢  \nð_Docs\n  â¢  \nð¢_Discord\n
 \n\nSweep allows you to create and review GitHub issues with easy.\nSimply
 describe any issue and Sweep will do the rest.\nIt will plan out what needs to
 be done, what changes to make, and write the changes to a PR. \n\n---\n\n## â¨
 Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-
 ai) to one of your repos and see the magic happen.\n\n[Demo](https://
 github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
 0af02f2b0e47)\n\n## ð Getting Started\n\n### ð¥ï¸ Sweep Chat\nSweep Chat
```

### Comparing `sweepai-0.2.0/PKG-INFO` & `sweepai-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.2.0
+Version: 0.2.1
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.58.2)
 Requires-Dist: config-path (>=1.0.3,<2.0.0)
@@ -19,14 +19,16 @@
     <img src=".assets/sweep-banner-github.png">
 </p>
 <p align="center">
     <i>Spend time reviewing code generated by AI, not writing it.</i>
 </p>
 
 <p align="center">
+<a href="https://sweep.dev/">🌐 Website</a>
+<span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.sweep.dev/">📚 Docs</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://discord.gg/sweep-ai">📢 Discord</a>
 </p>
 
 <b>Sweep</b> allows you to create and review GitHub issues with easy.
 Simply describe any issue and Sweep will do the rest.
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.2.0 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.2.1 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.11,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path (>=1.0.3,<2.0.0)
 Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: typer
 (>=0.9.0,<0.10.0) Requires-Dist: urllib3 (>=2.0.3,<3.0.0) Description-Content-
 Type: text/markdown
                        [.assets/sweep-banner-github.png]
           Spend time reviewing code generated by AI, not writing it.
-                        ð_Docs   â¢   ð¢_Discord
+              ð_Website   â¢   ð_Docs   â¢   ð¢_Discord
 Sweep allows you to create and review GitHub issues with easy. Simply describe
 any issue and Sweep will do the rest. It will plan out what needs to be done,
 what changes to make, and write the changes to a PR. --- ## â¨ Demo For the
 best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of
 your repos and see the magic happen. [Demo](https://github.com/sweepai/sweep/
 assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47) ## ð Getting Started
 ### ð¥ï¸ Sweep Chat Sweep Chat allows you to interact with Sweep locally and
```

