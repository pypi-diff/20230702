# Comparing `tmp/PyObfuscator-0.1.1.tar.gz` & `tmp/PyObfuscator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyObfuscator-0.1.1.tar", last modified: Sun Mar 19 21:58:11 2023, max compression
+gzip compressed data, was "PyObfuscator-0.1.2.tar", last modified: Sun Jul  2 17:55:32 2023, max compression
```

## Comparing `PyObfuscator-0.1.1.tar` & `PyObfuscator-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-03-19 21:58:11.388605 PyObfuscator-0.1.1/
--rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       72 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     8902 2023-03-19 21:58:11.388605 PyObfuscator-0.1.1/PKG-INFO
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-03-19 21:58:11.384603 PyObfuscator-0.1.1/PyObfuscator.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     8902 2023-03-19 21:58:11.000000 PyObfuscator-0.1.1/PyObfuscator.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      530 2023-03-19 21:58:11.000000 PyObfuscator-0.1.1/PyObfuscator.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-03-19 21:58:11.000000 PyObfuscator-0.1.1/PyObfuscator.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-03-19 21:58:11.000000 PyObfuscator-0.1.1/PyObfuscator.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-03-19 21:58:11.000000 PyObfuscator-0.1.1/PyObfuscator.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    39328 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/PyObfuscator.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7804 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-03-19 21:58:11.388605 PyObfuscator-0.1.1/examples/
--rw-r--r--   0 kali      (1000) kali      (1000)       12 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/other.py
--rw-r--r--   0 kali      (1000) kali      (1000)       14 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/other2.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2728 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/test.py
--rw-r--r--   0 kali      (1000) kali      (1000)      363 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/test_import.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8001 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/test_import_level2.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15161 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/test_level1.py
--rw-r--r--   0 kali      (1000) kali      (1000)    45994 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/test_level2.py
--rw-r--r--   0 kali      (1000) kali      (1000)    21269 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/test_level3.py
--rw-r--r--   0 kali      (1000) kali      (1000)    97236 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/test_level4.py
--rw-r--r--   0 kali      (1000) kali      (1000)   120121 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/test_level5.py
--rw-r--r--   0 kali      (1000) kali      (1000)   485904 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/examples/test_level6.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-03-19 21:58:11.388605 PyObfuscator-0.1.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1633 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-03-19 21:58:11.388605 PyObfuscator-0.1.1/tests/
--rw-r--r--   0 kali      (1000) kali      (1000)    42060 2023-03-19 21:48:31.000000 PyObfuscator-0.1.1/tests/TestPyObfuscator.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35821 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       72 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     8902 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/PKG-INFO
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/PyObfuscator.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     8902 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      520 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       51 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-02 17:55:31.000000 PyObfuscator-0.1.2/PyObfuscator.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    40617 2023-07-02 17:42:10.000000 PyObfuscator-0.1.2/PyObfuscator.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7804 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/examples/
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/examples/other.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/examples/other2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3220 2023-07-02 17:34:38.000000 PyObfuscator-0.1.2/examples/test.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      380 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/examples/test_import.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    14243 2023-07-02 17:44:28.000000 PyObfuscator-0.1.2/examples/test_import_level2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    15561 2023-07-02 17:41:22.000000 PyObfuscator-0.1.2/examples/test_level1.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    88954 2023-07-02 17:35:40.000000 PyObfuscator-0.1.2/examples/test_level2.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    54463 2023-07-02 17:35:46.000000 PyObfuscator-0.1.2/examples/test_level3.py
+-rw-r--r--   0 kali      (1000) kali      (1000)   250704 2023-07-02 17:35:52.000000 PyObfuscator-0.1.2/examples/test_level4.py
+-rw-r--r--   0 kali      (1000) kali      (1000)   316806 2023-07-02 17:35:58.000000 PyObfuscator-0.1.2/examples/test_level5.py
+-rw-r--r--   0 kali      (1000) kali      (1000)  1270388 2023-07-02 17:36:04.000000 PyObfuscator-0.1.2/examples/test_level6.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1633 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-02 17:55:32.056936 PyObfuscator-0.1.2/tests/
+-rw-r--r--   0 kali      (1000) kali      (1000)    43367 2023-07-02 09:32:18.000000 PyObfuscator-0.1.2/tests/TestPyObfuscator.py
```

### Comparing `PyObfuscator-0.1.1/LICENSE.txt` & `PyObfuscator-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.1/PKG-INFO` & `PyObfuscator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyObfuscator
-Version: 0.1.1
+Version: 0.1.2
 Summary: This module obfuscates python code.
 Home-page: https://github.com/mauricelambert/PyObfuscator/
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PyObfuscator-0.1.1/PyObfuscator.egg-info/PKG-INFO` & `PyObfuscator-0.1.2/PyObfuscator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyObfuscator
-Version: 0.1.1
+Version: 0.1.2
 Summary: This module obfuscates python code.
 Home-page: https://github.com/mauricelambert/PyObfuscator/
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PyObfuscator-0.1.1/PyObfuscator.egg-info/SOURCES.txt` & `PyObfuscator-0.1.2/PyObfuscator.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 PyObfuscator.py
 README.md
-setup.cfg
 setup.py
 PyObfuscator.egg-info/PKG-INFO
 PyObfuscator.egg-info/SOURCES.txt
 PyObfuscator.egg-info/dependency_links.txt
 PyObfuscator.egg-info/entry_points.txt
 PyObfuscator.egg-info/top_level.txt
 examples/other.py
```

### Comparing `PyObfuscator-0.1.1/PyObfuscator.py` & `PyObfuscator-0.1.2/PyObfuscator.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     -----------------------------------------------
     TOTAL                         400      1    99%
 
 """
 
 default_dir = dir()
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = "This module obfuscates python code."
 license = "GPL-3.0 License"
 __url__ = "https://github.com/mauricelambert/PyObfuscator/"
@@ -101,23 +101,23 @@
     alias,
     arg,
     parse,
     unparse,
 )
 from argparse import ArgumentParser, Namespace
 from logging import debug, info, basicConfig
+from random import choice, choices, randint
 from string import ascii_letters, digits
 from typing import Tuple, Dict, List
-from random import choice, choices
 from dataclasses import dataclass
 from os.path import splitext
 from base64 import b85encode
+from re import sub, finditer
 from gzip import compress
 from json import dump
-from re import sub
 import builtins
 
 
 class DocPassword:
 
     """
     Password is a string to encrypt python code with xor.
@@ -305,15 +305,15 @@
         """
         This function returns content and AST from python file.
         """
 
         with open(self.filename, encoding=self.encoding) as file:
             code = self.code = file.read()
 
-        debug(f"Get code from {self.filename}")
+        debug(f"Get code from {self.filename!r}")
 
         astcode = self.astcode = parse(code)
         return code, astcode
 
     def add_super_arguments(self, code: str = None) -> Tuple[str, AST]:
         r"""
         This function adds super arguments because super
@@ -701,14 +701,67 @@
             if isinstance(element, Expr) and isinstance(
                 element.value, Constant
             ):
                 del astcode.body[i]
 
         return astcode
 
+    def string_obfuscation(self, string: str) -> str:
+        """
+        This function obfuscate a string.
+        """
+
+        def to_hex(car: str) -> str:
+            return f"'\\x{ord(car):0>2x}'"
+
+        def to_octal(car: str) -> str:
+            return f"'\\{ord(car):0>3o}'"
+
+        def to_chr(car: str) -> str:
+            return f"chr({ord(car)})"
+
+        def to_chrbin(car: str) -> str:
+            return f"chr({bin(ord(car))})"
+
+        def to_chradd(car: str) -> str:
+            value = ord(car)
+            temp_value = randint(0, value)
+            return f"chr({bin(temp_value)} + {oct(value - temp_value)})"
+
+        def to_chrsub(car: str) -> str:
+            value = ord(car)
+            temp_value = randint(value, value * value)
+            return f"chr({temp_value} - {temp_value - value})"
+
+        functions = (to_hex, to_octal, to_chr, to_chrbin, to_chradd, to_chrsub)
+        string_repr = repr(string)
+        code = self.code
+        debug('Hard coded string obfuscation: ' + string_repr)
+        while string_repr in code:
+            code = code.replace(string_repr, ' + '.join(choice(functions)(car) for car in string), 1)
+        self.code = code
+        return code
+
+    def int_call_obfuscation(self) -> str:
+        """
+        This method obfuscates int calls for int obfuscation.
+        """
+
+        code = self.code
+        for match in finditer(r"\('0o[0-7]+', 8\)", code):
+            string = match.group()
+            debug('Int call obfuscation: ' + repr(string))
+            _8 = choice(('ord("\\x08")', oct(8), bin(8), (lambda x: f"{x} - {x - 8}")(randint(8, 256 * 256))))
+            value = string.split("'")[1]
+            self.code = code.replace(string, f"('{value}', {_8})", 1)
+            code = self.string_obfuscation(value)
+
+        self.code = code
+        return code
+
     def default_obfuscation(self) -> None:
         """
         This function starts the default obfuscation process.
 
         - get the code
         - initialize obfuscation
         - obfuscate names and values
@@ -724,18 +777,20 @@
         code, astcode = self.init_crypt_strings(code)
         self.init_builtins()
         astcode = self.visit(astcode)
 
         attributes_obfuscator = AttributeObfuscation(self)
         astcode = attributes_obfuscator.visit(astcode)
 
-        code = unparse(astcode)
-        self.code = code.replace(
-            "'decode'", "'\\x64\\x65\\x63\\x6f\\x64\\x65'"
-        ).replace("'utf-8'", "'\\x75\\x74\\x66\\x2d\\x38'")
+        self.code = unparse(astcode)
+
+        self.string_obfuscation('decode')
+        self.code = self.string_obfuscation('utf-8')
+        self.code = self.int_call_obfuscation()
+
         code = self.add_builtins()
         code = self.gzip(code)
         code = self.xor_code(code)
         code = self.base85(code)
         self.code = self.hexadecimal(code)
         code = self.write_code()
         self.write_deobfuscate()
@@ -777,32 +832,18 @@
 
         if self.level < 2:
             info("Level is less than 2 no Constant obfuscation.")
             return astcode
 
         is_str = isinstance(astcode.value, str)
 
-        if is_str and self.in_format_string:
-            debug(f"Format string obfuscation for {astcode.value!r}.")
-            astcode.value = astcode.value.encode(self.encoding)
-            astcode = self.generic_visit(astcode)
-
-            return Constant(
-                value="".join(
-                    f"\\x{x:0>2x}" if i % 2 else f"\\{x:0>3o}"
-                    for i, x in enumerate(astcode.value)
-                ),
-                kind=None,
-            )
-
-        elif is_str:
+        if is_str and not self.in_format_string:
             debug(f"String obfuscation for {astcode.value!r}.")
             astcode.value = astcode.value.encode(self.encoding)
             astcode = self.generic_visit(astcode)
