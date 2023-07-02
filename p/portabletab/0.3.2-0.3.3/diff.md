# Comparing `tmp/portabletab-0.3.2.tar.gz` & `tmp/portabletab-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portabletab-0.3.2.tar", max compression
+gzip compressed data, was "portabletab-0.3.3.tar", max compression
```

## Comparing `portabletab-0.3.2.tar` & `portabletab-0.3.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-04-01 08:14:02.000000 portabletab-0.3.2/LICENSE
--rw-r--r--   0        0        0      203 2023-04-29 09:02:48.188411 portabletab-0.3.2/PortableTab/__init__.py
--rw-r--r--   0        0        0     4861 2023-04-29 09:02:43.908411 portabletab-0.3.2/PortableTab/__main__.py
--rw-r--r--   0        0        0     1917 2023-04-05 12:03:54.000000 portabletab-0.3.2/PortableTab/base_table.py
--rw-r--r--   0        0        0     4697 2023-04-29 09:02:48.188411 portabletab-0.3.2/PortableTab/capnp_manager.py
--rw-r--r--   0        0        0    18486 2023-04-29 09:02:48.188411 portabletab-0.3.2/PortableTab/capnp_table.py
--rw-r--r--   0        0        0      155 2023-04-29 09:02:43.908411 portabletab-0.3.2/PortableTab/exceptions.py
--rw-r--r--   0        0        0     1837 2023-04-09 02:51:51.000000 portabletab-0.3.2/README.md
--rw-r--r--   0        0        0      634 2023-04-29 09:02:48.188411 portabletab-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 portabletab-0.3.2/setup.py
--rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 portabletab-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-03-23 04:47:41.138638 portabletab-0.3.3/LICENSE
+-rw-r--r--   0        0        0      203 2023-07-02 08:12:40.637313 portabletab-0.3.3/PortableTab/__init__.py
+-rw-r--r--   0        0        0     4861 2023-04-11 03:07:38.494545 portabletab-0.3.3/PortableTab/__main__.py
+-rw-r--r--   0        0        0     1917 2023-04-04 07:41:11.567861 portabletab-0.3.3/PortableTab/base_table.py
+-rw-r--r--   0        0        0     4697 2023-07-02 08:10:59.976983 portabletab-0.3.3/PortableTab/capnp_manager.py
+-rw-r--r--   0        0        0    18443 2023-07-02 08:09:44.284891 portabletab-0.3.3/PortableTab/capnp_table.py
+-rw-r--r--   0        0        0      155 2023-04-11 03:07:38.498545 portabletab-0.3.3/PortableTab/exceptions.py
+-rw-r--r--   0        0        0     1837 2023-04-11 03:07:29.170336 portabletab-0.3.3/README.md
+-rw-r--r--   0        0        0      634 2023-07-02 08:12:36.821296 portabletab-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 portabletab-0.3.3/PKG-INFO
```

### Comparing `portabletab-0.3.2/LICENSE` & `portabletab-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.2/PortableTab/__main__.py` & `portabletab-0.3.3/PortableTab/__main__.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.2/PortableTab/base_table.py` & `portabletab-0.3.3/PortableTab/base_table.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.2/PortableTab/capnp_manager.py` & `portabletab-0.3.3/PortableTab/capnp_manager.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.2/PortableTab/capnp_table.py` & `portabletab-0.3.3/PortableTab/capnp_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,17 +92,16 @@
         Notes
         -----
         - This method is automatically called when needed.
           There is no need to call it explicitly from the user program.
         """
         config = self.get_config()
         module_name = config["module_name"]
-        logger.debug(f"module_name: '{module_name}")
-        if module_name not in CapnpManager.modules:
-            logger.debug(f"{module_name} is not in modules, loading schema.")
+        if module_name not in CapnpManager.modules or \
+                CapnpManager.modules[module_name] is None:
             CapnpManager.load_schema(
                 self.get_dir() / config["capnp_file"],
                 module_name)
 
     @lru_cache(maxsize=128)
     def get_record_type(self) -> Any:
         """
@@ -269,15 +268,15 @@
                 "module_name": self.tablename,
                 "record_type": record_type,
                 "list_type": list_type,
                 "count": 0
             }, fp=f)
 
         # Load this schema once and generate the ID automatically.
-        self._load_capnp_file()
+        CapnpManager.load_schema(copied, self.tablename)
 
         return table_dir
 
     def get_record(
             self,
             pos: int,
             as_dict: bool = False) -> Any:
