# Comparing `tmp/dxsp-3.1.1.tar.gz` & `tmp/dxsp-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-3.1.1.tar", max compression
+gzip compressed data, was "dxsp-3.1.2.tar", max compression
```

## Comparing `dxsp-3.1.1.tar` & `dxsp-3.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2023-07-02 12:46:36.966737 dxsp-3.1.1/LICENSE
--rw-r--r--   0        0        0     2378 2023-07-02 12:46:36.966737 dxsp-3.1.1/README.md
--rw-r--r--   0        0        0      114 2023-07-02 12:46:37.714740 dxsp-3.1.1/dxsp/__init__.py
--rw-r--r--   0        0        0      418 2023-07-02 12:46:36.966737 dxsp-3.1.1/dxsp/config.py
--rw-r--r--   0        0        0     8028 2023-07-02 12:46:36.966737 dxsp-3.1.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    15335 2023-07-02 12:46:36.966737 dxsp-3.1.1/dxsp/main.py
--rw-r--r--   0        0        0      103 2023-07-02 12:46:36.966737 dxsp-3.1.1/dxsp/protocols/__init__.py
--rw-r--r--   0        0        0     3536 2023-07-02 12:46:36.966737 dxsp-3.1.1/dxsp/protocols/oneinch.py
--rw-r--r--   0        0        0     2559 2023-07-02 12:46:36.966737 dxsp-3.1.1/dxsp/protocols/uniswap.py
--rw-r--r--   0        0        0      941 2023-07-02 12:46:36.966737 dxsp-3.1.1/dxsp/protocols/zerox.py
--rw-r--r--   0        0        0     2144 2023-07-02 12:46:37.714740 dxsp-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 dxsp-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-02 17:29:16.677899 dxsp-3.1.2/LICENSE
+-rw-r--r--   0        0        0     2378 2023-07-02 17:29:16.677899 dxsp-3.1.2/README.md
+-rw-r--r--   0        0        0      114 2023-07-02 17:29:17.417893 dxsp-3.1.2/dxsp/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-02 17:29:16.677899 dxsp-3.1.2/dxsp/config.py
+-rw-r--r--   0        0        0     8093 2023-07-02 17:29:16.677899 dxsp-3.1.2/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    15355 2023-07-02 17:29:16.677899 dxsp-3.1.2/dxsp/main.py
+-rw-r--r--   0        0        0      103 2023-07-02 17:29:16.677899 dxsp-3.1.2/dxsp/protocols/__init__.py
+-rw-r--r--   0        0        0     3536 2023-07-02 17:29:16.681899 dxsp-3.1.2/dxsp/protocols/oneinch.py
+-rw-r--r--   0        0        0     2645 2023-07-02 17:29:16.681899 dxsp-3.1.2/dxsp/protocols/uniswap.py
+-rw-r--r--   0        0        0      941 2023-07-02 17:29:16.681899 dxsp-3.1.2/dxsp/protocols/zerox.py
+-rw-r--r--   0        0        0     2144 2023-07-02 17:29:17.417893 dxsp-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 dxsp-3.1.2/PKG-INFO
```

### Comparing `dxsp-3.1.1/LICENSE` & `dxsp-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.1/README.md` & `dxsp-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.1/dxsp/default_settings.toml` & `dxsp-3.1.2/dxsp/default_settings.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 dex_protocol_type = "uniswap_v2" #0x
 dex_chain_id = 1
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_0x_url = "https://api.0x.org/mainnet"
 dex_0x_api_key = "" 
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D"
 dex_router_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v2/router02.abi"
+dex_factory_contract_addr = "0x5C69bEe701ef814a2B6a3EDD4B1652CB9cc5aA6f"
 dex_erc20_abi_url = "https://raw.githubusercontent.com/Uniswap/interface/44c355c7f0f8ab5bdb3e0790560e84e59f5666f7/src/abis/erc20.json"
 dex_quoter_contract_addr = "0x61fFE014bA17989E743c5F6cB21bF9697530B21e"
 dex_quoter_abi_url = "https://raw.githubusercontent.com/uniswap-python/uniswap-python/master/uniswap/assets/uniswap-v3/quoter.abi"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_block_explorer_api =  "798437294880920392"
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
@@ -99,15 +100,15 @@
 trading_risk_amount = 10
 dex_trading_slippage = 2
 headers = {User-Agent= 'Mozilla/5.0'}
 token_mainnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/all.json"
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 
-[test_pancake_chain_56]
+[test_chain_56]
 VALUE = "chain_56"
 dex_chain_id = 56
 dxsp_enabled = true
 dex_wallet_address = "0xf977814e90da44bfa03b6295a0616a897441acec"
 dex_protocol_type = "0x"
 dex_rpc = "https://rpc.ankr.com/bsc"
 dex_0x_url = "https://bsc.api.0x.org/"
