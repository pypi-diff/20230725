# Comparing `tmp/omxpy-0.0.5.tar.gz` & `tmp/omxpy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omxpy-0.0.5.tar", max compression
+gzip compressed data, was "omxpy-0.0.7.tar", max compression
```

## Comparing `omxpy-0.0.5.tar` & `omxpy-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1073 2023-07-07 07:31:44.811240 omxpy-0.0.5/LICENSE
--rw-r--r--   0        0        0     4238 2023-07-07 07:31:44.811240 omxpy-0.0.5/README.md
--rw-r--r--   0        0        0       77 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/__init__.py
--rw-r--r--   0        0        0     1156 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/base_client.py
--rw-r--r--   0        0        0      468 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/__init__.py
--rw-r--r--   0        0        0    15318 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_base_token/__init__.py
--rw-r--r--   0        0        0     1274 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_olp_manager/__init__.py
--rw-r--r--   0        0        0    28821 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_orderbook/__init__.py
--rw-r--r--   0        0        0     1492 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_pair/__init__.py
--rw-r--r--   0        0        0     2690 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_price_feed/__init__.py
--rw-r--r--   0        0        0    19161 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_router/__init__.py
--rw-r--r--   0        0        0    33559 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_vault/__init__.py
--rw-r--r--   0        0        0     2612 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_vault_price_feed/__init__.py
--rw-r--r--   0        0        0    14048 2023-07-07 07:31:44.811240 omxpy-0.0.5/omxpy/contracts/omx_cw_wrapped_token/__init__.py
--rw-r--r--   0        0        0      294 2023-07-07 07:31:44.815240 omxpy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 omxpy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-25 15:59:04.449569 omxpy-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4238 2023-07-25 15:59:04.449569 omxpy-0.0.7/README.md
+-rw-r--r--   0        0        0       77 2023-07-25 15:59:04.449569 omxpy-0.0.7/omxpy/__init__.py
+-rw-r--r--   0        0        0     1156 2023-07-25 15:59:04.449569 omxpy-0.0.7/omxpy/base_client.py
+-rw-r--r--   0        0        0      415 2023-07-25 15:59:04.449569 omxpy-0.0.7/omxpy/contracts/__init__.py
+-rw-r--r--   0        0        0    15318 2023-07-25 15:59:04.449569 omxpy-0.0.7/omxpy/contracts/omx_cw_base_token/__init__.py
+-rw-r--r--   0        0        0     1274 2023-07-25 15:59:04.449569 omxpy-0.0.7/omxpy/contracts/omx_cw_olp_manager/__init__.py
+-rw-r--r--   0        0        0    28821 2023-07-25 15:59:04.449569 omxpy-0.0.7/omxpy/contracts/omx_cw_orderbook/__init__.py
+-rw-r--r--   0        0        0     1492 2023-07-25 15:59:04.449569 omxpy-0.0.7/omxpy/contracts/omx_cw_pair/__init__.py
+-rw-r--r--   0        0        0    19161 2023-07-25 15:59:04.453569 omxpy-0.0.7/omxpy/contracts/omx_cw_router/__init__.py
+-rw-r--r--   0        0        0    34465 2023-07-25 15:59:04.453569 omxpy-0.0.7/omxpy/contracts/omx_cw_vault/__init__.py
+-rw-r--r--   0        0        0     2777 2023-07-25 15:59:04.453569 omxpy-0.0.7/omxpy/contracts/omx_cw_vault_price_feed/__init__.py
+-rw-r--r--   0        0        0    14048 2023-07-25 15:59:04.453569 omxpy-0.0.7/omxpy/contracts/omx_cw_wrapped_token/__init__.py
+-rw-r--r--   0        0        0      294 2023-07-25 15:59:04.453569 omxpy-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 omxpy-0.0.7/PKG-INFO
```

### Comparing `omxpy-0.0.5/LICENSE` & `omxpy-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.5/README.md` & `omxpy-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.5/omxpy/base_client.py` & `omxpy-0.0.7/omxpy/base_client.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.5/omxpy/contracts/omx_cw_base_token/__init__.py` & `omxpy-0.0.7/omxpy/contracts/omx_cw_base_token/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.5/omxpy/contracts/omx_cw_olp_manager/__init__.py` & `omxpy-0.0.7/omxpy/contracts/omx_cw_olp_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.5/omxpy/contracts/omx_cw_orderbook/__init__.py` & `omxpy-0.0.7/omxpy/contracts/omx_cw_orderbook/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.5/omxpy/contracts/omx_cw_pair/__init__.py` & `omxpy-0.0.7/omxpy/contracts/omx_cw_pair/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.5/omxpy/contracts/omx_cw_router/__init__.py` & `omxpy-0.0.7/omxpy/contracts/omx_cw_router/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.5/omxpy/contracts/omx_cw_vault/__init__.py` & `omxpy-0.0.7/omxpy/contracts/omx_cw_vault/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,26 @@
 	delta: "Uint128"
 	has_profit: bool
 
 QueryResponse_position_fee = str
 
 QueryResponse_position_leverage = str
 
