# Comparing `tmp/hubble_exchange-0.3.0.tar.gz` & `tmp/hubble_exchange-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubble_exchange-0.3.0.tar", last modified: Mon Jul 17 11:43:19 2023, max compression
+gzip compressed data, was "hubble_exchange-0.4.0.tar", last modified: Tue Jul 25 07:26:08 2023, max compression
```

## Comparing `hubble_exchange-0.3.0.tar` & `hubble_exchange-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-17 11:43:19.120891 hubble_exchange-0.3.0/
--rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.3.0/LICENSE
--rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.3.0/MANIFEST.in
--rw-r--r--   0 shubham    (501) staff       (20)     5648 2023-07-17 11:43:19.120759 hubble_exchange-0.3.0/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     3991 2023-07-17 10:52:10.000000 hubble_exchange-0.3.0/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-17 11:43:19.119423 hubble_exchange-0.3.0/hubble_exchange/
--rw-r--r--   0 shubham    (501) staff       (20)      351 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     6220 2023-07-17 10:10:11.000000 hubble_exchange-0.3.0/hubble_exchange/client.py
--rw-r--r--   0 shubham    (501) staff       (20)      202 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/constants.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-17 11:43:19.120292 hubble_exchange-0.3.0/hubble_exchange/contract_abis/
--rw-r--r--   0 shubham    (501) staff       (20)    23029 2023-06-28 04:43:57.000000 hubble_exchange-0.3.0/hubble_exchange/contract_abis/OrderBook.json
--rw-r--r--   0 shubham    (501) staff       (20)     1200 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/eip712.py
--rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/errors.py
--rw-r--r--   0 shubham    (501) staff       (20)     5038 2023-07-17 09:02:27.000000 hubble_exchange-0.3.0/hubble_exchange/eth.py
--rw-r--r--   0 shubham    (501) staff       (20)     3152 2023-07-17 11:37:43.000000 hubble_exchange-0.3.0/hubble_exchange/models.py
--rw-r--r--   0 shubham    (501) staff       (20)     4407 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/order_book.py
--rw-r--r--   0 shubham    (501) staff       (20)      466 2023-07-14 06:05:29.000000 hubble_exchange-0.3.0/hubble_exchange/utils.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-17 11:43:19.120101 hubble_exchange-0.3.0/hubble_exchange.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)     5648 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      531 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)       88 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       16 2023-07-17 11:43:19.000000 hubble_exchange-0.3.0/hubble_exchange.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)     1002 2023-07-17 11:42:21.000000 hubble_exchange-0.3.0/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2023-07-17 11:43:19.120925 hubble_exchange-0.3.0/setup.cfg
--rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.3.0/setup.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-25 07:26:08.069373 hubble_exchange-0.4.0/
+-rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.4.0/LICENSE
+-rw-r--r--   0 shubham    (501) staff       (20)      101 2023-06-29 11:35:24.000000 hubble_exchange-0.4.0/MANIFEST.in
+-rw-r--r--   0 shubham    (501) staff       (20)     6421 2023-07-25 07:26:08.069117 hubble_exchange-0.4.0/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     4764 2023-07-25 07:13:22.000000 hubble_exchange-0.4.0/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-25 07:26:08.067297 hubble_exchange-0.4.0/hubble_exchange/
+-rw-r--r--   0 shubham    (501) staff       (20)      369 2023-07-25 06:59:23.000000 hubble_exchange-0.4.0/hubble_exchange/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     7500 2023-07-25 07:15:33.000000 hubble_exchange-0.4.0/hubble_exchange/client.py
+-rw-r--r--   0 shubham    (501) staff       (20)      202 2023-07-25 07:14:44.000000 hubble_exchange-0.4.0/hubble_exchange/constants.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-25 07:26:08.068671 hubble_exchange-0.4.0/hubble_exchange/contract_abis/
+-rw-r--r--   0 shubham    (501) staff       (20)    15194 2023-07-25 05:55:50.000000 hubble_exchange-0.4.0/hubble_exchange/contract_abis/OrderBook.json
+-rw-r--r--   0 shubham    (501) staff       (20)     1200 2023-07-14 06:05:29.000000 hubble_exchange-0.4.0/hubble_exchange/eip712.py
+-rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.4.0/hubble_exchange/errors.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5612 2023-07-25 07:10:52.000000 hubble_exchange-0.4.0/hubble_exchange/eth.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3467 2023-07-25 06:36:39.000000 hubble_exchange-0.4.0/hubble_exchange/models.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5176 2023-07-25 07:14:09.000000 hubble_exchange-0.4.0/hubble_exchange/order_book.py
+-rw-r--r--   0 shubham    (501) staff       (20)      562 2023-07-22 11:56:49.000000 hubble_exchange-0.4.0/hubble_exchange/utils.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2023-07-25 07:26:08.068510 hubble_exchange-0.4.0/hubble_exchange.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)     6421 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      531 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       88 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       16 2023-07-25 07:26:08.000000 hubble_exchange-0.4.0/hubble_exchange.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)     1002 2023-07-25 07:16:14.000000 hubble_exchange-0.4.0/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2023-07-25 07:26:08.069455 hubble_exchange-0.4.0/setup.cfg
+-rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.4.0/setup.py
```

### Comparing `hubble_exchange-0.3.0/LICENSE` & `hubble_exchange-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.3.0/PKG-INFO` & `hubble_exchange-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble_exchange
-Version: 0.3.0
+Version: 0.4.0
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -86,14 +86,17 @@
 
     # get current order book for market = 1
     order_book = await client.get_order_book(1, callback)
 
     # get current margin and positions(uses the address for which private key is set)
     positions = await client.get_margin_and_positions(callback)
 