```

### Comparing `dxsp-3.1.1/dxsp/main.py` & `dxsp-3.1.2/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,24 +178,24 @@
                 abi=router_abi,
             )
             if self.router.functions is None:
                 raise ValueError("Router/Chain setup incorrect")
         except Exception as error:
             raise error
 
-    async def quoter_contract(self):
-        """ create a quoter contract """
-        try:
-            quoter_abi = await self.get(settings.dex_quoter_abi_url)
-            self.quoter = self.w3.eth.contract(
-                address=self.w3.to_checksum_address(
-                    settings.dex_quoter_contract_addr),
-                abi=quoter_abi)
-        except Exception as error:
-            raise error
+    # async def quoter_contract(self):
+    #     """ create a quoter contract """
+    #     try:
+    #         quoter_abi = await self.get(settings.dex_quoter_abi_url)
+    #         self.quoter = self.w3.eth.contract(
+    #             address=self.w3.to_checksum_address(
+    #                 settings.dex_quoter_contract_addr),
+    #             abi=quoter_abi)
+    #     except Exception as error:
+    #         raise error
 
     async def calculate_sell_amount(self, sell_token_address, quantity):
         """Returns amount based on risk percentage."""
         sell_balance = await self.get_token_balance(sell_token_address)
         sell_contract = await self.get_token_contract(sell_token_address)
         sell_decimals = sell_contract.functions.decimals().call() if sell_contract is not None else 18
         risk_percentage = settings.trading_risk_amount
```

### Comparing `dxsp-3.1.1/dxsp/protocols/oneinch.py` & `dxsp-3.1.2/dxsp/protocols/oneinch.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.1/dxsp/protocols/uniswap.py` & `dxsp-3.1.2/dxsp/protocols/uniswap.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 from dxsp.config import settings
 from dxsp.main import DexSwap
 from uniswap import Uniswap
 
 
 
 class DexSwapUniswap(DexSwap):
+   # async def 
+    
+    
     async def get_quote(
         self,
         buy_address,
         sell_address,
         amount=10
     ):
         try:
-            uniswap = Uniswap(address=self.wallet_address, private_key=self.private_key, version=2, web3=self.w3, router_contract_addr=settings.dex_router_contract_addr)
-            uniswap.get_price_input(sell_address, buy_address, amount ** await self.get_token_decimals(buy_address))
+            uniswap = Uniswap(address=self.wallet_address, private_key=self.private_key, version=2, web3=self.w3, factory_contract_addr=settings.dex_factory_contract_addr, router_contract_addr=settings.dex_router_contract_addr)
+            quote = uniswap.get_price_input(sell_address, buy_address, amount ** await self.get_token_decimals(buy_address))
             # await self.router_contract()
             # if self.protocol_type == "uniswap_v2":
             #     await self.router_contract()
             #     path = [sell_address,buy_address]
             #     print(path)
             #     amount_out = self.router.functions.getAmountsOut(
             #         amount * await self.get_token_decimals(buy_address),
@@ -33,15 +36,15 @@
                 # await self.quoter_contract()
                 # sqrtPriceLimitX96 = 0
                 # fee = 3000
                 # quote = self.quoter.functions.quoteExactInputSingle(
                 #     buy_address,
                 #     sell_address,
                 #     fee, amount, sqrtPriceLimitX96).call()
-                # return quote
+            return quote
 
         except Exception as error:
             raise ValueError(f"Quote failed {error}") 
 
 
     async def get_swap(self, sell_address, buy_address, amount):
         try:
```

### Comparing `dxsp-3.1.1/dxsp/protocols/zerox.py` & `dxsp-3.1.2/dxsp/protocols/zerox.py`

 * *Files identical despite different names*

### Comparing `dxsp-3.1.1/pyproject.toml` & `dxsp-3.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "3.1.1"
+version = "3.1.2"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-3.1.1/PKG-INFO` & `dxsp-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 3.1.1
+Version: 3.1.2
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

