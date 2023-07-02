# Comparing `tmp/pymudclient-0.4.0.tar.gz` & `tmp/pymudclient-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymudclient-0.4.0.tar", last modified: Sat Jul  1 16:30:30 2023, max compression
+gzip compressed data, was "pymudclient-0.5.0.tar", last modified: Sun Jul  2 07:49:45 2023, max compression
```

## Comparing `pymudclient-0.4.0.tar` & `pymudclient-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 16:30:30.867963 pymudclient-0.4.0/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.4.0/LICENSE
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6301 2023-07-01 16:30:30.867658 pymudclient-0.4.0/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)     5630 2023-07-01 16:30:00.000000 pymudclient-0.4.0/README.md
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 16:30:30.863504 pymudclient-0.4.0/pymudclient/
--rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 12:57:57.000000 pymudclient-0.4.0/pymudclient/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      456 2023-07-01 06:34:42.000000 pymudclient-0.4.0/pymudclient/display.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     7001 2023-07-01 15:57:58.000000 pymudclient-0.4.0/pymudclient/input_cmd.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     4543 2023-07-01 16:13:21.000000 pymudclient-0.4.0/pymudclient/kbhit.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     3365 2023-07-01 16:17:10.000000 pymudclient-0.4.0/pymudclient/mud.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1924 2023-07-01 16:00:32.000000 pymudclient-0.4.0/pymudclient/recv.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/shared_data.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1396 2023-07-01 13:53:52.000000 pymudclient-0.4.0/pymudclient/tmp.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 16:30:30.867103 pymudclient-0.4.0/pymudclient/utils/
--rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/utils/__init__.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/utils/codec.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/utils/colors.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1331 2023-07-01 16:16:19.000000 pymudclient-0.4.0/pymudclient/utils/print.py
--rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pymudclient/utils/telnet.py
-drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-01 16:30:30.865368 pymudclient-0.4.0/pymudclient.egg-info/
--rw-r--r--   0 eddiehsu   (501) staff       (20)     6301 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/PKG-INFO
--rw-r--r--   0 eddiehsu   (501) staff       (20)      533 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/SOURCES.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/dependency_links.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/requires.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-07-01 16:30:30.000000 pymudclient-0.4.0/pymudclient.egg-info/top_level.txt
--rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.4.0/pyproject.toml
--rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-07-01 16:30:30.868058 pymudclient-0.4.0/setup.cfg
--rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-07-01 16:20:26.000000 pymudclient-0.4.0/setup.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-02 07:49:45.582465 pymudclient-0.5.0/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1063 2023-06-29 07:55:53.000000 pymudclient-0.5.0/LICENSE
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     8284 2023-07-02 07:49:45.581999 pymudclient-0.5.0/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     6004 2023-07-02 07:48:09.000000 pymudclient-0.5.0/README.md
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-02 07:49:45.557196 pymudclient-0.5.0/pymudclient/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      376 2023-06-29 12:57:57.000000 pymudclient-0.5.0/pymudclient/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      456 2023-06-29 13:26:20.000000 pymudclient-0.5.0/pymudclient/display.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     7001 2023-07-01 15:57:58.000000 pymudclient-0.5.0/pymudclient/input_cmd.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     4543 2023-07-01 16:13:21.000000 pymudclient-0.5.0/pymudclient/kbhit.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     3365 2023-07-01 16:17:10.000000 pymudclient-0.5.0/pymudclient/mud.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1943 2023-07-02 07:35:14.000000 pymudclient-0.5.0/pymudclient/recv.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      800 2023-06-29 07:55:53.000000 pymudclient-0.5.0/pymudclient/shared_data.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1396 2023-07-01 13:53:13.000000 pymudclient-0.5.0/pymudclient/tmp.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-02 07:49:45.580749 pymudclient-0.5.0/pymudclient/utils/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        0 2023-06-29 07:55:53.000000 pymudclient-0.5.0/pymudclient/utils/__init__.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      197 2023-06-29 07:55:53.000000 pymudclient-0.5.0/pymudclient/utils/codec.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1563 2023-06-29 07:55:53.000000 pymudclient-0.5.0/pymudclient/utils/colors.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1331 2023-07-01 16:16:19.000000 pymudclient-0.5.0/pymudclient/utils/print.py
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      483 2023-06-29 07:55:53.000000 pymudclient-0.5.0/pymudclient/utils/telnet.py
+drwxr-xr-x   0 eddiehsu   (501) staff       (20)        0 2023-07-02 07:49:45.559492 pymudclient-0.5.0/pymudclient.egg-info/
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     8284 2023-07-02 07:49:45.000000 pymudclient-0.5.0/pymudclient.egg-info/PKG-INFO
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      533 2023-07-02 07:49:45.000000 pymudclient-0.5.0/pymudclient.egg-info/SOURCES.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)        1 2023-07-02 07:49:45.000000 pymudclient-0.5.0/pymudclient.egg-info/dependency_links.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       55 2023-07-02 07:49:45.000000 pymudclient-0.5.0/pymudclient.egg-info/requires.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       12 2023-07-02 07:49:45.000000 pymudclient-0.5.0/pymudclient.egg-info/top_level.txt
+-rw-r--r--   0 eddiehsu   (501) staff       (20)      689 2023-06-29 07:55:53.000000 pymudclient-0.5.0/pyproject.toml
+-rw-r--r--   0 eddiehsu   (501) staff       (20)       38 2023-07-02 07:49:45.582635 pymudclient-0.5.0/setup.cfg
+-rw-r--r--   0 eddiehsu   (501) staff       (20)     1362 2023-07-02 07:49:25.000000 pymudclient-0.5.0/setup.py
```

### Comparing `pymudclient-0.4.0/LICENSE` & `pymudclient-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/PKG-INFO` & `pymudclient-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: pymudclient
-Version: 0.4.0
-Summary: A MUD client core written in Python
-Home-page: https://github.com/griiid/PyMudClient
-Download-URL: https://pypi.org/project/pymudclient/
-Author: griiid
-Author-email: gridwing@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # PyMudClient: 用 Python 開發的 MUD Client 核心
 
 ## 這是什麼？
 
 - MUD, Multi-User Dungeon，是多人即時虛擬類遊戲，通常以文字描述為基礎。
 - **pymudclient** 實作了連線、斷線重連、顯示、輸入介面、Alias、Trigger、Timer 的功能。
 
