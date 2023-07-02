# Comparing `tmp/khoj_assistant-0.7.0.tar.gz` & `tmp/khoj_assistant-0.7.1.dev10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Jul  1 12:44:22 2023, max compression
+gzip compressed data, last modified: Sun Jul  2 04:37:11 2023, max compression
```

## Comparing `khoj_assistant-0.7.0.tar` & `khoj_assistant-0.7.1.dev10.tar`

### file list

```diff
@@ -1,80 +1,78 @@
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/__init__.py
--rw-r--r--   0        0        0    11337 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/configure.py
--rw-r--r--   0        0        0     4956 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2987 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/file_browser.py
--rw-r--r--   0        0        0      987 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/labelled_text_field.py
--rw-r--r--   0        0        0    17819 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1316 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3532 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    14414 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0     6212 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6990 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     6799 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    19296 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3644 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0   205167 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     6056 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     4386 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     6478 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13768 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/ledger/__init__.py
--rw-r--r--   0        0        0     5708 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/ledger/beancount_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7338 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5193 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    18153 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1941 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4394 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7560 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2112 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2510 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2995 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6852 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4215 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/LICENSE
--rw-r--r--   0        0        0    23224 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/README.md
--rw-r--r--   0        0        0     2841 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    25625 2023-07-01 12:44:22.000000 khoj_assistant-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11412 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/configure.py
+-rw-r--r--   0        0        0     5379 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3532 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    14414 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0     6212 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6990 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     6799 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    19296 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3644 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0   205167 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     6056 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     4386 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     6478 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13481 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/ledger/__init__.py
+-rw-r--r--   0        0        0     5708 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/ledger/beancount_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7338 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5193 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    18153 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1941 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     4394 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7560 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2088 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2510 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2995 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6852 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4215 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/LICENSE
+-rw-r--r--   0        0        0    23398 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/README.md
+-rw-r--r--   0        0        0     2841 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/pyproject.toml
+-rw-r--r--   0        0        0    25805 2023-07-02 04:37:11.000000 khoj_assistant-0.7.1.dev10/PKG-INFO
```

### Comparing `khoj_assistant-0.7.0/src/khoj/configure.py` & `khoj_assistant-0.7.1.dev10/src/khoj/configure.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 
 logger = logging.getLogger(__name__)
 
 
 def configure_server(args, required=False):
     if args.config is None:
         if required:
-            logger.error(f"Exiting as Khoj is not configured.\nConfigure it via GUI or by editing {state.config_file}.")
+            logger.error(
+                f"Exiting as Khoj is not configured.\nConfigure it via http://localhost:8000/config or by editing {state.config_file}."
+            )
             sys.exit(1)
         else:
             logger.warning(
-                f"Khoj is not configured.\nConfigure it via khoj GUI, plugins or by editing {state.config_file}."
+                f"Khoj is not configured.\nConfigure it via http://localhost:8000/config, plugins or by editing {state.config_file}."
             )
             return
     else:
         state.config = args.config
 
     # Initialize Processor from Config
     state.processor_config = configure_processor(args.config.processor)
```

### Comparing `khoj_assistant-0.7.0/src/khoj/main.py` & `khoj_assistant-0.7.1.dev10/src/khoj/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import signal
 import sys
 import logging
 import threading
 import warnings
 from platform import system
+import webbrowser
 
 # Ignore non-actionable warnings
 warnings.filterwarnings("ignore", message=r"snapshot_download.py has been made private", category=FutureWarning)
 warnings.filterwarnings("ignore", message=r"legacy way to download files from the HF hub,", category=FutureWarning)
 
 # External Packages
 import uvicorn
@@ -59,25 +60,28 @@
     # Set Log File
     fh = logging.FileHandler(state.config_file.parent / "khoj.log", encoding="utf-8")
     fh.setLevel(logging.DEBUG)
     logger.addHandler(fh)
 
     logger.info("🌘 Starting Khoj")
 
-    if args.no_gui:
-        # Setup task scheduler
-        poll_task_scheduler()
+    if not args.gui:
+        if not state.demo:
+            # Setup task scheduler
+            poll_task_scheduler()
+
         # Start Server
         configure_server(args, required=False)
         configure_routes(app)
         start_server(app, host=args.host, port=args.port, socket=args.socket)
     else:
+        logger.warning("🚧 GUI is being deprecated and may not work as expected. Starting...")
         # Setup GUI
         gui = QtWidgets.QApplication([])