+    # get order fills
+    order_fills = await client.get_order_fills
+
     # subscribe to order book updates for market = 0; receives a new message every second(only for those prices where the quantity has changed)
     async def on_message(ws, message):
         print(f"Received orderbook update: {message}")
 
     asyncio.run(client.subscribe_to_order_book_depth(0, callback=on_message))
 ```
 
@@ -139,7 +142,21 @@
 client = HubbleClient(os.getenv("PRIVATE_KEY"))
 placed_orders = await client.place_orders(orders, callback, mode=TransactionMode.wait_for_accept)
 
 # or set the default mode for all transactions
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
+
+## Trader feed
+
+All order updates related to a particular trader can be subscribed to using the `subscribe_to_trader_updates` method.
+It can be subscribed in 2 confirmation modes - head block or accepted block. Events received in head block mode are not finalised and can be reverted. When an event is removed from the chain, the client will receive a `removed=True` event. Events received in accepted block mode are finalised and will alwats have `removed=False`.
+
+```python
+import os
+from hubble_exchange import HubbleClient, ConfirmationMode
+
+async def main():
+    client = HubbleClient(os.getenv("PRIVATE_KEY"))
+    await client.subscribe_to_trader_updates(ConfirmationMode.accepted, callback)
+```
```

### Comparing `hubble_exchange-0.3.0/README.md` & `hubble_exchange-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
     # get current order book for market = 1
     order_book = await client.get_order_book(1, callback)
 
     # get current margin and positions(uses the address for which private key is set)
     positions = await client.get_margin_and_positions(callback)
 
+    # get order fills
+    order_fills = await client.get_order_fills
+
     # subscribe to order book updates for market = 0; receives a new message every second(only for those prices where the quantity has changed)
     async def on_message(ws, message):
         print(f"Received orderbook update: {message}")
 
     asyncio.run(client.subscribe_to_order_book_depth(0, callback=on_message))
 ```
 
@@ -106,7 +109,21 @@
 client = HubbleClient(os.getenv("PRIVATE_KEY"))
 placed_orders = await client.place_orders(orders, callback, mode=TransactionMode.wait_for_accept)
 
 # or set the default mode for all transactions
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
+
+## Trader feed
+
+All order updates related to a particular trader can be subscribed to using the `subscribe_to_trader_updates` method.
+It can be subscribed in 2 confirmation modes - head block or accepted block. Events received in head block mode are not finalised and can be reverted. When an event is removed from the chain, the client will receive a `removed=True` event. Events received in accepted block mode are finalised and will alwats have `removed=False`.
+
+```python
+import os
+from hubble_exchange import HubbleClient, ConfirmationMode
+
+async def main():
+    client = HubbleClient(os.getenv("PRIVATE_KEY"))
+    await client.subscribe_to_trader_updates(ConfirmationMode.accepted, callback)
+```
```

### Comparing `hubble_exchange-0.3.0/hubble_exchange/client.py` & `hubble_exchange-0.4.0/hubble_exchange/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import json
-from typing import List
+from typing import Dict, List
 
 import websockets
 from hexbytes import HexBytes
 
-from hubble_exchange.eth import get_web3_client, get_websocket_endpoint
+from hubble_exchange.eth import get_async_web3_client, get_websocket_endpoint
 from hubble_exchange.models import (AsyncOrderBookDepthCallback,
                                     AsyncOrderStatusCallback,
                                     AsyncPlaceOrdersCallback,
                                     AsyncPositionCallback,
                                     AsyncSubscribeToOrderBookDepthCallback,
-                                    Order, OrderBookDepthUpdateResponse,
-                                    OrderStatusResponse, WebsocketResponse)
+                                    ConfirmationMode, Order,
+                                    OrderBookDepthUpdateResponse,
+                                    OrderStatusResponse, TraderFeedUpdate,
+                                    WebsocketResponse)
 from hubble_exchange.order_book import OrderBookClient, TransactionMode
 from hubble_exchange.utils import (float_to_scaled_int,
                                    get_address_from_private_key, get_new_salt)
 
 
 class HubbleClient:
     def __init__(self, private_key: str):
         if not private_key:
             raise ValueError("Private key is not set")
         self.trader_address = get_address_from_private_key(private_key)
         if not self.trader_address:
             raise ValueError("Cannot determine trader address from private key")
 
-        self.web3_client = get_web3_client()
+        self.web3_client = get_async_web3_client()
         self.websocket_endpoint = get_websocket_endpoint()
         self.order_book_client = OrderBookClient(private_key)
 
     def set_transaction_mode(self, mode: TransactionMode):
         self.order_book_client.set_transaction_mode(mode)
 
     async def get_order_book(self, market: int, callback: AsyncOrderBookDepthCallback):
-        order_book_depth = self.web3_client.eth.get_order_book_depth(market)
+        order_book_depth = await self.web3_client.eth.get_order_book_depth(market)
         return await callback(order_book_depth)
 
     async def get_margin_and_positions(self, callback: AsyncPositionCallback):
-        response = self.web3_client.eth.get_margin_and_positions(self.trader_address)
+        response = await self.web3_client.eth.get_margin_and_positions(self.trader_address)
         return await callback(response)
 
     async def get_order_status(self, order_id: HexBytes, callback: AsyncOrderStatusCallback):
-        response = self.web3_client.eth.get_order_status(order_id.hex()) # type: ignore
+        response = await self.web3_client.eth.get_order_status(order_id.hex()) # type: ignore
         return await callback(response)
 
     async def place_orders(self, orders: List[Order], callback: AsyncPlaceOrdersCallback, tx_options = None, mode=None):
         if len(orders) > 75:
             raise ValueError("Cannot place more than 75 orders at once")
 
         for order in orders:
@@ -60,38 +62,38 @@
 
             # trader and salt can be set automatically
             if order.trader in [None, "0x", ""]:
                 order.trader = self.trader_address
             if order.salt in [None, 0]:
                 order.salt = get_new_salt()
 
-        response = self.order_book_client.place_orders(orders, tx_options, mode)
+        response = await self.order_book_client.place_orders(orders, tx_options, mode)
         return await callback(response)
 
     async def place_single_order(
         self, market: int, base_asset_quantity: float, price: float, reduce_only: bool, callback, tx_options = None, mode=None
     ) -> Order:
         order = Order(
             id=None,
             amm_index=market,
             trader=self.trader_address,
             base_asset_quantity=float_to_scaled_int(base_asset_quantity, 18),
             price=float_to_scaled_int(price, 6),
             salt=get_new_salt(),
             reduce_only=reduce_only,
         )
