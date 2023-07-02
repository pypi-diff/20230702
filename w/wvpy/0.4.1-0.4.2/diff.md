# Comparing `tmp/wvpy-0.4.1.tar.gz` & `tmp/wvpy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wvpy-0.4.1.tar", last modified: Thu Apr 27 00:11:11 2023, max compression
+gzip compressed data, was "wvpy-0.4.2.tar", last modified: Sun Jul  2 18:15:23 2023, max compression
```

## Comparing `wvpy-0.4.1.tar` & `wvpy-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-27 00:11:11.150036 wvpy-0.4.1/
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-27 00:11:11.145807 wvpy-0.4.1/Doc/
--rw-r--r--   0 johnmount   (501) staff       (20)      108 2019-07-23 14:11:39.000000 wvpy-0.4.1/Doc/documentation.txt
--rw-r--r--   0 johnmount   (501) staff       (20)     1494 2019-07-23 14:35:20.000000 wvpy-0.4.1/LICENSE
--rw-r--r--   0 johnmount   (501) staff       (20)       82 2019-07-23 14:11:39.000000 wvpy-0.4.1/MANIFEST.in
--rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-04-27 00:11:11.149743 wvpy-0.4.1/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)      373 2022-12-29 19:46:58.000000 wvpy-0.4.1/README.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-04-27 00:11:11.150116 wvpy-0.4.1/setup.cfg
--rw-r--r--   0 johnmount   (501) staff       (20)     1367 2023-04-11 19:46:06.000000 wvpy-0.4.1/setup.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-27 00:11:11.147225 wvpy-0.4.1/wvpy/
--rw-r--r--   0 johnmount   (501) staff       (20)      173 2023-04-11 19:46:02.000000 wvpy-0.4.1/wvpy/__init__.py
--rw-r--r--   0 johnmount   (501) staff       (20)    20444 2023-04-26 23:33:57.000000 wvpy-0.4.1/wvpy/jtools.py
--rw-r--r--   0 johnmount   (501) staff       (20)     5898 2022-12-29 19:46:58.000000 wvpy-0.4.1/wvpy/pysheet.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3234 2022-12-29 19:46:58.000000 wvpy-0.4.1/wvpy/render_workbook.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-27 00:11:11.149308 wvpy-0.4.1/wvpy.egg-info/
--rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)      272 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/SOURCES.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/dependency_links.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       69 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/requires.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        5 2023-04-27 00:11:11.000000 wvpy-0.4.1/wvpy.egg-info/top_level.txt
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-07-02 18:15:23.994511 wvpy-0.4.2/
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-07-02 18:15:23.991641 wvpy-0.4.2/Doc/
+-rw-r--r--   0 johnmount   (501) staff       (20)      108 2023-07-02 14:36:25.000000 wvpy-0.4.2/Doc/documentation.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)     1494 2023-07-02 14:36:25.000000 wvpy-0.4.2/LICENSE
+-rw-r--r--   0 johnmount   (501) staff       (20)       82 2023-07-02 14:36:25.000000 wvpy-0.4.2/MANIFEST.in
+-rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-07-02 18:15:23.994270 wvpy-0.4.2/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)      373 2023-07-02 14:36:25.000000 wvpy-0.4.2/README.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-07-02 18:15:23.994573 wvpy-0.4.2/setup.cfg
+-rw-r--r--   0 johnmount   (501) staff       (20)     1367 2023-07-02 14:36:25.000000 wvpy-0.4.2/setup.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-07-02 18:15:23.991878 wvpy-0.4.2/tests/
+-rw-r--r--   0 johnmount   (501) staff       (20)     7779 2023-07-02 16:47:54.000000 wvpy-0.4.2/tests/test_nb_fns.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-07-02 18:15:23.992878 wvpy-0.4.2/wvpy/
+-rw-r--r--   0 johnmount   (501) staff       (20)      173 2023-07-02 14:36:25.000000 wvpy-0.4.2/wvpy/__init__.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    21552 2023-07-02 17:12:26.000000 wvpy-0.4.2/wvpy/jtools.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     5898 2023-07-02 14:36:25.000000 wvpy-0.4.2/wvpy/pysheet.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3234 2023-07-02 14:36:25.000000 wvpy-0.4.2/wvpy/render_workbook.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-07-02 18:15:23.993978 wvpy-0.4.2/wvpy.egg-info/
+-rw-r--r--   0 johnmount   (501) staff       (20)      995 2023-07-02 18:15:23.000000 wvpy-0.4.2/wvpy.egg-info/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)      293 2023-07-02 18:15:23.000000 wvpy-0.4.2/wvpy.egg-info/SOURCES.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-07-02 18:15:23.000000 wvpy-0.4.2/wvpy.egg-info/dependency_links.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       69 2023-07-02 18:15:23.000000 wvpy-0.4.2/wvpy.egg-info/requires.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        5 2023-07-02 18:15:23.000000 wvpy-0.4.2/wvpy.egg-info/top_level.txt
```

### Comparing `wvpy-0.4.1/LICENSE` & `wvpy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wvpy-0.4.1/PKG-INFO` & `wvpy-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wvpy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Convert Jupyter notebooks to and from Python files.
 Home-page: https://github.com/WinVector/wvpy
 Author: John Mount
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `wvpy-0.4.1/setup.py` & `wvpy-0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 DESCRIPTION = "Convert Jupyter notebooks to and from Python files."
 LONG_DESCRIPTION = """
 Convert Jupyter notebooks to and from Python files.
 """
 
 setuptools.setup(
     name="wvpy",
-    version="0.4.1",
+    version="0.4.2",
     author="John Mount",
     author_email="jmount@win-vector.com",
     url="https://github.com/WinVector/wvpy",
     packages=setuptools.find_packages(exclude=['tests', 'Examples']),
     install_requires=[
         "IPython",
         "nbformat",
```

