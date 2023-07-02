# Comparing `tmp/Blockthon-4.9.6.tar.gz` & `tmp/Blockthon-4.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Blockthon-4.9.6.tar", last modified: Sun Jul  2 02:31:47 2023, max compression
+gzip compressed data, was "Blockthon-4.9.9.tar", last modified: Sun Jul  2 03:50:39 2023, max compression
```

## Comparing `Blockthon-4.9.6.tar` & `Blockthon-4.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 02:31:47.699440 Blockthon-4.9.6/
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 02:31:47.698354 Blockthon-4.9.6/Blockthon/
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1716 2023-07-01 10:53:50.000000 Blockthon-4.9.6/Blockthon/Bitcoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:26:12.000000 Blockthon-4.9.6/Blockthon/BitcoinGold.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3810 2023-06-30 08:06:48.000000 Blockthon-4.9.6/Blockthon/Check.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:26:50.000000 Blockthon-4.9.6/Blockthon/Dash.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:29:40.000000 Blockthon-4.9.6/Blockthon/Digibyte.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:27:46.000000 Blockthon-4.9.6/Blockthon/Dogecoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:24:32.000000 Blockthon-4.9.6/Blockthon/Ethereum.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1356 2023-07-01 10:52:46.000000 Blockthon-4.9.6/Blockthon/Litecoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:30:34.000000 Blockthon-4.9.6/Blockthon/Qtum.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:30:06.000000 Blockthon-4.9.6/Blockthon/Ravencoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      455 2023-07-01 10:24:32.000000 Blockthon-4.9.6/Blockthon/Tron.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3339 2023-06-30 09:21:44.000000 Blockthon-4.9.6/Blockthon/Utils.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    13912 2023-07-01 22:48:40.000000 Blockthon-4.9.6/Blockthon/Wallet.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      581 2023-07-01 10:38:46.000000 Blockthon-4.9.6/Blockthon/__init__.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    18089 2023-07-02 02:20:10.000000 Blockthon-4.9.6/Blockthon/lib.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:31:18.000000 Blockthon-4.9.6/Blockthon/zCash.py
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 02:31:47.699116 Blockthon-4.9.6/Blockthon.egg-info/
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/PKG-INFO
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      509 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/SOURCES.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/dependency_links.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      166 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/requires.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-02 02:31:47.000000 Blockthon-4.9.6/Blockthon.egg-info/top_level.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 02:31:47.699322 Blockthon-4.9.6/PKG-INFO
--rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     6378 2023-07-02 01:04:09.000000 Blockthon-4.9.6/README.md
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-02 02:31:47.699481 Blockthon-4.9.6/setup.cfg
--rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     1498 2023-07-02 02:31:18.000000 Blockthon-4.9.6/setup.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 03:50:39.253476 Blockthon-4.9.9/
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 03:50:39.252549 Blockthon-4.9.9/Blockthon/
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1620 2023-07-02 03:33:53.000000 Blockthon-4.9.9/Blockthon/Bitcoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:26:12.000000 Blockthon-4.9.9/Blockthon/BitcoinGold.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3810 2023-06-30 08:06:48.000000 Blockthon-4.9.9/Blockthon/Check.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:26:50.000000 Blockthon-4.9.9/Blockthon/Dash.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:29:40.000000 Blockthon-4.9.9/Blockthon/Digibyte.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:27:46.000000 Blockthon-4.9.9/Blockthon/Dogecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:24:32.000000 Blockthon-4.9.9/Blockthon/Ethereum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1292 2023-07-02 03:35:14.000000 Blockthon-4.9.9/Blockthon/Litecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:30:34.000000 Blockthon-4.9.9/Blockthon/Qtum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:30:06.000000 Blockthon-4.9.9/Blockthon/Ravencoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      455 2023-07-01 10:24:32.000000 Blockthon-4.9.9/Blockthon/Tron.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3339 2023-06-30 09:21:44.000000 Blockthon-4.9.9/Blockthon/Utils.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    13912 2023-07-01 22:48:40.000000 Blockthon-4.9.9/Blockthon/Wallet.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      597 2023-07-02 03:31:21.000000 Blockthon-4.9.9/Blockthon/__init__.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    18089 2023-07-02 02:20:10.000000 Blockthon-4.9.9/Blockthon/lib.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:31:18.000000 Blockthon-4.9.9/Blockthon/zCash.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 03:50:39.253193 Blockthon-4.9.9/Blockthon.egg-info/
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/PKG-INFO
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      509 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      166 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/requires.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/top_level.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 03:50:39.253358 Blockthon-4.9.9/PKG-INFO
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     6378 2023-07-02 01:04:09.000000 Blockthon-4.9.9/README.md
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-02 03:50:39.253510 Blockthon-4.9.9/setup.cfg
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     1498 2023-07-02 03:45:01.000000 Blockthon-4.9.9/setup.py
```

### Comparing `Blockthon-4.9.6/Blockthon/Bitcoin.py` & `Blockthon-4.9.9/Blockthon/Litecoin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-from .Utils import HexToBTC
+from .Utils import HexToLTC
 from .lib import Hexlify, MnemonicToBytes, DecToBytes
 
 
 def Address_From_PrivateKey(privatekey: str, Type: str) -> str:
     """
-    Convert Private Key (Hex) To All Type's Bitcoin Address.
+    Convert Private Key (Hex) To All Type's Litecoin Address.
 
-    >>> # Example Address With a Type's: 'P2PKH'/'P2SH'/'P2WPKH'/'P2WSH'/'P2WPKHinP2SH'/ 'P2WSHinP2SH'
-    >>> P2PKH = Address_From_PrivateKey(privatekey, Type='P2PKH')
-    >>> P2SH = Address_From_PrivateKey(privatekey, Type='P2SH')
-    >>> P2WPKH = Address_From_PrivateKey(privatekey, Type='P2WPKH')
-    >>> P2WSH = Address_From_PrivateKey(privatekey, Type='P2WSH')
-    >>> P2WPKH_Segwit = Address_From_PrivateKey(privatekey, Type='P2WPKHinP2SH')
-    >>> P2WSH_Segwit = Address_From_PrivateKey(privatekey, Type='P2WSHinP2SH')
+    >>> # Example Address With Type's: 'P2PKH'/'P2SH'/'P2WPKH'/'P2WSH'
+    >>> P2PKH_Litecoin = Address_From_PrivateKey(privatekey, Type='P2PKH')
+    >>> P2SH_Litecoin = Address_From_PrivateKey(privatekey, Type='P2SH')
+    >>> P2WPKH_Litecoin = Address_From_PrivateKey(privatekey, Type='P2WPKH')
+    >>> P2WSH_Litecoin = Address_From_PrivateKey(privatekey, Type='P2WSH')
 
-    :return: BitcoinAddress_string.
+    :return: LitecoinAddress_string.
     """
