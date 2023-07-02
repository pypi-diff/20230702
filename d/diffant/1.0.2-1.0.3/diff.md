# Comparing `tmp/diffant-1.0.2.tar.gz` & `tmp/diffant-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffant-1.0.2.tar", max compression
+gzip compressed data, was "diffant-1.0.3.tar", max compression
```

## Comparing `diffant-1.0.2.tar` & `diffant-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-06-30 14:30:46.195418 diffant-1.0.2/LICENSE
--rw-r--r--   0        0        0     4187 2023-06-30 23:33:01.963065 diffant-1.0.2/README.md
--rw-r--r--   0        0        0      169 2023-06-23 14:54:16.052445 diffant-1.0.2/diffant/__init__.py
--rw-r--r--   0        0        0    13780 2023-06-30 15:57:50.187364 diffant-1.0.2/diffant/diffabc.py
--rw-r--r--   0        0        0     1072 2023-06-29 17:56:20.082459 diffant-1.0.2/diffant/diffini.py
--rw-r--r--   0        0        0     1121 2023-06-28 21:48:02.247536 diffant-1.0.2/diffant/diffjson.py
--rw-r--r--   0        0        0     2141 2023-06-28 23:00:39.610174 diffant-1.0.2/diffant/diffxml.py
--rw-r--r--   0        0        0     1132 2023-06-29 17:31:32.565365 diffant-1.0.2/diffant/diffyml.py
--rw-r--r--   0        0        0      655 2023-06-30 16:01:07.110238 diffant-1.0.2/diffant/exceptions.py
--rw-r--r--   0        0        0     4246 2023-06-30 16:00:12.361435 diffant-1.0.2/diffant/main.py
--rw-r--r--   0        0        0     2553 2023-06-27 21:11:06.231309 diffant-1.0.2/diffant/nested.py
--rw-r--r--   0        0        0     1435 2023-06-30 22:36:14.881070 diffant-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 diffant-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-30 14:30:46.195418 diffant-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4187 2023-06-30 23:33:01.963065 diffant-1.0.3/README.md
+-rw-r--r--   0        0        0      169 2023-06-23 14:54:16.052445 diffant-1.0.3/diffant/__init__.py
+-rw-r--r--   0        0        0    13780 2023-06-30 15:57:50.187364 diffant-1.0.3/diffant/diffabc.py
+-rw-r--r--   0        0        0     1072 2023-06-29 17:56:20.082459 diffant-1.0.3/diffant/diffini.py
+-rw-r--r--   0        0        0     1121 2023-06-28 21:48:02.247536 diffant-1.0.3/diffant/diffjson.py
+-rw-r--r--   0        0        0     1151 2023-07-02 00:44:34.140759 diffant-1.0.3/diffant/diffxml.py
+-rw-r--r--   0        0        0     1132 2023-06-29 17:31:32.565365 diffant-1.0.3/diffant/diffyml.py
+-rw-r--r--   0        0        0      655 2023-06-30 16:01:07.110238 diffant-1.0.3/diffant/exceptions.py
+-rw-r--r--   0        0        0     4331 2023-07-02 00:44:34.144759 diffant-1.0.3/diffant/main.py
+-rw-r--r--   0        0        0     2553 2023-06-27 21:11:06.231309 diffant-1.0.3/diffant/nested.py
+-rw-r--r--   0        0        0     1485 2023-07-02 00:44:34.144759 diffant-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5149 1970-01-01 00:00:00.000000 diffant-1.0.3/PKG-INFO
```

### Comparing `diffant-1.0.2/LICENSE` & `diffant-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `diffant-1.0.2/README.md` & `diffant-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `diffant-1.0.2/diffant/diffabc.py` & `diffant-1.0.3/diffant/diffabc.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.2/diffant/diffini.py` & `diffant-1.0.3/diffant/diffini.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.2/diffant/diffjson.py` & `diffant-1.0.3/diffant/diffjson.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.2/diffant/diffyml.py` & `diffant-1.0.3/diffant/diffyml.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.2/diffant/exceptions.py` & `diffant-1.0.3/diffant/exceptions.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.2/diffant/main.py` & `diffant-1.0.3/diffant/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 from pathlib import Path
 from typing import Dict, Type
 
 from diffant import exceptions
 from diffant.diffabc import DiffABC
 from diffant.diffini import DiffIni
 from diffant.diffjson import DiffJson
