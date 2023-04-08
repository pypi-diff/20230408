# Comparing `tmp/dxsp-0.0.1.tar.gz` & `tmp/dxsp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-0.0.1.tar", last modified: Sat Apr  8 21:11:14 2023, max compression
+gzip compressed data, was "dxsp-0.0.2.tar", last modified: Sat Apr  8 21:17:02 2023, max compression
```

## Comparing `dxsp-0.0.1.tar` & `dxsp-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:11:14.278715 dxsp-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 21:11:02.000000 dxsp-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-08 21:11:14.278715 dxsp-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-08 21:11:02.000000 dxsp-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:11:14.278715 dxsp-0.0.1/dxsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-08 21:11:14.000000 dxsp-0.0.1/dxsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-08 21:11:14.000000 dxsp-0.0.1/dxsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:11:14.000000 dxsp-0.0.1/dxsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 21:11:14.000000 dxsp-0.0.1/dxsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-08 21:11:02.000000 dxsp-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:11:14.278715 dxsp-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:11:14.278715 dxsp-0.0.1/swapportunity/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-08 21:11:02.000000 dxsp-0.0.1/swapportunity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-08 21:11:02.000000 dxsp-0.0.1/swapportunity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:17:02.570829 dxsp-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 21:16:49.000000 dxsp-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-08 21:17:02.570829 dxsp-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-08 21:16:49.000000 dxsp-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:17:02.566829 dxsp-0.0.2/dxsp/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 21:16:49.000000 dxsp-0.0.2/dxsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-08 21:16:49.000000 dxsp-0.0.2/dxsp/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:17:02.570829 dxsp-0.0.2/dxsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-08 21:17:02.000000 dxsp-0.0.2/dxsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-08 21:17:02.000000 dxsp-0.0.2/dxsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:17:02.000000 dxsp-0.0.2/dxsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 21:17:02.000000 dxsp-0.0.2/dxsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-08 21:16:49.000000 dxsp-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:17:02.570829 dxsp-0.0.2/setup.cfg
```

### Comparing `dxsp-0.0.1/LICENSE` & `dxsp-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-0.0.1/PKG-INFO` & `dxsp-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.1
-Summary: A defi swap helper package DeX SwaP
+Version: 0.0.2
+Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # swapportunity
-DXSP (DeX SwaP), A defi swap helper package . 
+DXSP (DeX SwaP), A defi swap helper package. 
 Easy peasy Swap.
 
