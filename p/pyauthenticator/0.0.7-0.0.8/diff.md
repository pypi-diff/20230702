# Comparing `tmp/pyauthenticator-0.0.7.tar.gz` & `tmp/pyauthenticator-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyauthenticator-0.0.7.tar", last modified: Mon Mar 27 16:57:08 2023, max compression
+gzip compressed data, was "pyauthenticator-0.0.8.tar", last modified: Sun Jul  2 18:13:15 2023, max compression
```

## Comparing `pyauthenticator-0.0.7.tar` & `pyauthenticator-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:57:08.857568 pyauthenticator-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 16:57:08.857568 pyauthenticator-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:57:08.857568 pyauthenticator-0.0.7/pyauthenticator/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/pyauthenticator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/pyauthenticator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-27 16:57:08.857568 pyauthenticator-0.0.7/pyauthenticator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/pyauthenticator/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:57:08.857568 pyauthenticator-0.0.7/pyauthenticator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 16:57:08.000000 pyauthenticator-0.0.7/pyauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-27 16:57:08.000000 pyauthenticator-0.0.7/pyauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 16:57:08.000000 pyauthenticator-0.0.7/pyauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-27 16:57:08.000000 pyauthenticator-0.0.7/pyauthenticator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-27 16:57:08.000000 pyauthenticator-0.0.7/pyauthenticator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 16:57:08.000000 pyauthenticator-0.0.7/pyauthenticator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-27 16:57:08.857568 pyauthenticator-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-27 16:57:08.000000 pyauthenticator-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:57:08.857568 pyauthenticator-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/tests/test_share.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/tests/test_user_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-27 16:57:05.000000 pyauthenticator-0.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:13:15.208463 pyauthenticator-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-02 18:13:15.208463 pyauthenticator-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:13:15.208463 pyauthenticator-0.0.8/pyauthenticator/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/pyauthenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/pyauthenticator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-02 18:13:15.208463 pyauthenticator-0.0.8/pyauthenticator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/pyauthenticator/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:13:15.208463 pyauthenticator-0.0.8/pyauthenticator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-02 18:13:15.000000 pyauthenticator-0.0.8/pyauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-02 18:13:15.000000 pyauthenticator-0.0.8/pyauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 18:13:15.000000 pyauthenticator-0.0.8/pyauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-02 18:13:15.000000 pyauthenticator-0.0.8/pyauthenticator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-02 18:13:15.000000 pyauthenticator-0.0.8/pyauthenticator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 18:13:15.000000 pyauthenticator-0.0.8/pyauthenticator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-02 18:13:15.208463 pyauthenticator-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-02 18:13:14.000000 pyauthenticator-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:13:15.208463 pyauthenticator-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/tests/test_share.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/tests/test_user_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-02 18:13:09.000000 pyauthenticator-0.0.8/versioneer.py
```

### Comparing `pyauthenticator-0.0.7/LICENSE` & `pyauthenticator-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyauthenticator-0.0.7/PKG-INFO` & `pyauthenticator-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauthenticator
-Version: 0.0.7
+Version: 0.0.8
 Summary: Similar to the Google authenticator just written in python.
 Home-page: https://github.com/pyscioffice/pyauthenticator
 Author: Jan Janssen
 Author-email: jan.janssen@outlook.com
 License: BSD
 License-File: LICENSE
```

### Comparing `pyauthenticator-0.0.7/README.md` & `pyauthenticator-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyauthenticator-0.0.7/pyauthenticator/__init__.py` & `pyauthenticator-0.0.8/pyauthenticator/__init__.py`

 * *Files identical despite different names*

### Comparing `pyauthenticator-0.0.7/pyauthenticator/__main__.py` & `pyauthenticator-0.0.8/tests/test_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 """
-Generate two factor authentication codes on the command line
+Test for core functionality
 """
-import argparse
-from pyauthenticator.share import (
-    list_services,
-    load_config,
-    generate_qrcode,
-    add_service,
-    get_two_factor_code,
-)
-
-
-def command_line_parser():
-    """
-    Main function primarly used for the command line interface
-    """
-    parser = argparse.ArgumentParser(prog="pyauthenticator")
-    config_dict = load_config()
-    parser.add_argument(
-        "service",
-        help="Service to generate optauth code for. Available services are: "
-        + str(list_services(config_dict=config_dict)),
-    )
-    parser.add_argument(
-        "-qr",
-        "--qrcode",
-        action="store_true",
-        help="Generate qrcode as <service.png> file.",
-    )
-    parser.add_argument(
-        "-a",
-        "--add",
-        help="Add service by providing the qrcode png file as additional argument.",
-    )
-    args = parser.parse_args()
-    if args.qrcode:
-        generate_qrcode(key=args.service, config_dict=config_dict)
-    elif args.add:
+import unittest
+from pyauthenticator.share import list_services, load_config, generate_qrcode, add_service, get_two_factor_code
+import os
+
+
+class TestCore(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls):
+        cls.qr_code_png = "test.png"
+        cls.config_dict = {
+            "test": "otpauth://totp/Test%3A%20root%40github.com?secret=6IQXETC4ADOSMMUN&issuer=Test&period=60"
+        }
+        generate_qrcode(
+            key="test",
+            config_dict=cls.config_dict,
+            file_name=None
+        )
+
+    @classmethod
+    def tearDownClass(cls):
+        os.remove(cls.qr_code_png)
+
+    def test_list_services(self):
+        service_lst = list_services(config_dict=self.config_dict)
+        self.assertEqual(["test"], service_lst)
+
+    def test_add_service(self):
+        config_file = "test_config.json"
         add_service(
-            key=args.service, qrcode_png_file_name=args.add, config_dict=config_dict
+            key="test",
+            qrcode_png_file_name=self.qr_code_png,
+            config_dict={},
+            config_file_to_write=config_file
         )
