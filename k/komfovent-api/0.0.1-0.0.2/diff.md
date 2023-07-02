# Comparing `tmp/komfovent-api-0.0.1.tar.gz` & `tmp/komfovent-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komfovent-api-0.0.1.tar", last modified: Sun Jul  2 14:48:12 2023, max compression
+gzip compressed data, was "komfovent-api-0.0.2.tar", last modified: Sun Jul  2 15:56:20 2023, max compression
```

## Comparing `komfovent-api-0.0.1.tar` & `komfovent-api-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-07-02 14:48:12.113266 komfovent-api-0.0.1/
--rw-r--r--   0 alex       (502) staff       (20)    10762 2023-07-02 07:26:53.000000 komfovent-api-0.0.1/LICENSE
--rw-r--r--   0 alex       (502) staff       (20)     1137 2023-07-02 14:48:12.113123 komfovent-api-0.0.1/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)      421 2023-07-02 14:43:54.000000 komfovent-api-0.0.1/README.md
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-07-02 14:48:12.112194 komfovent-api-0.0.1/komfovent_api/
--rw-r--r--   0 alex       (502) staff       (20)      242 2023-07-02 14:26:38.000000 komfovent-api-0.0.1/komfovent_api/__init__.py
--rw-r--r--   0 alex       (502) staff       (20)     2436 2023-07-02 14:26:00.000000 komfovent-api-0.0.1/komfovent_api/api.py
--rw-r--r--   0 alex       (502) staff       (20)     1077 2023-07-02 14:20:07.000000 komfovent-api-0.0.1/komfovent_api/classes.py
--rw-r--r--   0 alex       (502) staff       (20)     1334 2023-07-02 14:22:57.000000 komfovent-api-0.0.1/komfovent_api/networking.py
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-07-02 14:48:12.112922 komfovent-api-0.0.1/komfovent_api.egg-info/
--rw-r--r--   0 alex       (502) staff       (20)     1137 2023-07-02 14:48:12.000000 komfovent-api-0.0.1/komfovent_api.egg-info/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)      316 2023-07-02 14:48:12.000000 komfovent-api-0.0.1/komfovent_api.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (502) staff       (20)        1 2023-07-02 14:48:12.000000 komfovent-api-0.0.1/komfovent_api.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (502) staff       (20)       13 2023-07-02 14:48:12.000000 komfovent-api-0.0.1/komfovent_api.egg-info/requires.txt
--rw-r--r--   0 alex       (502) staff       (20)       14 2023-07-02 14:48:12.000000 komfovent-api-0.0.1/komfovent_api.egg-info/top_level.txt
--rw-r--r--   0 alex       (502) staff       (20)      896 2023-07-02 12:08:41.000000 komfovent-api-0.0.1/pyproject.toml
--rw-r--r--   0 alex       (502) staff       (20)       38 2023-07-02 14:48:12.113314 komfovent-api-0.0.1/setup.cfg
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-07-02 15:56:20.205611 komfovent-api-0.0.2/
+-rw-r--r--   0 alex       (502) staff       (20)    10762 2023-07-02 07:26:53.000000 komfovent-api-0.0.2/LICENSE
+-rw-r--r--   0 alex       (502) staff       (20)     1137 2023-07-02 15:56:20.205484 komfovent-api-0.0.2/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)      421 2023-07-02 14:43:54.000000 komfovent-api-0.0.2/README.md
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-07-02 15:56:20.204466 komfovent-api-0.0.2/komfovent_api/
+-rw-r--r--   0 alex       (502) staff       (20)      276 2023-07-02 15:55:36.000000 komfovent-api-0.0.2/komfovent_api/__init__.py
+-rw-r--r--   0 alex       (502) staff       (20)     2439 2023-07-02 15:55:22.000000 komfovent-api-0.0.2/komfovent_api/api.py
+-rw-r--r--   0 alex       (502) staff       (20)     1078 2023-07-02 15:55:22.000000 komfovent-api-0.0.2/komfovent_api/classes.py
+-rw-r--r--   0 alex       (502) staff       (20)     1334 2023-07-02 14:22:57.000000 komfovent-api-0.0.2/komfovent_api/networking.py
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-07-02 15:56:20.205279 komfovent-api-0.0.2/komfovent_api.egg-info/
+-rw-r--r--   0 alex       (502) staff       (20)     1137 2023-07-02 15:56:20.000000 komfovent-api-0.0.2/komfovent_api.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)      316 2023-07-02 15:56:20.000000 komfovent-api-0.0.2/komfovent_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (502) staff       (20)        1 2023-07-02 15:56:20.000000 komfovent-api-0.0.2/komfovent_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (502) staff       (20)       13 2023-07-02 15:56:20.000000 komfovent-api-0.0.2/komfovent_api.egg-info/requires.txt
+-rw-r--r--   0 alex       (502) staff       (20)       14 2023-07-02 15:56:20.000000 komfovent-api-0.0.2/komfovent_api.egg-info/top_level.txt
+-rw-r--r--   0 alex       (502) staff       (20)      896 2023-07-02 15:55:48.000000 komfovent-api-0.0.2/pyproject.toml
+-rw-r--r--   0 alex       (502) staff       (20)       38 2023-07-02 15:56:20.205664 komfovent-api-0.0.2/setup.cfg
```

### Comparing `komfovent-api-0.0.1/LICENSE` & `komfovent-api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `komfovent-api-0.0.1/PKG-INFO` & `komfovent-api-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komfovent-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Implementing Komfovent C6 API in python
 Author-email: Aleksandr Tsernoh <foralwork@gmail.com>
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ProstoSanja/komfovent-api-python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
```

