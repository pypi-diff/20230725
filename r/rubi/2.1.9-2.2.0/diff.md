# Comparing `tmp/rubi-2.1.9.tar.gz` & `tmp/rubi-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.1.9.tar", max compression
+gzip compressed data, was "rubi-2.2.0.tar", max compression
```

## Comparing `rubi-2.1.9.tar` & `rubi-2.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0    11357 2023-07-24 16:30:23.476596 rubi-2.1.9/LICENSE
--rw-r--r--   0        0        0     2757 2023-07-24 16:30:23.476596 rubi-2.1.9/README.md
--rw-r--r--   0        0        0     6735 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      833 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/arbitrum_one/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/arbitrum_one/abis/router.json
--rw-r--r--   0        0        0      840 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/arbitrum_one/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      858 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-24 16:30:23.476596 rubi-2.1.9/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      760 2023-07-24 16:30:23.480596 rubi-2.1.9/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-07-24 16:30:23.480596 rubi-2.1.9/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-07-24 16:30:23.480596 rubi-2.1.9/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      832 2023-07-24 16:30:23.480596 rubi-2.1.9/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0     1746 2023-07-24 16:31:00.617204 rubi-2.1.9/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/__init__.py
--rw-r--r--   0        0        0    29209 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/client.py
--rw-r--r--   0        0        0      163 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    65755 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/contracts/aid.py
--rw-r--r--   0        0        0    12261 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0       74 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/contracts/contract_types/__init__.py
--rw-r--r--   0        0        0    15898 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/contracts/contract_types/events.py
--rw-r--r--   0        0        0     2805 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/contracts/contract_types/transaction_reciept.py
--rw-r--r--   0        0        0    18565 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24880 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/contracts/market.py
--rw-r--r--   0        0        0    14915 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/contracts/router.py
--rw-r--r--   0        0        0       77 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/data/README.md
--rw-r--r--   0        0        0       31 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/data/__init__.py
--rw-r--r--   0        0        0    10670 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/data/market.py
--rw-r--r--   0        0        0       72 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/network/__init__.py
--rw-r--r--   0        0        0     8475 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/network/network.py
--rw-r--r--   0        0        0       94 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/rubicon_types/__init__.py
--rw-r--r--   0        0        0    16249 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/rubicon_types/order.py
--rw-r--r--   0        0        0    11554 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/rubicon_types/order_query.py
--rw-r--r--   0        0        0     6323 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/rubicon_types/orderbook.py
--rw-r--r--   0        0        0     2779 2023-07-24 16:30:23.480596 rubi-2.1.9/rubi/rubicon_types/pair.py
--rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 19:28:26.901551 rubi-2.2.0/LICENSE
+-rw-r--r--   0        0        0     2757 2023-07-25 19:28:26.901551 rubi-2.2.0/README.md
+-rw-r--r--   0        0        0     6735 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      833 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/arbitrum_one/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/arbitrum_one/abis/router.json
+-rw-r--r--   0        0        0      840 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/arbitrum_one/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      858 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      760 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-07-25 19:28:26.901551 rubi-2.2.0/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-07-25 19:28:26.905551 rubi-2.2.0/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      832 2023-07-25 19:28:26.905551 rubi-2.2.0/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0     1746 2023-07-25 19:28:52.861166 rubi-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/__init__.py
+-rw-r--r--   0        0        0    30904 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/client.py
+-rw-r--r--   0        0        0      163 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    65755 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    12337 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0       74 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/contract_types/__init__.py
+-rw-r--r--   0        0        0    15898 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/contract_types/events.py
+-rw-r--r--   0        0        0     2805 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/contract_types/transaction_reciept.py
+-rw-r--r--   0        0        0    18565 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24880 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14915 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/contracts/router.py
+-rw-r--r--   0        0        0       77 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/data/README.md
+-rw-r--r--   0        0        0       31 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/data/__init__.py
+-rw-r--r--   0        0        0    17073 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/data/market.py
+-rw-r--r--   0        0        0       72 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/network/__init__.py
+-rw-r--r--   0        0        0     8475 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/network/network.py
+-rw-r--r--   0        0        0      121 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/__init__.py
+-rw-r--r--   0        0        0    16249 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/order.py
+-rw-r--r--   0        0        0    11701 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/order_query.py
+-rw-r--r--   0        0        0     6323 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/orderbook.py
+-rw-r--r--   0        0        0     2779 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/pair.py
+-rw-r--r--   0        0        0    11414 2023-07-25 19:28:26.905551 rubi-2.2.0/rubi/rubicon_types/trade_query.py
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 rubi-2.2.0/PKG-INFO
```

### Comparing `rubi-2.1.9/LICENSE` & `rubi-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/README.md` & `rubi-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/ERC20.json` & `rubi-2.2.0/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/README.md` & `rubi-2.2.0/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/abitrum_goerli/abis/market.json` & `rubi-2.2.0/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/abitrum_goerli/abis/router.json` & `rubi-2.2.0/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/abitrum_goerli/network.yaml` & `rubi-2.2.0/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/arbitrum_one/abis/market.json` & `rubi-2.2.0/network_config/arbitrum_one/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/arbitrum_one/abis/router.json` & `rubi-2.2.0/network_config/arbitrum_one/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/arbitrum_one/network.yaml` & `rubi-2.2.0/network_config/arbitrum_one/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/optimism/abis/market.json` & `rubi-2.2.0/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/optimism/abis/router.json` & `rubi-2.2.0/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/optimism/network.yaml` & `rubi-2.2.0/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/optimism_goerli/abis/market.json` & `rubi-2.2.0/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/optimism_goerli/abis/router.json` & `rubi-2.2.0/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/optimism_goerli/network.yaml` & `rubi-2.2.0/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/polygon_mumbai/abis/market.json` & `rubi-2.2.0/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/polygon_mumbai/abis/router.json` & `rubi-2.2.0/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/network_config/polygon_mumbai/network.yaml` & `rubi-2.2.0/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/pyproject.toml` & `rubi-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.1.9"
+version = "2.2.0"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**/*"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `rubi-2.1.9/rubi/client.py` & `rubi-2.2.0/rubi/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -652,44 +652,82 @@
 
         return self.market.batch_cancel(ids=order_ids, **transaction.args())
 
     ######################################################################
     # data methods (raw data) TODO: once we have cleanly formatted data functions, we can switch to only exposing those
     ######################################################################
 
+    # TODO: i would like to remove pay_gem and buy_gem and follow the same pattern as the get_trades method but do not want to cause breaking changes
     def get_offers(
         self,
-        maker: Optional[str] = None,
-        from_address: Optional[str] = None,
+        first: int = 10000000,  # TODO: decide on a default value
+        order_by: str = "timestamp",
+        order_direction: str = "desc",
+        formatted: bool = True,
+        book_side: OrderSide = OrderSide.NEUTRAL,
+        maker: Optional[Union[ChecksumAddress, str]] = None,
+        from_address: Optional[Union[ChecksumAddress, str]] = None,
         pair_name: Optional[str] = None,
-        book_side: Optional[OrderSide] = None,
-        pay_gem: Optional[str] = None,
-        buy_gem: Optional[str] = None,
+        pay_gem: Optional[Union[ChecksumAddress, str]] = None,
+        buy_gem: Optional[Union[ChecksumAddress, str]] = None,
         open: Optional[bool] = None,
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
-        first: Optional[int] = 1000,
-        order_by: Optional[str] = "timestamp",
-        order_direction: Optional[str] = "desc",
-        formatted: Optional[bool] = True,
     ) -> pd.DataFrame:
         df = self.market_data.get_offers(
-            maker,
-            from_address,
-            pair_name,
-            book_side,
-            pay_gem,
-            buy_gem,
-            open,
-            start_time,
-            end_time,
-            first,
-            order_by,
-            order_direction,
-            formatted,
+            maker=maker,
+            from_address=from_address,
+            pair_name=pair_name,
+            book_side=book_side,
+            pay_gem=pay_gem,
+            buy_gem=buy_gem,
+            open=open,
+            start_time=start_time,
+            end_time=end_time,
+            first=first,
+            order_by=order_by,
+            order_direction=order_direction,
+            formatted=formatted,
+        )
+        return df
+
+    def get_trades(
+        self,
+        first: int = 10000000,  # TODO: decide on a default value
+        order_by: str = "timestamp",
+        order_direction: str = "desc",
+        formatted: bool = True,
+        book_side: OrderSide = OrderSide.NEUTRAL,
+        taker: Optional[Union[ChecksumAddress, str]] = None,
+        from_address: Optional[Union[ChecksumAddress, str]] = None,
+        pair_name: Optional[str] = None,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+    ) -> pd.DataFrame:
+        # handle the pair_name parameter
+        if pair_name:
+            base, quote = pair_name.split("/")
+            base_asset = ERC20.from_network(name=base, network=self.network).address
+            quote_asset = ERC20.from_network(name=quote, network=self.network).address
+        else:
+            base_asset = None
+            quote_asset = None
+
+        df = self.market_data.get_trades(
+            first=first,
+            order_by=order_by,
+            order_direction=order_direction,
+            book_side=book_side,
+            formatted=formatted,
+            taker=taker,
+            from_address=from_address,
+            take_gem=base_asset,
+            give_gem=quote_asset,
+            start_time=start_time,
+            end_time=end_time,
         )
         return df
 
     ######################################################################
     # helper methods
     ######################################################################
```

### Comparing `rubi-2.1.9/rubi/contracts/aid.py` & `rubi-2.2.0/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/rubi/contracts/base_contract.py` & `rubi-2.2.0/rubi/contracts/base_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from typing import Optional, Callable, Type, Dict, Any
 
 from eth_account.datastructures import SignedTransaction
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3._utils.filters import LogFilter  # noqa
 from web3.contract import Contract
-from web3.contract.contract import ContractFunction
+from web3.contract.contract import (
+    ContractFunction,
+)  # TODO: figure out why jupyter notebook is complaining about this
 from web3.types import ABI, Nonce
 
 from rubi.contracts.contract_types import BaseEvent, TransactionReceipt
 
 
 class BaseContract:
     """Base class representation of a contract which defines the structure of a contract and provides several helpful
```

### Comparing `rubi-2.1.9/rubi/contracts/contract_types/events.py` & `rubi-2.2.0/rubi/contracts/contract_types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/rubi/contracts/contract_types/transaction_reciept.py` & `rubi-2.2.0/rubi/contracts/contract_types/transaction_reciept.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/rubi/contracts/erc20.py` & `rubi-2.2.0/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/rubi/contracts/market.py` & `rubi-2.2.0/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/rubi/contracts/router.py` & `rubi-2.2.0/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/rubi/data/market.py` & `rubi-2.2.0/rubi/data/market.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import Optional, Dict
+from typing import Optional, Dict, Union
 
 import pandas as pd
 from eth_typing import ChecksumAddress
 from subgrounds import Subgrounds
 
 from rubi.contracts import (
     ERC20,
 )
 from rubi.network import (
     Network,
 )
 from rubi.rubicon_types import (
     OrderSide,
     OrderQuery,
+    TradeQuery,
 )
 
 
 class MarketData:
     """This class represents the RubiconV2 Subgraph, which contains data primarily related to the RubiconMarket.sol
     contract. If a Network object is not passed in instantiation then this class will only be used to query data related
      to the subgraph.
@@ -61,14 +62,15 @@
                     except:
                         raise ValueError(
                             f"Both subgraph_url: {self.subgraph_url} and fallback_url: {self.subgraph_fallback_url} failed when attempting to load. Error: {str(e)}"
                         )
 
         # Initialize the query classes
         self.offer_query = OrderQuery(self.sg, self.data, self.network, self.tokens)
+        self.trade_query = TradeQuery(self.sg, self.data, self.network, self.tokens)
 
     @classmethod
     def from_network_with_tokens(
         cls, network: Network, network_tokens: Dict[ChecksumAddress, ERC20]
     ) -> "MarketData":
         """Initialize a MarketData object using a Network object."""
         return cls(
@@ -82,31 +84,27 @@
     #####################################
     # Subgraph Query Methods            #
     #####################################
 
     # TODO: refactor using a decorator to handle the parameter validation
     def get_offers(
         self,
-        maker: Optional[str] = None,
-        from_address: Optional[str] = None,
+        first: int = 1000,
+        order_by: str = "timestamp",
+        order_direction: str = "desc",
+        formatted: bool = False,
+        book_side: OrderSide = OrderSide.NEUTRAL,
+        maker: Optional[Union[ChecksumAddress, str]] = None,
+        from_address: Optional[Union[ChecksumAddress, str]] = None,
         pair_name: Optional[str] = None,
-        book_side: Optional[OrderSide] = None,
-        pay_gem: Optional[
-            str
-        ] = None,  # TODO: maybe we should allow the user to pass in an address here?
-        buy_gem: Optional[
-            str
-        ] = None,  # TODO: maybe we should allow the user to pass in an address here?
+        pay_gem: Optional[Union[ChecksumAddress, str]] = None,
+        buy_gem: Optional[Union[ChecksumAddress, str]] = None,
         open: Optional[bool] = None,
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
-        first: Optional[int] = 1000,
-        order_by: Optional[str] = "timestamp",
-        order_direction: Optional[str] = "desc",
-        formatted: Optional[bool] = False,
     ) -> pd.DataFrame:
         """Returns a dataframe of offers placed on the market contract, with the option to pass in filters.
 
         :param maker: the address of the maker of the offer
         :type maker: str
         :param from_address: the address that originated the transaction that created the offer
         :type from_address: str
@@ -141,15 +139,17 @@
         # handle the pair_name parameter
         if pair_name:
             base, quote = pair_name.split("/")
             base_asset = ERC20.from_network(name=base, network=self.network)
             quote_asset = ERC20.from_network(name=quote, network=self.network)
 
         # handle the book_side parameter
-        if book_side and pair_name:
+        if (
+            book_side and pair_name
+        ):  # TODO: we need to handle the case where neither of these are passed
             match book_side:
                 case OrderSide.BUY:
                     buy_query = self.offer_query.offers_query(
                         order_by,
                         order_direction,
                         first,
                         maker,
@@ -243,9 +243,152 @@
                 buy_gem=buy_gem,
                 open=open,
                 start_time=start_time,
                 end_time=end_time,
             )
             fields = self.offer_query.offers_fields(query)
             df = self.offer_query.query_offers(fields)
+            df["side"] = "N/A"
 
             return df
+
+    # TODO: add an optional filter by maker when
+    def get_trades(
+        self,
+        first: int = 1000,  # TODO: maybe this should be a large number by default?
+        order_by: str = "timestamp",
+        order_direction: str = "desc",
+        formatted: bool = False,
+        book_side: OrderSide = OrderSide.NEUTRAL,
+        taker: Optional[Union[ChecksumAddress, str]] = None,
+        from_address: Optional[Union[ChecksumAddress, str]] = None,
+        take_gem: Optional[Union[ChecksumAddress, str]] = None,
+        give_gem: Optional[Union[ChecksumAddress, str]] = None,
+        start_time: Optional[int] = None,
+        end_time: Optional[int] = None,
+    ) -> pd.DataFrame:
+        """Returns a dataframe of trades that have occurred on the market contract, with the option to pass in filters.
+
+        :param taker: the address of the taker of the trade
+        :type taker: str
+        :param from_address: the address that originated the transaction that created the trade
+        :type from_address: str
+        :param book_side: the side of the order book that the trade occurred on (defaults to neutral, options: buy, sell, neutral)
+        :type book_side: OrderSide
+        :param take_gem: the address of the token that the taker received
+        :type take_gem: str
+        :param give_gem: the address of the token that the taker gave
+        :type give_gem: str
+        :param start_time: the timestamp of the earliest trade to return
+        :type start_time: int
+        :param end_time: the timestamp of the latest trade to return
+        :type end_time: int
+        :param first: the number of trades to return
+        :type first: int
+        :param order_by: the field to order the trades by (default: timestamp, options: timestamp) TODO: expand this list
+        :type order_by: str
+        :param order_direction: the direction to order the trades by (default: desc, options: asc, desc)
+        :type order_direction: str
+        :param formatted: whether or not to return the formatted fields (default: False, requires a network object to be passed)
+        :type formatted: bool
+        :return: a dataframe of trades that have occurred on the market contract
+        :rtype: pd.DataFrame
+        """
+
+        # if we want formatted fields, make sure we have a network object
+        if formatted and not self.network:
+            raise ValueError(
+                "Cannot return formatted fields without a network object initialized on the class."
+            )
+
+        if take_gem is None and give_gem is None:
+            all_trades_query = self.trade_query.trades_query(
+                order_by,
+                order_direction,
+                first,
+                taker,
+                from_address,
+                take_gem=take_gem,
+                give_gem=give_gem,
+                start_time=start_time,
+                end_time=end_time,
+            )
+            all_trades_fields = self.trade_query.trades_fields(
+                all_trades_query, formatted
+            )
+            all_trades_df = self.trade_query.query_trades(all_trades_fields, formatted)
+            all_trades_df["side"] = "N/A"
+
+            return all_trades_df
+
+        else:
+            match book_side:
+                case OrderSide.BUY:
+                    buy_query = self.trade_query.trades_query(
+                        order_by,
+                        order_direction,
+                        first,
+                        taker,
+                        from_address,
+                        take_gem=take_gem,
+                        give_gem=give_gem,
+                        start_time=start_time,
+                        end_time=end_time,
+                    )
+                    buy_fields = self.trade_query.trades_fields(buy_query, formatted)
+                    buy_df = self.trade_query.query_trades(buy_fields, formatted)
+                    buy_df["side"] = "buy"
+
+                    return buy_df
+
+                case OrderSide.SELL:
+                    sell_query = self.trade_query.trades_query(
+                        order_by,
+                        order_direction,
+                        first,
+                        taker,
+                        from_address,
+                        take_gem=give_gem,
+                        give_gem=take_gem,
+                        start_time=start_time,
+                        end_time=end_time,
+                    )
+                    sell_fields = self.trade_query.trades_fields(sell_query, formatted)
+                    sell_df = self.trade_query.query_trades(sell_fields, formatted)
+                    sell_df["side"] = "sell"
+
+                    return sell_df
+
+                case OrderSide.NEUTRAL:
+                    buy_query = self.trade_query.trades_query(
+                        order_by,
+                        order_direction,
+                        first,  # TODO: decide if we only want to pass half the values here
+                        taker,
+                        from_address,
+                        take_gem=take_gem,
+                        give_gem=give_gem,
+                        start_time=start_time,
+                        end_time=end_time,
+                    )
+                    buy_fields = self.trade_query.trades_fields(buy_query, formatted)
+                    buy_df = self.trade_query.query_trades(buy_fields, formatted)
+                    buy_df["side"] = "buy"
+
+                    sell_query = self.trade_query.trades_query(
+                        order_by,
+                        order_direction,
+                        first,
+                        taker,
+                        from_address,
+                        take_gem=give_gem,
+                        give_gem=take_gem,
+                        start_time=start_time,
+                        end_time=end_time,
+                    )
+                    sell_fields = self.trade_query.trades_fields(sell_query, formatted)
+                    sell_df = self.trade_query.query_trades(sell_fields, formatted)
+                    sell_df["side"] = "sell"
+
+                    return pd.concat([buy_df, sell_df]).reset_index(
+                        drop=True
+                    )  # TODO: decide what we want to do here, maybe we just return both dataframes?
```

### Comparing `rubi-2.1.9/rubi/network/network.py` & `rubi-2.2.0/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/rubi/rubicon_types/order.py` & `rubi-2.2.0/rubi/rubicon_types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/rubi/rubicon_types/order_query.py` & `rubi-2.2.0/rubi/rubicon_types/order_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import List, Optional, Dict, Any
+from typing import List, Optional, Dict, Any, Union
 
 import pandas as pd
 from eth_typing import ChecksumAddress
 from subgrounds import Subgrounds
 from subgrounds.pagination import ShallowStrategy
 from subgrounds.subgraph import SyntheticField
 
@@ -116,18 +116,18 @@
         return Offer
 
     def offers_query(
         self,
         order_by: str,
         order_direction: str,
         first: int,
-        maker: Optional[str] = None,
-        from_address: Optional[str] = None,
-        pay_gem: Optional[str] = None,
-        buy_gem: Optional[str] = None,
+        maker: Optional[Union[ChecksumAddress, str]] = None,
+        from_address: Optional[Union[ChecksumAddress, str]] = None,
+        pay_gem: Optional[Union[ChecksumAddress, str]] = None,
+        buy_gem: Optional[Union[ChecksumAddress, str]] = None,
         open: Optional[bool] = None,
         start_time: Optional[int] = None,
         end_time: Optional[int] = None,
         # TODO: there is definitely a clear way to pass these parameters in a more concise way, prolly **kargs
     ):  # TODO: return a typed object (see subgrounds documentation for more info)
         # determine that the parameters are valid
         error_messages = []
@@ -160,18 +160,20 @@
 
         # raise an error if there are any
         if error_messages:
             raise ValueError("\n".join(error_messages))
 
         # build the list of where conditions
         where = [
-            self.offer.maker == maker.lower() if maker else None,
-            self.offer.from_address == from_address.lower() if from_address else None,
-            self.offer.pay_gem == pay_gem.lower() if pay_gem else None,
-            self.offer.buy_gem == buy_gem.lower() if buy_gem else None,
+            self.offer.maker == str(maker).lower() if maker else None,
+            self.offer.from_address == str(from_address).lower()
+            if from_address
+            else None,
+            self.offer.pay_gem == str(pay_gem).lower() if pay_gem else None,
+            self.offer.buy_gem == str(buy_gem).lower() if buy_gem else None,
             self.offer.open == open if open is not None else None,
             self.offer.timestamp >= start_time if start_time else None,
             self.offer.timestamp <= end_time if end_time else None,
         ]
         where = [condition for condition in where if condition is not None]
 
         """Helper method to build a query for the offers subgraph entity."""
```

### Comparing `rubi-2.1.9/rubi/rubicon_types/orderbook.py` & `rubi-2.2.0/rubi/rubicon_types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/rubi/rubicon_types/pair.py` & `rubi-2.2.0/rubi/rubicon_types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.1.9/PKG-INFO` & `rubi-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.1.9
+Version: 2.2.0
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

