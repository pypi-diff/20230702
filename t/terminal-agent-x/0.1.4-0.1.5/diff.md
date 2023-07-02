# Comparing `tmp/terminal-agent-x-0.1.4.tar.gz` & `tmp/terminal-agent-x-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal-agent-x-0.1.4.tar", last modified: Tue Jun 13 04:41:26 2023, max compression
+gzip compressed data, was "terminal-agent-x-0.1.5.tar", last modified: Sun Jul  2 16:51:48 2023, max compression
```

## Comparing `terminal-agent-x-0.1.4.tar` & `terminal-agent-x-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4128 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3246 2023-06-13 04:40:45.000000 terminal-agent-x-0.1.4/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      976 2023-06-13 04:37:46.000000 terminal-agent-x-0.1.4/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-13 04:41:26.167598 terminal-agent-x-0.1.4/terminal_agent_x/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.4/terminal_agent_x/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6973 2023-06-13 04:17:58.000000 terminal-agent-x-0.1.4/terminal_agent_x/tax.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4128 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      302 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-06-13 04:41:26.000000 terminal-agent-x-0.1.4/terminal_agent_x.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-13 04:41:26.171598 terminal-agent-x-0.1.4/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      498 2023-06-06 16:47:27.000000 terminal-agent-x-0.1.4/tests/test.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    35149 2023-05-08 10:01:27.000000 terminal-agent-x-0.1.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4099 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3217 2023-07-02 16:48:43.000000 terminal-agent-x-0.1.5/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      976 2023-07-02 16:41:45.000000 terminal-agent-x-0.1.5/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-02 16:51:48.646097 terminal-agent-x-0.1.5/terminal_agent_x/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-09 00:14:06.000000 terminal-agent-x-0.1.5/terminal_agent_x/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7077 2023-07-02 16:37:25.000000 terminal-agent-x-0.1.5/terminal_agent_x/tax.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4099 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      302 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       50 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       17 2023-07-02 16:51:48.000000 terminal-agent-x-0.1.5/terminal_agent_x.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-02 16:51:48.650097 terminal-agent-x-0.1.5/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      498 2023-06-06 16:47:27.000000 terminal-agent-x-0.1.5/tests/test.py
```

### Comparing `terminal-agent-x-0.1.4/LICENSE` & `terminal-agent-x-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal-agent-x-0.1.4/PKG-INFO` & `terminal-agent-x-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.4
+Version: 0.1.5
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Project-URL: Wiki, https://github.com/LyuLumos/Terminal-Agent-X/wiki
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -26,70 +26,58 @@
 
 ```bash
 pip install terminal-agent-x
 ```
 
 ## Config
 
