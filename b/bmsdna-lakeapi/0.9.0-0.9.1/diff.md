# Comparing `tmp/bmsdna_lakeapi-0.9.0.tar.gz` & `tmp/bmsdna_lakeapi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.9.0.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.9.1.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.9.0.tar` & `bmsdna_lakeapi-0.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1081 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/LICENSE
--rw-r--r--   0        0        0     9068 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/README.md
--rw-r--r--   0        0        0      337 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1138 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      625 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     7183 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0    10630 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6255 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11269 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12650 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0     7474 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/detail_endpoint.py
--rw-r--r--   0        0        0    10144 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6887 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6813 2023-07-01 21:26:57.008231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4437 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3781 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3136 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2456 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1084 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     2017 2023-07-01 21:26:57.012231 bmsdna_lakeapi-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    10266 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/LICENSE
+-rw-r--r--   0        0        0     9068 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/README.md
+-rw-r--r--   0        0        0      380 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1138 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      625 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     7186 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0    10634 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6256 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11183 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12623 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/datasource.py
+-rw-r--r--   0        0        0     6839 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/detail_endpoint.py
+-rw-r--r--   0        0        0     9907 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6891 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6813 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4443 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3770 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3040 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2409 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1084 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     2017 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.1/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.9.0/LICENSE` & `bmsdna_lakeapi-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/README.md` & `bmsdna_lakeapi-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from deltalake import DeltaTable
 import pyarrow.dataset
 import pypika.queries
 import polars as pl
 from bmsdna.lakeapi.core.config import SearchConfig
 import pypika.terms
 
+
 if TYPE_CHECKING:
     import pandas as pd
 
 
 def get_sql(sql_or_pypika: str | pypika.queries.QueryBuilder, limit_zero=False) -> str:
     if limit_zero:
         sql_or_pypika = (
@@ -205,15 +206,15 @@
                 uri,
             )
             return datetime.fromtimestamp(dt.history(1)[-1]["timestamp"] / 1000.0, tz=timezone.utc)
         import os
 
         return datetime.fromtimestamp(os.path.getmtime(uri), tz=timezone.utc)
 
