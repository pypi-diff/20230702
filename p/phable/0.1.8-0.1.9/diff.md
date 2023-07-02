# Comparing `tmp/phable-0.1.8.tar.gz` & `tmp/phable-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phable-0.1.8.tar", max compression
+gzip compressed data, was "phable-0.1.9.tar", max compression
```

## Comparing `phable-0.1.8.tar` & `phable-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.8/LICENSE
--rw-r--r--   0        0        0     2894 2023-06-02 16:37:32.321897 phable-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.8/phable/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 02:17:33.194840 phable-0.1.8/phable/auth/__init__.py
--rw-r--r--   0        0        0     7571 2023-06-02 15:16:52.369248 phable-0.1.8/phable/auth/scram.py
--rw-r--r--   0        0        0     9577 2023-06-02 15:45:01.035920 phable-0.1.8/phable/client.py
--rw-r--r--   0        0        0      663 2023-06-02 02:25:41.532878 phable-0.1.8/phable/exceptions.py
--rw-r--r--   0        0        0     1785 2023-06-02 14:50:39.440150 phable-0.1.8/phable/http.py
--rw-r--r--   0        0        0     4268 2023-06-02 14:33:04.856035 phable-0.1.8/phable/kinds.py
--rw-r--r--   0        0        0        0 2023-06-02 02:17:33.196550 phable-0.1.8/phable/parser/__init__.py
--rw-r--r--   0        0        0     4826 2023-06-02 02:17:33.196760 phable-0.1.8/phable/parser/json.py
--rw-r--r--   0        0        0      721 2023-06-02 16:40:43.139404 phable-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 phable-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-18 20:20:49.329618 phable-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2894 2023-07-01 11:26:36.087939 phable-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 18:42:50.546791 phable-0.1.9/phable/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:17:33.194840 phable-0.1.9/phable/auth/__init__.py
+-rw-r--r--   0        0        0     7668 2023-06-29 11:54:21.546987 phable-0.1.9/phable/auth/scram.py
+-rw-r--r--   0        0        0     9771 2023-06-29 11:54:21.547291 phable-0.1.9/phable/client.py
+-rw-r--r--   0        0        0      663 2023-06-02 02:25:41.532878 phable-0.1.9/phable/exceptions.py
+-rw-r--r--   0        0        0     1807 2023-06-29 11:54:21.547531 phable-0.1.9/phable/http.py
+-rw-r--r--   0        0        0     4260 2023-07-01 11:26:36.088779 phable-0.1.9/phable/kinds.py
+-rw-r--r--   0        0        0        0 2023-06-02 02:17:33.196550 phable-0.1.9/phable/parser/__init__.py
+-rw-r--r--   0        0        0     4876 2023-06-29 11:54:21.547786 phable-0.1.9/phable/parser/json.py
+-rw-r--r--   0        0        0        0 2023-07-01 11:26:36.088820 phable-0.1.9/phable/py.typed
+-rw-r--r--   0        0        0     1000 2023-07-01 16:27:14.195156 phable-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 phable-0.1.9/PKG-INFO
```

### Comparing `phable-0.1.8/LICENSE` & `phable-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phable-0.1.8/README.md` & `phable-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```python
 from phable.client import Client
 from phable.kinds import Grid, Ref
 from typing import Any
 import pandas as pd
 
 # define these settings specific to your use case
-# Reminder:  Probably secure your login credentials!!!
+# Reminder:  Properly secure your login credentials!!!
 uri = "http://localhost:8080/api/demo"
 username = "su"
 password = "su"
 
 
 # define convenience func for converting Haystack Grid to Pandas DataFrame
 def to_pandas(grid: Grid) -> pd.DataFrame:
```

