# Comparing `tmp/pygount-1.6.0.tar.gz` & `tmp/pygount-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygount-1.6.0.tar", max compression
+gzip compressed data, was "pygount-1.6.1.tar", max compression
```

## Comparing `pygount-1.6.0.tar` & `pygount-1.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1488 2023-01-02 08:17:33.701239 pygount-1.6.0/LICENSE.txt
--rw-r--r--   0        0        0     4888 2023-06-25 23:16:15.321381 pygount-1.6.0/README.md
--rw-r--r--   0        0        0      685 2023-06-02 15:02:53.678813 pygount-1.6.0/pygount/__init__.py
--rw-r--r--   0        0        0    35084 2023-06-25 23:13:58.547023 pygount-1.6.0/pygount/analysis.py
--rw-r--r--   0        0        0    15396 2023-06-06 08:13:21.872180 pygount-1.6.0/pygount/command.py
--rw-r--r--   0        0        0     6476 2023-06-13 20:37:39.920761 pygount-1.6.0/pygount/common.py
--rw-r--r--   0        0        0     1371 2023-06-25 22:16:01.849583 pygount-1.6.0/pygount/git_storage.py
--rw-r--r--   0        0        0     2085 2023-01-02 08:17:33.702607 pygount-1.6.0/pygount/lexers.py
--rw-r--r--   0        0        0     9253 2023-01-02 08:17:33.702836 pygount-1.6.0/pygount/summary.py
--rw-r--r--   0        0        0    10648 2023-06-02 16:31:08.551599 pygount-1.6.0/pygount/write.py
--rw-r--r--   0        0        0     4296 2023-01-02 08:17:33.703237 pygount-1.6.0/pygount/xmldialect.py
--rw-r--r--   0        0        0     2093 2023-06-14 17:19:06.908521 pygount-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     6315 1970-01-01 00:00:00.000000 pygount-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-01-02 08:17:33.701239 pygount-1.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     4888 2023-06-25 23:16:15.321381 pygount-1.6.1/README.md
+-rw-r--r--   0        0        0      685 2023-06-02 15:02:53.678813 pygount-1.6.1/pygount/__init__.py
+-rw-r--r--   0        0        0    35167 2023-06-30 16:03:18.509620 pygount-1.6.1/pygount/analysis.py
+-rw-r--r--   0        0        0    15396 2023-06-06 08:13:21.872180 pygount-1.6.1/pygount/command.py
+-rw-r--r--   0        0        0     6476 2023-06-13 20:37:39.920761 pygount-1.6.1/pygount/common.py
+-rw-r--r--   0        0        0     1371 2023-06-25 22:16:01.849583 pygount-1.6.1/pygount/git_storage.py
+-rw-r--r--   0        0        0     2085 2023-01-02 08:17:33.702607 pygount-1.6.1/pygount/lexers.py
+-rw-r--r--   0        0        0     9253 2023-01-02 08:17:33.702836 pygount-1.6.1/pygount/summary.py
+-rw-r--r--   0        0        0    10648 2023-06-02 16:31:08.551599 pygount-1.6.1/pygount/write.py
+-rw-r--r--   0        0        0     4296 2023-01-02 08:17:33.703237 pygount-1.6.1/pygount/xmldialect.py
+-rw-r--r--   0        0        0     2138 2023-06-30 16:03:18.509974 pygount-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6315 1970-01-01 00:00:00.000000 pygount-1.6.1/PKG-INFO
```

### Comparing `pygount-1.6.0/LICENSE.txt` & `pygount-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/README.md` & `pygount-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/pygount/__init__.py` & `pygount-1.6.1/pygount/__init__.py`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/pygount/analysis.py` & `pygount-1.6.1/pygount/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -722,14 +722,19 @@
         if token_text.endswith("\n"):
             yield line_marks
             line_marks = set()
     if len(line_marks) >= 1:
         yield line_marks
 
 
+def check_file_handle_is_seekable(file_handle: Optional[Union[BufferedIOBase, RawIOBase]], source_path: str):
+    if not file_handle.seekable():
+        raise pygount.Error(f"cannot determine encoding: file handle must be seekable: {source_path}")
+
+
 def encoding_for(
     source_path: str,
     encoding: str = "automatic",
     fallback_encoding: Optional[str] = None,
     file_handle: Optional[Union[BufferedIOBase, RawIOBase]] = None,
 ) -> str:
     """
@@ -751,18 +756,15 @@
     assert encoding is not None
 
     if encoding == "automatic":
         if file_handle is None:
             with open(source_path, "rb") as source_file:
                 heading = source_file.read(128)
         else:
-            if not file_handle.seekable:
-                raise pygount.Error(
-                    f"cannot automatically determine encoding: file handle must be seekable: {source_path}"
-                )
+            check_file_handle_is_seekable(file_handle, source_path)
             heading = file_handle.read(128)
             file_handle.seek(-len(heading), SEEK_CUR)
         result = None
         if len(heading) == 0:
             # File is empty, assume a dummy encoding.
             result = "utf-8"
         if result is None:
@@ -790,16 +792,15 @@
             _detector is not None
         ), 'without chardet installed, encoding="chardet" must be rejected before calling encoding_for()'
         _detector.reset()
         if file_handle is None:
             with open(source_path, "rb") as source_file:
                 lines = source_file.readlines()
         else:
-            if not file_handle.seekable:
-                raise pygount.Error(f"cannot determine encoding: file handle must be seekable: {source_path}")
+            check_file_handle_is_seekable(file_handle, source_path)
             file_position = file_handle.tell()
             lines = file_handle.readlines()
             file_handle.seek(file_position)
         for line in lines:
             _detector.feed(line)
             if _detector.done:
                 break
@@ -820,17 +821,18 @@
         else:
             try:
                 # Attempt to read the file as UTF-8.
                 if file_handle is None:
                     with open(source_path, encoding="utf-8") as source_file:
                         source_file.read()
                 else:
-                    file_handle.seekable and file_handle.seek(0)
+                    check_file_handle_is_seekable(file_handle, source_path)
+                    file_position = file_handle.tell()
                     file_handle.read()
-                    file_handle.seekable and file_handle.seek(0)
+                    file_handle.seek(file_position)
                 result = "utf-8"
             except UnicodeDecodeError:
                 # UTF-8 did not work out, use the default as last resort.
                 result = DEFAULT_FALLBACK_ENCODING
             _log.debug("%s: no fallback encoding specified, using %s", source_path, result)
 
     assert result is not None
```

