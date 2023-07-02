# Comparing `tmp/khoj_assistant-0.7.1.dev10.tar.gz` & `tmp/khoj_assistant-0.7.1.dev12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Jul  2 04:37:11 2023, max compression
+gzip compressed data, last modified: Sun Jul  2 16:14:08 2023, max compression
```

## Comparing `khoj_assistant-0.7.1.dev10.tar` & `khoj_assistant-0.7.1.dev12.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/__init__.py
--rw-r--r--   0        0        0    11412 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/configure.py
--rw-r--r--   0        0        0     5379 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3532 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    14414 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     6212 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6990 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6799 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    19296 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3644 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0   205167 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6056 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13481 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7338 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5193 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    18153 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4394 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7560 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2088 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2510 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2995 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6852 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4215 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/LICENSE
--rw-r--r--   0        0        0    23398 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/README.md
--rw-r--r--   0        0        0     2841 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/pyproject.toml
--rw-r--r--   0        0        0    25805 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11412 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/configure.py
+-rw-r--r--   0        0        0     5379 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3532 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    14414 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     6212 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6990 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6799 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    19296 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3644 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0   205167 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6056 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13481 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5193 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    18153 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4394 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7560 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2088 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2510 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2995 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6852 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4215 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/LICENSE
+-rw-r--r--   0        0        0    23398 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/README.md
+-rw-r--r--   0        0        0     2841 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/pyproject.toml
+-rw-r--r--   0        0        0    25805 2023-07-02 16:14:08.000000 khoj_assistant-0.7.1.dev12/PKG-INFO
```

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/configure.py` & `khoj_assistant-0.7.1.dev12/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/main.py` & `khoj_assistant-0.7.1.dev12/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.1.dev12/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Standard Packages
 import glob
 import logging
 import re
+import urllib3
 from pathlib import Path
 from typing import List
 
 # Internal Packages
 from khoj.processor.text_to_jsonl import TextToJsonl
 from khoj.utils.helpers import get_absolute_path, is_none_or_empty, timer
 from khoj.utils.constants import empty_escape_sequences
@@ -141,15 +142,16 @@
         "Convert each Markdown entries into a dictionary"
         entries = []
         for parsed_entry in parsed_entries:
             raw_filename = entry_to_file_map[parsed_entry]
 
             # Check if raw_filename is a URL. If so, save it as is. If not, convert it to a Path.
             if type(raw_filename) == str and re.search(r"^https?://", raw_filename):
-                entry_filename = raw_filename
+                # Escape the URL to avoid issues with special characters
+                entry_filename = urllib3.util.parse_url(raw_filename).url
             else:
                 entry_filename = str(Path(raw_filename))
             stem = Path(raw_filename).stem
 
             heading = parsed_entry.splitlines()[0] if re.search("^#+\s", parsed_entry) else ""
             # Append base filename to compiled entry for context to model
             # Increment heading level for heading entries and make filename as its top level heading
```

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.1.dev12/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/routers/api.py` & `khoj_assistant-0.7.1.dev12/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/routers/api_beta.py` & `khoj_assistant-0.7.1.dev12/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.1.dev12/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.1.dev12/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.1.dev12/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.1.dev12/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.1.dev12/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.1.dev12/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.1.dev12/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/utils/cli.py` & `khoj_assistant-0.7.1.dev12/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/utils/config.py` & `khoj_assistant-0.7.1.dev12/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/utils/constants.py` & `khoj_assistant-0.7.1.dev12/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.1.dev12/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.1.dev12/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/utils/models.py` & `khoj_assistant-0.7.1.dev12/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.1.dev12/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/utils/state.py` & `khoj_assistant-0.7.1.dev12/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.1.dev12/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/.gitignore` & `khoj_assistant-0.7.1.dev12/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/LICENSE` & `khoj_assistant-0.7.1.dev12/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/README.md` & `khoj_assistant-0.7.1.dev12/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/pyproject.toml` & `khoj_assistant-0.7.1.dev12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.1.dev10/PKG-INFO` & `khoj_assistant-0.7.1.dev12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.1.dev10
+Version: 0.7.1.dev12
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