+Addr = str
+
+PositionKey__is_long = bool
+
+class PositionKey(TypedDict):
+	account: "Addr"
+	collateral_token: "Addr"
+	index_token: "Addr"
+	is_long: bool
+
+QueryResponse_positions = List["PositionKey"]
+
 QueryResponse_redemption_amount = str
 
 QueryResponse_redemption_collateral = str
 
 QueryResponse_redemption_collateral_usd = str
 
 QueryResponse_reserved_amounts = str
@@ -85,16 +97,14 @@
 
 QueryResponse_usdo_amount = str
 
 QueryResponse_utilization = str
 
 QueryResponse_validate_liquidation = str
 
-Addr = str
-
 class QueryResponse_vault_config(TypedDict):
 	usdo: "Addr"
 
 Duration__nanos = int
 
 Duration__secs = int
 
@@ -564,14 +574,31 @@
 
 class PositionQuery(TypedDict):
 	account: str
 	collateral_token: str
 	index_token: str
 	is_long: bool
 
+PositionsQuery__account = Optional[str]
+
+PositionsQuery__collateral_token = Optional[str]
+
+PositionsQuery__index_token = Optional[str]
+
+PositionsQuery__is_long = Optional[bool]
+
+PositionsQuery__valid = Optional[bool]
+
+class PositionsQuery(TypedDict):
+	account: str
+	collateral_token: str
+	index_token: str
+	is_long: bool
+	valid: bool
+
 RedemptionAmountQuery__token = str
 
 class RedemptionAmountQuery(TypedDict):
 	token: str
 	usdo_amount: "Uint128"
 
 RedemptionCollateralQuery__token = str
@@ -813,24 +840,27 @@
 
 class QueryMsg__pool_amount(TypedDict):
 	pool_amount: "PoolAmountQuery"
 
 class QueryMsg__whitelisted_token(TypedDict):
 	whitelisted_token: "WhitelistedTokenQuery"
 
+class QueryMsg__positions(TypedDict):
+	positions: "PositionsQuery"
+
 class QueryMsg__position(TypedDict):
 	position: "PositionQuery"
 
 class QueryMsg__fee_reserves(TypedDict):
 	fee_reserves: "FeeReservesQuery"
 
 class QueryMsg__validate_liquidation(TypedDict):
 	validate_liquidation: "ValidateLiquidationQuery"
 
