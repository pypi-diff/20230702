# Comparing `tmp/Blockthon-4.9.9.tar.gz` & `tmp/Blockthon-5.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Blockthon-4.9.9.tar", last modified: Sun Jul  2 03:50:39 2023, max compression
+gzip compressed data, was "Blockthon-5.3.6.tar", last modified: Sun Jul  2 03:54:44 2023, max compression
```

## Comparing `Blockthon-4.9.9.tar` & `Blockthon-5.3.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 03:50:39.253476 Blockthon-4.9.9/
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 03:50:39.252549 Blockthon-4.9.9/Blockthon/
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1620 2023-07-02 03:33:53.000000 Blockthon-4.9.9/Blockthon/Bitcoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:26:12.000000 Blockthon-4.9.9/Blockthon/BitcoinGold.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3810 2023-06-30 08:06:48.000000 Blockthon-4.9.9/Blockthon/Check.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:26:50.000000 Blockthon-4.9.9/Blockthon/Dash.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:29:40.000000 Blockthon-4.9.9/Blockthon/Digibyte.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:27:46.000000 Blockthon-4.9.9/Blockthon/Dogecoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:24:32.000000 Blockthon-4.9.9/Blockthon/Ethereum.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1292 2023-07-02 03:35:14.000000 Blockthon-4.9.9/Blockthon/Litecoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:30:34.000000 Blockthon-4.9.9/Blockthon/Qtum.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:30:06.000000 Blockthon-4.9.9/Blockthon/Ravencoin.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      455 2023-07-01 10:24:32.000000 Blockthon-4.9.9/Blockthon/Tron.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3339 2023-06-30 09:21:44.000000 Blockthon-4.9.9/Blockthon/Utils.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    13912 2023-07-01 22:48:40.000000 Blockthon-4.9.9/Blockthon/Wallet.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      597 2023-07-02 03:31:21.000000 Blockthon-4.9.9/Blockthon/__init__.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    18089 2023-07-02 02:20:10.000000 Blockthon-4.9.9/Blockthon/lib.py
--rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:31:18.000000 Blockthon-4.9.9/Blockthon/zCash.py
-drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 03:50:39.253193 Blockthon-4.9.9/Blockthon.egg-info/
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/PKG-INFO
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      509 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/SOURCES.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/dependency_links.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      166 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/requires.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-02 03:50:39.000000 Blockthon-4.9.9/Blockthon.egg-info/top_level.txt
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     6888 2023-07-02 03:50:39.253358 Blockthon-4.9.9/PKG-INFO
--rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     6378 2023-07-02 01:04:09.000000 Blockthon-4.9.9/README.md
--rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-02 03:50:39.253510 Blockthon-4.9.9/setup.cfg
--rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     1498 2023-07-02 03:45:01.000000 Blockthon-4.9.9/setup.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 03:54:44.786457 Blockthon-5.3.6/
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 03:54:44.785561 Blockthon-5.3.6/Blockthon/
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1620 2023-07-02 03:33:53.000000 Blockthon-5.3.6/Blockthon/Bitcoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:26:12.000000 Blockthon-5.3.6/Blockthon/BitcoinGold.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3810 2023-06-30 08:06:48.000000 Blockthon-5.3.6/Blockthon/Check.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:26:50.000000 Blockthon-5.3.6/Blockthon/Dash.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:29:40.000000 Blockthon-5.3.6/Blockthon/Digibyte.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:27:46.000000 Blockthon-5.3.6/Blockthon/Dogecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:24:32.000000 Blockthon-5.3.6/Blockthon/Ethereum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     1292 2023-07-02 03:35:14.000000 Blockthon-5.3.6/Blockthon/Litecoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      461 2023-07-01 10:30:34.000000 Blockthon-5.3.6/Blockthon/Qtum.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:30:06.000000 Blockthon-5.3.6/Blockthon/Ravencoin.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      455 2023-07-01 10:24:32.000000 Blockthon-5.3.6/Blockthon/Tron.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)     3339 2023-06-30 09:21:44.000000 Blockthon-5.3.6/Blockthon/Utils.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    13912 2023-07-01 22:48:40.000000 Blockthon-5.3.6/Blockthon/Wallet.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      597 2023-07-02 03:31:21.000000 Blockthon-5.3.6/Blockthon/__init__.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)    18089 2023-07-02 02:20:10.000000 Blockthon-5.3.6/Blockthon/lib.py
+-rw-rw-r--   0 mohammadrezafekri   (501) staff       (20)      459 2023-07-01 10:31:18.000000 Blockthon-5.3.6/Blockthon/zCash.py
+drwxr-xr-x   0 mohammadrezafekri   (501) staff       (20)        0 2023-07-02 03:54:44.786143 Blockthon-5.3.6/Blockthon.egg-info/
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     9743 2023-07-02 03:54:44.000000 Blockthon-5.3.6/Blockthon.egg-info/PKG-INFO
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      509 2023-07-02 03:54:44.000000 Blockthon-5.3.6/Blockthon.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)        1 2023-07-02 03:54:44.000000 Blockthon-5.3.6/Blockthon.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)      166 2023-07-02 03:54:44.000000 Blockthon-5.3.6/Blockthon.egg-info/requires.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       10 2023-07-02 03:54:44.000000 Blockthon-5.3.6/Blockthon.egg-info/top_level.txt
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)     9743 2023-07-02 03:54:44.786304 Blockthon-5.3.6/PKG-INFO
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     9303 2023-07-02 03:50:16.000000 Blockthon-5.3.6/README.md
+-rw-r--r--   0 mohammadrezafekri   (501) staff       (20)       38 2023-07-02 03:54:44.786498 Blockthon-5.3.6/setup.cfg
+-rwxrwxrwx   0 mohammadrezafekri   (501) staff       (20)     1498 2023-07-02 03:54:32.000000 Blockthon-5.3.6/setup.py
```

### Comparing `Blockthon-4.9.9/Blockthon/Bitcoin.py` & `Blockthon-5.3.6/Blockthon/Bitcoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.9/Blockthon/Check.py` & `Blockthon-5.3.6/Blockthon/Check.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.9/Blockthon/Litecoin.py` & `Blockthon-5.3.6/Blockthon/Litecoin.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.9/Blockthon/Utils.py` & `Blockthon-5.3.6/Blockthon/Utils.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.9/Blockthon/Wallet.py` & `Blockthon-5.3.6/Blockthon/Wallet.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.9/Blockthon/__init__.py` & `Blockthon-5.3.6/Blockthon/__init__.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.9/Blockthon/lib.py` & `Blockthon-5.3.6/Blockthon/lib.py`

 * *Files identical despite different names*

### Comparing `Blockthon-4.9.9/Blockthon.egg-info/PKG-INFO` & `Blockthon-5.3.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,291 +1,347 @@
-Metadata-Version: 2.1
-Name: Blockthon
-Version: 4.9.9
-Summary: Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, and Decimal.
-Home-page: https://github.com/Blockthon/Blockthon
-Author: Pymmdrza
-Author-email: Pymmdrza@gmail.com
-Project-URL: Documentation, https://blockthon.github.io/Blockthon/
-Project-URL: Personal Website, https://mmdrza.com
-Keywords: blockthon,bitcoin,ethereum,tron,dogecoin,dash,qtum,litecoin,bitcoingold,wallet,private key,mnemonic,seed,binary,hex,hunter,compress,un compress,compress address,un compress address
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# Blockthon
-Blockthon Python Package for Generate and Converting Wallet Private Key and Mnemonic for Address Bitcoin
-
-```bash
-# on windows
-pip install Blockthon
-
-# on Linux
-pip3 install Blockthon
-```
-
-or for download manual:
-```bash
-git clone https://github.com/Blockthon/Blockthon
-cd Blockthon
-make
-```
-
-
-### Private Key
-
-generated random private key without repeat :
-
-```python
-from Blockthon import Wallet
-
-Privatekey = Wallet.getPrivateKey()
-```
----
-### Mnemonic
-Generated random mnemonic with standard size :
-```python
-from Blockthon import Wallet
-# default size 12 . can use [12, 18, 24]
-mnemonicString = Wallet.getMnemonic(size=12)
-```
-----
-### Bytes (seed)
-
-Generated Random Bytes Without Repeat :
-
-```python
-from Blockthon import Wallet
-byte = Wallet.getBytes()
-```
----
-### Binary
-Generate Random Binary Without repeat `0/1`:
-
-```python
-from Blockthon import Wallet
-
-binary_string = Wallet.getBin(256)
-```
----
-### Private Key To Bytes
-```python
-from Blockthon import Wallet
-
-privatekey = Wallet.getPrivateKey()
-# Convert Private Key HEX To Bytes SEED
-byte = Wallet.PrivateKey_To_Bytes(privatekey)
-
-```
----
-### Private Key To Wif
-
-generated private key (hex) and convert to wif compressed and uncompressed.
-```python
-from Blockthon import Wallet
-
-privatekey = Wallet.getPrivateKey()
-# Convert Private key Hex To Wif
-# wif compressed
-wif_compress = Wallet.PrivateKey_To_Wif(privatekey, compress=True)
-# wif Uncompressed
-wif_uncompress = Wallet.PrivateKey_To_Wif(privatekey, compress=False)
-```
----
-### Private Key To Mnemonic
-
-```python
-from Blockthon import Wallet
-
-privatekey = Wallet.getPrivateKey()
-# convert private key [hex] To mnemonic
-mnemonic_string = Wallet.PrivateKey_To_Mnemonics(privatekey, size=12)
-# for size mnemonic can use [12, 18, 24]
-```
----
-### Private Key To Binary
-
-```python
-from Blockthon import Wallet
-
-privatekey = Wallet.getPrivateKey()
-# convert hex to bin
-binary_string = Wallet.PrivateKey_To_Binary(privatekey)
-```
----
-### Private Key To Decimal (int)
-```python
-from Blockthon import Wallet
-
-privatekey = Wallet.getPrivateKey()
-# convert private key hex to number (dec)
-dec = Wallet.PrivateKey_To_Dec(privatekey)
-```
----
-### Private Key To RIPEMD160
-```python
-from Blockthon import Wallet
-
-privatekey = Wallet.getPrivateKey()
-# convert private key to ripemd160 (hash160)
-ripemd160 = Wallet.PrivateKey_To_RIPEMD160(privatekey)
-```
----
-### Private Key To Address
-
-convert private key `Hex` to Compress and Uncompress Address
-```python
-from Blockthon import Wallet
-
-privatekey = Wallet.getPrivateKey()
-# convert private key to compress address
-compress_Address = Wallet.PrivateKey_To_Address(privatekey, compress=True)
-# convert to uncompress address
-uncompress_Address = Wallet.PrivateKey_To_Address(privatekey, compress=False)
-```
----
-### Private Key To Public Key
-
-generated private key and convert to public key compress and uncompress:
-
-```python
-from Blockthon import Wallet
-
-privatekey = Wallet.getPrivateKey()
-# convert to public key uncompress
-public_uncompress = Wallet.PrivateKey_To_PublicKey(privatekey)
-# convert private key hex to public key compress
-public_compress = Wallet.PrivateKey_To_PublicKey(privatekey, compress=True)
-```
----
-### Bytes To Private Key
-```python
-from Blockthon import Wallet
-
-byte = Wallet.getBytes()
-# convert bytes to hex (private key)
-privatekey = Wallet.Bytes_To_PrivateKey(byte)
-```
-### Bytes To mnemonic 
-convert bytes to mnemonic with default `size=12`
-
-can use standard sizr: `12, 18, 24`
-
-```python
-from Blockthon import Wallet
-
-byte = Wallet.getBytes()
-# Convert bytes to mnemonic with default size 12
-mnemonic_words = Wallet.Bytes_To_Mnemonic(byte, 12)
-```
----
-### Bytes To Wif
-convert bytes To wif Compress and uncompress:
-```python
-from Blockthon import Wallet
-
-byte = Wallet.getBytes()
-# compress wif
-wif_compress = Wallet.Bytes_To_Wif(byte, compress=True)
-#uncompress Wif
-wif_uncompress = Wallet.Bytes_To_Wif(byte, compress=False)
-```
----
-### Bytes To Public Key
-
-convert bytes to public key compress and uncompress
-```python
-from Blockthon import Wallet
-
-byte = Wallet.getBytes()
-# compress Publickey
-Pub_compress = Wallet.Bytes_To_PublicKey(byte, compress=True)
-#uncompress Wif
-Pub_uncompress = Wallet.Bytes_To_PublicKey(byte, compress=False)
-```
----
-### Bytes to Dec (number)
-
-convert bytes to decimal number
-
-```python
-from Blockthon import Wallet
-
-byte = Wallet.getBytes()
-#convert to integer 
-dec = Wallet.Bytes_To_Dec(byte)
-```
----
-### Wif To Public Key
-convert wif to public key compress and uncompress
-```python
-from Blockthon import Wallet
-
-wif = "WIF_STRING_HERE"
-pub_compress = Wallet.Wif_To_PublicKey(wif, compress=True)
-pub_uncompress = Wallet.Wif_To_PublicKey(wif)
-```
----
-### Wif To Mnemonic 
-convert Wif To Mnemonic With Default `size=12`, Can use Standard Size `12, 18, 24`
-```python
-from Blockthon import Wallet
-
-wif = "WIF_STRING_HERE"
-mnemonic_string = Wallet.Wif_To_Mnemonic(wif, 12)
-```
----
-### Wif To RIPEMD160
-convert wif to RIPEMD160 return `hex string` 
-```python
-from Blockthon import Wallet
-
-wif = "WIF_STRING_HERE"
-RIPEMD160 = Wallet.Wif_To_RIPEMD160(wif)
-```
-### Mnemonic To Root Key (XPRV)
-```python
-from Blockthon import Wallet
-
-mnemonic_string = Wallet.getMnemonic(12)
-xprv = Wallet.Mnemonic_To_RootKey(mnemonic_string)
-```
----
-### Mnemonic To Private key
-```python
-from Blockthon import Wallet
-
-mnemonic_string = Wallet.getMnemonic(12)
-pivatekey = Wallet.Mnemonic_To_PrivateKey()
-
-```
----
-### Mnemonic To Address
-convert mnemonic to compressed and uncompressed Address
-```python
-from Blockthon import Wallet
-
-mnemonic_string = Wallet.getMnemonic(12)
-# compress Address
-compress_Address = Wallet.Mnemonic_To_Address(mnemonic_string, True)
-# uncompress Address
-uncompress_Address = Wallet.Mnemonic_To_Address(mnemonic_stringm False)
-```
----
-### Passphrase To Private Key
-convert word passphrase to private key (hex)
-```python
-from Blockthon import Wallet
-passphrase = 'Mmdrza.Com'
-privatekey = Wallet.Passphrase_To_PrivateKey(passphrase)
-```
----
-### Passphrase to Wif
-```python
-from Blockthon import Wallet
-
-passphrase = 'Mmdrza.Com'
-
-wif = Wallet.Passphrase_To_Wif(passphrase)
-```
+# Blockthon
+Blockthon Python Package for Generate and Converting Wallet Private Key and Mnemonic for Address Bitcoin
+
+```bash
+# on windows
+pip install Blockthon
+
+# on Linux
+pip3 install Blockthon
+```
+
+or for download manual:
+```bash
+git clone https://github.com/Blockthon/Blockthon
+cd Blockthon
+make
+```
+---
+
+### Private Key
+
+generated random private key without repeat :
+
+```python
+from Blockthon import Wallet
+
+Privatekey = Wallet.getPrivateKey()
+```
+---
+### Mnemonic
+Generated random mnemonic with standard size :
+```python
+from Blockthon import Wallet
+# default size 12 . can use [12, 18, 24]
+mnemonicString = Wallet.getMnemonic(size=12)
+```
+----
+### Bytes (seed)
+
+Generated Random Bytes Without Repeat :
+
+```python
+from Blockthon import Wallet
+byte = Wallet.getBytes()
+```
+---
+### Binary
+Generate Random Binary Without repeat `0/1`:
+
+```python
+from Blockthon import Wallet
+
+binary_string = Wallet.getBin(256)
+```
+---
+### Private Key To Bytes
+```python
+from Blockthon import Wallet
+
+privatekey = Wallet.getPrivateKey()
+# Convert Private Key HEX To Bytes SEED
+byte = Wallet.PrivateKey_To_Bytes(privatekey)
+
+```
+---
+### Private Key To Wif
+
+generated private key (hex) and convert to wif compressed and uncompressed.
+```python
+from Blockthon import Wallet
+
+privatekey = Wallet.getPrivateKey()
+# Convert Private key Hex To Wif
+# wif compressed
+wif_compress = Wallet.PrivateKey_To_Wif(privatekey, compress=True)
+# wif Uncompressed
+wif_uncompress = Wallet.PrivateKey_To_Wif(privatekey, compress=False)
+```
+---
+### Private Key To Mnemonic
+
+```python
+from Blockthon import Wallet
+
+privatekey = Wallet.getPrivateKey()
+# convert private key [hex] To mnemonic
+mnemonic_string = Wallet.PrivateKey_To_Mnemonics(privatekey, size=12)
+# for size mnemonic can use [12, 18, 24]
+```
+---
+### Private Key To Binary
+
+```python
+from Blockthon import Wallet
+
+privatekey = Wallet.getPrivateKey()
+# convert hex to bin
+binary_string = Wallet.PrivateKey_To_Binary(privatekey)
+```
+---
+### Private Key To Decimal (int)
+```python
+from Blockthon import Wallet
+
+privatekey = Wallet.getPrivateKey()
+# convert private key hex to number (dec)
+dec = Wallet.PrivateKey_To_Dec(privatekey)
+```
+---
+### Private Key To RIPEMD160
+```python
+from Blockthon import Wallet
+
+privatekey = Wallet.getPrivateKey()
+# convert private key to ripemd160 (hash160)
+ripemd160 = Wallet.PrivateKey_To_RIPEMD160(privatekey)
+```
+---
+### Private Key To Address
+
+convert private key `Hex` to Compress and Uncompress Address
+```python
+from Blockthon import Wallet
+
+privatekey = Wallet.getPrivateKey()
+# convert private key to compress address
+compress_Address = Wallet.PrivateKey_To_Address(privatekey, compress=True)
+# convert to uncompress address
+uncompress_Address = Wallet.PrivateKey_To_Address(privatekey, compress=False)
+```
+---
+### Private Key To Public Key
+
+generated private key and convert to public key compress and uncompress:
+
+```python
+from Blockthon import Wallet
+
+privatekey = Wallet.getPrivateKey()
+# convert to public key uncompress
+public_uncompress = Wallet.PrivateKey_To_PublicKey(privatekey)
+# convert private key hex to public key compress
+public_compress = Wallet.PrivateKey_To_PublicKey(privatekey, compress=True)
+```
+---
+### Bytes To Private Key
+```python
+from Blockthon import Wallet
+
+byte = Wallet.getBytes()
+# convert bytes to hex (private key)
+privatekey = Wallet.Bytes_To_PrivateKey(byte)
+```
+### Bytes To mnemonic 
+convert bytes to mnemonic with default `size=12`
+
+can use standard sizr: `12, 18, 24`
+
+```python
+from Blockthon import Wallet
+
+byte = Wallet.getBytes()
+# Convert bytes to mnemonic with default size 12
+mnemonic_words = Wallet.Bytes_To_Mnemonic(byte, 12)
+```
+---
+### Bytes To Wif
+convert bytes To wif Compress and uncompress:
+```python
+from Blockthon import Wallet
+
+byte = Wallet.getBytes()
+# compress wif
+wif_compress = Wallet.Bytes_To_Wif(byte, compress=True)
+#uncompress Wif
+wif_uncompress = Wallet.Bytes_To_Wif(byte, compress=False)
+```
+---
+### Bytes To Public Key
+
+convert bytes to public key compress and uncompress
+```python
+from Blockthon import Wallet
+
+byte = Wallet.getBytes()
+# compress Publickey
+Pub_compress = Wallet.Bytes_To_PublicKey(byte, compress=True)
+#uncompress Wif
+Pub_uncompress = Wallet.Bytes_To_PublicKey(byte, compress=False)
+```
+---
+### Bytes to Dec (number)
+
+convert bytes to decimal number
+
+```python
+from Blockthon import Wallet
+
+byte = Wallet.getBytes()
+#convert to integer 
+dec = Wallet.Bytes_To_Dec(byte)
+```
+---
+### Wif To Public Key
+convert wif to public key compress and uncompress
+```python
+from Blockthon import Wallet
+
+wif = "WIF_STRING_HERE"
+pub_compress = Wallet.Wif_To_PublicKey(wif, compress=True)
+pub_uncompress = Wallet.Wif_To_PublicKey(wif)
+```
+---
+### Wif To Mnemonic 
+convert Wif To Mnemonic With Default `size=12`, Can use Standard Size `12, 18, 24`
+```python
+from Blockthon import Wallet
+
+wif = "WIF_STRING_HERE"
+mnemonic_string = Wallet.Wif_To_Mnemonic(wif, 12)
+```
+---
+### Wif To RIPEMD160
+convert wif to RIPEMD160 return `hex string` 
+```python
+from Blockthon import Wallet
+
+wif = "WIF_STRING_HERE"
+RIPEMD160 = Wallet.Wif_To_RIPEMD160(wif)
+```
+### Mnemonic To Root Key (XPRV)
+```python
+from Blockthon import Wallet
+
+mnemonic_string = Wallet.getMnemonic(12)
+xprv = Wallet.Mnemonic_To_RootKey(mnemonic_string)
+```
+---
+### Mnemonic To Private key
+```python
+from Blockthon import Wallet
+
+mnemonic_string = Wallet.getMnemonic(12)
+pivatekey = Wallet.Mnemonic_To_PrivateKey()
+
+```
+---
+### Mnemonic To Address
+convert mnemonic to compressed and uncompressed Address
+```python
+from Blockthon import Wallet
+
+mnemonic_string = Wallet.getMnemonic(12)
+# compress Address
+compress_Address = Wallet.Mnemonic_To_Address(mnemonic_string, True)
+# uncompress Address
+uncompress_Address = Wallet.Mnemonic_To_Address(mnemonic_stringm False)
+```
+---
+### Passphrase To Private Key
+convert word passphrase to private key (hex)
+```python
+from Blockthon import Wallet
+passphrase = 'Mmdrza.Com'
+privatekey = Wallet.Passphrase_To_PrivateKey(passphrase)
+```
+---
+### Passphrase to Wif
+```python
+from Blockthon import Wallet
+
+passphrase = 'Mmdrza.Com'
+
+wif = Wallet.Passphrase_To_Wif(passphrase)
+```
+---
+Example:
+```python
+from Blockthon import Wallet, Ethereum, Tron, Dogecoin, Bitcoin, Litecoin, Dash, Digibyte, BitcoinGold, Ravencoin, Qtum, zCash
+
+seed = Wallet.getSeed()
+privatekey = Wallet.Bytes_To_PrivateKey(seed)
+mnemonics = Wallet.Bytes_To_Mnemonic(seed, 12)
+wif_compress = Wallet.Bytes_To_Wif(seed, compress=True)
+wif_uncompress = Wallet.Bytes_To_Wif(seed, compress=False)
+dec = Wallet.Bytes_To_Dec(seed)
+xprv = Wallet.Mnemonic_To_RootKey(mnemonics)
+publickey = Wallet.Bytes_To_PublicKey(seed)
+ripemd160 = Wallet.Bytes_To_RIPEMD160(seed)
+compressAddress = Wallet.Bytes_To_Address(seed, compress=True)
+uncompressAddress = Wallet.Bytes_To_Address(seed, compress=False)
+p2pkhAddress = Bitcoin.Address_From_PrivateKey(privatekey, Type='P2PKH')
+p2shAddress = Bitcoin.Address_From_PrivateKey(privatekey, Type='P2SH')
+p2wpkhAddress = Bitcoin.Address_From_PrivateKey(privatekey, Type='P2WPKH')
+p2wshAddress = Bitcoin.Address_From_PrivateKey(privatekey, Type='P2WSH')
+p2wpkhSegwit = Bitcoin.Address_From_PrivateKey(privatekey, Type='P2WPKHinP2SH')
+p2wshSegwit = Bitcoin.Address_From_PrivateKey(privatekey, Type='P2WSHinP2SH')
+p2pkh_ltc = Litecoin.Address_From_PrivateKey(privatekey, 'P2PKH')
+p2sh_ltc = Litecoin.Address_From_PrivateKey(privatekey, 'P2SH')
+p2wpkh_ltc = Litecoin.Address_From_PrivateKey(privatekey, 'P2WPKH')
+p2wsh_ltc = Litecoin.Address_From_PrivateKey(privatekey, 'P2WSH')
+ethereumAddress = Ethereum.Address_From_PrivateKey(privatekey)
+tronAddress = Tron.Address_From_PrivateKey(privatekey)
+dogeAddress = Dogecoin.Address_From_PrivateKey(privatekey)
+dashAddress = Dash.Address_From_PrivateKey(privatekey)
+digibyteAddress = Digibyte.Address_From_PrivateKey(privatekey)
+RVNAddress = Ravencoin.Address_From_PrivateKey(privatekey)
+QtumAddress = Qtum.Address_From_PrivateKey(privatekey)
+zcashAddress = zCash.Address_From_PrivateKey(privatekey)
+print(f"""
+Seed : {seed}
+PrivateKey [Hex]: {privatekey}
+Mnemonic: {mnemonics}
+Wif Compressed: {wif_compress}
+Wif UnCompressed: {wif_uncompress}
+Decimal: {dec}
+RIPEMD160: {ripemd160}
+{'-' * 22} Address's {'-' * 22}
+Compressed Address: {compressAddress}
+UnCompressed Address: {uncompressAddress}
+Bitcoin P2PKH: {p2pkhAddress}
+Bitcoin P2SH: {p2shAddress}
+Bitcoin P2WPKH: {p2wpkhAddress}
+Bitcoin P2WSH: {p2wshAddress}
+Bitcoin P2WPKH in Segwit: {p2wpkhSegwit}
+Bitcoin P2WSH in Segwit: {p2wshSegwit}
+Litecoin P2PKH: {p2pkh_ltc}
+Litecoin P2SH: {p2sh_ltc}
+Litecoin P2WSH: {p2wsh_ltc}
+Litecoin P2WPKH: {p2wpkh_ltc}
+Ethereum: {ethereumAddress}
+Tron: {tronAddress}
+Dogecoin: {dogeAddress}
+DASH: {dashAddress}
+DigiByte: {digibyteAddress}
+Ravencoin: {RVNAddress}
+QTUM: {QtumAddress}
+zCASH: {zcashAddress} 
+""")
+```
+Programmer & Owner : Mmdrza.Com
+
+Email : PyMmdrza@Gmail.Com
+
+Github: [Blockthon/Blockthon](https://github.com/Blockthon/Blockthon)
+
+Document: [Blockthon](https://blockthon.github.io/Blockthon)
```

### Comparing `Blockthon-4.9.9/setup.py` & `Blockthon-5.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="Blockthon",
-    version="4.9.9",
+    version="5.3.6",
     author="Pymmdrza",
     author_email="Pymmdrza@gmail.com",
     description="Blockthon: Fast and easy generation of Private Keys and Mnemonics, converting Seed, Binary, "
                 "and Decimal.",
     keywords=['blockthon','bitcoin', 'ethereum', 'tron', 'dogecoin', 'dash', 'qtum', 'litecoin', 'bitcoingold', 'wallet', 'private key', 'mnemonic', 'seed', 'binary', 'hex', 'hunter', 'compress', 'un compress', 'compress address', 'un compress address'],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

