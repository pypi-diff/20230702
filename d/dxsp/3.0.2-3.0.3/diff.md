# Comparing `tmp/dxsp-3.0.2.tar.gz` & `tmp/dxsp-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.0.2.tar", max compression
+gzip compressed data, was "dxsp-3.0.3.tar", max compression
```

## Comparing `dxsp-3.0.2.tar` & `dxsp-3.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-01 21:19:40.483796 dxsp-3.0.2/LICENSE
--rw-r--r--   0        0        0     2249 2023-07-01 21:19:40.483796 dxsp-3.0.2/README.md
--rw-r--r--   0        0        0      114 2023-07-01 21:19:41.363792 dxsp-3.0.2/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/config.py
--rw-r--r--   0        0        0     8028 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/default_settings.toml
--rw-r--r--   0        0        0    15086 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     2335 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      941 2023-07-01 21:19:40.483796 dxsp-3.0.2/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2118 2023-07-01 21:19:41.363792 dxsp-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     3051 1970-01-01 00:00:00.000000 dxsp-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-02 07:26:35.069110 dxsp-3.0.3/LICENSE
+-rw-r--r--   0        0        0     2249 2023-07-02 07:26:35.069110 dxsp-3.0.3/README.md
+-rw-r--r--   0        0        0      114 2023-07-02 07:26:35.873117 dxsp-3.0.3/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/config.py
+-rw-r--r--   0        0        0     8028 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    15086 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     2220 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      941 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2118 2023-07-02 07:26:35.873117 dxsp-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3051 1970-01-01 00:00:00.000000 dxsp-3.0.3/PKG-INFO
```

### Comparing `dxsp-3.0.2/LICENSE` & `dxsp-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.2/README.md` & `dxsp-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.2/dxsp/default_settings.toml` & `dxsp-3.0.3/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.2/dxsp/main.py` & `dxsp-3.0.3/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.2/dxsp/protocols/oneinch.py` & `dxsp-3.0.3/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.2/dxsp/protocols/uniswap.py` & `dxsp-3.0.3/dxsp/protocols/uniswap.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,20 +14,17 @@
         try:
             await self.router_contract()
             if self.protocol_type == "uniswap_v2":
                 await self.router_contract()
                 path = [sell_address,buy_address]
                 print(path)
                 amount_out = self.router.functions.getAmountsOut(
-                    amount,
+                    amount * await self.get_token_decimals(buy_address),
                     path).call()[-1]
-                quote = int((
-                    amount_out * (10 ** await self.get_token_decimals(sell_address))) 
-                    // ((10 **await self.get_token_decimals(buy_address))
-                     + settings.dex_trading_slippage))
+                quote = int(amount_out / await self.get_token_decimals(sell_address))
                 return quote
 
             if self.protocol_type == "uniswap_v3":
                 pass
                 # await self.quoter_contract()
                 # sqrtPriceLimitX96 = 0
                 # fee = 3000
```

### Comparing `dxsp-3.0.2/dxsp/protocols/zerox.py` & `dxsp-3.0.3/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.2/pyproject.toml` & `dxsp-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "3.0.2"
+version = "3.0.3"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.0.2/PKG-INFO` & `dxsp-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.0.2
+Version: 3.0.3
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

