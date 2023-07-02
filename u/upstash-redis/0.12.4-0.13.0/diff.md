# Comparing `tmp/upstash_redis-0.12.4.tar.gz` & `tmp/upstash_redis-0.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.12.4.tar", max compression
+gzip compressed data, was "upstash_redis-0.13.0.tar", max compression
```

## Comparing `upstash_redis-0.12.4.tar` & `upstash_redis-0.13.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis-0.12.4/LICENSE
--rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis-0.12.4/README.md
--rw-r--r--   0        0        0      434 2023-06-30 21:25:55.440375 upstash_redis-0.12.4/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-30 10:23:27.543198 upstash_redis-0.12.4/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-06-29 09:51:44.031185 upstash_redis-0.12.4/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     4603 2023-06-30 18:46:43.369679 upstash_redis-0.12.4/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     4790 2023-06-30 18:55:39.814269 upstash_redis-0.12.4/upstash_redis/client.py
--rw-r--r--   0        0        0       98 2023-06-29 09:49:58.469586 upstash_redis-0.12.4/upstash_redis/commands/__init__.py
--rw-r--r--   0        0        0      102 2023-06-30 14:20:06.203122 upstash_redis-0.12.4/upstash_redis/commands/async_commands.py
--rw-r--r--   0        0        0    22281 2023-06-30 14:06:30.500480 upstash_redis-0.12.4/upstash_redis/commands/async_commands.pyi
--rw-r--r--   0        0        0    71995 2023-06-30 17:28:46.668722 upstash_redis-0.12.4/upstash_redis/commands/commands.py
--rw-r--r--   0        0        0    21313 2023-06-30 14:14:41.609808 upstash_redis-0.12.4/upstash_redis/commands/commands.pyi
--rw-r--r--   0        0        0    83861 2023-06-30 14:05:28.406050 upstash_redis-0.12.4/upstash_redis/commands-old.py
--rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis-0.12.4/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis-0.12.4/upstash_redis/exception.py
--rw-r--r--   0        0        0      834 2023-06-22 15:12:55.454825 upstash_redis-0.12.4/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     5478 2023-06-30 18:56:49.908728 upstash_redis-0.12.4/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      431 2023-06-22 15:12:55.456040 upstash_redis-0.12.4/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0     1174 2023-06-22 15:12:55.456402 upstash_redis-0.12.4/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      752 2023-06-22 15:12:55.456727 upstash_redis-0.12.4/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis-0.12.4/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      172 2023-06-29 13:07:48.827924 upstash_redis-0.12.4/upstash_redis/typing.py
--rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis-0.12.4/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis-0.12.4/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-06-22 15:12:55.457479 upstash_redis-0.12.4/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     8827 2023-06-30 17:25:24.184093 upstash_redis-0.12.4/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9832 1970-01-01 00:00:00.000000 upstash_redis-0.12.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis-0.13.0/LICENSE
+-rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis-0.13.0/README.md
+-rw-r--r--   0        0        0      467 2023-07-02 09:22:06.079913 upstash_redis-0.13.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-30 10:23:27.543198 upstash_redis-0.13.0/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-29 09:51:44.031185 upstash_redis-0.13.0/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     4782 2023-07-01 22:51:26.915848 upstash_redis-0.13.0/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     4999 2023-07-01 22:51:14.000967 upstash_redis-0.13.0/upstash_redis/client.py
+-rw-r--r--   0        0        0       82 2023-07-01 09:47:03.295810 upstash_redis-0.13.0/upstash_redis/commands/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-01 09:47:03.278399 upstash_redis-0.13.0/upstash_redis/commands/async_commands.py
+-rw-r--r--   0        0        0    22111 2023-07-01 23:27:47.297643 upstash_redis-0.13.0/upstash_redis/commands/async_commands.pyi
+-rw-r--r--   0        0        0    71548 2023-07-01 23:27:46.350521 upstash_redis-0.13.0/upstash_redis/commands/commands.py
+-rw-r--r--   0        0        0    21221 2023-07-01 23:27:46.330353 upstash_redis-0.13.0/upstash_redis/commands/commands.pyi
+-rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis-0.13.0/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis-0.13.0/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-06-22 15:12:55.454825 upstash_redis-0.13.0/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     5478 2023-07-01 02:19:38.193972 upstash_redis-0.13.0/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0      431 2023-06-22 15:12:55.456040 upstash_redis-0.13.0/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0      738 2023-07-01 18:41:41.722004 upstash_redis-0.13.0/upstash_redis/schema/commands/returns.py
+-rw-r--r--   0        0        0      752 2023-06-22 15:12:55.456727 upstash_redis-0.13.0/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis-0.13.0/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      172 2023-07-01 02:24:32.912661 upstash_redis-0.13.0/upstash_redis/typing.py
+-rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis-0.13.0/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis-0.13.0/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-06-22 15:12:55.457479 upstash_redis-0.13.0/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     9368 2023-07-01 22:51:44.121000 upstash_redis-0.13.0/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9832 1970-01-01 00:00:00.000000 upstash_redis-0.13.0/PKG-INFO
```

### Comparing `upstash_redis-0.12.4/LICENSE` & `upstash_redis-0.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.4/README.md` & `upstash_redis-0.13.0/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.4/upstash_redis/asyncio/client.py` & `upstash_redis-0.13.0/upstash_redis/asyncio/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from os import environ
 from typing import Any, List, Type, Union
 
 from aiohttp import ClientSession
-from upstash_redis.commands.async_commands import AsyncBasicKeyCommands
+from upstash_redis.commands.async_commands import AsyncCommands
 from upstash_redis.config import REST_ENCODING, REST_RETRIES, REST_RETRY_INTERVAL, FORMAT_RETURN, ALLOW_TELEMETRY
 from upstash_redis.http.execute import async_execute
 
 from upstash_redis.schema.http import RESTEncoding, RESTResult
 from upstash_redis.schema.telemetry import TelemetryData
 from upstash_redis.utils.format import FormattedResponse
 
 
-class Redis(FormattedResponse, AsyncBasicKeyCommands):
+class Redis(FormattedResponse, AsyncCommands):
     
     def __init__(
         self,
         url: str,
         token: str,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
@@ -119,13 +119,13 @@
             telemetry_data=self.telemetry_data,
         )
 
         main_command = command[0]
         if len(command) > 1 and (main_command == "PUBSUB" or main_command == "SCRIPT"):
             main_command = f"{main_command} {command[1]}"
 