```

### Comparing `portabletab-0.3.2/README.md` & `portabletab-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.2/pyproject.toml` & `portabletab-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PortableTab"
-version = "0.3.2"
+version = "0.3.3"
 description = "Python package for serializing tables in portable format with Capnp."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "PortableTab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `portabletab-0.3.2/setup.py` & `portabletab-0.3.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,73 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: portabletab
+Version: 0.3.3
+Summary: Python package for serializing tables in portable format with Capnp.
+License: MIT
+Author: Takeshi Sagara
+Author-email: sagara@info-proto.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: docopt (>=0.6.2,<0.7.0)
+Requires-Dist: marisa-trie (>=0.7.8,<0.8.0)
+Requires-Dist: pycapnp (>=1.3.0,<2.0.0)
+Description-Content-Type: text/markdown
+
+# PortableTab
+
+*PortableTab* is a Python library that allows for serialization of 
+typed tables into a set of files, as well as deserialization of
+specific rows extracted from the files.
+
+## Features
+
+The serialized files are independent of OS and CPU architecture, so it can
+be used to create portable table which is useful when working with large
+datasets that need to be shared between different systems or environments.
+
+It also allows fast deserialization of only specified rows without loading
+the entire table into memory, so it does not take time to load and
+deserialize the table on the first access, nor consume memory during execution.
+
+- [Capn' Proto](https://capnproto.org/) is used for serialization,
+  making the file format portable.
+- Since *PortableTab* uses mmap for file access, it does not consume
+  much memory even when handling large tables.
+- Indexes on strings are created using
+  [Marisa-trie](https://github.com/pytries/marisa-trie),
+  the output files are also portable and accessible using mmap.
+
+## Limitations
+
+The tables are serialized into compact files so they cannot be dynamically
+modified.
+
+- Rows can only be retrieved at their specified position. If you want to
+  access by an attribute such as *id*, you must create an index on that attribute.
+- Updating records in serialized files is possible but very slow.
+- It is not possible to insert rows in the middle of a serialized file. If you
+  want to insert rows in the middle, the only way is to deserialize
+  the entire table and recreate another table.
+
+## How to use
+
+Please refer to the documentation at
+[PortableTab Document](https://portabletab.readthedocs.io/en/latest/).
+
+## Development status
+
+Unstable alpha version.
 
-packages = \
-['PortableTab']
+## License
 
-package_data = \
-{'': ['*']}
+This package is available according to the MIT license.
 
-install_requires = \
-['docopt>=0.6.2,<0.7.0', 'marisa-trie>=0.7.8,<0.8.0', 'pycapnp>=1.3.0,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['portabletab = PortableTab.__main__:main']}
-
-setup_kwargs = {
-    'name': 'portabletab',
-    'version': '0.3.2',
-    'description': 'Python package for serializing tables in portable format with Capnp.',
-    'long_description': "# PortableTab\n\n*PortableTab* is a Python library that allows for serialization of \ntyped tables into a set of files, as well as deserialization of\nspecific rows extracted from the files.\n\n## Features\n\nThe serialized files are independent of OS and CPU architecture, so it can\nbe used to create portable table which is useful when working with large\ndatasets that need to be shared between different systems or environments.\n\nIt also allows fast deserialization of only specified rows without loading\nthe entire table into memory, so it does not take time to load and\ndeserialize the table on the first access, nor consume memory during execution.\n\n- [Capn' Proto](https://capnproto.org/) is used for serialization,\n  making the file format portable.\n- Since *PortableTab* uses mmap for file access, it does not consume\n  much memory even when handling large tables.\n- Indexes on strings are created using\n  [Marisa-trie](https://github.com/pytries/marisa-trie),\n  the output files are also portable and accessible using mmap.\n\n## Limitations\n\nThe tables are serialized into compact files so they cannot be dynamically\nmodified.\n\n- Rows can only be retrieved at their specified position. If you want to\n  access by an attribute such as *id*, you must create an index on that attribute.\n- Updating records in serialized files is possible but very slow.\n- It is not possible to insert rows in the middle of a serialized file. If you\n  want to insert rows in the middle, the only way is to deserialize\n  the entire table and recreate another table.\n\n## How to use\n\nPlease refer to the documentation at\n[PortableTab Document](https://portabletab.readthedocs.io/en/latest/).\n\n## Development status\n\nUnstable alpha version.\n\n## License\n\nThis package is available according to the MIT license.\n\n## Author\n\nTakeshi SAGARA <sagara@info-proto.com>\n",
-    'author': 'Takeshi Sagara',
-    'author_email': 'sagara@info-proto.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+## Author
 
+Takeshi SAGARA <sagara@info-proto.com>
 
-setup(**setup_kwargs)
```

