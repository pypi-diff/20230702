# Comparing `tmp/upstash_ratelimit-0.3.0.tar.gz` & `tmp/upstash_ratelimit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit-0.3.0.tar", max compression
+gzip compressed data, was "upstash_ratelimit-0.3.1.tar", max compression
```

## Comparing `upstash_ratelimit-0.3.0.tar` & `upstash_ratelimit-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-05-24 13:49:29.501847 upstash_ratelimit-0.3.0/LICENSE
--rw-r--r--   0        0        0    11067 2023-06-21 06:26:04.086481 upstash_ratelimit-0.3.0/README.md
--rw-r--r--   0        0        0      398 2023-07-01 01:38:59.014707 upstash_ratelimit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-06-30 22:13:44.524574 upstash_ratelimit-0.3.0/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0     1828 2023-07-01 00:54:30.139483 upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/algorithm.py
--rw-r--r--   0        0        0     3243 2023-07-01 00:40:41.395386 upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/fixed_window_core.py
--rw-r--r--   0        0        0     5777 2023-07-01 00:17:49.801642 upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/sliding_window_core.py
--rw-r--r--   0        0        0     5231 2023-07-01 00:17:45.426985 upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/token_bucket_core.py
--rw-r--r--   0        0        0       86 2023-07-01 00:19:13.681310 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/__init__.py
--rw-r--r--   0        0        0     1161 2023-07-01 01:02:11.086857 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/async_blocker.py
--rw-r--r--   0        0        0     2981 2023-07-01 01:17:19.839016 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/fixed_window.py
--rw-r--r--   0        0        0     3506 2023-07-01 01:06:06.660882 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/limiter.py
--rw-r--r--   0        0        0     3788 2023-07-01 01:03:13.817815 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/sliding_window.py
--rw-r--r--   0        0        0     3399 2023-07-01 01:06:25.788183 upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/token_bucket.py
--rw-r--r--   0        0        0      167 2023-05-24 13:49:29.504075 upstash_ratelimit-0.3.0/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     3489 2023-07-01 01:05:05.419552 upstash_ratelimit-0.3.0/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-05-24 13:49:29.504232 upstash_ratelimit-0.3.0/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      475 2023-06-21 04:18:16.326882 upstash_ratelimit-0.3.0/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0     2824 2023-07-01 01:01:07.547407 upstash_ratelimit-0.3.0/upstash_ratelimit/sync/fixed_window.py
--rw-r--r--   0        0        0     3477 2023-07-01 01:01:01.211066 upstash_ratelimit-0.3.0/upstash_ratelimit/sync/sliding_window.py
--rw-r--r--   0        0        0     1111 2023-07-01 01:00:30.604276 upstash_ratelimit-0.3.0/upstash_ratelimit/sync/sync_blocker.py
--rw-r--r--   0        0        0     3185 2023-07-01 01:01:11.877570 upstash_ratelimit-0.3.0/upstash_ratelimit/sync/token_bucket.py
--rw-r--r--   0        0        0      392 2023-06-21 04:18:16.327167 upstash_ratelimit-0.3.0/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0    11656 1970-01-01 00:00:00.000000 upstash_ratelimit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-02 12:21:59.482998 upstash_ratelimit-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7542 2023-07-02 12:21:59.482998 upstash_ratelimit-0.3.1/README.md
+-rw-r--r--   0        0        0      475 2023-07-02 12:21:59.482998 upstash_ratelimit-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/algorithms/algorithm.py
+-rw-r--r--   0        0        0     3243 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/algorithms/fixed_window_core.py
+-rw-r--r--   0        0        0     5777 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/algorithms/sliding_window_core.py
+-rw-r--r--   0        0        0     5231 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/algorithms/token_bucket_core.py
+-rw-r--r--   0        0        0       86 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/async_blocker.py
+-rw-r--r--   0        0        0     2981 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/fixed_window.py
+-rw-r--r--   0        0        0     3506 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/limiter.py
+-rw-r--r--   0        0        0     3788 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/sliding_window.py
+-rw-r--r--   0        0        0     3399 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/token_bucket.py
+-rw-r--r--   0        0        0      172 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     3489 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      475 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0     2824 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/sync/fixed_window.py
+-rw-r--r--   0        0        0     3477 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/sync/sliding_window.py
+-rw-r--r--   0        0        0     1111 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/sync/sync_blocker.py
+-rw-r--r--   0        0        0     3185 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/sync/token_bucket.py
+-rw-r--r--   0        0        0      392 2023-07-02 12:21:59.486998 upstash_ratelimit-0.3.1/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0     8175 1970-01-01 00:00:00.000000 upstash_ratelimit-0.3.1/PKG-INFO
```

### Comparing `upstash_ratelimit-0.3.0/LICENSE` & `upstash_ratelimit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/algorithm.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/algorithms/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from upstash_redis.schema.telemetry import TelemetryData
 from upstash_ratelimit.config import SDK, PREFIX
 from upstash_ratelimit.schema.response import RateLimitResponse
 from asyncio import sleep
 from time import time_ns
 
 
