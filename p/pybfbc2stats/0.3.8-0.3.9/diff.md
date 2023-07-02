# Comparing `tmp/pybfbc2stats-0.3.8.tar.gz` & `tmp/pybfbc2stats-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybfbc2stats-0.3.8.tar", last modified: Wed Sep 14 19:10:08 2022, max compression
+gzip compressed data, was "pybfbc2stats-0.3.9.tar", last modified: Tue Mar  7 17:09:27 2023, max compression
```

## Comparing `pybfbc2stats-0.3.8.tar` & `pybfbc2stats-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-14 19:10:08.431911 pybfbc2stats-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)    15234 2022-09-14 19:10:08.431911 pybfbc2stats-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    14585 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-14 19:10:08.431911 pybfbc2stats-0.3.8/pybfbc2stats/
--rw-r--r--   0 runner    (1001) docker     (116)     1149 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pybfbc2stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16314 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pybfbc2stats/asyncio_client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5117 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pybfbc2stats/asyncio_connection.py
--rw-r--r--   0 runner    (1001) docker     (116)    32127 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pybfbc2stats/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     5412 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pybfbc2stats/connection.py
--rw-r--r--   0 runner    (1001) docker     (116)    35154 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pybfbc2stats/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)      421 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pybfbc2stats/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)       56 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pybfbc2stats/logger.py
--rw-r--r--   0 runner    (1001) docker     (116)     6530 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pybfbc2stats/packet.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-14 19:10:08.431911 pybfbc2stats-0.3.8/pybfbc2stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    15234 2022-09-14 19:10:08.000000 pybfbc2stats-0.3.8/pybfbc2stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      438 2022-09-14 19:10:08.000000 pybfbc2stats-0.3.8/pybfbc2stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-14 19:10:08.000000 pybfbc2stats-0.3.8/pybfbc2stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2022-09-14 19:10:08.000000 pybfbc2stats-0.3.8/pybfbc2stats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      103 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      698 2022-09-14 19:10:08.431911 pybfbc2stats-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-09-14 19:09:52.000000 pybfbc2stats-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 17:09:27.046692 pybfbc2stats-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1074 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (116)    16386 2023-03-07 17:09:27.046692 pybfbc2stats-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    15737 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 17:09:27.042692 pybfbc2stats-0.3.9/pybfbc2stats/
+-rw-r--r--   0 runner    (1001) docker     (116)     1149 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15411 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/asyncio_client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4712 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/asyncio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)      687 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (116)    34863 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5011 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)    35499 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/constants.py
+-rw-r--r--   0 runner    (1001) docker     (116)      421 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)       56 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/logger.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10990 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pybfbc2stats/packet.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-07 17:09:27.042692 pybfbc2stats-0.3.9/pybfbc2stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    16386 2023-03-07 17:09:27.000000 pybfbc2stats-0.3.9/pybfbc2stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      461 2023-03-07 17:09:27.000000 pybfbc2stats-0.3.9/pybfbc2stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-07 17:09:27.000000 pybfbc2stats-0.3.9/pybfbc2stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2023-03-07 17:09:27.000000 pybfbc2stats-0.3.9/pybfbc2stats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      103 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      698 2023-03-07 17:09:27.046692 pybfbc2stats-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-07 17:09:17.000000 pybfbc2stats-0.3.9/setup.py
```

### Comparing `pybfbc2stats-0.3.8/LICENSE.md` & `pybfbc2stats-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybfbc2stats-0.3.8/PKG-INFO` & `pybfbc2stats-0.3.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-Metadata-Version: 2.1
-Name: pybfbc2stats
-Version: 0.3.8
-Summary: Python library for retrieving statistics of Battlefield: Bad Company 2 players
-Home-page: https://github.com/cetteup/pybfbc2stats
-Author: cetteup
-Author-email: me@cetteup.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/cetteup/pybfbc2stats/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # pybfbc2stats
 
 Python 🐍 library for retrieving statistics of Battlefield: Bad Company 2 players. Possible thanks to previous work by Luigi Auriemma and nemo.
 
