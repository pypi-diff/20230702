# Comparing `tmp/pymino-1.2.2.4.tar.gz` & `tmp/pymino-1.2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\New folder\pymino\dist\.tmp-esawe27c\pymino-1.2.2.4.tar", last modified: Wed Jun 28 10:21:37 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino push\dist\.tmp-zf55okvu\pymino-1.2.2.5.tar", last modified: Sun Jul  2 21:06:08 2023, max compression
```

## Comparing `pymino-1.2.2.4.tar` & `pymino-1.2.2.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 10:21:37.165024 pymino-1.2.2.4/
--rw-rw-rw-   0        0        0     1085 2023-06-28 09:49:18.000000 pymino-1.2.2.4/LICENSE
--rw-rw-rw-   0        0        0     7424 2023-06-28 10:21:37.165518 pymino-1.2.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-06-28 10:21:17.000000 pymino-1.2.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 10:21:37.089630 pymino-1.2.2.4/pymino/
--rw-rw-rw-   0        0        0      721 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/__init__.py
--rw-rw-rw-   0        0        0    11011 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/async_bot.py
--rw-rw-rw-   0        0        0    30258 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/bot.py
--rw-rw-rw-   0        0        0    36824 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-06-28 10:21:37.127327 pymino-1.2.2.4/pymino/ext/
--rw-rw-rw-   0        0        0      528 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    11196 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/account.py
--rw-rw-rw-   0        0        0   343766 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    21404 2023-06-28 10:17:31.000000 pymino-1.2.2.4/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25866 2023-06-28 10:17:41.000000 pymino-1.2.2.4/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7238 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   342510 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/console.py
--rw-rw-rw-   0        0        0    45497 2023-06-28 10:17:36.000000 pymino-1.2.2.4/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1856 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-06-28 10:21:37.152126 pymino-1.2.2.4/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    15640 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43596 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4802 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1839 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0    70180 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/global_client.py
--rw-rw-rw-   0        0        0      543 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6657 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-06-28 10:21:37.164032 pymino-1.2.2.4/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11320 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1110 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10322 2023-06-28 09:49:18.000000 pymino-1.2.2.4/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-28 10:21:37.105999 pymino-1.2.2.4/pymino.egg-info/
--rw-rw-rw-   0        0        0     7424 2023-06-28 10:21:37.000000 pymino-1.2.2.4/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1555 2023-06-28 10:21:37.000000 pymino-1.2.2.4/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 10:21:37.000000 pymino-1.2.2.4/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-06-28 10:21:37.000000 pymino-1.2.2.4/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-28 10:21:37.000000 pymino-1.2.2.4/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-06-28 10:21:37.171966 pymino-1.2.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-06-28 09:49:18.000000 pymino-1.2.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.376103 pymino-1.2.2.5/
+-rw-rw-rw-   0        0        0     1085 2023-06-28 09:49:18.000000 pymino-1.2.2.5/LICENSE
+-rw-rw-rw-   0        0        0     7424 2023-07-02 21:06:08.376599 pymino-1.2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-06-28 10:21:17.000000 pymino-1.2.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.281367 pymino-1.2.2.5/pymino/
+-rw-rw-rw-   0        0        0      721 2023-07-01 20:52:00.000000 pymino-1.2.2.5/pymino/__init__.py
+-rw-rw-rw-   0        0        0    11727 2023-07-02 15:44:24.000000 pymino-1.2.2.5/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    30988 2023-07-02 15:43:21.000000 pymino-1.2.2.5/pymino/bot.py
+-rw-rw-rw-   0        0        0    36824 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.321047 pymino-1.2.2.5/pymino/ext/
+-rw-rw-rw-   0        0        0      528 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/_global.py
+-rw-rw-rw-   0        0        0    11196 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   343766 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    21408 2023-07-02 15:57:37.000000 pymino-1.2.2.5/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25886 2023-07-02 15:58:45.000000 pymino-1.2.2.5/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7238 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   342679 2023-07-02 15:30:17.000000 pymino-1.2.2.5/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    45528 2023-07-02 20:56:56.000000 pymino-1.2.2.5/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1856 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.349815 pymino-1.2.2.5/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    15825 2023-07-02 15:04:30.000000 pymino-1.2.2.5/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43596 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4802 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    70299 2023-07-02 15:19:03.000000 pymino-1.2.2.5/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     6657 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.375111 pymino-1.2.2.5/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11357 2023-07-02 15:09:23.000000 pymino-1.2.2.5/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1110 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10322 2023-06-28 09:49:18.000000 pymino-1.2.2.5/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:06:08.299223 pymino-1.2.2.5/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7424 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1555 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 21:06:08.000000 pymino-1.2.2.5/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-07-02 21:06:08.379574 pymino-1.2.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-06-28 09:49:18.000000 pymino-1.2.2.5/setup.py
```

### Comparing `pymino-1.2.2.4/LICENSE` & `pymino-1.2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/PKG-INFO` & `pymino-1.2.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.2.4
+Version: 1.2.2.5
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.2.4 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.2.5 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.2.4/README.md` & `pymino-1.2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/__init__.py` & `pymino-1.2.2.5/pymino/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.2.4'
+__version__ = '1.2.2.5'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.2.2.4/pymino/async_bot.py` & `pymino-1.2.2.5/pymino/async_bot.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,22 +16,27 @@
         community_id: Union[str, int] = None,
         device_id: Optional[str] = None,
         intents: bool = False,
         online_status: bool = False,
         proxy: Optional[str] = None
         ):
         self.loop:              asyncio.AbstractEventLoop = asyncio.get_event_loop()
+        self._cooldown_message  = None
         self._debug:            bool = check_debugger()
         self._intents:          bool = intents
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
+
         self.command_prefix:    Optional[str] = command_prefix
