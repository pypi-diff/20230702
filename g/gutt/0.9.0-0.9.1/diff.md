# Comparing `tmp/gutt-0.9.0.tar.gz` & `tmp/gutt-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gutt-0.9.0.tar", max compression
+gzip compressed data, was "gutt-0.9.1.tar", max compression
```

## Comparing `gutt-0.9.0.tar` & `gutt-0.9.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1066 2021-07-17 10:44:45.174164 gutt-0.9.0/LICENSE
--rw-r--r--   0        0        0     3269 2022-02-21 13:23:39.045107 gutt-0.9.0/README.md
--rw-r--r--   0        0        0      620 2022-04-04 13:15:06.274601 gutt-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      123 2021-07-17 15:13:55.911586 gutt-0.9.0/src/gutt/__init__.py
--rw-r--r--   0        0        0      271 2022-04-04 13:15:14.610811 gutt-0.9.0/src/gutt/_meta.py
--rw-r--r--   0        0        0        0 2022-02-28 06:46:08.922342 gutt-0.9.0/src/gutt/cli/__init__.py
--rw-r--r--   0        0        0     7355 2022-04-04 12:40:42.366008 gutt-0.9.0/src/gutt/cli/main.py
--rw-r--r--   0        0        0     2226 2022-04-04 12:27:33.558527 gutt-0.9.0/src/gutt/model.py
--rw-r--r--   0        0        0     4310 2022-04-04 13:01:56.646695 gutt-0.9.0/src/gutt/template.py
--rw-r--r--   0        0        0     2685 2022-03-06 11:04:25.207359 gutt-0.9.0/src/gutt/utils.py
--rw-r--r--   0        0        0     4266 2022-04-04 13:25:52.914018 gutt-0.9.0/setup.py
--rw-r--r--   0        0        0     3974 2022-04-04 13:25:52.918371 gutt-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2021-07-17 10:44:45.174164 gutt-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3269 2022-02-21 13:23:39.045107 gutt-0.9.1/README.md
+-rw-r--r--   0        0        0      620 2022-07-09 07:32:01.901009 gutt-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      123 2021-07-17 15:13:55.911586 gutt-0.9.1/src/gutt/__init__.py
+-rw-r--r--   0        0        0      271 2022-07-09 07:32:18.318377 gutt-0.9.1/src/gutt/_meta.py
+-rw-r--r--   0        0        0        0 2022-02-28 06:46:08.922342 gutt-0.9.1/src/gutt/cli/__init__.py
+-rw-r--r--   0        0        0     7355 2022-04-04 12:40:42.366008 gutt-0.9.1/src/gutt/cli/main.py
+-rw-r--r--   0        0        0     2226 2022-04-04 12:27:33.558527 gutt-0.9.1/src/gutt/model.py
+-rw-r--r--   0        0        0     4352 2022-07-09 07:31:43.139453 gutt-0.9.1/src/gutt/template.py
+-rw-r--r--   0        0        0     2685 2022-03-06 11:04:25.207359 gutt-0.9.1/src/gutt/utils.py
+-rw-r--r--   0        0        0     4266 2022-07-09 07:33:50.968649 gutt-0.9.1/setup.py
+-rw-r--r--   0        0        0     3974 2022-07-09 07:33:50.969298 gutt-0.9.1/PKG-INFO
```

### Comparing `gutt-0.9.0/LICENSE` & `gutt-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gutt-0.9.0/README.md` & `gutt-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `gutt-0.9.0/pyproject.toml` & `gutt-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gutt"
-version = "0.9.0"
+version = "0.9.1"
 description = "Auto generate unit test templates"
 authors = ["Ryan <ryanchao2012@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ryanchao2012/gutt"
 
 [tool.poetry.dependencies]
```

### Comparing `gutt-0.9.0/src/gutt/cli/main.py` & `gutt-0.9.1/src/gutt/cli/main.py`

 * *Files identical despite different names*

### Comparing `gutt-0.9.0/src/gutt/model.py` & `gutt-0.9.1/src/gutt/model.py`

 * *Files identical despite different names*

### Comparing `gutt-0.9.0/src/gutt/template.py` & `gutt-0.9.1/src/gutt/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,17 @@
     def args(self):
         return arguments()
 
     @property
     def body(self):
         return [
             ImportFrom(
-                module=self._src.module.name, names=[alias(name=self._src.ast.name)]
+                module=self._src.module.name,
+                names=[alias(name=self._src.ast.name)],
+                level=0,
             ),
             Pass(),
         ]
 
 
 class MethodLayout(FunctionLayout):
     @property