+[![ci](https://img.shields.io/github/workflow/status/cetteup/pybfbc2stats/ci?label=ci)](https://github.com/cetteup/pybfbc2stats/actions?query=workflow%3Aci)
+[![License](https://img.shields.io/github/license/cetteup/pybfbc2stats)](/LICENSE)
+[![Package](https://img.shields.io/pypi/v/pybfbc2stats)](https://pypi.org/project/pybfbc2stats/)
+[![Last commit](https://img.shields.io/github/last-commit/cetteup/pybfbc2stats)](https://github.com/cetteup/pybfbc2stats/commits/main)
+
 ## Features
 
 - lookup players/personas by id or name on any platform
 - search for players/personas by name on any platform (with wildcard support)
 - retrieve all available statistics for players on PC/PS3
 - retrieve player leaderboards on PC/PS3
 - retrieve server list for PC/PS3
@@ -436,18 +423,40 @@
 
 Retrieve full details and player list for a given server.
 
 **Arguments**
 
   Argument     | Type | Opt/Required | Note
 ---------------|------|--------------|-----
-lobby_id       | int  | Required     | If of the game server lobby the server is hosted in
+lobby_id       | int  | Required     | Id of the game server lobby the server is hosted in
 game_id        | int  | Required     | Game (server) id
 
 **Example**
 
 ```python
 from pybfbc2stats import TheaterClient, Platform
 
 client = TheaterClient('bfbc2-ps3-server.theater.ea.com', 18336, 'your_lkey', Platform.ps3)
 general, detailed, players = client.get_server_details(257, 120018)
 ```
+
+----
+
+#### \[Async\]TheaterClient.get_current_server(user_id)
+
+Retrieve full details and player list for a given user's current server (server they are currently playing on, 
+raises a PlayerNotFound exception if the player is not currently playing online).
+
+**Arguments**
+
+  Argument     | Type | Opt/Required | Note
+---------------|------|--------------|-----
+user_id       | int  | Required     | Id of the user whose current server to get
+
+**Example**
+
+```python
+from pybfbc2stats import TheaterClient, Platform
+
+client = TheaterClient('bfbc2-ps3-server.theater.ea.com', 18336, 'your_lkey', Platform.ps3)
+general, detailed, players = client.get_current_server(227528903)
+```
```

### Comparing `pybfbc2stats-0.3.8/README.md` & `pybfbc2stats-0.3.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,34 @@
+Metadata-Version: 2.1
+Name: pybfbc2stats
+Version: 0.3.9
+Summary: Python library for retrieving statistics of Battlefield: Bad Company 2 players
+Home-page: https://github.com/cetteup/pybfbc2stats
+Author: cetteup
+Author-email: me@cetteup.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/cetteup/pybfbc2stats/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # pybfbc2stats
 
 Python 🐍 library for retrieving statistics of Battlefield: Bad Company 2 players. Possible thanks to previous work by Luigi Auriemma and nemo.
 
+[![ci](https://img.shields.io/github/workflow/status/cetteup/pybfbc2stats/ci?label=ci)](https://github.com/cetteup/pybfbc2stats/actions?query=workflow%3Aci)
+[![License](https://img.shields.io/github/license/cetteup/pybfbc2stats)](/LICENSE)
+[![Package](https://img.shields.io/pypi/v/pybfbc2stats)](https://pypi.org/project/pybfbc2stats/)
+[![Last commit](https://img.shields.io/github/last-commit/cetteup/pybfbc2stats)](https://github.com/cetteup/pybfbc2stats/commits/main)
+
 ## Features
 
 - lookup players/personas by id or name on any platform
 - search for players/personas by name on any platform (with wildcard support)
 - retrieve all available statistics for players on PC/PS3
 - retrieve player leaderboards on PC/PS3
 - retrieve server list for PC/PS3
@@ -418,18 +441,40 @@
 
 Retrieve full details and player list for a given server.
 
 **Arguments**
 
   Argument     | Type | Opt/Required | Note
 ---------------|------|--------------|-----
-lobby_id       | int  | Required     | If of the game server lobby the server is hosted in
+lobby_id       | int  | Required     | Id of the game server lobby the server is hosted in
 game_id        | int  | Required     | Game (server) id
 
 **Example**
 
 ```python
 from pybfbc2stats import TheaterClient, Platform
 
 client = TheaterClient('bfbc2-ps3-server.theater.ea.com', 18336, 'your_lkey', Platform.ps3)
 general, detailed, players = client.get_server_details(257, 120018)
 ```
+
+----
+
+#### \[Async\]TheaterClient.get_current_server(user_id)
+
+Retrieve full details and player list for a given user's current server (server they are currently playing on, 
+raises a PlayerNotFound exception if the player is not currently playing online).
+
+**Arguments**
+
+  Argument     | Type | Opt/Required | Note
+---------------|------|--------------|-----
+user_id       | int  | Required     | Id of the user whose current server to get
+
+**Example**
+
+```python
+from pybfbc2stats import TheaterClient, Platform
+
+client = TheaterClient('bfbc2-ps3-server.theater.ea.com', 18336, 'your_lkey', Platform.ps3)
+general, detailed, players = client.get_current_server(227528903)
+```
```

### Comparing `pybfbc2stats-0.3.8/pybfbc2stats/__init__.py` & `pybfbc2stats-0.3.9/pybfbc2stats/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     NotFoundError, ServerNotFoundError, LobbyNotFoundError
 
 """
 pybfbc2stats.
 Python library for retrieving statistics of Battlefield: Bad Company 2 players.
 """
 
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 __author__ = 'cetteup'
 __credits__ = 'nemo, Luigi Auriemma'
 __all__ = ['Connection', 'SecureConnection', 'FeslClient', 'TheaterClient',
            'AsyncConnection', 'AsyncSecureConnection', 'AsyncFeslClient', 'AsyncTheaterClient',
            'Platform', 'Namespace', 'DEFAULT_LEADERBOARD_KEYS', 'STATS_KEYS',
            'Error', 'ConnectionError', 'ParameterError', 'TimeoutError',
            'AuthError', 'NotFoundError', 'PlayerNotFoundError',
```

### Comparing `pybfbc2stats-0.3.8/pybfbc2stats/asyncio_client.py` & `pybfbc2stats-0.3.9/pybfbc2stats/asyncio_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,19 +17,14 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *excinfo):
         await self.connection.close()
 
     async def wrapped_read(self, tid: int) -> Packet:
-        """
-        Read a single packet from the connection and automatically respond plus read next packet if the initial packet
-        was one that requires an immediate response (memcheck, ping)
-        :return: A packet containing "real" data
-        """
         initial_packet = await self.connection.read()
 
         # Check packet is not a "real" data packet but one that prompts a response (memcheck, ping)
         auto_respond, handler = self.is_auto_respond_packet(initial_packet)
         if auto_respond:
             # Call auto respond handler
             await handler()
@@ -218,50 +213,42 @@
                  for (key, value) in persona.items()} for persona in parsed_response]
 
     async def get_list_response(self, tid: int, list_entry_prefix: bytes) -> Tuple[List[dict], List[bytes]]:
         response = b''
         last_packet = False
         while not last_packet:
             packet = await self.wrapped_read(tid)
-            data, last_packet = self.handle_list_response_packet(packet, list_entry_prefix)
+            data, last_packet = self.handle_list_response_packet(packet)
             response += data
 
         return self.parse_list_response(response, list_entry_prefix)
 
 
 class AsyncTheaterClient(TheaterClient, AsyncClient):
     def __init__(self, host: str, port: int, lkey: str, platform: Platform, timeout: float = 3.0,
                  track_steps: bool = True):
         connection = AsyncConnection(host, port, TheaterPacket)
         # "Skip" TheaterClient constructor, for details see note in AsyncFeslClient.__init__
         super(TheaterClient, self).__init__(connection, platform, timeout, track_steps)
         self.lkey = lkey.encode('utf8')
 
     async def connect(self) -> bytes:
-        """
-        Initialize the connection to the Theater backend by sending the initial CONN/hello packet
-        :return: Response packet data
-        """
         if self.track_steps and TheaterStep.conn in self.completed_steps:
             return bytes(self.completed_steps[TheaterStep.conn])
 
         tid = self.get_transaction_id()
         connect_packet = self.build_conn_paket(tid, BACKEND_DETAILS[self.platform]['clientString'])
         await self.connection.write(connect_packet)
 
         response = await self.connection.read()
         self.completed_steps[TheaterStep.conn] = response
 
         return bytes(response)
 
     async def authenticate(self) -> bytes:
-        """
-        Authenticate against/log into the Theater backend using the lkey retrieved via FESL
-        :return: Response packet data
-        """
         if self.track_steps and TheaterStep.user in self.completed_steps:
             return bytes(self.completed_steps[TheaterStep.user])
         elif self.track_steps and TheaterStep.conn not in self.completed_steps:
             await self.connect()
 
         tid = self.get_transaction_id()
         auth_packet = self.build_user_packet(tid, self.lkey)
@@ -277,18 +264,14 @@
         return bytes(response)
 
     async def ping(self) -> None:
         ping_packet = self.build_ping_packet()
         await self.connection.write(ping_packet)
 
     async def get_lobbies(self) -> List[dict]:
-        """
-        Retrieve all available game (server) lobbies
-        :return: List of lobby details
-        """
         if self.track_steps and TheaterStep.user not in self.completed_steps:
             await self.authenticate()
 
         tid = self.get_transaction_id()
         lobby_list_packet = self.build_llst_packet(tid)
         await self.connection.write(lobby_list_packet)
 
@@ -304,19 +287,14 @@
             ldat_response = await self.wrapped_read(tid)
             ldat = self.parse_simple_response(ldat_response)
             lobbies.append(ldat)
 
         return lobbies
 
     async def get_servers(self, lobby_id: int) -> List[dict]:
-        """
-        Retrieve all available game servers from the given lobby
-        :param lobby_id: Id of the game server lobby
-        :return: List of server details
-        """
         if self.track_steps and TheaterStep.user not in self.completed_steps:
             await self.authenticate()
 
         tid = self.get_transaction_id()
         server_list_packet = self.build_glst_packet(tid, str(lobby_id).encode('utf8'))
         await self.connection.write(server_list_packet)
 
@@ -336,28 +314,27 @@
             gdat_response = await self.wrapped_read(tid)
             gdat = self.parse_simple_response(gdat_response)
             servers.append(gdat)
 
         return servers
 
     async def get_server_details(self, lobby_id: int, game_id: int) -> Tuple[dict, dict, List[dict]]:
-        """
-        Retrieve full details and player list for a given server
-        :param lobby_id: If of the game server lobby the server is hosted in
-        :param game_id: Game (server) id
-        :return: Tuple of (general server details, extended details, player list)
-        """
+        return await self.get_gdat(lid=str(lobby_id).encode('utf8'), gid=str(game_id).encode('utf8'))
+
+    async def get_current_server(self, user_id: int) -> Tuple[dict, dict, List[dict]]:
+        return await self.get_gdat(uid=str(user_id).encode('utf8'))
+
+    async def get_gdat(self, **kwargs: bytes) -> Tuple[dict, dict, List[dict]]:
         if self.track_steps and TheaterStep.user not in self.completed_steps:
             await self.authenticate()
 
         tid = self.get_transaction_id()
         server_details_packet = self.build_gdat_packet(
             tid,
-            str(lobby_id).encode('utf8'),
-            str(game_id).encode('utf8')
+            **kwargs
         )
         await self.connection.write(server_details_packet)
 
         # Similar structure to before, but with one difference: Theater returns a GDAT packet (general game data),
         # followed by a GDET packet (extended server data). Finally, it sends a PDAT packet for every player
         gdat_response = await self.wrapped_read(tid)
         # Response may indicate an error if given lobby id and /or game id do not exist
```

### Comparing `pybfbc2stats-0.3.8/pybfbc2stats/asyncio_connection.py` & `pybfbc2stats-0.3.9/pybfbc2stats/asyncio_connection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import socket
 import time
 from typing import Tuple, Type
 
+from .buffer import Buffer
 from .connection import Connection, SecureConnection
-from .constants import HEADER_LENGTH
 from .exceptions import TimeoutError, ConnectionError
 from .logger import logger
 from .packet import Packet
 
 
 class AsyncConnection(Connection):
     sock: socket.socket
@@ -33,91 +33,78 @@
             self.is_connected = False
             raise TimeoutError(f'Connection attempt to {self.host}:{self.port} timed out')
         except (socket.error, ConnectionResetError) as e:
             self.is_connected = False
             raise ConnectionError(f'Failed to connect to {self.host}:{self.port} ({e})')
 
     async def write(self, packet: Packet) -> None:
-        logger.debug('Writing to socket')
         if not self.is_connected:
             logger.debug('Socket is not connected yet, connecting now')
             await self.connect()
 
+        logger.debug('Writing to socket')
+
         try:
             self.writer.write(bytes(packet))
             await self.writer.drain()
         except (socket.error, ConnectionResetError, RuntimeError) as e:
             raise ConnectionError(f'Failed to send data to server ({e})')
 
         logger.debug(packet)
 
     async def read(self) -> Packet:
-        logger.debug('Reading from socket')
         if not self.is_connected:
             logger.debug('Socket is not connected yet, connecting now')
             await self.connect()
 
-        # Init empty packet
-        packet = self.packet_type()
+        logger.debug('Reading from socket')
 
-        # Read header only first
-        logger.debug('Reading packet header')
+        packet = self.packet_type()
         last_received = time.time()
         timed_out = False
-        while len(packet.header) < HEADER_LENGTH and not timed_out:
-            iteration_buffer = await self.read_safe(HEADER_LENGTH - len(packet.header))
-            packet.header += iteration_buffer
-
-            # Update timestamp if any data was retrieved during current iteration
-            if len(iteration_buffer) > 0:
-                last_received = time.time()
-            timed_out = time.time() > last_received + self.timeout
+        while (packet_buflen := packet.buflen()) > 0 and not timed_out:
+            iteration_buffer = await self.read_safe(packet_buflen)
 
-        logger.debug(packet.header)
+            # Append whatever data is missing from the header to it
+            if (header_buflen := packet.header_buflen()) > 0:
+                packet.header += iteration_buffer.read(min(header_buflen, iteration_buffer.length))
+                # Log packet header once complete
+                if packet.header_buflen() == 0:
+                    logger.debug(f'Received header: {packet.header}')
 
-        # Make sure packet header is valid (throws exception if invalid)
-        packet.validate_header()
+                    # Make sure packet header is valid (throws exception if invalid)
+                    packet.validate_header()
 
-        if timed_out:
-            raise TimeoutError('Timed out while reading packet header')
-
-        # Read number of bytes indicated by packet header
-        logger.debug('Reading packet body')
-        last_received = time.time()
-        timed_out = False
-        while len(packet.body) < packet.indicated_body_length() and not timed_out:
-            iteration_buffer = await self.read_safe(packet.indicated_body_length() - len(packet.body))
-            packet.body += iteration_buffer
+            # Append any remaining data to body
+            packet.body += iteration_buffer.get_buffer()
 
             # Update timestamp if any data was retrieved during current iteration
-            if len(iteration_buffer) > 0:
+            if iteration_buffer.length > 0:
                 last_received = time.time()
             timed_out = time.time() > last_received + self.timeout
 
-        logger.debug(packet.body)
-
         if timed_out:
-            raise TimeoutError('Timed out while reading packet body')
+            raise TimeoutError('Timed out while reading packet header')
+
+        logger.debug(f'Received body: {packet.body}')
 
         # Validate packet body (throws exception if invalid)
         packet.validate_body()
 
         return packet
 
-    async def read_safe(self, buflen: int) -> bytes:
+    async def read_safe(self, buflen: int) -> Buffer:
         future = self.reader.read(buflen)
         try:
-            buffer = await asyncio.wait_for(future, self.timeout)
+            return Buffer(await asyncio.wait_for(future, self.timeout))
         except (socket.timeout, asyncio.TimeoutError):
             raise TimeoutError('Timed out while receiving server data')
         except (socket.error, ConnectionResetError) as e:
             raise ConnectionError(f'Failed to receive data from server ({e})')
 
-        return buffer
-
     async def open_connection(self) -> Tuple[asyncio.StreamReader, asyncio.StreamWriter]:
         return await asyncio.open_connection(sock=self.sock)
 
     def __del__(self):
         pass
 
     async def close(self) -> bool:
```

### Comparing `pybfbc2stats-0.3.8/pybfbc2stats/client.py` & `pybfbc2stats-0.3.9/pybfbc2stats/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from base64 import b64encode, b64decode
 from typing import List, Union, Dict, Tuple, Optional, Callable
 from urllib.parse import quote_from_bytes, unquote_to_bytes
 
 from .connection import SecureConnection, Connection
 from .constants import STATS_KEYS, DEFAULT_BUFFER_SIZE, FeslStep, Namespace, Platform, BACKEND_DETAILS, LookupType, \
-    DEFAULT_LEADERBOARD_KEYS, Step, TheaterStep
+    DEFAULT_LEADERBOARD_KEYS, Step, TheaterStep, FeslTransmissionType, TheaterTransmissionType
 from .exceptions import ParameterError, Error, PlayerNotFoundError, \
     SearchError, AuthError, ServerNotFoundError, LobbyNotFoundError
 from .packet import Packet, FeslPacket, TheaterPacket
 
 
 class Client:
     platform: Platform
@@ -265,15 +265,15 @@
         return is_auto_respond_packet, handler
 
     def get_list_response(self, tid: int, list_entry_prefix: bytes) -> Tuple[List[dict], List[bytes]]:
         response = b''
         last_packet = False
         while not last_packet:
             packet = self.wrapped_read(tid)
-            data, last_packet = self.handle_list_response_packet(packet, list_entry_prefix)
+            data, last_packet = self.handle_list_response_packet(packet)
             response += data
 
         return self.parse_list_response(response, list_entry_prefix)
 
     @staticmethod
     def build_list_body(items: List[Union[bytes, Dict[bytes, bytes]]], prefix: bytes) -> bytes:
         # Convert item list to bytes following "prefix.index.key=value"-format
@@ -295,81 +295,89 @@
     @staticmethod
     def build_list_item(dotted_elements: List[bytes], value: bytes) -> bytes:
         return b'.'.join(dotted_elements) + b'=' + value
 
     @staticmethod
     def build_hello_packet(tid: int, client_string: bytes) -> FeslPacket:
         return FeslPacket.build(
-            b'fsys\xc0\x00\x00\x00',
+            b'fsys',
             b'TXN=Hello\nclientString=' + client_string +
             b'\nsku=PC\nlocale=en_US\nclientPlatform=PC\nclientVersion=2.0\nSDKVersion=5.1.2.0.0\nprotocolVersion=2.0\n'
             b'fragmentSize=8096\nclientType=server',
+            FeslTransmissionType.SinglePacketRequest,
             tid
         )
 
     @staticmethod
     def build_memcheck_packet() -> FeslPacket:
         return FeslPacket.build(
-            b'fsys\x80\x00\x00\x00',
-            b'TXN=MemCheck\nresult='
+            b'fsys',
+            b'TXN=MemCheck\nresult=',
+            FeslTransmissionType.SinglePacketResponse
         )
 
     @staticmethod
     def build_login_packet(tid: int, username: bytes, password: bytes) -> FeslPacket:
         return FeslPacket.build(
-            b'acct\xc0\x00\x00\x00',
+            b'acct',
             b'TXN=Login\nreturnEncryptedInfo=0\n'
             b'name=' + username + b'\npassword=' + password + b'\nmacAddr=$000000000000',
+            FeslTransmissionType.SinglePacketRequest,
             tid
         )
 
     @staticmethod
     def build_logout_packet(tid: int) -> FeslPacket:
         return FeslPacket.build(
-            b'fsys\xc0\x00\x00\x00',
+            b'fsys',
             b'TXN=Goodbye\nreason=GOODBYE_CLIENT_NORMAL\nmessage="Disconnected via front-end"',
+            FeslTransmissionType.SinglePacketRequest,
             tid
         )
 
     @staticmethod
     def build_ping_packet() -> FeslPacket:
         return FeslPacket.build(
-            b'fsys\x80\x00\x00\x00',
-            b'TXN=Ping'
+            b'fsys',
+            b'TXN=Ping',
+            FeslTransmissionType.SinglePacketResponse
         )
 
     @staticmethod
     def build_user_lookup_packet(tid: int, user_identifiers: List[str],
                                  namespace: Namespace, lookup_type: LookupType) -> FeslPacket:
         user_dicts = [{bytes(lookup_type): identifier.encode('utf8'), b'namespace': bytes(namespace)}
                       for identifier in user_identifiers]
         lookup_list = FeslClient.build_list_body(user_dicts, b'userInfo')
         return FeslPacket.build(
-            b'acct\xc0\x00\x00\x00',
+            b'acct',
             b'TXN=NuLookupUserInfo\n' + lookup_list,
+            FeslTransmissionType.SinglePacketRequest,
             tid
         )
 
     @staticmethod
     def build_search_packet(tid: int, screen_name: str, namespace: Namespace) -> FeslPacket:
         return FeslPacket.build(
-            b'acct\xc0\x00\x00\x00',
+            b'acct',
             b'TXN=NuSearchOwners\nscreenName=' + screen_name.encode('utf8') + b'\nsearchType=1\nretrieveUserIds=0\n'
             b'nameSpaceId=' + bytes(namespace),
+            FeslTransmissionType.SinglePacketRequest,
             tid
         )
 
     @staticmethod
     def build_leaderboard_query_packet(tid: int, min_rank: int, max_rank: int,
                                        sort_by: bytes, keys: List[bytes]) -> FeslPacket:
         key_list = FeslClient.build_list_body(keys, b'keys')
         return FeslPacket.build(
-            b'rank\xc0\x00\x00\x00',
+            b'rank',
             b'TXN=GetTopNAndStats\nkey=' + sort_by + b'\nownerType=1\nminRank=' + str(min_rank).encode('utf8') +
             b'\nmaxRank=' + str(max_rank).encode('utf8') + b'\nperiodId=0\nperiodPast=0\nrankOrder=0\n' + key_list,
+            FeslTransmissionType.SinglePacketRequest,
             tid
         )
 
     @staticmethod
     def build_stats_query_packets(tid: int, userid: int, keys: List[bytes]) -> List[FeslPacket]:
         userid_bytes = str(userid).encode('utf8')
         key_list = FeslClient.build_list_body(keys, b'keys')
@@ -384,16 +392,17 @@
         stats_query_enc = quote_from_bytes(stats_query_b64).encode('utf8')
 
         # Split query into chunks and build packets around them
         chunk_packets = []
         for i in range(0, len(stats_query_enc), available_packet_length):
             query_chunk = stats_query_enc[i:i + available_packet_length]
             chunk_packet = FeslPacket.build(
-                b'rank\xf0\x00\x00\x00',
+                b'rank',
                 b'size=' + encoded_query_size.encode('utf8') + b'\ndata=' + query_chunk,
+                FeslTransmissionType.MultiPacketRequest,
                 tid
             )
             chunk_packets.append(chunk_packet)
 
         return chunk_packets
 
     @staticmethod
@@ -449,15 +458,17 @@
             else:
                 # Add scaler value to dict
                 datasets[index][key] = value
 
         return datasets, meta_lines
 
     @staticmethod
-    def handle_list_response_packet(packet: Packet, list_entry_prefix: bytes) -> Tuple[bytes, bool]:
+    def handle_list_response_packet(packet: Packet) -> Tuple[bytes, bool]:
+        # Fifth byte indicates whether packet is single/multi packet request/response or ping packet
+        transmission_type = packet.get_transmission_type()
         body = packet.get_data()
         lines = packet.get_data_lines()
 
         # Check for errors
         if b'errorCode' in body:
             method_line = next((line for line in lines if line.startswith(b'TXN')), b'')
             method = method_line.split(b'=').pop()
@@ -468,19 +479,20 @@
             elif error_code == b'101' and method == b'NuLookupUserInfo':
                 raise PlayerNotFoundError('FESL returned player not found error')
             elif error_code == b'104' and method == b'NuSearchOwners':
                 # Error code is returned if a) no results matched the query or b) too many results matched the query
                 raise SearchError('FESL found no or too many results matching the search query')
             else:
                 raise Error(f'FESL returned an error (code {error_code.decode("utf")})')
-        elif b'data=' not in body and list_entry_prefix + b'[]' not in body:
+        elif transmission_type is not FeslTransmissionType.SinglePacketResponse and \
+                transmission_type is not FeslTransmissionType.MultiPacketResponse:
             # Packet is neither one data packet of a multi-packet response nor a single-packet response
             raise Error('FESL returned invalid response')
 
-        if b'data=' in body:
+        if transmission_type is FeslTransmissionType.MultiPacketResponse:
             # Packet is one of multiple => base64 decode content
             data_line = next(line for line in lines if line.startswith(b'data='))
             # URL decode/unquote and base64 decode data
             data = b64decode(unquote_to_bytes(data_line[5:]))
             last_packet = data[-1:] == b'\x00'
             # Remove "eof" indicator from last packet's data
             if last_packet:
@@ -615,23 +627,45 @@
             servers.append(gdat)
 
         return servers
 
     def get_server_details(self, lobby_id: int, game_id: int) -> Tuple[dict, dict, List[dict]]:
         """
         Retrieve full details and player list for a given server
-        :param lobby_id: If of the game server lobby the server is hosted in
+        :param lobby_id: Id of the game server lobby the server is hosted in
         :param game_id: Game (server) id
         :return: Tuple of (general server details, extended details, player list)
         """
+        return self.get_gdat(lid=str(lobby_id).encode('utf8'), gid=str(game_id).encode('utf8'))
+
+    def get_current_server(self, user_id: int) -> Tuple[dict, dict, List[dict]]:
+        """
+        Retrieve full details and player list for a given user's current server (server they are currently playing on,
+        raises a PlayerNotFound exception if the player is not currently playing online)
+        :param user_id: Id of the user whose current server to get
+        :return: Tuple of (general server details, extended details, player list)
+        """
+        return self.get_gdat(uid=str(user_id).encode('utf8'))
+
+    def get_gdat(self, **kwargs: bytes)  -> Tuple[dict, dict, List[dict]]:
+        """
+        Get GDAT for an individual server
+        :param kwargs: Id(s) to identify the game (server):
+            a) id of lobby the game server is hosted in (lid) and Id of the game server or (gid)
+            b) id of user for which the current server should be returned (uid)
+        :return: Tuple of (general server details, extended details, player list)
+        """
         if self.track_steps and TheaterStep.user not in self.completed_steps:
             self.authenticate()
 
         tid = self.get_transaction_id()
-        server_details_packet = self.build_gdat_packet(tid, str(lobby_id).encode('utf8'), str(game_id).encode('utf8'))
+        server_details_packet = self.build_gdat_packet(
+            tid,
+            **kwargs
+        )
         self.connection.write(server_details_packet)
 
         # Similar structure to before, but with one difference: Theater returns a GDAT packet (general game data),
         # followed by a GDET packet (extended server data). Finally, it sends a PDAT packet for every player
         gdat_response = self.wrapped_read(tid)
         # Response may indicate an error if given lobby id and /or game id do not exist
         is_error, error = self.is_error_response(gdat_response)
@@ -667,100 +701,117 @@
         """
         Build the initial hello/connection packet
         :param tid: Transaction id (usually 1, must be sent as first packet)
         :param client_string: Game client string (e.g. "bfbc2-pc")
         :return: Complete packet to establish connection
         """
         return TheaterPacket.build(
-            b'CONN@\x00\x00\x00',
+            b'CONN',
             b'PROT=2\nPROD=' + client_string + b'\nVERS=1.1\nPLAT=PC\nLOCALE=en_US\nSDKVERSION=5.0.0.0.0',
+            TheaterTransmissionType.Request,
             tid
         )
 
     @staticmethod
     def build_user_packet(tid: int, lkey: bytes) -> TheaterPacket:
         """
         Build the user/login packet
         :param tid: Transaction id (usually 2, must be sent as second packet)
         :param lkey: Login key from a FESL session
         :return: Complete packet to perform login
         """
         return TheaterPacket.build(
-            b'USER@\x00\x00\x00',
+            b'USER',
             b'MAC=$000000000000\nSKU=125170\nLKEY=' + lkey + b'\nNAME=',
+            TheaterTransmissionType.Request,
             tid
         )
 
     @staticmethod
     def build_ping_packet() -> TheaterPacket:
         """
         Build a ping response packet
         :return: Complete packet to respond to ping with
         """
         return TheaterPacket.build(
-            b'PING\x00\x00\x00\x00',
-            b'TID=0'
+            b'PING',
+            b'TID=0',
+            TheaterTransmissionType.Request
         )
 
     @staticmethod
     def build_llst_packet(tid: int) -> TheaterPacket:
         """
         Build the llst/lobby list packet
         :param tid: Transaction id
         :return: Complete packet to list all available game lobbies
         """
         return TheaterPacket.build(
-            b'LLST@\x00\x00\x00',
+            b'LLST',
             b'FILTER-FAV-ONLY=0\nFILTER-NOT-FULL=0\nFILTER-NOT-PRIVATE=0\nFILTER-NOT-CLOSED=0\nFILTER-MIN-SIZE=0\n'
             b'FAV-PLAYER=\nFAV-GAME=\nFAV-PLAYER-UID=\nFAV-GAME-UID=',
+            TheaterTransmissionType.Request,
             tid
         )
 
     @staticmethod
     def build_glst_packet(tid: int, lid: bytes) -> TheaterPacket:
         """
         Build the glst/game (server) list packet
         :param tid: Transaction id
         :param lid: Id of lobby to retrieve games from
         :return: Complete packet to list all available game servers in lobby
         """
         return TheaterPacket.build(
-            b'GLST@\x00\x00\x00',
+            b'GLST',
             b'LID=' + lid + b'\nTYPE=\nFILTER-FAV-ONLY=0\nFILTER-NOT-FULL=0\nFILTER-NOT-PRIVATE=0\n'
             b'FILTER-NOT-CLOSED=0\nFILTER-MIN-SIZE=0\nFAV-PLAYER=\nFAV-GAME=\nCOUNT=-1\nFAV-PLAYER-UID=\n'
             b'FAV-GAME-UID=',
+            TheaterTransmissionType.Request,
             tid
         )
 
     @staticmethod
-    def build_gdat_packet(tid: int, lid: bytes, gid: bytes) -> TheaterPacket:
+    def build_gdat_packet(tid: int, **kwargs: bytes) -> TheaterPacket:
         """
         Build the gdat/game (server) detailed data packet
         :param tid: Transaction id
-        :param lid: Id of lobby the game server is hosted in
-        :param gid: Id of the game server
+        :param kwargs: Id(s) to identify the game (server):
+            a) id of lobby the game server is hosted in (lid) and Id of the game server or (gid)
+            b) id of user for which the current server should be returned (uid)
         :return: Complete packet to retrieve detailed data for the game server
         """
         return TheaterPacket.build(
-            b'GDAT@\x00\x00\x00',
-            b'LID=' + lid + b'\nGID=' + gid,
+            b'GDAT',
+            b'\n'.join(
+                key.upper().encode('utf8') + b'=' + value
+                for (key, value) in kwargs.items()
+            ),
+            TheaterTransmissionType.Request,
             tid
         )
 
     @staticmethod
     def is_valid_authentication_response(response: Packet) -> bool:
         return b'NAME=' in response.body
 
     @staticmethod
     def is_error_response(response: Packet) -> Tuple[bool, Optional[Error]]:
         is_error, error = False, None
         if response.header.startswith(b'GLSTnrom'):
             # Theater returns a header starting with b'GLSTnrom' ("no room"?, room=lobby?) if the given
             # lobby_id does not exist (only applies to retrieving server lists from lobby,
-            # individual server queries return the above b'GDATngam' instead)
+            # individual server queries return the below b'GDATngam' instead)
             is_error, error = True, LobbyNotFoundError('Theater returned lobby not found error')
         elif response.header.startswith(b'GDATngam'):
-            # Theater returns a header starting with b'GDATngam' ("no game?") if the given
+            # Theater returns a header starting with b'GDATngam' ("no game"?) if the given
             # lobby_id-game_id combination does not exist
             is_error, error = True, ServerNotFoundError('Theater returned server not found error')
+        elif response.header.startswith(b'GDATntfn'):
+            # Theater return a header starting with b'GDATntfn' ("not found"?) both if the user whose uid was given
+            # is not currently playing on any server and if no user with that id exists
+            is_error, error = True, PlayerNotFoundError('Theater returned player not found/not online error')
+        elif response.header[4:8] == b'bpar':
+            # Theater returns a header containing b'bpar' if parameters are not provided correctly
+            is_error, error = True, ParameterError('Theater returned bad parameter error')
 
         return is_error, error
```

### Comparing `pybfbc2stats-0.3.8/pybfbc2stats/connection.py` & `pybfbc2stats-0.3.9/pybfbc2stats/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import socket
 import ssl
 import time
 from typing import Type
 
-from .constants import HEADER_LENGTH
+from .buffer import Buffer
 from .exceptions import TimeoutError, ConnectionError
 from .logger import logger
 from .packet import Packet
 
 
 class Connection:
     host: str
@@ -37,89 +37,76 @@
             self.is_connected = False
             raise TimeoutError(f'Connection attempt to {self.host}:{self.port} timed out')
         except (socket.error, ConnectionResetError) as e:
             self.is_connected = False
             raise ConnectionError(f'Failed to connect to {self.host}:{self.port} ({e})')
 
     def write(self, packet: Packet) -> None:
-        logger.debug('Writing to socket')
         if not self.is_connected:
             logger.debug('Socket is not connected yet, connecting now')
             self.connect()
 
+        logger.debug('Writing to socket')
+
         try:
             self.sock.sendall(bytes(packet))
         except (socket.error, ConnectionResetError, RuntimeError) as e:
             raise ConnectionError(f'Failed to send data to server ({e})')
 
         logger.debug(packet)
 
     def read(self) -> Packet:
-        logger.debug('Reading from socket')
         if not self.is_connected:
             logger.debug('Socket is not connected yet, connecting now')
             self.connect()
 
-        # Init empty packet
-        packet = self.packet_type()
+        logger.debug('Reading from socket')
 
-        # Read header only first
-        logger.debug('Reading packet header')
+        packet = self.packet_type()
         last_received = time.time()
         timed_out = False
-        while len(packet.header) < HEADER_LENGTH and not timed_out:
-            iteration_buffer = self.read_safe(HEADER_LENGTH - len(packet.header))
-            packet.header += iteration_buffer
-
-            # Update timestamp if any data was retrieved during current iteration
-            if len(iteration_buffer) > 0:
-                last_received = time.time()
-            timed_out = time.time() > last_received + self.timeout
+        while (packet_buflen := packet.buflen()) > 0 and not timed_out:
+            iteration_buffer = self.read_safe(packet_buflen)
 
-        if timed_out:
-            raise TimeoutError('Timed out while reading packet header')
+            # Append whatever data is missing from the head to it
+            if (header_buflen := packet.header_buflen()) > 0:
+                packet.header += iteration_buffer.read(min(header_buflen, iteration_buffer.length))
+                # Log packet header once complete
+                if packet.header_buflen() == 0:
+                    logger.debug(f'Received header: {packet.header}')
 
-        logger.debug(packet.header)
+                    # Make sure packet header is valid (throws exception if invalid)
+                    packet.validate_header()
 
-        # Make sure packet header is valid (throws exception if invalid)
-        packet.validate_header()
-
-        # Read number of bytes indicated by packet header
-        logger.debug('Reading packet body')
-        last_received = time.time()
-        timed_out = False
-        while len(packet.body) < packet.indicated_body_length() and not timed_out:
-            iteration_buffer = self.read_safe(packet.indicated_body_length() - len(packet.body))
-            packet.body += iteration_buffer
+            # Append any remaining data to body
+            packet.body += iteration_buffer.get_buffer()
 
             # Update timestamp if any data was retrieved during current iteration
-            if len(iteration_buffer) > 0:
+            if iteration_buffer.length > 0:
                 last_received = time.time()
             timed_out = time.time() > last_received + self.timeout
 
-        logger.debug(packet.body)
-
         if timed_out:
-            raise TimeoutError('Timed out while reading packet body')
+            raise TimeoutError('Timed out while reading packet header')
+
+        logger.debug(f'Received body: {packet.body}')
 
         # Validate packet body (throws exception if invalid)
         packet.validate_body()
 
         return packet
 
-    def read_safe(self, buflen: int) -> bytes:
+    def read_safe(self, buflen: int) -> Buffer:
         try:
-            buffer = self.sock.recv(buflen)
+            return Buffer(self.sock.recv(buflen))
         except socket.timeout:
             raise TimeoutError('Timed out while receiving server data')
         except (socket.error, ConnectionResetError) as e:
             raise ConnectionError(f'Failed to receive data from server ({e})')
 
-        return buffer
-
     def init_socket(self) -> socket.socket:
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.settimeout(self.timeout)
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
 
         return sock
```

### Comparing `pybfbc2stats-0.3.8/pybfbc2stats/constants.py` & `pybfbc2stats-0.3.9/pybfbc2stats/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,38 @@
 class Platform(int, Enum):
     pc = 1
     # XBOX is not yet supported
     # xbox360 = 2
     ps3 = 3
 
 
+class TransmissionType(int, Enum):
+    pass
+
+
+class FeslTransmissionType(TransmissionType):
+    Ping = 1
+    SinglePacketResponse = 2
+    MultiPacketResponse = 3
+    SinglePacketRequest = 4
+    MultiPacketRequest = 5
+
+
+class TheaterTransmissionType(TransmissionType):
+    Request = 1
+    OKResponse = 2
+    ErrorResponse = 3
+
+
 DEFAULT_BUFFER_SIZE = 8096
 HEADER_LENGTH = 12
 HEADER_BYTE_ORDER = 'big'
 VALID_HEADER_TYPES_FESL = [b'acct', b'fsys', b'rank']
 VALID_HEADER_TYPES_THEATER = [b'CONN', b'USER', b'LLST', b'LDAT', b'GLST', b'GDAT', b'GDET', b'PDAT', b'PING']
-VALID_HEADER_ERROR_INDICATORS = [b'ngam', b'nrom']
+VALID_HEADER_ERROR_INDICATORS = [b'ngam', b'nrom', b'bpar', b'ntfn']
 BACKEND_DETAILS = {
     Platform.pc: {
         'host': 'bfbc2-pc-server.fesl.ea.com',
         'port': 18321,
         'clientString': b'bfbc2-pc'
     },
     Platform.ps3: {
```

### Comparing `pybfbc2stats-0.3.8/pybfbc2stats.egg-info/PKG-INFO` & `pybfbc2stats-0.3.9/pybfbc2stats.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: pybfbc2stats
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python library for retrieving statistics of Battlefield: Bad Company 2 players
 Home-page: https://github.com/cetteup/pybfbc2stats
 Author: cetteup
 Author-email: me@cetteup.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cetteup/pybfbc2stats/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # pybfbc2stats
 
 Python 🐍 library for retrieving statistics of Battlefield: Bad Company 2 players. Possible thanks to previous work by Luigi Auriemma and nemo.
 
+[![ci](https://img.shields.io/github/workflow/status/cetteup/pybfbc2stats/ci?label=ci)](https://github.com/cetteup/pybfbc2stats/actions?query=workflow%3Aci)
+[![License](https://img.shields.io/github/license/cetteup/pybfbc2stats)](/LICENSE)
+[![Package](https://img.shields.io/pypi/v/pybfbc2stats)](https://pypi.org/project/pybfbc2stats/)
+[![Last commit](https://img.shields.io/github/last-commit/cetteup/pybfbc2stats)](https://github.com/cetteup/pybfbc2stats/commits/main)
+
 ## Features
 
 - lookup players/personas by id or name on any platform
 - search for players/personas by name on any platform (with wildcard support)
 - retrieve all available statistics for players on PC/PS3
 - retrieve player leaderboards on PC/PS3
 - retrieve server list for PC/PS3
@@ -436,18 +441,40 @@
 
 Retrieve full details and player list for a given server.
 
 **Arguments**
 
   Argument     | Type | Opt/Required | Note
 ---------------|------|--------------|-----
-lobby_id       | int  | Required     | If of the game server lobby the server is hosted in
+lobby_id       | int  | Required     | Id of the game server lobby the server is hosted in
 game_id        | int  | Required     | Game (server) id
 
 **Example**
 
 ```python
 from pybfbc2stats import TheaterClient, Platform
 
 client = TheaterClient('bfbc2-ps3-server.theater.ea.com', 18336, 'your_lkey', Platform.ps3)
 general, detailed, players = client.get_server_details(257, 120018)
 ```
+
+----
+
+#### \[Async\]TheaterClient.get_current_server(user_id)
+
+Retrieve full details and player list for a given user's current server (server they are currently playing on, 
+raises a PlayerNotFound exception if the player is not currently playing online).
+
+**Arguments**
+
+  Argument     | Type | Opt/Required | Note
+---------------|------|--------------|-----
+user_id       | int  | Required     | Id of the user whose current server to get
+
+**Example**
+
+```python
+from pybfbc2stats import TheaterClient, Platform
+
+client = TheaterClient('bfbc2-ps3-server.theater.ea.com', 18336, 'your_lkey', Platform.ps3)
+general, detailed, players = client.get_current_server(227528903)
+```
```

### Comparing `pybfbc2stats-0.3.8/setup.cfg` & `pybfbc2stats-0.3.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybfbc2stats
-version = 0.3.8
+version = 0.3.9
 description = Python library for retrieving statistics of Battlefield: Bad Company 2 players
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cetteup/pybfbc2stats
 project_urls = 
 	Bug Tracker = https://github.com/cetteup/pybfbc2stats/issues
 author = cetteup
@@ -15,13 +15,13 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 
 [options]
 packages = pybfbc2stats
-python_requires = >=3.6
+python_requires = >=3.8
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