-QueryMsg = Union["QueryMsg__vault_state", "QueryMsg__vault_config", "QueryMsg__utilization", "QueryMsg__cumulative_funding_rates", "QueryMsg__position_leverage", "QueryMsg__token_to_usd_min", "QueryMsg__global_short_average_prices", "QueryMsg__global_short_sizes", "QueryMsg__position_delta", "QueryMsg__reserved_amounts", "QueryMsg__guaranteed_usd", "QueryMsg__usdo_amount", "QueryMsg__entry_funding_rate", "QueryMsg__next_global_short_average_price", "QueryMsg__next_funding_rate", "QueryMsg__funding_fee", "QueryMsg__min_price", "QueryMsg__max_price", "QueryMsg__redemption_amount", "QueryMsg__target_usdo_amount", "QueryMsg__adjust_for_decimals", "QueryMsg__is_router_approved", "QueryMsg__get_delta", "QueryMsg__redemption_collateral", "QueryMsg__redemption_collateral_usd", "QueryMsg__position_fee", "QueryMsg__max_global_short_price", "QueryMsg__next_average_price", "QueryMsg__is_manager", "QueryMsg__pool_amount", "QueryMsg__whitelisted_token", "QueryMsg__position", "QueryMsg__fee_reserves", "QueryMsg__validate_liquidation"]
+QueryMsg = Union["QueryMsg__vault_state", "QueryMsg__vault_config", "QueryMsg__utilization", "QueryMsg__cumulative_funding_rates", "QueryMsg__position_leverage", "QueryMsg__token_to_usd_min", "QueryMsg__global_short_average_prices", "QueryMsg__global_short_sizes", "QueryMsg__position_delta", "QueryMsg__reserved_amounts", "QueryMsg__guaranteed_usd", "QueryMsg__usdo_amount", "QueryMsg__entry_funding_rate", "QueryMsg__next_global_short_average_price", "QueryMsg__next_funding_rate", "QueryMsg__funding_fee", "QueryMsg__min_price", "QueryMsg__max_price", "QueryMsg__redemption_amount", "QueryMsg__target_usdo_amount", "QueryMsg__adjust_for_decimals", "QueryMsg__is_router_approved", "QueryMsg__get_delta", "QueryMsg__redemption_collateral", "QueryMsg__redemption_collateral_usd", "QueryMsg__position_fee", "QueryMsg__max_global_short_price", "QueryMsg__next_average_price", "QueryMsg__is_manager", "QueryMsg__pool_amount", "QueryMsg__whitelisted_token", "QueryMsg__positions", "QueryMsg__position", "QueryMsg__fee_reserves", "QueryMsg__validate_liquidation"]
 
 
 
 class OmxCwVault(BaseOmxClient):
 	def clone(self) -> "OmxCwVault":
 		instance = self.__class__.__new__(self.__class__)
 		instance.tx = self.tx
@@ -1028,14 +1058,17 @@
 
 	def pool_amount(self, token: str) -> "QueryResponse_pool_amount":
 		return self.query({"pool_amount": {"token": token}})
 
 	def whitelisted_token(self, token: str) -> "QueryResponse_whitelisted_token":
 		return self.query({"whitelisted_token": {"token": token}})
 
+	def positions(self, account: str, collateral_token: str, index_token: str, is_long: bool, valid: bool) -> "QueryResponse_positions":
+		return self.query({"positions": {"account": account, "collateral_token": collateral_token, "index_token": index_token, "is_long": is_long, "valid": valid}})
+
 	def position(self, account: str, collateral_token: str, index_token: str, is_long: bool) -> "QueryResponse_position":
 		return self.query({"position": {"account": account, "collateral_token": collateral_token, "index_token": index_token, "is_long": is_long}})
 
 	def fee_reserves(self, token: str) -> "QueryResponse_fee_reserves":
 		return self.query({"fee_reserves": {"token": token}})
 
 	def validate_liquidation(self, account: str, collateral_token: str, index_token: str, is_long: bool, should_raise: bool) -> "QueryResponse_validate_liquidation":
```

### Comparing `omxpy-0.0.5/omxpy/contracts/omx_cw_vault_price_feed/__init__.py` & `omxpy-0.0.7/omxpy/contracts/omx_cw_vault_price_feed/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 from cosmpy.aerial.tx_helpers import SubmittedTx
 from cosmpy.aerial.wallet import Wallet
 from typing import TypedDict, Union
 
 
 QueryResponse_price = str
 
-Addr = str
+Identifier = str
+
+SetAdminExec__admin = str
 
 class SetAdminExec(TypedDict):
-	admin: "Addr"
+	admin: str
 
-SetPriceSampleSpaceExec__value = int
+SetMaxPriceAgeExec__value = int
 