-        if self.format_return and (main_command in self.FORMATTERS) :
+        if (self.format_return or main_command == "HSCAN" or main_command == "SMEMBERS" or main_command == "SDIFF" or main_command == "SINTER" or main_command == "SSCAN" or main_command == "SUNION" or main_command == "ZSCAN") and (main_command in self.FORMATTERS):
             return self.FORMATTERS[main_command](res, command)
 
         return res
```

### Comparing `upstash_redis-0.12.4/upstash_redis/client.py` & `upstash_redis-0.13.0/upstash_redis/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from os import environ
 from typing import Any, List, Type, Union
 
 from aiohttp import ClientSession
-from upstash_redis.commands.commands import BasicKeyCommands
+from upstash_redis.commands.commands import Commands
 from upstash_redis.config import REST_ENCODING, REST_RETRIES, REST_RETRY_INTERVAL, FORMAT_RETURN, ALLOW_TELEMETRY
 from upstash_redis.http.execute import sync_execute
 
 from upstash_redis.schema.http import RESTEncoding, RESTResult
 from upstash_redis.schema.telemetry import TelemetryData
 from upstash_redis.utils.format import FormattedResponse
 from requests import Session
 
-class Redis(FormattedResponse, BasicKeyCommands):
+class Redis(FormattedResponse, Commands):
     
     def __init__(
         self,
         url: str,
         token: str,
         rest_encoding: RESTEncoding = REST_ENCODING,
         rest_retries: int = REST_RETRIES,
@@ -104,15 +104,16 @@
             telemetry_data,
         )
     
     def close(self):
         """
         Closes the session.
         """
-        self._session.close()
+        if self._session:
+            self._session.close()
 
     def run(self, command: List) -> RESTResult:
         """
         Specify the http options and execute the command.
         """
 
         res = sync_execute(
@@ -127,13 +128,13 @@
                     telemetry_data=self.telemetry_data,
         )
 
         main_command = command[0]
         if len(command) > 1 and (main_command == "PUBSUB"):
             main_command = f"{main_command} {command[1]}"
 
-        if self.format_return and (main_command in self.FORMATTERS) :
+        if (self.format_return or main_command == "HSCAN" or main_command == "SMEMBERS" or main_command == "SDIFF" or main_command == "SINTER" or main_command == "SSCAN" or main_command == "SUNION" or main_command == "ZSCAN") and (main_command in self.FORMATTERS):
             return self.FORMATTERS[main_command](res, command)
 
         return res
```

### Comparing `upstash_redis-0.12.4/upstash_redis/commands/async_commands.pyi` & `upstash_redis-0.13.0/upstash_redis/commands/async_commands.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 
 from upstash_redis.schema.commands.returns import (
     GeoMembersReturn,
     FormattedGeoMembersReturn,
-    HashReturn,
-    FormattedHashReturn,
-    SortedSetReturn,
-    FormattedSortedSetReturn,
 )
 
 from upstash_redis.schema.commands.parameters import (
     BitFieldOffset,
     GeoMember,
     FloatMinMax,
 )
 
-from typing import Any, Union, List, Literal, Dict
+from typing import Any, Iterable, Optional, Set, Tuple, Union, List, Literal, Dict
 
-class AsyncBasicKeyCommands:
+class AsyncCommands:
     def __init__(self):
         ...
 
     async def bitcount(
         self, key: str, start: Union[int, None] = None, end: Union[int, None] = None
     ) -> int: 
         ...
 
     def bitfield(self, key: str) -> "BitFieldCommands":
         ...
 
-    async def bitfield_ro(self, key: str) -> "BitFieldRO":
+    def bitfield_ro(self, key: str) -> "BitFieldRO":
         ...
 
     async def bitop(
         self, operation: Literal["AND", "OR", "XOR", "NOT"], destkey: str, *srckeys: str
     ) -> int:
         ...
 
@@ -258,15 +254,15 @@
 
     async def hexists(self, key: str, field: str) -> Union[Literal[1, 0], bool]:
         ...
 
     async def hget(self, key: str, field: str) -> Union[str, None]:
         ...
 
-    async def hgetall(self, key: str) -> Union[HashReturn, FormattedHashReturn]:
+    async def hgetall(self, key: str) -> Union[List[str], Dict[str, str]]:
         ...
 
     async def hincrby(self, key: str, field: str, increment: int) -> int:
         ...
 
     async def hincrbyfloat(
         self, key: str, field: str, increment: float
@@ -283,27 +279,27 @@
         ...
 
     async def hmset(self, key: str, field_value_pairs: Dict) -> str:
         ...
 
     async def hrandfield(
         self, key: str, count: Union[int, None] = None, withvalues: bool = False
-    ) -> Union[(Union[str, None]), Union[HashReturn, FormattedHashReturn]]:
+    ):
         ...
 
     async def hscan(
         self,
-        key: str,
+        name: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Union[List[Union[str, HashReturn]], List[Union[int, FormattedHashReturn]]]:
+    ) -> Tuple[int, Dict[str, str]]:
         ...
 
-    async def hset(self, key: str, field_value_pairs: Dict) -> int:
+    async def hset(self, name: str, key: Optional[str] = None, val: Optional[str] = None, field_value_pairs: Optional[Dict] = None) -> int:
         ...
 
     async def hsetnx(
         self, key: str, field: str, value: Any
     ) -> Union[Literal[1, 0], bool]:
         ...
 
@@ -322,27 +318,27 @@
     async def pfmerge(self, destkey: str, *sourcekeys: str) -> str:
         ...
 
     async def lindex(self, key: str, index: int) -> Union[str, None]:
         ...
 
     async def linsert(
-        self, key: str, position: Literal["BEFORE", "AFTER"], pivot: Any, element: Any
+        self, key: str, position: Literal["BEFORE", "AFTER", "before", "after"], pivot: Any, element: Any
     ) -> int:
        ...
 
     async def llen(self, key: str) -> int:
         ...
 
     async def lmove(
         self,
         source: str,
         destination: str,
-        source_position: Literal["LEFT", "RIGHT"],
-        destination_position: Literal["LEFT", "RIGHT"],
+        source_position: Literal["LEFT", "RIGHT"] = "LEFT",
+        destination_position: Literal["LEFT", "RIGHT"] = "RIGHT",
     ) -> Union[str, None]:
         ...
 
     async def lpop(
         self, key: str, count: Union[int, None] = None
     ) -> Union[(Union[str, None]), List[str]]:
         ...