### Comparing `komfovent-api-0.0.1/komfovent_api/api.py` & `komfovent-api-0.0.2/komfovent_api/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,27 @@
         return (KomfoventConnectionResult.INVALID_INPUT, None)
 
 def __string_to_float(input: str) -> float:
     return float(''.join(c for c in input if c.isdigit() or c == '.'))
 
 # check_settings
 
-async def get_settings(creds: KomfoventCredentials) -> tuple[KomfoventConnectionResult, KomfoventSettins]:
+async def get_settings(creds: KomfoventCredentials) -> tuple[KomfoventConnectionResult, KomfoventSettings]:
     status, response = await request("/st.html", creds)
     if (status != KomfoventConnectionResult.SUCCESS):
         return (status, None)
     return (status, __parse_settings(response))
 
-def __parse_settings(data: str) -> KomfoventSettins:
+def __parse_settings(data: str) -> KomfoventSettings:
     root = LX.fromstring(data)
     name = root.xpath("//input[@name='204']")[0].value.strip()
     model = root.find_class("hide_cfg")[0].xpath("input")[0].value.strip()
     version = root.get_element_by_id("mmf1").value.strip()
     serial_number = root.get_element_by_id("c6sn").value.strip()
-    return KomfoventSettins(name, model, version, serial_number)
+    return KomfoventSettings(name, model, version, serial_number)
 
 # get_unit_status
 
 async def get_unit_status(creds: KomfoventCredentials) -> tuple[KomfoventConnectionResult, KomfoventUnit]:
     status, response = await request("/i.asp", creds)
     if (status != KomfoventConnectionResult.SUCCESS):
         return (status, None)
```

### Comparing `komfovent-api-0.0.1/komfovent_api/classes.py` & `komfovent-api-0.0.2/komfovent_api/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     AWAY = 1
     NORMAL = 2
     INTENSIVE = 3
     BOOST = 4
 
 
 @dataclass
-class KomfoventSettins():
+class KomfoventSettings():
     name: str
     model: str
     version: str
     serial_number: str
 
 
 @dataclass
```

### Comparing `komfovent-api-0.0.1/komfovent_api/networking.py` & `komfovent-api-0.0.2/komfovent_api/networking.py`

 * *Files identical despite different names*

### Comparing `komfovent-api-0.0.1/komfovent_api.egg-info/PKG-INFO` & `komfovent-api-0.0.2/komfovent_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komfovent-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: Implementing Komfovent C6 API in python
 Author-email: Aleksandr Tsernoh <foralwork@gmail.com>
 License: Apache-2.0
 Project-URL: Repository, https://github.com/ProstoSanja/komfovent-api-python
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
```

### Comparing `komfovent-api-0.0.1/pyproject.toml` & `komfovent-api-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "komfovent-api"
-version = "0.0.1"
+version = "0.0.2"
 license = {text = "Apache-2.0"}
 description = "Implementing Komfovent C6 API in python"
 readme = {file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.10"
 authors = [
     {name = "Aleksandr Tsernoh", email = "foralwork@gmail.com"}
 ]
```

