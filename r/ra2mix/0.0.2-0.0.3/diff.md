# Comparing `tmp/ra2mix-0.0.2.tar.gz` & `tmp/ra2mix-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ra2mix-0.0.2.tar", last modified: Sat Jul  1 19:17:49 2023, max compression
+gzip compressed data, was "ra2mix-0.0.3.tar", last modified: Sun Jul  2 04:26:25 2023, max compression
```

## Comparing `ra2mix-0.0.2.tar` & `ra2mix-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:17:49.146535 ra2mix-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 19:17:38.000000 ra2mix-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-01 19:17:49.146535 ra2mix-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-01 19:17:38.000000 ra2mix-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-01 19:17:38.000000 ra2mix-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:17:49.146535 ra2mix-0.0.2/ra2mix/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-01 19:17:38.000000 ra2mix-0.0.2/ra2mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-01 19:17:38.000000 ra2mix-0.0.2/ra2mix/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-01 19:17:38.000000 ra2mix-0.0.2/ra2mix/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 19:17:49.146535 ra2mix-0.0.2/ra2mix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-01 19:17:49.000000 ra2mix-0.0.2/ra2mix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-01 19:17:49.000000 ra2mix-0.0.2/ra2mix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 19:17:49.000000 ra2mix-0.0.2/ra2mix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 19:17:49.000000 ra2mix-0.0.2/ra2mix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-01 19:17:49.000000 ra2mix-0.0.2/ra2mix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 19:17:49.146535 ra2mix-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:26:25.111780 ra2mix-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 04:26:16.000000 ra2mix-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 04:26:25.111780 ra2mix-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 04:26:16.000000 ra2mix-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 04:26:16.000000 ra2mix-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:26:25.111780 ra2mix-0.0.3/ra2mix/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:26:25.111780 ra2mix-0.0.3/ra2mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:26:25.111780 ra2mix-0.0.3/setup.cfg
```

### Comparing `ra2mix-0.0.2/LICENSE` & `ra2mix-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.2/PKG-INFO` & `ra2mix-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ra2mix
-Version: 0.0.2
+Version: 0.0.3
 Summary: ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files
 Author-email: nyte_owl <nyteowldev@gmail.com>
 Project-URL: Homepage, https://github.com/endless-creation/ra2mix
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ra2mix-0.0.2/pyproject.toml` & `ra2mix-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "ra2mix"
 authors = [
     {name = "nyte_owl", email = "nyteowldev@gmail.com"}
 ]
 description = "ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
     "crc"
 ]
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `ra2mix-0.0.2/ra2mix/checksum.py` & `ra2mix-0.0.3/ra2mix/checksum.py`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.2/ra2mix/reader.py` & `ra2mix-0.0.3/ra2mix/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import struct
 from collections import namedtuple
 
+from . import const
 from .checksum import ra2_crc
 
 Header = namedtuple("Header", "flags file_count data_size")
-HEADER_SIZE = 10
 
-FileEntry = namedtuple("FileEntry", "id offset size")
-FILE_ENTRY_SIZE = 12
 
-MIX_DB_FILENAME = "local mix database.dat"
-
-
-def get_file_entries(header: Header, mix_data: bytes) -> list[FileEntry]:
+def get_file_entries(header: Header, mix_data: bytes) -> list[const.FileEntry]:
     file_entries = []
     for i in range(header.file_count):
-        start = 10 + (i * FILE_ENTRY_SIZE)
-        end = start + FILE_ENTRY_SIZE
+        start = 10 + (i * const.FILE_ENTRY_SIZE)
+        end = start + const.FILE_ENTRY_SIZE
         # print(binascii.b2a_hex(mix_data[start:end], ":"))
-        file_entries.append(FileEntry._make(struct.unpack("=3I", mix_data[start:end])))
+
+        # ID is unpacked as an unsigned integer because the CRC computer creates
+        # unsigned integers; they need to match for comparison sake
+        file_entries.append(
+            const.FileEntry._make(struct.unpack("=3I", mix_data[start:end]))
+        )
 
     return file_entries
 
 
 def get_filenames_from_mix_db(mix_db_file_data: bytes) -> list[str]:
     filenames = []
-    end = 52
-    start = 52
+    end = (start := const.XCC_HEADER_SIZE)
     while start < len(mix_db_file_data):
         while mix_db_file_data[end] != 0:
             end += 1
         filename = mix_db_file_data[start:end].decode("utf-8")
         filenames.append(filename)
         # print(f"{start=}, {end=}, {filename=}")
         end += 1
         start = end
 
     return filenames
 
 
-def get_file_data_from_mix_body(file_entry: FileEntry, mix_body_data: bytes) -> bytes:
+def get_file_data_from_mix_body(
+    file_entry: const.FileEntry, mix_body_data: bytes
+) -> bytes:
     return mix_body_data[file_entry.offset : file_entry.offset + file_entry.size]
 
 
-def get_file_map(file_entries: list[FileEntry], mix_data: bytes):
+def get_file_map(file_entries: list[const.FileEntry], mix_data: bytes):
     if len(file_entries) == 1:
         return {}
 
-    MIX_DB_ID = ra2_crc(MIX_DB_FILENAME)
+    MIX_DB_ID = ra2_crc(const.MIX_DB_FILENAME)
 
-    BODY_START = HEADER_SIZE + (FILE_ENTRY_SIZE * len(file_entries))
+    BODY_START = const.HEADER_SIZE + (const.FILE_ENTRY_SIZE * len(file_entries))
     for file_entry in file_entries:
         if file_entry.id != MIX_DB_ID:
             continue
         mix_db_file_entry = file_entry
         break
 
     mix_body_data = mix_data[BODY_START:]
@@ -67,18 +68,18 @@
     for file_entry in file_entries:
         file_data = get_file_data_from_mix_body(file_entry, mix_body_data)
         filemap[filename_id_map[file_entry.id]] = file_data
 
     return filemap
 
 
-def read(mix_filename: str) -> dict[str, bytes]:
-    with open(mix_filename, "rb") as fp:
+def read(mix_filepath: str) -> dict[str, bytes]:
+    with open(mix_filepath, "rb") as fp:
         mix_data = fp.read()
 
-    header = Header._make(struct.unpack("=I H I", mix_data[:HEADER_SIZE]))
+    header = Header._make(struct.unpack("=I H I", mix_data[: const.HEADER_SIZE]))
     if (header.flags & 2) != 0:
         raise NotImplementedError("Cannot parse encrypted mix header")
 
     file_entries = get_file_entries(header, mix_data)
 
     return get_file_map(file_entries, mix_data)
```

### Comparing `ra2mix-0.0.2/ra2mix.egg-info/PKG-INFO` & `ra2mix-0.0.3/ra2mix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ra2mix
-Version: 0.0.2
+Version: 0.0.3
 Summary: ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files
 Author-email: nyte_owl <nyteowldev@gmail.com>
 Project-URL: Homepage, https://github.com/endless-creation/ra2mix
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