### Comparing `phable-0.1.8/phable/auth/scram.py` & `phable-0.1.9/phable/auth/scram.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,21 @@
         functions defined in this module are used in HTTP messages sent and received by
         the Client class in `phable.client.py`.
 """
 
 import hashlib
 import hmac
 import re
-from base64 import urlsafe_b64decode, urlsafe_b64encode, b64encode
+from base64 import b64encode, urlsafe_b64decode, urlsafe_b64encode
 from dataclasses import dataclass
-from hashlib import pbkdf2_hmac
 from functools import cached_property
-from phable.exceptions import NotFoundError
+from hashlib import pbkdf2_hmac
 from uuid import uuid4
 
-
+from phable.exceptions import NotFoundError
 from phable.http import HttpResponse
 
 
 @dataclass(frozen=True)
 class Scram:
     """Data container for RFC5802 SCRAM exchange with helper properties."""
 
@@ -33,15 +32,17 @@
     c1_bare: str
     s_nonce: str
     salt: str
     iter_count: int
 
     @cached_property
     def _salted_password(self) -> bytes:
-        return _salted_password(self.salt, self.iter_count, self.hash, self.password)
+        return _salted_password(
+            self.salt, self.iter_count, self.hash, self.password
+        )
 
     @property
     def client_key(self) -> bytes:
         return _hmac(self._salted_password, b"Client Key", self.hash)
 
     @property
     def stored_key(self) -> bytes:
@@ -58,15 +59,17 @@
         return (
             f"{self.c1_bare},r={self.s_nonce},s={self.salt},"
             + f"i={self.iter_count},{self.client_final_no_proof}"
         )
 
     @property
     def client_signature(self) -> bytes:
-        return _hmac(self.stored_key, self.auth_message.encode("utf-8"), self.hash)
+        return _hmac(
+            self.stored_key, self.auth_message.encode("utf-8"), self.hash
+        )
 
     @property
     def client_proof(self) -> str:
         return to_base64(_xor(self.client_key, self.client_signature))
 
     @property
     def server_key(self) -> bytes:
@@ -82,15 +85,17 @@
 
     @property
     def client_final_message(self) -> str:
         client_final = self.client_final_no_proof + ",p=" + self.client_proof
         return to_base64(client_final)
 
 
-def parse_hello_call_result(hello_call_result: HttpResponse) -> tuple[str, str]:
+def parse_hello_call_result(
+    hello_call_result: HttpResponse,
+) -> tuple[str, str]:
     """Parses the handshake token and hash from the 'WWW-Authenticate' header in the
     server generated HELLO message.
     """
 
     auth_header = hello_call_result.headers["WWW-Authenticate"]
 
     # find the handshake token
@@ -122,30 +127,34 @@
         s_new = "sha256"
 
     hash = s_new
 
     return handshake_token, hash
 
 
-def parse_first_call_result(first_call_result: HttpResponse) -> tuple[str, str, int]:
+def parse_first_call_result(
+    first_call_result: HttpResponse,
+) -> tuple[str, str, int]:
     """Parses the server nonce, salt, and iteration count from the 'WWW-Authenticate'
     header in the "server-first-message".
     """
 
     auth_header = first_call_result.headers["WWW-Authenticate"]
     exclude_msg = "scram data="
     scram_data = re.search(f"({exclude_msg})[a-zA-Z0-9]+", auth_header)
 
     if scram_data is None:
         raise NotFoundError(
             f"Scram data not found in the 'WWW-Authenticate' header:\n{auth_header}"
         )
 
     decoded_scram_data = _from_base64(scram_data.group(0)[len(exclude_msg) :])
-    s_nonce, salt, iteration_count = decoded_scram_data.replace(" ", "").split(",")
+    s_nonce, salt, iteration_count = decoded_scram_data.replace(" ", "").split(
+        ","
+    )
 
     if "r=" not in s_nonce:
         raise NotFoundError(
             f"Server nonce not found in the 'WWW-Authenticate' header:\n{auth_header}"
         )
     elif "s=" not in salt:
         raise NotFoundError(
@@ -156,17 +165,17 @@
             (
                 "Iteration count not found in the 'WWW-Authenticate' header:"
                 f"\n{auth_header}"
             )
         )
 
     return (
-        s_nonce.replace("r=", ""),
-        salt.replace("s=", ""),
-        int(iteration_count.replace("i=", "")),
+        s_nonce.replace("r=", "", 1),
+        salt.replace("s=", "", 1),
+        int(iteration_count.replace("i=", "", 1)),
     )
 
 
 def parse_final_call_result(resp: HttpResponse) -> tuple[str, str]:
     """Parses the auth token from the 'WWW-Authenticate' header in the
     "server-final-message".
     """
@@ -184,15 +193,15 @@
     auth_token = s1.group(0)[len(exclude_msg1) :]
 
     exclude_msg2 = "data="
     s2 = re.search(f"({exclude_msg2})[^,]+", auth_header)
 
     data = s2.group(0)[len(exclude_msg2) :]
 
-    server_signature = _from_base64(data).replace("v=", "")
+    server_signature = _from_base64(data).replace("v=", "", 1)
 
     return auth_token, server_signature
 
 
 def c1_bare(username: str) -> str:
     nonce = str(uuid4()).replace("-", "")
     return f"n={username},r={nonce}"
@@ -225,15 +234,17 @@
     return output
 
 
 def _salted_password(
     salt: str, iterations: int, hash_func: str, password: str
 ) -> bytes:
     """Generates a salted password according to RFC5802."""
-    dk = pbkdf2_hmac(hash_func, password.encode(), urlsafe_b64decode(salt), iterations)
+    dk = pbkdf2_hmac(
+        hash_func, password.encode(), urlsafe_b64decode(salt), iterations
+    )
     return dk
 
 
 def _from_base64(msg: str) -> str:  # str
     return urlsafe_b64decode(_to_bytes(msg)).decode("utf-8")
```

### Comparing `phable-0.1.8/phable/client.py` & `phable-0.1.9/phable/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 from typing import Any, Optional
 
 from phable.auth.scram import (
+    Scram,
     c1_bare,
-    parse_hello_call_result,
     parse_final_call_result,
-    Scram,
-    to_base64,
     parse_first_call_result,
+    parse_hello_call_result,
+    to_base64,
 )
 from phable.exceptions import (
     IncorrectHttpStatus,
     InvalidCloseError,
-    UnknownRecError,
-    ServerSignatureNotEqualError,
     ScramAuthError,
+    ServerSignatureNotEqualError,
+    UnknownRecError,
 )
 from phable.http import request
 from phable.kinds import Grid, Ref
 
 logger = logging.getLogger(__name__)
 
 
@@ -58,37 +58,43 @@
         """
         try:
             self._hello_call()
             self._c1_bare = c1_bare(self.username)
             self._first_call()
             self._final_call()
         except Exception:
