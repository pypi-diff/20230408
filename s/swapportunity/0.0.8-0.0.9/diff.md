# Comparing `tmp/swapportunity-0.0.8.tar.gz` & `tmp/swapportunity-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swapportunity-0.0.8.tar", last modified: Sat Apr  8 15:49:17 2023, max compression
+gzip compressed data, was "swapportunity-0.0.9.tar", last modified: Sat Apr  8 16:07:23 2023, max compression
```

## Comparing `swapportunity-0.0.8.tar` & `swapportunity-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:49:17.004624 swapportunity-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 15:49:07.000000 swapportunity-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-08 15:49:17.004624 swapportunity-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-08 15:49:07.000000 swapportunity-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-08 15:49:07.000000 swapportunity-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 15:49:17.004624 swapportunity-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:49:17.004624 swapportunity-0.0.8/swapportunity/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-08 15:49:07.000000 swapportunity-0.0.8/swapportunity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-08 15:49:07.000000 swapportunity-0.0.8/swapportunity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:49:17.004624 swapportunity-0.0.8/swapportunity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-08 15:49:16.000000 swapportunity-0.0.8/swapportunity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-08 15:49:17.000000 swapportunity-0.0.8/swapportunity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 15:49:16.000000 swapportunity-0.0.8/swapportunity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 15:49:16.000000 swapportunity-0.0.8/swapportunity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:07:23.270139 swapportunity-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 16:07:10.000000 swapportunity-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-08 16:07:23.270139 swapportunity-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-08 16:07:10.000000 swapportunity-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-08 16:07:10.000000 swapportunity-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:07:23.270139 swapportunity-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:07:23.270139 swapportunity-0.0.9/swapportunity/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-08 16:07:10.000000 swapportunity-0.0.9/swapportunity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-08 16:07:10.000000 swapportunity-0.0.9/swapportunity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:07:23.270139 swapportunity-0.0.9/swapportunity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-08 16:07:23.000000 swapportunity-0.0.9/swapportunity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-08 16:07:23.000000 swapportunity-0.0.9/swapportunity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:07:23.000000 swapportunity-0.0.9/swapportunity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 16:07:23.000000 swapportunity-0.0.9/swapportunity.egg-info/top_level.txt
```

### Comparing `swapportunity-0.0.8/LICENSE` & `swapportunity-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `swapportunity-0.0.8/PKG-INFO` & `swapportunity-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swapportunity
-Version: 0.0.8
+Version: 0.0.9
 Summary: A defi swap helper package
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/swapportunity
 Project-URL: Bug Tracker, https://github.com/mraniki/swapportunity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swapportunity-0.0.8/README.md` & `swapportunity-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `swapportunity-0.0.8/pyproject.toml` & `swapportunity-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "swapportunity"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="MrAniki" },
 ]
 description = "A defi swap helper package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `swapportunity-0.0.8/swapportunity/main.py` & `swapportunity-0.0.9/swapportunity/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,49 +31,83 @@
                  wallet_address = 0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE,
                  private_key = 0x111111111117dc0aa78b770fa6a738034120c302,
                  execution_mode=1,
                  dex_exchange = 'uniswap_v2'
                  ):
         self.w3 = w3
         self.chain_id = chain_id
-        self.address = wallet_address
+        self.wallet_address = wallet_address
         self.private_key = private_key
         self.execution_mode = execution_mode
         self.dex_exchange = dex_exchange
 
         base_url = 'https://api.1inch.exchange/'
         version = "v5.0"
         url = f"{base_url}/{version}/{chain_id}"
 
     @staticmethod
     def _get(url, params=None, headers=None):
         headers = { "User-Agent": "Mozilla/5.0" }
         response = requests.get(url,params =params,headers=headers)
         return response.json()
