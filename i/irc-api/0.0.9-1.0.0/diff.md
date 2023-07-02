# Comparing `tmp/irc_api-0.0.9.tar.gz` & `tmp/irc_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irc_api-0.0.9.tar", last modified: Sat Jul  1 20:19:09 2023, max compression
+gzip compressed data, was "irc_api-1.0.0.tar", last modified: Sun Jul  2 13:21:58 2023, max compression
```

## Comparing `irc_api-0.0.9.tar` & `irc_api-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:19:09.750967 irc_api-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 20:18:56.000000 irc_api-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:19:09.746967 irc_api-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-01 20:18:56.000000 irc_api-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-01 20:18:56.000000 irc_api-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:19:09.750967 irc_api-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:19:09.742967 irc_api-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:19:09.746967 irc_api-0.0.9/src/irc_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/irc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-01 20:18:56.000000 irc_api-0.0.9/src/irc_api/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:19:09.746967 irc_api-0.0.9/src/irc_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-01 20:19:09.000000 irc_api-0.0.9/src/irc_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:21:58.490130 irc_api-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 13:21:44.000000 irc_api-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-02 13:21:58.490130 irc_api-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-02 13:21:44.000000 irc_api-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-02 13:21:44.000000 irc_api-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:21:58.490130 irc_api-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:21:58.490130 irc_api-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:21:58.490130 irc_api-1.0.0/src/irc_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/irc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-02 13:21:44.000000 irc_api-1.0.0/src/irc_api/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:21:58.490130 irc_api-1.0.0/src/irc_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-02 13:21:58.000000 irc_api-1.0.0/src/irc_api.egg-info/top_level.txt
```

### Comparing `irc_api-0.0.9/LICENSE` & `irc_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.9/PKG-INFO` & `irc_api-1.0.0/src/irc_api.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irc_api
-Version: 0.0.9
+Name: irc-api
+Version: 1.0.0
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # IRC API
 [![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest)
 
-## Licence
-The code is provided under GNU General Public Licence version 3 or later (GPLv3+).
+## Description
+IRC API is a small API to make Python IRC bots. This API is based on decorators to make commands like the `cog` module in `discord.py`.
 
-See LICENCE for more informations.
+If you encounter any issue feel free to [open one](https://github.com/Shadow15510/irc_api/issues).
+A full documentation is available on [readthedocs](https://irc-api.readthedocs.io/en/latest/).
 
-## Description
+## Installation
+To install IRC API, you should use ``pip install irc-api``, check out the [Pypi project page](https://pypi.org/project/irc-api/) for more informations.
 
-IRC API is an api to make IRC bots.
+## Licence
+This project is under GNU General Public Licence v3.0 or later (GPLv3+).
+Please see [LICENCE](https://github.com/Shadow15510/irc_api/blob/master/LICENSE) for more informations
```

### Comparing `irc_api-0.0.9/pyproject.toml` & `irc_api-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.9/src/irc_api/bot.py` & `irc_api-1.0.0/src/irc_api/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Provide a Bot class that react to IRC's message and events."""
 
 import logging
-from threading import Thread
 import time
 import re
 
+from threading import Thread
 from irc_api.irc import IRC
 from irc_api.history import History
 
-PREFIX = ""
 
 class Bot:
-    """Run the connexion between IRC's server and V5 one.
+    """Watch the IRC server and handle commands.
 
     Attributes
     ----------
     prefix : str, public
         The bot's prefix for named command.
-    irc : IRC, public
+    irc : irc_api.irc.IRC, public
         IRC wrapper which handle communication with IRC server.
-    history : History, public
+    history : irc_api.history.History, public
         The messages history. 
     channels : list, public
         The channels the bot will listen.
     auth : tuple, public
         This contains the username and the password for a SASL auth.
     callbacks : dict, public
         The callbacks of the bot. This dictionnary is like {name: command} where name is the name of
@@ -47,15 +46,15 @@
         Allow to add a module of command to the bot.
     remove_command : NoneType, public
         Remove a command.
     """
     def __init__(
             self,
             irc_params: tuple,
-            *commands_modules
+            *commands_modules,
             auth: tuple=(),
             channels: list=["#general"],
             prefix: str="",
             limit: int=100,
         ):
         """Initialize the Bot instance.
 
@@ -82,17 +81,15 @@
             my_bot = api.Bot(
                     irc_params=(irc.exemple.com, 6697),
                     channels=["#general", "#bot-test"],
                     prefix="!",
                     cmnd_pack1, cmnd_pack2
                 )
         """
-        global PREFIX
-        PREFIX = prefix
-        self.prefix = PREFIX
+        self.prefix = prefix
 
         self.irc = IRC(*irc_params)
         self.history = History(limit)
         self.channels = channels
         self.auth = auth
         self.callbacks = {}
         self.commands_help = {}
@@ -116,25 +113,24 @@
         for channel in self.channels:
             self.irc.join(channel)
 
         # mainloop
         while True:
             message = self.irc.receive()
             self.history.add(message)
-            logging.info("received %s", message)
+            
             if message is not None:
                 for callback in self.callbacks.values():
                     if not False in [event(message) for event in callback.events]:
-                        logging.info("matched %s", callback.name)
-
-                        # others command types
+                        logging.info("callback triggered: %s", callback.name)
+                        # event commands
                         if callback.cmnd_type == 0:
                             callback(message)
 
-                        # @api.command
+                        # named commands
                         elif callback.cmnd_type == 1:
                             args = check_args(callback.func, *parse(message.text)[1:])
                             if isinstance(args, list):
                                 callback(message, *args)
                             else:
                                 self.send(
                                         message.to,
@@ -162,20 +158,28 @@
         command : BotCommand
             The command to add to the bot.
         add_to_help : bool, optionnal
             If the command should be added to the documented functions.
         """
         command.bot = self
 
+        if command.cmnd_type == 1:
+            command.events.append(
+                    lambda m: True in \
+                    [m.text == self.prefix + cmd or m.text.startswith(f"{self.prefix}{cmd} ")
+                    for cmd in command.alias]
+                )
+
         if command.cmnd_type == 2:
             def timed_func(bot):
                 while True:
                     command.func(bot)
                     time.sleep(command.events)
-                    logging.info("auto call : %s", command.name)
+                    logging.info("automatic callback: %s", command.name)
+                    
 
             self.threads.append(Thread(target=timed_func, args=(self,)))
             self.threads[-1].start()
         else:
             self.callbacks[command.name] = command
 
         if add_to_help:
```

### Comparing `irc_api-0.0.9/src/irc_api/commands.py` & `irc_api-1.0.0/src/irc_api/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Defines the decorators for bot commands."""
-from irc_api.bot import BotCommand, PREFIX
+from irc_api.bot import BotCommand
 
 def command(name: str, alias: tuple=(), desc: str=""):
     """Create a new bot's command. Note that's a decorator.
     
     Parameters
     ----------
     name : str
@@ -29,25 +29,23 @@
         @commands.command(name="ping", desc="Answer 'pong' when the user enters 'ping'.")
         def foo(bot, message):
             bot.send(message.to, "pong")
     """
     if not alias or not name in alias:
         alias += (name,)
     def decorator(func):
-        return BotCommand(
+        cmnd = BotCommand(
                 name=name,
                 func=func,
-                events=[
-                        lambda m: True in \
-                        [m.text == PREFIX + cmd or m.text.startswith(PREFIX + cmd + " ")
-                        for cmd in alias]
-                    ],
+                events=[],
                 desc=desc,
                 cmnd_type=1
             )
+        cmnd.alias = alias
+        return cmnd
     return decorator
 
 
 def on(event, desc: str=""):
     """Make a command on a custom event. It can be useful if you want to have a complex calling
     processus. Such as a regex recognition or a specific pattern. This decorator allows you to call
     a command when a specific event is verified.
@@ -238,13 +236,13 @@
     """Auto generated help command."""
     if fct_name and fct_name in bot.commands_help.keys():
         cmnd = bot.commands_help[fct_name]
         answer = f"Help on the command: {bot.prefix}{fct_name}\n"
         for line in bot.commands_help[fct_name].desc.splitlines():
             answer += f" │ {line}\n"
     else:
-        answer = f"List of available commands ({PREFIX}help <cmnd> for more informations)\n"
+        answer = f"List of available commands ({bot.prefix}help <cmnd> for more informations)\n"
         for cmnd_name, cmnd in bot.commands_help.items():
             if cmnd.cmnd_type == 1:
                 answer += f" - {cmnd_name}\n"
 
     bot.send(msg.to, answer)
```

### Comparing `irc_api-0.0.9/src/irc_api/history.py` & `irc_api-1.0.0/src/irc_api/history.py`

 * *Files identical despite different names*

### Comparing `irc_api-0.0.9/src/irc_api/irc.py` & `irc_api-1.0.0/src/irc_api/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import logging
 import socket
 import ssl
 
 from queue import Queue
 from threading import Thread
-
 from irc_api.message import Message
 
 
 class IRC:
     """Manage connexion to an IRC server, authentication and callbacks.
 
     Attributes
@@ -106,26 +105,27 @@
             The incoming processed private message.
         """
         while True:
             message = self.__inbox.get()
             if " PRIVMSG " in message:
                 msg = Message(message)
                 if msg:
+                    logging.info("receive: %s", msg)
                     return msg
 
     def join(self, channel: str):
         """Join a channel.
         
         Parameters
         ----------
         channel : str
             The name of the channel to join.
         """
+        logging.info("join %s", channel)
         self.send(f"JOIN {channel}")
-        logging.info("joined %s", channel)
 
     def waitfor(self, condition):
         """Wait for a raw message that matches the condition.
 
         Parameters
         ----------
         condition : function
@@ -153,9 +153,8 @@
             for msg in data.split('\r\n'):
                 # Manage ping
                 if msg.startswith("PING"):
                     self.send(msg.replace("PING", "PONG"))
 
                 # Or add a new message to inbox
                 elif len(msg):
-                    self.__inbox.put(msg)
-                    logging.debug("received %s", msg)
+                    self.__inbox.put(msg)
```

### Comparing `irc_api-0.0.9/src/irc_api/message.py` & `irc_api-1.0.0/src/irc_api/message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Parse the raw incoming message into a Message instance."""
 
 import re
-import logging
+
 
 class Message:
     """Parse the raw message in three fields: the author, the channel and the text content.
     
     Attributes
     ----------
     pattern : re.Pattern, public
@@ -30,17 +30,15 @@
             The raw received message.
         """
         match = re.search(Message.pattern, raw)
         if match:
             self.author = match.group("author")
             self.to = match.group("to")
             self.text = match.group("text")
-            logging.debug("sucessfully parsed %s into %s", raw, self.__str__())
         else:
             self.author = ""
             self.to = ""
             self.text = ""
-            logging.warning("failed to parse %s into valid message", raw)
 
     def __str__(self):
         """Convert the Message's instance into a human readable string."""
         return f"{self.author} to {self.to}: {self.text}"
```

### Comparing `irc_api-0.0.9/src/irc_api.egg-info/PKG-INFO` & `irc_api-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irc-api
-Version: 0.0.9
+Name: irc_api
+Version: 1.0.0
 Summary: An API written in Python to make IRC bots.
 Author: Sha-chan
 Project-URL: Homepage, https://github.com/Shadow15510/irc_api
 Project-URL: Documentation, https://irc-api.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 License-File: LICENSE
 
 # IRC API
 [![Documentation Status](https://readthedocs.org/projects/irc-api/badge/?version=latest)](https://irc-api.readthedocs.io/en/latest/?badge=latest)
 
-## Licence
-The code is provided under GNU General Public Licence version 3 or later (GPLv3+).
+## Description
+IRC API is a small API to make Python IRC bots. This API is based on decorators to make commands like the `cog` module in `discord.py`.
 
-See LICENCE for more informations.
+If you encounter any issue feel free to [open one](https://github.com/Shadow15510/irc_api/issues).
+A full documentation is available on [readthedocs](https://irc-api.readthedocs.io/en/latest/).
 
-## Description
+## Installation
+To install IRC API, you should use ``pip install irc-api``, check out the [Pypi project page](https://pypi.org/project/irc-api/) for more informations.
 
-IRC API is an api to make IRC bots.
+## Licence
+This project is under GNU General Public Licence v3.0 or later (GPLv3+).
+Please see [LICENCE](https://github.com/Shadow15510/irc_api/blob/master/LICENSE) for more informations
```