### Comparing `wvpy-0.4.1/wvpy/jtools.py` & `wvpy-0.4.2/wvpy/jtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import datetime
 import os
 import nbformat
 from nbconvert import HTMLExporter
 from nbconvert.preprocessors import ExecutePreprocessor
 from multiprocessing import Pool
 import sys
+import pickle
+import tempfile
 
 from typing import Iterable, List, Optional
 from functools import total_ordering
 
 have_pdf_kit = False
 try:
     import pdfkit
@@ -283,29 +285,31 @@
 def render_as_html(
     notebook_file_name: str,
     *,
     output_suffix: Optional[str] = None,
     timeout:int = 60000,
     kernel_name: Optional[str] = None,
     verbose: bool = True,
+    sheet_vars = None,
     init_code: Optional[str] = None,
     exclude_input: bool = False,
     prompt_strip_regexp: Optional[str] = r'<\s*div\s+class\s*=\s*"jp-OutputPrompt[^<>]*>[^<>]*Out[^<>]*<\s*/div\s*>',
     convert_to_pdf: bool = False,
 ) -> None:
     """
     Render a Jupyter notebook in the current directory as HTML.
     Exceptions raised in the rendering notebook are allowed to pass trough.
 
     :param notebook_file_name: name of source file, must end with .ipynb or .py (or type gotten from file system)
     :param output_suffix: optional name to add to result name
     :param timeout: Maximum time in seconds each notebook cell is allowed to run.
                     passed to nbconvert.preprocessors.ExecutePreprocessor.
     :param kernel_name: Jupyter kernel to use. passed to nbconvert.preprocessors.ExecutePreprocessor.
-    :param verbose logical, if True print while running 
+    :param verbose logical, if True print while running
+    :param sheet_vars: if not None value is de-serialized as a variable named "sheet_vars"
     :param init_code: Python init code for first cell
     :param exclude_input: if True, exclude input cells
     :param prompt_strip_regexp: regexp to strip prompts, only used if exclude_input is True
     :param convert_to_pdf: if True convert HTML to PDF, and delete HTML
     :return: None
     """
     assert isinstance(notebook_file_name, str)
@@ -331,15 +335,28 @@
     elif notebook_file_name.endswith(".py"):
         suffix = ".py"
         with open(notebook_file_name, 'r') as f:
             text = f.read()
         nb = convert_py_code_to_notebook(text)
     else:
         raise ValueError('{ipynb_exists}: file must end with .py or .ipynb')
+    tmp_path = None
     # do the conversion
+    if sheet_vars is not None:
+        with tempfile.NamedTemporaryFile(delete=False) as ntf:
+            tmp_path = ntf.name
+            pickle.dump(sheet_vars, file=ntf)
+        if (init_code is None) or (len(init_code) <= 0):
+            init_code = ""
+        pickle_code = f"""
+import pickle
+with open({tmp_path.__repr__()}, 'rb') as pf:
+   sheet_vars = pickle.load(pf)
+""" 
+        init_code = init_code + "\n\n" + pickle_code
     if (init_code is not None) and (len(init_code) > 0):
         assert isinstance(init_code, str)
         nb = prepend_code_cell_to_notebook(
             nb, 
             code_text=f'\n\n{init_code}\n\n')
     html_name = os.path.basename(notebook_file_name)
     html_name = html_name.removesuffix(suffix)
@@ -380,38 +397,49 @@
         else:
             assert have_pdf_kit
             pdf_name = html_name.removesuffix('.html') + '.pdf'
             pdfkit.from_string(html_body, pdf_name)
         caught = ep.caught_exception
     except Exception as e:
         caught = e
+    if tmp_path is not None:
+        try:
+            os.remove(tmp_path)
+        except FileNotFoundError:
+            pass
     if caught is not None:
         raise caught
     if verbose:
         print(f'\tdone render_as_html "{html_name}" {datetime.datetime.now()}')
 
 