-
             return Call(
                 func=Call(
                     func=NameAst(
                         id=self.default_names["getattr"].obfuscation,
                         ctx=Load(),
                     ),
                     args=[
@@ -834,26 +875,23 @@
                     id=self.default_names["xor"].obfuscation, ctx=Load()
                 ),
                 args=[Constant(value=self.xor(astcode.value))],
                 keywords=[],
             )
 
         elif isinstance(astcode.value, int) and not self.in_format_string:
-            info(f"Integer obfuscation for {astcode.value!r}")
+            debug(f"Integer obfuscation for {astcode.value!r}")
             astcode = self.generic_visit(astcode)
             return Call(
                 func=NameAst(
                     id=self.default_names["int"].obfuscation, ctx=Load()
                 ),
                 args=[
                     Constant(
-                        value="".join(
-                            f"\\x{x:0>2x}" if i % 2 else f"\\{x:0>3o}"
-                            for i, x in enumerate(oct(astcode.value).encode())
-                        )
+                        value=oct(astcode.value)
                     ),
                     Constant(value=8),
                 ],
                 keywords=[],
             )
         else:
             info(
@@ -1009,15 +1047,15 @@
         This function obfuscates name.
 
         astcode(Name): the name to obfuscate
         returns a Name with different id
         """
 
         if self.level >= 1:
-            debug(f"Name obfuscation for {astcode.id}")
+            debug(f"Name obfuscation for {astcode.id!r}")
             astcode.id = self.get_random_name(astcode.id).obfuscation
 
         astcode = self.generic_visit(astcode)
         return astcode
 
     def visit_Global(self, astcode: Global) -> Global:
         """
@@ -1177,15 +1215,16 @@
 
     parser = ArgumentParser(description="This tool obfuscates python code.")
     add_argument = parser.add_argument
 
     add_argument("filename")
     add_argument(
         "--output-filename",
-        "--output" "-o",
+        "--output",
+        "-o",
         default=None,
         help="Filename to write the obfuscate code.",
     )
     add_argument(
         "--level", "-l", type=int, default=6, help="Obfuscation level to use."
     )
     add_argument(
```

### Comparing `PyObfuscator-0.1.1/README.md` & `PyObfuscator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.1/setup.py` & `PyObfuscator-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `PyObfuscator-0.1.1/tests/TestPyObfuscator.py` & `PyObfuscator-0.1.2/tests/TestPyObfuscator.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,1307 +1,1307 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-###################
-#    Test for file named Obfuscator.py
-#    Copyright (C) 2021  Maurice Lambert
-
-#    This program is free software: you can redistribute it and/or modify
-#    it under the terms of the GNU General Public License as published by
-#    the Free Software Foundation, either version 3 of the License, or
-#    (at your option) any later version.
-
-#    This program is distributed in the hope that it will be useful,
-#    but WITHOUT ANY WARRANTY; without even the implied warranty of
-#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#    GNU General Public License for more details.
-
-#    You should have received a copy of the GNU General Public License
-#    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-###################
-
-"""
-Tests:
- - python3 -m doctest -v PyObfuscator.py
- - python3 -m unittest discover -s tests -p Test*.py -v
-"""
-
-default_dir = dir()
-
-from os import path, getcwd, remove, environ
-from unittest.mock import MagicMock, Mock
-from unittest import TestCase
-import unittest
-import json
-import ast
-import sys
-
-sys.path.append(path.join(path.dirname(__file__), "..", "PyObfuscator"))
-
-from PyObfuscator import Obfuscator, Name, AttributeObfuscation, DocPassword, DocLevels, parse_args, main
-import PyObfuscator
-
-class Test_DocPassword(TestCase):
-    def test_print_the_doc(self):
-        DocPassword.print_the_doc()
-        
-class Test_DocLevels(TestCase):
-    def test_print_the_doc(self):
-        DocLevels.print_the_doc()
-
-class Test_Name(TestCase):
-    def test_build_Name(self):
-        name = Name("name", "obfu_name", False, None)
-        self.assertIsInstance(name, Name, "a Name is not instance of Name")
-        self.assertIsNone(
-            name.namespace_name,
-            "When Name.namespace_name is defined as None, isn't None",
-        )
-        self.assertFalse(
-            name.is_defined, "When Name.is_defined is defined as False, isn't False"
-        )
-        self.assertEqual(
-            name.name,
-            "name",
-            "When Name.name is defined as 'name', isn't equal to 'name'",
-        )
-        self.assertEqual(
-            name.obfuscation,
-            "obfu_name",
-            "When Name.obfuscation is defined as 'obfu_name', isn't equal to 'obfu_name'",
-        )
-
-
-class Test_AttributeObfuscation(TestCase):
-    def test_visit_AugAssign(self):
-        obfu = Obfuscator("")
-        obfu_attr = AttributeObfuscation(obfu)
-        obfu_attr.generic_visit = lambda x: self.assertTrue(obfu_attr.in_assign)
-        obfu_attr.visit_AugAssign(Mock())
-        self.assertFalse(obfu_attr.in_assign)
-        
-    def test_visit_Assign(self):
-        obfu = Obfuscator("")
-        obfu_attr = AttributeObfuscation(obfu)
-        obfu_attr.generic_visit = lambda x: self.assertTrue(obfu_attr.in_assign)
-        obfu_attr.visit_Assign(Mock())
-        self.assertFalse(obfu_attr.in_assign)
-
-    def test_visit_Attribute(self):
-        name1 = Name("test1", "obfu1", True, None)
-        name2 = Name("test2", "obfu2", False, None)
-        obfu = Obfuscator(
-            "",
-            names={
-                "test1": name1,
-                "test2": name2,
-                'getattr': Name("getattr", 'obfu3', False, None),
-                'xor': Name("xor", 'obfu4', False, None),
-            },
-        )
-        obfu._xor_password_key = b'\0'
-        obfu._xor_password_key_length = 1
-
-        attribute1 = ast.Attribute(
-            value=ast.Name(id="self", ctx=ast.Load()), attr="test1", ctx=ast.Load()
-        )
-        attribute2 = ast.Attribute(
-            value=ast.Name(id="self", ctx=ast.Load()), attr="test2", ctx=ast.Load()
-        )
-        obfu_attr = AttributeObfuscation(obfu)
-
-        attribute = obfu_attr.visit(attribute2)
-        self.assertEqual(
-            attribute.args[1].func.args[0].args[0].value, b"test2", "visit_Attribute change undefined name"
-        )
-        
-        attribute = obfu_attr.visit(attribute1)
-        self.assertEqual(
-            attribute.args[1].func.args[0].args[0].value, b"obfu1", "visit_Attribute don't change defined name"
-        )
-        
-        obfu_attr.in_assign = True
-        attribute = obfu_attr.visit(attribute1)
-        self.assertEqual(attribute.attr, "obfu1")
-
-
-class Test_Function(TestCase):
-    def test_parse_args(self):
-        PyObfuscator.ArgumentParser.parse_args = Mock()
-        parse_args()
-        PyObfuscator.ArgumentParser.parse_args.assert_called_once_with()
-        
-    def test_main(self):
-        PyObfuscator.parse_args = Mock(return_value=Mock(names=["test:test"]))
-        default_obfuscation = Obfuscator.default_obfuscation
-        Obfuscator.default_obfuscation = Mock()
-        main()
-        PyObfuscator.parse_args.assert_called_once_with()
-        Obfuscator.default_obfuscation.assert_called_once_with()
-        Obfuscator.default_obfuscation = default_obfuscation
-
-class Test_Obfuscator(TestCase):
-    def test_add_super_arguments(self):
-        obfu = Obfuscator("")
-        code, astcode = obfu.add_super_arguments("class A:\n\tdef __init__(self):super().__init__()")
-        self.assertEqual(code, 'class A:\n\tdef __init__(self):super(self.__class__, self).__init__()')
-
-    def test_set_namespace_name(self):
-        obfu = Obfuscator("")
-
-        self.assertIsNone(
-            obfu.current_class, "default Obfuscator.current_name is not None"
-        )
-        precedent_name = obfu.set_namespace_name("abc")
-        self.assertIsNone(
-            precedent_name,
-            "Obfuscator.set_namespace_name don't return the precedent name",
-        )
-        self.assertEqual(
-            "abc",
-            obfu.current_class,
-            "Obfuscator.set_namespace_name don't set the good name",
-        )
-        precedent_name = obfu.set_namespace_name("test")
-        self.assertEqual(
-            precedent_name,
-            "abc",
-            "Obfuscator.set_namespace_name don't return the precedent name",
-        )
-        self.assertEqual(
-            "abc.test",
-            obfu.current_class,
-            "Obfuscator.set_namespace_name don't set the good name",
-        )
-
-    def test_get_random_name(self):
-        from string import ascii_letters
-
-        obfu = Obfuscator("")
-        name = obfu.get_random_name("abc")
-
-        self.assertEqual(
-            name,
-            obfu.get_random_name("abc"),
-            "get_random_name don't return initialised name",
-        )
-
-        self.assertIsInstance(name, Name, "get_rendom_name don't return a str")
-        self.assertEqual(
-            len(name.obfuscation), 12, "Default get_random_name length is not 12."
-        )
-
-        for i in range(100):
-            name = obfu.get_random_name(name.obfuscation)
-            self.assertIn(
-                name.obfuscation[0],
-                ascii_letters + "_",
-                "First character of get_random_name isn't valid.",
-            )
-            self.assertRegex(
-                name.obfuscation,
-                "^[a-zA-Z_][a-zA-Z0-9_]{11}$",
-                "Name returned by get_random_name is not valid.",
-            )
-
-    def test_get_code(self):
-        from ast import AST, dump
-
-        test_filename = path.join(getcwd(), "test.py")
-
-        with open(test_filename, "w") as file:
-            file.write("print('Hello World !')")
-
-        obfu = Obfuscator(test_filename)
-        code, parsed_code = obfu.get_code()
-
-        self.assertIsInstance(
-            code, str, "First returned value of get_code is not a str"
-        )
-        self.assertIsInstance(
-            parsed_code, AST, "Second returned value of get_code is not a ast.AST"
-        )
-
-        self.assertEqual(
-            code, "print('Hello World !')", "get_code don't return the good code"
-        )
-
-        self.assertIn(
-            "Hello World !", dump(parsed_code), "get_code don't return the good ast.AST"
-        )
-        self.assertIn(
-            "print", dump(parsed_code), "get_code don't return the good ast.AST"
-        )
-
-        # remove(test_filename)
-
-    def test_gzip(self):
-        mock = Mock()
-        mock.level = 0
-
-        mock.code = "environ['test'] = 'Hello World !'"
-        code = "environ['test'] = 'Python Hello World !'"
-
-        obfu = Obfuscator("")
-        self.assertEqual(
-            Obfuscator.gzip(mock),
-            "environ['test'] = 'Hello World !'",
-            "Gzip obfuscation must not executed with level 0",
-        )
-
-        mock.level = 6
-        gziped_code = Obfuscator.gzip(mock)
-
-        #########################
-        ##  TEST WITHOUT PARAMS
-        #########################
-
-        for zipped_code in (gziped_code, mock.code):
-            self.assertRegex(
-                zipped_code,
-                r"^from gzip import decompress as __;_=exec;_\(__\(b'[\x00-\xff]+'\){2}$",
-                "gzip obfuscation: bad return value",
-            )
-            exec(zipped_code)
-
-            self.assertEqual(
-                environ["test"],
-                "Hello World !",
-                "Gzip obfuscation: bad execution",
-            )
-
-        #########################
-        ##  TEST WITH PARAMS
-        #########################
-
-        gziped_code = obfu.gzip(code)
-
-        for zipped_code in (gziped_code, obfu.code):
-            self.assertRegex(
-                zipped_code,
-                r"^from gzip import decompress as __;_=exec;_\(__\(b'[\x00-\xff]+'\){2}$",
-                "gzip obfuscation: bad return value",
-            )
-            exec(zipped_code)
-
-            self.assertEqual(
-                environ["test"],
-                "Python Hello World !",
-                "Gzip obfuscation: bad execution",
-            )
-
-    def test_hexadecimal(self):
-        mock = Mock()
-        mock.level = 0
-
-        mock.code = "environ['test'] = 'Hello World !'"
-        non_obfu_code1_length = len(mock.code)
-
-        code = "environ['test'] = 'Python Hello World !'"
-        non_obfu_code2_length = len(code)
-
-        obfu = Obfuscator("")
-        self.assertEqual(
-            Obfuscator.hexadecimal(mock),
-            "environ['test'] = 'Hello World !'",
-            "hexadecimal obfuscation must not executed with level 0",
-        )
-
-        mock.level = 6
-        hexa_code = Obfuscator.hexadecimal(mock)
-
-        #########################
-        ##  TEST WITHOUT PARAMS
-        #########################
-
-        for hexa__code in (hexa_code, mock.code):
-            self.assertRegex(
-                hexa__code,
-                r"^_=exec;_\('(\\x[0-9a-f]{2}){size}'\)$".replace(
-                    "size", str(non_obfu_code1_length)
-                ),
-                "hexadecimal obfuscation: bad return value",
-            )
-            exec(hexa__code)
-
-            self.assertEqual(
-                environ["test"],
-                "Hello World !",
-                "hexadecimal obfuscation: bad execution",
-            )
-
-        #########################
-        ##  TEST WITH PARAMS
-        #########################
-
-        hexa_code = obfu.hexadecimal(code)
-
-        for hexa__code in (hexa_code, obfu.code):
-            self.assertRegex(
-                hexa__code,
-                r"^_=exec;_[(]'(\\x[0-9a-f]{2}){size}'[)]$".replace(
-                    "size", str(non_obfu_code2_length)
-                ),
-                "hexadecimal obfuscation: bad return value",
-            )
-            exec(hexa__code)
-
-            self.assertEqual(
-                environ["test"],
-                "Python Hello World !",
-                "hexadecimal: bad execution",
-            )
-
-    def test_base85(self):
-        mock = Mock()
-        mock.level = 0
-
-        mock.code = "environ['test'] = 'Hello World !'"
-        code = "environ['test'] = 'Python Hello World !'"
-
-        obfu = Obfuscator("")
-        self.assertEqual(
-            Obfuscator.base85(mock),
-            "environ['test'] = 'Hello World !'",
-            "Level 0 must not obfuscate code with base85",
-        )
-
-        mock.level = 6
-        base85_code = Obfuscator.base85(mock)
-
-        #########################
-        ##  TEST WITHOUT PARAMS
-        #########################
-
-        for encoded_code in (base85_code, mock.code):
-            self.assertRegex(
-                encoded_code,
-                r"^from base64 import b85decode as _;___=bytes\.decode;__=exec;__\(___\(_\(b'.*'\){3}$",
-                "base85: bad return value.",
-            )
-            exec(encoded_code)
-
-            self.assertEqual(
-                environ["test"],
-                "Hello World !",
-                "Bad execution with base85 obfuscation",
-            )
-
-        #########################
-        ##  TEST WITH PARAMS
-        #########################
-
-        base85_code = obfu.base85(code)
-
-        for encoded_code in (base85_code, obfu.code):
-            self.assertRegex(
-                encoded_code,
-                r"^from base64 import b85decode as _;___=bytes\.decode;__=exec;__\(___\(_\(b'.*'\){3}$",
-                "base85: bad return value.",
-            )
-            exec(encoded_code)
-
-            self.assertEqual(
-                environ["test"],
-                "Python Hello World !",
-                "Bad execution with base85 obfuscation",
-            )
-
-    def test_xor_code(self):
-        def input(string):
-            return "abc"
-
-        mock1 = Mock()
-        mock2 = Mock()
-        mock1.level = 0
-        mock2.level = 6
-
-        mock1.code = "environ['test'] = 'Hello World !'"
-        mock1.password = None
-        non_obfu_code1_length = len(mock1.code)
-
-        self.assertEqual(
-            Obfuscator.xor_code(mock1),
-            "environ['test'] = 'Hello World !'",
-            "xor_code change code with level 0",
-        )
-        mock1.level = 6
-
-        mock2.code = "environ['test'] = 'Hello World !'"
-        mock2.password = "abc"
-
-        code = "environ['test'] = 'Python Hello World !'"
-        non_obfu_code2_length = len(code)
-
-        obfu1 = Obfuscator("")
-        obfu2 = Obfuscator("", password="abc")
-        xor_code1 = Obfuscator.xor_code(mock1)
-        xor_code2 = Obfuscator.xor_code(mock2)
-
-        #########################
-        ##  TEST WITHOUT PARAMS AND PASSWORD
-        #########################
-
-        for cipher_code in (xor_code1, mock1.code):
-            regexs = (
-                (
-                    "^_=\[([0-9]{1,3}(,[ ])?){40}\];__=len[(]_[)];___=exec;_____"
-                    "='';\nfor _______,______ in enumerate[(]\[([0-9]{1,3}(,[ ])?)"
-                    "{size}\][)]:_____\+=chr"
-                    "[(]______\^_\[_______%__\][)]\n___[(]_____[)]$"
-                )
-                .replace("size", str(non_obfu_code1_length))
-                .split("\n")
-            )
-
-            lines = cipher_code.split("\n")
-
-            for line, regex in zip(lines, regexs):
-                self.assertRegex(
-                    line,
-                    regex,
-                    "xor_code don't return the good python code",
-                )
-
-            exec(cipher_code)
-
-            self.assertEqual(
-                environ["test"],
-                "Hello World !",
-                "xor_code don't execute the good python code",
-            )
-
-        #########################
-        ##  TEST WITHOUT PARAMS, WITH PASSWORD
-        #########################
-
-        for cipher_code in (xor_code2, mock2.code):
-            regexs = (
-                (
-                    "^_=input[(]'Password: '[)].encode[(][)];__=len[(]_[)];___=exec;_____"
-                    "='';\nfor _______,______ in enumerate[(]\[([0-9]{1,3}(,[ ])?)"
-                    "{size}\][)]:_____\+=chr"
-                    "[(]______\^_\[_______%__\][)]\n___[(]_____[)]$"
-                )
-                .replace("size", str(non_obfu_code2_length))
-                .split("\n")
-            )
-
-            lines = cipher_code.split("\n")
-
-            for line, regex in zip(lines, regexs):
-                self.assertRegex(
-                    line,
-                    regex,
-                    "xor_code don't return the good python code",
-                )
-
-            exec(cipher_code)
-
-            self.assertEqual(
-                environ["test"],
-                "Hello World !",
-                "xor_code don't execute the good python code",
-            )
-
-        #########################
-        ##  TEST WITH PARAMS, WITHOUT PASSWORD
-        #########################
-
-        xor_code1 = obfu1.xor_code(code)
-
-        for cipher_code in (xor_code1, obfu1.code):
-            regexs = (
-                (
-                    "^_=\[([0-9]{1,3}(,[ ])?){40}\];__=len[(]_[)];___=exec;_____"
-                    "='';\nfor _______,______ in enumerate[(]\[([0-9]{1,3}(,[ ])?)"
-                    "{size}\][)]:_____\+=chr"
-                    "[(]______\^_\[_______%__\][)]\n___[(]_____[)]$"
-                )
-                .replace("size", str(non_obfu_code2_length))
-                .split("\n")
-            )
-
-            lines = cipher_code.split("\n")
-
-            for line, regex in zip(lines, regexs):
-                self.assertRegex(
-                    line,
-                    regex,
-                    "xor_code don't return the good python code",
-                )
-
-            exec(cipher_code)
-
-            self.assertEqual(
-                environ["test"],
-                "Python Hello World !",
-                "xor_code don't execute the good python code",
-            )
-
-        #########################
-        ##  TEST WITH PARAMS AND PASSWORD
-        #########################
-
-        xor_code2 = obfu2.xor_code(code)
-
-        for cipher_code in (xor_code2, obfu2.code):
-            regexs = (
-                (
-                    "^_=input[(]'Password: '[)].encode[(][)];__=len[(]_[)];___=exec;_____"
-                    "='';\nfor _______,______ in enumerate[(]\[([0-9]{1,3}(,[ ])?)"
-                    "{size}\][)]:_____\+=chr"
-                    "[(]______\^_\[_______%__\][)]\n___[(]_____[)]$"
-                )
-                .replace("size", str(non_obfu_code2_length))
-                .split("\n")
-            )
-
-            lines = cipher_code.split("\n")
-
-            for line, regex in zip(lines, regexs):
-                self.assertRegex(
-                    line,
-                    regex,
-                    "xor_code don't return the good python code",
-                )
-
-            exec(cipher_code)
-
-            self.assertEqual(
-                environ["test"],
-                "Python Hello World !",
-                "xor_code don't execute the good python code",
-            )
-
-    def test_visit_Constant(self):
-        constant1 = ast.Constant(value="abc")
-        constant2 = ast.Constant(value=b"abc")
-        constant3 = ast.Constant(value=2)
-
-        obfu = Obfuscator("", level=0)
-        obfu.get_random_name("xor")
-        obfu.init_crypt_strings()
-        constant = obfu.visit_Constant(constant1)
-        self.assertEqual(
-            constant.value, "abc", "visit_Constant change code with level 0"
-        )
-        obfu.level = 6
-
-        call1 = obfu.visit_Constant(constant1)
-        call2 = obfu.visit_Constant(constant2)
-        constant3_bis = obfu.visit_Constant(constant3)
-
-        for constant in (call1, call2):
-            self.assertIsInstance(
-                constant, ast.Call, "visit_Constant don't return a ast.Call."
-            )
-
-        self.assertEqual(
-            b"abc",
-            obfu.xor(call2.args[0].value),
-            "visit_Constant don't return the good value with bytes",
-        )
-        self.assertEqual(
-            "abc",
-            obfu.xor(call1.func.args[0].args[0].value).decode(),
-            "visit_Constant don't return the good value with str",
-        )
-        self.assertEqual(
-            constant3.value, constant3_bis.value, "visit_Constant change integer value"
-        )
-
-    def test_visit_Module(self):
-        (doc, *_), (body_without_doc, *_), module, obfu = builds()
-        obfu.level = 0
-
-        module_test = obfu.visit_Module(module)
-        self.assertIn(
-            doc, module_test.body, "visit_Module delete doc string with level 0"
-        )
-
-        obfu.level = 6
-        module_test = obfu.visit_Module(module)
-
-        self.assertNotIn(doc, module_test.body, "visit_Module don't delete doc string")
-        self.assertListEqual(
-            module_test.body,
-            body_without_doc,
-            "visit_Module don't delete only doc string",
-        )
-
-    def test_default_obfuscation(self):
-        obfu = Obfuscator("test.py")
-        default_code = (
-            "from os import environ;environ['test']='default_obfuscation test'"
-        )
-
-        with open("test.py", "w") as file:
-            file.write(default_code)
-
-        obfu.default_obfuscation()
-
-        self.assertTrue(
-            obfu.using_default_obfu,
-            "default_obfuscation don't set using_default_obfu to True",
-        )
-        self.assertTrue(
-            path.isfile(obfu.output_filename),
-            "default_obfuscation don't write the code",
-        )
-        self.assertTrue(
-            path.isfile("deobfuscate.json"),
-            "default_obfuscation don't write the deobfuscate file",
-        )
-
-        with open(obfu.output_filename) as file:
-            code = file.read()
-
-        self.assertNotEqual(
-            code, default_code, "default_obfuscation don't obfuscate the code"
-        )
-
-        import test_obfu
-
-        self.assertEqual(
-            "default_obfuscation test",
-            getattr(test_obfu, obfu.default_names["environ"].obfuscation)["test"],
-            "default_obfuscation don't obfuscate the correctly/good code",
-        )
-
-        # remove("test.py")
-        # remove("test_obfu.py")
-        remove("deobfuscate.json")
-
-    def test_get_attributes_from(self):
-        obfu = Obfuscator("")
-        mock1 = Mock()
-        mock1.test_attr = True
-
-        mock2 = Mock()
-        mock2 = obfu.get_attributes_from(mock2, mock1)
-
-        self.assertTrue(
-            mock2.test_attr,
-            "get_attributes_from don't set all attributes on the new object",
-        )
-
-    def test_delete_doc_string(self):
-        (doc, *_), (body_without_doc, *_), ast_doc_string, obfu = builds()
-
-        ast_test = obfu.delete_doc_string(ast_doc_string)
-
-        self.assertNotIn(
-            doc, ast_test.body, "delete_doc_string don't delete doc string"
-        )
-        self.assertListEqual(
-            ast_test.body,
-            body_without_doc,
-            "delete_doc_string don't delete only doc string",
-        )
-
-    def test_delete_field(self):
-        _, _, ast_with_body, obfu = builds()
-
-        ast_without_body = obfu.delete_field(ast_with_body, "body")
-
-        with self.assertRaises(AttributeError, msg="delete_field don't delete field"):
-            ast_without_body.body
-
-    def test_delete_annotations(self):
-        _, _, ast_with_annotation, obfu = builds()
-
-        ast_without_annotation = obfu.delete_annotations(ast_with_annotation)
-
-        with self.assertRaises(
-            AttributeError, msg="delete_annotations don't delete annotations"
-        ):
-            ast_without_annotation.annotation
-
-    def test_delete_returns(self):
-        _, _, ast_with_returns, obfu = builds()
-
-        ast_without_returns = obfu.delete_returns(ast_with_returns)
-
-        with self.assertRaises(
-            AttributeError, msg="delete_returns don't delete returns"
-        ):
-            ast_without_returns.returns
-
-    def test_get_targets_and_value_for_import(self):
-        elements = [ast.alias(name="dump"), ast.alias(name="Assign", asname="custom")]
-        module = "ast"
-
-        obfu = Obfuscator("")
-        obfu.get_random_name("xor")
-        # init_obfu_names(obfu)
-        obfu.init_builtins()
-        obfu.init_crypt_strings()
-        targets, values = obfu.get_targets_and_value_for_import(module, elements)
-
-        targets = obfu.visit(targets)
-        values = obfu.visit(values)
-
-        self.assertIsInstance(
-            targets,
-            ast.Tuple,
-            "get_targets_and_value_for_import don't return ast.Tuple object",
-        )
-        self.assertIsInstance(
-            values,
-            ast.Tuple,
-            "get_targets_and_value_for_import don't return ast.Tuple object",
-        )
-
-        for target in targets.elts:
-            self.assertIn(
-                obfu.obfu_names[target.id].name,
-                [
-                    element.__dict__.get("asname") or element.__dict__.get("name")
-                    for element in elements
-                ],
-                "get_targets_and_value_for_import return bad obfu name in first tuple",
-            )
-
-        for value in values.elts:
-            self.assertEqual(
-                value.args[0].func.id,
-                obfu.default_names["myimport"].obfuscation,
-                "get_targets_and_value_for_import don't return import function in second tuple",
-            )
-            self.assertEqual(
-                obfu.xor(value.args[0].args[0].func.args[0].args[0].value).decode(),
-                module,
-                "get_targets_and_value_for_import don't import the good function name in second tuple",
-            )
-            self.assertEqual(
-                value.func.id,
-                obfu.default_names["getattr"].obfuscation,
-                "get_targets_and_value_for_import don't return obfu __dict__ name in second tuple",
-            )
-            self.assertIn(
-                obfu.xor(value.args[1].func.args[0].args[0].value).decode(),
-                [element.name for element in elements],
-                "get_targets_and_value_for_import don't import the good element name in second tuple",
-            )
-
-    def test_visit_Import(self):
-        import1 = ast.Import(names=[ast.alias(name="os"), ast.alias(name="sys"), ast.alias(name="xml.dom.minidom"), ast.alias(name="urllib.request", asname="req")])
-
-        obfu = Obfuscator("", level=0)
-        obfu.init_crypt_strings()
-        import1 = obfu.visit_Import(import1)
-
-        self.assertIsInstance(
-            import1,
-            ast.Import,
-            "visit_Import don't return an ast.Import object with level 0",
-        )
-
-        obfu.level = 6
-        obfu.init_builtins()
-        assign = obfu.visit_Import(import1)
-
-        self.assertIsInstance(
-            assign, ast.Assign, "visit_Import don't return an ast.Assign object"
-        )
-
-        for name in assign.targets[0].elts:
-            self.assertIn(
-                obfu.obfu_names[name.id].name,
-                ["os", "sys", "xml", "req"],
-                "visit_Import don't assign the good variable name",
-            )
-
-        for call in assign.value.elts:
-            try:
-                first = True
-                module = obfu.xor(call.args[0].args[0].func.args[0].args[0].value).decode()
-            except:
-                first = False
-                module = obfu.xor(call.args[0].func.args[0].args[0].value).decode()
-            if first:
-                self.assertEqual(
-                    obfu.obfu_names[call.args[0].func.id].name,
-                    "myimport",
-                    "visit_Import don't call __import__ functions",
-                )
-                self.assertIn(
-                    module,
-                    ["urllib.request"],
-                    "visit_Import don't import good module",
-                )
-            else:
-                self.assertEqual(
-                    obfu.obfu_names[call.func.id].name,
-                    "__import__",
-                    "visit_Import don't call __import__ functions",
-                )
-                self.assertIn(
-                    module,
-                    ["os", "sys", 'xml.dom.minidom'],
-                    "visit_Import don't import good module",
-                )
-
-    def test_visit_ImportFrom(self):
-        import_from1 = ast.ImportFrom(
-            module="dataclasses", names=[ast.alias(name="dataclass")], level=0
-        )
-        import_from2 = ast.ImportFrom(
-            module="ast", names=[ast.alias(name="*")], level=0
-        )
-
-        ast_attr = [
-            attr
-            for attr in dir(ast)
-            if not (attr.startswith("__") and attr.endswith("__"))
-        ]
-
-        obfu = Obfuscator("", level=0)
-        obfu.init_crypt_strings()
-        import_from1 = obfu.visit_ImportFrom(import_from1)
-        self.assertIsInstance(
-            import_from1,
-            ast.ImportFrom,
-            "visit_ImportFrom don't return an ast.ImportFrom object with level 0",
-        )
-
-        obfu.level = 6
-        obfu.init_builtins()
-        assign = obfu.visit_ImportFrom(import_from1)
-
-        self.assertIsInstance(
-            assign, ast.Assign, "visit_ImportFrom don't return an ast.Assign object"
-        )
-
-        assign = obfu.visit_ImportFrom(import_from2)
-        self.assertEqual(
-            len(ast_attr),
-            len(assign.targets[0].elts),
-            "visit_ImportFrom don't import all attributes when import *",
-        )
-        obfu_ast_attr = [obfu.default_names[attr].obfuscation for attr in ast_attr]
-        self.assertListEqual(
-            obfu_ast_attr,
-            [name.id for name in assign.targets[0].elts],
-            "visit_ImportFrom don't import good attributes when import *",
-        )
-
-    def test_init_builtins(self):
-        global default_dir
-
-        obfu = Obfuscator("")
-        builtins_obfu = obfu.init_builtins()
-
-        elements = (
-            list(globals()["__builtins__"].keys())
-            if isinstance(__builtins__, dict)
-            else dir(__builtins__)
-        ) + default_dir
-
-        self.assertEqual(
-            builtins_obfu,
-            obfu.default_variables,
-            "init builtins obfuscation: Bad return value",
-        )
-
-        builtins_obfu = builtins_obfu.split("\n")[0]
-        obfu_builtins, builtins = builtins_obfu.split("=")
-        builtins, obfu_builtins = builtins.split(","), obfu_builtins.split(",")
-
-        self.assertEqual(
-            len(builtins),
-            len(obfu_builtins),
-            "len(builtins) is not equal to len(obfu_builtins) in init_builtins",
-        )
-
-        for i, obfu_name in enumerate(obfu_builtins):
-            self.assertEqual(
-                builtins[i],
-                obfu.obfu_names[obfu_name].name,
-                "order of builtins or obfuscate_name is not good",
-            )
-            self.assertIn(
-                builtins[i], elements, f"{builtins[i]} isn't in defaults variables"
-            )
-
-    def test_init_crypt_strings(self):
-        obfu1 = Obfuscator("")
-        code1, astcode1 = obfu1.init_crypt_strings()
-
-        obfu2 = Obfuscator("")
-        code2, astcode2 = obfu2.init_crypt_strings("abc='abc'")
-
-        for code, obfu in ((code1, obfu1), (code2, obfu2)):
-            self.assertIsNotNone(
-                obfu._xor_password_key, "init_crypt_strings don't set the xor key"
-            )
-            self.assertEqual(
-                len(obfu._xor_password_key),
-                obfu._xor_password_key_length,
-                "init_crypt_strings don't set the xor key with good length",
-            )
-
-            self.assertRegex(
-                code,
-                "^xor=lambda bytes_:\(bytes\(\[x\^\[([0-9]{1,3}(,[ ])?){40}\]\[i%40\] for i,x in enumerate\(bytes_\)\]\)\)\n.*$",
-                "init_crypt_strings don't return the good code",
-            )
-
-            exec(code)
-            encrypt = eval("xor(b'abc')")
-            self.assertEqual(
-                len(encrypt),
-                3,
-                "init_crypt_strings don't define xor lambda function",
-            )
-            self.assertEqual(
-                eval(f"xor({encrypt})"),
-                b"abc",
-                "init_crypt_strings don't decrypt correctly an encrypted bytes",
-            )
-
-    def test_xor(self):
-        obfu = Obfuscator("")
-
-        with self.assertRaises(
-            RuntimeError,
-            msg="xor don't raise RuntimeError when _xor_password_key is None",
-        ):
-            obfu.xor(b"abc")
-
-        obfu.init_crypt_strings()
-
-        self.assertEqual(
-            obfu.xor(obfu.xor(b"abc")),
-            b"abc",
-            "xor don't decrypt correctly an encrypted bytes",
-        )
-
-    def test_visit_ClassDef(self):
-        class_ = ast.ClassDef(
-            name="Test",
-            bases=[ast.Name(id="Classe", ctx=ast.Load())],
-            keywords=[],
-            body=[ast.Expr(value=ast.Constant(value=" Doc String "))],
-            decorator_list=[],
-        )
-
-        obfu = Obfuscator("", level=0)
-        class_ = obfu.visit_ClassDef(class_)
-
-        self.assertEqual(
-            class_.name, "Test", "visit_ClassDef change the class name with level 0"
-        )
-        self.assertEqual(
-            len(class_.body), 1, "visit_ClassDef delete doc string with level 0"
-        )
-
-        obfu.level = 6
-        class_ = obfu.visit_ClassDef(class_)
-
-        self.assertEqual(len(class_.body), 0, "visit_ClassDef don't delete doc string")
-        self.assertNotEqual(
-            class_.name, "Test", "visit_ClassDef don't change the class name"
-        )
-        self.assertEqual(
-            obfu.default_names["Test"].obfuscation,
-            class_.name,
-            "visit_ClassDef the new class name is bad",
-        )
-        self.assertEqual(
-            obfu.obfu_names[class_.name].name,
-            "Test",
-            "visit_ClassDef the new class name is bad",
-        )
-
-    def test_visit_FunctionDef(self):
-        function1 = ast.FunctionDef(
-            name="__init__",
-            args=ast.arguments(
-                posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[]
-            ),
-            body=[ast.Expr(value=ast.Constant(value=" Doc String "))],
-            decorator_list=[],
-        )
-
-        function2 = ast.FunctionDef(
-            name="init",
-            args=ast.arguments(
-                posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[]
-            ),
-            body=[ast.Expr(value=ast.Constant(value=" Doc String "))],
-            decorator_list=[],
-        )
-
-        obfu = Obfuscator("", level=0)
-        function = obfu.visit_FunctionDef(function2)
-        self.assertEqual(
-            function.name,
-            "init",
-            "visit_FunctionDef change the function name with level 0",
-        )
-        self.assertEqual(
-            len(function.body), 1, "visit_FunctionDef delete doc string with level 0"
-        )
-
-        obfu.level = 6
-
-        function = obfu.visit_FunctionDef(function2)
-        self.assertEqual(
-            len(function.body), 0, "visit_FunctionDef don't delete doc string"
-        )
-        self.assertNotEqual(
-            function.name, "init", "visit_FunctionDef don't change the function name"
-        )
-        self.assertEqual(
-            obfu.default_names["init"].obfuscation,
-            function.name,
-            "visit_FunctionDef the new function name is bad",
-        )
-        self.assertEqual(
-            obfu.obfu_names[function.name].name,
-            "init",
-            "visit_FunctionDef the new function name is bad",
-        )
-
-        function = obfu.visit_FunctionDef(function1)
-        self.assertEqual(
-            function.name,
-            "__init__",
-            "visit_FunctionDef change the magic function name",
-        )
-
-    def test_visit_Name(self):
-        name = ast.Name(id="name", ctx=ast.Store())
-
-        obfu = Obfuscator("", level=0)
-        name = obfu.visit_Name(name)
-        self.assertEqual(name.id, "name", "visit_Name change Name.id with level 0")
-
-        obfu.level = 6
-        name = obfu.visit_Name(name)
-
-        self.assertEqual(
-            obfu.default_names["name"].obfuscation,
-            name.id,
-            "visit_Name don't return a Name with a good id",
-        )
-
-    def test_visit_Global(self):
-        names = ["f0", "f1"]
-        global_ = ast.Global(names=names.copy())
-
-        obfu = Obfuscator("", level=0)
-        global_ = obfu.visit_Global(global_)
-        self.assertListEqual(
-            global_.names, names, "visit_Global change names with level 0"
-        )
-
-        obfu.level = 6
-        global_ = obfu.visit_Global(global_)
-
-        for i, name in enumerate(global_.names):
-            self.assertIn(
-                obfu.obfu_names[name].name,
-                names,
-                "visit_Global don't return good obfuscate names",
-            )
-            self.assertEqual(
-                obfu.obfu_names[name].name,
-                f"f{i}",
-                "visit_Global don't return names with good order",
-            )
-
-    def test_visit_arg(self):
-        arg = ast.arg(arg="arg", annotation=ast.Name(id="str", ctx=ast.Load()))
-
-        obfu = Obfuscator("", level=0)
-        arg = obfu.visit_arg(arg)
-
-        self.assertIsNotNone(arg.annotation, "visit_arg delete annotation with level 0")
-        self.assertEqual(
-            arg.annotation.id, "str", "visit_arg change annotation with level 0"
-        )
-
-        obfu.level = 6
-        arg = obfu.visit_arg(arg)
-
-        self.assertIsNone(arg.annotation, "visit_arg don't delete annotation")
-        self.assertEqual(
-            obfu.default_names["arg"].obfuscation,
-            arg.arg,
-            "visit_arg don't return arg(object) with good arg(attribute)",
-        )
-
-    def test_visit_AnnAssign(self):
-        assign = ast.AnnAssign(
-            target=ast.Name(id="abc", ctx=ast.Store()),
-            annotation=ast.Name(id="str", ctx=ast.Load()),
-            value=ast.Constant(value="abc"),
-            simple=1,
-        )
-
-        obfu = Obfuscator("", level=0)
-        assign = obfu.visit_AnnAssign(assign)
-
-        self.assertIsInstance(
-            assign,
-            ast.AnnAssign,
-            "visit_AnnAssign change AnnAssign object with level 0",
-        )
-
-        obfu.level = 6
-        obfu.init_crypt_strings()
-        assign = obfu.visit_AnnAssign(assign)
-
-        self.assertIsInstance(
-            assign, ast.Assign, "visit_AnnAssign don't build Assign object"
-        )
-        self.assertEqual(
-            obfu.obfu_names[assign.targets[0].id].name,
-            "abc",
-            "visit_AnnAssign don't assign the good variable name",
-        )
-        self.assertEqual(
-            obfu.xor(assign.value.func.args[0].args[0].value).decode(),
-            "abc",
-            "visit_AnnAssign don't assign the good value",
-        )
-
-    def test_write_deobfuscate(self):
-        obfu = Obfuscator("test.py", names={"a": Name("a", "b", False, None)})
-        obfu.write_deobfuscate()
-
-        self.assertTrue(
-            path.isfile("deobfuscate.json"),
-            "write_deobfuscate don't create deobfuscate file",
-        )
-
-        with open("deobfuscate.json") as file:
-            config = json.load(file)
-
-        self.assertDictEqual(
-            config["names"][0],
-            {
-                "name": "a",
-                "obfuscation_name": "b",
-                "definition": False,
-                "namespace": None,
-            },
-            "write_deobfuscate don't write good names.",
-        )
-        self.assertIsNone(config["encryption_key"])
-        self.assertDictEqual(
-            config["Obfuscator"],
-            {
-                "level": 6,
-                "default_obfuscation": False,
-                "encoding": "utf-8",
-                "output_file": "test_obfu.py",
-            },
-        )
-
-        remove("deobfuscate.json")
-        obfu.deobfuscate = False
-        obfu.write_deobfuscate()
-
-        self.assertFalse(
-            path.isfile("deobfuscate.json"),
-            "write_deobfuscate create deobfuscate file when deobfuscate is desactivated",
-        )
-
-    def test_add_builtins(self):
-        obfu = Obfuscator("")
-
-        with self.assertRaises(
-            RuntimeError,
-            msg="add_builtins don't raise Error if default_variables isn't defined",
-        ):
-            obfu.add_builtins()
-
-        obfu.default_variables = "p=print\n"
-
-        with self.assertRaises(
-            RuntimeError, msg="add_builtins don't raise Error if code isn't defined"
-        ):
-            obfu.add_builtins()
-
-        obfu.code = "p('Hello World !')"
-        obfu.add_builtins()
-
-        self.assertEqual(
-            obfu.code,
-            "p=print\n" + "p('Hello World !')",
-            "add_builtins don't return the good code",
-        )
-
-    def test_write_code(self):
-        obfu = Obfuscator("")
-
-        with self.assertRaises(
-            RuntimeError, msg="write_code don't raise Error if code isn't defined"
-        ):
-            obfu.write_code()
-
-        obfu.code = "print('Hello World !')"
-
-        code = obfu.write_code()
-
-        self.assertEqual(
-            code,
-            obfu.code,
-            "write_code don't return the good code",
-        )
-
-        with open("_obfu.py") as file:
-            self.assertEqual(
-                file.read(),
-                obfu.code,
-                "write_code don't write the good code",
-            )
-
-        # remove("_obfu.py")
-
-
-def init_obfu_names(obfu):
-    for name in dir(__builtins__):
-        obfu.get_random_name(name)
-
-
-def builds():
-    doc = ast.Expr(value=ast.Constant(value="abc"))
-    false_doc = ast.Expr(value=Mock())
-
-    AST_test = ast.AST(
-        body=[doc, false_doc], annotation="annotation", returns=ast.Constant(value=None)
-    )
-    AST_test._fields = tuple(AST_test.__dict__.keys())
-
-    body_without_doc = AST_test.body.copy()
-    body_without_doc.remove(doc)
-
-    obfu = Obfuscator("")
-    obfu.init_crypt_strings()
-
-    return (doc, false_doc), (body_without_doc,), AST_test, obfu
-
-
-def write_ast():
-    with open("code_using_for_test.py") as file:
-        python_code = file.read()
-
-    ast_code = ast.parse(python_code)
-
-    with open("ast_code_using_for_test.py", "w") as file:
-        file.write(ast.dump(ast_code, indent=4))
-
-
-if __name__ == "__main__":
-    # write_ast()
-    unittest.main()
-
-    """
-        - Check if all functions are tested
-        - Check if all fonctionnalities are tested in all functions
-        - Test commands lines and executables
-    """
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+###################
+#    Test for file named Obfuscator.py
+#    Copyright (C) 2021  Maurice Lambert
+
+#    This program is free software: you can redistribute it and/or modify
+#    it under the terms of the GNU General Public License as published by
+#    the Free Software Foundation, either version 3 of the License, or
+#    (at your option) any later version.
+
+#    This program is distributed in the hope that it will be useful,
+#    but WITHOUT ANY WARRANTY; without even the implied warranty of
+#    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#    GNU General Public License for more details.
+
+#    You should have received a copy of the GNU General Public License
+#    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+###################
+
+"""
+Tests:
+ - python3 -m doctest -v PyObfuscator.py
+ - python3 -m unittest discover -s tests -p Test*.py -v
+"""
+
+default_dir = dir()
+
+from os import path, getcwd, remove, environ
+from unittest.mock import MagicMock, Mock
+from unittest import TestCase
+import unittest
+import json
+import ast
+import sys
+
+sys.path.append(path.join(path.dirname(__file__), "..", "PyObfuscator"))
+
+from PyObfuscator import Obfuscator, Name, AttributeObfuscation, DocPassword, DocLevels, parse_args, main
+import PyObfuscator
+
+class Test_DocPassword(TestCase):
+    def test_print_the_doc(self):
+        DocPassword.print_the_doc()
+        
+class Test_DocLevels(TestCase):
+    def test_print_the_doc(self):
+        DocLevels.print_the_doc()
+
+class Test_Name(TestCase):
+    def test_build_Name(self):
+        name = Name("name", "obfu_name", False, None)
+        self.assertIsInstance(name, Name, "a Name is not instance of Name")
+        self.assertIsNone(
+            name.namespace_name,
+            "When Name.namespace_name is defined as None, isn't None",
+        )
+        self.assertFalse(
+            name.is_defined, "When Name.is_defined is defined as False, isn't False"
+        )
+        self.assertEqual(
+            name.name,
+            "name",
+            "When Name.name is defined as 'name', isn't equal to 'name'",
+        )
+        self.assertEqual(
+            name.obfuscation,
+            "obfu_name",
+            "When Name.obfuscation is defined as 'obfu_name', isn't equal to 'obfu_name'",
+        )
+
+
+class Test_AttributeObfuscation(TestCase):
+    def test_visit_AugAssign(self):
+        obfu = Obfuscator("")
+        obfu_attr = AttributeObfuscation(obfu)
+        obfu_attr.generic_visit = lambda x: self.assertTrue(obfu_attr.in_assign)
+        obfu_attr.visit_AugAssign(Mock())
+        self.assertFalse(obfu_attr.in_assign)
+        
+    def test_visit_Assign(self):
+        obfu = Obfuscator("")
+        obfu_attr = AttributeObfuscation(obfu)
+        obfu_attr.generic_visit = lambda x: self.assertTrue(obfu_attr.in_assign)
+        obfu_attr.visit_Assign(Mock())
+        self.assertFalse(obfu_attr.in_assign)
+
+    def test_visit_Attribute(self):
+        name1 = Name("test1", "obfu1", True, None)
+        name2 = Name("test2", "obfu2", False, None)
+        obfu = Obfuscator(
+            "",
+            names={
+                "test1": name1,
+                "test2": name2,
+                'getattr': Name("getattr", 'obfu3', False, None),
+                'xor': Name("xor", 'obfu4', False, None),
+            },
+        )
+        obfu._xor_password_key = b'\0'
+        obfu._xor_password_key_length = 1
+
+        attribute1 = ast.Attribute(
+            value=ast.Name(id="self", ctx=ast.Load()), attr="test1", ctx=ast.Load()
+        )
+        attribute2 = ast.Attribute(
+            value=ast.Name(id="self", ctx=ast.Load()), attr="test2", ctx=ast.Load()
+        )
+        obfu_attr = AttributeObfuscation(obfu)
+
+        attribute = obfu_attr.visit(attribute2)
+        self.assertEqual(
+            attribute.args[1].func.args[0].args[0].value, b"test2", "visit_Attribute change undefined name"
+        )
+        
+        attribute = obfu_attr.visit(attribute1)
+        self.assertEqual(
+            attribute.args[1].func.args[0].args[0].value, b"obfu1", "visit_Attribute don't change defined name"
+        )
+        
+        obfu_attr.in_assign = True
+        attribute = obfu_attr.visit(attribute1)
+        self.assertEqual(attribute.attr, "obfu1")
+
+
+class Test_Function(TestCase):
+    def test_parse_args(self):
+        PyObfuscator.ArgumentParser.parse_args = Mock()
+        parse_args()
+        PyObfuscator.ArgumentParser.parse_args.assert_called_once_with()
+        
+    def test_main(self):
+        PyObfuscator.parse_args = Mock(return_value=Mock(names=["test:test"]))
+        default_obfuscation = Obfuscator.default_obfuscation
+        Obfuscator.default_obfuscation = Mock()
+        main()
+        PyObfuscator.parse_args.assert_called_once_with()
+        Obfuscator.default_obfuscation.assert_called_once_with()
+        Obfuscator.default_obfuscation = default_obfuscation
+
+class Test_Obfuscator(TestCase):
+    def test_add_super_arguments(self):
+        obfu = Obfuscator("")
+        code, astcode = obfu.add_super_arguments("class A:\n\tdef __init__(self):super().__init__()")
+        self.assertEqual(code, 'class A:\n\tdef __init__(self):super(self.__class__, self).__init__()')
+
+    def test_set_namespace_name(self):
+        obfu = Obfuscator("")
+
+        self.assertIsNone(
+            obfu.current_class, "default Obfuscator.current_name is not None"
+        )
+        precedent_name = obfu.set_namespace_name("abc")
+        self.assertIsNone(
+            precedent_name,
+            "Obfuscator.set_namespace_name don't return the precedent name",
+        )
+        self.assertEqual(
+            "abc",
+            obfu.current_class,
+            "Obfuscator.set_namespace_name don't set the good name",
+        )
+        precedent_name = obfu.set_namespace_name("test")
+        self.assertEqual(
+            precedent_name,
+            "abc",
+            "Obfuscator.set_namespace_name don't return the precedent name",
+        )
+        self.assertEqual(
+            "abc.test",
+            obfu.current_class,
+            "Obfuscator.set_namespace_name don't set the good name",
+        )
+
+    def test_get_random_name(self):
+        from string import ascii_letters
+
+        obfu = Obfuscator("")
+        name = obfu.get_random_name("abc")
+
+        self.assertEqual(
+            name,
+            obfu.get_random_name("abc"),
+            "get_random_name don't return initialised name",
+        )
+
+        self.assertIsInstance(name, Name, "get_rendom_name don't return a str")
+        self.assertEqual(
+            len(name.obfuscation), 12, "Default get_random_name length is not 12."
+        )
+
+        for i in range(100):
+            name = obfu.get_random_name(name.obfuscation)
+            self.assertIn(
+                name.obfuscation[0],
+                ascii_letters + "_",
+                "First character of get_random_name isn't valid.",
+            )
+            self.assertRegex(
+                name.obfuscation,
+                "^[a-zA-Z_][a-zA-Z0-9_]{11}$",
+                "Name returned by get_random_name is not valid.",
+            )
+
+    def test_get_code(self):
+        from ast import AST, dump
+
+        test_filename = path.join(getcwd(), "test.py")
+
+        with open(test_filename, "w") as file:
+            file.write("print('Hello World !')")
+
+        obfu = Obfuscator(test_filename)
+        code, parsed_code = obfu.get_code()
+
+        self.assertIsInstance(
+            code, str, "First returned value of get_code is not a str"
+        )
+        self.assertIsInstance(
+            parsed_code, AST, "Second returned value of get_code is not a ast.AST"
+        )
+
+        self.assertEqual(
+            code, "print('Hello World !')", "get_code don't return the good code"
+        )
+
+        self.assertIn(
+            "Hello World !", dump(parsed_code), "get_code don't return the good ast.AST"
+        )
+        self.assertIn(
+            "print", dump(parsed_code), "get_code don't return the good ast.AST"
+        )
+
+        # remove(test_filename)
+
+    def test_gzip(self):
+        mock = Mock()
+        mock.level = 0
+
+        mock.code = "environ['test'] = 'Hello World !'"
+        code = "environ['test'] = 'Python Hello World !'"
+
+        obfu = Obfuscator("")
+        self.assertEqual(
+            Obfuscator.gzip(mock),
+            "environ['test'] = 'Hello World !'",
+            "Gzip obfuscation must not executed with level 0",
+        )
+
+        mock.level = 6
+        gziped_code = Obfuscator.gzip(mock)
+
+        #########################
+        ##  TEST WITHOUT PARAMS
+        #########################
+
+        for zipped_code in (gziped_code, mock.code):
+            self.assertRegex(
+                zipped_code,
+                r"^from gzip import decompress as __;_=exec;_\(__\(b'[\x00-\xff]+'\){2}$",
+                "gzip obfuscation: bad return value",
+            )
+            exec(zipped_code)
+
+            self.assertEqual(
+                environ["test"],
+                "Hello World !",
+                "Gzip obfuscation: bad execution",
+            )
+
+        #########################
+        ##  TEST WITH PARAMS
+        #########################
+
+        gziped_code = obfu.gzip(code)
+
+        for zipped_code in (gziped_code, obfu.code):
+            self.assertRegex(
+                zipped_code,
+                r"^from gzip import decompress as __;_=exec;_\(__\(b'[\x00-\xff]+'\){2}$",
+                "gzip obfuscation: bad return value",
+            )
+            exec(zipped_code)
+
+            self.assertEqual(
+                environ["test"],
+                "Python Hello World !",
+                "Gzip obfuscation: bad execution",
+            )
+
+    def test_hexadecimal(self):
+        mock = Mock()
+        mock.level = 0
+
+        mock.code = "environ['test'] = 'Hello World !'"
+        non_obfu_code1_length = len(mock.code)
+
+        code = "environ['test'] = 'Python Hello World !'"
+        non_obfu_code2_length = len(code)
+
+        obfu = Obfuscator("")
+        self.assertEqual(
+            Obfuscator.hexadecimal(mock),
+            "environ['test'] = 'Hello World !'",
+            "hexadecimal obfuscation must not executed with level 0",
+        )
+
+        mock.level = 6
+        hexa_code = Obfuscator.hexadecimal(mock)
+
+        #########################
+        ##  TEST WITHOUT PARAMS
+        #########################
+
+        for hexa__code in (hexa_code, mock.code):
+            self.assertRegex(
+                hexa__code,
+                r"^_=exec;_\('(\\x[0-9a-f]{2}){size}'\)$".replace(
+                    "size", str(non_obfu_code1_length)
+                ),
+                "hexadecimal obfuscation: bad return value",
+            )
+            exec(hexa__code)
+
+            self.assertEqual(
+                environ["test"],
+                "Hello World !",
+                "hexadecimal obfuscation: bad execution",
+            )
+
+        #########################
+        ##  TEST WITH PARAMS
+        #########################
+
+        hexa_code = obfu.hexadecimal(code)
+
+        for hexa__code in (hexa_code, obfu.code):
+            self.assertRegex(
+                hexa__code,
+                r"^_=exec;_[(]'(\\x[0-9a-f]{2}){size}'[)]$".replace(
+                    "size", str(non_obfu_code2_length)
+                ),
+                "hexadecimal obfuscation: bad return value",
+            )
+            exec(hexa__code)
+
+            self.assertEqual(
+                environ["test"],
+                "Python Hello World !",
+                "hexadecimal: bad execution",
+            )
+
+    def test_base85(self):
+        mock = Mock()
+        mock.level = 0
+
+        mock.code = "environ['test'] = 'Hello World !'"
+        code = "environ['test'] = 'Python Hello World !'"
+
+        obfu = Obfuscator("")
+        self.assertEqual(
+            Obfuscator.base85(mock),
+            "environ['test'] = 'Hello World !'",
+            "Level 0 must not obfuscate code with base85",
+        )
+
+        mock.level = 6
+        base85_code = Obfuscator.base85(mock)
+
+        #########################
+        ##  TEST WITHOUT PARAMS
+        #########################
+
+        for encoded_code in (base85_code, mock.code):
+            self.assertRegex(
+                encoded_code,
+                r"^from base64 import b85decode as _;___=bytes\.decode;__=exec;__\(___\(_\(b'.*'\){3}$",
+                "base85: bad return value.",
+            )
+            exec(encoded_code)
+
+            self.assertEqual(
+                environ["test"],
+                "Hello World !",
+                "Bad execution with base85 obfuscation",
+            )
+
+        #########################
+        ##  TEST WITH PARAMS
+        #########################
+
+        base85_code = obfu.base85(code)
+
+        for encoded_code in (base85_code, obfu.code):
+            self.assertRegex(
+                encoded_code,
+                r"^from base64 import b85decode as _;___=bytes\.decode;__=exec;__\(___\(_\(b'.*'\){3}$",
+                "base85: bad return value.",
+            )
+            exec(encoded_code)
+
+            self.assertEqual(
+                environ["test"],
+                "Python Hello World !",
+                "Bad execution with base85 obfuscation",
+            )
+
+    def test_xor_code(self):
+        def input(string):
+            return "abc"
+
+        mock1 = Mock()
+        mock2 = Mock()
+        mock1.level = 0
+        mock2.level = 6
+
+        mock1.code = "environ['test'] = 'Hello World !'"
+        mock1.password = None
+        non_obfu_code1_length = len(mock1.code)
+
+        self.assertEqual(
+            Obfuscator.xor_code(mock1),
+            "environ['test'] = 'Hello World !'",
+            "xor_code change code with level 0",
+        )
+        mock1.level = 6
+
+        mock2.code = "environ['test'] = 'Hello World !'"
+        mock2.password = "abc"
+
+        code = "environ['test'] = 'Python Hello World !'"
+        non_obfu_code2_length = len(code)
+
+        obfu1 = Obfuscator("")
+        obfu2 = Obfuscator("", password="abc")
+        xor_code1 = Obfuscator.xor_code(mock1)
+        xor_code2 = Obfuscator.xor_code(mock2)
+
+        #########################
+        ##  TEST WITHOUT PARAMS AND PASSWORD
+        #########################
+
+        for cipher_code in (xor_code1, mock1.code):
+            regexs = (
+                (
+                    "^_=\[([0-9]{1,3}(,[ ])?){40}\];__=len[(]_[)];___=exec;_____"
+                    "='';\nfor _______,______ in enumerate[(]\[([0-9]{1,3}(,[ ])?)"
+                    "{size}\][)]:_____\+=chr"
+                    "[(]______\^_\[_______%__\][)]\n___[(]_____[)]$"
+                )
+                .replace("size", str(non_obfu_code1_length))
+                .split("\n")
+            )
+
+            lines = cipher_code.split("\n")
+
+            for line, regex in zip(lines, regexs):
+                self.assertRegex(
+                    line,
+                    regex,
+                    "xor_code don't return the good python code",
+                )
+
+            exec(cipher_code)
+
+            self.assertEqual(
+                environ["test"],
+                "Hello World !",
+                "xor_code don't execute the good python code",
+            )
+
+        #########################
+        ##  TEST WITHOUT PARAMS, WITH PASSWORD
+        #########################
+
+        for cipher_code in (xor_code2, mock2.code):
+            regexs = (
+                (
+                    "^_=input[(]'Password: '[)].encode[(][)];__=len[(]_[)];___=exec;_____"
+                    "='';\nfor _______,______ in enumerate[(]\[([0-9]{1,3}(,[ ])?)"
+                    "{size}\][)]:_____\+=chr"
+                    "[(]______\^_\[_______%__\][)]\n___[(]_____[)]$"
+                )
+                .replace("size", str(non_obfu_code2_length))
+                .split("\n")
+            )
+
+            lines = cipher_code.split("\n")
+
+            for line, regex in zip(lines, regexs):
+                self.assertRegex(
+                    line,
+                    regex,
+                    "xor_code don't return the good python code",
+                )
+
+            exec(cipher_code)
+
+            self.assertEqual(
+                environ["test"],
+                "Hello World !",
+                "xor_code don't execute the good python code",
+            )
+
+        #########################
+        ##  TEST WITH PARAMS, WITHOUT PASSWORD
+        #########################
+
+        xor_code1 = obfu1.xor_code(code)
+
+        for cipher_code in (xor_code1, obfu1.code):
+            regexs = (
+                (
+                    "^_=\[([0-9]{1,3}(,[ ])?){40}\];__=len[(]_[)];___=exec;_____"
+                    "='';\nfor _______,______ in enumerate[(]\[([0-9]{1,3}(,[ ])?)"
+                    "{size}\][)]:_____\+=chr"
+                    "[(]______\^_\[_______%__\][)]\n___[(]_____[)]$"
+                )
+                .replace("size", str(non_obfu_code2_length))
+                .split("\n")
+            )
+
+            lines = cipher_code.split("\n")
+
+            for line, regex in zip(lines, regexs):
+                self.assertRegex(
+                    line,
+                    regex,
+                    "xor_code don't return the good python code",
+                )
+
+            exec(cipher_code)
+
+            self.assertEqual(
+                environ["test"],
+                "Python Hello World !",
+                "xor_code don't execute the good python code",
+            )
+
+        #########################
+        ##  TEST WITH PARAMS AND PASSWORD
+        #########################
+
+        xor_code2 = obfu2.xor_code(code)
+
+        for cipher_code in (xor_code2, obfu2.code):
+            regexs = (
+                (
+                    "^_=input[(]'Password: '[)].encode[(][)];__=len[(]_[)];___=exec;_____"
+                    "='';\nfor _______,______ in enumerate[(]\[([0-9]{1,3}(,[ ])?)"
+                    "{size}\][)]:_____\+=chr"
+                    "[(]______\^_\[_______%__\][)]\n___[(]_____[)]$"
+                )
+                .replace("size", str(non_obfu_code2_length))
+                .split("\n")
+            )
+
+            lines = cipher_code.split("\n")
+
+            for line, regex in zip(lines, regexs):
+                self.assertRegex(
+                    line,
+                    regex,
+                    "xor_code don't return the good python code",
+                )
+
+            exec(cipher_code)
+
+            self.assertEqual(
+                environ["test"],
+                "Python Hello World !",
+                "xor_code don't execute the good python code",
+            )
+
+    def test_visit_Constant(self):
+        constant1 = ast.Constant(value="abc")
+        constant2 = ast.Constant(value=b"abc")
+        constant3 = ast.Constant(value=2)
+
+        obfu = Obfuscator("", level=0)
+        obfu.get_random_name("xor")
+        obfu.init_crypt_strings()
+        constant = obfu.visit_Constant(constant1)
+        self.assertEqual(
+            constant.value, "abc", "visit_Constant change code with level 0"
+        )
+        obfu.level = 6
+
+        call1 = obfu.visit_Constant(constant1)
+        call2 = obfu.visit_Constant(constant2)
+        constant3_bis = obfu.visit_Constant(constant3)
+
+        for constant in (call1, call2):
+            self.assertIsInstance(
+                constant, ast.Call, "visit_Constant don't return a ast.Call."
+            )
+
+        self.assertEqual(
+            b"abc",
+            obfu.xor(call2.args[0].value),
+            "visit_Constant don't return the good value with bytes",
+        )
+        self.assertEqual(
+            "abc",
+            obfu.xor(call1.func.args[0].args[0].value).decode(),
+            "visit_Constant don't return the good value with str",
+        )
+        self.assertEqual(
+            constant3.value, constant3_bis.value, "visit_Constant change integer value"
+        )
+
+    def test_visit_Module(self):
+        (doc, *_), (body_without_doc, *_), module, obfu = builds()
+        obfu.level = 0
+
+        module_test = obfu.visit_Module(module)
+        self.assertIn(
+            doc, module_test.body, "visit_Module delete doc string with level 0"
+        )
+
+        obfu.level = 6
+        module_test = obfu.visit_Module(module)
+
+        self.assertNotIn(doc, module_test.body, "visit_Module don't delete doc string")
+        self.assertListEqual(
+            module_test.body,
+            body_without_doc,
+            "visit_Module don't delete only doc string",
+        )
+
+    def test_default_obfuscation(self):
+        obfu = Obfuscator("test.py")
+        default_code = (
+            "from os import environ;environ['test']='default_obfuscation test'"
+        )
+
+        with open("test.py", "w") as file:
+            file.write(default_code)
+
+        obfu.default_obfuscation()
+
+        self.assertTrue(
+            obfu.using_default_obfu,
+            "default_obfuscation don't set using_default_obfu to True",
+        )
+        self.assertTrue(
+            path.isfile(obfu.output_filename),
+            "default_obfuscation don't write the code",
+        )
+        self.assertTrue(
+            path.isfile("deobfuscate.json"),
+            "default_obfuscation don't write the deobfuscate file",
+        )
+
+        with open(obfu.output_filename) as file:
+            code = file.read()
+
+        self.assertNotEqual(
+            code, default_code, "default_obfuscation don't obfuscate the code"
+        )
+
+        import test_obfu
+
+        self.assertEqual(
+            "default_obfuscation test",
+            getattr(test_obfu, obfu.default_names["environ"].obfuscation)["test"],
+            "default_obfuscation don't obfuscate the correctly/good code",
+        )
+
+        # remove("test.py")
+        # remove("test_obfu.py")
+        remove("deobfuscate.json")
+
+    def test_get_attributes_from(self):
+        obfu = Obfuscator("")
+        mock1 = Mock()
+        mock1.test_attr = True
+
+        mock2 = Mock()
+        mock2 = obfu.get_attributes_from(mock2, mock1)
+
+        self.assertTrue(
+            mock2.test_attr,
+            "get_attributes_from don't set all attributes on the new object",
+        )
+
+    def test_delete_doc_string(self):
+        (doc, *_), (body_without_doc, *_), ast_doc_string, obfu = builds()
+
+        ast_test = obfu.delete_doc_string(ast_doc_string)
+
+        self.assertNotIn(
+            doc, ast_test.body, "delete_doc_string don't delete doc string"
+        )
+        self.assertListEqual(
+            ast_test.body,
+            body_without_doc,
+            "delete_doc_string don't delete only doc string",
+        )
+
+    def test_delete_field(self):
+        _, _, ast_with_body, obfu = builds()
+
+        ast_without_body = obfu.delete_field(ast_with_body, "body")
+
+        with self.assertRaises(AttributeError, msg="delete_field don't delete field"):
+            ast_without_body.body
+
+    def test_delete_annotations(self):
+        _, _, ast_with_annotation, obfu = builds()
+
+        ast_without_annotation = obfu.delete_annotations(ast_with_annotation)
+
+        with self.assertRaises(
+            AttributeError, msg="delete_annotations don't delete annotations"
+        ):
+            ast_without_annotation.annotation
+
+    def test_delete_returns(self):
+        _, _, ast_with_returns, obfu = builds()
+
+        ast_without_returns = obfu.delete_returns(ast_with_returns)
+
+        with self.assertRaises(
+            AttributeError, msg="delete_returns don't delete returns"
+        ):
+            ast_without_returns.returns
+
+    def test_get_targets_and_value_for_import(self):
+        elements = [ast.alias(name="dump"), ast.alias(name="Assign", asname="custom")]
+        module = "ast"
+
+        obfu = Obfuscator("")
+        obfu.get_random_name("xor")
+        # init_obfu_names(obfu)
+        obfu.init_builtins()
+        obfu.init_crypt_strings()
+        targets, values = obfu.get_targets_and_value_for_import(module, elements)
+
+        targets = obfu.visit(targets)
+        values = obfu.visit(values)
+
+        self.assertIsInstance(
+            targets,
+            ast.Tuple,
+            "get_targets_and_value_for_import don't return ast.Tuple object",
+        )
+        self.assertIsInstance(
+            values,
+            ast.Tuple,
+            "get_targets_and_value_for_import don't return ast.Tuple object",
+        )
+
+        for target in targets.elts:
+            self.assertIn(
+                obfu.obfu_names[target.id].name,
+                [
+                    element.__dict__.get("asname") or element.__dict__.get("name")
+                    for element in elements
+                ],
+                "get_targets_and_value_for_import return bad obfu name in first tuple",
+            )
+
+        for value in values.elts:
+            self.assertEqual(
+                value.args[0].func.id,
+                obfu.default_names["myimport"].obfuscation,
+                "get_targets_and_value_for_import don't return import function in second tuple",
+            )
+            self.assertEqual(
+                obfu.xor(value.args[0].args[0].func.args[0].args[0].value).decode(),
+                module,
+                "get_targets_and_value_for_import don't import the good function name in second tuple",
+            )
+            self.assertEqual(
+                value.func.id,
+                obfu.default_names["getattr"].obfuscation,
+                "get_targets_and_value_for_import don't return obfu __dict__ name in second tuple",
+            )
+            self.assertIn(
+                obfu.xor(value.args[1].func.args[0].args[0].value).decode(),
+                [element.name for element in elements],
+                "get_targets_and_value_for_import don't import the good element name in second tuple",
+            )
+
+    def test_visit_Import(self):
+        import1 = ast.Import(names=[ast.alias(name="os"), ast.alias(name="sys"), ast.alias(name="xml.dom.minidom"), ast.alias(name="urllib.request", asname="req")])
+
+        obfu = Obfuscator("", level=0)
+        obfu.init_crypt_strings()
+        import1 = obfu.visit_Import(import1)
+
+        self.assertIsInstance(
+            import1,
+            ast.Import,
+            "visit_Import don't return an ast.Import object with level 0",
+        )
+
+        obfu.level = 6
+        obfu.init_builtins()
+        assign = obfu.visit_Import(import1)
+
+        self.assertIsInstance(
+            assign, ast.Assign, "visit_Import don't return an ast.Assign object"
+        )
+
+        for name in assign.targets[0].elts:
+            self.assertIn(
+                obfu.obfu_names[name.id].name,
+                ["os", "sys", "xml", "req"],
+                "visit_Import don't assign the good variable name",
+            )
+
+        for call in assign.value.elts:
+            try:
+                first = True
+                module = obfu.xor(call.args[0].args[0].func.args[0].args[0].value).decode()
+            except:
+                first = False
+                module = obfu.xor(call.args[0].func.args[0].args[0].value).decode()
+            if first:
+                self.assertEqual(
+                    obfu.obfu_names[call.args[0].func.id].name,
+                    "myimport",
+                    "visit_Import don't call __import__ functions",
+                )
+                self.assertIn(
+                    module,
+                    ["urllib.request"],
+                    "visit_Import don't import good module",
+                )
+            else:
+                self.assertEqual(
+                    obfu.obfu_names[call.func.id].name,
+                    "__import__",
+                    "visit_Import don't call __import__ functions",
+                )
+                self.assertIn(
+                    module,
+                    ["os", "sys", 'xml.dom.minidom'],
+                    "visit_Import don't import good module",
+                )
+
+    def test_visit_ImportFrom(self):
+        import_from1 = ast.ImportFrom(
+            module="dataclasses", names=[ast.alias(name="dataclass")], level=0
+        )
+        import_from2 = ast.ImportFrom(
+            module="ast", names=[ast.alias(name="*")], level=0
+        )
+
+        ast_attr = [
+            attr
+            for attr in dir(ast)
+            if not (attr.startswith("__") and attr.endswith("__"))
+        ]
+
+        obfu = Obfuscator("", level=0)
+        obfu.init_crypt_strings()
+        import_from1 = obfu.visit_ImportFrom(import_from1)
+        self.assertIsInstance(
+            import_from1,
+            ast.ImportFrom,
+            "visit_ImportFrom don't return an ast.ImportFrom object with level 0",
+        )
+
+        obfu.level = 6
+        obfu.init_builtins()
+        assign = obfu.visit_ImportFrom(import_from1)
+
+        self.assertIsInstance(
+            assign, ast.Assign, "visit_ImportFrom don't return an ast.Assign object"
+        )
+
+        assign = obfu.visit_ImportFrom(import_from2)
+        self.assertEqual(
+            len(ast_attr),
+            len(assign.targets[0].elts),
+            "visit_ImportFrom don't import all attributes when import *",
+        )
+        obfu_ast_attr = [obfu.default_names[attr].obfuscation for attr in ast_attr]
+        self.assertListEqual(
+            obfu_ast_attr,
+            [name.id for name in assign.targets[0].elts],
+            "visit_ImportFrom don't import good attributes when import *",
+        )
+
+    def test_init_builtins(self):
+        global default_dir
+
+        obfu = Obfuscator("")
+        builtins_obfu = obfu.init_builtins()
+
+        elements = (
+            list(globals()["__builtins__"].keys())
+            if isinstance(__builtins__, dict)
+            else dir(__builtins__)
+        ) + default_dir
+
+        self.assertEqual(
+            builtins_obfu,
+            obfu.default_variables,
+            "init builtins obfuscation: Bad return value",
+        )
+
+        builtins_obfu = builtins_obfu.split("\n")[0]
+        obfu_builtins, builtins = builtins_obfu.split("=")
+        builtins, obfu_builtins = builtins.split(","), obfu_builtins.split(",")
+
+        self.assertEqual(
+            len(builtins),
+            len(obfu_builtins),
+            "len(builtins) is not equal to len(obfu_builtins) in init_builtins",
+        )
+
+        for i, obfu_name in enumerate(obfu_builtins):
+            self.assertEqual(
+                builtins[i],
+                obfu.obfu_names[obfu_name].name,
+                "order of builtins or obfuscate_name is not good",
+            )
+            self.assertIn(
+                builtins[i], elements, f"{builtins[i]} isn't in defaults variables"
+            )
+
+    def test_init_crypt_strings(self):
+        obfu1 = Obfuscator("")
+        code1, astcode1 = obfu1.init_crypt_strings()
+
+        obfu2 = Obfuscator("")
+        code2, astcode2 = obfu2.init_crypt_strings("abc='abc'")
+
+        for code, obfu in ((code1, obfu1), (code2, obfu2)):
+            self.assertIsNotNone(
+                obfu._xor_password_key, "init_crypt_strings don't set the xor key"
+            )
+            self.assertEqual(
+                len(obfu._xor_password_key),
+                obfu._xor_password_key_length,
+                "init_crypt_strings don't set the xor key with good length",
+            )
+
+            self.assertRegex(
+                code,
+                "^xor=lambda bytes_:\(bytes\(\[x\^\[([0-9]{1,3}(,[ ])?){40}\]\[i%40\] for i,x in enumerate\(bytes_\)\]\)\)\n.*$",
+                "init_crypt_strings don't return the good code",
+            )
+
+            exec(code)
+            encrypt = eval("xor(b'abc')")
+            self.assertEqual(
+                len(encrypt),
+                3,
+                "init_crypt_strings don't define xor lambda function",
+            )
+            self.assertEqual(
+                eval(f"xor({encrypt})"),
+                b"abc",
+                "init_crypt_strings don't decrypt correctly an encrypted bytes",
+            )
+
+    def test_xor(self):
+        obfu = Obfuscator("")
+
+        with self.assertRaises(
+            RuntimeError,
+            msg="xor don't raise RuntimeError when _xor_password_key is None",
+        ):
+            obfu.xor(b"abc")
+
+        obfu.init_crypt_strings()
+
+        self.assertEqual(
+            obfu.xor(obfu.xor(b"abc")),
+            b"abc",
+            "xor don't decrypt correctly an encrypted bytes",
+        )
+
+    def test_visit_ClassDef(self):
+        class_ = ast.ClassDef(
+            name="Test",
+            bases=[ast.Name(id="Classe", ctx=ast.Load())],
+            keywords=[],
+            body=[ast.Expr(value=ast.Constant(value=" Doc String "))],
+            decorator_list=[],
+        )
+
+        obfu = Obfuscator("", level=0)
+        class_ = obfu.visit_ClassDef(class_)
+
+        self.assertEqual(
+            class_.name, "Test", "visit_ClassDef change the class name with level 0"
+        )
+        self.assertEqual(
+            len(class_.body), 1, "visit_ClassDef delete doc string with level 0"
+        )
+
+        obfu.level = 6
+        class_ = obfu.visit_ClassDef(class_)
+
+        self.assertEqual(len(class_.body), 0, "visit_ClassDef don't delete doc string")
+        self.assertNotEqual(
+            class_.name, "Test", "visit_ClassDef don't change the class name"
+        )
+        self.assertEqual(
+            obfu.default_names["Test"].obfuscation,
+            class_.name,
+            "visit_ClassDef the new class name is bad",
+        )
+        self.assertEqual(
+            obfu.obfu_names[class_.name].name,
+            "Test",
+            "visit_ClassDef the new class name is bad",
+        )
+
+    def test_visit_FunctionDef(self):
+        function1 = ast.FunctionDef(
+            name="__init__",
+            args=ast.arguments(
+                posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[]
+            ),
+            body=[ast.Expr(value=ast.Constant(value=" Doc String "))],
+            decorator_list=[],
+        )
+
+        function2 = ast.FunctionDef(
+            name="init",
+            args=ast.arguments(
+                posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[]
+            ),
+            body=[ast.Expr(value=ast.Constant(value=" Doc String "))],
+            decorator_list=[],
+        )
+
+        obfu = Obfuscator("", level=0)
+        function = obfu.visit_FunctionDef(function2)
+        self.assertEqual(
+            function.name,
+            "init",
+            "visit_FunctionDef change the function name with level 0",
+        )
+        self.assertEqual(
+            len(function.body), 1, "visit_FunctionDef delete doc string with level 0"
+        )
+
+        obfu.level = 6
+
+        function = obfu.visit_FunctionDef(function2)
+        self.assertEqual(
+            len(function.body), 0, "visit_FunctionDef don't delete doc string"
+        )
+        self.assertNotEqual(
+            function.name, "init", "visit_FunctionDef don't change the function name"
+        )
+        self.assertEqual(
+            obfu.default_names["init"].obfuscation,
+            function.name,
+            "visit_FunctionDef the new function name is bad",
+        )
+        self.assertEqual(
+            obfu.obfu_names[function.name].name,
+            "init",
+            "visit_FunctionDef the new function name is bad",
+        )
+
+        function = obfu.visit_FunctionDef(function1)
+        self.assertEqual(
+            function.name,
+            "__init__",
+            "visit_FunctionDef change the magic function name",
+        )
+
+    def test_visit_Name(self):
+        name = ast.Name(id="name", ctx=ast.Store())
+
+        obfu = Obfuscator("", level=0)
+        name = obfu.visit_Name(name)
+        self.assertEqual(name.id, "name", "visit_Name change Name.id with level 0")
+
+        obfu.level = 6
+        name = obfu.visit_Name(name)
+
+        self.assertEqual(
+            obfu.default_names["name"].obfuscation,
+            name.id,
+            "visit_Name don't return a Name with a good id",
+        )
+
+    def test_visit_Global(self):
+        names = ["f0", "f1"]
+        global_ = ast.Global(names=names.copy())
+
+        obfu = Obfuscator("", level=0)
+        global_ = obfu.visit_Global(global_)
+        self.assertListEqual(
+            global_.names, names, "visit_Global change names with level 0"
+        )
+
+        obfu.level = 6
+        global_ = obfu.visit_Global(global_)
+
+        for i, name in enumerate(global_.names):
+            self.assertIn(
+                obfu.obfu_names[name].name,
+                names,
+                "visit_Global don't return good obfuscate names",
+            )
+            self.assertEqual(
+                obfu.obfu_names[name].name,
+                f"f{i}",
+                "visit_Global don't return names with good order",
+            )
+
+    def test_visit_arg(self):
+        arg = ast.arg(arg="arg", annotation=ast.Name(id="str", ctx=ast.Load()))
+
+        obfu = Obfuscator("", level=0)
+        arg = obfu.visit_arg(arg)
+
+        self.assertIsNotNone(arg.annotation, "visit_arg delete annotation with level 0")
+        self.assertEqual(
+            arg.annotation.id, "str", "visit_arg change annotation with level 0"
+        )
+
+        obfu.level = 6
+        arg = obfu.visit_arg(arg)
+
+        self.assertIsNone(arg.annotation, "visit_arg don't delete annotation")
+        self.assertEqual(
+            obfu.default_names["arg"].obfuscation,
+            arg.arg,
+            "visit_arg don't return arg(object) with good arg(attribute)",
+        )
+
+    def test_visit_AnnAssign(self):
+        assign = ast.AnnAssign(
+            target=ast.Name(id="abc", ctx=ast.Store()),
+            annotation=ast.Name(id="str", ctx=ast.Load()),
+            value=ast.Constant(value="abc"),
+            simple=1,
+        )
+
+        obfu = Obfuscator("", level=0)
+        assign = obfu.visit_AnnAssign(assign)
+
+        self.assertIsInstance(
+            assign,
+            ast.AnnAssign,
+            "visit_AnnAssign change AnnAssign object with level 0",
+        )
+
+        obfu.level = 6
+        obfu.init_crypt_strings()
+        assign = obfu.visit_AnnAssign(assign)
+
+        self.assertIsInstance(
+            assign, ast.Assign, "visit_AnnAssign don't build Assign object"
+        )
+        self.assertEqual(
+            obfu.obfu_names[assign.targets[0].id].name,
+            "abc",
+            "visit_AnnAssign don't assign the good variable name",
+        )
+        self.assertEqual(
+            obfu.xor(assign.value.func.args[0].args[0].value).decode(),
+            "abc",
+            "visit_AnnAssign don't assign the good value",
+        )
+
+    def test_write_deobfuscate(self):
+        obfu = Obfuscator("test.py", names={"a": Name("a", "b", False, None)})
+        obfu.write_deobfuscate()
+
+        self.assertTrue(
+            path.isfile("deobfuscate.json"),
+            "write_deobfuscate don't create deobfuscate file",
+        )
+
+        with open("deobfuscate.json") as file:
+            config = json.load(file)
+
+        self.assertDictEqual(
+            config["names"][0],
+            {
+                "name": "a",
+                "obfuscation_name": "b",
+                "definition": False,
+                "namespace": None,
+            },
+            "write_deobfuscate don't write good names.",
+        )
+        self.assertIsNone(config["encryption_key"])
+        self.assertDictEqual(
+            config["Obfuscator"],
+            {
+                "level": 6,
+                "default_obfuscation": False,
+                "encoding": "utf-8",
+                "output_file": "test_obfu.py",
+            },
+        )
+
+        remove("deobfuscate.json")
+        obfu.deobfuscate = False
+        obfu.write_deobfuscate()
+
+        self.assertFalse(
+            path.isfile("deobfuscate.json"),
+            "write_deobfuscate create deobfuscate file when deobfuscate is desactivated",
+        )
+
+    def test_add_builtins(self):
+        obfu = Obfuscator("")
+
+        with self.assertRaises(
+            RuntimeError,
+            msg="add_builtins don't raise Error if default_variables isn't defined",
+        ):
+            obfu.add_builtins()
+
+        obfu.default_variables = "p=print\n"
+
+        with self.assertRaises(
+            RuntimeError, msg="add_builtins don't raise Error if code isn't defined"
+        ):
+            obfu.add_builtins()
+
+        obfu.code = "p('Hello World !')"
+        obfu.add_builtins()
+
+        self.assertEqual(
+            obfu.code,
+            "p=print\n" + "p('Hello World !')",
+            "add_builtins don't return the good code",
+        )
+
+    def test_write_code(self):
+        obfu = Obfuscator("")
+
+        with self.assertRaises(
+            RuntimeError, msg="write_code don't raise Error if code isn't defined"
+        ):
+            obfu.write_code()
+
+        obfu.code = "print('Hello World !')"
+
+        code = obfu.write_code()
+
+        self.assertEqual(
+            code,
+            obfu.code,
+            "write_code don't return the good code",
+        )
+
+        with open("_obfu.py") as file:
+            self.assertEqual(
+                file.read(),
+                obfu.code,
+                "write_code don't write the good code",
+            )
+
+        # remove("_obfu.py")
+
+
+def init_obfu_names(obfu):
+    for name in dir(__builtins__):
+        obfu.get_random_name(name)
+
+
+def builds():
+    doc = ast.Expr(value=ast.Constant(value="abc"))
+    false_doc = ast.Expr(value=Mock())
+
+    AST_test = ast.AST(
+        body=[doc, false_doc], annotation="annotation", returns=ast.Constant(value=None)
+    )
+    AST_test._fields = tuple(AST_test.__dict__.keys())
+
+    body_without_doc = AST_test.body.copy()
+    body_without_doc.remove(doc)
+
+    obfu = Obfuscator("")
+    obfu.init_crypt_strings()
+
+    return (doc, false_doc), (body_without_doc,), AST_test, obfu
+
+
+def write_ast():
+    with open("code_using_for_test.py") as file:
+        python_code = file.read()
+
+    ast_code = ast.parse(python_code)
+
+    with open("ast_code_using_for_test.py", "w") as file:
+        file.write(ast.dump(ast_code, indent=4))
+
+
+if __name__ == "__main__":
+    # write_ast()
+    unittest.main()
+
+    """
+        - Check if all functions are tested
+        - Check if all fonctionnalities are tested in all functions
+        - Test commands lines and executables
+    """
```