-        main_window = MainWindow(args.config_file)
+        main_window = MainWindow(args.host, args.port)
 
         # System tray is only available on Windows, MacOS.
         # On Linux (Gnome) the System tray is not supported.
         # Since only the Main Window is available
         # Quitting it should quit the application
         if system() in ["Windows", "Darwin"]:
             gui.setQuitOnLastWindowClosed(False)
@@ -85,14 +89,21 @@
             tray.show()
 
         # Setup Server
         configure_server(args, required=False)
         configure_routes(app)
         server = ServerThread(app, args.host, args.port, args.socket)
 
+        url = f"http://{args.host}:{args.port}"
+        logger.info(f"🌗 Khoj is running at {url}")
+        try:
+            webbrowser.open(url)
+        except:
+            logger.warning("🚧 Unable to open browser. Please open it manually to configure Khoj.")
+
         # Show Main Window on First Run Experience or if on Linux
         if args.config is None or system() not in ["Windows", "Darwin"]:
             main_window.show()
 
         # Setup Signal Handlers
         signal.signal(signal.SIGINT, sigint_handler)
         # Invoke Python interpreter every 500ms to handle signals, run scheduled tasks
```

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/desktop/system_tray.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     tray = QtWidgets.QSystemTrayIcon(icon)
     tray.setVisible(True)
 
     # Create the menu and menu actions
     menu = QtWidgets.QMenu()
     menu_actions = [
         ("Search", lambda: webbrowser.open(f"http://{state.host}:{state.port}/")),
-        ("Configure", main_window.show_on_top),
+        ("Configure", lambda: webbrowser.open(f"http://{state.host}:{state.port}/config")),
+        ("App", main_window.show),
         ("Quit", gui.quit),
     ]
 
     # Add the menu actions to the menu
     for action_text, action_function in menu_actions:
         menu_action = QtGui.QAction(action_text, menu)
         menu_action.triggered.connect(action_function)  # type: ignore[attr-defined]
```

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.1.dev10/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/github/github_to_jsonl.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,25 +35,21 @@
             logger.info(f"Github Rate limit reached. Waiting for {wait_time} seconds")
             time.sleep(wait_time)
             return func(*args, **kwargs)
         else:
             return
 
     def process(self, previous_entries=None):
-        # If demo mode is enabled, don't re-process any of the repositories. This is resource intensive.
-        if state.demo and previous_entries is not None:
-            return self.update_entries_with_ids(previous_entries, previous_entries)
-
         current_entries = []
         for repo in self.config.repos:
-            current_entries += self.process_repo(repo, previous_entries)
+            current_entries += self.process_repo(repo)
 
         return self.update_entries_with_ids(current_entries, previous_entries)
 
-    def process_repo(self, repo: GithubRepoConfig, previous_entries=None):
+    def process_repo(self, repo: GithubRepoConfig):
         repo_url = f"https://api.github.com/repos/{repo.owner}/{repo.name}"
         repo_shorthand = f"{repo.owner}/{repo.name}"
         logger.info(f"Processing github repo {repo_shorthand}")
         with timer("Download markdown files from github repo", logger):
             try:
                 markdown_files, org_files = self.get_files(repo_url, repo)
             except Exception as e:
```

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/ledger/beancount_to_jsonl.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/ledger/beancount_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.1.dev10/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/routers/api.py` & `khoj_assistant-0.7.1.dev10/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/routers/api_beta.py` & `khoj_assistant-0.7.1.dev10/src/khoj/routers/api_beta.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.1.dev10/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.1.dev10/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.1.dev10/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.1.dev10/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.1.dev10/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.1.dev10/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.1.dev10/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/utils/cli.py` & `khoj_assistant-0.7.1.dev10/src/khoj/utils/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
     # Setup Argument Parser for the Commandline Interface
     parser = argparse.ArgumentParser(
         description="Start Khoj; A Natural Language Search Engine for your personal Notes, Transactions and Photos"
     )
     parser.add_argument(
         "--config-file", "-c", default="~/.khoj/khoj.yml", type=pathlib.Path, help="YAML file to configure Khoj"
     )
-    parser.add_argument(
-        "--no-gui", action="store_true", default=False, help="Do not show native desktop GUI. Default: false"
-    )
+    parser.add_argument("--gui", action="store_true", default=False, help="Show native desktop GUI. Default: false")
     parser.add_argument(
         "--regenerate",
         action="store_true",
         default=False,
         help="Regenerate model embeddings from source files. Default: false",
     )
     parser.add_argument("--verbose", "-v", action="count", default=0, help="Show verbose conversion logs. Default: 0")
```

