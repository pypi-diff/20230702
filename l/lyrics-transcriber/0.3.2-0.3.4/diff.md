# Comparing `tmp/lyrics_transcriber-0.3.2.tar.gz` & `tmp/lyrics_transcriber-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyrics_transcriber-0.3.2.tar", max compression
+gzip compressed data, was "lyrics_transcriber-0.3.4.tar", max compression
```

## Comparing `lyrics_transcriber-0.3.2.tar` & `lyrics_transcriber-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.3.2/LICENSE
--rw-r--r--   0        0        0      175 2023-07-01 00:06:58.761216 lyrics_transcriber-0.3.2/README.md
--rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.3.2/lyrics_transcriber/__init__.py
--rw-r--r--   0        0        0     8814 2023-07-01 08:07:26.470781 lyrics_transcriber-0.3.2/lyrics_transcriber/transcriber.py
--rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.3.2/lyrics_transcriber/utils/__init__.py
--rwxr-xr-x   0        0        0     3247 2023-07-01 07:57:15.589521 lyrics_transcriber-0.3.2/lyrics_transcriber/utils/cli.py
--rw-r--r--   0        0        0      828 2023-07-01 16:44:21.031404 lyrics_transcriber-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 lyrics_transcriber-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-01 00:07:55.170976 lyrics_transcriber-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3457 2023-07-02 16:05:39.055430 lyrics_transcriber-0.3.4/README.md
+-rw-r--r--   0        0        0       94 2023-07-01 16:43:51.383557 lyrics_transcriber-0.3.4/lyrics_transcriber/__init__.py
+-rw-r--r--   0        0        0     8878 2023-07-02 03:32:57.507705 lyrics_transcriber-0.3.4/lyrics_transcriber/transcriber.py
+-rw-r--r--   0        0        0        0 2023-06-30 23:05:50.978048 lyrics_transcriber-0.3.4/lyrics_transcriber/utils/__init__.py
+-rwxr-xr-x   0        0        0     3247 2023-07-01 07:57:15.589521 lyrics_transcriber-0.3.4/lyrics_transcriber/utils/cli.py
+-rw-r--r--   0        0        0      851 2023-07-02 16:27:21.619207 lyrics_transcriber-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4389 1970-01-01 00:00:00.000000 lyrics_transcriber-0.3.4/PKG-INFO
```

### Comparing `lyrics_transcriber-0.3.2/LICENSE` & `lyrics_transcriber-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.3.2/lyrics_transcriber/transcriber.py` & `lyrics_transcriber-0.3.4/lyrics_transcriber/transcriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         self.result_metadata["midico_lrc_filepath"] = self.get_cache_filepath(".lrc")
         self.write_midico_lrc_file()
 
         self.calculate_singing_percentage()
 
         if self.genius_api_token and self.song_artist and self.song_title:
-            log(f"fetching lyrics from Genius as genius_api_token, song_artist and song_title were set")
+            log(f"fetching lyrics from Genius as genius_api_token: {self.genius_api_token}, song_artist: {self.song_artist} and song_title: {self.song_title} were set")
             self.result_metadata["genius_lyrics_filepath"] = self.get_cache_filepath("-genius.txt")
             self.write_genius_lyrics_file()
         else:
             log(f"not fetching lyrics from Genius as song_artist and song_title were not set")
 
         # TODO: attempt to match up segments from genius lyrics with whisper segments
```

### Comparing `lyrics_transcriber-0.3.2/lyrics_transcriber/utils/cli.py` & `lyrics_transcriber-0.3.4/lyrics_transcriber/utils/cli.py`

 * *Files identical despite different names*

### Comparing `lyrics_transcriber-0.3.2/pyproject.toml` & `lyrics_transcriber-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "lyrics-transcriber"
-version = "0.3.2"
+version = "0.3.4"
 description = "Automatically create synchronised lyrics files in ASS and MidiCo LRC formats with word-level timestamps, using Whisper and lyrics from Genius and Spotify"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "lyrics_transcriber"}]
+packages = [{ include = "lyrics_transcriber" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.11"
 Cython = "^0"
 dtw-python = "^1"
 llvmlite = "^0"
 numba = "^0.57"
 numpy = "^1"
 onnx = "^1"
 onnxruntime = "^1"
 torch = "^1"
 tqdm = "^4"
 lyricsgenius = "^3.0.1"
+openai-whisper = "*"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [tool.black]
 line-length = 140
```