-You need to add the environment variable `OpenAI_KEY` to the path.
-
-```bash
-# On Linux
-vim ~/.bashrc
-# add this line to the end of the file
-export OpenAI_KEY=sk-xxx
-# save and execute
-source ~/.bashrc
-
-# For Windows, you can google how to set environment variables on Windows.
-```
+You need to add the environment variable `OpenAI_KEY` to the path. Please get your `OpenAI_KEY` from [OpenAI](https://platform.openai.com/account/api-keys).
 
 Use `python -c "import os;print(os.environ.get('OpenAI_KEY'))"` for testing.
 
-You can get your `OpenAI_KEY` from [OpenAI](https://platform.openai.com/account/api-keys).
-
 
 ## Get Started
 
-You can use the `tax <prompt>` to interact with the model, like this:
+You can use the `tax <prompt>` to interact with the model, like:
 
 ```
-tax write a python code for fibonacci
+$ tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
 usage: tax.py [-h] [-k KEY] [--model MODEL] [-i INPUT] [-o OUTPUT] [--url URL] [--show_all] prompt [prompt ...]
 
 Tax: A terminal agent using OpenAI/Claude API
 
 positional arguments:
   prompt                Prompt
 
 options:
   -h, --help            show this help message and exit
   -k KEY, --key KEY     Your key for OpenAI/Claude.
-  --model MODEL         Model name. Choose from gpt-3.5/4s, claude or DALLE.
+  --model MODEL         Model name. Choose from gpt-3.5/4s or DALLE.
   -i INPUT, --input INPUT
                         Input file. If specified, the prompt will be read from the file.
   -o OUTPUT, --output OUTPUT
                         Output file. If specified, the response will be saved to the file.
-  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be
-                        accessd under GFW.
+  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url.
   --show_all            Show all contents in the response.
 ```
 
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
 
+Anthropic Claude API in not available since July 2023. Please use OpenAI API instead.
+
 ## License
 
 [GNU General Public License v3.0](LICENSE)
 
 ## Development Logs
 
 <details>
@@ -128,7 +116,13 @@
 <details>
 <summary>0.1.4</summary>
 
 - Feat: Add support for reading prompt from file.
 - Feat: Add support for OpenAI DALL·E.
 - Fix: Resolve the bug of curl command on Windows platform using IPv6 address to access Claude.
 </details>
+
+<details>
+<summary>0.1.5</summary>
+
+- Fix: Change api to a third-party proxy. Affected by GFW's DNS domain pollution, the original proxy is temporarily unavailable.
+</details>
```

### Comparing `terminal-agent-x-0.1.4/README.md` & `terminal-agent-x-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,70 +6,58 @@
 
 ```bash
 pip install terminal-agent-x
 ```
 
 ## Config
 
-You need to add the environment variable `OpenAI_KEY` to the path.
-
-```bash
-# On Linux
-vim ~/.bashrc
-# add this line to the end of the file
-export OpenAI_KEY=sk-xxx
-# save and execute
-source ~/.bashrc
-
-# For Windows, you can google how to set environment variables on Windows.
-```
+You need to add the environment variable `OpenAI_KEY` to the path. Please get your `OpenAI_KEY` from [OpenAI](https://platform.openai.com/account/api-keys).
 
 Use `python -c "import os;print(os.environ.get('OpenAI_KEY'))"` for testing.
 
-You can get your `OpenAI_KEY` from [OpenAI](https://platform.openai.com/account/api-keys).
-
 
 ## Get Started
 
-You can use the `tax <prompt>` to interact with the model, like this:
+You can use the `tax <prompt>` to interact with the model, like:
 
 ```
-tax write a python code for fibonacci
+$ tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
 usage: tax.py [-h] [-k KEY] [--model MODEL] [-i INPUT] [-o OUTPUT] [--url URL] [--show_all] prompt [prompt ...]
 
 Tax: A terminal agent using OpenAI/Claude API
 
 positional arguments:
   prompt                Prompt
 
 options:
   -h, --help            show this help message and exit
   -k KEY, --key KEY     Your key for OpenAI/Claude.
-  --model MODEL         Model name. Choose from gpt-3.5/4s, claude or DALLE.
+  --model MODEL         Model name. Choose from gpt-3.5/4s or DALLE.
   -i INPUT, --input INPUT
                         Input file. If specified, the prompt will be read from the file.
   -o OUTPUT, --output OUTPUT
                         Output file. If specified, the response will be saved to the file.
-  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be
-                        accessd under GFW.
+  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url.
   --show_all            Show all contents in the response.
 ```
 
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
 
+Anthropic Claude API in not available since July 2023. Please use OpenAI API instead.
+
 ## License
 
 [GNU General Public License v3.0](LICENSE)
 
 ## Development Logs
 
 <details>
@@ -107,8 +95,14 @@
 
 <details>
 <summary>0.1.4</summary>
 
 - Feat: Add support for reading prompt from file.
 - Feat: Add support for OpenAI DALL·E.
 - Fix: Resolve the bug of curl command on Windows platform using IPv6 address to access Claude.
+</details>
+
+<details>
+<summary>0.1.5</summary>
+
+- Fix: Change api to a third-party proxy. Affected by GFW's DNS domain pollution, the original proxy is temporarily unavailable.
 </details>
```

### Comparing `terminal-agent-x-0.1.4/pyproject.toml` & `terminal-agent-x-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal-agent-x"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="LyuLumos", email="lyujiuyang0@gmail.com" },
 ]
 
 description = "A terminal agent for terminal users."
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `terminal-agent-x-0.1.4/terminal_agent_x/tax.py` & `terminal-agent-x-0.1.5/terminal_agent_x/tax.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,23 +81,26 @@
     ]
     terminal_headers = [
         f"Authorization='Bearer {openai_key}'",
         "'Content-Type'='application/json'"
     ]
 
     urls = {
-        'openai_gfw': 'https://api.lyulumos.space/v1/chat/completions',
+        'openai_gfw': 'https://api.openai-proxy.com/v1/chat/completions',
         'openai': 'https://api.openai.com/v1/chat/completions',
-        'claude': 'https://claude-api.lyulumos.space/v1/chat/completions'
+        # 'claude': 'https://claude-api.lyulumos.space/v1/chat/completions'
     }
-    url_option = 'claude' if model == 'claude' else url_option
+    # url_option = 'claude' if model == 'claude' else url_option
+    # claude API is not accessible
+    if model == 'claude':
+        assert False, 'Claude API is not accessible now. Please use OpenAI API instead.'
     url = urls[url_option] if url_option in urls else url_option
 
     if model.lower() == 'dalle':
-        url = 'https://api.lyulumos.space/v1/images/generations' if url_option == 'openai_gfw' else 'https://api.openai.com/v1/images/generations'
+        url = 'https://api.openai-proxy.com/v1/images/generations' if url_option == 'openai_gfw' else 'https://api.openai.com/v1/images/generations'
         data = f'{{"prompt": "{prompt}"}}'
     else:
         data = f'{{"model": "{model}","messages": [{{"role": "user", "content": "{prompt}"}}]}}'
     return url, headers, terminal_headers, data
 
 
 def find_code(text: str) -> str:
@@ -119,21 +122,21 @@
 def main() -> None:
     parser = argparse.ArgumentParser(
         description='Tax: A terminal agent using OpenAI/Claude API')
     parser.add_argument("prompt", nargs='+', type=str, help="Prompt")
     parser.add_argument('-k', '--key', type=str,
                         help='Your key for OpenAI/Claude.')
     parser.add_argument('--model', type=str,
-                        default='gpt-3.5-turbo', help='Model name. Choose from gpt-3.5/4s, claude or DALLE.')
+                        default='gpt-3.5-turbo', help='Model name. Choose from gpt-3.5/4s or DALLE.')
     parser.add_argument('-i', '--input', type=str,
                         help='Input file. If specified, the prompt will be read from the file.')
     parser.add_argument('-o', '--output', type=str,
                         help='Output file. If specified, the response will be saved to the file.')
-    parser.add_argument('--url', type=str, default='openai_gfw',
-                        help="URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be accessd under GFW.")
+    parser.add_argument('--url', type=str, default='openai',
+                        help="URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url.")
     parser.add_argument('--show_all', action='store_true',
                         help='Show all contents in the response.')
     args = parser.parse_args()
 
     prompt = ' '.join(args.prompt)
     prompt = f'{prompt}\\n{load_file(args.input)}' if args.input else prompt
```

### Comparing `terminal-agent-x-0.1.4/terminal_agent_x.egg-info/PKG-INFO` & `terminal-agent-x-0.1.5/terminal_agent_x.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-agent-x
-Version: 0.1.4
+Version: 0.1.5
 Summary: A terminal agent for terminal users.
 Author-email: LyuLumos <lyujiuyang0@gmail.com>
 Project-URL: Homepage, https://github.com/LyuLumos/Terminal-Agent-X
 Project-URL: Bug Tracker, https://github.com/LyuLumos/Terminal-Agent-X/issues
 Project-URL: Wiki, https://github.com/LyuLumos/Terminal-Agent-X/wiki
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -26,70 +26,58 @@
 
 ```bash
 pip install terminal-agent-x
 ```
 
 ## Config
 
-You need to add the environment variable `OpenAI_KEY` to the path.
-
-```bash
-# On Linux
-vim ~/.bashrc
-# add this line to the end of the file
-export OpenAI_KEY=sk-xxx
-# save and execute
-source ~/.bashrc
-
-# For Windows, you can google how to set environment variables on Windows.
-```
+You need to add the environment variable `OpenAI_KEY` to the path. Please get your `OpenAI_KEY` from [OpenAI](https://platform.openai.com/account/api-keys).
 
 Use `python -c "import os;print(os.environ.get('OpenAI_KEY'))"` for testing.
 
-You can get your `OpenAI_KEY` from [OpenAI](https://platform.openai.com/account/api-keys).
-
 
 ## Get Started
 
-You can use the `tax <prompt>` to interact with the model, like this:
+You can use the `tax <prompt>` to interact with the model, like:
 
 ```
-tax write a python code for fibonacci
+$ tax write a python code for fibonacci
 ```
 
 Use `tax -h` to get more information.
 ```bash
 usage: tax.py [-h] [-k KEY] [--model MODEL] [-i INPUT] [-o OUTPUT] [--url URL] [--show_all] prompt [prompt ...]
 
 Tax: A terminal agent using OpenAI/Claude API
 
 positional arguments:
   prompt                Prompt
 
 options:
   -h, --help            show this help message and exit
   -k KEY, --key KEY     Your key for OpenAI/Claude.
-  --model MODEL         Model name. Choose from gpt-3.5/4s, claude or DALLE.
+  --model MODEL         Model name. Choose from gpt-3.5/4s or DALLE.
   -i INPUT, --input INPUT
                         Input file. If specified, the prompt will be read from the file.
   -o OUTPUT, --output OUTPUT
                         Output file. If specified, the response will be saved to the file.
-  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url. The default one can be
-                        accessd under GFW.
+  --url URL             URL for API request. Choose from ['openai_gfw', 'openai', 'claude'] or your custom url.
   --show_all            Show all contents in the response.
 ```
 
 ## Attention
 
 You can see a directive after the generated command that says
 ```
 Do you want to execute the command? (y/n)
 ```
 Please execute it or not at your own discretion. I am not responsible for the consequences of generated commands.
 
+Anthropic Claude API in not available since July 2023. Please use OpenAI API instead.
+
 ## License
 
 [GNU General Public License v3.0](LICENSE)
 
 ## Development Logs
 
 <details>
@@ -128,7 +116,13 @@
 <details>
 <summary>0.1.4</summary>
 
 - Feat: Add support for reading prompt from file.
 - Feat: Add support for OpenAI DALL·E.
 - Fix: Resolve the bug of curl command on Windows platform using IPv6 address to access Claude.
 </details>
+
+<details>
+<summary>0.1.5</summary>
+
+- Fix: Change api to a third-party proxy. Affected by GFW's DNS domain pollution, the original proxy is temporarily unavailable.
+</details>
```