+        if self.command_prefix == "":
+            raise InvalidCommandPrefix()
+
         self.community_id:      Union[str, int] = community_id
         self.online_status:     bool = online_status
         self.device_id:         Optional[str] = device_id or generate_device_id()
         self.request:           AsyncRequestHandler = AsyncRequestHandler(
                                 bot = self,
                                 loop = self.loop,
                                 proxy=proxy
@@ -49,15 +54,14 @@
     def debug(self) -> bool:
         return self._debug
 
     @debug.setter
     def debug(self, value: bool) -> None:
         self._debug = value
 
-
     @property
     def intents(self) -> bool:
         return self._intents
     
     @intents.setter
     def intents(self, value: bool) -> None:
         self._intents = value
@@ -85,14 +89,29 @@
         return self._sid
 
     @sid.setter
     def sid(self, value: str) -> None:
         self._sid = value
 
 
+    def set_cooldown_message(self, message: str) -> None:
+        """
+        Changes the default cooldown message.
+        
+        :param message: The message to set as the default cooldown message.
+        :type message: str
+        :return: None
+        
+        This method changes the default cooldown message. The default cooldown message is used when a command is on cooldown
+        
+        **Note:** This method only sets the default cooldown message and cannot be used to retrieve the default cooldown message.
+        """
+        self._cooldown_message = message
+
+
     async def authenticate(self, email: str, password: str, device_id: str=None) -> dict:
         if device_id:
             self.device_id = device_id
 
         return ApiResponse(await self.request.handler(
             method="POST",
             url = "/g/s/auth/login",
```

### Comparing `pymino-1.2.2.4/pymino/bot.py` & `pymino-1.2.2.5/pymino/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,21 +217,26 @@
         intents: bool = False,
         online_status: bool = False,
         proxy: str = None
         ):
         
         self._debug:            bool = check_debugger()
         self._console_enabled:  bool = console_enabled
+        self._cooldown_message  = None
         self._intents:          bool = intents
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
+
         self.command_prefix:    Optional[str] = command_prefix
+        if self.command_prefix == "":
+            raise InvalidCommandPrefix()
+        
         self.community_id:      Union[str, int] = community_id
         self.online_status:     bool = online_status
         self.device_id:         Optional[str] = device_id or generate_device_id()
         self.request:           RequestHandler = RequestHandler(
                                 bot = self,
                                 proxy=proxy
                                 )
@@ -453,14 +458,29 @@
         posting messages or retrieving user information.
 
         **Note:** This setter only sets the session ID and cannot be used to retrieve the session ID. To retrieve the session
         ID, use the `self.sid` property.
         """
         self._sid = value
 
+    
+    def set_cooldown_message(self, message: str) -> None:
+        """
+        Changes the default cooldown message.
+        
+        :param message: The message to set as the default cooldown message.
+        :type message: str
+        :return: None
+        
+        This method changes the default cooldown message. The default cooldown message is used when a command is on cooldown
+        
+        **Note:** This method only sets the default cooldown message and cannot be used to retrieve the default cooldown message.
+        """
+        self._cooldown_message = message
+
 
     def authenticate(self, email: str, password: str, device_id: str=None) -> dict:
         """
         Authenticates the bot with the provided email and password.
 
         :param email: The email to use to log in.
         :type email: str
```

### Comparing `pymino-1.2.2.4/pymino/client.py` & `pymino-1.2.2.5/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/__init__.py` & `pymino-1.2.2.5/pymino/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/account.py` & `pymino-1.2.2.5/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/async_community.py` & `pymino-1.2.2.5/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/async_context.py` & `pymino-1.2.2.5/pymino/ext/async_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         ```
         """
         if not self.intents:
             raise IntentsNotEnabled
 
         start = time()
 
-        with self.cache as cache:
+        with self.bot.cache as cache:
             while time() - start < timeout:
                 cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
 
                 if cached_message == message:
                     cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
                     return 200
```

### Comparing `pymino-1.2.2.4/pymino/ext/async_event_handler.py` & `pymino-1.2.2.5/pymino/ext/async_event_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     `**Parameters**``
     - `session` - The session we are using.
 
     """
     def __init__(self):
         self.command_prefix:    str = self.command_prefix
         self._events:           dict = {}
-        self._wait_for:         Cache = Cache("cache")
         self._commands:         Commands = Commands()
         self.context:           AsyncContext = AsyncContext
 
 
     def register_event(self, event_name: str) -> Callable:
         def decorator(event_handler: Callable) -> Callable:
             self._events[event_name] = event_handler
@@ -64,17 +63,18 @@
                 await func(self.community)
 
             await asyncio.sleep(interval)
 
 
     def task(self, interval: int = 10):
         def decorator(func: Callable) -> Callable:
-            async def wrapper(interval: int):
+            async def wrapper():
                 await self._handle_task(func, interval)
-            self.loop.create_task(wrapper(interval=interval))
+            self.loop.create_task(wrapper())
+            return func
         return decorator
 
 
     async def _set_parameters(self, context: AsyncContext, func: Callable, message: str = None) -> list:
         try:
             message = message if isinstance(message, str) else context.message.content
         except AttributeError:
@@ -213,21 +213,22 @@
     def fetch_command(self, command_name: str) -> Command:
         return self._commands.fetch_command(command_name)
 
 
     async def _handle_command(self, data: Message, context: AsyncContext):
         """Handles commands."""
         command_name = next(iter(data.content[len(self.command_prefix):].split(" ")))
-
+        
         message = data.content[len(self.command_prefix) + len(command_name) + 1:]
         command = self._commands.fetch_command(command_name)
 
         if command is None:
             if command_name == "help" and data.content == f"{self.command_prefix}help":
-                return await context.reply(self._commands.__help__())
+                cooldown_message = self._cooldown_message or self._commands.__help__()
+                return context.reply(content=cooldown_message)
             
             if self._events.get("text_message"):
                 return await self._handle_all_events(event="text_message", data=data, context=context)
 
         if data.content[:len(self.command_prefix)] != self.command_prefix:
             return None
 
@@ -256,17 +257,17 @@
                 userId=data.author.userId
                 )
 
         return 200
 
 
     def _add_cache(self, chatId: str, userId: str, content: str):
-        with self._wait_for as cache:
+        with self.cache as cache:
             if cache.get(f"{chatId}_{userId}") is not None:
-                self._wait_for.clear(f"{chatId}_{userId}")
+                self.cache.clear(f"{chatId}_{userId}")
 
             cache.add(
                 key=f"{chatId}_{userId}",
                 value=content,
                 expire=90
                 )
```

### Comparing `pymino-1.2.2.4/pymino/ext/async_socket.py` & `pymino-1.2.2.5/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/community.py` & `pymino-1.2.2.5/pymino/ext/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -4263,20 +4263,20 @@
         return ApiResponse(self.session.handler(
             method = "POST",
             url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}"
             ))
 
 
     @community
-    def leave_chat(self, chatId: str, comId: Union[str, int] = None) -> ApiResponse:
+    def leave_chat(self, chatId: Union[str, List[str]], comId: Union[str, int] = None) -> ApiResponse:
         """
-        Leaves a chat.
+        Leaves a chat or multiple chats.
 
-        :param chatId: The ID of the chat to leave.
-        :type chatId: str
+        :param chatId: A list of chat thread IDs to leave or a single chat thread ID to leave.
+        :type chatId: Union[str, List[str]]
         :param comId: The ID of the community where the chat is located. If not provided, the current community ID is used.
         :type comId: Union[str, int]
         :return: An `ApiResponse` object containing information about the request status.
         :rtype: ApiResponse
 
         The `community` decorator is used to ensure that the user is logged in and the community ID is present.
 
@@ -4287,23 +4287,24 @@
         - `duration`: The duration of the API request.
         - `timestamp`: The timestamp of the API request.
 
         **Example usage:**
 
         To leave a chat with ID "0000-0000-0000-0000" in the current community:
 
-        >>> response = client.community.leave_chat(chatId="0000-0000-0000-0000")
+        >>> response = client.community.leave_chat(chatId=["0000-0000-0000-0000", "1111-1111-1111-1111"])
         ... if response.statuscode == 0:
         ...     print("Left chat successfully!")
         ... else:
         ...     print("Failed to leave chat.")
         """
+
         return ApiResponse(self.session.handler(
             method = "DELETE",
-            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/{chatId}/member/{self.userId}"
+            url = f"/x{self.community_id if comId is None else comId}/s/chat/thread/leave?threadIds={','.join(chatId) if isinstance(chatId, list) else chatId}"
             ))
 
 
     @community
     def kick(self, userId: str, chatId: str, allowRejoin: bool = True, comId: Union[str, int] = None) -> ApiResponse:
         """
         Kicks a user from a chat.
```

### Comparing `pymino-1.2.2.4/pymino/ext/console.py` & `pymino-1.2.2.5/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/context.py` & `pymino-1.2.2.5/pymino/ext/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         ```
         """
         if not self.intents:
             raise IntentsNotEnabled
 
         start = time()
 
-        with self.cache as cache:
+        with self.bot.cache as cache:
             while time() - start < timeout:
                 cached_message = cache.get(f"{self.message.chatId}_{self.message.author.userId}")
 
                 if cached_message == message:
                     cache.clear(f"{self.message.chatId}_{self.message.author.userId}")
                     return 200
 
@@ -616,15 +616,14 @@
     `**Parameters**``
     - `session` - The session we are using.
 
     """
     def __init__(self):
         self.command_prefix:    str = self.command_prefix
         self._events:           dict = {}
-        self._wait_for:         Cache = Cache("cache")
         self._commands:         Commands = Commands()
         self.context:           Context = Context
 
 
     def register_event(self, event_name: str) -> Callable:
         def decorator(event_handler: Callable) -> Callable:
             self._events[event_name] = event_handler
@@ -825,18 +824,19 @@
 
     def _handle_command(self, data: Message, context: Context):
         """Handles commands."""
         command_name = next(iter(data.content[len(self.command_prefix):].split(" ")))
 
         message = data.content[len(self.command_prefix) + len(command_name) + 1:]
         command = self._commands.fetch_command(command_name)
-
+    
         if command is None:
             if command_name == "help" and data.content == f"{self.command_prefix}help":
-                return context.reply(self._commands.__help__())
+                cooldown_message = self._cooldown_message or self._commands.__help__()
+                return context.reply(content=cooldown_message)
             
             if self._events.get("text_message"):
                 return self._handle_all_events(event="text_message", data=data, context=context)
 
         if data.content[:len(self.command_prefix)] != self.command_prefix:
             return None
 
@@ -865,17 +865,17 @@
                 userId=data.author.userId
                 )
 
         return 200
 
 
     def _add_cache(self, chatId: str, userId: str, content: str):
-        with self._wait_for as cache:
+        with self.cache as cache:
             if cache.get(f"{chatId}_{userId}") is not None:
-                self._wait_for.clear(f"{chatId}_{userId}")
+                self.cache.clear(f"{chatId}_{userId}")
 
             cache.add(
                 key=f"{chatId}_{userId}",
                 value=content,
                 expire=90
                 )
```

### Comparing `pymino-1.2.2.4/pymino/ext/dispatcher.py` & `pymino-1.2.2.5/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/acm.py` & `pymino-1.2.2.5/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/admin_log.py` & `pymino-1.2.2.5/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/api_response.py` & `pymino-1.2.2.5/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/bubble.py` & `pymino-1.2.2.5/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/chat_threads.py` & `pymino-1.2.2.5/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/comments.py` & `pymino-1.2.2.5/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/enums.py` & `pymino-1.2.2.5/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/exceptions.py` & `pymino-1.2.2.5/pymino/ext/entities/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,7 +493,13 @@
             )
         
 class IntentsNotEnabled(Exception):
     def __init__(self):
         super().__init__(
             "Intents are not enabled. Please enable them in your Bot instance and try again."
             )
+
+class InvalidCommandPrefix(Exception):
+    def __init__(self):
+        super().__init__(
+            "Invalid command prefix. Please provide a valid command prefix."
+            )
```

### Comparing `pymino-1.2.2.4/pymino/ext/entities/general.py` & `pymino-1.2.2.5/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/handlers.py` & `pymino-1.2.2.5/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/link_info.py` & `pymino-1.2.2.5/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/member.py` & `pymino-1.2.2.5/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/messages.py` & `pymino-1.2.2.5/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/notification.py` & `pymino-1.2.2.5/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/sticker.py` & `pymino-1.2.2.5/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/threads.py` & `pymino-1.2.2.5/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/userprofile.py` & `pymino-1.2.2.5/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/entities/wsevents.py` & `pymino-1.2.2.5/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/global_client.py` & `pymino-1.2.2.5/pymino/ext/global_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1634,32 +1634,32 @@
         return ApiResponse(self.make_request(
             method="POST",
             url=f"/g/s/chat/thread/{chatId}/member/{self.userId}"
             ))
 
 
     @authenticated
-    def leave_chat(self, chatId: str) -> ApiResponse:
+    def leave_chat(self, chatId: Union[str, List[str]]) -> ApiResponse:
         """
         Removes the authenticated user from a chat thread.
 
-        :param chatId: The ID of the chat thread to leave.
-        :type chatId: str
+        :param chatId: A list of chat thread IDs to leave or a single chat thread ID to leave.
+        :type chatId: Union[str, List[str]]
         :return: The API response.
         :rtype: ApiResponse
 
         This method removes the authenticated user from a chat thread. The user must be a member of the chat thread in order
         to leave it.
 
         **Note:** This method requires authentication. If the client is not authenticated, a `LoginRequired` exception will
         be raised.
         """
         return ApiResponse(self.make_request(
             method="DELETE",
-            url=f"/g/s/chat/thread/{chatId}/member/{self.userId}"
+            url = f"/g/s/chat/thread/leave?threadIds={','.join(chatId) if isinstance(chatId, list) else chatId}"
             ))
 
 
     @authenticated
     def join_community(self, community_id: int, invitationId = None) -> ApiResponse:
         """
         Joins the user to a community with the provided community ID.
```

### Comparing `pymino-1.2.2.4/pymino/ext/handle_queue.py` & `pymino-1.2.2.5/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/socket.py` & `pymino-1.2.2.5/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.2.5/pymino/ext/utilities/async_request_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,427 +282,429 @@
 00001190: 2020 2043 6c69 656e 7452 6573 706f 6e73     ClientRespons
 000011a0: 6545 7272 6f72 2c0d 0a20 2020 2020 2020  eError,..       
 000011b0: 2020 2020 2043 6c69 656e 7448 7474 7050       ClientHttpP
 000011c0: 726f 7879 4572 726f 722c 0d0a 2020 2020  roxyError,..    
 000011d0: 2020 2020 2020 2020 5753 5365 7276 6572          WSServer
 000011e0: 4861 6e64 7368 616b 6545 7272 6f72 2c0d  HandshakeError,.
 000011f0: 0a20 2020 2020 2020 2029 3a0d 0a20 2020  .        ):..   
-00001200: 2020 2020 2020 2020 2061 7761 6974 2073           await s
-00001210: 656c 662e 6861 6e64 6c65 7228 6d65 7468  elf.handler(meth
-00001220: 6f64 2c20 7572 6c2c 2064 6174 612c 2063  od, url, data, c
-00001230: 6f6e 7465 6e74 5f74 7970 6529 0d0a 0d0a  ontent_type)....
-00001240: 0d0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
-00001250: 6861 6e64 6c65 7228 0d0a 2020 2020 2020  handler(..      
-00001260: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
-00001270: 2020 2020 2020 2020 206d 6574 686f 643a           method:
-00001280: 2073 7472 2c0d 0a20 2020 2020 2020 2020   str,..         
-00001290: 2020 2075 726c 3a20 7374 722c 0d0a 2020     url: str,..  
-000012a0: 2020 2020 2020 2020 2020 6461 7461 3a20            data: 
-000012b0: 556e 696f 6e5b 6469 6374 2c20 6279 7465  Union[dict, byte
-000012c0: 732c 204e 6f6e 655d 203d 204e 6f6e 652c  s, None] = None,
-000012d0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-000012e0: 6e74 656e 745f 7479 7065 3a20 4f70 7469  ntent_type: Opti
-000012f0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
-00001300: 0d0a 2020 2020 2920 2d3e 2064 6963 743a  ..    ) -> dict:
-00001310: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001320: 2020 2020 2020 2060 6861 6e64 6c65 7260         `handler`
-00001330: 202d 2048 616e 646c 6573 2061 6c6c 2072   - Handles all r
-00001340: 6571 7565 7374 730d 0a0d 0a20 2020 2020  equests....     
-00001350: 2020 2060 2a2a 5061 7261 6d65 7465 7273     `**Parameters
-00001360: 2a2a 6060 0d0a 2020 2020 2020 2020 2d20  **``..        - 
-00001370: 606d 6574 686f 6460 202d 2054 6865 2072  `method` - The r
-00001380: 6571 7565 7374 206d 6574 686f 6420 746f  equest method to
-00001390: 2075 7365 2e0d 0a20 2020 2020 2020 202d   use...        -
-000013a0: 2060 7572 6c60 202d 2054 6865 2075 726c   `url` - The url
-000013b0: 2074 6f20 7365 6e64 2074 6865 2072 6571   to send the req
-000013c0: 7565 7374 2074 6f2e 0d0a 2020 2020 2020  uest to...      
-000013d0: 2020 2d20 6064 6174 6160 202d 2054 6865    - `data` - The
-000013e0: 2064 6174 6120 746f 2073 656e 6420 7769   data to send wi
-000013f0: 7468 2074 6865 2072 6571 7565 7374 2e0d  th the request..
-00001400: 0a20 2020 2020 2020 202d 2060 636f 6e74  .        - `cont
-00001410: 656e 745f 7479 7065 6020 2d20 5468 6520  ent_type` - The 
-00001420: 636f 6e74 656e 7420 7479 7065 206f 6620  content type of 
-00001430: 7468 6520 6461 7461 2e0d 0a0d 0a20 2020  the data.....   
-00001440: 2020 2020 2060 2a2a 5265 7475 726e 732a       `**Returns*
-00001450: 2a60 600d 0a20 2020 2020 2020 202d 2060  *``..        - `
-00001460: 6469 6374 6020 2d20 5468 6520 7265 7370  dict` - The resp
-00001470: 6f6e 7365 2066 726f 6d20 7468 6520 7265  onse from the re
-00001480: 7175 6573 742e 0d0a 0d0a 2020 2020 2020  quest.....      
-00001490: 2020 2222 220d 0a20 2020 2020 2020 2075    """..        u
-000014a0: 726c 203d 2073 656c 662e 7365 7276 6963  rl = self.servic
-000014b0: 655f 7572 6c28 7572 6c29 0d0a 0d0a 2020  e_url(url)....  
-000014c0: 2020 2020 2020 7572 6c2c 2068 6561 6465        url, heade
-000014d0: 7273 2c20 6269 6e61 7279 5f64 6174 6120  rs, binary_data 
-000014e0: 3d20 6177 6169 7420 7365 6c66 2e73 6572  = await self.ser
-000014f0: 7669 6365 5f68 616e 646c 6572 2875 726c  vice_handler(url
-00001500: 2c20 6461 7461 2c20 636f 6e74 656e 745f  , data, content_
-00001510: 7479 7065 290d 0a0d 0a20 2020 2020 2020  type)....       
-00001520: 2069 6620 616c 6c28 5b6d 6574 686f 6420   if all([method 
-00001530: 3d3d 2022 504f 5354 222c 2064 6174 6120  == "POST", data 
-00001540: 6973 204e 6f6e 655d 293a 0d0a 2020 2020  is None]):..    
-00001550: 2020 2020 2020 2020 6865 6164 6572 735b          headers[
-00001560: 2243 4f4e 5445 4e54 2d54 5950 4522 5d20  "CONTENT-TYPE"] 
-00001570: 3d20 2261 7070 6c69 6361 7469 6f6e 2f6f  = "application/o
-00001580: 6374 6574 2d73 7472 6561 6d22 0d0a 0d0a  ctet-stream"....
-00001590: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
-000015a0: 2020 2020 2020 2020 2020 7374 6174 7573            status
-000015b0: 5f63 6f64 652c 2063 6f6e 7465 6e74 203d  _code, content =
-000015c0: 2061 7761 6974 2073 656c 662e 7365 6e64   await self.send
-000015d0: 5f72 6571 7565 7374 280d 0a20 2020 2020  _request(..     
-000015e0: 2020 2020 2020 2020 2020 206d 6574 686f             metho
-000015f0: 642c 2075 726c 2c20 6269 6e61 7279 5f64  d, url, binary_d
-00001600: 6174 612c 2068 6561 6465 7273 2c20 636f  ata, headers, co
-00001610: 6e74 656e 745f 7479 7065 0d0a 2020 2020  ntent_type..    
-00001620: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-00001630: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00001640: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
-00001650: 2020 2020 2020 2070 7269 6e74 2865 290d         print(e).
-00001660: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
-00001670: 7072 696e 745f 7265 7370 6f6e 7365 286d  print_response(m
-00001680: 6574 686f 643d 6d65 7468 6f64 2c20 7572  ethod=method, ur
-00001690: 6c3d 7572 6c2c 2073 7461 7475 735f 636f  l=url, status_co
-000016a0: 6465 3d73 7461 7475 735f 636f 6465 290d  de=status_code).
-000016b0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-000016c0: 6e20 7365 6c66 2e68 616e 646c 655f 7265  n self.handle_re
-000016d0: 7370 6f6e 7365 2873 7461 7475 735f 636f  sponse(status_co
-000016e0: 6465 3d73 7461 7475 735f 636f 6465 2c20  de=status_code, 
-000016f0: 7265 7370 6f6e 7365 3d63 6f6e 7465 6e74  response=content
-00001700: 290d 0a0d 0a0d 0a20 2020 2061 7379 6e63  )......    async
-00001710: 2064 6566 2073 6572 7669 6365 5f68 616e   def service_han
-00001720: 646c 6572 280d 0a20 2020 2020 2020 2020  dler(..         
-00001730: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
-00001740: 2020 2020 2020 7572 6c3a 2073 7472 2c0d        url: str,.
-00001750: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00001760: 613a 2055 6e69 6f6e 5b64 6963 742c 2062  a: Union[dict, b
-00001770: 7974 6573 2c20 4e6f 6e65 5d20 3d20 4e6f  ytes, None] = No
-00001780: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-00001790: 2063 6f6e 7465 6e74 5f74 7970 653a 204f   content_type: O
-000017a0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-000017b0: 6f6e 650d 0a20 2020 2029 202d 3e20 5475  one..    ) -> Tu
-000017c0: 706c 655b 7374 722c 2064 6963 742c 2055  ple[str, dict, U
-000017d0: 6e69 6f6e 5b64 6963 742c 2062 7974 6573  nion[dict, bytes
-000017e0: 2c20 4e6f 6e65 5d5d 3a0d 0a20 2020 2020  , None]]:..     
-000017f0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00001800: 6073 6572 7669 6365 5f68 616e 646c 6572  `service_handler
-00001810: 6020 2d20 5369 676e 7320 7468 6520 7265  ` - Signs the re
-00001820: 7175 6573 7420 616e 6420 7265 7475 726e  quest and return
-00001830: 7320 7468 6520 7365 7276 6963 6520 7572  s the service ur
-00001840: 6c2c 2068 6561 6465 7273 2061 6e64 2064  l, headers and d
-00001850: 6174 610d 0a0d 0a20 2020 2020 2020 2060  ata....        `
-00001860: 2a2a 5061 7261 6d65 7465 7273 2a2a 6060  **Parameters**``
-00001870: 0d0a 2020 2020 2020 2020 2d20 6075 726c  ..        - `url
-00001880: 6020 2d20 5468 6520 7572 6c20 746f 2073  ` - The url to s
-00001890: 656e 6420 7468 6520 7265 7175 6573 7420  end the request 
-000018a0: 746f 2e0d 0a20 2020 2020 2020 202d 2060  to...        - `
-000018b0: 6461 7461 6020 2d20 5468 6520 6461 7461  data` - The data
-000018c0: 2074 6f20 7365 6e64 2077 6974 6820 7468   to send with th
-000018d0: 6520 7265 7175 6573 742e 0d0a 2020 2020  e request...    
-000018e0: 2020 2020 2d20 6063 6f6e 7465 6e74 5f74      - `content_t
-000018f0: 7970 6560 202d 2054 6865 2063 6f6e 7465  ype` - The conte
-00001900: 6e74 2074 7970 6520 6f66 2074 6865 2064  nt type of the d
-00001910: 6174 612e 0d0a 0d0a 2020 2020 2020 2020  ata.....        
-00001920: 602a 2a52 6574 7572 6e73 2a2a 6060 0d0a  `**Returns**``..
-00001930: 2020 2020 2020 2020 2d20 6054 7570 6c65          - `Tuple
-00001940: 5b73 7472 2c20 6469 6374 2c20 556e 696f  [str, dict, Unio
-00001950: 6e5b 6469 6374 2c20 6279 7465 732c 204e  n[dict, bytes, N
-00001960: 6f6e 655d 5d60 202d 2054 6865 2073 6572  one]]` - The ser
-00001970: 7669 6365 2075 726c 2c20 6865 6164 6572  vice url, header
-00001980: 7320 616e 6420 6461 7461 2e0d 0a0d 0a20  s and data..... 
-00001990: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
-000019a0: 2020 2020 2020 6865 6164 6572 7320 3d20        headers = 
-000019b0: 7b22 4e44 4344 4556 4943 4549 4422 3a20  {"NDCDEVICEID": 
-000019c0: 6465 7669 6365 5f69 6428 292c 202a 2a61  device_id(), **a
-000019d0: 7761 6974 2073 656c 662e 7365 7276 6963  wait self.servic
-000019e0: 655f 6865 6164 6572 7328 297d 0d0a 0d0a  e_headers()}....
-000019f0: 2020 2020 2020 2020 6966 2064 6174 6120          if data 
-00001a00: 6f72 2063 6f6e 7465 6e74 5f74 7970 653a  or content_type:
-00001a10: 0d0a 2020 2020 2020 2020 2020 2020 6865  ..            he
-00001a20: 6164 6572 732c 2064 6174 6120 3d20 6177  aders, data = aw
-00001a30: 6169 7420 7365 6c66 2e66 6574 6368 5f73  ait self.fetch_s
-00001a40: 6967 6e61 7475 7265 2864 6174 612c 2068  ignature(data, h
-00001a50: 6561 6465 7273 2c20 636f 6e74 656e 745f  eaders, content_
-00001a60: 7479 7065 290d 0a0d 0a20 2020 2020 2020  type)....       
-00001a70: 2072 6574 7572 6e20 7572 6c2c 2068 6561   return url, hea
-00001a80: 6465 7273 2c20 7365 6c66 2e65 6e73 7572  ders, self.ensur
-00001a90: 655f 7574 6638 2864 6174 6129 0d0a 0d0a  e_utf8(data)....
-00001aa0: 0d0a 2020 2020 6465 6620 656e 7375 7265  ..    def ensure
-00001ab0: 5f75 7466 3828 7365 6c66 2c20 6461 7461  _utf8(self, data
-00001ac0: 3a20 556e 696f 6e5b 6469 6374 2c20 6279  : Union[dict, by
-00001ad0: 7465 732c 204e 6f6e 655d 2920 2d3e 2055  tes, None]) -> U
-00001ae0: 6e69 6f6e 5b64 6963 742c 2062 7974 6573  nion[dict, bytes
-00001af0: 2c20 4e6f 6e65 5d3a 0d0a 2020 2020 2020  , None]:..      
-00001b00: 2020 2222 220d 0a20 2020 2020 2020 2060    """..        `
-00001b10: 656e 7375 7265 5f75 7466 3860 202d 2045  ensure_utf8` - E
-00001b20: 6e73 7572 6573 2074 6865 2064 6174 6120  nsures the data 
-00001b30: 6973 2075 7466 2d38 2065 6e63 6f64 6564  is utf-8 encoded
-00001b40: 0d0a 0d0a 2020 2020 2020 2020 602a 2a50  ....        `**P
-00001b50: 6172 616d 6574 6572 732a 2a60 600d 0a20  arameters**``.. 
-00001b60: 2020 2020 2020 202d 2060 6461 7461 6020         - `data` 
-00001b70: 2d20 5468 6520 6461 7461 2074 6f20 656e  - The data to en
-00001b80: 636f 6465 2e0d 0a0d 0a20 2020 2020 2020  code.....       
-00001b90: 2060 2a2a 5265 7475 726e 732a 2a60 600d   `**Returns**``.
-00001ba0: 0a20 2020 2020 2020 202d 2060 556e 696f  .        - `Unio
-00001bb0: 6e5b 6469 6374 2c20 6279 7465 732c 204e  n[dict, bytes, N
-00001bc0: 6f6e 655d 6020 2d20 5468 6520 656e 636f  one]` - The enco
-00001bd0: 6465 6420 6461 7461 2e0d 0a0d 0a20 2020  ded data.....   
-00001be0: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
-00001bf0: 2020 2020 6966 2064 6174 6120 6973 204e      if data is N
-00001c00: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00001c10: 2020 7265 7475 726e 2064 6174 610d 0a0d    return data...
-00001c20: 0a20 2020 2020 2020 2064 6566 2068 616e  .        def han
-00001c30: 646c 655f 6469 6374 2864 6174 613a 2064  dle_dict(data: d
-00001c40: 6963 7429 3a0d 0a20 2020 2020 2020 2020  ict):..         
-00001c50: 2020 2072 6574 7572 6e20 7b6b 6579 3a20     return {key: 
-00001c60: 7365 6c66 2e65 6e73 7572 655f 7574 6638  self.ensure_utf8
-00001c70: 2876 616c 7565 2920 666f 7220 6b65 792c  (value) for key,
-00001c80: 2076 616c 7565 2069 6e20 6461 7461 2e69   value in data.i
-00001c90: 7465 6d73 2829 7d0d 0a0d 0a20 2020 2020  tems()}....     
-00001ca0: 2020 2064 6566 2068 616e 646c 655f 7374     def handle_st
-00001cb0: 7228 6461 7461 3a20 7374 7229 3a0d 0a20  r(data: str):.. 
-00001cc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001cd0: 6e20 6461 7461 2e65 6e63 6f64 6528 2275  n data.encode("u
-00001ce0: 7466 2d38 2229 0d0a 0d0a 2020 2020 2020  tf-8")....      
-00001cf0: 2020 6861 6e64 6c65 7273 203d 207b 0d0a    handlers = {..
-00001d00: 2020 2020 2020 2020 2020 2020 6469 6374              dict
-00001d10: 3a20 6861 6e64 6c65 5f64 6963 742c 0d0a  : handle_dict,..
-00001d20: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00001d30: 2068 616e 646c 655f 7374 720d 0a20 2020   handle_str..   
-00001d40: 2020 2020 207d 0d0a 0d0a 2020 2020 2020       }....      
-00001d50: 2020 7265 7475 726e 2068 616e 646c 6572    return handler
-00001d60: 732e 6765 7428 7479 7065 2864 6174 6129  s.get(type(data)
-00001d70: 2c20 6c61 6d62 6461 2078 3a20 7829 2864  , lambda x: x)(d
-00001d80: 6174 6129 0d0a 0d0a 0d0a 2020 2020 6173  ata)......    as
-00001d90: 796e 6320 6465 6620 6665 7463 685f 7369  ync def fetch_si
-00001da0: 676e 6174 7572 6528 0d0a 2020 2020 2020  gnature(..      
-00001db0: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
-00001dc0: 2020 2020 2020 2020 2064 6174 613a 2055           data: U
-00001dd0: 6e69 6f6e 5b64 6963 742c 2062 7974 6573  nion[dict, bytes
-00001de0: 2c20 4e6f 6e65 5d2c 0d0a 2020 2020 2020  , None],..      
-00001df0: 2020 2020 2020 6865 6164 6572 733a 2064        headers: d
-00001e00: 6963 742c 0d0a 2020 2020 2020 2020 2020  ict,..          
-00001e10: 2020 636f 6e74 656e 745f 7479 7065 3a20    content_type: 
-00001e20: 7374 7220 3d20 4e6f 6e65 0d0a 2020 2020  str = None..    
-00001e30: 2920 2d3e 2054 7570 6c65 5b64 6963 742c  ) -> Tuple[dict,
-00001e40: 2055 6e69 6f6e 5b64 6963 742c 2062 7974   Union[dict, byt
-00001e50: 6573 2c20 4e6f 6e65 5d5d 3a0d 0a20 2020  es, None]]:..   
-00001e60: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00001e70: 2020 6066 6574 6368 5f73 6967 6e61 7475    `fetch_signatu
-00001e80: 7265 6020 2d20 4665 7463 6865 7320 7468  re` - Fetches th
-00001e90: 6520 7369 676e 6174 7572 6520 616e 6420  e signature and 
-00001ea0: 7265 7475 726e 7320 7468 6520 6461 7461  returns the data
-00001eb0: 2061 6e64 2075 7064 6174 6564 2068 6561   and updated hea
-00001ec0: 6465 7273 0d0a 0d0a 2020 2020 2020 2020  ders....        
-00001ed0: 602a 2a50 6172 616d 6574 6572 732a 2a60  `**Parameters**`
-00001ee0: 600d 0a20 2020 2020 2020 202d 2060 6461  `..        - `da
-00001ef0: 7461 6020 2d20 5468 6520 6461 7461 2074  ta` - The data t
-00001f00: 6f20 7365 6e64 2077 6974 6820 7468 6520  o send with the 
-00001f10: 7265 7175 6573 742e 0d0a 2020 2020 2020  request...      
-00001f20: 2020 2d20 6068 6561 6465 7273 6020 2d20    - `headers` - 
-00001f30: 5468 6520 6865 6164 6572 7320 746f 2073  The headers to s
-00001f40: 656e 6420 7769 7468 2074 6865 2072 6571  end with the req
-00001f50: 7565 7374 2e0d 0a20 2020 2020 2020 202d  uest...        -
-00001f60: 2060 636f 6e74 656e 745f 7479 7065 6020   `content_type` 
-00001f70: 2d20 5468 6520 636f 6e74 656e 7420 7479  - The content ty
-00001f80: 7065 206f 6620 7468 6520 6461 7461 2e0d  pe of the data..
-00001f90: 0a0d 0a20 2020 2020 2020 2060 2a2a 5265  ...        `**Re
-00001fa0: 7475 726e 732a 2a60 600d 0a20 2020 2020  turns**``..     
-00001fb0: 2020 202d 2060 5475 706c 655b 6469 6374     - `Tuple[dict
-00001fc0: 2c20 556e 696f 6e5b 6469 6374 2c20 6279  , Union[dict, by
-00001fd0: 7465 732c 204e 6f6e 655d 5d60 202d 2054  tes, None]]` - T
-00001fe0: 6865 2068 6561 6465 7273 2061 6e64 2064  he headers and d
-00001ff0: 6174 612e 0d0a 0d0a 2020 2020 2020 2020  ata.....        
-00002000: 2222 220d 0a0d 0a20 2020 2020 2020 2069  """....        i
-00002010: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00002020: 2864 6174 612c 2062 7974 6573 293a 0d0a  (data, bytes):..
-00002030: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00002040: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
-00002050: 2020 2020 2020 6f72 6a73 6f6e 5f64 756d        orjson_dum
-00002060: 7073 2864 6174 6129 2e64 6563 6f64 6528  ps(data).decode(
-00002070: 2275 7466 2d38 2229 0d0a 2020 2020 2020  "utf-8")..      
-00002080: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00002090: 662e 6f72 6a73 6f6e 0d0a 2020 2020 2020  f.orjson..      
-000020a0: 2020 2020 2020 2020 2020 656c 7365 2064            else d
-000020b0: 756d 7073 2864 6174 6129 0d0a 2020 2020  umps(data)..    
-000020c0: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-000020d0: 2020 2020 2068 6561 6465 7273 2e75 7064       headers.upd
-000020e0: 6174 6528 0d0a 2020 2020 2020 2020 2020  ate(..          
-000020f0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00002100: 2020 2020 2022 434f 4e54 454e 542d 4c45       "CONTENT-LE
-00002110: 4e47 5448 223a 2066 227b 6c65 6e28 6461  NGTH": f"{len(da
-00002120: 7461 297d 222c 0d0a 2020 2020 2020 2020  ta)}",..        
-00002130: 2020 2020 2020 2020 2243 4f4e 5445 4e54          "CONTENT
-00002140: 2d54 5950 4522 3a20 636f 6e74 656e 745f  -TYPE": content_
-00002150: 7479 7065 206f 7220 2261 7070 6c69 6361  type or "applica
-00002160: 7469 6f6e 2f6a 736f 6e3b 2063 6861 7273  tion/json; chars
-00002170: 6574 3d75 7466 2d38 222c 0d0a 2020 2020  et=utf-8",..    
-00002180: 2020 2020 2020 2020 2020 2020 224e 4443              "NDC
-00002190: 2d4d 5347 2d53 4947 223a 2067 656e 6572  -MSG-SIG": gener
-000021a0: 6174 655f 7369 676e 6174 7572 6528 6461  ate_signature(da
-000021b0: 7461 292c 0d0a 2020 2020 2020 2020 2020  ta),..          
-000021c0: 2020 7d0d 0a20 2020 2020 2020 2029 0d0a    }..        )..
-000021d0: 2020 2020 2020 2020 7265 7475 726e 2068          return h
-000021e0: 6561 6465 7273 2c20 6461 7461 0d0a 0d0a  eaders, data....
-000021f0: 0d0a 2020 2020 6465 6620 7261 6973 655f  ..    def raise_
-00002200: 6572 726f 7228 7365 6c66 2c20 7265 7370  error(self, resp
-00002210: 6f6e 7365 3a20 6469 6374 2920 2d3e 204e  onse: dict) -> N
-00002220: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
-00002230: 220d 0a20 2020 2020 2020 2060 7261 6973  "..        `rais
-00002240: 655f 6572 726f 7260 202d 2052 6169 7365  e_error` - Raise
-00002250: 7320 616e 2065 7272 6f72 2069 6620 616e  s an error if an
-00002260: 2065 7272 6f72 2069 7320 696e 2074 6865   error is in the
-00002270: 2072 6573 706f 6e73 650d 0a0d 0a20 2020   response....   
-00002280: 2020 2020 2060 2a2a 5061 7261 6d65 7465       `**Paramete
-00002290: 7273 2a2a 6060 0d0a 2020 2020 2020 2020  rs**``..        
-000022a0: 2d20 6072 6573 706f 6e73 6560 202d 2054  - `response` - T
-000022b0: 6865 2072 6573 706f 6e73 6520 6672 6f6d  he response from
-000022c0: 2074 6865 2072 6571 7565 7374 2e0d 0a0d   the request....
-000022d0: 0a20 2020 2020 2020 2060 2a2a 5265 7475  .        `**Retu
-000022e0: 726e 732a 2a60 600d 0a20 2020 2020 2020  rns**``..       
-000022f0: 202d 2060 4e6f 6e65 6020 2d20 5261 6973   - `None` - Rais
-00002300: 6573 2061 6e20 6572 726f 7220 6966 2074  es an error if t
-00002310: 6865 2073 7461 7475 7320 636f 6465 2069  he status code i
-00002320: 7320 696e 2074 6865 2072 6573 706f 6e73  s in the respons
-00002330: 6520 6d61 702e 0d0a 0d0a 2020 2020 2020  e map.....      
-00002340: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
-00002350: 6620 616c 6c28 0d0a 2020 2020 2020 2020  f all(..        
-00002360: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
-00002370: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002380: 6573 706f 6e73 652e 6765 7428 2261 7069  esponse.get("api
-00002390: 3a73 7461 7475 7363 6f64 6522 2c20 3230  :statuscode", 20
-000023a0: 3029 203d 3d20 3130 352c 0d0a 2020 2020  0) == 105,..    
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 6861 7361 7474 7228 7365 6c66 2c20 2265  hasattr(self, "e
-000023d0: 6d61 696c 2229 2c0d 0a20 2020 2020 2020  mail"),..       
-000023e0: 2020 2020 2020 2020 2020 2020 2068 6173               has
-000023f0: 6174 7472 2873 656c 662c 2022 7061 7373  attr(self, "pass
-00002400: 776f 7264 2229 2c0d 0a20 2020 2020 2020  word"),..       
-00002410: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
-00002420: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
-00002430: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00002440: 626f 742e 7275 6e28 7365 6c66 2e65 6d61  bot.run(self.ema
-00002450: 696c 2c20 7365 6c66 2e70 6173 7377 6f72  il, self.passwor
-00002460: 642c 2075 7365 5f63 6163 6865 3d46 616c  d, use_cache=Fal
-00002470: 7365 290d 0a0d 0a20 2020 2020 2020 2065  se)....        e
-00002480: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00002490: 2020 7261 6973 6520 4150 4945 7863 6570    raise APIExcep
-000024a0: 7469 6f6e 2872 6573 706f 6e73 6529 0d0a  tion(response)..
-000024b0: 0d0a 0d0a 2020 2020 6465 6620 6861 6e64  ....    def hand
-000024c0: 6c65 5f72 6573 706f 6e73 6528 7365 6c66  le_response(self
-000024d0: 2c20 7374 6174 7573 5f63 6f64 653a 2069  , status_code: i
-000024e0: 6e74 2c20 7265 7370 6f6e 7365 3a20 7374  nt, response: st
-000024f0: 7229 202d 3e20 6469 6374 3a0d 0a20 2020  r) -> dict:..   
-00002500: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00002510: 2020 6068 616e 646c 655f 7265 7370 6f6e    `handle_respon
-00002520: 7365 6020 2d20 4861 6e64 6c65 7320 7468  se` - Handles th
-00002530: 6520 7265 7370 6f6e 7365 2061 6e64 2072  e response and r
-00002540: 6574 7572 6e73 2074 6865 2072 6573 706f  eturns the respo
-00002550: 6e73 6520 6173 2061 2064 6963 740d 0a0d  nse as a dict...
-00002560: 0a20 2020 2020 2020 2060 2a2a 5061 7261  .        `**Para
-00002570: 6d65 7465 7273 2a2a 6060 0d0a 2020 2020  meters**``..    
-00002580: 2020 2020 2d20 6073 7461 7475 735f 636f      - `status_co
-00002590: 6465 6020 2d20 5468 6520 7374 6174 7573  de` - The status
-000025a0: 2063 6f64 6520 6f66 2074 6865 2072 6573   code of the res
-000025b0: 706f 6e73 652e 0d0a 2020 2020 2020 2020  ponse...        
-000025c0: 2d20 6072 6573 706f 6e73 6560 202d 2054  - `response` - T
-000025d0: 6865 2072 6573 706f 6e73 6520 746f 2068  he response to h
-000025e0: 616e 646c 652e 0d0a 0d0a 2020 2020 2020  andle.....      
-000025f0: 2020 602a 2a52 6574 7572 6e73 2a2a 6060    `**Returns**``
-00002600: 0d0a 2020 2020 2020 2020 2d20 6064 6963  ..        - `dic
-00002610: 7460 202d 2054 6865 2072 6573 706f 6e73  t` - The respons
-00002620: 6520 6173 2061 2064 6963 742e 0d0a 0d0a  e as a dict.....
-00002630: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00002640: 2020 2020 2069 6620 7374 6174 7573 5f63       if status_c
-00002650: 6f64 6520 696e 2073 656c 662e 7265 7370  ode in self.resp
-00002660: 6f6e 7365 5f6d 6170 3a0d 0a20 2020 2020  onse_map:..     
-00002670: 2020 2020 2020 2072 6169 7365 2073 656c         raise sel
-00002680: 662e 7265 7370 6f6e 7365 5f6d 6170 5b73  f.response_map[s
-00002690: 7461 7475 735f 636f 6465 5d0d 0a0d 0a20  tatus_code].... 
-000026a0: 2020 2020 2020 2065 6c69 6620 7265 7370         elif resp
-000026b0: 6f6e 7365 2e73 7461 7274 7377 6974 6828  onse.startswith(
-000026c0: 226e 756c 6c22 293a 0d0a 2020 2020 2020  "null"):..      
-000026d0: 2020 2020 2020 7261 6973 6520 4e75 6c6c        raise Null
-000026e0: 5265 7370 6f6e 7365 0d0a 0d0a 2020 2020  Response....    
-000026f0: 2020 2020 656c 7365 3a0d 0a0d 0a20 2020      else:....   
-00002700: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
-00002710: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002720: 6573 706f 6e73 6520 3d20 280d 0a20 2020  esponse = (..   
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 206f 726a 736f 6e5f 6c6f 6164 7328 7265   orjson_loads(re
-00002750: 7370 6f6e 7365 290d 0a20 2020 2020 2020  sponse)..       
-00002760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00002770: 7365 6c66 2e6f 726a 736f 6e0d 0a20 2020  self.orjson..   
-00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002790: 2065 6c73 6520 6c6f 6164 7328 7265 7370   else loads(resp
-000027a0: 6f6e 7365 290d 0a20 2020 2020 2020 2020  onse)..         
-000027b0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000027c0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-000027d0: 6570 7469 6f6e 3a0d 0a20 2020 2020 2020  eption:..       
-000027e0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-000027f0: 6520 3d20 6c6f 6164 7328 7265 7370 6f6e  e = loads(respon
-00002800: 7365 290d 0a0d 0a20 2020 2020 2020 2020  se)....         
-00002810: 2020 2069 6620 7374 6174 7573 5f63 6f64     if status_cod
-00002820: 6520 213d 2032 3030 3a0d 0a20 2020 2020  e != 200:..     
-00002830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002840: 7261 6973 655f 6572 726f 7228 7265 7370  raise_error(resp
-00002850: 6f6e 7365 290d 0a0d 0a20 2020 2020 2020  onse)....       
-00002860: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
-00002870: 6f6e 7365 0d0a 0d0a 0d0a 2020 2020 6465  onse......    de
-00002880: 6620 7072 696e 745f 7265 7370 6f6e 7365  f print_response
-00002890: 2873 656c 662c 206d 6574 686f 643a 2073  (self, method: s
-000028a0: 7472 2c20 7572 6c3a 2073 7472 2c20 7374  tr, url: str, st
-000028b0: 6174 7573 5f63 6f64 653a 2069 6e74 293a  atus_code: int):
-000028c0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000028d0: 2020 2020 2020 2060 7072 696e 745f 7265         `print_re
-000028e0: 7370 6f6e 7365 6020 2d20 5072 696e 7473  sponse` - Prints
-000028f0: 2074 6865 2072 6573 706f 6e73 6520 6966   the response if
-00002900: 2064 6562 7567 2069 7320 656e 6162 6c65   debug is enable
-00002910: 640d 0a0d 0a20 2020 2020 2020 2060 2a2a  d....        `**
-00002920: 5061 7261 6d65 7465 7273 2a2a 6060 0d0a  Parameters**``..
-00002930: 2020 2020 2020 2020 2d20 606d 6574 686f          - `metho
-00002940: 6460 202d 2054 6865 2072 6571 7565 7374  d` - The request
-00002950: 206d 6574 686f 6420 7573 6564 2e0d 0a20   method used... 
-00002960: 2020 2020 2020 202d 2060 7572 6c60 202d         - `url` -
-00002970: 2054 6865 2075 726c 2074 6865 2072 6571   The url the req
-00002980: 7565 7374 2077 6173 2073 656e 7420 746f  uest was sent to
-00002990: 2e0d 0a20 2020 2020 2020 202d 2060 7374  ...        - `st
-000029a0: 6174 7573 5f63 6f64 6560 202d 2054 6865  atus_code` - The
-000029b0: 2073 7461 7475 7320 636f 6465 206f 6620   status code of 
-000029c0: 7468 6520 7265 7370 6f6e 7365 2e0d 0a20  the response... 
-000029d0: 2020 2020 2020 202d 2060 7265 7370 6f6e         - `respon
-000029e0: 7365 6020 2d20 5468 6520 7265 7370 6f6e  se` - The respon
-000029f0: 7365 2074 6f20 7072 696e 742e 0d0a 0d0a  se to print.....
-00002a00: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00002a10: 2020 2020 2069 6620 7365 6c66 2e62 6f74       if self.bot
-00002a20: 2e64 6562 7567 3a0d 0a20 2020 2020 2020  .debug:..       
-00002a30: 2020 2020 2063 6f6c 6f72 203d 2028 0d0a       color = (..
-00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a50: 466f 7265 2e52 4544 0d0a 2020 2020 2020  Fore.RED..      
-00002a60: 2020 2020 2020 2020 2020 6966 2073 7461            if sta
-00002a70: 7475 735f 636f 6465 2021 3d20 3230 300d  tus_code != 200.
-00002a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a90: 2065 6c73 6520 7b0d 0a20 2020 2020 2020   else {..       
-00002aa0: 2020 2020 2020 2020 2020 2020 2022 4745               "GE
-00002ab0: 5422 3a20 466f 7265 2e42 4c55 452c 0d0a  T": Fore.BLUE,..
+00001200: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001210: 6177 6169 7420 7365 6c66 2e68 616e 646c  await self.handl
+00001220: 6572 286d 6574 686f 642c 2075 726c 2c20  er(method, url, 
+00001230: 6461 7461 2c20 636f 6e74 656e 745f 7479  data, content_ty
+00001240: 7065 290d 0a0d 0a0d 0a20 2020 2061 7379  pe)......    asy
+00001250: 6e63 2064 6566 2068 616e 646c 6572 280d  nc def handler(.
+00001260: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001270: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
+00001280: 6d65 7468 6f64 3a20 7374 722c 0d0a 2020  method: str,..  
+00001290: 2020 2020 2020 2020 2020 7572 6c3a 2073            url: s
+000012a0: 7472 2c0d 0a20 2020 2020 2020 2020 2020  tr,..           
+000012b0: 2064 6174 613a 2055 6e69 6f6e 5b64 6963   data: Union[dic
+000012c0: 742c 2062 7974 6573 2c20 4e6f 6e65 5d20  t, bytes, None] 
+000012d0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
+000012e0: 2020 2020 2063 6f6e 7465 6e74 5f74 7970       content_typ
+000012f0: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
+00001300: 203d 204e 6f6e 650d 0a20 2020 2029 202d   = None..    ) -
+00001310: 3e20 6469 6374 3a0d 0a20 2020 2020 2020  > dict:..       
+00001320: 2022 2222 0d0a 2020 2020 2020 2020 6068   """..        `h
+00001330: 616e 646c 6572 6020 2d20 4861 6e64 6c65  andler` - Handle
+00001340: 7320 616c 6c20 7265 7175 6573 7473 0d0a  s all requests..
+00001350: 0d0a 2020 2020 2020 2020 602a 2a50 6172  ..        `**Par
+00001360: 616d 6574 6572 732a 2a60 600d 0a20 2020  ameters**``..   
+00001370: 2020 2020 202d 2060 6d65 7468 6f64 6020       - `method` 
+00001380: 2d20 5468 6520 7265 7175 6573 7420 6d65  - The request me
+00001390: 7468 6f64 2074 6f20 7573 652e 0d0a 2020  thod to use...  
+000013a0: 2020 2020 2020 2d20 6075 726c 6020 2d20        - `url` - 
+000013b0: 5468 6520 7572 6c20 746f 2073 656e 6420  The url to send 
+000013c0: 7468 6520 7265 7175 6573 7420 746f 2e0d  the request to..
+000013d0: 0a20 2020 2020 2020 202d 2060 6461 7461  .        - `data
+000013e0: 6020 2d20 5468 6520 6461 7461 2074 6f20  ` - The data to 
+000013f0: 7365 6e64 2077 6974 6820 7468 6520 7265  send with the re
+00001400: 7175 6573 742e 0d0a 2020 2020 2020 2020  quest...        
+00001410: 2d20 6063 6f6e 7465 6e74 5f74 7970 6560  - `content_type`
+00001420: 202d 2054 6865 2063 6f6e 7465 6e74 2074   - The content t
+00001430: 7970 6520 6f66 2074 6865 2064 6174 612e  ype of the data.
+00001440: 0d0a 0d0a 2020 2020 2020 2020 602a 2a52  ....        `**R
+00001450: 6574 7572 6e73 2a2a 6060 0d0a 2020 2020  eturns**``..    
+00001460: 2020 2020 2d20 6064 6963 7460 202d 2054      - `dict` - T
+00001470: 6865 2072 6573 706f 6e73 6520 6672 6f6d  he response from
+00001480: 2074 6865 2072 6571 7565 7374 2e0d 0a0d   the request....
+00001490: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000014a0: 2020 2020 2020 7572 6c20 3d20 7365 6c66        url = self
+000014b0: 2e73 6572 7669 6365 5f75 726c 2875 726c  .service_url(url
+000014c0: 290d 0a0d 0a20 2020 2020 2020 2075 726c  )....        url
+000014d0: 2c20 6865 6164 6572 732c 2062 696e 6172  , headers, binar
+000014e0: 795f 6461 7461 203d 2061 7761 6974 2073  y_data = await s
+000014f0: 656c 662e 7365 7276 6963 655f 6861 6e64  elf.service_hand
+00001500: 6c65 7228 7572 6c2c 2064 6174 612c 2063  ler(url, data, c
+00001510: 6f6e 7465 6e74 5f74 7970 6529 0d0a 0d0a  ontent_type)....
+00001520: 2020 2020 2020 2020 6966 2061 6c6c 285b          if all([
+00001530: 6d65 7468 6f64 203d 3d20 2250 4f53 5422  method == "POST"
+00001540: 2c20 6461 7461 2069 7320 4e6f 6e65 5d29  , data is None])
+00001550: 3a0d 0a20 2020 2020 2020 2020 2020 2068  :..            h
+00001560: 6561 6465 7273 5b22 434f 4e54 454e 542d  eaders["CONTENT-
+00001570: 5459 5045 225d 203d 2022 6170 706c 6963  TYPE"] = "applic
+00001580: 6174 696f 6e2f 6f63 7465 742d 7374 7265  ation/octet-stre
+00001590: 616d 220d 0a0d 0a20 2020 2020 2020 2074  am"....        t
+000015a0: 7279 3a0d 0a20 2020 2020 2020 2020 2020  ry:..           
+000015b0: 2073 7461 7475 735f 636f 6465 2c20 636f   status_code, co
+000015c0: 6e74 656e 7420 3d20 6177 6169 7420 7365  ntent = await se
+000015d0: 6c66 2e73 656e 645f 7265 7175 6573 7428  lf.send_request(
+000015e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000015f0: 2020 6d65 7468 6f64 2c20 7572 6c2c 2062    method, url, b
+00001600: 696e 6172 795f 6461 7461 2c20 6865 6164  inary_data, head
+00001610: 6572 732c 2063 6f6e 7465 6e74 5f74 7970  ers, content_typ
+00001620: 650d 0a20 2020 2020 2020 2020 2020 2029  e..            )
+00001630: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+00001640: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00001650: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00001660: 696e 7428 6529 0d0a 0d0a 2020 2020 2020  int(e)....      
+00001670: 2020 7365 6c66 2e70 7269 6e74 5f72 6573    self.print_res
+00001680: 706f 6e73 6528 6d65 7468 6f64 3d6d 6574  ponse(method=met
+00001690: 686f 642c 2075 726c 3d75 726c 2c20 7374  hod, url=url, st
+000016a0: 6174 7573 5f63 6f64 653d 7374 6174 7573  atus_code=status
+000016b0: 5f63 6f64 6529 0d0a 0d0a 2020 2020 2020  _code)....      
+000016c0: 2020 7265 7475 726e 2061 7761 6974 2073    return await s
+000016d0: 656c 662e 6861 6e64 6c65 5f72 6573 706f  elf.handle_respo
+000016e0: 6e73 6528 7374 6174 7573 5f63 6f64 653d  nse(status_code=
+000016f0: 7374 6174 7573 5f63 6f64 652c 2072 6573  status_code, res
+00001700: 706f 6e73 653d 636f 6e74 656e 7429 0d0a  ponse=content)..
+00001710: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
+00001720: 6620 7365 7276 6963 655f 6861 6e64 6c65  f service_handle
+00001730: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
+00001740: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
+00001750: 2020 2075 726c 3a20 7374 722c 0d0a 2020     url: str,..  
+00001760: 2020 2020 2020 2020 2020 6461 7461 3a20            data: 
+00001770: 556e 696f 6e5b 6469 6374 2c20 6279 7465  Union[dict, byte
+00001780: 732c 204e 6f6e 655d 203d 204e 6f6e 652c  s, None] = None,
+00001790: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+000017a0: 6e74 656e 745f 7479 7065 3a20 4f70 7469  ntent_type: Opti
+000017b0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+000017c0: 0d0a 2020 2020 2920 2d3e 2054 7570 6c65  ..    ) -> Tuple
+000017d0: 5b73 7472 2c20 6469 6374 2c20 556e 696f  [str, dict, Unio
+000017e0: 6e5b 6469 6374 2c20 6279 7465 732c 204e  n[dict, bytes, N
+000017f0: 6f6e 655d 5d3a 0d0a 2020 2020 2020 2020  one]]:..        
+00001800: 2222 220d 0a20 2020 2020 2020 2060 7365  """..        `se
+00001810: 7276 6963 655f 6861 6e64 6c65 7260 202d  rvice_handler` -
+00001820: 2053 6967 6e73 2074 6865 2072 6571 7565   Signs the reque
+00001830: 7374 2061 6e64 2072 6574 7572 6e73 2074  st and returns t
+00001840: 6865 2073 6572 7669 6365 2075 726c 2c20  he service url, 
+00001850: 6865 6164 6572 7320 616e 6420 6461 7461  headers and data
+00001860: 0d0a 0d0a 2020 2020 2020 2020 602a 2a50  ....        `**P
+00001870: 6172 616d 6574 6572 732a 2a60 600d 0a20  arameters**``.. 
+00001880: 2020 2020 2020 202d 2060 7572 6c60 202d         - `url` -
+00001890: 2054 6865 2075 726c 2074 6f20 7365 6e64   The url to send
+000018a0: 2074 6865 2072 6571 7565 7374 2074 6f2e   the request to.
+000018b0: 0d0a 2020 2020 2020 2020 2d20 6064 6174  ..        - `dat
+000018c0: 6160 202d 2054 6865 2064 6174 6120 746f  a` - The data to
+000018d0: 2073 656e 6420 7769 7468 2074 6865 2072   send with the r
+000018e0: 6571 7565 7374 2e0d 0a20 2020 2020 2020  equest...       
+000018f0: 202d 2060 636f 6e74 656e 745f 7479 7065   - `content_type
+00001900: 6020 2d20 5468 6520 636f 6e74 656e 7420  ` - The content 
+00001910: 7479 7065 206f 6620 7468 6520 6461 7461  type of the data
+00001920: 2e0d 0a0d 0a20 2020 2020 2020 2060 2a2a  .....        `**
+00001930: 5265 7475 726e 732a 2a60 600d 0a20 2020  Returns**``..   
+00001940: 2020 2020 202d 2060 5475 706c 655b 7374       - `Tuple[st
+00001950: 722c 2064 6963 742c 2055 6e69 6f6e 5b64  r, dict, Union[d
+00001960: 6963 742c 2062 7974 6573 2c20 4e6f 6e65  ict, bytes, None
+00001970: 5d5d 6020 2d20 5468 6520 7365 7276 6963  ]]` - The servic
+00001980: 6520 7572 6c2c 2068 6561 6465 7273 2061  e url, headers a
+00001990: 6e64 2064 6174 612e 0d0a 0d0a 2020 2020  nd data.....    
+000019a0: 2020 2020 2222 220d 0a0d 0a20 2020 2020      """....     
+000019b0: 2020 2068 6561 6465 7273 203d 207b 224e     headers = {"N
+000019c0: 4443 4445 5649 4345 4944 223a 2064 6576  DCDEVICEID": dev
+000019d0: 6963 655f 6964 2829 2c20 2a2a 6177 6169  ice_id(), **awai
+000019e0: 7420 7365 6c66 2e73 6572 7669 6365 5f68  t self.service_h
+000019f0: 6561 6465 7273 2829 7d0d 0a0d 0a20 2020  eaders()}....   
+00001a00: 2020 2020 2069 6620 6461 7461 206f 7220       if data or 
+00001a10: 636f 6e74 656e 745f 7479 7065 3a0d 0a20  content_type:.. 
+00001a20: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+00001a30: 7273 2c20 6461 7461 203d 2061 7761 6974  rs, data = await
+00001a40: 2073 656c 662e 6665 7463 685f 7369 676e   self.fetch_sign
+00001a50: 6174 7572 6528 6461 7461 2c20 6865 6164  ature(data, head
+00001a60: 6572 732c 2063 6f6e 7465 6e74 5f74 7970  ers, content_typ
+00001a70: 6529 0d0a 0d0a 2020 2020 2020 2020 7265  e)....        re
+00001a80: 7475 726e 2075 726c 2c20 6865 6164 6572  turn url, header
+00001a90: 732c 2073 656c 662e 656e 7375 7265 5f75  s, self.ensure_u
+00001aa0: 7466 3828 6461 7461 290d 0a0d 0a0d 0a20  tf8(data)...... 
+00001ab0: 2020 2064 6566 2065 6e73 7572 655f 7574     def ensure_ut
+00001ac0: 6638 2873 656c 662c 2064 6174 613a 2055  f8(self, data: U
+00001ad0: 6e69 6f6e 5b64 6963 742c 2062 7974 6573  nion[dict, bytes
+00001ae0: 2c20 4e6f 6e65 5d29 202d 3e20 556e 696f  , None]) -> Unio
+00001af0: 6e5b 6469 6374 2c20 6279 7465 732c 204e  n[dict, bytes, N
+00001b00: 6f6e 655d 3a0d 0a20 2020 2020 2020 2022  one]:..        "
+00001b10: 2222 0d0a 2020 2020 2020 2020 6065 6e73  ""..        `ens
+00001b20: 7572 655f 7574 6638 6020 2d20 456e 7375  ure_utf8` - Ensu
+00001b30: 7265 7320 7468 6520 6461 7461 2069 7320  res the data is 
+00001b40: 7574 662d 3820 656e 636f 6465 640d 0a0d  utf-8 encoded...
+00001b50: 0a20 2020 2020 2020 2060 2a2a 5061 7261  .        `**Para
+00001b60: 6d65 7465 7273 2a2a 6060 0d0a 2020 2020  meters**``..    
+00001b70: 2020 2020 2d20 6064 6174 6160 202d 2054      - `data` - T
+00001b80: 6865 2064 6174 6120 746f 2065 6e63 6f64  he data to encod
+00001b90: 652e 0d0a 0d0a 2020 2020 2020 2020 602a  e.....        `*
+00001ba0: 2a52 6574 7572 6e73 2a2a 6060 0d0a 2020  *Returns**``..  
+00001bb0: 2020 2020 2020 2d20 6055 6e69 6f6e 5b64        - `Union[d
+00001bc0: 6963 742c 2062 7974 6573 2c20 4e6f 6e65  ict, bytes, None
+00001bd0: 5d60 202d 2054 6865 2065 6e63 6f64 6564  ]` - The encoded
+00001be0: 2064 6174 612e 0d0a 0d0a 2020 2020 2020   data.....      
+00001bf0: 2020 2222 220d 0a0d 0a20 2020 2020 2020    """....       
+00001c00: 2069 6620 6461 7461 2069 7320 4e6f 6e65   if data is None
+00001c10: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00001c20: 6574 7572 6e20 6461 7461 0d0a 0d0a 2020  eturn data....  
+00001c30: 2020 2020 2020 6465 6620 6861 6e64 6c65        def handle
+00001c40: 5f64 6963 7428 6461 7461 3a20 6469 6374  _dict(data: dict
+00001c50: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001c60: 7265 7475 726e 207b 6b65 793a 2073 656c  return {key: sel
+00001c70: 662e 656e 7375 7265 5f75 7466 3828 7661  f.ensure_utf8(va
+00001c80: 6c75 6529 2066 6f72 206b 6579 2c20 7661  lue) for key, va
+00001c90: 6c75 6520 696e 2064 6174 612e 6974 656d  lue in data.item
+00001ca0: 7328 297d 0d0a 0d0a 2020 2020 2020 2020  s()}....        
+00001cb0: 6465 6620 6861 6e64 6c65 5f73 7472 2864  def handle_str(d
+00001cc0: 6174 613a 2073 7472 293a 0d0a 2020 2020  ata: str):..    
+00001cd0: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+00001ce0: 6174 612e 656e 636f 6465 2822 7574 662d  ata.encode("utf-
+00001cf0: 3822 290d 0a0d 0a20 2020 2020 2020 2068  8")....        h
+00001d00: 616e 646c 6572 7320 3d20 7b0d 0a20 2020  andlers = {..   
+00001d10: 2020 2020 2020 2020 2064 6963 743a 2068           dict: h
+00001d20: 616e 646c 655f 6469 6374 2c0d 0a20 2020  andle_dict,..   
+00001d30: 2020 2020 2020 2020 2073 7472 3a20 6861           str: ha
+00001d40: 6e64 6c65 5f73 7472 0d0a 2020 2020 2020  ndle_str..      
+00001d50: 2020 7d0d 0a0d 0a20 2020 2020 2020 2072    }....        r
+00001d60: 6574 7572 6e20 6861 6e64 6c65 7273 2e67  eturn handlers.g
+00001d70: 6574 2874 7970 6528 6461 7461 292c 206c  et(type(data), l
+00001d80: 616d 6264 6120 783a 2078 2928 6461 7461  ambda x: x)(data
+00001d90: 290d 0a0d 0a0d 0a20 2020 2061 7379 6e63  )......    async
+00001da0: 2064 6566 2066 6574 6368 5f73 6967 6e61   def fetch_signa
+00001db0: 7475 7265 280d 0a20 2020 2020 2020 2020  ture(..         
+00001dc0: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
+00001dd0: 2020 2020 2020 6461 7461 3a20 556e 696f        data: Unio
+00001de0: 6e5b 6469 6374 2c20 6279 7465 732c 204e  n[dict, bytes, N
+00001df0: 6f6e 655d 2c0d 0a20 2020 2020 2020 2020  one],..         
+00001e00: 2020 2068 6561 6465 7273 3a20 6469 6374     headers: dict
+00001e10: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+00001e20: 6f6e 7465 6e74 5f74 7970 653a 2073 7472  ontent_type: str
+00001e30: 203d 204e 6f6e 650d 0a20 2020 2029 202d   = None..    ) -
+00001e40: 3e20 5475 706c 655b 6469 6374 2c20 556e  > Tuple[dict, Un
+00001e50: 696f 6e5b 6469 6374 2c20 6279 7465 732c  ion[dict, bytes,
+00001e60: 204e 6f6e 655d 5d3a 0d0a 2020 2020 2020   None]]:..      
+00001e70: 2020 2222 220d 0a20 2020 2020 2020 2060    """..        `
+00001e80: 6665 7463 685f 7369 676e 6174 7572 6560  fetch_signature`
+00001e90: 202d 2046 6574 6368 6573 2074 6865 2073   - Fetches the s
+00001ea0: 6967 6e61 7475 7265 2061 6e64 2072 6574  ignature and ret
+00001eb0: 7572 6e73 2074 6865 2064 6174 6120 616e  urns the data an
+00001ec0: 6420 7570 6461 7465 6420 6865 6164 6572  d updated header
+00001ed0: 730d 0a0d 0a20 2020 2020 2020 2060 2a2a  s....        `**
+00001ee0: 5061 7261 6d65 7465 7273 2a2a 6060 0d0a  Parameters**``..
+00001ef0: 2020 2020 2020 2020 2d20 6064 6174 6160          - `data`
+00001f00: 202d 2054 6865 2064 6174 6120 746f 2073   - The data to s
+00001f10: 656e 6420 7769 7468 2074 6865 2072 6571  end with the req
+00001f20: 7565 7374 2e0d 0a20 2020 2020 2020 202d  uest...        -
+00001f30: 2060 6865 6164 6572 7360 202d 2054 6865   `headers` - The
+00001f40: 2068 6561 6465 7273 2074 6f20 7365 6e64   headers to send
+00001f50: 2077 6974 6820 7468 6520 7265 7175 6573   with the reques
+00001f60: 742e 0d0a 2020 2020 2020 2020 2d20 6063  t...        - `c
+00001f70: 6f6e 7465 6e74 5f74 7970 6560 202d 2054  ontent_type` - T
+00001f80: 6865 2063 6f6e 7465 6e74 2074 7970 6520  he content type 
+00001f90: 6f66 2074 6865 2064 6174 612e 0d0a 0d0a  of the data.....
+00001fa0: 2020 2020 2020 2020 602a 2a52 6574 7572          `**Retur
+00001fb0: 6e73 2a2a 6060 0d0a 2020 2020 2020 2020  ns**``..        
+00001fc0: 2d20 6054 7570 6c65 5b64 6963 742c 2055  - `Tuple[dict, U
+00001fd0: 6e69 6f6e 5b64 6963 742c 2062 7974 6573  nion[dict, bytes
+00001fe0: 2c20 4e6f 6e65 5d5d 6020 2d20 5468 6520  , None]]` - The 
+00001ff0: 6865 6164 6572 7320 616e 6420 6461 7461  headers and data
+00002000: 2e0d 0a0d 0a20 2020 2020 2020 2022 2222  .....        """
+00002010: 0d0a 0d0a 2020 2020 2020 2020 6966 206e  ....        if n
+00002020: 6f74 2069 7369 6e73 7461 6e63 6528 6461  ot isinstance(da
+00002030: 7461 2c20 6279 7465 7329 3a0d 0a20 2020  ta, bytes):..   
+00002040: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+00002050: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
+00002060: 2020 206f 726a 736f 6e5f 6475 6d70 7328     orjson_dumps(
+00002070: 6461 7461 292e 6465 636f 6465 2822 7574  data).decode("ut
+00002080: 662d 3822 290d 0a20 2020 2020 2020 2020  f-8")..         
+00002090: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
+000020a0: 726a 736f 6e0d 0a20 2020 2020 2020 2020  rjson..         
+000020b0: 2020 2020 2020 2065 6c73 6520 6475 6d70         else dump
+000020c0: 7328 6461 7461 290d 0a20 2020 2020 2020  s(data)..       
+000020d0: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+000020e0: 2020 6865 6164 6572 732e 7570 6461 7465    headers.update
+000020f0: 280d 0a20 2020 2020 2020 2020 2020 207b  (..            {
+00002100: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002110: 2020 2243 4f4e 5445 4e54 2d4c 454e 4754    "CONTENT-LENGT
+00002120: 4822 3a20 6622 7b6c 656e 2864 6174 6129  H": f"{len(data)
+00002130: 7d22 2c0d 0a20 2020 2020 2020 2020 2020  }",..           
+00002140: 2020 2020 2022 434f 4e54 454e 542d 5459       "CONTENT-TY
+00002150: 5045 223a 2063 6f6e 7465 6e74 5f74 7970  PE": content_typ
+00002160: 6520 6f72 2022 6170 706c 6963 6174 696f  e or "applicatio
+00002170: 6e2f 6a73 6f6e 3b20 6368 6172 7365 743d  n/json; charset=
+00002180: 7574 662d 3822 2c0d 0a20 2020 2020 2020  utf-8",..       
+00002190: 2020 2020 2020 2020 2022 4e44 432d 4d53           "NDC-MS
+000021a0: 472d 5349 4722 3a20 6765 6e65 7261 7465  G-SIG": generate
+000021b0: 5f73 6967 6e61 7475 7265 2864 6174 6129  _signature(data)
+000021c0: 2c0d 0a20 2020 2020 2020 2020 2020 207d  ,..            }
+000021d0: 0d0a 2020 2020 2020 2020 290d 0a20 2020  ..        )..   
+000021e0: 2020 2020 2072 6574 7572 6e20 6865 6164       return head
+000021f0: 6572 732c 2064 6174 610d 0a0d 0a0d 0a20  ers, data...... 
+00002200: 2020 2061 7379 6e63 2064 6566 2072 6169     async def rai
+00002210: 7365 5f65 7272 6f72 2873 656c 662c 2072  se_error(self, r
+00002220: 6573 706f 6e73 653a 2064 6963 7429 202d  esponse: dict) -
+00002230: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
+00002240: 2022 2222 0d0a 2020 2020 2020 2020 6072   """..        `r
+00002250: 6169 7365 5f65 7272 6f72 6020 2d20 5261  aise_error` - Ra
+00002260: 6973 6573 2061 6e20 6572 726f 7220 6966  ises an error if
+00002270: 2061 6e20 6572 726f 7220 6973 2069 6e20   an error is in 
+00002280: 7468 6520 7265 7370 6f6e 7365 0d0a 0d0a  the response....
+00002290: 2020 2020 2020 2020 602a 2a50 6172 616d          `**Param
+000022a0: 6574 6572 732a 2a60 600d 0a20 2020 2020  eters**``..     
+000022b0: 2020 202d 2060 7265 7370 6f6e 7365 6020     - `response` 
+000022c0: 2d20 5468 6520 7265 7370 6f6e 7365 2066  - The response f
+000022d0: 726f 6d20 7468 6520 7265 7175 6573 742e  rom the request.
+000022e0: 0d0a 0d0a 2020 2020 2020 2020 602a 2a52  ....        `**R
+000022f0: 6574 7572 6e73 2a2a 6060 0d0a 2020 2020  eturns**``..    
+00002300: 2020 2020 2d20 604e 6f6e 6560 202d 2052      - `None` - R
+00002310: 6169 7365 7320 616e 2065 7272 6f72 2069  aises an error i
+00002320: 6620 7468 6520 7374 6174 7573 2063 6f64  f the status cod
+00002330: 6520 6973 2069 6e20 7468 6520 7265 7370  e is in the resp
+00002340: 6f6e 7365 206d 6170 2e0d 0a0d 0a20 2020  onse map.....   
+00002350: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00002360: 2020 6966 2061 6c6c 280d 0a20 2020 2020    if all(..     
+00002370: 2020 2020 2020 2020 2020 205b 0d0a 2020             [..  
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 2020 7265 7370 6f6e 7365 2e67 6574 2822    response.get("
+000023a0: 6170 693a 7374 6174 7573 636f 6465 222c  api:statuscode",
+000023b0: 2032 3030 2920 3d3d 2031 3035 2c0d 0a20   200) == 105,.. 
+000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023d0: 2020 2068 6173 6174 7472 2873 656c 662c     hasattr(self,
+000023e0: 2022 656d 6169 6c22 292c 0d0a 2020 2020   "email"),..    
+000023f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002400: 6861 7361 7474 7228 7365 6c66 2c20 2270  hasattr(self, "p
+00002410: 6173 7377 6f72 6422 292c 0d0a 2020 2020  assword"),..    
+00002420: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
+00002430: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
+00002440: 2020 2020 2020 2072 6574 7572 6e20 6177         return aw
+00002450: 6169 7420 7365 6c66 2e62 6f74 2e72 756e  ait self.bot.run
+00002460: 2873 656c 662e 656d 6169 6c2c 2073 656c  (self.email, sel
+00002470: 662e 7061 7373 776f 7264 2c20 7573 655f  f.password, use_
+00002480: 6361 6368 653d 4661 6c73 6529 0d0a 0d0a  cache=False)....
+00002490: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000024a0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000024b0: 2041 5049 4578 6365 7074 696f 6e28 7265   APIException(re
+000024c0: 7370 6f6e 7365 290d 0a0d 0a0d 0a20 2020  sponse)......   
+000024d0: 2061 7379 6e63 2064 6566 2068 616e 646c   async def handl
+000024e0: 655f 7265 7370 6f6e 7365 2873 656c 662c  e_response(self,
+000024f0: 2073 7461 7475 735f 636f 6465 3a20 696e   status_code: in
+00002500: 742c 2072 6573 706f 6e73 653a 2073 7472  t, response: str
+00002510: 2920 2d3e 2064 6963 743a 0d0a 2020 2020  ) -> dict:..    
+00002520: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00002530: 2060 6861 6e64 6c65 5f72 6573 706f 6e73   `handle_respons
+00002540: 6560 202d 2048 616e 646c 6573 2074 6865  e` - Handles the
+00002550: 2072 6573 706f 6e73 6520 616e 6420 7265   response and re
+00002560: 7475 726e 7320 7468 6520 7265 7370 6f6e  turns the respon
+00002570: 7365 2061 7320 6120 6469 6374 0d0a 0d0a  se as a dict....
+00002580: 2020 2020 2020 2020 602a 2a50 6172 616d          `**Param
+00002590: 6574 6572 732a 2a60 600d 0a20 2020 2020  eters**``..     
+000025a0: 2020 202d 2060 7374 6174 7573 5f63 6f64     - `status_cod
+000025b0: 6560 202d 2054 6865 2073 7461 7475 7320  e` - The status 
+000025c0: 636f 6465 206f 6620 7468 6520 7265 7370  code of the resp
+000025d0: 6f6e 7365 2e0d 0a20 2020 2020 2020 202d  onse...        -
+000025e0: 2060 7265 7370 6f6e 7365 6020 2d20 5468   `response` - Th
+000025f0: 6520 7265 7370 6f6e 7365 2074 6f20 6861  e response to ha
+00002600: 6e64 6c65 2e0d 0a0d 0a20 2020 2020 2020  ndle.....       
+00002610: 2060 2a2a 5265 7475 726e 732a 2a60 600d   `**Returns**``.
+00002620: 0a20 2020 2020 2020 202d 2060 6469 6374  .        - `dict
+00002630: 6020 2d20 5468 6520 7265 7370 6f6e 7365  ` - The response
+00002640: 2061 7320 6120 6469 6374 2e0d 0a0d 0a20   as a dict..... 
+00002650: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00002660: 2020 2020 6966 2073 7461 7475 735f 636f      if status_co
+00002670: 6465 2069 6e20 7365 6c66 2e72 6573 706f  de in self.respo
+00002680: 6e73 655f 6d61 703a 0d0a 2020 2020 2020  nse_map:..      
+00002690: 2020 2020 2020 7261 6973 6520 7365 6c66        raise self
+000026a0: 2e72 6573 706f 6e73 655f 6d61 705b 7374  .response_map[st
+000026b0: 6174 7573 5f63 6f64 655d 0d0a 0d0a 2020  atus_code]....  
+000026c0: 2020 2020 2020 656c 6966 2072 6573 706f        elif respo
+000026d0: 6e73 652e 7374 6172 7473 7769 7468 2822  nse.startswith("
+000026e0: 6e75 6c6c 2229 3a0d 0a20 2020 2020 2020  null"):..       
+000026f0: 2020 2020 2072 6169 7365 204e 756c 6c52       raise NullR
+00002700: 6573 706f 6e73 650d 0a0d 0a20 2020 2020  esponse....     
+00002710: 2020 2065 6c73 653a 0d0a 0d0a 2020 2020     else:....    
+00002720: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00002730: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00002740: 7370 6f6e 7365 203d 2028 0d0a 2020 2020  sponse = (..    
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 6f72 6a73 6f6e 5f6c 6f61 6473 2872 6573  orjson_loads(res
+00002770: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
+00002780: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00002790: 656c 662e 6f72 6a73 6f6e 0d0a 2020 2020  elf.orjson..    
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 656c 7365 206c 6f61 6473 2872 6573 706f  else loads(respo
+000027c0: 6e73 6529 0d0a 2020 2020 2020 2020 2020  nse)..          
+000027d0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+000027e0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+000027f0: 7074 696f 6e3a 0d0a 2020 2020 2020 2020  ption:..        
+00002800: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00002810: 203d 206c 6f61 6473 2872 6573 706f 6e73   = loads(respons
+00002820: 6529 0d0a 0d0a 2020 2020 2020 2020 2020  e)....          
+00002830: 2020 6966 2073 7461 7475 735f 636f 6465    if status_code
+00002840: 2021 3d20 3230 303a 0d0a 2020 2020 2020   != 200:..      
+00002850: 2020 2020 2020 2020 2020 6177 6169 7420            await 
+00002860: 7365 6c66 2e72 6169 7365 5f65 7272 6f72  self.raise_error
+00002870: 2872 6573 706f 6e73 6529 0d0a 0d0a 2020  (response)....  
+00002880: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002890: 2072 6573 706f 6e73 650d 0a0d 0a0d 0a20   response...... 
+000028a0: 2020 2064 6566 2070 7269 6e74 5f72 6573     def print_res
+000028b0: 706f 6e73 6528 7365 6c66 2c20 6d65 7468  ponse(self, meth
+000028c0: 6f64 3a20 7374 722c 2075 726c 3a20 7374  od: str, url: st
+000028d0: 722c 2073 7461 7475 735f 636f 6465 3a20  r, status_code: 
+000028e0: 696e 7429 3a0d 0a20 2020 2020 2020 2022  int):..        "
+000028f0: 2222 0d0a 2020 2020 2020 2020 6070 7269  ""..        `pri
+00002900: 6e74 5f72 6573 706f 6e73 6560 202d 2050  nt_response` - P
+00002910: 7269 6e74 7320 7468 6520 7265 7370 6f6e  rints the respon
+00002920: 7365 2069 6620 6465 6275 6720 6973 2065  se if debug is e
+00002930: 6e61 626c 6564 0d0a 0d0a 2020 2020 2020  nabled....      
+00002940: 2020 602a 2a50 6172 616d 6574 6572 732a    `**Parameters*
+00002950: 2a60 600d 0a20 2020 2020 2020 202d 2060  *``..        - `
+00002960: 6d65 7468 6f64 6020 2d20 5468 6520 7265  method` - The re
+00002970: 7175 6573 7420 6d65 7468 6f64 2075 7365  quest method use
+00002980: 642e 0d0a 2020 2020 2020 2020 2d20 6075  d...        - `u
+00002990: 726c 6020 2d20 5468 6520 7572 6c20 7468  rl` - The url th
+000029a0: 6520 7265 7175 6573 7420 7761 7320 7365  e request was se
+000029b0: 6e74 2074 6f2e 0d0a 2020 2020 2020 2020  nt to...        
+000029c0: 2d20 6073 7461 7475 735f 636f 6465 6020  - `status_code` 
+000029d0: 2d20 5468 6520 7374 6174 7573 2063 6f64  - The status cod
+000029e0: 6520 6f66 2074 6865 2072 6573 706f 6e73  e of the respons
+000029f0: 652e 0d0a 2020 2020 2020 2020 2d20 6072  e...        - `r
+00002a00: 6573 706f 6e73 6560 202d 2054 6865 2072  esponse` - The r
+00002a10: 6573 706f 6e73 6520 746f 2070 7269 6e74  esponse to print
+00002a20: 2e0d 0a0d 0a20 2020 2020 2020 2022 2222  .....        """
+00002a30: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00002a40: 662e 626f 742e 6465 6275 673a 0d0a 2020  f.bot.debug:..  
+00002a50: 2020 2020 2020 2020 2020 636f 6c6f 7220            color 
+00002a60: 3d20 280d 0a20 2020 2020 2020 2020 2020  = (..           
+00002a70: 2020 2020 2046 6f72 652e 5245 440d 0a20       Fore.RED.. 
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002a90: 6620 7374 6174 7573 5f63 6f64 6520 213d  f status_code !=
+00002aa0: 2032 3030 0d0a 2020 2020 2020 2020 2020   200..          
+00002ab0: 2020 2020 2020 656c 7365 207b 0d0a 2020        else {..  
 00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2020 2020 2250 4f53 5422 3a20 466f 7265      "POST": Fore
-00002ae0: 2e47 5245 454e 2c0d 0a20 2020 2020 2020  .GREEN,..       
-00002af0: 2020 2020 2020 2020 2020 2020 2022 4445               "DE
-00002b00: 4c45 5445 223a 2046 6f72 652e 4d41 4745  LETE": Fore.MAGE
-00002b10: 4e54 412c 0d0a 2020 2020 2020 2020 2020  NTA,..          
-00002b20: 2020 2020 2020 2020 2020 224c 4954 4522            "LITE"
-00002b30: 3a20 466f 7265 2e59 454c 4c4f 572c 0d0a  : Fore.YELLOW,..
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 7d2e 6765 7428 6d65 7468 6f64 2c20 466f  }.get(method, Fo
-00002b60: 7265 2e52 4544 290d 0a20 2020 2020 2020  re.RED)..       
-00002b70: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-00002b80: 2020 2020 7072 696e 7428 6622 7b63 6f6c      print(f"{col
-00002b90: 6f72 7d7b 5374 796c 652e 4252 4947 4854  or}{Style.BRIGHT
-00002ba0: 7d7b 6d65 7468 6f64 7d7b 5374 796c 652e  }{method}{Style.
-00002bb0: 5245 5345 545f 414c 4c7d 202d 207b 7572  RESET_ALL} - {ur
-00002bc0: 6c7d 2229 0d0a 0d0a 0d0a 2020 2020 6173  l}")......    as
-00002bd0: 796e 6320 6465 6620 636c 6f73 6528 7365  ync def close(se
-00002be0: 6c66 2920 2d3e 204e 6f6e 653a 0d0a 2020  lf) -> None:..  
-00002bf0: 2020 2020 2020 2222 2243 6c6f 7365 7320        """Closes 
-00002c00: 7468 6520 4854 5450 2073 6573 7369 6f6e  the HTTP session
-00002c10: 2e22 2222 0d0a 2020 2020 2020 2020 6177  ."""..        aw
-00002c20: 6169 7420 7365 6c66 2e73 6573 7369 6f6e  ait self.session
-00002c30: 2e63 6c6f 7365 2829                      .close()
+00002ad0: 2020 2247 4554 223a 2046 6f72 652e 424c    "GET": Fore.BL
+00002ae0: 5545 2c0d 0a20 2020 2020 2020 2020 2020  UE,..           
+00002af0: 2020 2020 2020 2020 2022 504f 5354 223a           "POST":
+00002b00: 2046 6f72 652e 4752 4545 4e2c 0d0a 2020   Fore.GREEN,..  
+00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b20: 2020 2244 454c 4554 4522 3a20 466f 7265    "DELETE": Fore
+00002b30: 2e4d 4147 454e 5441 2c0d 0a20 2020 2020  .MAGENTA,..     
+00002b40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002b50: 4c49 5445 223a 2046 6f72 652e 5945 4c4c  LITE": Fore.YELL
+00002b60: 4f57 2c0d 0a20 2020 2020 2020 2020 2020  OW,..           
+00002b70: 2020 2020 207d 2e67 6574 286d 6574 686f       }.get(metho
+00002b80: 642c 2046 6f72 652e 5245 4429 0d0a 2020  d, Fore.RED)..  
+00002b90: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
+00002ba0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+00002bb0: 227b 636f 6c6f 727d 7b53 7479 6c65 2e42  "{color}{Style.B
+00002bc0: 5249 4748 547d 7b6d 6574 686f 647d 7b53  RIGHT}{method}{S
+00002bd0: 7479 6c65 2e52 4553 4554 5f41 4c4c 7d20  tyle.RESET_ALL} 
+00002be0: 2d20 7b75 726c 7d22 290d 0a0d 0a0d 0a20  - {url}")...... 
+00002bf0: 2020 2061 7379 6e63 2064 6566 2063 6c6f     async def clo
+00002c00: 7365 2873 656c 6629 202d 3e20 4e6f 6e65  se(self) -> None
+00002c10: 3a0d 0a20 2020 2020 2020 2022 2222 436c  :..        """Cl
+00002c20: 6f73 6573 2074 6865 2048 5454 5020 7365  oses the HTTP se
+00002c30: 7373 696f 6e2e 2222 220d 0a20 2020 2020  ssion."""..     
+00002c40: 2020 2061 7761 6974 2073 656c 662e 7365     await self.se
+00002c50: 7373 696f 6e2e 636c 6f73 6528 29         ssion.close()
```

### Comparing `pymino-1.2.2.4/pymino/ext/utilities/chat_console.py` & `pymino-1.2.2.5/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/utilities/commands.py` & `pymino-1.2.2.5/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/utilities/community_console.py` & `pymino-1.2.2.5/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/utilities/generate.py` & `pymino-1.2.2.5/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/utilities/menu.py` & `pymino-1.2.2.5/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/utilities/profile_console.py` & `pymino-1.2.2.5/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino/ext/utilities/request_handler.py` & `pymino-1.2.2.5/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/pymino.egg-info/PKG-INFO` & `pymino-1.2.2.5/pymino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.2.4
+Version: 1.2.2.5
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.2.4 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.2.5 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.2.2.4/pymino.egg-info/SOURCES.txt` & `pymino-1.2.2.5/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.2.2.4/setup.cfg` & `pymino-1.2.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e32 2e34 0d0a 6175  on = 1.2.2.4..au
+00000020: 6f6e 203d 2031 2e32 2e32 2e35 0d0a 6175  on = 1.2.2.5..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.2.4/setup.py` & `pymino-1.2.2.5/setup.py`

 * *Files identical despite different names*

