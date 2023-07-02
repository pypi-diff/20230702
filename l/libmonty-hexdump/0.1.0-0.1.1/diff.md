# Comparing `tmp/libmonty-hexdump-0.1.0.tar.gz` & `tmp/libmonty-hexdump-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmonty-hexdump-0.1.0.tar", last modified: Tue Jun 13 11:31:23 2023, max compression
+gzip compressed data, was "libmonty-hexdump-0.1.1.tar", last modified: Sun Jul  2 12:10:11 2023, max compression
```

## Comparing `libmonty-hexdump-0.1.0.tar` & `libmonty-hexdump-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:31:23.705669 libmonty-hexdump-0.1.0/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    16725 2022-08-26 18:54:24.000000 libmonty-hexdump-0.1.0/LICENSE
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        2 2023-06-12 11:39:50.000000 libmonty-hexdump-0.1.0/MANIFEST.in
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1950 2023-06-13 11:31:23.705669 libmonty-hexdump-0.1.0/PKG-INFO
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      752 2023-06-13 10:16:36.000000 libmonty-hexdump-0.1.0/README.md
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      108 2022-08-26 19:16:16.000000 libmonty-hexdump-0.1.0/pyproject.toml
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       44 2023-06-13 11:07:44.000000 libmonty-hexdump-0.1.0/requirements.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1382 2023-06-13 11:31:23.705669 libmonty-hexdump-0.1.0/setup.cfg
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:31:23.701669 libmonty-hexdump-0.1.0/src/
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:31:23.701669 libmonty-hexdump-0.1.0/src/libmonty_hexdump/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-08-26 18:54:24.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3398 2023-06-13 10:56:27.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump/__main__.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:31:23.701669 libmonty-hexdump-0.1.0/src/libmonty_hexdump/components/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-06-13 10:46:37.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump/components/__init__.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3612 2023-06-13 10:56:27.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump/components/arguments.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2878 2023-06-13 10:56:28.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump/components/lines.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      981 2023-06-13 10:56:27.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump/components/streams.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      963 2023-06-13 10:56:27.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump/components/width.py
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      326 2023-06-13 10:22:20.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump/version.py
-drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-06-13 11:31:23.701669 libmonty-hexdump-0.1.0/src/libmonty_hexdump.egg-info/
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1950 2023-06-13 11:31:23.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump.egg-info/PKG-INFO
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      649 2023-06-13 11:31:23.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump.egg-info/SOURCES.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        1 2023-06-13 11:31:23.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump.egg-info/dependency_links.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       68 2023-06-13 11:31:23.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump.egg-info/entry_points.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       40 2023-06-13 11:31:23.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump.egg-info/requires.txt
--rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       17 2023-06-13 11:31:23.000000 libmonty-hexdump-0.1.0/src/libmonty_hexdump.egg-info/top_level.txt
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 12:10:11.180957 libmonty-hexdump-0.1.1/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)    16725 2022-08-26 18:54:24.000000 libmonty-hexdump-0.1.1/LICENSE
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        2 2023-06-12 11:39:50.000000 libmonty-hexdump-0.1.1/MANIFEST.in
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2093 2023-07-02 12:10:11.180957 libmonty-hexdump-0.1.1/PKG-INFO
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      895 2023-06-13 11:43:58.000000 libmonty-hexdump-0.1.1/README.md
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      108 2022-08-26 19:16:16.000000 libmonty-hexdump-0.1.1/pyproject.toml
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       44 2023-07-02 11:39:23.000000 libmonty-hexdump-0.1.1/requirements.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1382 2023-07-02 12:10:11.180957 libmonty-hexdump-0.1.1/setup.cfg
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 12:10:11.176957 libmonty-hexdump-0.1.1/src/
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 12:10:11.180957 libmonty-hexdump-0.1.1/src/libmonty_hexdump/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2022-08-26 18:54:24.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3641 2023-07-02 12:05:21.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump/__main__.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 12:10:11.180957 libmonty-hexdump-0.1.1/src/libmonty_hexdump/components/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      268 2023-06-13 10:46:37.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump/components/__init__.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3956 2023-07-02 12:05:21.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump/components/arguments.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     3168 2023-07-02 12:05:21.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump/components/lines.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1064 2023-07-02 11:47:04.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump/components/streams.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     1111 2023-07-02 12:05:21.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump/components/width.py
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      357 2023-07-02 12:05:21.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump/version.py
+drwxrwxr-x   0 anemeth   (1000) anemeth   (1000)        0 2023-07-02 12:10:11.180957 libmonty-hexdump-0.1.1/src/libmonty_hexdump.egg-info/
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)     2093 2023-07-02 12:10:11.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump.egg-info/PKG-INFO
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)      649 2023-07-02 12:10:11.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump.egg-info/SOURCES.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)        1 2023-07-02 12:10:11.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump.egg-info/dependency_links.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       68 2023-07-02 12:10:11.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump.egg-info/entry_points.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       40 2023-07-02 12:10:11.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump.egg-info/requires.txt
+-rw-rw-r--   0 anemeth   (1000) anemeth   (1000)       17 2023-07-02 12:10:11.000000 libmonty-hexdump-0.1.1/src/libmonty_hexdump.egg-info/top_level.txt
```

### Comparing `libmonty-hexdump-0.1.0/LICENSE` & `libmonty-hexdump-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libmonty-hexdump-0.1.0/PKG-INFO` & `libmonty-hexdump-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmonty-hexdump
-Version: 0.1.0
+Version: 0.1.1
 Summary: libmonty-hexdump - Python library - hexdump utility
 Home-page: https://codeberg.org/sunarch/libmonty-hexdump
 Author: András Németh (sunarch)
 Author-email: sunarch@protonmail.com
 Maintainer: András Németh (sunarch)
 Maintainer-email: sunarch@protonmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