@@ -115,15 +95,22 @@
 
 ### Alias
 
 #### Alias class 參數
 
 - start_text `string`: Alias 的指令，可以包含空格。
 - pattern `string`: (optional) 要替換的指令，會傳到 host。
-- func `function`: (optional) 要呼叫的 function，會傳一個 `text` 參數，會把除了 start_text 外的後面的文字全部傳入；如果 function 有回傳文字，會傳給 host。
+- func `function`: (optional) 要呼叫的 function。
+  - function prototype:
+    ```py
+    def func(text: str) -> str or None:
+      ...
+    ```
+  - `text` 參數會把除了 start_text 外的後面的文字全部傳入。
+  - 如果 function 有回傳文字，會傳給 host。
 
 pattern 跟 func 2 選 1。
 
 #### 使用範例
 
 ```py
 from pymudclient import Alias
@@ -141,23 +128,31 @@
 
 ### Trigger
 
 #### Trigger class 參數
 
 - pattern `string`: 觸發的 pattern，使用 regex。
 - data `string`: (optional) 要直接送出的文字，如果是固定文字用這個就好。
-- func `function`: (optional) 要呼叫的 function，會傳一個 `match` 參數，會把 regex match 到的 `match.groups()` 傳入；如果 function 有回傳文字，會傳給 host。
+- func `function`: (optional) 要呼叫的 function。
+  - function prototype:
+    ```py
+    def func(text: str, match_group: list) -> str or None:
+        ...
+    ```
+  - `text` 參數會把有符合 trigger 條件的整行文字傳入。
+  - `match_group` 參數會把 regex match 到的 `match.groups()` 傳入
+  - 如果 function 有回傳文字，會傳給 host。
 
 #### 使用範例
 
 ```py
 from pymudclient import Trigger
 