```

### Comparing `gutt-0.9.0/src/gutt/utils.py` & `gutt-0.9.1/src/gutt/utils.py`

 * *Files identical despite different names*

### Comparing `gutt-0.9.0/setup.py` & `gutt-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['asttrs<1.0.0', 'black<23.0.0', 'click<9.0.0', 'isort<6.0.0']
 
 entry_points = \
 {'console_scripts': ['gutt = gutt.cli.main:main']}
 
 setup_kwargs = {
     'name': 'gutt',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Auto generate unit test templates',
     'long_description': "![](https://github.com/ryanchao2012/gutt/actions/workflows/gutt-run-unittests.yml/badge.svg)\n![](https://img.shields.io/pypi/v/gutt.svg)\n![](https://img.shields.io/pypi/pyversions/gutt)\n![](https://img.shields.io/github/license/ryanchao2012/gutt)\n\n# gutt\nAuto Generate Unit Test Templates\n\n\n## Install\n\n```\n$ pip install gutt\n```\n\n\n## Basic Usage\n\nAssume you have a package, and its layout:\n\n```\nmy_awesome_package\n├── __init__.py\n└── module1.py\n```\n\nsome codes inside `my_awesome_package/module1.py`:\n\n```python\n\nimport sys\n\nMY_CONST = 123\n\ndef funcion1():\n    pass\n\n\ndef function2():\n    pass\n\n\nclass MyObject:\n    def method1(self):\n        pass\n\n    @classmethod\n    def classmethod1(cls):\n        pass\n\n    @staticmethod\n    def staticmethod1():\n        pass\n\n```\n\n`gutt` can generate unit testing templates for all implementations in just one line:\n\n```\n$ gutt -m my_awesome_package -o mytests\n```\n\nThe output layout:\n\n```\nmytests\n├── __init__.py\n└── my_awesome_package\n    ├── __init__.py\n    └── test_module1.py\n\n```\n\nThe unit test templates inside `test_module1.py`\n\n```python\ndef test_funcion1():\n    from my_awesome_package.module1 import funcion1\n\n    assert funcion1\n\n\ndef test_function2():\n    from my_awesome_package.module1 import function2\n\n    assert function2\n\n\nclass TestMyObject:\n    @classmethod\n    def setup_class(cls):\n        from my_awesome_package.module1 import MyObject\n\n        assert MyObject\n\n    @classmethod\n    def teardown_class(cls):\n        pass\n\n    def setup_method(self, method):\n        pass\n\n    def teardown_method(self, method):\n        pass\n\n    def test_method1(self):\n        pass\n\n    def test_classmethod1(self):\n        pass\n\n    def test_staticmethod1(self):\n        pass\n\n```\n\nEach module in source codes maps to a testing module(`module1.py --> test_module1.py`), and each function, each class and all methods inside that class maps to corresponding test templates. \n\n- `gutt` will skip code generation if the test templates for the functions already exist.\n- `gutt` won't delete the corresponding test templates if the source codes get deleted or renamed.\n- For new added codes: modules, functions or methods inside class, just re-run `gutt` to generate new test templates for them.\n\n\nRun unit test with `pytest`, for example:\n\n```\n$ pytest --doctest-modules --cov=my_awesome_package mytests\n\n=============================== test session starts ===============================\nplatform linux -- Python 3.8.8, pytest-4.6.11, py-1.10.0, pluggy-0.13.1\nrootdir: /home/ryan/Workspace/my_awesome_package\nplugins: mock-1.13.0, cov-2.11.1\ncollected 5 items                                                                 \n\nmytests/my_awesome_package/test_module1.py .....                            [100%]\n\n----------- coverage: platform linux, python 3.8.8-final-0 -----------\nName                             Stmts   Miss  Cover\n----------------------------------------------------\nmy_awesome_package/__init__.py       0      0   100%\nmy_awesome_package/module1.py       13      5    62%\n----------------------------------------------------\nTOTAL                               13      5    62%\n\n\n============================ 5 passed in 0.07 seconds =============================\n```",
     'author': 'Ryan',
     'author_email': 'ryanchao2012@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ryanchao2012/gutt',
```

### Comparing `gutt-0.9.0/PKG-INFO` & `gutt-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gutt
-Version: 0.9.0
+Version: 0.9.1
 Summary: Auto generate unit test templates
 Home-page: https://github.com/ryanchao2012/gutt
 License: MIT
 Author: Ryan
 Author-email: ryanchao2012@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

