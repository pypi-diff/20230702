# Comparing `tmp/Blockthon-3.6.9.tar.gz` & `tmp/Blockthon-4.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Blockthon-3.6.9.tar", last modified: Fri Jun 16 16:14:04 2023, max compression
+gzip compressed data, was "Blockthon-4.6.9.tar", last modified: Sun Jul  2 01:38:11 2023, max compression
```

## Comparing `Blockthon-3.6.9.tar` & `Blockthon-4.6.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 16:14:04.995639 Blockthon-3.6.9/
-drwxrwxrwx   0        0        0        0 2023-06-16 16:14:04.983213 Blockthon-3.6.9/Blockthon/
--rw-rw-rw-   0        0        0     2160 2023-06-02 20:46:04.000000 Blockthon-3.6.9/Blockthon/Base58.py
--rw-rw-rw-   0        0        0     3705 2023-06-04 19:05:17.000000 Blockthon-3.6.9/Blockthon/Bitcoin.py
--rw-rw-rw-   0        0        0     1159 2023-06-03 18:38:02.000000 Blockthon-3.6.9/Blockthon/BitcoinGold.py
--rw-rw-rw-   0        0        0     1041 2023-06-03 18:38:02.000000 Blockthon-3.6.9/Blockthon/Dash.py
--rw-rw-rw-   0        0        0     1032 2023-06-03 18:38:02.000000 Blockthon-3.6.9/Blockthon/DigiByte.py
--rw-rw-rw-   0        0        0      497 2023-06-03 12:50:01.000000 Blockthon-3.6.9/Blockthon/Dogecoin.py
--rw-rw-rw-   0        0        0      492 2023-06-02 23:40:53.000000 Blockthon-3.6.9/Blockthon/Ethereum.py
--rw-rw-rw-   0        0        0     1407 2023-06-03 13:19:05.000000 Blockthon-3.6.9/Blockthon/Litecoin.py
--rw-rw-rw-   0        0        0      859 2023-06-04 00:55:43.000000 Blockthon-3.6.9/Blockthon/Qtum.py
--rw-rw-rw-   0        0        0      847 2023-06-04 00:59:12.000000 Blockthon-3.6.9/Blockthon/Ravencoin.py
--rw-rw-rw-   0        0        0      495 2023-06-02 23:40:53.000000 Blockthon-3.6.9/Blockthon/Tron.py
--rw-rw-rw-   0        0        0    30361 2023-06-16 16:11:36.000000 Blockthon-3.6.9/Blockthon/Utils.py
--rw-rw-rw-   0        0        0     1607 2023-06-16 16:11:36.000000 Blockthon-3.6.9/Blockthon/Wallet.py
--rw-rw-rw-   0        0        0      588 2023-06-04 01:02:25.000000 Blockthon-3.6.9/Blockthon/__init__.py
--rw-rw-rw-   0        0        0      822 2023-06-04 00:29:18.000000 Blockthon-3.6.9/Blockthon/zCash.py
-drwxrwxrwx   0        0        0        0 2023-06-16 16:14:04.995639 Blockthon-3.6.9/Blockthon.egg-info/
--rw-rw-rw-   0        0        0     3514 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-16 16:14:04.000000 Blockthon-3.6.9/Blockthon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3514 2023-06-16 16:14:04.995639 Blockthon-3.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     2674 2023-06-04 01:48:32.000000 Blockthon-3.6.9/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 16:14:04.995639 Blockthon-3.6.9/setup.cfg
--rw-rw-rw-   0        0        0     1477 2023-06-16 16:13:07.000000 Blockthon-3.6.9/setup.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 01:38:11.945119 Blockthon-4.6.9/
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 01:38:11.944138 Blockthon-4.6.9/Blockthon/
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1716 2023-07-01 10:53:50.000000 Blockthon-4.6.9/Blockthon/Bitcoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:26:12.000000 Blockthon-4.6.9/Blockthon/BitcoinGold.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3810 2023-06-30 08:06:48.000000 Blockthon-4.6.9/Blockthon/Check.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:26:50.000000 Blockthon-4.6.9/Blockthon/Dash.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:29:40.000000 Blockthon-4.6.9/Blockthon/Digibyte.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:27:46.000000 Blockthon-4.6.9/Blockthon/Dogecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:24:32.000000 Blockthon-4.6.9/Blockthon/Ethereum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1356 2023-07-01 10:52:46.000000 Blockthon-4.6.9/Blockthon/Litecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:30:34.000000 Blockthon-4.6.9/Blockthon/Qtum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:30:06.000000 Blockthon-4.6.9/Blockthon/Ravencoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      455 2023-07-01 10:24:32.000000 Blockthon-4.6.9/Blockthon/Tron.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3339 2023-06-30 09:21:44.000000 Blockthon-4.6.9/Blockthon/Utils.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    13912 2023-07-01 22:48:40.000000 Blockthon-4.6.9/Blockthon/Wallet.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      581 2023-07-01 10:38:46.000000 Blockthon-4.6.9/Blockthon/__init__.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    20274 2023-07-01 06:20:10.000000 Blockthon-4.6.9/Blockthon/lib.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:31:18.000000 Blockthon-4.6.9/Blockthon/zCash.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 01:38:11.944797 Blockthon-4.6.9/Blockthon.egg-info/
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/PKG-INFO
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      509 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      166 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/requires.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-02 01:38:11.000000 Blockthon-4.6.9/Blockthon.egg-info/top_level.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 01:38:11.944992 Blockthon-4.6.9/PKG-INFO
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     6378 2023-07-02 01:04:09.000000 Blockthon-4.6.9/README.md
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-02 01:38:11.945163 Blockthon-4.6.9/setup.cfg
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     1498 2023-07-02 01:17:15.000000 Blockthon-4.6.9/setup.py
```

### Comparing `Blockthon-3.6.9/Blockthon/__init__.py` & `Blockthon-4.6.9/Blockthon/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # programmer Mmdrza.Com
 