+# TODO might delete this
 class RateLimitAlgorithm(ABC):
     @abstractmethod
     def __init__(self, prefix: str = PREFIX):
         """
         :param redis: the Redis client that will be used to execute the algorithm's commands. If not given, will read from env variables `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN`
         :param prefix: a prefix to distinguish between the keys used for rate limiting and others
         """
```

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/fixed_window_core.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/algorithms/fixed_window_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/sliding_window_core.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/algorithms/sliding_window_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/algorithms/token_bucket_core.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/algorithms/token_bucket_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/async_blocker.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/async_blocker.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/fixed_window.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/fixed_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/limiter.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/sliding_window.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/sliding_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/asyncio/token_bucket.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/asyncio/token_bucket.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/limiter.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/sync/fixed_window.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/sync/fixed_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/sync/sliding_window.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/sync/sliding_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/sync/sync_blocker.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/sync/sync_blocker.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/upstash_ratelimit/sync/token_bucket.py` & `upstash_ratelimit-0.3.1/upstash_ratelimit/sync/token_bucket.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.0/PKG-INFO` & `upstash_ratelimit-0.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,164 +1,146 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit
-Version: 0.3.0
-Summary: 
+Version: 0.3.1
+Summary: Serverless ratelimiting package from Upstash
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
-Requires-Dist: upstash-redis (>=0.12.4,<0.13.0)
+Requires-Dist: upstash-redis (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # Upstash Rate Limit - python edition
 
 upstash-ratelimit is a connectionless rate limiting library for python, designed to be used in serverless environments such as:
 - AWS Lambda
+- Vercel Serverless
 - Google Cloud Functions
 - and other environments where HTTP is preferred over TCP.
 
 The sdk is currently compatible with python 3.10 and above.
 
 <!-- toc -->
-
+- [Upstash Rate Limit - python edition](#upstash-rate-limit---python-edition)
 - [Quick Start](#quick-start)
   - [Install](#install)
     - [PyPi](#pypi)
   - [Setup database client](#setup-database-client)
-  - [Usage](#usage)
-  - [Telemetry](#telemetry)
+  - [Ratelimit](#ratelimit)
+    - [Importing Options](#importing-options)
+    - [Usage](#usage)
   - [Block until ready](#block-until-ready)
-  - [Timeout](#timeout)
   - [Rate-limiting outbound requests](#rate-limiting-outbound-requests)
 - [Ratelimiting algorithms](#ratelimiting-algorithms)
   - [Fixed Window](#fixed-window)
-    - [Pros:](#pros)
-    - [Cons:](#cons)
-    - [Usage:](#usage)
+    - [Pros](#pros)
+    - [Cons](#cons)
+    - [Usage](#usage-1)
   - [Sliding Window](#sliding-window)
-    - [Pros:](#pros-1)
-    - [Cons:](#cons-1)
-    - [Usage:](#usage-1)
+    - [Pros](#pros-1)
+    - [Cons](#cons-1)
+    - [Usage](#usage-2)
   - [Token Bucket](#token-bucket)
-    - [Pros:](#pros-2)
-    - [Cons:](#cons-2)
-    - [Usage:](#usage-2)
+    - [Pros](#pros-2)
+    - [Cons](#cons-2)
+    - [Usage](#usage-3)
 - [Contributing](#contributing)
   - [Preparing the environment](#preparing-the-environment)
-  - [Adding new algorithms](#adding-new-algorithms)
   - [Running tests](#running-tests)
-  - [Releasing](#releasing)
 
 <!-- tocstop -->
 
 # Quick Start
 
 ## Install
 
 ### PyPi
 
 ```bash
 pip install upstash-ratelimit
 ```
 
-If you are using a packaging and dependency management tool like [Poetry](https://python-poetry.org), you might want to check
-the respective docs in regard to adding a dependency. For example, in a Poetry-managed virtual environment, you can use:
-
-```bash
-poetry add upstash-ratelimit
-```
-
 ## Setup database client
-To be able to use upstash-ratelimit, you need to create a database on [Upstash](https://console.upstash.com/) and instantiate
-a client with the serverless driver:
-
-```python
-from upstash_redis.client import Redis
-
-redis = Redis(url="UPSTASH_REDIS_REST_URL", token="UPSTASH_REDIS_REST_TOKEN")
-```
-
-Or, if you want to automatically load the credentials from the environment:
-
-```python
-from upstash_redis.client import Redis
-
-redis = Redis.from_env()
-```
-
-The constructor can take even more optional parameters, some of them being (types expanded):
-
-```python
-url: str
-
-token: str
-
-rest_encoding: Literal["base64"] | Literal[False] = "base64"
-
-rest_retries: int = 1
-
-rest_retry_interval: int = 3 # In seconds.
-
-allow_deprecated: bool = False
+To be able to use upstash-ratelimit, you need to create a database on [Upstash](https://console.upstash.com/) and get `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN` environment variables.
 
-format_return: bool = True
+## Ratelimit
+### Importing Options
+- #### Directly from ratelimit: This method will use your `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN` variables that you set as env variables. 
+
+    ```python
+    # for sync client
+    from upstash_ratelimit import RateLimit
+    ratelimit = RateLimit()
+
+    # for async client
+    from upstash_ratelimit.asyncio import RateLimit
+    ratelimit = Ratelimit()
+    ```
+
+- #### Explicit Redis Client: This method will use the Redis client that you manually initiate.
+    ```python
+    # for snyc client
+    from upstash_ratelimit import RateLimit
+    from upstash_redis import Redis
+
+    rate_limit = RateLimit(Redis(url="UPSTASH_REDIS_REST_URL", token="UPSTASH_REDIS_REST_TOKEN"))
+
+
+    # for asnyc client
+    from upstash_ratelimit.asyncio import RateLimit
+    from upstash_redis.asyncio import Redis
+
+    rate_limit = RateLimit(Redis(url="UPSTASH_REDIS_REST_URL", token="UPSTASH_REDIS_REST_TOKEN"))
+    ```
+    For possible Redis client configurations, have a look at the [redis sdk repository](https://github.com/upstash/redis-python/blob/main/upstash_redis/client.py).
+
+- You can also pass a `prefix` to the `RateLimit` constructor to distinguish between the keys used for rate limiting and others.
+It defaults to `"ratelimit"`
+    ```python
+    ratelimit = Ratelimit(prefix="app1_ratelimiter")
+    ```
+    
+### Usage
 
-allow_telemetry: bool = True
-```
 
+**All of the examples below can be implemented in async context as well. Only adding the correct import with async client, and necessary `await` expressions are sufficient for async use.**
 
-## Usage
 
 ```python
-from upstash_ratelimit.limiter import RateLimit
-from upstash_ratelimit.schema.response import RateLimitResponse
-
-from upstash_redis.client import Redis
-
-# Create a ratelimit instance and load the Redis credentials from the environment.
-rate_limit = RateLimit(Redis.from_env())  # Optionally, pass your own client instance.
-
 # Chose one algorithm.
 fixed_window = rate_limit.fixed_window(
     max_number_of_requests=1,
     window=3,
     unit="s"
 )
 
 """
 Use a constant to limit all the requests together.
 For enforcing individual limits, use some kind of identifying variable (IP address, API key, etc.).
 """
 identifier: str = "constant"
 
-
-async def main() -> str:
-    request_result: RateLimitResponse = await fixed_window.limit(identifier)
+def main():
+    request_result = fixed_window.limit(identifier)
 
     if not request_result["is_allowed"]:
         return f"{identifier} is rate-limited!"
     else:
         return "Request passed!"
 ```
 
-You can also pass a `prefix` to the `RateLimit` constructor to distinguish between the keys used for rate limiting and others.
-It defaults to `"ratelimit"`.
-
-The `limit` method also returns some metadata that might be useful :
+The `limit` method also returns the following metadata :
 
 ```python
-from typing import TypedDict
-
-
 class RateLimitResponse(TypedDict):
     """
     The response given by the rate-limiting methods, with additional metadata.
     """
     is_allowed: bool
 
     # The maximum number of requests allowed within a window.
@@ -168,114 +150,53 @@
     remaining: int
 
     # The unix time in milliseconds when the next window begins.
     reset: int
 ```
 
 
-## Telemetry
-The underlying serverless driver can collect the following anonymous telemetry:
-  - the runtime (ex: `python@v.3.10.0`)
-  - the sdk or sdks you're using (ex: `upstash-py@development, upstash-ratelimit@v.0.1.0`)
-  - the platform you're running on (ex: `AWS-lambda`)
-
-If you want to opt-out, simply pass `allow_telemetry=False` to the Redis client.
-
-
 ## Block until ready
 You also have the option to try and wait for a request to pass in the given timeout.
 If the first request is blocked and the timeout exceeds the time needed for the next interval to come,
 we wait and retry once that happens.
 
 ```python
-from upstash_ratelimit.limiter import RateLimit
-from upstash_ratelimit.schema.response import RateLimitResponse
-
-from upstash_redis.client import Redis
-
-rate_limit = RateLimit(Redis.from_env())
-
 fixed_window = rate_limit.fixed_window(
     max_number_of_requests=1,
     window=3,
     unit="s"
 )
 
 identifier: str = "constant"
 
-
-async def main() -> str:
-    request_result: RateLimitResponse = await fixed_window.block_until_ready(identifier, timeout=2000)
+def main() -> str:
+    request_result = fixed_window.block_until_ready(identifier, timeout=2000)
 
     if not request_result["is_allowed"]:
         return f"The {identifier}'s request cannot be processed, even after 2 seconds."
     else:
         return "Request passed!"
 ```
 
 
-## Timeout
-If you worry that network issues can cause your application to reject requests, you can use python's `wait_for` to 
-allow the requests which exceed a given timeout to pass regardless of what the current limit is.
-
-```python
-from upstash_ratelimit.limiter import RateLimit
-from upstash_ratelimit.schema.response import RateLimitResponse
-
-from upstash_redis.client import Redis
-
-from asyncio import wait_for
-
-rate_limit = RateLimit(Redis.from_env())
-
-fixed_window = rate_limit.fixed_window(
-    max_number_of_requests=1,
-    window=3,
-    unit="s"
-)
-
-identifier: str = "constant"
-
-
-async def main() -> str:
-    try:
-        request_result: RateLimitResponse = await wait_for(fixed_window.limit(identifier), 2.0)  # Wait for two seconds.
-
-        if not request_result["is_allowed"]:
-            return f"{identifier} is rate-limited!"
-
-        return "Request passed!"
-
-    except TimeoutError:
-        return "Request passed"
-```
-
-
 ## Rate-limiting outbound requests
 It's also possible to limit the number of requests you're making to an external API.
 
 ```python
-from upstash_ratelimit.limiter import RateLimit
-from upstash_ratelimit.schema.response import RateLimitResponse
-
-from upstash_redis.client import Redis
-
-rate_limit = RateLimit(Redis.from_env())
-
 fixed_window = rate_limit.fixed_window(
     max_number_of_requests=1,
     window=3,
     unit="s"
 )
 
 identifier: str = "constant"  # Or, use an identifier to limit your requests to a certain endpoint.
 
 
-async def main() -> str:
-    request_result: RateLimitResponse = await fixed_window.limit(identifier)
+def main() -> str:
+    request_result = fixed_window.limit(identifier)
 
     if not request_result["is_allowed"]:
         return f"{identifier} is rate-limited!"
     else:
         # Call the API
         # ...
         return "Request passed!"
@@ -293,20 +214,14 @@
 
 ### Cons
 - Can cause high bursts at the window boundaries to leak through
 
 ### Usage
 
 ```python
-from upstash_ratelimit.limiter import RateLimit
-
-from upstash_redis.client import Redis
-
-rate_limit = RateLimit(Redis.from_env())
-
 fixed_window = rate_limit.fixed_window(
     max_number_of_requests=1,
     window=3,
     unit="s"
 )
 ```
 
@@ -321,20 +236,14 @@
 ### Cons
 - More expensive in terms of storage and computation
 - It's only an approximation because it assumes a uniform request flow in the previous window
 
 ### Usage
 
 ```python
-from upstash_ratelimit.limiter import RateLimit
-
-from upstash_redis.client import Redis
-
-rate_limit = RateLimit(Redis.from_env())
-
 sliding_window = rate_limit.sliding_window(
     max_number_of_requests=1,
     window=3,
     unit="s"
 )
 ```
 
@@ -348,66 +257,29 @@
 
 ### Cons
 - Expensive in terms of computation
 
 ### Usage
 
 ```python
-from upstash_ratelimit.limiter import RateLimit
-
-from upstash_redis.client import Redis
-
-rate_limit = RateLimit(Redis.from_env())
-
 token_bucket = rate_limit.token_bucket(
     max_number_of_tokens=2,
     refill_rate=1,
     interval=3,
     unit="s"
 )
 ```
 
 # Contributing
 
 ## Preparing the environment
-This project uses [Poetry](https://python-poetry.org) for packaging and dependency management. 
-
-See [this](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) for a detailed explanation on how
-to work with the virtual environment.
-
-You will also need a database on [Upstash](https://console.upstash.com/). If you already have one, make sure to empty it before running 
-tests. You can do so by sending `FLUSHDB` from the console.
-
-
-## Adding new algorithms
-All the algorithms subclass and implement abstract [RateLimitAlgorithm](upstash_ratelimit/algorithm.py)'s methods.
-
-They are also grouped in the [RateLimit](upstash_ratelimit/limiter.py) class for ease of use.
+This project uses [Poetry](https://python-poetry.org) for packaging and dependency management. Make sure you are able to create the poetry shell with relevant dependencies.
 
+You will also need a database on [Upstash](https://console.upstash.com/).
 
 ## Running tests
-All tests live in the [test](./tests) folder.
-
-Only the logic of 100%-accuracy algorithms and other utility functions are unit-tested.
-
-To run all the tests, make sure you are in the `tests` folder and have the poetry virtual environment activated with all 
+To run all the tests, make sure the poetry virtual environment activated with all 
 the necessary dependencies. Set the `UPSTASH_REDIS_REST_URL` and `UPSTASH_REDIS_REST_TOKEN` environment variables and run:
 
 ```bash
-poetry run pytest --import-mode importlib
+poetry run pytest
 ```
-
-The reason we need to use the `importlib` mode is because there are multiple test files with the same name. See the 
-[pytest docs](https://docs.pytest.org/en/stable/explanation/pythonpath.html#import-modes) for more info.
-
-**Warning**: The current evaluation speed of the tests does not take the HTTP requests duration into account. 
-Because of that, if a request takes more than 2 seconds to complete, a test might fail.
-
-
-## Releasing
-To create a new release, first use Poetry's [version](https://python-poetry.org/docs/cli/#version) command.
-
-You will then need to connect your PyPi API token to Poetry. 
-A simple tutorial showcasing how to do it was posted by Tony Tran
-[on DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)
-
-From there, use `poetry publish --build`.
```