-class SetPriceSampleSpaceExec(TypedDict):
+class SetMaxPriceAgeExec(TypedDict):
 	value: int
 
-SetTokenConfigExec__is_strict_stable = bool
+SetPriceFeedExec__address = str
 
-SetTokenConfigExec__price_decimals = int
+class SetPriceFeedExec(TypedDict):
+	address: str
 
-SetTokenConfigExec__price_feed = str
+SetTokenConfigExec__is_strict_stable = bool
 
 SetTokenConfigExec__token = str
 
 class SetTokenConfigExec(TypedDict):
 	is_strict_stable: bool
-	price_decimals: int
-	price_feed: str
+	price_feed: "Identifier"
 	token: str
 
 PriceQuery__include_amm_price = bool
 
 PriceQuery__maximize = bool
 
 PriceQuery__token = str
@@ -43,18 +45,21 @@
 
 class ExecuteMsg__set_admin(TypedDict):
 	set_admin: "SetAdminExec"
 
 class ExecuteMsg__set_token_config(TypedDict):
 	set_token_config: "SetTokenConfigExec"
 
-class ExecuteMsg__set_price_sample_space(TypedDict):
-	set_price_sample_space: "SetPriceSampleSpaceExec"
+class ExecuteMsg__set_price_feed(TypedDict):
+	set_price_feed: "SetPriceFeedExec"
 
-ExecuteMsg = Union["ExecuteMsg__set_admin", "ExecuteMsg__set_token_config", "ExecuteMsg__set_price_sample_space"]
+class ExecuteMsg__set_max_price_age(TypedDict):
+	set_max_price_age: "SetMaxPriceAgeExec"
+
+ExecuteMsg = Union["ExecuteMsg__set_admin", "ExecuteMsg__set_token_config", "ExecuteMsg__set_price_feed", "ExecuteMsg__set_max_price_age"]
 
 class QueryMsg__price(TypedDict):
 	price: "PriceQuery"
 
 QueryMsg = "QueryMsg__price"
 
 
@@ -80,18 +85,21 @@
 		return o
 
 	def with_wallet(self, wallet: Wallet) -> "OmxCwVaultPriceFeed":
 		o = self.clone()
 		o.wallet = wallet
 		return o
 
-	def set_admin(self, admin: "Addr") -> SubmittedTx:
+	def set_admin(self, admin: str) -> SubmittedTx:
 		return self.execute({"set_admin": {"admin": admin}})
 
-	def set_token_config(self, is_strict_stable: bool, price_decimals: int, price_feed: str, token: str) -> SubmittedTx:
-		return self.execute({"set_token_config": {"is_strict_stable": is_strict_stable, "price_decimals": price_decimals, "price_feed": price_feed, "token": token}})
+	def set_token_config(self, is_strict_stable: bool, price_feed: "Identifier", token: str) -> SubmittedTx:
+		return self.execute({"set_token_config": {"is_strict_stable": is_strict_stable, "price_feed": price_feed, "token": token}})
+
+	def set_price_feed(self, address: str) -> SubmittedTx:
+		return self.execute({"set_price_feed": {"address": address}})
 
-	def set_price_sample_space(self, value: int) -> SubmittedTx:
-		return self.execute({"set_price_sample_space": {"value": value}})
+	def set_max_price_age(self, value: int) -> SubmittedTx:
+		return self.execute({"set_max_price_age": {"value": value}})
 
 	def price(self, include_amm_price: bool, maximize: bool, token: str) -> "QueryResponse_price":
 		return self.query({"price": {"include_amm_price": include_amm_price, "maximize": maximize, "token": token}})
```

### Comparing `omxpy-0.0.5/omxpy/contracts/omx_cw_wrapped_token/__init__.py` & `omxpy-0.0.7/omxpy/contracts/omx_cw_wrapped_token/__init__.py`

 * *Files identical despite different names*

### Comparing `omxpy-0.0.5/PKG-INFO` & `omxpy-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omxpy
-Version: 0.0.5
+Version: 0.0.7
 Summary: 
 License: MIT
 Author: Omx
 Author-email: omxlabs@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

