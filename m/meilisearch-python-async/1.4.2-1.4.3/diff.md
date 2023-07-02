# Comparing `tmp/meilisearch_python_async-1.4.2.tar.gz` & `tmp/meilisearch_python_async-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_python_async-1.4.2.tar", max compression
+gzip compressed data, was "meilisearch_python_async-1.4.3.tar", max compression
```

## Comparing `meilisearch_python_async-1.4.2.tar` & `meilisearch_python_async-1.4.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/LICENSE
--rw-r--r--   0        0        0     5759 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/README.md
--rw-r--r--   0        0        0      151 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/__init__.py
--rw-r--r--   0        0        0     2759 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/_http_requests.py
--rw-r--r--   0        0        0       18 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/_version.py
--rw-r--r--   0        0        0    22205 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/client.py
--rw-r--r--   0        0        0     2085 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/errors.py
--rw-r--r--   0        0        0    89041 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/index.py
--rw-r--r--   0        0        0        0 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/__init__.py
--rw-r--r--   0        0        0     1576 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/client.py
--rw-r--r--   0        0        0      202 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/documents.py
--rw-r--r--   0        0        0       95 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/health.py
--rw-r--r--   0        0        0      392 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/index.py
--rw-r--r--   0        0        0     1285 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/search.py
--rw-r--r--   0        0        0     1119 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/settings.py
--rw-r--r--   0        0        0      769 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/task.py
--rw-r--r--   0        0        0      215 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/models/version.py
--rw-r--r--   0        0        0        0 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/py.typed
--rw-r--r--   0        0        0    11932 2023-06-25 13:09:51.134898 meilisearch_python_async-1.4.2/meilisearch_python_async/task.py
--rw-r--r--   0        0        0     2243 2023-06-25 13:09:51.138898 meilisearch_python_async-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-02 00:19:36.085285 meilisearch_python_async-1.4.3/LICENSE
+-rw-r--r--   0        0        0     5759 2023-07-02 00:19:36.085285 meilisearch_python_async-1.4.3/README.md
+-rw-r--r--   0        0        0      151 2023-07-02 00:19:36.085285 meilisearch_python_async-1.4.3/meilisearch_python_async/__init__.py
+-rw-r--r--   0        0        0     2759 2023-07-02 00:19:36.085285 meilisearch_python_async-1.4.3/meilisearch_python_async/_http_requests.py
+-rw-r--r--   0        0        0     1441 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/_utils.py
+-rw-r--r--   0        0        0       18 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/_version.py
+-rw-r--r--   0        0        0    23114 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/client.py
+-rw-r--r--   0        0        0     2085 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/errors.py
+-rw-r--r--   0        0        0    89314 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/index.py
+-rw-r--r--   0        0        0        0 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/models/__init__.py
+-rw-r--r--   0        0        0     4213 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/models/client.py
+-rw-r--r--   0        0        0      202 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/models/documents.py
+-rw-r--r--   0        0        0       95 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/models/health.py
+-rw-r--r--   0        0        0     1845 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/models/index.py
+-rw-r--r--   0        0        0     1334 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/models/search.py
+-rw-r--r--   0        0        0     1119 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/models/settings.py
+-rw-r--r--   0        0        0     3110 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/models/task.py
+-rw-r--r--   0        0        0      215 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/models/version.py
+-rw-r--r--   0        0        0        0 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/py.typed
+-rw-r--r--   0        0        0    11932 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/meilisearch_python_async/task.py
+-rw-r--r--   0        0        0     2243 2023-07-02 00:19:36.089285 meilisearch_python_async-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 meilisearch_python_async-1.4.3/PKG-INFO
```

### Comparing `meilisearch_python_async-1.4.2/LICENSE` & `meilisearch_python_async-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.2/README.md` & `meilisearch_python_async-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.2/meilisearch_python_async/_http_requests.py` & `meilisearch_python_async-1.4.3/meilisearch_python_async/_http_requests.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.2/meilisearch_python_async/client.py` & `meilisearch_python_async-1.4.3/meilisearch_python_async/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from types import TracebackType
 from typing import Any
 
 import jwt
 from httpx import AsyncClient
 
 from meilisearch_python_async._http_requests import HttpRequests