-__version__: str = "v2.6.3"
+__version__: str = "v4.6.3"
 __license__: str = "MIT"
 __author__: str = "Mohammadreza Fekri"
 __email__: str = "PyMmdrza@gmail.com"
 __description__: str = "Fast And Easy Generated Wallet on Python With Blockthon"
 
 
 __all__: list = [
     "__version__",
     "__license__",
     "__author__",
     "__email__",
     "__description__",
     "Wallet",
+    "Check",
+    "lib",
+    "Utils",
     "Ethereum",
-    "Bitcoin",
     "BitcoinGold",
-    "Dogecoin",
-    "DigiByte",
-    "Dash",
-    "Litecoin",
+    "Tron",
     "Qtum",
     "Ravencoin",
-    "Tron",
-    "zCash",
-    "Base58",
-    "Utils"
-]
+    "Dash",
+    "Dogecoin",
+    "Digibyte",
+    "Litecoin",
+    "zCash"
+]
```

### Comparing `Blockthon-3.6.9/setup.py` & `Blockthon-4.6.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Blockthon",
-    version="3.6.9",
+    version="4.6.9",
     author="Pymmdrza",
     author_email="Pymmdrza@gmail.com",
-    description="Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.",
+    description="Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, "
+                "and Decimal.",
     keywords=['blockthon','bitcoin', 'ethereum', 'tron', 'dogecoin', 'dash', 'qtum', 'litecoin', 'bitcoingold', 'wallet', 'private key', 'mnemonic', 'seed', 'binary', 'hex', 'hunter', 'compress', 'un compress', 'compress address', 'un compress address'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Blockthon/Blockthon",
     project_urls={
-        "Documentation": "https://mmdrza.gitbook.io/blockthon/",
-        "Personal Website": "https://mmdrza.com",
+        "Documentation": "https://blockthon.github.io/Blockthon/",
+        "Personal Website": "https://mmdrza.com"
     },
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

