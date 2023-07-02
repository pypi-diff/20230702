# Comparing `tmp/srt_equalizer-0.1.5.tar.gz` & `tmp/srt_equalizer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_equalizer-0.1.5.tar", max compression
+gzip compressed data, was "srt_equalizer-0.1.6.tar", max compression
```

## Comparing `srt_equalizer-0.1.5.tar` & `srt_equalizer-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-03-14 12:00:05.282587 srt_equalizer-0.1.5/LICENSE
--rw-r--r--   0        0        0     2688 2023-07-02 13:42:11.385032 srt_equalizer-0.1.5/README.md
--rw-r--r--   0        0        0      519 2023-07-02 15:17:34.795707 srt_equalizer-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      104 2023-04-01 12:40:07.008580 srt_equalizer-0.1.5/src/srt_equalizer/__init__.py
--rw-r--r--   0        0        0     3605 2023-04-02 12:51:15.799391 srt_equalizer-0.1.5/src/srt_equalizer/srt_equalizer.py
--rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 srt_equalizer-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-14 12:00:05.282587 srt_equalizer-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2688 2023-07-02 13:42:11.385032 srt_equalizer-0.1.6/README.md
+-rw-r--r--   0        0        0      519 2023-07-02 16:42:19.886623 srt_equalizer-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-04-01 12:40:07.008580 srt_equalizer-0.1.6/src/srt_equalizer/__init__.py
+-rw-r--r--   0        0        0     3628 2023-07-02 16:42:09.008793 srt_equalizer-0.1.6/src/srt_equalizer/srt_equalizer.py
+-rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 srt_equalizer-0.1.6/PKG-INFO
```

### Comparing `srt_equalizer-0.1.5/LICENSE` & `srt_equalizer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_equalizer-0.1.5/README.md` & `srt_equalizer-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `srt_equalizer-0.1.5/pyproject.toml` & `srt_equalizer-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "srt_equalizer"
-version = "0.1.5"
+version = "0.1.6"
 description = "Transform subtitle line lengths, splitting into multiple subtitle fragments if necessary. "
 authors = ["Peter Krantz"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/peterk/srt_equalizer"
 
 [tool.poetry.dependencies]
```

### Comparing `srt_equalizer-0.1.5/src/srt_equalizer/srt_equalizer.py` & `srt_equalizer-0.1.6/src/srt_equalizer/srt_equalizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from datetime import timedelta
 import srt
+from typing import List
 
-
-def load_srt(filepath: str) -> list[srt.Subtitle]:
+def load_srt(filepath: str) -> List[srt.Subtitle]:
     """Load an SRT subtitle file and return an array of srt.Subtitle items."""
     filedata = ""
     with open(filepath, 'r') as f:
         filedata = f.read()
 
     return list(srt.parse(filedata))
 
 
-def write_srt(filepath: str, subs: list[srt.Subtitle]):
+def write_srt(filepath: str, subs: List[srt.Subtitle]):
     """Write an SRT subtitle file to disk."""
     with open(filepath, "w") as f:
         f.write(srt.compose(subs))
 
 
-def whisper_result_to_srt(segments: list[dict]) -> list[srt.Subtitle]:
+def whisper_result_to_srt(segments: List[dict]) -> list[srt.Subtitle]:
     """Convert Whisper ASR result segments to a list of srt.Subtitle items."""
     subs = []
 
     for i, segment in enumerate(segments, start=1):
         start_time = timedelta(seconds=int(segment['start']))
         end_time = timedelta(seconds=int(segment['end']))
         content = segment['text']
         subs.append(srt.Subtitle(index=i, content=content, start=start_time, end=end_time))
 
     return subs
 
 
-def split_subtitle(sub: srt.Subtitle, target_chars: int = 42, start_from_index: int = 1) -> list[srt.Subtitle]:
+def split_subtitle(sub: srt.Subtitle, target_chars: int = 42, start_from_index: int = 1) -> List[srt.Subtitle]:
     """If the subtitle length is > target_chars, split it into a list of subtitles within the same
     time span. If not, return the subtitle as is. The time code is adjusted proportionally
     to the length of the subtitle.
     
     Args:
         sub: A srt.Subtitle object.
         target_chars: The max number of characters for a subtitle line.
```

### Comparing `srt_equalizer-0.1.5/PKG-INFO` & `srt_equalizer-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-equalizer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Transform subtitle line lengths, splitting into multiple subtitle fragments if necessary. 
 Home-page: https://github.com/peterk/srt_equalizer
 License: MIT
 Author: Peter Krantz
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