-    if Type == 'P2PKH' or Type.lower():
-        return HexToBTC(privatekey, 'P2PKH')
-    elif Type == 'P2SH' or Type.lower():
-        return HexToBTC(privatekey, 'P2SH')
-    elif Type == 'P2WSH' or Type.lower():
-        return HexToBTC(privatekey, 'P2WSH')
-    elif Type == 'P2WPKH' or Type.lower():
-        return HexToBTC(privatekey, 'P2WPKH')
-    elif Type == 'P2WPKHinP2SH' or Type.lower():
-        return HexToBTC(privatekey, 'P2WPKHinP2SH')
-    elif Type == 'P2WSHinP2SH' or Type.lower():
-        return HexToBTC(privatekey, 'P2WSHinP2SH')
+    if Type == 'P2PKH':
+        return HexToLTC(privatekey, 'P2PKH')
+    elif Type == 'P2SH':
+        return HexToLTC(privatekey, 'P2SH')
+    elif Type == 'P2WSH':
+        return HexToLTC(privatekey, 'P2WSH')
+    elif Type == 'P2WPKH':
+        return HexToLTC(privatekey, 'P2WPKH')
     else:
-        return HexToBTC(privatekey, 'P2PKH')
+        return HexToLTC(privatekey, 'P2PKH')
 
 
 def Address_From_Bytes(byte: bytes) -> str: return Address_From_PrivateKey(Hexlify(byte))
 
 
 def Address_From_Mnemonic(mnemonics: str) -> str: return Address_From_Bytes(MnemonicToBytes(mnemonics))
```

### Comparing `Blockthon-4.9.6/Blockthon/Check.py` & `Blockthon-4.9.9/Blockthon/Check.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.6/Blockthon/Litecoin.py` & `Blockthon-4.9.9/Blockthon/Bitcoin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,39 @@
-from .Utils import HexToLTC
+from .Utils import HexToBTC
 from .lib import Hexlify, MnemonicToBytes, DecToBytes
 
 
 def Address_From_PrivateKey(privatekey: str, Type: str) -> str:
     """
-    Convert Private Key (Hex) To All Type's Litecoin Address.
+    Convert Private Key (Hex) To All Type's Bitcoin Address.
 
-    >>> # Example Address With Type's: 'P2PKH'/'P2SH'/'P2WPKH'/'P2WSH'
-    >>> P2PKH_Litecoin = Address_From_PrivateKey(privatekey, Type='P2PKH')
-    >>> P2SH_Litecoin = Address_From_PrivateKey(privatekey, Type='P2SH')
-    >>> P2WPKH_Litecoin = Address_From_PrivateKey(privatekey, Type='P2WPKH')
-    >>> P2WSH_Litecoin = Address_From_PrivateKey(privatekey, Type='P2WSH')
+    >>> # Example Address With a Type's: 'P2PKH'/'P2SH'/'P2WPKH'/'P2WSH'/'P2WPKHinP2SH'/ 'P2WSHinP2SH'
+    >>> P2PKH = Address_From_PrivateKey(privatekey, Type='P2PKH')
+    >>> P2SH = Address_From_PrivateKey(privatekey, Type='P2SH')
+    >>> P2WPKH = Address_From_PrivateKey(privatekey, Type='P2WPKH')
+    >>> P2WSH = Address_From_PrivateKey(privatekey, Type='P2WSH')
+    >>> P2WPKH_Segwit = Address_From_PrivateKey(privatekey, Type='P2WPKHinP2SH')
+    >>> P2WSH_Segwit = Address_From_PrivateKey(privatekey, Type='P2WSHinP2SH')
 
-    :return: LitecoinAddress_string.
+    :return: BitcoinAddress_string.
     """
