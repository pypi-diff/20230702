# Comparing `tmp/authomize-rest-api-client-4.3.0.tar.gz` & `tmp/authomize-rest-api-client-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.3.0.tar", last modified: Thu Jun 22 11:36:14 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.3.1.tar", last modified: Sun Jul  2 08:33:53 2023, max compression
```

## Comparing `authomize-rest-api-client-4.3.0.tar` & `authomize-rest-api-client-4.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2194 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76002 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43982 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   190165 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   102274 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-22 11:35:56.000000 authomize-rest-api-client-4.3.0/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      206 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-22 11:36:14.000000 authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-22 11:36:14.211358 authomize-rest-api-client-4.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-22 11:36:13.000000 authomize-rest-api-client-4.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76002 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45350 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   190165 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104842 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-02 08:33:35.000000 authomize-rest-api-client-4.3.1/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-02 08:33:53.000000 authomize-rest-api-client-4.3.1/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-02 08:33:53.000000 authomize-rest-api-client-4.3.1/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 08:33:53.000000 authomize-rest-api-client-4.3.1/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2023-07-02 08:33:53.000000 authomize-rest-api-client-4.3.1/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-02 08:33:53.000000 authomize-rest-api-client-4.3.1/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-02 08:33:53.745136 authomize-rest-api-client-4.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-07-02 08:33:38.000000 authomize-rest-api-client-4.3.1/setup.py
```

### Comparing `authomize-rest-api-client-4.3.0/LICENSE.txt` & `authomize-rest-api-client-4.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/README.md` & `authomize-rest-api-client-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.3.1/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.3.1/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.3.1/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -738,15 +738,15 @@
         title='Sourceapp',
     )
     createdAt: Optional[datetime] = Field(
         default=None,
         description='The date (in ISO 8601 format) that the asset was created\n',
         title='Createdat',
     )
-    lastUsedAt: Optional[str] = Field(
+    lastUsedAt: Optional[datetime] = Field(
         default=None,
         description='The date (in ISO 8601 format) of the last time that the asset was in use.',
         title='Lastusedat',
     )
     href: Optional[str] = Field(
         default=None,
         description='A link to the asset in the source application',
@@ -1019,14 +1019,34 @@
     )
     id: str = Field(..., description='Unique ID', title='Id')
     user: Optional[UserSchema] = Field(
         default=None, description='User Schema of the reviewer', title='User'
     )
 
 
+class SearchAssetsFilterBody(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    originId: Optional[OriginIdFilter] = Field(
+        default=None, description='Find assets by their origin ID', title='Originid'
+    )
+    appId: Optional[AppIdFilter] = Field(
+        default=None, description='Find assets by their app ID', title='Appid'
+    )
+    uniqueId: Optional[UniqueIdFilter] = Field(
+        default=None, description='Find assets by their unique ID', title='Uniqueid'
+    )
+    authomizeId: Optional[AssetIdFilter] = Field(
+        default=None,
+        description='Find assets by their Authomize ID',
+        title='Authomizeid',
+    )
+
+
 class SearchAssetsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     sort: Optional[List[SortSchemaSearchAssetsSortFields]] = Field(
         default=None,
         description="Sort the results by asset's name in ascending or descending order",
@@ -1076,14 +1096,34 @@
     sort: Optional[List[SortSchemaFieldName]] = Field(
         default=None,
         description='Sort the results by campaign fields in ascending or descending order',
         title='Sort',
     )
 
 
+class SearchGroupsFilterBody(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    uniqueId: Optional[SearchGroupsUniqueIdFilter] = Field(
+        default=None, description='Find groups by their unique ID', title='Uniqueid'
+    )
+    originId: Optional[SearchGroupsOriginIdFilter] = Field(
+        default=None, description='Find groups by their origin ID', title='Originid'
+    )
+    appId: Optional[SearchGroupsAppIdFilter] = Field(
+        default=None, description='Find groups by their app ID', title='Appid'
+    )
+    authomizeId: Optional[SearchGroupsIdFilter] = Field(
+        default=None,
+        description='Find groups by their Authomize ID',
+        title='Authomizeid',
+    )
+
+
 class SearchGroupsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     sort: Optional[List[SortSchemaSearchGroupsSortFields]] = Field(
         default=None,
         description="Sort the results by group's name in ascending or descending order",
```

### Comparing `authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.3.1/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999996709020147%*

 * *Differences: {"'components'": "{'schemas': {'AssetSchema': {'properties': {'lastUsedAt': {'format': "*

 * *                 "'date-time'}}}, 'SearchGroupsRequestSchema': {'properties': {'sort': "*

 * *                 "{'description': 'Sort the results by identity name in ascending or descending "*

 * *                 "order'}}}}}"}*

```diff
@@ -281,14 +281,15 @@
                     "incidentsCount": {
                         "description": "Number of associated incidents",
                         "title": "Incidentscount",
                         "type": "integer"
                     },
                     "lastUsedAt": {
                         "description": "The date (in ISO 8601 format) of the last time that the asset was in use.",
+                        "format": "date-time",
                         "title": "Lastusedat",
                         "type": "string"
                     },
                     "name": {
                         "description": "Name of the asset (for example, application, virtual machine, file, etc.)",
                         "title": "Name",
                         "type": "string"
@@ -2186,15 +2187,15 @@
                                 "$ref": "#/components/schemas/PaginationRequestSchema"
                             }
                         ],
                         "description": "Pagination metadata",
                         "title": "Pagination"
                     },
                     "sort": {
-                        "description": "Sort the results by group's name in ascending or descending order",
+                        "description": "Sort the results by identity name in ascending or descending order",
                         "items": {
                             "$ref": "#/components/schemas/SortSchema_SearchGroupsSortFields_"
                         },
                         "title": "Sort",
                         "type": "array"
                     }
                 },
```

### Comparing `authomize-rest-api-client-4.3.0/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.3.1/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.0/setup.py` & `authomize-rest-api-client-4.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.3.0',
+        version='4.3.1',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

