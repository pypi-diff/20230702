# Comparing `tmp/dxsp-3.0.3.tar.gz` & `tmp/dxsp-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.0.3.tar", max compression
+gzip compressed data, was "dxsp-3.1.0.tar", max compression
```

## Comparing `dxsp-3.0.3.tar` & `dxsp-3.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-02 07:26:35.069110 dxsp-3.0.3/LICENSE
--rw-r--r--   0        0        0     2249 2023-07-02 07:26:35.069110 dxsp-3.0.3/README.md
--rw-r--r--   0        0        0      114 2023-07-02 07:26:35.873117 dxsp-3.0.3/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/config.py
--rw-r--r--   0        0        0     8028 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0    15086 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     2220 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      941 2023-07-02 07:26:35.069110 dxsp-3.0.3/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2118 2023-07-02 07:26:35.873117 dxsp-3.0.3/pyproject.toml
--rw-r--r--   0        0        0     3051 1970-01-01 00:00:00.000000 dxsp-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-02 09:39:00.649756 dxsp-3.1.0/LICENSE
+-rw-r--r--   0        0        0     2249 2023-07-02 09:39:00.649756 dxsp-3.1.0/README.md
+-rw-r--r--   0        0        0      114 2023-07-02 09:39:01.401756 dxsp-3.1.0/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-02 09:39:00.649756 dxsp-3.1.0/dxsp/config.py
+-rw-r--r--   0        0        0     8028 2023-07-02 09:39:00.649756 dxsp-3.1.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    15086 2023-07-02 09:39:00.649756 dxsp-3.1.0/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-02 09:39:00.649756 dxsp-3.1.0/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-02 09:39:00.649756 dxsp-3.1.0/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     2559 2023-07-02 09:39:00.649756 dxsp-3.1.0/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      941 2023-07-02 09:39:00.649756 dxsp-3.1.0/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2144 2023-07-02 09:39:01.401756 dxsp-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3098 1970-01-01 00:00:00.000000 dxsp-3.1.0/PKG-INFO
```

### Comparing `dxsp-3.0.3/LICENSE` & `dxsp-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.3/README.md` & `dxsp-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.3/dxsp/default_settings.toml` & `dxsp-3.1.0/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.3/dxsp/main.py` & `dxsp-3.1.0/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.3/dxsp/protocols/oneinch.py` & `dxsp-3.1.0/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.3/dxsp/protocols/uniswap.py` & `dxsp-3.1.0/dxsp/protocols/uniswap.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 """
-uniswap V2  🦄
+uniswap  🦄
 """
 from dxsp.config import settings
 from dxsp.main import DexSwap
+from uniswap import Uniswap
+
+
 
 class DexSwapUniswap(DexSwap):
     async def get_quote(
         self,
         buy_address,
         sell_address,
-        amount=1
+        amount=10
     ):
         try:
-            await self.router_contract()
-            if self.protocol_type == "uniswap_v2":
-                await self.router_contract()
-                path = [sell_address,buy_address]
-                print(path)
-                amount_out = self.router.functions.getAmountsOut(
-                    amount * await self.get_token_decimals(buy_address),
-                    path).call()[-1]
-                quote = int(amount_out / await self.get_token_decimals(sell_address))
-                return quote
+            uniswap = Uniswap(address=self.wallet_address, private_key=self.private_key, version=2, web3=self.w3, router_contract_addr=settings.dex_router_contract_addr)
+            uniswap.get_price_input(sell_address, buy_address, amount ** await self.get_token_decimals(buy_address))
+            # await self.router_contract()
+            # if self.protocol_type == "uniswap_v2":
+            #     await self.router_contract()
+            #     path = [sell_address,buy_address]
+            #     print(path)
+            #     amount_out = self.router.functions.getAmountsOut(
+            #         amount * await self.get_token_decimals(buy_address),
+            #         path).call()[-1]
+            #     quote = int(amount_out / await self.get_token_decimals(sell_address))
+            #     return quote
 
-            if self.protocol_type == "uniswap_v3":
-                pass
+            # if self.protocol_type == "uniswap_v3":
+            #     pass
                 # await self.quoter_contract()
                 # sqrtPriceLimitX96 = 0
                 # fee = 3000
                 # quote = self.quoter.functions.quoteExactInputSingle(
                 #     buy_address,
                 #     sell_address,
                 #     fee, amount, sqrtPriceLimitX96).call()
```

### Comparing `dxsp-3.0.3/dxsp/protocols/zerox.py` & `dxsp-3.1.0/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.0.3/pyproject.toml` & `dxsp-3.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "3.0.3"
+version = "3.1.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
@@ -15,14 +15,15 @@
 "Issues" =  "https://github.com/mraniki/dxsp/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 web3 = "^6.4.0"
 pycoingecko = "^3.1.0"
+uniswap-python = "^0.7.0"
 #eip712 = "^0.2.1"
 #eth-ape'[recommended-plugins]' = "^0.6.11"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "^7.34.3"
 pytest = "^7.0"
 pytest-cov = "^4.1"
```

### Comparing `dxsp-3.0.3/PKG-INFO` & `dxsp-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.0.3
+Version: 3.1.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: pycoingecko (>=3.1.0,<4.0.0)
+Requires-Dist: uniswap-python (>=0.7.0,<0.8.0)
 Requires-Dist: web3 (>=6.4.0,<7.0.0)
 Project-URL: Changelog, https://github.com/mraniki/dxsp/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/dxsp/issues
 Project-URL: Support, https://github.com/mraniki/dxsp/discussions
 Description-Content-Type: text/markdown
 
 # DXSP (DeX SwaP)
```