-    if Type == 'P2PKH' or Type.lower():
-        return HexToLTC(privatekey, 'P2PKH')
-    elif Type == 'P2SH' or Type.lower():
-        return HexToLTC(privatekey, 'P2SH')
-    elif Type == 'P2WSH' or Type.lower():
-        return HexToLTC(privatekey, 'P2WSH')
-    elif Type == 'P2WPKH' or Type.lower():
-        return HexToLTC(privatekey, 'P2WPKH')
+    if Type == 'P2PKH':
+        return HexToBTC(privatekey, 'P2PKH')
+    elif Type == 'P2SH':
+        return HexToBTC(privatekey, 'P2SH')
+    elif Type == 'P2WSH':
+        return HexToBTC(privatekey, 'P2WSH')
+    elif Type == 'P2WPKH':
+        return HexToBTC(privatekey, 'P2WPKH')
+    elif Type == 'P2WPKHinP2SH':
+        return HexToBTC(privatekey, 'P2WPKHinP2SH')
+    elif Type == 'P2WSHinP2SH':
+        return HexToBTC(privatekey, 'P2WSHinP2SH')
     else:
-        return HexToLTC(privatekey, 'P2PKH')
+        return HexToBTC(privatekey, 'P2PKH')
 
 
 def Address_From_Bytes(byte: bytes) -> str: return Address_From_PrivateKey(Hexlify(byte))
 
 
 def Address_From_Mnemonic(mnemonics: str) -> str: return Address_From_Bytes(MnemonicToBytes(mnemonics))
```

### Comparing `Blockthon-4.9.6/Blockthon/Utils.py` & `Blockthon-4.9.9/Blockthon/Utils.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.6/Blockthon/Wallet.py` & `Blockthon-4.9.9/Blockthon/Wallet.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.6/Blockthon/__init__.py` & `Blockthon-4.9.9/Blockthon/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "__email__",
     "__description__",
     "Wallet",
     "Check",
     "lib",
     "Utils",
     "Ethereum",
+    "Bitcoin",
     "BitcoinGold",
     "Tron",
     "Qtum",
     "Ravencoin",
     "Dash",
     "Dogecoin",
     "Digibyte",
```

### Comparing `Blockthon-4.9.6/Blockthon/lib.py` & `Blockthon-4.9.9/Blockthon/lib.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.6/Blockthon.egg-info/PKG-INFO` & `Blockthon-4.9.9/Blockthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 4.9.6
+Version: 4.9.9
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 Project-URL: Documentation, https://blockthon.github.io/Blockthon/
 Project-URL: Personal Website, https://mmdrza.com
 Keywords: blockthon,bitcoin,ethereum,tron,dogecoin,dash,qtum,litecoin,bitcoingold,wallet,private key,mnemonic,seed,binary,hex,hunter,compress,un compress,compress address,un compress address
```

### Comparing `Blockthon-4.9.6/PKG-INFO` & `Blockthon-4.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Blockthon
-Version: 4.9.6
+Version: 4.9.9
 Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
 Home-page: https://github.com/Blockthon/Blockthon
 Author: Pymmdrza
 Author-email: Pymmdrza@gmail.com
 Project-URL: Documentation, https://blockthon.github.io/Blockthon/
 Project-URL: Personal Website, https://mmdrza.com
 Keywords: blockthon,bitcoin,ethereum,tron,dogecoin,dash,qtum,litecoin,bitcoingold,wallet,private key,mnemonic,seed,binary,hex,hunter,compress,un compress,compress address,un compress address
```

### Comparing `Blockthon-4.9.6/README.md` & `Blockthon-4.9.9/README.md`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.6/setup.py` & `Blockthon-4.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Blockthon",
-    version="4.9.6",
+    version="4.9.9",
     author="Pymmdrza",
     author_email="Pymmdrza@gmail.com",
     description="Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, "
                 "and Decimal.",
     keywords=['blockthon','bitcoin', 'ethereum', 'tron', 'dogecoin', 'dash', 'qtum', 'litecoin', 'bitcoingold', 'wallet', 'private key', 'mnemonic', 'seed', 'binary', 'hex', 'hunter', 'compress', 'un compress', 'compress address', 'un compress address'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