+
+    async def get_contract_address(self, symbol):
+        try:
+            alltokenlist=os.getenv("TOKENLIST", "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json") #https://raw.githubusercontent.com/viaprotocol/tokenlists/main/all_tokens/all.json
+            token_list = await self._get(alltokenlist)
+            print(token_list)
+            token_search = token_list['tokens']
+            for keyval in token_search:
+                if (keyval['symbol'] == symbol and keyval['chainId'] == int(chain_id)):
+                    print(keyval['address'])
+                    return keyval['address']
+        except Exception:
+            return
+
+    async def get_quote(self, token):
+            asset_in_address = await self.get_contract_address(token)
+            print(asset_in_address)
+            asset_out_address = await self.get_contract_address('usdc')
+            print(asset_out_address)
+            try:
+                asset_out_amount=1000000000000
+                quote_url = f"{url}/quote?fromTokenAddress={asset_in_address}&toTokenAddress={asset_out_address}&amount={asset_out_amount}"
+                print(quote_url)
+                quote = await self._get(quote_url)
+                print(quote['toTokenAmount'])
+                return quote['toTokenAmount']
+            except Exception:
+                return
+
+    def get_abi():
+        return
+
+
+    # def get_approve(self, asset_out_address: str, amount=None, decimal=None):
+    #     approval_check_URL = f"{url}/approve/allowance?tokenAddress={asset_out_address}&walletAddress={self.wallet_address}"
+    #     approval_response = await self._get(approval_check_URL)
+    #     approval_check = approval_response['allowance']
+    #     if (approval_check==0):
+    #         approval_URL = f"{url}/approve/transaction?tokenAddress={asset_out_address}"
+    #         approval_response = await self._get(approval_URL)
+
     # def swap(self, 
     #         from_token_symbol: str, 
     #         to_token_symbol: str,
     #         amount: float, 
     #         slippage=None, 
     #         decimal=None, 
     #         send_address=None
     #         ):
-    #     #await #approve_asset_router(asset_out_address,asset_out_contract)
+    #     #await self.approve_asset_router(asset_out_address,asset_out_contract)
     #     swap_url = f"{url}/swap?fromTokenAddress={asset_out_address}&toTokenAddress={asset_in_address}&amount={transaction_amount}&fromAddress={walletaddress}&slippage={slippage}"
-        #swap_TX = await retrieve_url_json(swap_url)
-        #tx_token= await sign_transaction_dex(swap_TX)
-        #return tx_token
-    # def get_approve(self, from_token_symbol: str, amount=None, decimal=None):
-    #     return
-        # approval_check_URL = f"{dex_1inch_api}/{chain_id}/approve/allowance?tokenAddress={asset_out_address}&walletAddress={walletaddress}"
-        # approval_response = await retrieve_url_json(approval_check_URL)
-        # approval_check = approval_response['allowance']
-        # if (approval_check==0):
-        #     approval_URL = f"{dex_1inch_api}/{chain_id}/approve/transaction?tokenAddress={asset_out_address}"
-        #     approval_response = await retrieve_url_json(approval_URL)
+    #     swap_TX = await retrieve_url_json(swap_url)
+    #     tx_token= await sign_transaction_dex(swap_TX)
+    #     return tx_token
+
     #def get_sign()
         # try:
         #     if dex_version in ['uni_v2']:
         #         tx_params = {
         #         'from': walletaddress,
         #         'gas': int(gasLimit),
         #         'gasPrice': ex.to_wei(gasPrice,'gwei'),
@@ -99,41 +133,14 @@
         #     raw_tx = signed.rawTransaction
         #     return ex.eth.send_raw_transaction(raw_tx)
         # except Exception as e:
         #     logger.debug(msg=f"sign_transaction_dex contract {tx} error {e}")
         #     await handle_exception(e)
         #     return
 
-    async def get_contract_address(self, symbol):
-        try:
-            alltokenlist=os.getenv("TOKENLIST", "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json") #https://raw.githubusercontent.com/viaprotocol/tokenlists/main/all_tokens/all.json
-            token_list = await self._get(alltokenlist)
-            token_search = token_list['tokens']
-            for keyval in token_search:
-                if (keyval['symbol'] == symbol and keyval['chainId'] == int(chain_id)):
-                    return keyval['address']
-        except Exception:
-            return
-
-    async def get_quote(self, token):
-            asset_in_address = await self.get_contract_address(token)
-            asset_out_address = await self.get_contract_address('usdc')
-            try:
-                asset_out_amount=1000000000000
-                quote_url = f"{url}/quote?fromTokenAddress={asset_in_address}&toTokenAddress={asset_out_address}&amount={asset_out_amount}"
-                quote = self._get(quote_url)
-                return quote['toTokenAmount']
-            except Exception:
-                return
-
-    def get_abi():
-        return
-
-
-
 
 # class DexLimitSwap:
     # dex_1inch_limit_api = "https://limit-orders.1inch.io/v3.0"
     # dex_0x_api = "https://api.0x.org/orderbook/v1"
 
 if __name__ == '__main__':
     pass
```

### Comparing `swapportunity-0.0.8/swapportunity.egg-info/PKG-INFO` & `swapportunity-0.0.9/swapportunity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swapportunity
-Version: 0.0.8
+Version: 0.0.9
 Summary: A defi swap helper package
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/swapportunity
 Project-URL: Bug Tracker, https://github.com/mraniki/swapportunity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