+from meilisearch_python_async._utils import is_pydantic_2
 from meilisearch_python_async.errors import InvalidRestriction, MeilisearchApiError
 from meilisearch_python_async.index import Index
 from meilisearch_python_async.models.client import (
     ClientStats,
     Key,
     KeyCreate,
     KeySearch,
@@ -384,15 +385,18 @@
             >>>         actions=["search"],
             >>>         indexes=["movies"],
             >>>     )
             >>>     keys = await client.create_key(key_info)
         """
         # The json.loads(key.json()) is because Pydantic can't serialize a date in a Python dict,
         # but can when converting to a json string.
-        response = await self._http_requests.post("keys", json.loads(key.json(by_alias=True)))
+        if is_pydantic_2:
+            response = await self._http_requests.post("keys", json.loads(key.model_dump_json(by_alias=True)))  # type: ignore[attr-defined]
+        else:  # pragma: no cover
+            response = await self._http_requests.post("keys", json.loads(key.json(by_alias=True)))  # type: ignore[attr-defined]
 
         return Key(**response.json())
 
     async def delete_key(self, key: str) -> int:
         """Deletes an API key.
 
         Args:
@@ -491,19 +495,26 @@
                         key="abc123",
             >>>         indexes=["*"],
             >>>     )
             >>>     keys = await client.update_key(key_info)
         """
         # The json.loads(key.json()) is because Pydantic can't serialize a date in a Python dict,
         # but can when converting to a json string.
-        payload = {
-            k: v
-            for k, v in json.loads(key.json(by_alias=True)).items()
-            if v is not None and k != "key"
-        }
+        if is_pydantic_2:
+            payload = {  # type: ignore[attr-defined]
+                k: v
+                for k, v in json.loads(key.model_dump_json(by_alias=True)).items()
+                if v is not None and k != "key"
+            }
+        else:  # pragma: no cover
+            payload = {  # type: ignore[attr-defined]
+                k: v
+                for k, v in json.loads(key.json(by_alias=True)).items()
+                if v is not None and k != "key"
+            }
         response = await self._http_requests.patch(f"keys/{key.key}", payload)
 
         return Key(**response.json())
 
     async def multi_search(self, queries: list[SearchParams]) -> list[SearchResultsWithUID]:
         """Multi-index search.
 
@@ -528,17 +539,22 @@
             >>>     queries = [
             >>>         SearchParams(index_uid="my_first_index", query"Some search"),
             >>>         SearchParams(index_uid="my_second_index", query="Another search")
             >>>     ]
             >>>     search_results = await client.search(queries)
         """
         url = "multi-search"
-        response = await self._http_requests.post(
-            url, body={"queries": [x.dict(by_alias=True) for x in queries]}
-        )
+        if is_pydantic_2:
+            response = await self._http_requests.post(
+                url, body={"queries": [x.model_dump(by_alias=True) for x in queries]}  # type: ignore[attr-defined]
+            )
+        else:  # pragma: no cover
+            response = await self._http_requests.post(
+                url, body={"queries": [x.dict(by_alias=True) for x in queries]}  # type: ignore[attr-defined]
+            )
 
         return [SearchResultsWithUID(**x) for x in response.json()["results"]]
 
     async def get_raw_index(self, uid: str) -> IndexInfo | None:
         """Gets the index and returns all the index information rather than an Index instance.
 
         Args:
```

### Comparing `meilisearch_python_async-1.4.2/meilisearch_python_async/errors.py` & `meilisearch_python_async-1.4.3/meilisearch_python_async/errors.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.2/meilisearch_python_async/index.py` & `meilisearch_python_async-1.4.3/meilisearch_python_async/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import Any, Generator
 from urllib.parse import urlencode
 
 import aiofiles
 from httpx import AsyncClient
 
 from meilisearch_python_async._http_requests import HttpRequests
