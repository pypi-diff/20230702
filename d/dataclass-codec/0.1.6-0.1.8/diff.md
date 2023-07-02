# Comparing `tmp/dataclass_codec-0.1.6.tar.gz` & `tmp/dataclass_codec-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_codec-0.1.6.tar", max compression
+gzip compressed data, was "dataclass_codec-0.1.8.tar", max compression
```

## Comparing `dataclass_codec-0.1.6.tar` & `dataclass_codec-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      101 2023-06-21 01:55:42.515322 dataclass_codec-0.1.6/README.md
--rw-r--r--   0        0        0      600 2023-06-21 01:56:10.975311 dataclass_codec-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-18 01:48:53.622553 dataclass_codec-0.1.6/src/dataclass_codec/__init__.py
--rw-r--r--   0        0        0    10238 2023-06-21 01:55:42.515322 dataclass_codec-0.1.6/src/dataclass_codec/decode.py
--rw-r--r--   0        0        0     2929 2023-06-21 01:55:42.515322 dataclass_codec-0.1.6/src/dataclass_codec/encode.py
--rw-r--r--   0        0        0        0 2023-06-18 00:31:15.872983 dataclass_codec-0.1.6/src/dataclass_codec/py.typed
--rw-r--r--   0        0        0    16060 2023-06-21 01:55:42.515322 dataclass_codec-0.1.6/src/dataclass_codec/tests/test_dataclass_codec.py
--rw-r--r--   0        0        0      243 2023-06-17 23:50:02.973209 dataclass_codec-0.1.6/src/dataclass_codec/types_predicates.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 dataclass_codec-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      101 2023-06-21 01:50:47.819434 dataclass_codec-0.1.8/README.md
+-rw-r--r--   0        0        0      600 2023-07-02 21:56:10.944136 dataclass_codec-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-21 01:44:15.139451 dataclass_codec-0.1.8/src/dataclass_codec/__init__.py
+-rw-r--r--   0        0        0    11144 2023-07-02 21:54:59.534143 dataclass_codec-0.1.8/src/dataclass_codec/decode.py
+-rw-r--r--   0        0        0     2929 2023-06-21 01:51:35.509431 dataclass_codec-0.1.8/src/dataclass_codec/encode.py
+-rw-r--r--   0        0        0        0 2023-06-21 01:44:15.139451 dataclass_codec-0.1.8/src/dataclass_codec/py.typed
+-rw-r--r--   0        0        0    16307 2023-07-02 21:49:06.364177 dataclass_codec-0.1.8/src/dataclass_codec/tests/test_dataclass_codec.py
+-rw-r--r--   0        0        0      391 2023-07-02 21:53:28.544152 dataclass_codec-0.1.8/src/dataclass_codec/types_predicates.py
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 dataclass_codec-0.1.8/PKG-INFO
```

### Comparing `dataclass_codec-0.1.6/src/dataclass_codec/decode.py` & `dataclass_codec-0.1.8/src/dataclass_codec/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     cast,
 )
 from uuid import UUID
 
 from dataclass_codec.types_predicates import (
     is_dataclass_predicate,
     is_enum_predicate,
+    is_generic_dataclass_predicate,
 )
 
 
 ANYTYPE = Type[Any]
 
 
 TYPEMATCHPREDICATE = Callable[[ANYTYPE], bool]
@@ -225,14 +226,40 @@
             return decode_it(obj[k], _type.__dataclass_fields__[k].type)
 
     return _type(
         **{k: make_value(k) for k in _type.__dataclass_fields__.keys()}
     )
 
 
+def generic_dataclass_from_primitive_dict(
+    obj: Any, _type: ANYTYPE, decode_it: DECODEIT
+) -> Any:
+    cxt = decode_context()
+    assert is_generic_dataclass_predicate(_type), "{} is not a dataclass".format(
+        _type.__name__
+    )
+
+    assert isinstance(obj, dict), "{} is {} not dict".format(
+        current_path(), type(obj)
+    )
+
+    def make_value(k: str) -> Any:
+        with current_path_scope(current_path() + "." + k):
+            if k not in obj:
+                if cxt.dataclass_unset_as_none:
+                    return None
+                else:
+                    raise ValueError(f"Missing key {k}")
+
+            return decode_it(obj[k], _type.__args__[0])
+
+    return _type(
+        **{k: make_value(k) for k in _type.__origin__.__dataclass_fields__.keys()}
+    )
+
 def decimal_from_str(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
     assert isinstance(
         obj, (str, int, float)
     ), "{} is {} not str, int or float".format(current_path(), type(obj))
     return Decimal(obj)
 
 def uuid_from_str(obj: Any, _type: ANYTYPE, _decode_it: DECODEIT) -> Any:
@@ -362,14 +389,15 @@
     time: iso_time_to_time,
     Decimal: decimal_from_str,
     UUID: uuid_from_str,
 }
 
 DEFAULT_DECODERS_BY_PREDICATE: List[Tuple[TYPEMATCHPREDICATE, TYPEDECODER]] = [
     (is_dataclass_predicate, dataclass_from_primitive_dict),
+    (is_generic_dataclass_predicate, generic_dataclass_from_primitive_dict),
     (is_generic_list_predicate, generic_list_decoder),
     (is_generic_dict_predicate, generic_dict_decoder),
     (is_union_predicate, generic_union_decoder),
     # This must be before is_enum_predicate
     (is_new_type_predicate, generic_new_type_decoder),
     (is_enum_predicate, enum_decoder),
     # This must be last
```

### Comparing `dataclass_codec-0.1.6/src/dataclass_codec/encode.py` & `dataclass_codec-0.1.8/src/dataclass_codec/encode.py`

 * *Files identical despite different names*

### Comparing `dataclass_codec-0.1.6/src/dataclass_codec/tests/test_dataclass_codec.py` & `dataclass_codec-0.1.8/src/dataclass_codec/tests/test_dataclass_codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 from dataclasses import dataclass
 from datetime import date, datetime, time, timezone
 from decimal import Decimal
 from enum import Enum
 import json
-from typing import Any, Dict, List, NewType, Optional, Union
+from typing import Any, Dict, Generic, List, NewType, Optional, TypeVar, Union
 
 import pytest
 
 from dataclass_codec import (
     encode,
     decode,
     decode_context_scope,
@@ -581,7 +581,17 @@
 
     def test_decode_raw_uuid(self) -> None:
         import uuid
 
         assert decode(
             "12345678-1234-5678-1234-567812345678", uuid.UUID
         ) == uuid.UUID("12345678-1234-5678-1234-567812345678")
+
+
+    def test_generic_dataclass(self) -> None:
+        T = TypeVar("T"	)
+        
+        @dataclass
+        class GenericDummy(Generic[T]):
+            a: T
+
+        assert decode({"a": 1}, GenericDummy[int]) == GenericDummy(1)
```

### Comparing `dataclass_codec-0.1.6/PKG-INFO` & `dataclass_codec-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-codec
-Version: 0.1.6
+Version: 0.1.8
 Summary: 
 Author: lucas.silva
 Author-email: lucas.silva@jeaholding.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