+from diffant.diffxml import DiffXML
 from diffant.diffyml import DiffYML
 
 # map file types: 'ini' to class to process that type: IniDiff
 DIFF_MAPPING: Dict[str, Type[DiffABC]] = {
     "ini": DiffIni,
     "json": DiffJson,
+    "xml": DiffXML,
     "yml": DiffYML,
 }
 
 
 def main() -> bool:
     """main as is tradition
 
@@ -51,15 +53,16 @@
         str: The input directory.
 
     Raises:
         FileNotFoundError: If the supplied directory does not exist.
         NotADirectoryError: If the supplied path is not a directory.
         SystemExit (via argparse): If the required argument is not provided.
     """
-    parser = argparse.ArgumentParser(description="JSON file comparison tool.")
+    msg = "json, xml, yaml, ini file comparison tool."
+    parser = argparse.ArgumentParser(description=msg)
     parser.add_argument(
         "input_dir",
         type=str,
         help="Path to dir containing config files of the same type.",
     )
 
     args = parser.parse_args()
@@ -116,15 +119,15 @@
 
     extension = next(iter(file_extensions))  # Get the first and only item from the set
 
     return str(extension[1:])  # remove the leading dot from the extension
 
 
 def create_differ(mapping: Dict[str, Type[DiffABC]], file_type: str) -> DiffABC:
-    """ Return the Diff class we want to instanciate.
+    """Return the Diff class we want to instanciate.
 
     Args:
         mapping (Dict): map file type strings to Diff* classes
         file_type (str): extension / file type examples: 'json', 'ini'
 
     Raises:
         exceptions.InputDirContentsError:
```

### Comparing `diffant-1.0.2/diffant/nested.py` & `diffant-1.0.3/diffant/nested.py`

 * *Files identical despite different names*

### Comparing `diffant-1.0.2/pyproject.toml` & `diffant-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "diffant"
-version = "1.0.2"
+version = "1.0.3"
 description = "tool to compare structured files like json, ini , yaml"
 authors = ["omacneil <dan@omacneil.org>"]
 license = "GPL-3.0-or-later"
 readme  = "README.md"
 homepage = "https://github.com/omacneil/diffant"
 repository = "https://github.com/omacneil/diffant"
 keywords = ["json", "yaml","ini","diff","configuration","compare"]
@@ -16,14 +16,16 @@
         'Programming Language :: Python :: 3.12',
     ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 pyyaml = "6.0"
 types-pyyaml = "6.0.12.10"
+xmltodict = "0.13.0"
+types-xmltodict = "0.13.0.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 coverage = "7.2.5"
 flake8 = "6.0.0"
 isort = "5.12.0"
 mypy = "1.3.0"
```

### Comparing `diffant-1.0.2/PKG-INFO` & `diffant-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffant
-Version: 1.0.2
+Version: 1.0.3
 Summary: tool to compare structured files like json, ini , yaml
 Home-page: https://github.com/omacneil/diffant
 License: GPL-3.0-or-later
 Keywords: json,yaml,ini,diff,configuration,compare
 Author: omacneil
 Author-email: dan@omacneil.org
 Requires-Python: >=3.8.1,<4.0.0
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: pyyaml (==6.0)
 Requires-Dist: types-pyyaml (==6.0.12.10)
+Requires-Dist: types-xmltodict (==0.13.0.2)
+Requires-Dist: xmltodict (==0.13.0)
 Project-URL: Repository, https://github.com/omacneil/diffant
 Description-Content-Type: text/markdown
 
 # `diffant`
 `diffant` uses the structure of configuration files to do a more helpful comparison than standard diff.
 
 `diffant` allows you to compare:
```