@@ -29,14 +29,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libmonty-hexdump
 
 Python library - a hex hump utility
 
+## Installation
+
+The package is on PyPI: [libmonty-hexdump](https://pypi.org/project/libmonty-hexdump/)
+
+```
+pip install libmonty-hexdump
+```
+
 ## License
 
 [Mozilla Public License 2.0](https://www.mozilla.org/en-US/MPL/2.0/)
 
 ```
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
```

### Comparing `libmonty-hexdump-0.1.0/README.md` & `libmonty-hexdump-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # libmonty-hexdump
 
 Python library - a hex hump utility
 
+## Installation
+
+The package is on PyPI: [libmonty-hexdump](https://pypi.org/project/libmonty-hexdump/)
+
+```
+pip install libmonty-hexdump
+```
+
 ## License
 
 [Mozilla Public License 2.0](https://www.mozilla.org/en-US/MPL/2.0/)
 
 ```
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
```

### Comparing `libmonty-hexdump-0.1.0/setup.cfg` & `libmonty-hexdump-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `libmonty-hexdump-0.1.0/src/libmonty_hexdump/components/arguments.py` & `libmonty-hexdump-0.1.1/src/libmonty_hexdump/components/arguments.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from typing import Tuple, Callable, Union
+"""Arguments
+"""
 
+# imports: library
+from argparse import ArgumentParser
+from typing import Callable, Union
+
+# imports: dependencies
 from libmonty.formatting import char_str, number_str
 
+# imports: project
 from libmonty_hexdump.components import streams
 
 
-def create_arguments(parser_hexer):
+def create_arguments(parser_hexer: ArgumentParser) -> None:
+    """Create arguments"""
 
     parser_hexer.add_argument('-s', '--stream',
                               help='Stream',
                               action='store', type=str, default='random',
                               dest='stream')
 
     parser_hexer.add_argument('-b', '--bytes-per-line',
@@ -31,78 +39,82 @@
 
     parser_hexer.add_argument('-i', '--index-format',
                               help='Index format',
                               action='store', type=str, default='hexadecimal',
                               dest='index_format')
 
 
-def stream(source: Union[Callable, str]) -> Tuple[Callable, Callable]:
+def stream(source: Union[Callable, str]) -> (Callable, Callable):
+    """Stream source"""
 
     if isinstance(source, Callable):
-        f_stream = source
-        f_char_converter = char_str.byte_to_compact_printable_with_dots
+        f_stream: Callable = source
+        f_char_converter: Callable = char_str.byte_to_compact_printable_with_dots
 
     else:
         if source == 'random':
-            f_stream = streams.random_data
-            f_char_converter = char_str.byte_to_compact_printable_with_dots
+            f_stream: Callable = streams.random_data
+            f_char_converter: Callable = char_str.byte_to_compact_printable_with_dots
 
         else:
             try:
-                f_stream = streams.create_from_file(source)
-            except FileNotFoundError as err:
-                raise ValueError(str(err))
+                f_stream: Callable = streams.create_from_file(source)
+            except FileNotFoundError as exc:
+                raise ValueError(str(exc)) from exc
 
-            f_char_converter = char_str.byte_to_compact_printable_with_frames
+            f_char_converter: Callable = char_str.byte_to_compact_printable_with_frames
 
     return f_stream, f_char_converter
 
 
 def bytes_per_line(count: int) -> int:
+    """Bytes per line"""
 
     if count < 1:
         raise ValueError
 
     return count
 
 
 def sleep(speed: Union[float, int, str]) -> float:
+    """Sleep"""
 
-    d_speeds = {
+    speeds: dict[str, float] = {
         'f': 0.01,
         'fast': 0.01,
         'm': 0.05,
         'med': 0.05,
         'medium': 0.05,
         's': 0.1,
         'slow': 0.1,
         'step': 0.5
     }
 
     if isinstance(speed, int):
-        speed = float(speed)
+        speed: float = float(speed)
 
-    if isinstance(speed, float) or isinstance(speed, int):
+    if isinstance(speed, (float, int)):
         if speed <= 0:
             raise ValueError
 
     elif isinstance(speed, str):
         try:
-            speed = d_speeds[speed]
+            speed: float = speeds[speed]
         except KeyError:
             print(f'Bad value for \'sleep\': \'{speed}\'')
             speed = 0.01
             print(f'Using default value for \'sleep\': \'{speed}\'')
 
     return speed
 
 
 def index_converter(converter: Union[Callable, str]) -> Callable:
+    """Index converter"""
 
-    d_index_formats = {
+    index_formats: dict[str, Callable] = {
         'h': number_str.hexadecimal,
         'hex': number_str.hexadecimal,
         'hexadecimal': number_str.hexadecimal,
 
         'd': number_str.decimal,
         'dec': number_str.decimal,
         'decimal': number_str.decimal,
@@ -112,13 +124,13 @@
         'octal': number_str.octal
     }
 
     if isinstance(converter, Callable):
         return converter
 
     try:
-        return d_index_formats[converter]
+        return index_formats[converter]
     except KeyError:
         print(f'Value for index format not recognized: \'{converter}\'')
-        converter = 'hexadecimal'
+        converter: str = 'hexadecimal'
         print(f'Using default value for index format: \'{converter}\'')
-        return d_index_formats[converter]
+        return index_formats[converter]
```

### Comparing `libmonty-hexdump-0.1.0/src/libmonty_hexdump/components/lines.py` & `libmonty-hexdump-0.1.1/src/libmonty_hexdump/components/lines.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,103 +1,116 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+"""Lines
+"""
+
+# imports: library
 from typing import Callable
 
+# imports: dependencies
 from libmonty.formatting import number_str
 from libmonty.formatting import char_str
 
 
 COUNTER_DIGITS = 10
 
 
 def print_header(bytes_per_line: int,
                  index_converter: Callable,
                  extra_width: int
                  ) -> None:
+    """Print header"""
 
-    s_counter = f'Offset ({index_converter(-1)})'
-    s_line = f' {s_counter:^{COUNTER_DIGITS + extra_width}}  '
+    counter_text: str = f'Offset ({index_converter(-1)})'
+    line: str = f' {counter_text:^{COUNTER_DIGITS + extra_width}}  '
 
     try:
-        b_unit = bytes(range(bytes_per_line))
+        bytes_unit: bytes = bytes(range(bytes_per_line))
     except ValueError:
         if bytes_per_line > 256:
-            full = bytes(range(256)) * (bytes_per_line // 256)
-            fraction = bytes(range(bytes_per_line % 256))
-            b_unit = full + fraction
+            full: bytes = bytes(range(256)) * (bytes_per_line // 256)
+            fraction: bytes = bytes(range(bytes_per_line % 256))
+            bytes_unit: bytes = full + fraction
         else:
             raise
 
-    s_line += _part_bytes(b_unit, bytes_per_line, index_converter)
+    line += _part_bytes(bytes_unit, bytes_per_line, index_converter)
 
-    s_line += 'Decoded text'
+    line += 'Decoded text'
 
-    print(s_line, flush=True)
+    print(line, flush=True)
 
 
 def print_data(b_unit: bytes,
                bytes_per_line: int,
                offset: int,
                index_converter: Callable,
                char_converter: Callable,
                extra_width: int
                ) -> None:
+    """Print data"""
 
-    s = construct(b_unit,
-                  bytes_per_line,
-                  offset,
-                  index_converter,
-                  char_converter,
-                  extra_width)
+    text: str = construct(
+        b_unit,
+        bytes_per_line,
+        offset,
+        index_converter,
+        char_converter,
+        extra_width
+    )
 
-    print(s, flush=True)
+    print(text, flush=True)
 
 
 def construct(b_unit: bytes,
               bytes_per_line: int,
               offset: int = 0,
               index_converter: Callable = number_str.pseudo,
               char_converter: Callable = char_str.pseudo,
               extra_width: int = 0
               ) -> str:
+    """Construct"""
 
-    s_counter = _part_counter(offset, COUNTER_DIGITS + extra_width, index_converter)
+    counter_text: str = _part_counter(offset, COUNTER_DIGITS + extra_width, index_converter)
 
-    s_bytes = _part_bytes(b_unit, bytes_per_line, number_str.hexadecimal)
+    bytes_text: str = _part_bytes(b_unit, bytes_per_line, number_str.hexadecimal)
 
-    s_chars = _part_chars(b_unit, char_converter)
+    chars_text: str = _part_chars(b_unit, char_converter)
 
-    return s_counter + s_bytes + s_chars
+    return counter_text + bytes_text + chars_text
 
 
 def _part_counter(offset: int = 0,
                   digits: int = COUNTER_DIGITS,
                   index_formatter: Callable = number_str.pseudo,
                   ) -> str:
+    """Part: counter"""
 
     return ' ' + index_formatter(offset, digits) + '  '
 
 
 def _part_bytes(b_unit: bytes,
                 bytes_per_line: int,
                 number_converter: Callable = number_str.pseudo
                 ) -> str:
+    """Part: bytes"""
 
-    s_bytes = ' '.join(map(lambda b: number_converter(b, 2), b_unit))
+    bytes_text: str = ' '.join(map(lambda b: number_converter(b, 2), b_unit))
 
     if len(b_unit) < bytes_per_line:
-        s_format = '{:<' + str((bytes_per_line * 3) - 1) + '}'
-        s_bytes = s_format.format(s_bytes)
+        format_string: str = '{:<' + str((bytes_per_line * 3) - 1) + '}'
+        bytes_text: str = format_string.format(bytes_text)
 
-    return s_bytes + '  '
+    return bytes_text + '  '
 
 
-def _part_chars(b_unit: bytes,
+def _part_chars(bytes_unit: bytes,
                 char_converter: Callable = char_str.pseudo,
                 ) -> str:
+    """Part: chars"""
 
-    return ''.join(map(char_converter, b_unit))
+    return ''.join(map(char_converter, bytes_unit))
```

### Comparing `libmonty-hexdump-0.1.0/src/libmonty_hexdump/components/streams.py` & `libmonty-hexdump-0.1.1/src/libmonty_hexdump/components/streams.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8, vim: expandtab:ts=4 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-import random
-import os.path
+"""Streams
+"""
 
+# imports: library
+import os.path
+import random
 from typing import Callable, Generator
 
 
 def create_from_file(path: str) -> Callable:
+    """Create from file"""
 
     if not os.path.isfile(path):
         raise FileNotFoundError(f'File not found: \'{path}\'')
 
     def file_contents(bytes_per_line: int) -> Generator:
         with open(path, 'rb') as f_stream:
 
@@ -30,10 +34,11 @@
 
                 yield data
 
     return file_contents
 
 
 def random_data(bytes_per_line: int) -> Generator:
+    """Random data"""
 
     while True:
         yield random.randbytes(bytes_per_line)
```

### Comparing `libmonty-hexdump-0.1.0/src/libmonty_hexdump.egg-info/PKG-INFO` & `libmonty-hexdump-0.1.1/src/libmonty_hexdump.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmonty-hexdump
-Version: 0.1.0
+Version: 0.1.1
 Summary: libmonty-hexdump - Python library - hexdump utility
 Home-page: https://codeberg.org/sunarch/libmonty-hexdump
 Author: András Németh (sunarch)
 Author-email: sunarch@protonmail.com
 Maintainer: András Németh (sunarch)
 Maintainer-email: sunarch@protonmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
@@ -29,14 +29,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libmonty-hexdump
 
 Python library - a hex hump utility
 
+## Installation
+
+The package is on PyPI: [libmonty-hexdump](https://pypi.org/project/libmonty-hexdump/)
+
+```
+pip install libmonty-hexdump
+```
+
 ## License
 
 [Mozilla Public License 2.0](https://www.mozilla.org/en-US/MPL/2.0/)
 
 ```
 This Source Code Form is subject to the terms of the Mozilla Public
 License, v. 2.0. If a copy of the MPL was not distributed with this
```

### Comparing `libmonty-hexdump-0.1.0/src/libmonty_hexdump.egg-info/SOURCES.txt` & `libmonty-hexdump-0.1.1/src/libmonty_hexdump.egg-info/SOURCES.txt`

 * *Files identical despite different names*