@@ -407,45 +403,45 @@
         args: Union[List, None] = None,
     ) -> Any:
         ...
 
     async def dbsize(self) -> int:
         ...
 
-    async def flushall(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> str:
+    async def flushall(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> Union[str, bool]:
         ...
 
-    async def flushdb(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> str:
+    async def flushdb(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> Union[str, bool]:
         ...
 
     async def time(self) -> Union[List[str], Dict[str, int]]:
         ...
 
     async def sadd(self, key: str, *members: Any) -> int:
         ...
 
     async def scard(self, key: str) -> int:
         ...
 
-    async def sdiff(self, *keys: str) -> List[str]:
+    async def sdiff(self, *keys: str) -> Set[str]:
         ...
 
     async def sdiffstore(self, destination: str, *keys: str) -> int:
         ...
 
-    async def sinter(self, *keys: str) -> List[str]:
+    async def sinter(self, *keys: str) -> Set[str]:
         ...
 
     async def sinterstore(self, destination: str, *keys: str) -> int:
         ...
 
     async def sismember(self, key: str, member: Any) -> Union[Literal[1, 0], bool]:
         ...
 
-    async def smembers(self, key: str) -> List[str]:
+    async def smembers(self, key: str) -> Set[str]:
         ...
 
     async def smove(
         self, source: str, destination: str, member: Any
     ) -> Union[Literal[1, 0], bool]:
         ...
 
@@ -461,21 +457,21 @@
 
     async def srem(self, key: str, *members: Any) -> int:
         ...
 
     async def sscan(
         self,
         key: str,
-        cursor: int,
+        cursor: int = 0,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]:
+    ) -> Tuple[int, List[str]]:
         ...
 
-    async def sunion(self, *keys: str) -> List[str]:
+    async def sunion(self, *keys: str) -> Set[str]:
         ...
 
     async def sunionstore(self, destination: str, *keys: str) -> int:
         ...
 
     async def zadd(
         self,
@@ -494,79 +490,79 @@
         ...
 
     async def zcount(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
     ) -> int:
         ...
 
-    async def zdiff(
-        self, *keys: str, withscores: bool = False
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    def zdiff(
+        self, keys: List[str], withscores: bool = False
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
-    async def zdiffstore(self, destination: str, *keys: str) -> int:
+    async def zdiffstore(self, destination: str, keys: List[str]) -> int:
         ...
 
     async def zincrby(
         self, key: str, increment: float, member: str
     ) -> Union[str, float]:
         ...
 
     async def zinter(
         self,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     async def zinterstore(
         self,
         destination: str,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int:
         ...
 
     async def zlexcount(self, key: str, min_score: str, max_score: str) -> int:
         ...
 
     async def zmscore(
-        self, key: str, *members: str
+        self, key: str, members: List[str]
     ) -> Union[List[Union[str, None]], List[Union[float, None]]]:
         ...
 
     async def zpopmax(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     async def zpopmin(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     async def zrandmember(
         self, key: str, count: Union[int, None] = None, withscores: bool = False
-    ) -> Union[(Union[str, None]), (Union[SortedSetReturn, FormattedSortedSetReturn])]:
+    ) -> Union[(Union[str, None]), (Union[List[str], List[Tuple[str, float]]])]:
         ...
 
     async def zrange(
         self,
         key: str,
         start: FloatMinMax,
         stop: FloatMinMax,
         range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
         withscores: bool = False,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     async def zrangebylex(
         self,
         key: str,
         min_score: str,
         max_score: str,
@@ -577,25 +573,25 @@
 
     async def zrangebyscore(
         self,
         key: str,
         min_score: FloatMinMax,
         max_score: FloatMinMax,
         withscores: bool = False,
-        offset: Union[int, None] = None,
-        count: Union[int, None] = None,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     async def zrangestore(
         self,
         dst: str,
         src: str,
-        min_score: FloatMinMax,
-        max_score: FloatMinMax,
+        start: FloatMinMax,
+        stop: FloatMinMax,
         range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
     ) -> int:
         ...
 
@@ -614,67 +610,67 @@
     async def zremrangebyscore(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
     ) -> int:
         ...
 
     async def zrevrange(
         self, key: str, start: int, stop: int, withscores: bool = False
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     async def zrevrangebylex(
         self,
         key: str,
         max_score: str,
         min_score: str,
-        offset: Union[int, None] = None,
-        count: Union[int, None] = None,
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
     ) -> List[str]:
         ...
 
     async def zrevrangebyscore(
         self,
         key: str,
         max_score: FloatMinMax,
         min_score: FloatMinMax,
         withscores: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     async def zrevrank(self, key: str, member: str) -> Union[int, None]:
         ...
 
     async def zscan(
         self,
         key: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Union[List[Union[str, SortedSetReturn]],List[Union[int, FormattedSortedSetReturn]]]:
+    ) -> Tuple[int, List[Tuple[str, float]]]:
         ...
 
     async def zscore(self, key: str, member: str) -> Union[str, None, float]:
         ...
 
-    async def zunion(
+    def zunion(
         self,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     async def zunionstore(
         self,
         destination: str,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int:
         ...
 
     async def append(self, key: str, value: Any) -> int:
         ...
 
@@ -763,15 +759,15 @@
 
     def script(self) -> "Script":
         ...
 
 
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
-    def __init__(self, client: AsyncBasicKeyCommands, key: str):
+    def __init__(self, client: AsyncCommands, key: str):
         ...
 
     def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldCommands":
         ...
 
     def set(self, encoding: str, offset: BitFieldOffset, value: int) -> "BitFieldCommands":
         ...
@@ -783,26 +779,26 @@
         ...
 
     async def execute(self) -> List:
         ...
 
 
 class BitFieldRO:
-    def __init__(self, client: AsyncBasicKeyCommands, key: str):
+    def __init__(self, client: AsyncCommands, key: str):
         ...
 
     def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldRO":
         ...
 
     async def execute(self) -> List:
         ...
 
 
 class PubSub:
-    def __init__(self, client: AsyncBasicKeyCommands):
+    def __init__(self, client: AsyncCommands):
         ...
 
     async def channels(self, pattern: Union[str, None] = None) -> List[str]:
         ...
 
     async def numpat(self) -> int:
         ...
@@ -810,15 +806,15 @@
     async def numsub(
         self, *channels: str
     ) -> Union[List[Union[str, int]], Dict[str, int]]:
         ...
 
 
 class Script:
-    def __init__(self, client: AsyncBasicKeyCommands):
+    def __init__(self, client: AsyncCommands):
         ...
 
     async def exists(self, *sha1: str) -> Union[List[Literal[1, 0]], List[bool]]:
         ...
 
     async def flush(self, mode: Literal["ASYNC", "SYNC"]) -> str:
         ...
```

### Comparing `upstash_redis-0.12.4/upstash_redis/commands/commands.py` & `upstash_redis-0.13.0/upstash_redis/commands/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,19 @@
 )
 from upstash_redis.utils.comparison import number_are_not_none
 from upstash_redis.schema.commands.parameters import (
     BitFieldOffset,
     GeoMember,
     FloatMinMax,
 )
-from upstash_redis.schema.commands.returns import (
-    GeoMembersReturn,
-    FormattedGeoMembersReturn,
-    HashReturn,
-    FormattedHashReturn,
-    SortedSetReturn,
-    FormattedSortedSetReturn,
-)
-from aiohttp import ClientSession
-from typing import Type, Any, Literal, Union, List, Dict
-from os import environ
+
+from typing import Any, Iterable, Literal, Optional, Union, List, Dict
 
 
-class BasicKeyCommands(CommandsProtocol):
+class Commands(CommandsProtocol):
     def run(self, command):
         ...
 
     def bitcount(
         self, key: str, start: Union[int, None] = None, end: Union[int, None] = None
     ) -> ResponseType:
         """
@@ -295,16 +286,14 @@
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
         scan_type: Union[str, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/scan
 
-        :param return_cursor: if set to False, it won't return the cursor
-
         :param scan_type: replacement for "TYPE"
         :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
         Only the List of elements will be returned if "return_cursor" is False
         """
 
@@ -897,58 +886,60 @@
 
         if count is None and withvalues:
             raise Exception('"withvalues" can only be used together with "count"')
 
         command: List = ["HRANDFIELD", key]
 
         if count is not None:
-            command.extend(["COUNT", count])
+            command.extend([count])
 
             if withvalues:
                 command.append("WITHVALUES")
 
         return self.run(command)
 
     def hscan(
         self,
-        key: str,
+        name: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/hscan
 
-        :param return_cursor: if set to False, it won't return the cursor
         :param match_pattern: replacement for "MATCH"
-
-        :return: The cursor will be an integer if "format_return" is True.
-        Only a Dict of field-value pairs will be returned if "return_cursor" is False and "format_return" is True.
         """
 
-        command: List = ["HSCAN", key, cursor]
+        command: List = ["HSCAN", name, cursor]
 
         if match_pattern is not None:
             command.extend(["MATCH", match_pattern])
 
         if count is not None:
             command.extend(["COUNT", count])
 
         # The raw result is composed of the new cursor and the List of elements.
         return self.run(command)
 
-    def hset(self, key: str, field_value_pairs: Dict) -> ResponseType:
+    def hset(self, name: str, key: Optional[str] = None, val: Optional[str] = None, field_value_pairs: Optional[Dict] = None) -> ResponseType:
         """
         See https://redis.io/commands/hset
         """
+        command: List = ["HSET", name]
 
-        command: List = ["HSET", key]
+        if key is None and field_value_pairs is None:
+            raise Exception("'hset' with no key value pairs")
 
-        for field, value in field_value_pairs.items():
-            command.extend([field, value])
+        if key and val:
+            command.extend([key, val])
+
+        if field_value_pairs is not None:
+            for field, value in field_value_pairs.items():
+                command.extend([field, value])
 
         return self.run(command)
 
     def hsetnx(
         self, key: str, field: str, value: Any
     ) -> ResponseType:
         """
@@ -1017,15 +1008,15 @@
         """
 
         command: List = ["LINDEX", key, index]
 
         return self.run(command)
 
     def linsert(
-        self, key: str, position: Literal["BEFORE", "AFTER"], pivot: Any, element: Any
+        self, key: str, position: Literal["BEFORE", "AFTER", "before", "after"], pivot: Any, element: Any
     ) -> ResponseType:
         """
         See https://redis.io/commands/linsert
         """
 
         command: List = ["LINSERT", key, position, pivot, element]
 
@@ -1040,16 +1031,16 @@
 
         return self.run(command)
 
     def lmove(
         self,
         source: str,
         destination: str,
-        source_position: Literal["LEFT", "RIGHT"],
-        destination_position: Literal["LEFT", "RIGHT"],
+        source_position: Literal["LEFT", "RIGHT"] = "LEFT",
+        destination_position: Literal["LEFT", "RIGHT"] = "RIGHT",
     ) -> ResponseType:
         """
         See https://redis.io/commands/lmove
         """
 
         command: List = [
             "LMOVE",
@@ -1457,26 +1448,24 @@
         command: List = ["SREM", key, *members]
 
         return self.run(command)
 
     def sscan(
         self,
         key: str,
-        cursor: int,
+        cursor: int = 0,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/sscan
 
-        :param return_cursor: if set to False, it won't return the cursor
         :param match_pattern: replacement for "MATCH"
 
         :return: The cursor will be an integer if "format_return" is True.
-        Only the List of elements will be returned if "return_cursor" is False.
         """
 
         command: List = ["SSCAN", key, cursor]
 
         if match_pattern is not None:
             command.extend(["MATCH", match_pattern])
 
@@ -1591,15 +1580,15 @@
 
     """
     This has actually 3 return scenarios, but, 
     whether "with_scores" is True or not, its raw return type will be List[str].
     """
 
     def zdiff(
-        self, *keys: str, withscores: bool = False
+        self, keys: List[str], withscores: bool = False
     ) -> ResponseType:
         """
         See https://redis.io/commands/zdiff
 
         The number of keys is calculated automatically.
 
         :return: A Dict of member-score pairs if "with_scores" and "format_return" are True.
@@ -1611,15 +1600,15 @@
         command: List = ["ZDIFF", len(keys), *keys]
 
         if withscores:
             command.append("WITHSCORES")
 
         return self.run(command)
 
-    def zdiffstore(self, destination: str, *keys: str) -> ResponseType:
+    def zdiffstore(self, destination: str, keys: List[str]) -> ResponseType:
         """
         See https://redis.io/commands/zdiffstore
 
         The number of keys is calculated automatically.
         """
 
         if len(keys) == 0:
@@ -1645,16 +1634,16 @@
     """
     This has actually 3 return scenarios, but, 
     whether "with_scores" is True or not, its raw return type will be List[str].
     """
 
     def zinter(
         self,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
     ) -> ResponseType:
         """
         See https://redis.io/commands/zinter
 
         The number of keys is calculated automatically.
@@ -1677,16 +1666,16 @@
             command.append("WITHSCORES")
 
         return self.run(command)
 
     def zinterstore(
         self,
         destination: str,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/zinterstore
 
         The number of keys is calculated automatically.
         """
@@ -1720,15 +1709,15 @@
             )
 
         command: List = ["ZLEXCOUNT", key, min_score, max_score]
 
         return self.run(command)
 
     def zmscore(
-        self, key: str, *members: str
+        self, key: str, members: List[str]
     ) -> ResponseType:
         """
         See https://redis.io/commands/zmscore
 
         :return: A List of float or None values if "format_return" is True.
         """
 
@@ -1874,66 +1863,64 @@
 
     def zrangebyscore(
         self,
         key: str,
         min_score: FloatMinMax,
         max_score: FloatMinMax,
         withscores: bool = False,
-        offset: Union[int, None] = None,
-        count: Union[int, None] = None,
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/zrangebyscore
 
         If you need to use "-inf" and "+inf", please write them as strings.
 
         :param min_score: replacement for "MIN"
         :param max_score: replacement for "MAX"
 
         :return: A Dict of member-score pairs if "withscores" and "format_return" are True.
         """
 
-        if number_are_not_none(offset, count, number=1):
+        if number_are_not_none(limit_offset, limit_count, number=1):
             raise Exception('Both "offset" and "count" must be specified.')
 
         command: List = ["ZRANGEBYSCORE", key, min_score, max_score]
 
-        if offset is not None:
-            command.extend(["LIMIT", offset, count])
+        if limit_offset is not None:
+            command.extend(["LIMIT", limit_offset, limit_count])
 
         if withscores:
             command.append("WITHSCORES")
 
         return self.run(command)
 
     def zrangestore(
         self,
         dst: str,
         src: str,
-        min_score: FloatMinMax,
-        max_score: FloatMinMax,
+        start: FloatMinMax,
+        stop: FloatMinMax,
         range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/zrangestore
 
-        :param min_score: replacement for "MIN"
-        :param max_score: replacement for "MAX"
-
-        If you need to use "-inf" and "+inf", please write them as strings.
+        :param start: replacement for "MIN"
+        :param stop: replacement for "MAX"
         """
 
         handle_non_deprecated_zrange_exceptions(
-            range_method, min_score, max_score, limit_offset, limit_count
+            range_method, start, stop, limit_offset, limit_count
         )
 
-        command: List = ["ZRANGESTORE", dst, src, min_score, max_score]
+        command: List = ["ZRANGESTORE", dst, src, start, stop]
 
         if range_method:
             command.append(range_method)
 
         if rev:
             command.append("REV")
 
@@ -2029,30 +2016,30 @@
         return self.run(command)
 
     def zrevrangebylex(
         self,
         key: str,
         max_score: str,
         min_score: str,
-        offset: Union[int, None] = None,
-        count: Union[int, None] = None,
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/zrevrangebylex
 
         :param min_score: replacement for "MIN"
         :param max_score: replacement for "MAX"
         """
 
-        handle_zrangebylex_exceptions(min_score, max_score, offset, count)
+        handle_zrangebylex_exceptions(min_score, max_score, limit_offset, limit_count)
 
         command: List = ["ZREVRANGEBYLEX", key, max_score, min_score]
 
-        if offset is not None:
-            command.extend(["LIMIT", offset, count])
+        if limit_offset is not None:
+            command.extend(["LIMIT", limit_offset, limit_count])
 
         return self.run(command)
 
     """
     This has actually 3 return scenarios, but,
     whether "withscores" is True or not, its raw return type will be List[str].
     """
@@ -2106,17 +2093,14 @@
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/zscan
 
         :param match_pattern: replacement for "MATCH"
-
-        :return: The cursor will be an integer if "format_return" is True.
-        Only a Dict of member-score pairs will be returned if "return_cursor" is False and "format_return" is True.
         """
 
         command: List = ["ZSCAN", key, cursor]
 
         if match_pattern is not None:
             command.extend(["MATCH", match_pattern])
 
@@ -2140,16 +2124,16 @@
     """
     This has actually 3 return scenarios, but,
     whether "withscores" is True or not, its raw return type will be List[str].
     """
 
     def zunion(
         self,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
     ) -> ResponseType:
         """
         See https://redis.io/commands/zunion
 
         The number of keys is calculated automatically.
@@ -2172,16 +2156,16 @@
             command.append("WITHSCORES")
 
         return self.run(command)
 
     def zunionstore(
         self,
         destination: str,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/zunionstore
 
         The number of keys is calculated automatically.
         """
@@ -2253,15 +2237,15 @@
         pxat: Union[int, None] = None,
         persist: Union[bool, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/getex
         """
 
-        if not number_are_not_none(ex, px, exat, pxat, persist, number=1):
+        if (ex or px or exat or pxat or persist) and not number_are_not_none(ex, px, exat, pxat, persist, number=1):
             raise Exception("Exactly one of the expiration settings must be specified.")
 
         command: List = ["GETEX", key]
 
         if ex is not None:
             command.extend(["EX", ex])
 
@@ -2371,31 +2355,31 @@
 
         return self.run(command)
 
     def set(
         self,
         key: str,
         value: Any,
-        nx: bool = False,
-        xx: bool = False,
-        get: bool = False,
+        nx: Union[bool, None] = None,
+        xx: Union[bool, None] = None,
+        get: Union[bool, None] = None,
         ex: Union[int, None] = None,
         px: Union[int, None] = None,
         exat: Union[int, None] = None,
         pxat: Union[int, None] = None,
-        keepttl: bool = False,
+        keepttl: Union[bool, None] = None,
     ) -> ResponseType:
         """
         See https://redis.io/commands/set
         """
 
         if nx and xx:
             raise Exception('"nx" and "xx" are mutually exclusive.')
 
-        if not number_are_not_none(ex, px, exat, pxat, keepttl, number=1):
+        if (ex or px or exat or pxat or keepttl) and not number_are_not_none(ex, px, exat, pxat, keepttl, number=1):
             raise Exception("Exactly one of the expiration settings must be specified.")
 
         if nx and get:
             raise Exception('"nx" and "get" are mutually exclusive.')
 
         command: List = ["SET", key, value]
 
@@ -2483,15 +2467,15 @@
         """
 
         return Script(client=self)
 
 
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
-    def __init__(self, client: BasicKeyCommands, key: str):
+    def __init__(self, client: Commands, key: str):
         self.client = client
         self.command: List = ["BITFIELD", key]
 
     def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldCommands":
         """
         Returns the specified bit field.
 
@@ -2545,15 +2529,15 @@
         return self
 
     def execute(self) -> ResponseType:
         return self.client.run(command=self.command)
 
 
 class BitFieldRO:
-    def __init__(self, client: BasicKeyCommands, key: str):
+    def __init__(self, client: Commands, key: str):
         self.client = client
         self.command: List = ["BITFIELD_RO", key]
 
     def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldRO":
         """
         Returns the specified bit field.
 
@@ -2566,15 +2550,15 @@
         return self
 
     def execute(self) -> ResponseType:
         return self.client.run(command=self.command)
 
 
 class PubSub:
-    def __init__(self, client: BasicKeyCommands):
+    def __init__(self, client: Commands):
         self.client = client
 
     def channels(self, pattern: Union[str, None] = None) -> ResponseType:
         """
         See https://redis.io/commands/pubsub-channels
         """
 
@@ -2604,15 +2588,15 @@
         """
 
         command: List = ["PUBSUB", "NUMSUB", *channels]
 
         return self.client.run(command)
 
 class Script:
-    def __init__(self, client: BasicKeyCommands):
+    def __init__(self, client: Commands):
         self.client = client
 
     def exists(self, *sha1: str) -> ResponseType:
         """
         See https://redis.io/commands/script-exists
 
         :return: A List of bools if "format_return" is True.
```

### Comparing `upstash_redis-0.12.4/upstash_redis/commands/commands.pyi` & `upstash_redis-0.13.0/upstash_redis/commands/commands.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 
 from upstash_redis.schema.commands.returns import (
     GeoMembersReturn,
     FormattedGeoMembersReturn,
-    HashReturn,
-    FormattedHashReturn,
-    SortedSetReturn,
-    FormattedSortedSetReturn,
 )
 
 from upstash_redis.schema.commands.parameters import (
     BitFieldOffset,
     GeoMember,
     FloatMinMax,
 )
 
-from typing import Any, Union, List, Awaitable, Literal, Dict
+from typing import Any, Iterable, Optional, Set, Tuple, Union, List, Literal, Dict
 
-class BasicKeyCommands:
+class Commands:
     def bitcount(
         self, key: str, start: Union[int, None] = None, end: Union[int, None] = None
     ) -> int: 
         ...
 
     def bitfield(self, key: str) -> "BitFieldCommands":
         ...
@@ -255,15 +251,15 @@
 
     def hexists(self, key: str, field: str) -> Union[Literal[1, 0], bool]:
         ...
 
     def hget(self, key: str, field: str) -> Union[str, None]:
         ...
 
-    def hgetall(self, key: str) -> Union[HashReturn, FormattedHashReturn]:
+    def hgetall(self, key: str) -> Union[List[str], Dict[str, str]]:
         ...
 
     def hincrby(self, key: str, field: str, increment: int) -> int:
         ...
 
     def hincrbyfloat(
         self, key: str, field: str, increment: float
@@ -280,27 +276,27 @@
         ...
 
     def hmset(self, key: str, field_value_pairs: Dict) -> str:
         ...
 
     def hrandfield(
         self, key: str, count: Union[int, None] = None, withvalues: bool = False
-    ) -> Union[(Union[str, None]), Union[HashReturn, FormattedHashReturn]]:
+    ):
         ...
 
     def hscan(
         self,
-        key: str,
+        name: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Union[List[Union[str, HashReturn]], List[Union[int, FormattedHashReturn]]]:
+    ) -> Tuple[int, Dict[str, str]]:
         ...
 
-    def hset(self, key: str, field_value_pairs: Dict) -> int:
+    def hset(self, name: str, key: Optional[str] = None, val: Optional[str] = None, field_value_pairs: Optional[Dict] = None) -> int:
         ...
 
     def hsetnx(
         self, key: str, field: str, value: Any
     ) -> Union[Literal[1, 0], bool]:
         ...
 
@@ -319,27 +315,27 @@
     def pfmerge(self, destkey: str, *sourcekeys: str) -> str:
         ...
 
     def lindex(self, key: str, index: int) -> Union[str, None]:
         ...
 
     def linsert(
-        self, key: str, position: Literal["BEFORE", "AFTER"], pivot: Any, element: Any
+        self, key: str, position: Literal["BEFORE", "AFTER", "before", "after"], pivot: Any, element: Any
     ) -> int:
        ...
 
     def llen(self, key: str) -> int:
         ...
 
     def lmove(
         self,
         source: str,
         destination: str,
-        source_position: Literal["LEFT", "RIGHT"],
-        destination_position: Literal["LEFT", "RIGHT"],
+        source_position: Literal["LEFT", "RIGHT"] = "LEFT",
+        destination_position: Literal["LEFT", "RIGHT"] = "RIGHT",
     ) -> Union[str, None]:
         ...
 
     def lpop(
         self, key: str, count: Union[int, None] = None
     ) -> Union[(Union[str, None]), List[str]]:
         ...
@@ -404,45 +400,45 @@
         args: Union[List, None] = None,
     ) -> Any:
         ...
 
     def dbsize(self) -> int:
         ...
 
-    def flushall(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> str:
+    def flushall(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> Union[str, bool]:
         ...
 
-    def flushdb(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> str:
+    def flushdb(self, mode: Union[Literal["ASYNC", "SYNC"], None] = None) -> Union[str, bool]:
         ...
 
     def time(self) -> Union[List[str], Dict[str, int]]:
         ...
 
     def sadd(self, key: str, *members: Any) -> int:
         ...
 
     def scard(self, key: str) -> int:
         ...
 
-    def sdiff(self, *keys: str) -> List[str]:
+    def sdiff(self, *keys: str) -> Set[str]:
         ...
 
     def sdiffstore(self, destination: str, *keys: str) -> int:
         ...
 
-    def sinter(self, *keys: str) -> List[str]:
+    def sinter(self, *keys: str) -> Set[str]:
         ...
 
     def sinterstore(self, destination: str, *keys: str) -> int:
         ...
 
     def sismember(self, key: str, member: Any) -> Union[Literal[1, 0], bool]:
         ...
 
-    def smembers(self, key: str) -> List[str]:
+    def smembers(self, key: str) -> Set[str]:
         ...
 
     def smove(
         self, source: str, destination: str, member: Any
     ) -> Union[Literal[1, 0], bool]:
         ...
 
@@ -458,21 +454,21 @@
 
     def srem(self, key: str, *members: Any) -> int:
         ...
 
     def sscan(
         self,
         key: str,
-        cursor: int,
+        cursor: int = 0,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Union[List[Union[str, List[str]]], List[Union[int, List[str]]]]:
+    ) -> Tuple[int, List[str]]:
         ...
 
-    def sunion(self, *keys: str) -> List[str]:
+    def sunion(self, *keys: str) -> Set[str]:
         ...
 
     def sunionstore(self, destination: str, *keys: str) -> int:
         ...
 
     def zadd(
         self,
@@ -492,78 +488,78 @@
 
     def zcount(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
     ) -> int:
         ...
 
     def zdiff(
-        self, *keys: str, withscores: bool = False
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+        self, keys: List[str], withscores: bool = False
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
-    def zdiffstore(self, destination: str, *keys: str) -> int:
+    def zdiffstore(self, destination: str, keys: List[str]) -> int:
         ...
 
     def zincrby(
         self, key: str, increment: float, member: str
     ) -> Union[str, float]:
         ...
 
     def zinter(
         self,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     def zinterstore(
         self,
         destination: str,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int:
         ...
 
     def zlexcount(self, key: str, min_score: str, max_score: str) -> int:
         ...
 
     def zmscore(
-        self, key: str, *members: str
+        self, key: str, members: List[str]
     ) -> Union[List[Union[str, None]], List[Union[float, None]]]:
         ...
 
     def zpopmax(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     def zpopmin(
         self, key: str, count: Union[int, None] = None
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     def zrandmember(
         self, key: str, count: Union[int, None] = None, withscores: bool = False
-    ) -> Union[(Union[str, None]), (Union[SortedSetReturn, FormattedSortedSetReturn])]:
+    ) -> Union[(Union[str, None]), (Union[List[str], List[Tuple[str, float]]])]:
         ...
 
     def zrange(
         self,
         key: str,
         start: FloatMinMax,
         stop: FloatMinMax,
         range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
         withscores: bool = False,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     def zrangebylex(
         self,
         key: str,
         min_score: str,
         max_score: str,
@@ -574,25 +570,25 @@
 
     def zrangebyscore(
         self,
         key: str,
         min_score: FloatMinMax,
         max_score: FloatMinMax,
         withscores: bool = False,
-        offset: Union[int, None] = None,
-        count: Union[int, None] = None,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     def zrangestore(
         self,
         dst: str,
         src: str,
-        min_score: FloatMinMax,
-        max_score: FloatMinMax,
+        start: FloatMinMax,
+        stop: FloatMinMax,
         range_method: Union[Literal["BYSCORE", "BYLEX"], None] = None,
         rev: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
     ) -> int:
         ...
 
@@ -611,67 +607,67 @@
     def zremrangebyscore(
         self, key: str, min_score: FloatMinMax, max_score: FloatMinMax
     ) -> int:
         ...
 
     def zrevrange(
         self, key: str, start: int, stop: int, withscores: bool = False
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     def zrevrangebylex(
         self,
         key: str,
         max_score: str,
         min_score: str,
-        offset: Union[int, None] = None,
-        count: Union[int, None] = None,
+        limit_offset: Union[int, None] = None,
+        limit_count: Union[int, None] = None,
     ) -> List[str]:
         ...
 
     def zrevrangebyscore(
         self,
         key: str,
         max_score: FloatMinMax,
         min_score: FloatMinMax,
         withscores: bool = False,
         limit_offset: Union[int, None] = None,
         limit_count: Union[int, None] = None,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     def zrevrank(self, key: str, member: str) -> Union[int, None]:
         ...
 
     def zscan(
         self,
         key: str,
         cursor: int,
         match_pattern: Union[str, None] = None,
         count: Union[int, None] = None,
-    ) -> Union[List[Union[str, SortedSetReturn]],List[Union[int, FormattedSortedSetReturn]]]:
+    ) -> Tuple[int, List[Tuple[str, float]]]:
         ...
 
     def zscore(self, key: str, member: str) -> Union[str, None, float]:
         ...
 
     def zunion(
         self,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
         withscores: bool = False,
-    ) -> Union[SortedSetReturn, FormattedSortedSetReturn]:
+    ) -> Union[List[str], List[Tuple[str, float]]]:
         ...
 
     def zunionstore(
         self,
         destination: str,
-        *keys: str,
-        weights: Union[List[float], None] = None,
+        keys: List[str],
+        weights: Union[List[float], List[int], None] = None,
         aggregate: Union[Literal["SUM", "MIN", "MAX"], None] = None,
     ) -> int:
         ...
 
     def append(self, key: str, value: Any) -> int:
         ...
 
@@ -759,15 +755,15 @@
         ...
 
     def script(self) -> "Script":
         ...
 
 # It doesn't inherit from "Redis" mainly because of the methods signatures.
 class BitFieldCommands:
-    def __init__(self, client: BasicKeyCommands, key: str):
+    def __init__(self, client: Commands, key: str):
         ...
 
     def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldCommands":
         ...
 
     def set(self, encoding: str, offset: BitFieldOffset, value: int) -> "BitFieldCommands":
         ...
@@ -779,26 +775,26 @@
         ...
 
     def execute(self) -> List:
         ...
 
 
 class BitFieldRO:
-    def __init__(self, client: BasicKeyCommands, key: str):
+    def __init__(self, client: Commands, key: str):
         ...
 
     def get(self, encoding: str, offset: BitFieldOffset) -> "BitFieldRO":
         ...
 
     def execute(self) -> List:
         ...
 
 
 class PubSub:
-    def __init__(self, client: BasicKeyCommands):
+    def __init__(self, client: Commands):
         ...
 
     def channels(self, pattern: Union[str, None] = None) -> List[str]:
         ...
 
     def numpat(self) -> int:
         ...
@@ -806,18 +802,21 @@
     def numsub(
         self, *channels: str
     ) -> Union[List[Union[str, int]], Dict[str, int]]:
         ...
 
 
 class Script:
-    def __init__(self, client: BasicKeyCommands):
+    def __init__(self, client: Commands):
         ...
 
     def exists(self, *sha1: str) -> Union[List[Literal[1, 0]], List[bool]]:
         ...
 
     def flush(self, mode: Literal["ASYNC", "SYNC"]) -> str:
         ...
 
     def load(self, script: str) -> str:
-        ...
+        ...
+
+
+# TODO: make sure all the relevant sorted set commands return tuples
```

### Comparing `upstash_redis-0.12.4/upstash_redis/http/decode.py` & `upstash_redis-0.13.0/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.4/upstash_redis/http/execute.py` & `upstash_redis-0.13.0/upstash_redis/http/execute.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.4/upstash_redis/schema/http.py` & `upstash_redis-0.13.0/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.4/upstash_redis/utils/exception.py` & `upstash_redis-0.13.0/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.12.4/upstash_redis/utils/format.py` & `upstash_redis-0.13.0/upstash_redis/utils/format.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from upstash_redis.schema.commands.returns import (
     GeoMembersReturn,
     FormattedGeoMembersReturn,
-    HashReturn,
-    FormattedHashReturn,
-    SortedSetReturn,
-    FormattedSortedSetReturn,
 )
-from typing import Literal, Union, List, Dict
+from typing import Literal, Tuple, Union, List, Dict
 
 
 def _list_to_dict(raw: List, command=None) -> Dict:
     """
     Convert a list that contains ungrouped pairs as consecutive elements (usually field-value or similar) into a dict.
     """
 
@@ -87,15 +83,15 @@
             formatted_member["latitude"] = float(member[1][1])
 
         result.append(formatted_member)
 
     return result
 
 
-def format_hash_return(raw: HashReturn) -> FormattedHashReturn:
+def format_hash_return(raw: List[str], command = None) -> Dict[str, str]:
     """
     Format the raw output given by Hash commands, usually the ones that return the field-value
     pairs of Hashes.
     """
 
     return _list_to_dict(raw=raw)
 
@@ -112,40 +108,46 @@
     """
     Format a list of boolean integers.
     """
 
     return [bool(value) for value in raw]
 
 
-def format_server_time_return(raw: List[str]) -> Dict[str, int]:
+def format_server_time_return(raw: List[str], command=None) -> Dict[str, int]:
     """
     Format the raw output returned by "TIME".
     """
 
     return {"seconds": int(raw[0]), "microseconds": int(raw[1])}
 
 
-def format_sorted_set_return(raw: SortedSetReturn) -> FormattedSortedSetReturn:
+def format_sorted_set_return(raw: List[str], command=None) -> list[Tuple[str, float]]:
     """
     Format the raw output given by Sorted Set commands, usually the ones that return the member-score
     pairs of Sorted Sets.
     """
-
-    return _list_to_dict(raw=raw)
+    it = iter(raw)
+    return list(zip(it, map(float, it)))
 
 
-def format_float_list(raw: List[Union[str, None]]) -> List[Union[float, None]]:
+def format_float_list(raw: List[Union[str, None]], command=None) -> List[Union[float, None]]:
     """
     Format a list of strings representing floats or None values.
     """
 
     return [float(value) if value is not None else None for value in raw]
 
 
 
+def to_set(res, command):
+    return set(res)
+
+def ok_to_bool(res, command):
+    return res == "OK"
+
 def to_bool(res, command):
     return bool(res)
 
 def to_float(res, command):
     return float(res)
 
 def scan_formatter(res, command):
@@ -255,15 +257,15 @@
         "GEODIST": to_float,
         "GEOPOS": format_geo_positions_return,
         "GEORADIUS": georadius_formatter,
         "GEORADIUS_RO": georadius_formatter, # same with the georadius, missing tests
         "GEORADIUSBYMEMBER": georadius_formatter, # same with the georadius, missing tests
         "GEORADIUSBYMEMBER_RO": georadius_formatter, # same with the georadius, missing tests
         "GEOSEARCH": georadius_formatter, # same with the georadius, missing tests
-        "HEXIST": to_bool, # missing test
+        "HEXISTS": to_bool, # missing test
         "HGETALL": format_hash_return, # missing test
         "HINCRBYFLOAT": to_float, # missing test
         "HRANDFIELD": hrandfield_formatter, # missing test
         "HSCAN": hscan_formatter, # missing test
         "HSETNX": to_bool, # missing test
         "PFADD": to_bool,
         "TIME": format_server_time_return, # missing test
@@ -285,11 +287,26 @@
         "ZSCAN": zscan_formatter, # missing test
         "ZSCORE": zscore_formatter, # missing test
         "ZUNION": zunion_formatter, # missing test
         "INCRBYFLOAT": to_float, # missing test
         "PUBSUB NUMSUB": _list_to_dict,
         "SCRIPT EXISTS": format_bool_list, # missing test
 
+        "FLUSHALL": ok_to_bool,
+        "FLUSHDB": ok_to_bool,
+        "MSETNX": to_bool,
+        "PSETEX": ok_to_bool,
+        "SET": ok_to_bool,
+        "SETEX": ok_to_bool,
+        "SETNX": to_bool,
+        "HMSET": ok_to_bool,
+
+        "SMEMBERS": to_set,
+        "SDIFF": to_set,
+        "SINTER": to_set,
+        "SUNION": to_set,
     }
 
     # TODO: Check return_cursor stuff.
-    # TODO: lots of duplicate formatters. unite them
+    # TODO: lots of duplicate formatters. unite them
+    # TODO: all formatters should take `command` parameter
+    # TODO: check commands using format_sorted_set_return
```

### Comparing `upstash_redis-0.12.4/PKG-INFO` & `upstash_redis-0.13.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 0.12.4
+Version: 0.13.0
 Summary: 
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