+from meilisearch_python_async._utils import is_pydantic_2, iso_to_date_time
 from meilisearch_python_async.errors import InvalidDocumentError, MeilisearchError
 from meilisearch_python_async.models.documents import DocumentsInfo
 from meilisearch_python_async.models.index import IndexStats
 from meilisearch_python_async.models.search import SearchResults
 from meilisearch_python_async.models.settings import (
     Faceting,
     MeilisearchSettings,
@@ -50,16 +51,16 @@
             uid: The index's unique identifier.
             primary_key: The primary key of the documents. Defaults to None.
             created_at: The date and time the index was created. Defaults to None.
             updated_at: The date and time the index was last updated. Defaults to None.
         """
         self.uid = uid
         self.primary_key = primary_key
-        self.created_at: datetime | None = _iso_to_date_time(created_at)
-        self.updated_at: datetime | None = _iso_to_date_time(updated_at)
+        self.created_at: datetime | None = iso_to_date_time(created_at)
+        self.updated_at: datetime | None = iso_to_date_time(updated_at)
         self._base_url = "indexes/"
         self._base_url_with_uid = f"{self._base_url}{self.uid}"
         self._documents_url = f"{self._base_url_with_uid}/documents"
         self._stats_url = f"{self._base_url_with_uid}/stats"
         self._settings_url = f"{self._base_url_with_uid}/settings"
         self.http_client = http_client
         self._http_requests = HttpRequests(http_client)
@@ -171,18 +172,18 @@
         """
         url = f"{self._base_url_with_uid}"
         response = await self._http_requests.get(url)
         index_dict = response.json()
         self.primary_key = index_dict["primaryKey"]
         loop = get_running_loop()
         self.created_at = await loop.run_in_executor(
-            None, partial(_iso_to_date_time, index_dict["createdAt"])
+            None, partial(iso_to_date_time, index_dict["createdAt"])
         )
         self.updated_at = await loop.run_in_executor(
-            None, partial(_iso_to_date_time, index_dict["updatedAt"])
+            None, partial(iso_to_date_time, index_dict["updatedAt"])
         )
         return self
 
     async def get_primary_key(self) -> str | None:
         """Get the primary key.
 
         Returns:
@@ -1473,15 +1474,18 @@
             >>>    displayed_attributes=["title", "description", "genre", "release_date"],
             >>>    sortable_attributes=["title", "release_date"],
             >>> )
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     await index.update_settings(new_settings)
         """
-        body_dict = {k: v for k, v in body.dict(by_alias=True).items() if v is not None}
+        if is_pydantic_2:
+            body_dict = {k: v for k, v in body.model_dump(by_alias=True).items() if v is not None}  # type: ignore[attr-defined]
+        else:  # pragma: no cover
+            body_dict = {k: v for k, v in body.dict(by_alias=True).items() if v is not None}  # type: ignore[attr-defined]
 
         url = f"{self._settings_url}"
         response = await self._http_requests.patch(url, body_dict)
 
         return TaskInfo(**response.json())
 
     async def reset_settings(self) -> TaskInfo:
@@ -2180,15 +2184,19 @@
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     TypoTolerance(enabled=False)
             >>>     await index.update_typo_tolerance()
         """
         url = f"{self._settings_url}/typo-tolerance"
-        response = await self._http_requests.patch(url, typo_tolerance.dict(by_alias=True))
+
+        if is_pydantic_2:
+            response = await self._http_requests.patch(url, typo_tolerance.model_dump(by_alias=True))  # type: ignore[attr-defined]
+        else:  # pragma: no cover
+            response = await self._http_requests.patch(url, typo_tolerance.dict(by_alias=True))  # type: ignore[attr-defined]
 
         return TaskInfo(**response.json())
 
     async def reset_typo_tolerance(self) -> TaskInfo:
         """Reset typo tolerance to default values.
 
         Returns:
@@ -2252,15 +2260,19 @@
 
             >>> from meilisearch_python_async import Client
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     await index.update_faceting(faceting=Faceting(max_values_per_facet=100))
         """
         url = f"{self._settings_url}/faceting"
-        response = await self._http_requests.patch(url, faceting.dict(by_alias=True))
+
+        if is_pydantic_2:
+            response = await self._http_requests.patch(url, faceting.model_dump(by_alias=True))  # type: ignore[attr-defined]
+        else:  # pragma: no cover
+            response = await self._http_requests.patch(url, faceting.dict(by_alias=True))  # type: ignore[attr-defined]
 
         return TaskInfo(**response.json())
 
     async def reset_faceting(self) -> TaskInfo:
         """Reset an index's faceting settings to their default value.
 
         Returns:
@@ -2325,15 +2337,19 @@
             >>> from meilisearch_python_async import Client
             >>> from meilisearch_python_async.models.settings import Pagination
             >>> async with Client("http://localhost.com", "masterKey") as client:
             >>>     index = client.index("movies")
             >>>     await index.update_pagination(settings=Pagination(max_total_hits=123))
         """
         url = f"{self._settings_url}/pagination"
-        response = await self._http_requests.patch(url, settings.dict(by_alias=True))
+
+        if is_pydantic_2:
+            response = await self._http_requests.patch(url, settings.model_dump(by_alias=True))  # type: ignore[attr-defined]
+        else:  # pragma: no cover
+            response = await self._http_requests.patch(url, settings.dict(by_alias=True))  # type: ignore[attr-defined]
 
         return TaskInfo(**response.json())
 
     async def reset_pagination(self) -> TaskInfo:
         """Reset an index's pagination settings to their default value.
 
         Returns:
@@ -2371,35 +2387,14 @@
         raise MeilisearchError(f"No {document_type} files found in {directory_path}")
 
 
 def _combine_documents(documents: list[list[Any]]) -> list[Any]:
     return [x for y in documents for x in y]
 
 
-def _iso_to_date_time(iso_date: datetime | str | None) -> datetime | None:
-    """Handle conversion of iso string to datetime.
-
-    The microseconds from Meilisearch are sometimes too long for python to convert so this
-    strips off the last digits to shorten it when that happens.
-    """
-    if not iso_date:
-        return None
-
-    if isinstance(iso_date, datetime):
-        return iso_date
-
-    try:
-        return datetime.strptime(iso_date, "%Y-%m-%dT%H:%M:%S.%fZ")
-    except ValueError:
-        split = iso_date.split(".")
-        reduce = len(split[1]) - 6
-        reduced = f"{split[0]}.{split[1][:-reduce]}Z"
-        return datetime.strptime(reduced, "%Y-%m-%dT%H:%M:%S.%fZ")
-
-
 async def _load_documents_from_file(
     file_path: Path | str,
     csv_delimiter: str | None = None,
 ) -> list[dict[Any, Any]]:
     if isinstance(file_path, str):
         file_path = Path(file_path)
```

### Comparing `meilisearch_python_async-1.4.2/meilisearch_python_async/models/search.py` & `meilisearch_python_async-1.4.3/meilisearch_python_async/models/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     matching_strategy: str = "all"
     hits_per_page: Optional[int] = None
     page: Optional[int] = None
 
 
 class SearchResults(CamelBase):
     hits: List[Dict[str, Any]]
-    offset: Optional[int]
-    limit: Optional[int]
-    estimated_total_hits: Optional[int]
+    offset: Optional[int] = None
+    limit: Optional[int] = None
+    estimated_total_hits: Optional[int] = None
     processing_time_ms: int
     query: str
     facet_distribution: Optional[Dict[str, Any]] = None
-    total_pages: Optional[int]
-    total_hits: Optional[int]
-    page: Optional[int]
-    hits_per_page: Optional[int]
+    total_pages: Optional[int] = None
+    total_hits: Optional[int] = None
+    page: Optional[int] = None
+    hits_per_page: Optional[int] = None
 
 
 class SearchResultsWithUID(SearchResults):
     index_uid: str
```

### Comparing `meilisearch_python_async-1.4.2/meilisearch_python_async/models/settings.py` & `meilisearch_python_async-1.4.3/meilisearch_python_async/models/settings.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.2/meilisearch_python_async/task.py` & `meilisearch_python_async-1.4.3/meilisearch_python_async/task.py`

 * *Files identical despite different names*

### Comparing `meilisearch_python_async-1.4.2/pyproject.toml` & `meilisearch_python_async-1.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-python-async"
-version = "1.4.2"
+version = "1.4.3"
 description = "A Python async client for the Meilisearch API"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-python-async"
 homepage = "https://github.com/sanders41/meilisearch-python-async"
 documentation = "https://meilisearch-python-async.paulsanders.dev"
```

### Comparing `meilisearch_python_async-1.4.2/PKG-INFO` & `meilisearch_python_async-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-python-async
-Version: 1.4.2
+Version: 1.4.3
 Summary: A Python async client for the Meilisearch API
 Home-page: https://github.com/sanders41/meilisearch-python-async
 License: MIT
 Keywords: meilisearch,async,python
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
```