-    def register_dataframe(
+    def register_datasource(
         self,
         name: str,
         uri: str,
         file_type: FileTypes,
         partitions: Optional[List[Tuple[str, str, Any]]],
     ):
         ds = self.get_pyarrow_dataset(uri, file_type, partitions)
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import pypika.enums
 import pypika
 import os
 from datetime import datetime, timezone
 from bmsdna.lakeapi.core.config import SearchConfig
 from uuid import uuid4
 
+
 ENABLE_COPY_TO = os.environ.get("ENABLE_COPY_TO", "0") == "1"
 
 
 def _get_temp_table_name():
     return "temp_" + str(uuid4()).replace("-", "")
 
 
@@ -208,15 +209,15 @@
             search_con.execute(f"PRAGMA create_fts_index('{persistence_name}', '{pk_name}', {scc})")
             search_con.close()
             if os.path.exists(persistance_file_name):
                 os.remove(persistance_file_name)
             os.rename(persistance_file_name_temp, persistance_file_name)
         self.persistance_file_name = persistance_file_name
 
-    def register_dataframe(
+    def register_datasource(
         self, name: str, uri: str, file_type: FileTypes, partitions: List[Tuple[str, str, Any]] | None
     ):
         self.modified_dates[name] = self.get_modified_date(uri, file_type)
         if file_type == "json":
             self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_json_auto('{uri}', format='array')")
             return
         if file_type == "ndjson":
@@ -224,15 +225,15 @@
             return
         if file_type == "parquet":
             self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_parquet('{uri}')")
             return
         if file_type == "csv":
             self.con.execute(f"CREATE VIEW {name} as SELECT *FROM read_csv_auto('{uri}', delim=',', header=True)")
             return
-        return super().register_dataframe(name, uri, file_type, partitions)
+        return super().register_datasource(name, uri, file_type, partitions)
 
     def list_tables(self) -> ResultData:
         return self.execute_sql(
             "SELECT table_name as name, table_type from information_schema.tables where table_schema='main'"
         )
 
     def __enter__(self):
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_polars.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
     def close(self):
         pass
 
     def json_function(self, term: pypika.terms.Term, assure_string=False):
         raise NotImplementedError()
 
-    def register_dataframe(
+    def register_datasource(
         self,
         name: str,
         uri: str,
         file_type: FileTypes,
         partitions: Optional[List[Tuple[str, str, Any]]],
     ):
         import polars as pl
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,16 @@
     Tuple,
     TypedDict,
     Union,
     cast,
     TYPE_CHECKING,
 )
 from typing_extensions import TypedDict, NotRequired, Required
-from fastapi import APIRouter, Request
 
 import yaml
-from polars.type_aliases import JoinStrategy
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 
 from bmsdna.lakeapi.core.log import get_logger
 from bmsdna.lakeapi.core.partition_utils import _with_implicit_parameters
 from bmsdna.lakeapi.core.types import FileTypes, OperatorType, Param, PolaryTypeFunction, Engines, SearchConfig
 
 if TYPE_CHECKING:
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/datasource.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,15 @@
     Literal,
     Optional,
     Tuple,
     Union,
     cast,
     get_args,
 )
-
 import pyarrow as pa
-import pyarrow.parquet as pq
 import pyarrow.parquet
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
 
 from bmsdna.lakeapi.core.config import BasicConfig, DatasourceConfig, Param
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 from bmsdna.lakeapi.core.log import get_logger
@@ -25,25 +23,26 @@
 from bmsdna.lakeapi.core.types import DeltaOperatorTypes, FileTypes
 from bmsdna.lakeapi.context.df_base import ResultData, ExecutionContext
 import pypika
 from pypika.queries import QueryBuilder
 import pypika.queries as fn
 from datetime import datetime
 
+
 logger = get_logger(__name__)
 
 endpoints = Literal["query", "meta", "request", "sql"]
 
 
 cache = cached(ttl=CACHE_EXPIRATION_TIME_SECONDS, cache=Cache.MEMORY, serializer=PickleSerializer())
 
 df_cache: dict[str, tuple[datetime, pyarrow.Table]] = {}
 
 
-class Dataframe:
+class Datasource:
     def __init__(
         self,
         version: str,
         tag: str,
         name: str,
         config: DatasourceConfig,
         sql_context: ExecutionContext,
@@ -120,15 +119,15 @@
                     if mod_date <= cache_date:
                         self.sql_context.register_arrow(self.tablename, df_t)
                         self.df = self.sql_context.execute_sql(self.query)
                     else:
                         df_cache.pop(self.tablename)
 
             if self.df is None:
-                self.sql_context.register_dataframe(
+                self.sql_context.register_datasource(
                     self.tablename,
                     self.uri,
                     self.config.file_type,
                     partitions=partitions,
                 )
                 self.df = self.sql_context.execute_sql(self.query)
             if self.config.in_memory and not self.tablename in df_cache:
@@ -233,15 +232,15 @@
     return cast(pypika.Criterion, expr)
 
 
 @cache
 async def _create_inner_expr(columns: Optional[List[str]], prmdef, e):
     inner_expr: Optional[pypika.Criterion] = None
     for ck, cv in e.items():
-        logger.info(f"key = {ck}, value = {cv}, columns = {columns}")
+        logger.debug(f"key = {ck}, value = {cv}, columns = {columns}")
         if (columns and not ck in columns) and not ck in prmdef.combi:
             pass
         else:
             if inner_expr is None:
                 inner_expr = pypika.Field(ck) == cv if cv or cv == 0 else pypika.Field(ck).isnull()
             else:
                 inner_expr = inner_expr & (pypika.Field(ck) == cv if cv or cv == 0 else pypika.Field(ck).isnull())
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/detail_endpoint.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/detail_endpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,27 @@
 from typing import Optional, cast
-from typing_extensions import TypedDict, NotRequired, Required
-import duckdb
-import polars as pl
 import pyarrow as pa
 import pypika
 import pypika.queries as fn
-from aiocache import Cache, cached
-from aiocache.serializers import PickleSerializer
 from deltalake import DeltaTable, Metadata
-from deltalake.exceptions import DeltaError
 from fastapi import (
     APIRouter,
-    BackgroundTasks,
-    Depends,
-    Header,
     HTTPException,
     Query,
     Request,
 )
 from pydantic import BaseModel
 from pypika.queries import QueryBuilder
 
 from bmsdna.lakeapi.context import get_context_by_engine
 from bmsdna.lakeapi.context.df_base import ResultData, get_sql
 from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs, Param, SearchConfig
-from bmsdna.lakeapi.core.dataframe import (
-    Dataframe,
-    filter_df_based_on_params,
-    filter_partitions_based_on_params,
-)
-from bmsdna.lakeapi.core.log import get_logger
-from bmsdna.lakeapi.core.model import create_parameter_model, create_response_model
+from bmsdna.lakeapi.core.datasource import Datasource
 from bmsdna.lakeapi.core.partition_utils import should_hide_colname
-from bmsdna.lakeapi.core.response import create_response
-from bmsdna.lakeapi.core.types import (
-    OutputFileType,
-    Engines,
-)
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
-
-
 from bmsdna.lakeapi.core.types import MetadataDetailResult, MetadataSchemaField, MetadataSchemaFieldType
 
 from typing import Optional
 
 
 def _to_dict(tblmeta: Optional[Metadata]):
     if not tblmeta:
@@ -76,15 +54,15 @@
     ) -> MetadataDetailResult:
         import json
 
         req.state.lake_api_basic_config = basic_config
         from bmsdna.lakeapi.context.df_duckdb import DuckDbExecutionContext
 
         with DuckDbExecutionContext(basic_config.default_chunk_size) as context:
-            realdataframe = Dataframe(
+            realdataframe = Datasource(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
 
             if not realdataframe.file_exists():
                 raise HTTPException(404)
             partition_columns = []
             partition_values = None
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 from typing import List, Literal, Optional, Type, Union
-from typing_extensions import TypedDict, NotRequired, Required
-import duckdb
-import polars as pl
 import pyarrow as pa
 import pypika
-import pypika.queries as fn
+from deltalake import DeltaTable
 from aiocache import Cache, cached
 from aiocache.serializers import PickleSerializer
-from deltalake import DeltaTable, Metadata
-from deltalake.exceptions import DeltaError
 from fastapi import (
     APIRouter,
     BackgroundTasks,
     Depends,
     Header,
     HTTPException,
     Query,
     Request,
 )
 from pydantic import BaseModel
-from pypika.queries import QueryBuilder
 
 from bmsdna.lakeapi.context import get_context_by_engine
 from bmsdna.lakeapi.context.df_base import ResultData, get_sql
-from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs, Param, SearchConfig
-from bmsdna.lakeapi.core.dataframe import (
-    Dataframe,
+from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs
+from bmsdna.lakeapi.core.datasource import (
+    Datasource,
     filter_df_based_on_params,
     filter_partitions_based_on_params,
 )
 from bmsdna.lakeapi.core.log import get_logger
 from bmsdna.lakeapi.core.model import create_parameter_model, create_response_model
 from bmsdna.lakeapi.core.partition_utils import should_hide_colname
 from bmsdna.lakeapi.core.response import create_response
@@ -40,18 +34,18 @@
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 
 cache = cached(ttl=CACHE_EXPIRATION_TIME_SECONDS, cache=Cache.MEMORY, serializer=PickleSerializer())
 
 logger = get_logger(__name__)
 
 
-async def get_partitions(dataframe: Dataframe, params: BaseModel, config: Config) -> Optional[list]:
+async def get_partitions(datasource: Datasource, params: BaseModel, config: Config) -> Optional[list]:
     parts = (
         await filter_partitions_based_on_params(
-            DeltaTable(dataframe.uri).metadata(),
+            DeltaTable(datasource.uri).metadata(),
             params.dict(exclude_unset=True) if params else {},
             config.params or [],
         )
         if config.datasource.file_type == "delta"
         else None
     )
     return parts
@@ -148,22 +142,22 @@
         offset: Optional[int] = 0,
         select: Union[str, None] = Query(title="$select", alias="$select", default=None, include_in_schema=False),
         distinct: bool = Query(title="$distinct", alias="$distinct", default=False, include_in_schema=False),
         engine: Engines = Query(title="$engine", alias="$engine", default="duckdb", include_in_schema=False),
         format: Optional[OutputFileType] = "json",
         jsonify_complex: bool = Query(title="jsonify_complex", include_in_schema=has_complex, default=False),
     ):  # type: ignore
-        logger.info(f"{params.dict(exclude_unset=True) if params else None}Union[ ,  ]{request.url.path}")
+        logger.debug(f"{params.dict(exclude_unset=True) if params else None}Union[ ,  ]{request.url.path}")
 
         engine = engine or basic_config.default_engine
 
-        logger.info(f"Engine: {engine}")
+        logger.debug(f"Engine: {engine}")
 
         with get_context_by_engine(engine, chunk_size=config.chunk_size or basic_config.default_chunk_size) as context:
-            realdataframe = Dataframe(
+            realdataframe = Datasource(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
             parts = await get_partitions(realdataframe, params, config)
             df = realdataframe.get_df(parts or None)
 
             expr = await get_params_filter_expr(df.columns(), config, params)
             base_schema = df.arrow_schema()
@@ -231,15 +225,15 @@
                     )
                 assert score_sum is not None
                 new_query = new_query.select(score_sum.as_("search_score"))
                 new_query = new_query.where(pypika.terms.NotNullCriterion(pypika.queries.Field("search_score")))
 
                 new_query = new_query.orderby(pypika.Field("search_score"), order=pypika.Order.desc)
 
-            logger.info(f"Query: {get_sql(new_query)}")
+            logger.debug(f"Query: {get_sql(new_query)}")
 
             df2 = context.execute_sql(new_query)
 
             try:
                 return await create_response(
                     request.url,
                     format or request.headers["Accept"],
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import pyarrow as pa
 
 cache = cached(ttl=CACHE_EXPIRATION_TIME_SECONDS, cache=Cache.MEMORY, serializer=PickleSerializer())
 
 
 def _make_model(v, name):
     if type(v) is dict:
-        return create_model(name, **{k: _make_model(v, k) for k, v in v.items()}), ... # type: ignore
+        return create_model(name, **{k: _make_model(v, k) for k, v in v.items()}), ...  # type: ignore
     return type(v), None
 
 
 def make_model(v: Dict, name: str):
     return _make_model(v, name)[0]
 
 
@@ -76,15 +76,15 @@
         assert isinstance(st, pa.StructType)
         res = {
             st.field(ind).name: get_schema_for(model_ns, st.field(ind).name, st.field(ind).type)
             for ind in range(0, st.num_fields)
         }
         return (
             Union[
-                create_model(model_ns + ("_" + field_name if field_name else ""), **res, __base__=TypeBaseModel), # type: ignore
+                create_model(model_ns + ("_" + field_name if field_name else ""), **res, __base__=TypeBaseModel),  # type: ignore
                 None,
             ],
             None,
         )
     if pa.types.is_list(field_type) or pa.types.is_large_list(field_type):
         if field_type.value_type is None:
             return (Union[List[Any], None], [])
@@ -158,15 +158,15 @@
                             param.real_default if not param.required else ...,
                         )
         for sc in search or []:
             query_params[sc.name] = (
                 Optional[str],
                 None,
             )
-        query_model = create_model(name + "Parameter", **query_params) # type: ignore
+        query_model = create_model(name + "Parameter", **query_params)  # type: ignore
         return query_model
     return empty_model
 
 
 class TypeBaseModel(BaseModel):
     class Config:
         orm_mode = True
@@ -176,8 +176,8 @@
     schema = frame.arrow_schema()
     props = {
         k: get_schema_for(name, schema.field(k).name, schema.field(k).type)
         for k in schema.names
         if not should_hide_colname(k)
     }
 
-    return create_model(name, **props, __base__=TypeBaseModel) # type: ignore
+    return create_model(name, **props, __base__=TypeBaseModel)  # type: ignore
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/route.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,17 @@
         for config in configs:
             methods = (
                 cast(list[Literal["get", "post"]], [config.api_method])
                 if isinstance(config.api_method, str)
                 else config.api_method
             )
             try:
-                from bmsdna.lakeapi.core.dataframe import Dataframe
+                from bmsdna.lakeapi.core.datasource import Datasource
 
-                realdataframe = Dataframe(
+                realdataframe = Datasource(
                     config.version_str, config.tag, config.name, config.datasource, context, basic_config
                 )
                 if not realdataframe.file_exists():
                     logger.warning(
                         f"Could not get response type for f{config.route}. Path does not exist:{realdataframe.uri}"
                     )
                     metamodel = None
@@ -95,17 +95,17 @@
             )
 
         @router.on_event("startup")
         @_repeat_every(seconds=60 * 60)  # 1 hour
         def _persist_search_endpoints() -> None:
             for config in configs:
                 if config.search:
-                    from bmsdna.lakeapi.core.dataframe import Dataframe
+                    from bmsdna.lakeapi.core.datasource import Datasource
 
-                    realdataframe = Dataframe(
+                    realdataframe = Datasource(
                         config.version_str, config.tag, config.name, config.datasource, context, basic_config
                     )
                     if realdataframe.file_exists():
                         with get_context_by_engine(
                             basic_config.default_engine, basic_config.default_chunk_size
                         ) as ctx:
                             ctx.init_search(realdataframe.tablename, config.search)
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from typing import Optional, Union
-import duckdb
 from fastapi import APIRouter, BackgroundTasks, Header, Query, Request
 from bmsdna.lakeapi.context.df_base import ExecutionContext
 from bmsdna.lakeapi.core.config import BasicConfig, Config, Configs, Param, SearchConfig
-from bmsdna.lakeapi.core.dataframe import Dataframe
+from bmsdna.lakeapi.core.datasource import Datasource
 from bmsdna.lakeapi.core.types import OutputFileType
 from bmsdna.lakeapi.core.response import create_response
 from bmsdna.lakeapi.context import get_context_by_engine, Engines
 
 sql_contexts: dict[str, ExecutionContext] = {}
 
 
 def init_duck_con(con: ExecutionContext, basic_config: BasicConfig, configs: Configs):
     for cfg in configs:
-        df = Dataframe(cfg.version_str, cfg.tag, cfg.name, cfg.datasource, con, basic_config)
+        df = Datasource(cfg.version_str, cfg.tag, cfg.name, cfg.datasource, con, basic_config)
         if df.file_exists():
-            con.register_dataframe(df.tablename, df.uri, df.config.file_type, None)
+            con.register_datasource(df.tablename, df.uri, df.config.file_type, None)
 
 
 def get_sql_context(engine: Engines, basic_config: BasicConfig, configs: Configs):
     global sql_contexts
     if not engine in sql_contexts:
         sql_contexts[engine] = get_context_by_engine(engine, basic_config.default_chunk_size)
         init_duck_con(sql_contexts[engine], basic_config, configs)
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from dataclasses import dataclass
 from typing import Any, List, Literal, cast
 from datetime import datetime, date, time, timedelta
 from decimal import Decimal
 from typing import Type, Optional
-from typing_extensions import TypedDict
-from polars.datatypes.convert import DataTypeMappings
 from pydantic import BaseModel
 
 
 Engines = Literal["duckdb", "polars"]
 
 
 FileTypes = Literal[
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/uservalidation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Sequence
 from fastapi import Depends, HTTPException, Request, status
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from bmsdna.lakeapi.core.config import BasicConfig, Configs, UserConfig
-from bmsdna.lakeapi.core.yaml import get_yaml
 from aiocache import cached, Cache
 from aiocache.serializers import PickleSerializer
 from bmsdna.lakeapi.core.env import CACHE_EXPIRATION_TIME_SECONDS
 from fastapi import FastAPI, Response
 
 cache = cached(
     ttl=CACHE_EXPIRATION_TIME_SECONDS * 10000,
```

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.0/pyproject.toml` & `bmsdna_lakeapi-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
@@ -24,16 +24,16 @@
 
 # auth
 argon2-cffi = {version = "^21.3.0", optional=true}
 
 xlsxwriter = "^3.1.0"
 pyjwt = {version = "^2.6.0", optional = true}
 "ruamel.yaml" = {version = "^0.17.26", optional = true}
-fastapi = "^0.96.0"
 deltalake = "^0.10.0"
+fastapi = "^0.99.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.308"
 black = "^23.3.0"
 uvicorn = "^0.22.0"
 psutil = "^5.9.5"
```

### Comparing `bmsdna_lakeapi-0.9.0/PKG-INFO` & `bmsdna_lakeapi-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Provides-Extra: polars
 Provides-Extra: schema
 Provides-Extra: useradd
 Requires-Dist: aiocache (>=0.12.1,<0.13.0)
 Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0) ; extra == "auth"
 Requires-Dist: deltalake (>=0.10.0,<0.11.0)
 Requires-Dist: duckdb (>=0.8.1,<0.9.0)
-Requires-Dist: fastapi (>=0.96.0,<0.97.0)
+Requires-Dist: fastapi (>=0.99.0,<0.100.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0) ; extra == "schema"
 Requires-Dist: polars (>=0.18.0,<0.19.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0) ; extra == "auth"
 Requires-Dist: pypika (>=0.48.9,<0.49.0)
 Requires-Dist: python2jsonschema (>=0.8,<0.9) ; extra == "schema"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: ruamel.yaml (>=0.17.26,<0.18.0) ; extra == "useradd"
```