-        order_hash = self.order_book_client.place_order(order, tx_options, mode)
+        order_hash = await self.order_book_client.place_order(order, tx_options, mode)
         order.id = order_hash
         return await callback(order)
 
     async def cancel_orders(self, orders: List[Order], callback, tx_options = None, mode=None):
         if len(orders) > 100:
             raise ValueError("Cannot cancel more than 100 orders at once")
 
-        self.order_book_client.cancel_orders(orders, tx_options, mode)
+        await self.order_book_client.cancel_orders(orders, tx_options, mode)
         return await callback()
 
     async def cancel_order_by_id(self, order_id: HexBytes, callback, tx_options = None, mode=None):
         async def order_status_callback(response: OrderStatusResponse) -> Order:
             position_side_multiplier = 1 if response.positionSide == "LONG" else -1
             return Order(
                 id=order_id,
@@ -102,14 +104,17 @@
                 salt=int(response.salt),
                 reduce_only=response.reduceOnly,
             )
         order = await self.get_order_status(order_id, order_status_callback)
         response = await self.cancel_orders([order], callback, tx_options, mode)
         return await callback(response)
 
+    async def get_order_fills(self, order_id: str) -> List[Dict]:
+        return await self.order_book_client.get_order_fills(order_id)
+
     async def subscribe_to_order_book_depth(
         self, market: int, callback: AsyncSubscribeToOrderBookDepthCallback
     ) -> None:
         async with websockets.connect(self.websocket_endpoint) as ws:
             msg = {
                 "jsonrpc": "2.0",
                 "id": 1,
@@ -128,7 +133,29 @@
                     response = OrderBookDepthUpdateResponse(
                         T=response.params['result']['T'],
                         symbol=response.params['result']['s'],
                         bids=response.params['result']['b'],
                         asks=response.params['result']['a'],
                     )
                     await callback(ws, response)
+
+    async def subscribe_to_trader_updates(
+        self, update_type: ConfirmationMode, callback
+    ) -> None:
+        async with websockets.connect(self.websocket_endpoint) as ws:
+            msg = {
+                "jsonrpc": "2.0",
+                "id": 1,
+                "method": "trading_subscribe",
+                "params": ["streamTraderUpdates", self.trader_address, update_type.value]
+            }
+            await ws.send(json.dumps(msg))
+
+            async for message in ws:
+                message_json = json.loads(message)
+                if message_json.get('result'):
+                    # ignore because it's a subscription confirmation with subscription id
+                    continue
+                response = WebsocketResponse(**message_json)
+                if response.method and response.method == "trading_subscription":
+                    response = TraderFeedUpdate(**response.params['result'])
+                    await callback(ws, response)
```

### Comparing `hubble_exchange-0.3.0/hubble_exchange/contract_abis/OrderBook.json` & `hubble_exchange-0.4.0/hubble_exchange/contract_abis/OrderBook.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4425735780423281%*

 * *Differences: {'0': "{'inputs': {3: {'internalType': 'uint256', 'name': 'toLiquidate', 'type': 'uint256'}, "*

 * *      "insert: [(0, OrderedDict([('indexed', True), ('internalType', 'address'), ('name', "*

 * *      "'trader'), ('type', 'address')])), (1, OrderedDict([('indexed', True), ('internalType', "*

 * *      "'bytes32'), ('name', 'orderHash'), ('type', 'bytes32')])), (2, OrderedDict([('indexed', "*

 * *      "False), ('internalType', 'string'), ('name', 'err'), ('type', 'string')]))]}, 'name': "*

 * *      "'LiquidationError'}",*

 * * '1': " […]*

```diff
@@ -1,38 +1,9 @@
 [
     {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "_clearingHouse",
-                "type": "address"
-            },
-            {
-                "internalType": "address",
-                "name": "_marginAccount",
-                "type": "address"
-            }
-        ],
-        "stateMutability": "nonpayable",
-        "type": "constructor"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint8",
-                "name": "version",
-                "type": "uint8"
-            }
-        ],
-        "name": "Initialized",
-        "type": "event"
-    },
-    {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": true,
                 "internalType": "address",
                 "name": "trader",
                 "type": "address"
@@ -134,14 +105,57 @@
         "type": "event"
     },
     {
         "anonymous": false,
         "inputs": [
             {
                 "indexed": true,
+                "internalType": "address",
+                "name": "trader",
+                "type": "address"
+            },
+            {
+                "indexed": true,
+                "internalType": "bytes32",
+                "name": "orderHash",
+                "type": "bytes32"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fillAmount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "price",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "openInterestNotional",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "timestamp",
+                "type": "uint256"
+            }
+        ],
+        "name": "OrderMatched",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": true,
                 "internalType": "bytes32",
                 "name": "orderHash",
                 "type": "bytes32"
             },
             {
                 "indexed": false,
                 "internalType": "string",
@@ -197,15 +211,15 @@
                     {
                         "internalType": "bool",
                         "name": "reduceOnly",
                         "type": "bool"
                     }
                 ],
                 "indexed": false,
-                "internalType": "struct IOrderBook.Order",
+                "internalType": "struct ILimitOrderBook.Order",
                 "name": "order",
                 "type": "tuple"
             },
             {
                 "indexed": false,
                 "internalType": "uint256",
                 "name": "timestamp",
@@ -261,66 +275,14 @@
                 "type": "uint256"
             }
         ],
         "name": "OrdersMatched",
         "type": "event"
     },
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "account",
-                "type": "address"
-            }
-        ],
-        "name": "Paused",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "account",
-                "type": "address"
-            }
-        ],
-        "name": "Unpaused",
-        "type": "event"
-    },
-    {
-        "inputs": [],
-        "name": "ORDER_TYPEHASH",
-        "outputs": [
-            {
-                "internalType": "bytes32",
-                "name": "",
-                "type": "bytes32"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "bibliophile",
-        "outputs": [
-            {
-                "internalType": "contract IHubbleBibliophile",
-                "name": "",
-                "type": "address"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "ammIndex",
                         "type": "uint256"
@@ -347,15 +309,15 @@
                     },
                     {
                         "internalType": "bool",
                         "name": "reduceOnly",
                         "type": "bool"
                     }
                 ],
-                "internalType": "struct IOrderBook.Order",
+                "internalType": "struct ILimitOrderBook.Order",
                 "name": "order",
                 "type": "tuple"
             }
         ],
         "name": "cancelOrder",
         "outputs": [],
         "stateMutability": "nonpayable",
@@ -392,101 +354,43 @@
                     },
                     {
                         "internalType": "bool",
                         "name": "reduceOnly",
                         "type": "bool"
                     }
                 ],
-                "internalType": "struct IOrderBook.Order[]",
+                "internalType": "struct ILimitOrderBook.Order[]",
                 "name": "orders",
                 "type": "tuple[]"
             }
         ],
         "name": "cancelOrders",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "clearingHouse",
-        "outputs": [
-            {
-                "internalType": "contract IClearingHouse",
-                "name": "",
-                "type": "address"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
-                "components": [
-                    {
-                        "internalType": "uint256",
-                        "name": "ammIndex",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "address",
-                        "name": "trader",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "int256",
-                        "name": "baseAssetQuantity",
-                        "type": "int256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "price",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "salt",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "bool",
-                        "name": "reduceOnly",
-                        "type": "bool"
-                    }
-                ],
-                "internalType": "struct IOrderBook.Order[2]",
+                "internalType": "bytes[2]",
                 "name": "orders",
-                "type": "tuple[2]"
+                "type": "bytes[2]"
             },
             {
                 "internalType": "int256",
                 "name": "fillAmount",
                 "type": "int256"
             }
         ],
         "name": "executeMatchedOrders",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getLastTradePrices",
-        "outputs": [
-            {
-                "internalType": "uint256[]",
-                "name": "lastTradePrices",
-                "type": "uint256[]"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "ammIndex",
                         "type": "uint256"
@@ -513,15 +417,15 @@
                     },
                     {
                         "internalType": "bool",
                         "name": "reduceOnly",
                         "type": "bool"
                     }
                 ],
-                "internalType": "struct IOrderBook.Order",
+                "internalType": "struct ILimitOrderBook.Order",
                 "name": "order",
                 "type": "tuple"
             }
         ],
         "name": "getOrderHash",
         "outputs": [
             {
@@ -533,88 +437,52 @@
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "int256",
-                "name": "baseAssetQuantity",
+                "name": "minSize",
                 "type": "int256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "price",
-                "type": "uint256"
-            }
-        ],
-        "name": "getRequiredMargin",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "requiredMargin",
-                "type": "uint256"
             }
         ],
-        "stateMutability": "view",
+        "name": "initializeMinSize",
+        "outputs": [],
+        "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "governance",
-        "outputs": [
+        "inputs": [
             {
                 "internalType": "address",
-                "name": "",
+                "name": "signer",
                 "type": "address"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "string",
-                "name": "_name",
-                "type": "string"
-            },
-            {
-                "internalType": "string",
-                "name": "_version",
-                "type": "string"
             },
             {
                 "internalType": "address",
-                "name": "_governance",
+                "name": "trader",
                 "type": "address"
             }
         ],
-        "name": "initialize",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
+        "name": "isTradingAuthority",
+        "outputs": [
             {
-                "internalType": "int256",
-                "name": "minSize",
-                "type": "int256"
+                "internalType": "bool",
+                "name": "",
+                "type": "bool"
             }
         ],
-        "name": "initializeMinSize",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "address",
-                "name": "",
+                "name": "validator",
                 "type": "address"
             }
         ],
         "name": "isValidator",
         "outputs": [
             {
                 "internalType": "bool",
@@ -629,179 +497,65 @@
         "inputs": [
             {
                 "internalType": "address",
                 "name": "trader",
                 "type": "address"
             },
             {
-                "components": [
-                    {
-                        "internalType": "uint256",
-                        "name": "ammIndex",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "address",
-                        "name": "trader",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "int256",
-                        "name": "baseAssetQuantity",
-                        "type": "int256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "price",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "salt",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "bool",
-                        "name": "reduceOnly",
-                        "type": "bool"
-                    }
-                ],
-                "internalType": "struct IOrderBook.Order",
+                "internalType": "bytes",
                 "name": "order",
-                "type": "tuple"
+                "type": "bytes"
             },
             {
                 "internalType": "uint256",
-                "name": "liquidationAmount",
+                "name": "toLiquidate",
                 "type": "uint256"
             }
         ],
         "name": "liquidateAndExecuteOrder",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "marginAccount",
-        "outputs": [
-            {
-                "internalType": "contract IMarginAccount",
-                "name": "",
-                "type": "address"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "minAllowableMargin",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "name": "minSizes",
-        "outputs": [
-            {
-                "internalType": "int256",
-                "name": "",
-                "type": "int256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "internalType": "bytes32",
-                "name": "",
-                "type": "bytes32"
-            }
-        ],
-        "name": "orderInfo",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "blockPlaced",
-                "type": "uint256"
-            },
-            {
-                "internalType": "int256",
-                "name": "filledAmount",
-                "type": "int256"
-            },
-            {
-                "internalType": "uint256",
-                "name": "reservedMargin",
-                "type": "uint256"
-            },
-            {
-                "internalType": "enum IOrderBook.OrderStatus",
-                "name": "status",
-                "type": "uint8"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "string",
-                "name": "err",
-                "type": "string"
-            }
-        ],
-        "name": "parseMatchingError",
-        "outputs": [
-            {
-                "internalType": "bytes32",
                 "name": "orderHash",
                 "type": "bytes32"
-            },
-            {
-                "internalType": "string",
-                "name": "reason",
-                "type": "string"
             }
         ],
-        "stateMutability": "pure",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "pause",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "paused",
+        "name": "orderStatus",
         "outputs": [
             {
-                "internalType": "bool",
+                "components": [
+                    {
+                        "internalType": "uint256",
+                        "name": "blockPlaced",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "int256",
+                        "name": "filledAmount",
+                        "type": "int256"
+                    },
+                    {
+                        "internalType": "uint256",
+                        "name": "reservedMargin",
+                        "type": "uint256"
+                    },
+                    {
+                        "internalType": "enum IOrderHandler.OrderStatus",
+                        "name": "status",
+                        "type": "uint8"
+                    }
+                ],
+                "internalType": "struct ILimitOrderBook.OrderInfo",
                 "name": "",
-                "type": "bool"
+                "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
@@ -834,15 +588,15 @@
                     },
                     {
                         "internalType": "bool",
                         "name": "reduceOnly",
                         "type": "bool"
                     }
                 ],
-                "internalType": "struct IOrderBook.Order",
+                "internalType": "struct ILimitOrderBook.Order",
                 "name": "order",
                 "type": "tuple"
             }
         ],
         "name": "placeOrder",
         "outputs": [],
         "stateMutability": "nonpayable",
@@ -879,236 +633,79 @@
                     },
                     {
                         "internalType": "bool",
                         "name": "reduceOnly",
                         "type": "bool"
                     }
                 ],
-                "internalType": "struct IOrderBook.Order[]",
+                "internalType": "struct ILimitOrderBook.Order[]",
                 "name": "orders",
                 "type": "tuple[]"
             }
         ],
         "name": "placeOrders",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "address",
-                "name": "",
+                "name": "trader",
                 "type": "address"
             },
             {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "name": "reduceOnlyAmount",
-        "outputs": [
-            {
-                "internalType": "int256",
-                "name": "",
-                "type": "int256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
                 "internalType": "address",
-                "name": "_bibliophile",
+                "name": "authority",
                 "type": "address"
             }
         ],
-        "name": "setBibliophile",
+        "name": "setTradingAuthority",
         "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "__governance",
-                "type": "address"
-            }
-        ],
-        "name": "setGovernace",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "bool",
-                "name": "useNew",
-                "type": "bool"
-            }
-        ],
-        "name": "setUseNewPricingAlgorithm",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "internalType": "address",
-                "name": "validator",
-                "type": "address"
-            },
-            {
-                "internalType": "bool",
-                "name": "status",
-                "type": "bool"
-            }
-        ],
-        "name": "setValidatorStatus",
-        "outputs": [],
-        "stateMutability": "nonpayable",
+        "stateMutability": "payable",
         "type": "function"
     },
     {
         "inputs": [],
         "name": "settleFunding",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "takerFee",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "unpause",
-        "outputs": [],
-        "stateMutability": "nonpayable",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
-                "internalType": "uint256",
-                "name": "ammIndex",
-                "type": "uint256"
+                "internalType": "bytes",
+                "name": "data",
+                "type": "bytes"
             },
             {
-                "internalType": "int256",
-                "name": "minSize",
-                "type": "int256"
+                "internalType": "bytes",
+                "name": "metadata",
+                "type": "bytes"
             }
         ],
-        "name": "updateMinSize",
+        "name": "updateOrder",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
     },
     {
         "inputs": [
             {
                 "internalType": "uint256",
-                "name": "_minAllowableMargin",
+                "name": "minAllowableMargin",
                 "type": "uint256"
             },
             {
                 "internalType": "uint256",
-                "name": "_takerFee",
+                "name": "takerFee",
                 "type": "uint256"
             }
         ],
         "name": "updateParams",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
-    },
-    {
-        "inputs": [],
-        "name": "useNewPricingAlgorithm",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
-        "inputs": [
-            {
-                "components": [
-                    {
-                        "internalType": "uint256",
-                        "name": "ammIndex",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "address",
-                        "name": "trader",
-                        "type": "address"
-                    },
-                    {
-                        "internalType": "int256",
-                        "name": "baseAssetQuantity",
-                        "type": "int256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "price",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "uint256",
-                        "name": "salt",
-                        "type": "uint256"
-                    },
-                    {
-                        "internalType": "bool",
-                        "name": "reduceOnly",
-                        "type": "bool"
-                    }
-                ],
-                "internalType": "struct IOrderBook.Order",
-                "name": "order",
-                "type": "tuple"
-            },
-            {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
-            }
-        ],
-        "name": "verifySigner",
-        "outputs": [
-            {
-                "internalType": "address",
-                "name": "",
-                "type": "address"
-            },
-            {
-                "internalType": "bytes32",
-                "name": "",
-                "type": "bytes32"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
     }
 ]
```

### Comparing `hubble_exchange-0.3.0/hubble_exchange/eip712.py` & `hubble_exchange-0.4.0/hubble_exchange/eip712.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.3.0/hubble_exchange/eth.py` & `hubble_exchange-0.4.0/hubble_exchange/eth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,119 @@
 
+import asyncio
 import os
-from typing import Callable, Dict
+from typing import Awaitable, Callable, Dict
 
 from eth_typing import Address
 from hexbytes import HexBytes
-from web3 import HTTPProvider, Web3
-from web3.eth.eth import Eth, Timeout
+from web3 import AsyncHTTPProvider, AsyncWeb3, HTTPProvider, Web3
+from web3.eth.async_eth import AsyncEth
 from web3.exceptions import TimeExhausted
-from web3.main import Web3, get_default_modules
+from web3.main import Web3, get_async_default_modules
 from web3.method import Method, default_root_munger
-from web3.middleware import geth_poa_middleware
-from web3.middleware.cache import construct_simple_cache_middleware
+from web3.middleware import async_geth_poa_middleware, geth_poa_middleware, construct_simple_cache_middleware
+from web3.middleware.async_cache import _async_simple_cache_middleware
 from web3.types import RPCEndpoint, _Hash32
 
 from hubble_exchange.errors import OrderNotFound, TraderNotFound
 from hubble_exchange.models import (GetPositionsResponse,
                                     OrderBookDepthResponse,
                                     OrderStatusResponse)
 
-
 rpc_endpoint = ""
 websocket_endpoint = ""
 
 
-class HubblenetEth(Eth):
-    _get_transaction_status: Method[Callable[[_Hash32], Dict]] = Method(RPCEndpoint("eth_getTransactionStatus"), mungers=[default_root_munger])
-    _get_order_status: Method[Callable[[_Hash32], Dict]] = Method(RPCEndpoint("trading_getOrderStatus"), mungers=[default_root_munger])
-    _get_margin_and_positions: Method[Callable[[Address], Dict]] = Method(RPCEndpoint("trading_getMarginAndPositions"), mungers=[default_root_munger])
-    _get_order_book_depth: Method[Callable[[int], Dict]] = Method(RPCEndpoint("trading_getTradingOrderBookDepth"), mungers=[default_root_munger])
-
-    def get_transaction_status(self, transaction_hash: _Hash32) -> Dict:
-        return self._get_transaction_status(transaction_hash)
+class HubblenetEth(AsyncEth):
+    _get_transaction_status: Method[Callable[[_Hash32], Awaitable[Dict]]] = Method(RPCEndpoint("eth_getTransactionStatus"), mungers=[default_root_munger])
+    _get_order_status: Method[Callable[[_Hash32], Awaitable[Dict]]] = Method(RPCEndpoint("trading_getOrderStatus"), mungers=[default_root_munger])
+    _get_margin_and_positions: Method[Callable[[Address], Awaitable[Dict]]] = Method(RPCEndpoint("trading_getMarginAndPositions"), mungers=[default_root_munger])
+    _get_order_book_depth: Method[Callable[[int], Awaitable[Dict]]] = Method(RPCEndpoint("trading_getTradingOrderBookDepth"), mungers=[default_root_munger])
 
-    def get_order_status(self, order_id: _Hash32) -> OrderStatusResponse:
+    async def get_order_status(self, order_id: _Hash32) -> OrderStatusResponse:
         try:
-            response = self._get_order_status(order_id)
+            response = await self._get_order_status(order_id)
             return OrderStatusResponse(**response)
         except ValueError as e:
             if len(e.args) > 0 and e.args[0].get('message', '') == "order not found":
                 raise OrderNotFound()
             else:
                 raise e
 
-    def get_margin_and_positions(self, trader: Address) -> GetPositionsResponse:
+    async def get_margin_and_positions(self, trader: Address) -> GetPositionsResponse:
         try:
-            response = self._get_margin_and_positions(trader)
+            response = await self._get_margin_and_positions(trader)
             return GetPositionsResponse(**response)
         except ValueError as e:
             if len(e.args) > 0 and e.args[0].get('message', '') == "trader not found":
                 raise TraderNotFound()
             else:
                 raise e
 
-    def get_order_book_depth(self, market: int) -> OrderBookDepthResponse:
-        response = self._get_order_book_depth(market)
+    async def get_order_book_depth(self, market: int) -> OrderBookDepthResponse:
+        response = await self._get_order_book_depth(market)
         return OrderBookDepthResponse(**response)
 
-    def wait_for_transaction_status(self, transaction_hash: HexBytes, timeout: float = 120, poll_latency: float = 0.1) -> Dict:
-        try:
-            with Timeout(timeout) as _timeout:
-                while True:
-                    try:
-                        tx_status = self._get_transaction_status(transaction_hash.hex())
-                    except:
-                        tx_status = None
-                    if tx_status is None or tx_status['status'] == "NOT_FOUND":
-                        _timeout.sleep(poll_latency)
-                        continue
-                    else:
-                        break
+    async def wait_for_transaction_status(self, transaction_hash: HexBytes, timeout: float = 120, poll_latency: float = 0.1) -> Dict:
+        async def _wait_for_status_with_timeout(
+            _tx_hash: _Hash32, _poll_latency: float
+        ) -> Dict:
+            while True:
+                try:
+                    tx_status = await self._get_transaction_status(_tx_hash.hex())
+                except:
+                    tx_status = None
+                if tx_status is None or tx_status['status'] == "NOT_FOUND":
+                    await asyncio.sleep(_poll_latency)
+                    continue
+                else:
+                    break
             return tx_status
 
-        except Timeout:
+        try:
+            return await asyncio.wait_for(
+                _wait_for_status_with_timeout(transaction_hash, poll_latency),
+                timeout=timeout,
+            )
+        except asyncio.TimeoutError:
             raise TimeExhausted(
                 f"Transaction {HexBytes(transaction_hash) !r} is not in the chain "
                 f"after {timeout} seconds"
             )
 
 
+class HubblenetWeb3(AsyncWeb3):
+    eth: HubblenetEth
+
+
 def get_web3_modules() -> Dict:
-    modules = get_default_modules()
+    modules = get_async_default_modules()
     modules["eth"] = HubblenetEth
     return modules
 
-class HubblenetWeb3(Web3):
-    eth: HubblenetEth
+
+def get_async_web3_client() -> HubblenetWeb3:
+    rpc_endpoint = get_rpc_endpoint()
+
+    web3_client = HubblenetWeb3(AsyncHTTPProvider(rpc_endpoint), modules=get_web3_modules())
+    web3_client.middleware_onion.inject(async_geth_poa_middleware, layer=0)
+
+    # cache frequent eth_chainId calls
+    web3_client.middleware_onion.add(_async_simple_cache_middleware, name="cache")
+    return web3_client
+
+
+def get_sync_web3_client() -> Web3:
+    rpc_endpoint = get_rpc_endpoint()
+
+    web3_client = Web3(HTTPProvider(rpc_endpoint))
+    web3_client.middleware_onion.inject(geth_poa_middleware, layer=0)
+
+    web3_client.middleware_onion.add(construct_simple_cache_middleware(), name="cache")
+    return web3_client
 
 
 def get_rpc_endpoint() -> str:
     global rpc_endpoint
     if not rpc_endpoint:
         rpc_host = os.getenv("HUBBLE_RPC_HOST")
         if not rpc_host:
@@ -109,19 +134,7 @@
             raise ValueError("HUBBLE_RPC_HOST environment variable not set")
         blockchain_id = os.getenv("HUBBLE_BLOCKCHAIN_ID")
         if not blockchain_id:
             raise ValueError("HUBBLE_BLOCKCHAIN_ID environment variable not set")
         path = f"/ext/bc/{blockchain_id}/ws"
         websocket_endpoint = f"wss://{rpc_host}{path}"
     return websocket_endpoint
-
-
-def get_web3_client() -> HubblenetWeb3:
-    rpc_endpoint = get_rpc_endpoint()
-    
-    web3_client = HubblenetWeb3(HTTPProvider(rpc_endpoint), modules=get_web3_modules())
-    web3_client.middleware_onion.inject(geth_poa_middleware, layer=0)
-
-    # cache frequent eth_chainId calls
-    cache_chain_id_middleware = construct_simple_cache_middleware()
-    web3_client.middleware_onion.add(cache_chain_id_middleware, name="cache")
-    return web3_client
```

### Comparing `hubble_exchange-0.3.0/hubble_exchange/models.py` & `hubble_exchange-0.4.0/hubble_exchange/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
-from typing import Any, Coroutine, List
+from enum import Enum
+from typing import Any, Coroutine, Dict, List
 
 from eth_typing import Address
 from hexbytes import HexBytes
 from typing_extensions import Protocol
 
 from hubble_exchange.utils import float_to_scaled_int, get_new_salt
 
@@ -120,14 +121,27 @@
 class OrderBookDepthUpdateResponse:
     T: int
     symbol: int
     bids: List[List[str]]
     asks: List[List[str]]
 
 
+@dataclass
+class TraderFeedUpdate:
+    Trader: Address
+    OrderId: HexBytes
+    OrderType: str
+    Removed: bool
+    EventName: str
+    Args: Dict
+    BlockNumber: int
+    BlockStatus: str
+    Timestamp: int
+
+
 class AsyncOrderBookDepthCallback(Protocol):
     def __call__(self, response: OrderBookDepthResponse) -> Coroutine[Any, Any, Any]: ...
 
 
 class AsyncPositionCallback(Protocol):
     def __call__(self, response: GetPositionsResponse) -> Coroutine[Any, Any, Any]: ...
 
@@ -138,7 +152,12 @@
 
 class AsyncPlaceOrdersCallback(Protocol):
     def __call__(self, response: List[Order]) -> Coroutine[Any, Any, Any]: ...
 
 
 class AsyncSubscribeToOrderBookDepthCallback(Protocol):
     def __call__(self, ws, response: OrderBookDepthUpdateResponse) -> Coroutine[Any, Any, Any]: ...
+
+
+class ConfirmationMode(Enum):
+    head = "head"
+    accepted = "accepted"
```

### Comparing `hubble_exchange-0.3.0/hubble_exchange/order_book.py` & `hubble_exchange-0.4.0/hubble_exchange/order_book.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,131 @@
 import json
 import os
+import time
 from enum import Enum
 from typing import Any, Dict, List
 
 from hexbytes import HexBytes
 
 from hubble_exchange.constants import (CHAIN_ID, GAS_PER_ORDER, MAX_GAS_LIMIT,
                                        OrderBookContractAddress)
 from hubble_exchange.eip712 import get_order_hash
 from hubble_exchange.eth import HubblenetWeb3 as Web3
-from hubble_exchange.eth import get_web3_client
+from hubble_exchange.eth import get_async_web3_client, get_sync_web3_client
 from hubble_exchange.models import Order
-from hubble_exchange.utils import get_address_from_private_key
+from hubble_exchange.utils import (get_address_from_private_key,
+                                   int_to_scaled_float)
 
 # read abi from file
 HERE = os.path.dirname(__file__)
 with open(f"{HERE}/contract_abis/OrderBook.json", 'r') as abi_file:
     abi_str = abi_file.read()
     ABI = json.loads(abi_str)
 
 
 class TransactionMode(Enum):
     no_wait = 0
-    wait_for_accept = 1
     wait_for_head = 1
+    wait_for_accept = 2
 
 
 class OrderBookClient(object):
     def __init__(self, private_key: str):
         self._private_key = private_key
         self.public_address = get_address_from_private_key(private_key)
 
-        self.web3_client = get_web3_client()
+        self.web3_client = get_async_web3_client()
         self.order_book = self.web3_client.eth.contract(address=OrderBookContractAddress, abi=ABI)
-        self.nonce = self.web3_client.eth.get_transaction_count(self.public_address)
-        self.transaction_mode = TransactionMode.no_wait
+
+        # get nonce from sync web3 client
+        sync_web3 = get_sync_web3_client()
+        self.nonce = sync_web3.eth.get_transaction_count(self.public_address)
+
+        self.transaction_mode = TransactionMode.no_wait  # default
 
     def set_transaction_mode(self, mode: TransactionMode):
         self.transaction_mode = mode
 
-    def place_order(self, order: Order, custom_tx_options=None, mode=None) -> HexBytes:
+    async def place_order(self, order: Order, custom_tx_options=None, mode=None) -> HexBytes:
         order_hash = get_order_hash(order)
 
         tx_options = {'gas': GAS_PER_ORDER}
         tx_options.update(custom_tx_options or {})
 
-        self._send_orderbook_transaction("placeOrder", [order.to_dict()], tx_options, mode)
+        await self._send_orderbook_transaction("placeOrder", [order.to_dict()], tx_options, mode)
         return order_hash
 
-    def place_orders(self, orders: List[Order], custom_tx_options=None, mode=None) -> List[Order]:
+    async def place_orders(self, orders: List[Order], custom_tx_options=None, mode=None) -> List[Order]:
         """
         Place multiple orders at once. This is more efficient than placing them one by one.
         """
         place_order_payload = []
 
         for order in orders:
             order_hash = get_order_hash(order)
             order.id = order_hash
             place_order_payload.append(order.to_dict())
 
         tx_options = {'gas': min(GAS_PER_ORDER * len(orders), MAX_GAS_LIMIT)}
         tx_options.update(custom_tx_options or {})
-        self._send_orderbook_transaction("placeOrders", [place_order_payload], tx_options, mode)
+        await self._send_orderbook_transaction("placeOrders", [place_order_payload], tx_options, mode)
         return orders
 
-    def cancel_orders(self, orders: list[Order], custom_tx_options=None, mode=None) -> None:
+    async def cancel_orders(self, orders: list[Order], custom_tx_options=None, mode=None) -> None:
         cancel_order_payload = []
         for order in orders:
             cancel_order_payload.append(order.to_dict())
 
         tx_options = {'gas': min(GAS_PER_ORDER * len(orders), MAX_GAS_LIMIT)}
         tx_options.update(custom_tx_options or {})
 
-        self._send_orderbook_transaction("cancelOrders", [cancel_order_payload], tx_options, mode)
+        await self._send_orderbook_transaction("cancelOrders", [cancel_order_payload], tx_options, mode)
+
+    async def get_order_fills(self, order_id: str) -> List[Dict]:
+        orders_matched_events = await self.order_book.events.OrderMatched().get_logs(
+            {"orderHash": order_id},
+            fromBlock='earliest',
+        )
+
+        fills = []
+        for event in orders_matched_events:
+            fills.append({
+                "block_number": event.blockNumber,
+                "transaction_hash": event.transactionHash,
+                "timestamp": event.args.timestamp,
+                "fill_amount": int_to_scaled_float(event.args.fillAmount, 18),
+                "price": int_to_scaled_float(event.args.price, 6),
+            })
+        return fills
 
-    def _get_nonce(self) -> int:
+    async def _get_nonce(self) -> int:
         if self.nonce is None:
-            self.nonce = self.web3_client.eth.get_transaction_count(self.public_address)
+            self.nonce = await self.web3_client.eth.get_transaction_count(self.public_address)
         else:
             self.nonce += 1
         return self.nonce - 1
 
-    def _send_orderbook_transaction(self, method_name: str, args: List[Any], tx_options: Dict, mode: TransactionMode) -> HexBytes:
+    async def _send_orderbook_transaction(self, method_name: str, args: List[Any], tx_options: Dict, mode: TransactionMode) -> HexBytes:
         if mode is None:
             mode = self.transaction_mode
 
         method = getattr(self.order_book.functions, method_name)
-        nonce = self._get_nonce()
+        nonce = await self._get_nonce()
         tx_params = {
             'from': self.public_address,
             'chainId': CHAIN_ID,
             'maxFeePerGas': Web3.to_wei(60, 'gwei'),  # base + tip
             'maxPriorityFeePerGas': 0,  # tip
             'nonce': nonce,
         }
         if tx_options:
             tx_params.update(tx_options)
 
-        transaction = method(*args).build_transaction(tx_params)
+        transaction = await method(*args).build_transaction(tx_params)
         signed_tx = self.web3_client.eth.account.sign_transaction(transaction, self._private_key)
-        tx_hash = self.web3_client.eth.send_raw_transaction(signed_tx.rawTransaction)
+        tx_hash = await self.web3_client.eth.send_raw_transaction(signed_tx.rawTransaction)
         if mode == TransactionMode.wait_for_accept:
-            self._wait_for_accept(tx_hash)
+            await self.web3_client.eth.wait_for_transaction_receipt(tx_hash, timeout=120, poll_latency=0.1)
         elif mode == TransactionMode.wait_for_head:
-            self._wait_for_head(tx_hash)
+            await self.web3_client.eth.wait_for_transaction_status(tx_hash, timeout=120, poll_latency=0.1)
 
         return tx_hash
-
-    def _wait_for_accept(self, tx_hash: HexBytes):
-        self.web3_client.eth.wait_for_transaction_receipt(tx_hash, timeout=120, poll_latency=0.1)
-
-    def _wait_for_head(self, tx_hash: HexBytes):
-        self.web3_client.eth.wait_for_transaction_status(tx_hash, timeout=120, poll_latency=0.1)
```

### Comparing `hubble_exchange-0.3.0/hubble_exchange.egg-info/PKG-INFO` & `hubble_exchange-0.4.0/hubble_exchange.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble-exchange
-Version: 0.3.0
+Version: 0.4.0
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -86,14 +86,17 @@
 
     # get current order book for market = 1
     order_book = await client.get_order_book(1, callback)
 
     # get current margin and positions(uses the address for which private key is set)
     positions = await client.get_margin_and_positions(callback)
 
+    # get order fills
+    order_fills = await client.get_order_fills
+
     # subscribe to order book updates for market = 0; receives a new message every second(only for those prices where the quantity has changed)
     async def on_message(ws, message):
         print(f"Received orderbook update: {message}")
 
     asyncio.run(client.subscribe_to_order_book_depth(0, callback=on_message))
 ```
 
@@ -139,7 +142,21 @@
 client = HubbleClient(os.getenv("PRIVATE_KEY"))
 placed_orders = await client.place_orders(orders, callback, mode=TransactionMode.wait_for_accept)
 
 # or set the default mode for all transactions
 
 client.set_transaction_mode(TransactionMode.wait_for_head)
 ```
+
+## Trader feed
+
+All order updates related to a particular trader can be subscribed to using the `subscribe_to_trader_updates` method.
+It can be subscribed in 2 confirmation modes - head block or accepted block. Events received in head block mode are not finalised and can be reverted. When an event is removed from the chain, the client will receive a `removed=True` event. Events received in accepted block mode are finalised and will alwats have `removed=False`.
+
+```python
+import os
+from hubble_exchange import HubbleClient, ConfirmationMode
+
+async def main():
+    client = HubbleClient(os.getenv("PRIVATE_KEY"))
+    await client.subscribe_to_trader_updates(ConfirmationMode.accepted, callback)
+```
```

### Comparing `hubble_exchange-0.3.0/hubble_exchange.egg-info/SOURCES.txt` & `hubble_exchange-0.4.0/hubble_exchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.3.0/pyproject.toml` & `hubble_exchange-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 author_email = "lumos@hubble.exchange"
 long_description = {file = "README.md"}
 long_description_content_type = "text/markdown"
 url = "https://github.com/hubble-exchange/python-sdk"
 
 [project]
 name = "hubble_exchange"
-version = "0.3.0"
+version = "0.4.0"
 description = "Official python SDK for Hubble Exchange"
 authors = [{name = "Lumos", email = "lumos@hubble.exchange"}]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies = [
     "web3 >= 6.5.0",
     "eth_typing >= 3.4.0",
```