-            logger.critical("Unable to scram authenticate with the Haystack Server.")
+            logger.critical(
+                "Unable to scram authenticate with the Haystack Server."
+            )
             raise ScramAuthError
 
     def _hello_call(self) -> None:
         """Defines and sends the HELLO message to the server and processes the server's
         response according to Project Haystack's SCRAM auth instructions."""
 
-        headers = {"Authorization": f"HELLO username={to_base64(self.username)}"}
+        headers = {
+            "Authorization": f"HELLO username={to_base64(self.username)}"
+        }
         response = request(self.uri + "/about", headers=headers, method="GET")
 
         self._handshake_token, self._hash = parse_hello_call_result(response)
 
     def _first_call(self) -> None:
         """Defines and sends the "client-first-message" to the server and processes the
         server's response according to RFC5802."""
 
         gs2_header = "n,,"
         headers = {
             "Authorization": f"scram handshakeToken={self._handshake_token}, "
             f"hash={self._hash}, data={to_base64(gs2_header+self._c1_bare)}"
         }
         response = request(self.uri + "/about", headers=headers, method="GET")
-        self._s_nonce, self._salt, self._iter_count = parse_first_call_result(response)
+        self._s_nonce, self._salt, self._iter_count = parse_first_call_result(
+            response
+        )
 
     def _final_call(self) -> None:
         """Defines and sends the "client-final-message" to the server and processes the
         server's response according to RFC5802.
 
         If the SCRAM authentication exchange was successful then the auth token parsed
         from the server's response is assigned to the _auth_token attribute in this
@@ -160,30 +166,36 @@
     def read_by_id(self, id: Ref) -> dict[str, Any]:
         """Read a record by its id."""
         grid = Grid.to_grid({"id": {"_kind": "ref", "val": id.val}})
         response = self.call("read", grid)
 
         # verify the rec was found
         if response.cols[0]["name"] == "empty":
-            raise UnknownRecError(f"Unable to locate id {id.val} on the server.")
+            raise UnknownRecError(
+                f"Unable to locate id {id.val} on the server."
+            )
 
         return response.rows[0]
 
     def read_by_ids(self, ids: list[Ref]) -> Grid:
         """Read records by their ids."""
         parsed_ids = [{"id": {"_kind": "ref", "val": id.val}} for id in ids]
         grid = Grid.to_grid(parsed_ids)
         response = self.call("read", grid)
 
         # verify the recs were found
         if len(response.rows) == 0:
-            raise UnknownRecError("Unable to locate any of the ids on the server.")
+            raise UnknownRecError(
+                "Unable to locate any of the ids on the server."
+            )
         for row in response.rows:
             if len(row) == 0:
-                raise UnknownRecError("Unable to locate one or more ids on the server.")
+                raise UnknownRecError(
+                    "Unable to locate one or more ids on the server."
+                )
 
         return response
 
     def his_read(self, ids: Ref | list[Ref], range: str) -> Grid:
         """Read history data on selected records for the given range."""
         if isinstance(ids, Ref):
             grid = Grid.to_grid(
@@ -220,15 +232,17 @@
     # ----------------------------------------------------------------------------------
     # base to Haystack and all other ops
     # ----------------------------------------------------------------------------------
 
     def call(
         self,
         op: str,
-        grid: Grid = Grid(meta={"ver": "3.0"}, cols=[{"name": "empty"}], rows=[]),
+        grid: Grid = Grid(
+            meta={"ver": "3.0"}, cols=[{"name": "empty"}], rows=[]
+        ),
     ) -> Grid:
         headers = {
             "Authorization": f"BEARER authToken={self._auth_token}",
             "Accept": "application/json",
         }
 
         data = {
```

### Comparing `phable-0.1.8/phable/exceptions.py` & `phable-0.1.9/phable/exceptions.py`

 * *Files identical despite different names*

### Comparing `phable-0.1.8/phable/http.py` & `phable-0.1.9/phable/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,17 @@
     data: Optional[dict[str, Any]] = None,
     headers: Optional[dict[str, Any]] = None,
     method: str = "GET",
     error_count: int = 0,
 ) -> HttpResponse:
     """Performs an HTTP request."""
     if not url.startswith("http"):
-        raise urllib.error.URLError("Incorrect and possibly insecure protocol in url")
+        raise urllib.error.URLError(
+            "Incorrect and possibly insecure protocol in url"
+        )
     headers = headers or {}
     data = data or {}
 
     request_data = json.dumps(data).encode()
     headers["Content-Type"] = "application/json; charset=UTF-8"
 
     httprequest = urllib.request.Request(
```

### Comparing `phable-0.1.8/phable/kinds.py` & `phable-0.1.9/phable/kinds.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
     def __str__(self):
         return "Grid"
 
 
 @dataclass(frozen=True, slots=True)
 class Number:
-    val: float
-    unit: Optional[str] = None
+    val: int
+    unit: str | None = None
 
     def __str__(self):
         return f"{self.val}{self.unit}"
 
 
 # Marker() is a singleton
 class Marker:
@@ -105,15 +105,15 @@
 
 # TODO: Determine if I need make_handle func on Ref()
 # TODO:  Should dis in Ref be mandatory?
 # TODO:  Improve human readability
 @dataclass(frozen=True, slots=True)
 class Ref:
     val: str
-    dis: Optional[str] = None
+    dis: str | None = None
 
     def __str__(self) -> str:
         return self.dis
 
 
 @dataclass(frozen=True, slots=True)
 class Date:
```

### Comparing `phable-0.1.8/phable/parser/json.py` & `phable-0.1.9/phable/parser/json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 from __future__ import annotations
 
 import logging
 from datetime import date, datetime, time
+from functools import lru_cache
 from typing import Any
 from zoneinfo import ZoneInfo, available_timezones
 
 from phable.exceptions import NotFoundError
-from phable.kinds import (NA, Coordinate, Date, DateTime, Grid, Marker, Number,
-                          Ref, Remove, Symbol, Time, Uri, XStr)
+from phable.kinds import (
+    NA,
+    Coordinate,
+    Date,
+    DateTime,
+    Grid,
+    Marker,
+    Number,
+    Ref,
+    Remove,
+    Symbol,
+    Time,
+    Uri,
+    XStr,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def json_to_grid(d: dict[str, Any]) -> Grid:
     _parse_kinds(d)
     return Grid(meta=d["meta"], cols=d["cols"], rows=d["rows"])
@@ -81,15 +95,17 @@
         return Number(float(d["val"]), unit)
     except KeyError:
         logger.debug(
             f"Received this input which did not have the expected 'val' key:\n{d}"
         )
         raise
     except ValueError:
-        logger.debug(f"Unable to parse the 'val' key's value into a float:\n{d}")
+        logger.debug(
+            f"Unable to parse the 'val' key's value into a float:\n{d}"
+        )
         raise
 
 
 def _parse_marker(d: dict[str, str]) -> Marker:
     return Marker()
 
 
@@ -117,46 +133,45 @@
         return Date(date.fromisoformat(d["val"]))
     except KeyError:
         logger.debug(
             f"Received this input which did not have the expected 'val' key:\n{d}"
         )
         raise
     except ValueError:
-        logger.debug(f"Unable to parse the 'val' key's value into a date:\n{d}")
+        logger.debug(
+            f"Unable to parse the 'val' key's value into a date:\n{d}"
+        )
         raise
 
 
 def _parse_time(d: dict[str, str]):
     try:
         return Time(time.fromisoformat(d["val"]))
     except KeyError:
         logger.debug(
             f"Received this input which did not have the expected 'val' key:\n{d}"
         )
         raise
     except ValueError:
-        logger.debug(f"Unable to parse the 'val' key's value into a time:\n{d}")
+        logger.debug(
+            f"Unable to parse the 'val' key's value into a time:\n{d}"
+        )
         raise
 
 
-def _build_iana_tz(haystack_tz: str) -> str:
-    for iana_tz in available_timezones():
-        if "/" + haystack_tz in iana_tz:
-            return iana_tz
-
-    raise NotFoundError(f"Can't locate the city {haystack_tz} in the IANA database")
-
-
+@lru_cache(maxsize=16)
 def _haystack_to_iana_tz(haystack_tz: str) -> ZoneInfo:
-    if haystack_tz in available_timezones():
-        iana_tz = haystack_tz
-    else:
-        iana_tz = _build_iana_tz(haystack_tz)
+    for iana_tz in available_timezones():
+        if "/" + haystack_tz in iana_tz or haystack_tz == iana_tz:
+            return ZoneInfo(iana_tz)
 
-    return ZoneInfo(iana_tz)
+    # future: maybe return None instead of raising error?
+    raise NotFoundError(
+        f"Can't locate the city {haystack_tz} in the IANA database"
+    )
 
 
 def _parse_date_time(d: dict[str, str]):
     try:
         haystack_tz: str = d["tz"]
         iana_tz: ZoneInfo = _haystack_to_iana_tz(haystack_tz)
         dt = datetime.fromisoformat(d["val"]).astimezone(iana_tz)
```

### Comparing `phable-0.1.8/PKG-INFO` & `phable-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phable
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 License: MIT
 Author: Rick Jennings
 Author-email: rjennings055@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 ```python
 from phable.client import Client
 from phable.kinds import Grid, Ref
 from typing import Any
 import pandas as pd
 
 # define these settings specific to your use case
-# Reminder:  Probably secure your login credentials!!!
+# Reminder:  Properly secure your login credentials!!!
 uri = "http://localhost:8080/api/demo"
 username = "su"
 password = "su"
 
 
 # define convenience func for converting Haystack Grid to Pandas DataFrame
 def to_pandas(grid: Grid) -> pd.DataFrame:
```