-![Pypi](https://img.shields.io/pypi/dm/swaportunity)
+![Pypi](https://img.shields.io/pypi/dm/dxsp)
 
 # Install
-`pip install swapportunity`
+`pip install dxsp`
 
 2 swap execution mode are supported:
- - Single SWAP via 1inch API v5 and Uniswap version 2 router
+ - Single SWAP via 1inch API v5 and Uniswap version 2 router DEX type
  - Limit SWAP via 1inch API v3
 
+
 # Example
 
 [example](examples/example.py)
-```
+```diff
 import os
 from dotenv import load_dotenv
 import asyncio
 from web3 import Web3
 import many_abis as ma
 
 #YOUR VARIABLES
@@ -56,19 +57,19 @@
 block_explorer_api = os.getenv("BLOCK_EXPLORER_API", "1X23Q4ACZ5T3KXG67WIAH7X8C510F1972TM")
 
 #DEX CONNECTIVITY
 w3 = Web3(Web3.HTTPProvider(network_provider_url))
 
 
 
-from dxsp import DexSwap
++ from dxsp import DexSwap
 
 async def main():
 	#SWAP HELPER
-	dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
+	+ dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
 
 
 	#get Contract Address
 	bitcoinaddress = await dex.get_contract_address('wBTC')
 	print("bitcoinaddress ", bitcoinaddress)
 
 	#getABI
@@ -81,15 +82,15 @@
 
 	#INPUT for a NORMAL SWAP
 	# transaction_amount_out = 10
 	# asset_out_symbol = "USDT"
 	# asset_in_symbol = "ETH"
 
 	#SWAP EXECUTION
-	# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
+	+# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
 	# print("transaction ", transaction)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `dxsp-0.0.1/README.md` & `dxsp-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # swapportunity
-DXSP (DeX SwaP), A defi swap helper package . 
+DXSP (DeX SwaP), A defi swap helper package. 
 Easy peasy Swap.
 
-![Pypi](https://img.shields.io/pypi/dm/swaportunity)
+![Pypi](https://img.shields.io/pypi/dm/dxsp)
 
 # Install
-`pip install swapportunity`
+`pip install dxsp`
 
 2 swap execution mode are supported:
- - Single SWAP via 1inch API v5 and Uniswap version 2 router
+ - Single SWAP via 1inch API v5 and Uniswap version 2 router DEX type
  - Limit SWAP via 1inch API v3
 
+
 # Example
 
 [example](examples/example.py)
-```
+```diff
 import os
 from dotenv import load_dotenv
 import asyncio
 from web3 import Web3
 import many_abis as ma
 
 #YOUR VARIABLES
@@ -42,19 +43,19 @@
 block_explorer_api = os.getenv("BLOCK_EXPLORER_API", "1X23Q4ACZ5T3KXG67WIAH7X8C510F1972TM")
 
 #DEX CONNECTIVITY
 w3 = Web3(Web3.HTTPProvider(network_provider_url))
 
 
 
-from dxsp import DexSwap
++ from dxsp import DexSwap
 
 async def main():
 	#SWAP HELPER
-	dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
+	+ dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
 
 
 	#get Contract Address
 	bitcoinaddress = await dex.get_contract_address('wBTC')
 	print("bitcoinaddress ", bitcoinaddress)
 
 	#getABI
@@ -67,15 +68,15 @@
 
 	#INPUT for a NORMAL SWAP
 	# transaction_amount_out = 10
 	# asset_out_symbol = "USDT"
 	# asset_in_symbol = "ETH"
 
 	#SWAP EXECUTION
-	# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
+	+# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
 	# print("transaction ", transaction)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `dxsp-0.0.1/dxsp.egg-info/PKG-INFO` & `dxsp-0.0.2/dxsp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 0.0.1
-Summary: A defi swap helper package DeX SwaP
+Version: 0.0.2
+Summary: DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap.
 Author: MrAniki
 Project-URL: Homepage, https://github.com/mraniki/dxsp
 Project-URL: Bug Tracker, https://github.com/mraniki/dxsp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # swapportunity
-DXSP (DeX SwaP), A defi swap helper package . 
+DXSP (DeX SwaP), A defi swap helper package. 
 Easy peasy Swap.
 
-![Pypi](https://img.shields.io/pypi/dm/swaportunity)
+![Pypi](https://img.shields.io/pypi/dm/dxsp)
 
 # Install
-`pip install swapportunity`
+`pip install dxsp`
 
 2 swap execution mode are supported:
- - Single SWAP via 1inch API v5 and Uniswap version 2 router
+ - Single SWAP via 1inch API v5 and Uniswap version 2 router DEX type
  - Limit SWAP via 1inch API v3
 
+
 # Example
 
 [example](examples/example.py)
-```
+```diff
 import os
 from dotenv import load_dotenv
 import asyncio
 from web3 import Web3
 import many_abis as ma
 
 #YOUR VARIABLES
@@ -56,19 +57,19 @@
 block_explorer_api = os.getenv("BLOCK_EXPLORER_API", "1X23Q4ACZ5T3KXG67WIAH7X8C510F1972TM")
 
 #DEX CONNECTIVITY
 w3 = Web3(Web3.HTTPProvider(network_provider_url))
 
 
 
-from dxsp import DexSwap
++ from dxsp import DexSwap
 
 async def main():
 	#SWAP HELPER
-	dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
+	+ dex = DexSwap(w3,chain_id,wallet_address,private_key,execution_mode,dex_exchange,block_explorer_api)
 
 
 	#get Contract Address
 	bitcoinaddress = await dex.get_contract_address('wBTC')
 	print("bitcoinaddress ", bitcoinaddress)
 
 	#getABI
@@ -81,15 +82,15 @@
 
 	#INPUT for a NORMAL SWAP
 	# transaction_amount_out = 10
 	# asset_out_symbol = "USDT"
 	# asset_in_symbol = "ETH"
 
 	#SWAP EXECUTION
-	# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
+	+# transaction = dex.get_swap(transaction_amount_out,asset_out_symbol,asset_in_symbol)
 	# print("transaction ", transaction)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
```

### Comparing `dxsp-0.0.1/pyproject.toml` & `dxsp-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dxsp"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="MrAniki" },
 ]
-description = "A defi swap helper package DeX SwaP"
+description = "DXSP (DeX SwaP), A defi swap helper package. Easy peasy Swap."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `dxsp-0.0.1/swapportunity/main.py` & `dxsp-0.0.2/dxsp/main.py`

 * *Files identical despite different names*