-        print(args.service, "added.")
-    else:
-        print(get_two_factor_code(key=args.service, config_dict=config_dict))
+        config_reload = load_config(config_file_to_load=config_file)
+        self.assertDictEqual(config_reload, self.config_dict)
+        os.remove(config_file)
+
+    def test_get_two_factor_code(self):
+        code = get_two_factor_code(key="test", config_dict=self.config_dict)
+        self.assertEqual(len(code), 6)
 
 
-if __name__ == "__main__":
-    command_line_parser()
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `pyauthenticator-0.0.7/pyauthenticator/share.py` & `pyauthenticator-0.0.8/pyauthenticator/share.py`

 * *Files identical despite different names*

### Comparing `pyauthenticator-0.0.7/pyauthenticator.egg-info/PKG-INFO` & `pyauthenticator-0.0.8/pyauthenticator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyauthenticator
-Version: 0.0.7
+Version: 0.0.8
 Summary: Similar to the Google authenticator just written in python.
 Home-page: https://github.com/pyscioffice/pyauthenticator
 Author: Jan Janssen
 Author-email: jan.janssen@outlook.com
 License: BSD
 License-File: LICENSE
```

### Comparing `pyauthenticator-0.0.7/setup.py` & `pyauthenticator-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     author_email='jan.janssen@outlook.com',
     license='BSD',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
         'otpauth>=2.0.0',
         'qrcode>=7.4.2',
         'pyzbar>=0.1.9',
-        'pillow>=9.4.0',
+        'pillow>=9.5.0',
     ],
     cmdclass=versioneer.get_cmdclass(),
     entry_points={
         "console_scripts": [
             'pyauthenticator=pyauthenticator.__main__:command_line_parser'
         ]
     }
```

### Comparing `pyauthenticator-0.0.7/tests/test_core.py` & `pyauthenticator-0.0.8/tests/test_user_interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,29 @@
-"""
-Test for core functionality
-"""
 import unittest
-from pyauthenticator.share import list_services, load_config, generate_qrcode, add_service, get_two_factor_code
 import os
+from pyauthenticator import get_two_factor_code, write_qrcode_to_file
+from pyauthenticator.share import expand_path, write_config, config_file
 
 
-class TestCore(unittest.TestCase):
+class TestUserInterface(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.qr_code_png = "test.png"
         cls.config_dict = {
-            "test": "otpauth://totp/Test%3A%20root%40github.com?secret=6IQXETC4ADOSMMUN&issuer=Test&period=60"
+            "test": "otpauth://totp/Test%3A%20root%40github.com?secret=6IQXETC4ADOSMMUN&issuer=Test"
         }
-        generate_qrcode(
-            key="test",
-            config_dict=cls.config_dict,
-            file_name=None
-        )
-
-    @classmethod
-    def tearDownClass(cls):
-        os.remove(cls.qr_code_png)
-
-    def test_list_services(self):
-        service_lst = list_services(config_dict=self.config_dict)
-        self.assertEqual(["test"], service_lst)
-
-    def test_add_service(self):
-        config_file = "test_config.json"
-        add_service(
-            key="test",
-            qrcode_png_file_name=self.qr_code_png,
-            config_dict={},
-            config_file_to_write=config_file
-        )
-        config_reload = load_config(config_file_to_load=config_file)
-        self.assertDictEqual(config_reload, self.config_dict)
-        os.remove(config_file)
+        cls.config_path = expand_path(config_file)
+        if not os.path.exists(cls.config_path):
+            write_config(
+                config_dict=cls.config_dict
+            )
 
     def test_get_two_factor_code(self):
-        code = get_two_factor_code(key="test", config_dict=self.config_dict)
+        code = get_two_factor_code(service="test")
         self.assertEqual(len(code), 6)
 
+    def test_write_qrcode_to_file(self):
+        write_qrcode_to_file(service="test")
+        self.assertTrue(os.path.exists("test.png"))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pyauthenticator-0.0.7/tests/test_share.py` & `pyauthenticator-0.0.8/tests/test_share.py`

 * *Files identical despite different names*

### Comparing `pyauthenticator-0.0.7/versioneer.py` & `pyauthenticator-0.0.8/versioneer.py`

 * *Files identical despite different names*

