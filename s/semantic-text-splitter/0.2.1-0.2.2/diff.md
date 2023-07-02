# Comparing `tmp/semantic_text_splitter-0.2.1.tar.gz` & `tmp/semantic_text_splitter-0.2.2.tar.gz`

## Comparing `semantic_text_splitter-0.2.1.tar` & `semantic_text_splitter-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123      685 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/.gitignore
--rw-r--r--   0     1001      123     1514 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/CHANGELOG.md
--rw-r--r--   0     1001      123     4027 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/README.md
--rw-r--r--   0     1001      123      472 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123    13095 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/semantic_text_splitter.pyi
--rw-r--r--   0     1001      123    19656 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123   711396 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/tests/bert-base-cased.json
--rw-r--r--   0     1001      123     2623 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/tests/test_integration.py
--rw-r--r--   0     1001      123    24957 2023-06-13 20:01:31.000000 semantic_text_splitter-0.2.1/Cargo.lock
--rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.2/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-07-02 20:43:31.000000 semantic_text_splitter-0.2.2/.gitignore
+-rw-r--r--   0     1001      123     1611 2023-07-02 20:43:31.000000 semantic_text_splitter-0.2.2/CHANGELOG.md
+-rw-r--r--   0     1001      123     4836 2023-07-02 20:43:31.000000 semantic_text_splitter-0.2.2/README.md
+-rw-r--r--   0     1001      123      472 2023-07-02 20:43:31.000000 semantic_text_splitter-0.2.2/pyproject.toml
+-rw-r--r--   0     1001      123    13095 2023-07-02 20:43:31.000000 semantic_text_splitter-0.2.2/semantic_text_splitter.pyi
+-rw-r--r--   0     1001      123    19656 2023-07-02 20:43:31.000000 semantic_text_splitter-0.2.2/src/lib.rs
+-rw-r--r--   0     1001      123   711396 2023-07-02 20:43:31.000000 semantic_text_splitter-0.2.2/tests/bert-base-cased.json
+-rw-r--r--   0     1001      123     2623 2023-07-02 20:43:31.000000 semantic_text_splitter-0.2.2/tests/test_integration.py
+-rw-r--r--   0     1001      123    24929 2023-07-02 20:43:31.000000 semantic_text_splitter-0.2.2/Cargo.lock
+-rw-r--r--   0        0        0     5767 1970-01-01 00:00:00.000000 semantic_text_splitter-0.2.2/PKG-INFO
```

### Comparing `semantic_text_splitter-0.2.1/Cargo.toml` & `semantic_text_splitter-0.2.2/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "semantic-text-splitter"
-version = "0.2.1"
+version = "0.2.2"
 authors = ["Ben Brandt <benjamin.j.brandt@gmail.com>"]
 edition = "2021"
 description = "Split text into semantic chunks, up to a desired chunk size. Supports calculating length by characters and tokens (when used with large language models)."
 repository = "https://github.com/benbrandt/text-splitter"
 license = "MIT"
 keywords = ["text", "split", "tokenizer", "nlp", "ai"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "semantic_text_splitter"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.19.0", features = ["abi3-py37"] }
-text-splitter = { version = "0.4.1", features = ["tiktoken-rs", "tokenizers"] }
-tiktoken-rs = "0.4.2"
+text-splitter = { version = "0.4.2", features = ["tiktoken-rs", "tokenizers"] }
+tiktoken-rs = "0.5.0"
 tokenizers = { version = "0.13.3", default_features = false, features = [
     "onig",
 ] }
```

### Comparing `semantic_text_splitter-0.2.1/.gitignore` & `semantic_text_splitter-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.2.1/CHANGELOG.md` & `semantic_text_splitter-0.2.2/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## v0.2.2
+
+### What's New
+
+- Update to v0.4.2 of `text-splitter` to support `tiktoken-rs@0.5.0`
+
 ## v0.2.1
 
 ### What's New
 
 - Support Open AI Tiktoken tokenizers. So you can now give an OpenAI model name to tokenize the text for when calculating chunk sizes.
 
 ```python
```

### Comparing `semantic_text_splitter-0.2.1/README.md` & `semantic_text_splitter-0.2.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -17,14 +17,42 @@
 max_characters = 1000
 # Optionally can also have the splitter not trim whitespace for you
 splitter = CharacterTextSplitter(trim_chunks=False)
 
 chunks = splitter.chunks("your document text", max_characters)
 ```
 
+### With Huggingface Tokenizer
+
+```python
+from semantic_text_splitter import HuggingFaceTextSplitter
+from tokenizers import Tokenizer
+
+# Maximum number of tokens in a chunk
+max_characters = 1000
+# Optionally can also have the splitter not trim whitespace for you
+tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
+splitter = HuggingFaceTextSplitter(tokenizer, trim_chunks=False)
+
+chunks = splitter.chunks("your document text", max_characters)
+```
+
+### With Tiktoken Tokenizer
+
+```python
+from semantic_text_splitter import TiktokenTextSplitter
+
+# Maximum number of tokens in a chunk
+max_tokens = 1000
+# Optionally can also have the splitter not trim whitespace for you
+splitter = TiktokenTextSplitter("gpt-3.5-turbo", trim_chunks=False)
+
+chunks = splitter.chunks("your document text", max_tokens)
+```
+
 ### Using a Range for Chunk Capacity
 
 You also have the option of specifying your chunk capacity as a range.
 
 Once a chunk has reached a length that falls within the range it will be returned.
 
 It is always possible that a chunk may be returned that is less than the `start` value, as adding the next piece of text may have made it larger than the `end` capacity.
```

### Comparing `semantic_text_splitter-0.2.1/semantic_text_splitter.pyi` & `semantic_text_splitter-0.2.2/semantic_text_splitter.pyi`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.2.1/src/lib.rs` & `semantic_text_splitter-0.2.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.2.1/tests/bert-base-cased.json` & `semantic_text_splitter-0.2.2/tests/bert-base-cased.json`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.2.1/tests/test_integration.py` & `semantic_text_splitter-0.2.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `semantic_text_splitter-0.2.1/Cargo.lock` & `semantic_text_splitter-0.2.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 name = "anyhow"
 version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "auto_enums"
-version = "0.8.0"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "10143e1d6fc660ac7bfc268c6ec2f9699129a3cfbb241eed50393d1562e0a4ce"
+checksum = "faa44067eaa1097fc513fcdea6b9c42ea8a792f750a181937d52b315477e7b7a"
 dependencies = [
  "derive_utils",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
@@ -258,20 +258,17 @@
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "hermit-abi"
-version = "0.2.6"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
@@ -297,17 +294,17 @@
 checksum = "284f18f85651fe11e8a991b2adb42cb078325c996ed026d994719efcfca1d54b"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.10.5"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
 version = "1.0.6"
@@ -318,17 +315,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
@@ -393,32 +390,32 @@
 name = "monostate-impl"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8795add3e14028f11f8e848bd3294898a8294767b3776b6f733560d33bd2530b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "once_cell"
@@ -487,17 +484,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.0"
@@ -556,17 +553,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -684,15 +681,15 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "semantic-text-splitter"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
  "pyo3",
  "text-splitter",
  "tiktoken-rs",
  "tokenizers",
 ]
 
@@ -709,22 +706,22 @@
 name = "serde_derive"
 version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -760,38 +757,38 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "text-splitter"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70fb0eba57256b96e1438c8542a99277bddd8c3774f8cfc629bf2f6fe13c09c1"
+checksum = "62a5c046e622fc8f2d16754acde6e2a752885cb4b7af7bf47454cf633d9bb57c"
 dependencies = [
  "auto_enums",
  "either",
- "itertools 0.10.5",
+ "itertools 0.11.0",
  "once_cell",
  "regex",
  "tiktoken-rs",
  "tokenizers",
  "unicode-segmentation",
 ]
 
@@ -808,22 +805,22 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tiktoken-rs"
-version = "0.4.2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ba161c549e2c0686f35f5d920e63fad5cafba2c28ad2caceaf07e5d9fa6e8c4"
+checksum = "1a99d843674a3468b4a9200a565bbe909a0152f95e82a52feae71e6bf2d4b49d"
 dependencies = [
  "anyhow",
  "base64 0.21.2",
  "bstr",
  "fancy-regex",
  "lazy_static",
  "parking_lot",
@@ -898,17 +895,17 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
```

### Comparing `semantic_text_splitter-0.2.1/PKG-INFO` & `semantic_text_splitter-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-text-splitter
-Version: 0.2.1
+Version: 0.2.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: black ; extra == 'test'
 Requires-Dist: tokenizers ; extra == 'test'
 Requires-Dist: pdoc ; extra == 'docs'
@@ -38,14 +38,42 @@
 max_characters = 1000
 # Optionally can also have the splitter not trim whitespace for you
 splitter = CharacterTextSplitter(trim_chunks=False)
 
 chunks = splitter.chunks("your document text", max_characters)
 ```
 
+### With Huggingface Tokenizer
+
+```python
+from semantic_text_splitter import HuggingFaceTextSplitter
+from tokenizers import Tokenizer
+
+# Maximum number of tokens in a chunk
+max_characters = 1000
+# Optionally can also have the splitter not trim whitespace for you
+tokenizer = Tokenizer.from_pretrained("bert-base-uncased")
+splitter = HuggingFaceTextSplitter(tokenizer, trim_chunks=False)
+
+chunks = splitter.chunks("your document text", max_characters)
+```
+
+### With Tiktoken Tokenizer
+
+```python
+from semantic_text_splitter import TiktokenTextSplitter
+
+# Maximum number of tokens in a chunk
+max_tokens = 1000
+# Optionally can also have the splitter not trim whitespace for you
+splitter = TiktokenTextSplitter("gpt-3.5-turbo", trim_chunks=False)
+
+chunks = splitter.chunks("your document text", max_tokens)
+```
+
 ### Using a Range for Chunk Capacity
 
 You also have the option of specifying your chunk capacity as a range.
 
 Once a chunk has reached a length that falls within the range it will be returned.
 
 It is always possible that a chunk may be returned that is less than the `start` value, as adding the next piece of text may have made it larger than the `end` capacity.
```

