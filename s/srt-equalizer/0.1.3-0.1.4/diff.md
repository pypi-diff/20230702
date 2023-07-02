# Comparing `tmp/srt_equalizer-0.1.3.tar.gz` & `tmp/srt_equalizer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_equalizer-0.1.3.tar", max compression
+gzip compressed data, was "srt_equalizer-0.1.4.tar", max compression
```

## Comparing `srt_equalizer-0.1.3.tar` & `srt_equalizer-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-03-14 12:00:05.282587 srt_equalizer-0.1.3/LICENSE
--rw-r--r--   0        0        0     2643 2023-04-02 12:58:18.971130 srt_equalizer-0.1.3/README.md
--rw-r--r--   0        0        0      464 2023-04-02 12:58:40.596336 srt_equalizer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      104 2023-04-01 12:40:07.008580 srt_equalizer-0.1.3/src/srt_equalizer/__init__.py
--rw-r--r--   0        0        0     3605 2023-04-02 12:51:15.799391 srt_equalizer-0.1.3/src/srt_equalizer/srt_equalizer.py
--rw-r--r--   0        0        0     3191 1970-01-01 00:00:00.000000 srt_equalizer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-14 12:00:05.282587 srt_equalizer-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2688 2023-07-02 13:42:11.385032 srt_equalizer-0.1.4/README.md
+-rw-r--r--   0        0        0      519 2023-07-02 13:46:44.045940 srt_equalizer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-04-01 12:40:07.008580 srt_equalizer-0.1.4/src/srt_equalizer/__init__.py
+-rw-r--r--   0        0        0     3605 2023-04-02 12:51:15.799391 srt_equalizer-0.1.4/src/srt_equalizer/srt_equalizer.py
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 srt_equalizer-0.1.4/PKG-INFO
```

### Comparing `srt_equalizer-0.1.3/LICENSE` & `srt_equalizer-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_equalizer-0.1.3/README.md` & `srt_equalizer-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # SRT Equalizer
 
 A Python module to transform subtitle line lengths, splitting into multiple subtitle
 fragments if necessary. Useful to adjust automatic speech recognition outputs from e.g. [Whisper](https://github.com/openai/whisper) to a more convenient size.
 
 This library works for all languages where spaces separate words.
 
+## Installing
+
+`pip install srt_equalizer`
+
 ## Example
 
 If the SRT file contains lines over a certain length like this:
 
 ```
 1
 00:00:00,000 --> 00:00:04,000
@@ -50,15 +54,15 @@
 difficult issue, an issue that is one of
 
 5
 00:00:08,979 --> 00:00:11,000
 the most profound of our time.
 ```
 
-## Adjust Whsiper subtitle lengths
+## Adjust Whisper subtitle lengths
 Is is also possible to work with the subtitle items with the following utility methods:
 
 ```python
 split_subtitle(sub: srt.Subtitle, target_chars: int=42, start_from_index: int=1) -> list[srt.Subtitle]:
 
 whisper_result_to_srt(segments: list[dict]) -> list[srt.Subtitle]:
 ```
@@ -84,10 +88,10 @@
 
 for i in equalized:
     print(i.content)
 ```
 
 ## Contributing
 
-This library is build with [Poetry](https://python-poetry.org). Checkout this repo and run `poetry install` in the source folder. To run tests use `poetry run pytest tests`.
+This library is built with [Poetry](https://python-poetry.org). Checkout this repo and run `poetry install` in the source folder. To run tests use `poetry run pytest tests`.
 
-If you want to explore the library start a `poetry shell`.
+If you want to explore the library start a `poetry shell`.
```

### Comparing `srt_equalizer-0.1.3/src/srt_equalizer/srt_equalizer.py` & `srt_equalizer-0.1.4/src/srt_equalizer/srt_equalizer.py`

 * *Files identical despite different names*

### Comparing `srt_equalizer-0.1.3/PKG-INFO` & `srt_equalizer-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: srt-equalizer
-Version: 0.1.3
+Version: 0.1.4
 Summary: Transform subtitle line lengths, splitting into multiple subtitle fragments if necessary. 
+Home-page: https://github.com/peterk/srt_equalizer
 License: MIT
 Author: Peter Krantz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: srt (>=3.5.3,<4.0.0)
+Project-URL: Repository, https://github.com/peterk/srt_equalizer
 Description-Content-Type: text/markdown
 
 # SRT Equalizer
 
 A Python module to transform subtitle line lengths, splitting into multiple subtitle
 fragments if necessary. Useful to adjust automatic speech recognition outputs from e.g. [Whisper](https://github.com/openai/whisper) to a more convenient size.
 
 This library works for all languages where spaces separate words.
 
+## Installing
+
+`pip install srt_equalizer`
+
 ## Example
 
 If the SRT file contains lines over a certain length like this:
 
 ```
 1
 00:00:00,000 --> 00:00:04,000
@@ -65,15 +71,15 @@
 difficult issue, an issue that is one of
 
 5
 00:00:08,979 --> 00:00:11,000
 the most profound of our time.
 ```
 
-## Adjust Whsiper subtitle lengths
+## Adjust Whisper subtitle lengths
 Is is also possible to work with the subtitle items with the following utility methods:
 
 ```python
 split_subtitle(sub: srt.Subtitle, target_chars: int=42, start_from_index: int=1) -> list[srt.Subtitle]:
 
 whisper_result_to_srt(segments: list[dict]) -> list[srt.Subtitle]:
 ```
@@ -99,10 +105,11 @@
 
 for i in equalized:
     print(i.content)
 ```
 
 ## Contributing
 
-This library is build with [Poetry](https://python-poetry.org). Checkout this repo and run `poetry install` in the source folder. To run tests use `poetry run pytest tests`.
+This library is built with [Poetry](https://python-poetry.org). Checkout this repo and run `poetry install` in the source folder. To run tests use `poetry run pytest tests`.
 
 If you want to explore the library start a `poetry shell`.
+
```