-def summon(match):
-    return f'summon {match[0]}'
+def summon(text, match_group):
+    return f'summon {match_group[0]}'
 
 TRIGGER_LIST = [
     Trigger(r"^您的英文名字\(新人物請輸入\'new\'\) :$", data=USER),
     Trigger(r"^請輸入密碼﹕$", data=PW),
     Trigger(r'\(([a-zA-Z]+)\)告訴你﹕sum$', func=summon),
 ]
 ```
@@ -167,15 +162,21 @@
 
 ### Timer
 
 #### Timer class 參數
 
 - seconds `number`: 多久執行一次，單位是秒。
 - data `string`: (optional) 要直接送出的文字，如果是固定文字用這個就好。
-- func `function`: (optional) 要呼叫的 function；如果 function 有回傳文字，會傳給 host。
+- func `function`: (optional) 要呼叫的 function。
+  - function prototype:
+    ```py
+    def func() -> str or None:
+      ...
+    ```
+  - 如果 function 有回傳文字，會傳給 host。
 
 #### 使用範例
 
 ```py
 from pymudclient import Timer
 
 TIMER_LIST = [
```

### Comparing `pymudclient-0.4.0/pymudclient/input_cmd.py` & `pymudclient-0.5.0/pymudclient/input_cmd.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/pymudclient/kbhit.py` & `pymudclient-0.5.0/pymudclient/kbhit.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/pymudclient/mud.py` & `pymudclient-0.5.0/pymudclient/mud.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/pymudclient/recv.py` & `pymudclient-0.5.0/pymudclient/recv.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         match = re.search(trigger.pattern, content_text_only)
         if not match:
             continue
 
         if trigger.data is not None:
             send_to_host(trigger.data, display=False)
         elif trigger.func is not None:
-            data = trigger.func(match.groups())
+            data = trigger.func(content_text_only, match.groups())
             if data is not None:
                 send_to_host(data, display=False)
 
 
 IGNORE_LINES = []
```

### Comparing `pymudclient-0.4.0/pymudclient/shared_data.py` & `pymudclient-0.5.0/pymudclient/shared_data.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/pymudclient/tmp.py` & `pymudclient-0.5.0/pymudclient/tmp.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/pymudclient/utils/colors.py` & `pymudclient-0.5.0/pymudclient/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/pymudclient/utils/print.py` & `pymudclient-0.5.0/pymudclient/utils/print.py`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/pymudclient.egg-info/SOURCES.txt` & `pymudclient-0.5.0/pymudclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/pyproject.toml` & `pymudclient-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymudclient-0.4.0/setup.py` & `pymudclient-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 PACKAGE_NAME = 'pymudclient'
 AUTHOR = 'griiid'
 AUTHOR_EMAIL = 'gridwing@gmail.com'
 URL = 'https://github.com/griiid/PyMudClient'
 DOWNLOAD_URL = 'https://pypi.org/project/pymudclient/'
 
 LICENSE = 'MIT'
-VERSION = '0.4.0'
+VERSION = '0.5.0'
 DESCRIPTION = 'A MUD client core written in Python'
 LONG_DESCRIPTION = (HERE  / 'README.md').read_text(encoding='utf8')
 LONG_DESC_TYPE = 'text/markdown'
 
 requirements = (HERE / 'requirements.txt').read_text(encoding='utf8')
 INSTALL_REQUIRES = [s.strip() for s in requirements.split('\n')]
```

