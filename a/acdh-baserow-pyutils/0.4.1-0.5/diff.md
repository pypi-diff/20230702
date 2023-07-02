# Comparing `tmp/acdh_baserow_pyutils-0.4.1.tar.gz` & `tmp/acdh_baserow_pyutils-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdh_baserow_pyutils-0.4.1.tar", last modified: Thu Feb 23 10:45:56 2023, max compression
+gzip compressed data, was "acdh_baserow_pyutils-0.5.tar", last modified: Sun Jul  2 11:06:55 2023, max compression
```

## Comparing `acdh_baserow_pyutils-0.4.1.tar` & `acdh_baserow_pyutils-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:45:56.989848 acdh_baserow_pyutils-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-02-23 10:45:30.000000 acdh_baserow_pyutils-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-02-23 10:45:56.989848 acdh_baserow_pyutils-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-23 10:45:30.000000 acdh_baserow_pyutils-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:45:56.989848 acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils/
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-02-23 10:45:30.000000 acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:45:56.989848 acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-02-23 10:45:56.000000 acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-23 10:45:56.000000 acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 10:45:56.000000 acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 10:45:56.000000 acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-23 10:45:56.000000 acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 10:45:56.000000 acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 10:45:56.989848 acdh_baserow_pyutils-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-02-23 10:45:30.000000 acdh_baserow_pyutils-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:06:55.707196 acdh_baserow_pyutils-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-02 11:06:43.000000 acdh_baserow_pyutils-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-02 11:06:55.707196 acdh_baserow_pyutils-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-02 11:06:43.000000 acdh_baserow_pyutils-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:06:55.707196 acdh_baserow_pyutils-0.5/acdh_baserow_pyutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-02 11:06:43.000000 acdh_baserow_pyutils-0.5/acdh_baserow_pyutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:06:55.707196 acdh_baserow_pyutils-0.5/acdh_baserow_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-02 11:06:55.000000 acdh_baserow_pyutils-0.5/acdh_baserow_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-02 11:06:55.000000 acdh_baserow_pyutils-0.5/acdh_baserow_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 11:06:55.000000 acdh_baserow_pyutils-0.5/acdh_baserow_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 11:06:55.000000 acdh_baserow_pyutils-0.5/acdh_baserow_pyutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 11:06:55.000000 acdh_baserow_pyutils-0.5/acdh_baserow_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-02 11:06:55.000000 acdh_baserow_pyutils-0.5/acdh_baserow_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 11:06:55.707196 acdh_baserow_pyutils-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-02 11:06:44.000000 acdh_baserow_pyutils-0.5/setup.py
```

### Comparing `acdh_baserow_pyutils-0.4.1/LICENSE` & `acdh_baserow_pyutils-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `acdh_baserow_pyutils-0.4.1/PKG-INFO` & `acdh_baserow_pyutils-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh_baserow_pyutils
-Version: 0.4.1
+Version: 0.5
 Summary: Utility functions to work with Baserow
 Home-page: https://github.com/acdh-oeaw/acdh-baserow-pyutils
 Author: Peter Andorfer
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `acdh_baserow_pyutils-0.4.1/README.md` & `acdh_baserow_pyutils-0.5/README.md`

 * *Files identical despite different names*

### Comparing `acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils/__init__.py` & `acdh_baserow_pyutils-0.5/acdh_baserow_pyutils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,22 @@
     def list_tables(self, br_database_id):
         db_url = f"{self.br_base_url}database/tables/database/{br_database_id}/"
         r = requests.get(
             url=db_url, headers={"Authorization": f"JWT {self.br_jwt_token}"}
         )
         return r.json()
 
+    def get_table_by_name(self, br_database_id, br_table_name):
+        tables = self.list_tables(br_database_id)
+        table_id = False
+        for x in tables:
+            if x["name"] == br_table_name:
+                table_id = str(x["id"])
+        return table_id
+
     def list_fields(self, br_table_id):
         url = f"{self.br_base_url}database/fields/table/{br_table_id}/"
         r = requests.get(url, headers={"Authorization": f"JWT {self.br_jwt_token}"})
         return r.json()
 
     def search_rows(self, br_table_id, q, query_field_id, lookup_type="contains"):
         url = f"{self.br_base_url}database/rows/table/{br_table_id}/?user_field_names=true&filter__field_{query_field_id}__{lookup_type}={q}"  # noqa
```

### Comparing `acdh_baserow_pyutils-0.4.1/acdh_baserow_pyutils.egg-info/PKG-INFO` & `acdh_baserow_pyutils-0.5/acdh_baserow_pyutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh-baserow-pyutils
-Version: 0.4.1
+Version: 0.5
 Summary: Utility functions to work with Baserow
 Home-page: https://github.com/acdh-oeaw/acdh-baserow-pyutils
 Author: Peter Andorfer
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT license
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `acdh_baserow_pyutils-0.4.1/setup.py` & `acdh_baserow_pyutils-0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,10 +34,10 @@
     include_package_data=True,
     name="acdh_baserow_pyutils",
     packages=find_packages(include=["acdh_baserow_pyutils", "acdh_baserow_pyutils.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/acdh-oeaw/acdh-baserow-pyutils",
-    version="v0.4.1",
+    version="v0.5",
     zip_safe=False,
 )
```