+_jtask_comparison_attributes = [
+    "sheet_name", "output_suffix", "exclude_input", "init_code", "path_prefix"]
+
+
 @total_ordering
 class JTask:
     def __init__(
         self,
         sheet_name: str,
         *,
         output_suffix: Optional[str] = None,
         exclude_input: bool = True,
+        sheet_vars = None,
         init_code: Optional[str] = None,
         path_prefix: Optional[str] = None,
         strict: bool = True,
     ) -> None:
         """
         Create a Jupyter task.
 
         :param sheet_name: name of sheet to run can be .ipynb or .py, and suffix can be omitted.
         :param output_suffix: optional string to append to rendered HTML file name.
         :param exclude_input: if True strip input cells out of HTML render.
+        :param sheet_vars: if not None value is de-serialized as a variable named "sheet_vars"
         :param init_code: optional code to insert at the top of the Jupyter sheet, used to pass parameters.
         :param path_prefix: optional prefix to add to sheet_name to find Jupyter source. 
         :param strict: if True check paths path_prefix and path_prefix/sheetname[.py|.ipynb] exist.
         """
         assert isinstance(sheet_name, str)
         assert isinstance(output_suffix, (str, type(None)))
         assert isinstance(exclude_input, bool)
@@ -428,63 +456,71 @@
                 path = path.removesuffix(".ipynb")
             py_exists = os.path.exists(path + ".py")
             ipynb_exists = os.path.exists(path + ".ipynb")
             assert (py_exists + ipynb_exists) == 1
         self.sheet_name = sheet_name
         self.output_suffix = output_suffix
         self.exclude_input = exclude_input
+        self.sheet_vars = sheet_vars
         self.init_code = init_code
         self.path_prefix = path_prefix
 
     def render_as_html(self) -> None:
         path = self.sheet_name
         if isinstance(self.path_prefix, str) and (len(self.path_prefix) > 0):
             path = os.path.join(self.path_prefix, self.sheet_name)
         render_as_html(
             path,
             exclude_input=self.exclude_input,
             output_suffix=self.output_suffix,
+            sheet_vars=self.sheet_vars,
             init_code=self.init_code,
         )
 
     def __getitem__(self, item):
          return getattr(self, item)
 
     def _is_valid_operand(self, other):
         return isinstance(other, JTask)
 
     def __eq__(self, other):
         if not self._is_valid_operand(other):
-            return NotImplemented
+            return False
         if str(type(self)) != str(type(other)):
             return False
-        for v in ["sheet_name", "output_suffix", "exclude_input", "init_code", "path_prefix"]:
+        for v in _jtask_comparison_attributes:
             if self[v] != other[v]:
                 return False
+        if str(self.sheet_vars) != str(other.sheet_vars):
+            return False
         return True
 
     def __lt__(self, other):
         if not self._is_valid_operand(other):
             return NotImplemented
         if str(type(self)) < str(type(other)):
             return True
-        for v in ["sheet_name", "output_suffix", "exclude_input", "init_code", "path_prefix"]:
+        for v in _jtask_comparison_attributes:
             v_self = self[v]
             v_other = other[v]
             # can't order compare None to None
-            if ((v_self is None) or (v_other is None)) and ((v_self is None) != (v_other is None)):
-                return v_self is None
-            if self[v] < other[v]:
-                return True
+            if ((v_self is None) or (v_other is None)):
+                if ((v_self is None) != (v_other is None)):
+                    return v_self is None
+            else:
+                if self[v] < other[v]:
+                    return True
+        if str(self.sheet_vars) < str(other.sheet_vars):
+            return True
         return False
     
     def __str__(self) -> str:
         args_str = ",\n".join([
-            f" {v}= {repr(self[v])}"
-            for v in ["sheet_name", "output_suffix", "exclude_input", "init_code", "path_prefix"]
+            f" {v}={repr(self[v])}"
+            for v in _jtask_comparison_attributes + ["sheet_vars"]
         ])
         return 'JTask(\n' + args_str + ",\n)"
 
     def __repr__(self) -> str:
         return self.__str__()
```

### Comparing `wvpy-0.4.1/wvpy/pysheet.py` & `wvpy-0.4.2/wvpy/pysheet.py`

 * *Files identical despite different names*

### Comparing `wvpy-0.4.1/wvpy/render_workbook.py` & `wvpy-0.4.2/wvpy/render_workbook.py`

 * *Files identical despite different names*

### Comparing `wvpy-0.4.1/wvpy.egg-info/PKG-INFO` & `wvpy-0.4.2/wvpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wvpy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Convert Jupyter notebooks to and from Python files.
 Home-page: https://github.com/WinVector/wvpy
 Author: John Mount
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