### Comparing `pygount-1.6.0/pygount/command.py` & `pygount-1.6.1/pygount/command.py`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/pygount/common.py` & `pygount-1.6.1/pygount/common.py`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/pygount/git_storage.py` & `pygount-1.6.1/pygount/git_storage.py`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/pygount/lexers.py` & `pygount-1.6.1/pygount/lexers.py`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/pygount/summary.py` & `pygount-1.6.1/pygount/summary.py`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/pygount/write.py` & `pygount-1.6.1/pygount/write.py`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/pygount/xmldialect.py` & `pygount-1.6.1/pygount/xmldialect.py`

 * *Files identical despite different names*

### Comparing `pygount-1.6.0/pyproject.toml` & `pygount-1.6.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
 target-version = [
-    "py37",
     "py38",
     "py39",
     "py310",
     "py311",
 ]
 exclude = '''
 /(
@@ -30,15 +29,15 @@
 ]
 testpaths = [
     "tests",
 ]
 
 [tool.poetry]
 name = "pygount"
-version = "1.6.0"
+version = "1.6.1"
 description = "count source lines of code (SLOC) using pygments"
 readme = "README.md"
 authors = ["Thomas Aglassinger <roskakori@users.sourceforge.net>"]
 license = "BSD"
 homepage = "https://github.com/roskakori/pygount"
 repository = "https://github.com/roskakori/pygount.git"
 documentation = "https://pygount.readthedocs.io"
@@ -71,18 +70,22 @@
 [tool.poetry.dev-dependencies]
 coveralls = "^3"
 coverage = "^6"
 pytest = "^7"
 pytest-cov = "^4"
 pre-commit = "^3"
 pur = "^7"
-Sphinx = "^5"
-sphinx-rtd-theme = "^1"
 twine = "^4"
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = "^7"
+
 [tool.poetry.scripts]
 pygount = "pygount.command:main"
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/roskakori/pygount/issues"
 "Changes" = "https://pygount.readthedocs.io/en/latest/changes.html"
```

### Comparing `pygount-1.6.0/PKG-INFO` & `pygount-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygount
-Version: 1.6.0
+Version: 1.6.1
 Summary: count source lines of code (SLOC) using pygments
 Home-page: https://github.com/roskakori/pygount
 License: BSD
 Keywords: code analysis,count,SLOC
 Author: Thomas Aglassinger
 Author-email: roskakori@users.sourceforge.net
 Requires-Python: >=3.8,<4
```