### Comparing `khoj_assistant-0.7.0/src/khoj/utils/config.py` & `khoj_assistant-0.7.1.dev10/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/utils/constants.py` & `khoj_assistant-0.7.1.dev10/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.1.dev10/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.1.dev10/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/utils/models.py` & `khoj_assistant-0.7.1.dev10/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.1.dev10/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/utils/state.py` & `khoj_assistant-0.7.1.dev10/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.1.dev10/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/.gitignore` & `khoj_assistant-0.7.1.dev10/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/LICENSE` & `khoj_assistant-0.7.1.dev10/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/README.md` & `khoj_assistant-0.7.1.dev10/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,21 +69,25 @@
 
 ## Demos
 ### Khoj in Obsidian
 https://github.com/khoj-ai/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
-- Install Khoj via `pip` and start Khoj backend in non-gui mode
-- Install Khoj plugin via Community Plugins settings pane on Obsidian app
-- Check the new Khoj plugin settings
-- Let Khoj backend index the markdown, pdf, Github markdown files in the current Vault
-- Open Khoj plugin on Obsidian via Search button on Left Pane
-- Search \"*Announce plugin to folks*\" in the [Obsidian Plugin docs](https://marcus.se.net/obsidian-plugin-docs/)
-- Jump to the [search result](https://marcus.se.net/obsidian-plugin-docs/publishing/submit-your-plugin)
+1. Install Khoj via `pip` and start Khoj backend in a terminal (Run `khoj`)
+    ```
+    python -m pip install khoj-assistant
+    khoj
+    ```
+2. Install Khoj plugin via Community Plugins settings pane on Obsidian app
+    - Check the new Khoj plugin settings
+    - Let Khoj backend index the markdown, pdf, Github markdown files in the current Vault
+    - Open Khoj plugin on Obsidian via Search button on Left Pane
+    - Search \"*Announce plugin to folks*\" in the [Obsidian Plugin docs](https://marcus.se.net/obsidian-plugin-docs/)
+    - Jump to the [search result](https://marcus.se.net/obsidian-plugin-docs/publishing/submit-your-plugin)
 </details>
 
 ### Khoj in Emacs, Browser
 https://user-images.githubusercontent.com/6413477/184735169-92c78bf1-d827-4663-9087-a1ea194b8f4b.mp4
 
 <details><summary>Description</summary>
 
@@ -156,15 +160,15 @@
 ## Use
 ### Khoj Search
 - **Khoj via Obsidian**
   - Click the *Khoj search* icon 🔎 on the [Ribbon](https://help.obsidian.md/User+interface/Workspace/Ribbon) or Search for *Khoj: Search* in the [Command Palette](https://help.obsidian.md/Plugins/Command+palette)
 - **Khoj via Emacs**
   - Run `M-x khoj <user-query>`
 - **Khoj via Web**
-  - Open <http://localhost:8000/> via desktop interface or directly
+  - Open <http://localhost:8000/> directly
 - **Khoj via API**
   - See the Khoj FastAPI [Swagger Docs](http://localhost:8000/docs), [ReDocs](http://localhost:8000/redocs)
 
 <details><summary>Query Filters</summary>
 
 Use structured query syntax to filter the natural language search results
 - **Word Filter**: Get entries that include/exclude a specified term
@@ -304,16 +308,15 @@
 
   2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
 
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
- - Open the Khoj desktop GUI, add your [OpenAI API key](https://beta.openai.com/account/api-keys) and click *Configure*
-   Ensure khoj is started **without** the `--no-gui` flag. Check your system tray to see if Khoj is minimized there.
+ - Open your [Khoj settings](http://localhost:8000/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:8000/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
     processor:
       conversation:
     -    openai-api-key: # "YOUR_OPENAI_API_KEY"
     +    openai-api-key: sk-aaaaaaaaaaaaaaaaaaaaaaaahhhhhhhhhhhhhhhhhhhhhhhh
         model: "text-davinci-003"
@@ -384,15 +387,15 @@
 
 ##### 2. Run
 1. Start Khoj
    ```shell
    khoj -vv
    ```
 2. Configure Khoj
-   - **Via GUI**: Add files, directories to index in the GUI window that pops up on starting Khoj, then Click Configure
+   - **Via the Settings UI**: Add files, directories to index the [Khoj settings](http://localhost:8000/config) UI once Khoj has started up. Once you've saved all your settings, click `Configure`.
    - **Manually**:
      - Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
      - Set `input-files` or `input-filter` in each relevant `content-type` section of `~/.khoj/khoj.yml`
        - Set `input-directories` field in `image` `content-type` section
      - Delete `content-type` and `processor` sub-section(s) irrelevant for your use-case
      - Restart khoj
```

### Comparing `khoj_assistant-0.7.0/pyproject.toml` & `khoj_assistant-0.7.1.dev10/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.0/PKG-INFO` & `khoj_assistant-0.7.1.dev10/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.0
+Version: 0.7.1.dev10
 Summary: A natural language search engine for your personal notes, transactions and images
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -127,21 +127,25 @@
 
 ## Demos
 ### Khoj in Obsidian
 https://github.com/khoj-ai/khoj/assets/6413477/3e33d8ea-25bb-46c8-a3bf-c92f78d0f56b
 
 <details><summary>Description</summary>
 
-- Install Khoj via `pip` and start Khoj backend in non-gui mode
-- Install Khoj plugin via Community Plugins settings pane on Obsidian app
-- Check the new Khoj plugin settings
-- Let Khoj backend index the markdown, pdf, Github markdown files in the current Vault
-- Open Khoj plugin on Obsidian via Search button on Left Pane
-- Search \"*Announce plugin to folks*\" in the [Obsidian Plugin docs](https://marcus.se.net/obsidian-plugin-docs/)
-- Jump to the [search result](https://marcus.se.net/obsidian-plugin-docs/publishing/submit-your-plugin)
+1. Install Khoj via `pip` and start Khoj backend in a terminal (Run `khoj`)
+    ```
+    python -m pip install khoj-assistant
+    khoj
+    ```
+2. Install Khoj plugin via Community Plugins settings pane on Obsidian app
+    - Check the new Khoj plugin settings
+    - Let Khoj backend index the markdown, pdf, Github markdown files in the current Vault
+    - Open Khoj plugin on Obsidian via Search button on Left Pane
+    - Search \"*Announce plugin to folks*\" in the [Obsidian Plugin docs](https://marcus.se.net/obsidian-plugin-docs/)
+    - Jump to the [search result](https://marcus.se.net/obsidian-plugin-docs/publishing/submit-your-plugin)
 </details>
 
 ### Khoj in Emacs, Browser
 https://user-images.githubusercontent.com/6413477/184735169-92c78bf1-d827-4663-9087-a1ea194b8f4b.mp4
 
 <details><summary>Description</summary>
 
@@ -214,15 +218,15 @@
 ## Use
 ### Khoj Search
 - **Khoj via Obsidian**
   - Click the *Khoj search* icon 🔎 on the [Ribbon](https://help.obsidian.md/User+interface/Workspace/Ribbon) or Search for *Khoj: Search* in the [Command Palette](https://help.obsidian.md/Plugins/Command+palette)
 - **Khoj via Emacs**
   - Run `M-x khoj <user-query>`
 - **Khoj via Web**
-  - Open <http://localhost:8000/> via desktop interface or directly
+  - Open <http://localhost:8000/> directly
 - **Khoj via API**
   - See the Khoj FastAPI [Swagger Docs](http://localhost:8000/docs), [ReDocs](http://localhost:8000/redocs)
 
 <details><summary>Query Filters</summary>
 
 Use structured query syntax to filter the natural language search results
 - **Word Filter**: Get entries that include/exclude a specified term
@@ -362,16 +366,15 @@
 
   2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
 
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
- - Open the Khoj desktop GUI, add your [OpenAI API key](https://beta.openai.com/account/api-keys) and click *Configure*
-   Ensure khoj is started **without** the `--no-gui` flag. Check your system tray to see if Khoj is minimized there.
+ - Open your [Khoj settings](http://localhost:8000/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:8000/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
     processor:
       conversation:
     -    openai-api-key: # "YOUR_OPENAI_API_KEY"
     +    openai-api-key: sk-aaaaaaaaaaaaaaaaaaaaaaaahhhhhhhhhhhhhhhhhhhhhhhh
         model: "text-davinci-003"
@@ -442,15 +445,15 @@
 
 ##### 2. Run
 1. Start Khoj
    ```shell
    khoj -vv
    ```
 2. Configure Khoj
-   - **Via GUI**: Add files, directories to index in the GUI window that pops up on starting Khoj, then Click Configure
+   - **Via the Settings UI**: Add files, directories to index the [Khoj settings](http://localhost:8000/config) UI once Khoj has started up. Once you've saved all your settings, click `Configure`.
    - **Manually**:
      - Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
      - Set `input-files` or `input-filter` in each relevant `content-type` section of `~/.khoj/khoj.yml`
        - Set `input-directories` field in `image` `content-type` section
      - Delete `content-type` and `processor` sub-section(s) irrelevant for your use-case
      - Restart khoj
```

