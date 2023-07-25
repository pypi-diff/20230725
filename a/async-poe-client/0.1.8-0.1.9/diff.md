# Comparing `tmp/async_poe_client-0.1.8.tar.gz` & `tmp/async_poe_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_poe_client-0.1.8.tar", max compression
+gzip compressed data, was "async_poe_client-0.1.9.tar", max compression
```

## Comparing `async_poe_client-0.1.8.tar` & `async_poe_client-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.1.8/async_poe_client/__init__.py
--rw-r--r--   0        0        0    48449 2023-07-24 13:56:23.918975 async_poe_client-0.1.8/async_poe_client/client.py
--rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.1.8/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.1.8/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.1.8/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.1.8/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
--rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.1.8/async_poe_client/poe_graphql/BioFragment.graphql
--rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.1.8/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
--rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.1.8/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.1.8/async_poe_client/poe_graphql/ChatFragment.graphql
--rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.1.8/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.1.8/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.1.8/async_poe_client/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.1.8/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.1.8/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.1.8/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.1.8/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.1.8/async_poe_client/poe_graphql/HandleFragment.graphql
--rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.1.8/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.1.8/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.1.8/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.1.8/async_poe_client/poe_graphql/MessageFragment.graphql
--rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.1.8/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.1.8/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.1.8/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.1.8/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.1.8/async_poe_client/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.1.8/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.1.8/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.1.8/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.1.8/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.1.8/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.1.8/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.1.8/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.1.8/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.1.8/async_poe_client/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.1.8/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.1.8/async_poe_client/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.1.8/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.1.8/async_poe_client/requirements.txt
--rw-r--r--   0        0        0     1648 2023-07-24 06:33:37.590357 async_poe_client-0.1.8/async_poe_client/util.py
--rw-r--r--   0        0        0      445 2023-07-24 11:33:59.741736 async_poe_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    16836 2023-07-24 06:32:46.931339 async_poe_client-0.1.8/README.md
--rw-r--r--   0        0        0    17088 1970-01-01 00:00:00.000000 async_poe_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.1.9/async_poe_client/__init__.py
+-rw-r--r--   0        0        0    48716 2023-07-25 01:15:45.644096 async_poe_client-0.1.9/async_poe_client/client.py
+-rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.1.9/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.1.9/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.1.9/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.1.9/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
+-rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.1.9/async_poe_client/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.1.9/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
+-rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.1.9/async_poe_client/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.1.9/async_poe_client/requirements.txt
+-rw-r--r--   0        0        0     1648 2023-07-24 06:33:37.590357 async_poe_client-0.1.9/async_poe_client/util.py
+-rw-r--r--   0        0        0      445 2023-07-25 01:17:52.886038 async_poe_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    16836 2023-07-24 06:32:46.931339 async_poe_client-0.1.9/README.md
+-rw-r--r--   0        0        0    17088 1970-01-01 00:00:00.000000 async_poe_client-0.1.9/PKG-INFO
```

### Comparing `async_poe_client-0.1.8/async_poe_client/client.py` & `async_poe_client-0.1.9/async_poe_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import hashlib
 import json
 import random
 import re
 import time
 import uuid
-from typing import List, Union, AsyncGenerator, Optional, Any
+from typing import List, Union, AsyncGenerator, Optional
 
 import aiohttp
 from aiohttp_socks import ProxyConnector
 from loguru import logger
 
 from .util import (
     HOME_URL,
@@ -23,54 +23,55 @@
 )
 
 Last_Use_Time = time.time()
 
 
 class Poe_Client:
     def __init__(self, p_b: str, formkey: str, proxy: str = ""):
+        self.channel_url: str = ""
         self.bots: dict = {}
         self.bot_list_url: str = ""
         self.formkey: str = formkey
         self.home_bot_list: List[str] = []
         self.next_data: dict = {}
         self.p_b: str = p_b
         self.sdid: str = ""
         self.subscription: dict = {}
         self.tchannel_data: dict = {}
         self.user_id: str = ""
         self.viewer: dict = {}
         self.ws_domain = f"tch{random.randint(1, int(1e6))}"[:8]
         self.proxy = proxy
         self.headers = {
-            'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
-            'Accept-Encoding': 'gzip, deflate, br',
-            'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
-            'Cache-Control': 'max-age=0',
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6",
+            "Cache-Control": "max-age=0",
             "Cookie": f"p-b={self.p_b}; SL_G_WPT_TO=zh-CN; SL_GWPT_Show_Hide_tmp=1; SL_wptGlobTipTmp=1;",
             "poe-formkey": self.formkey,
-            'Sec-Ch-Ua': '"Microsoft Edge";v="117", "Not;A Brand";v="8", "Chromium";v="117"',
-            'Sec-Ch-Ua-Mobile': '?0',
-            'Sec-Ch-Ua-Platform': '"Windows"',
-            'Sec-Fetch-Dest': 'document',
-            'Sec-Fetch-Mode': 'navigate',
-            'Sec-Fetch-Site': 'same-origin',
-            'Sec-Fetch-User': '?1',
-            'Upgrade-Insecure-Requests': '1',
-            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36 Edg/117.0.0.0',
+            "Sec-Ch-Ua": '"Microsoft Edge";v="117", "Not;A Brand";v="8", "Chromium";v="117"',
+            "Sec-Ch-Ua-Mobile": "?0",
+            "Sec-Ch-Ua-Platform": '"Windows"',
+            "Sec-Fetch-Dest": "document",
+            "Sec-Fetch-Mode": "navigate",
+            "Sec-Fetch-Site": "same-origin",
+            "Sec-Fetch-User": "?1",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36 Edg/117.0.0.0",
         }
 
     @property
     def session_args(self):
         args = {
-            'headers': self.headers,
-            'cookies': {"p-b": self.p_b},
+            "headers": self.headers,
+            "cookies": {"p-b": self.p_b},
         }
         if self.proxy:
             connector = ProxyConnector.from_url(self.proxy)
-            args['connector'] = connector
+            args["connector"] = connector
         return args
 
     async def get_basedata(self) -> None:
         """
         This function fetches the basic data from the HOME_URL and sets various attributes of the object.
 
         Raises:
@@ -106,59 +107,32 @@
                 self.home_bot_list.append(bot["node"]["handle"])
             self.sdid = str(uuid.uuid5(CONST_NAMESPACE, self.viewer["poeUser"]["id"]))
         except KeyError as e:
             raise ValueError(
                 "Failed to extract 'viewer' or 'user_id' from 'next_data'."
             ) from e
 
-        # """extract formkey from response html"""
-        # # by @aditiaryan and @ading2210
-        # try:
-        #     self.formkey = extract_formkey(text)
-        #     self.headers["poe-formkey"] = self.formkey
-        # except Exception as e:
-        #     raise ValueError(
-        #         "Failed to extract 'formkey' from the response text."
-        #     ) from e
-
     async def get_channel_data(self) -> None:
         """
         This function fetches the channel data from the SETTING_URL and sets the 'tchanneldata' attribute of the object.
 
         Raises:
             Raises a ValueError if it fails to extract the channel data from the response.
         """
         try:
             async with aiohttp.ClientSession(**self.session_args) as client:
                 response = await client.get(SETTING_URL)
                 data = await response.text()
                 json_data = json.loads(data)
                 self.tchannel_data = json_data["tchannelData"]
                 self.headers["Poe-Tchannel"] = self.tchannel_data["channel"]
+                self.channel_url = f'https://{self.ws_domain}.tch.{self.tchannel_data["baseHost"]}/up/{self.tchannel_data["boxName"]}/updates?min_seq={self.tchannel_data["minSeq"]}&channel={self.tchannel_data["channel"]}&hash={self.tchannel_data["channelHash"]}'
         except Exception as e:
             raise ValueError("Failed to extract tchannel from response.") from e
 
-    def get_websocket_url(self, channel=None) -> str:
-        """
-        This function generates and returns the WebSocket URL.
-
-        Args:
-            channel (dict): The channel data. If None, uses the 'tchanneldata' attribute of the object.
-
-        Returns:
-            Returns the WebSocket URL as a string.
-        """
-        if channel is None:
-            channel = self.tchannel_data
-        query = f'?min_seq={channel["minSeq"]}&channel={channel["channel"]}&hash={channel["channelHash"]}'
-        return (
-                f'wss://{self.ws_domain}.tch.{channel["baseHost"]}/up/{channel["boxName"]}/updates'
-                + query
-        )
-
     async def create(self):
         """
         This function initializes the Async_Poe_Client instance by fetching the base data, channel data, and bot data,
         and then subscribing to the channel.
 
         Returns:
             Returns the initialized instance of the Async_Poe_Client.
@@ -237,15 +211,17 @@
         try:
             async with aiohttp.ClientSession(**self.session_args) as client:
                 response = await client.get(url, timeout=3)
                 data = await response.text()
                 bot_info = json.loads(data)
                 return bot_info["pageProps"]
         except Exception as e:
-            raise ValueError(f"Failed to get bot info from {url}. Make sure the bot is not deleted") from e
+            raise ValueError(
+                f"Failed to get bot info from {url}. Make sure the bot is not deleted"
+            ) from e
 
     async def save_botdata(self, url_botname: str) -> None:
         """
         This function saves the bot's chat data for later use.
 
         Args:
             url_botname (str): The name of the bot used in the URL to fetch the bot's chat data.
@@ -273,15 +249,15 @@
         tasks = []
         for bot in self.home_bot_list:
             task = asyncio.create_task(self.save_botdata(bot))
             tasks.append(task)
 
         await asyncio.gather(*tasks)
 
-    async def send_query(self, query_name: str, variables: dict) -> Any | None:
+    async def send_query(self, query_name: str, variables: dict) -> Union[dict, None]:
         """
         A general-purpose function used to send queries to a server. This function is primarily used by other functions in the program.
 
         Args:
             query_name (str): The name of the query that should be sent.
             variables (dict): A dictionary of the variables that should be included in the message.
 
@@ -311,15 +287,19 @@
                         return None
                     else:
                         response = await client.post(
                             GQL_URL, data=data, headers=query_headers
                         )
                     data = await response.text()
                     json_data = json.loads(data)
-                    if "success" in json_data.keys() and not json_data["success"] or json_data["data"] is None:
+                    if (
+                        "success" in json_data.keys()
+                        and not json_data["success"]
+                        or json_data["data"] is None
+                    ):
                         detail_error = Exception(json_data["errors"][0]["message"])
                         raise detail_error
                     return json_data
             except Exception as e:
                 detail_error = e
                 logger.error(
                     f"Failed to sending query:{query_name},error:{detail_error}. (retry: {retry}/5)"
@@ -355,31 +335,31 @@
             logger.info("Succeed to subscribe")
         except Exception as e:
             raise Exception(
                 "Failed to subscribe by sending SubscriptionsMutation"
             ) from e
 
     async def create_bot(
-            self,
-            handle: str,
-            prompt: str,
-            display_name: Optional[str] = None,
-            base_model: str = "chinchilla",
-            description: Optional[str] = "",
-            intro_message: Optional[str] = "",
-            api_key: Optional[str] = None,
-            api_bot: Optional[bool] = False,
-            api_url: Optional[str] = None,
-            prompt_public: Optional[bool] = True,
-            profile_picture_url: Optional[str] = None,
-            linkification: Optional[bool] = False,
-            markdown_rendering: Optional[bool] = True,
-            suggested_replies: Optional[bool] = True,
-            private: Optional[bool] = False,
-            temperature: Optional[int] = None,
+        self,
+        handle: str,
+        prompt: str,
+        display_name: Optional[str] = None,
+        base_model: str = "chinchilla",
+        description: Optional[str] = "",
+        intro_message: Optional[str] = "",
+        api_key: Optional[str] = None,
+        api_bot: Optional[bool] = False,
+        api_url: Optional[str] = None,
+        prompt_public: Optional[bool] = True,
+        profile_picture_url: Optional[str] = None,
+        linkification: Optional[bool] = False,
+        markdown_rendering: Optional[bool] = True,
+        suggested_replies: Optional[bool] = True,
+        private: Optional[bool] = False,
+        temperature: Optional[int] = None,
     ) -> None:
         """
         This function is used to create a new bot with the specified configuration.
 
         Args:
             handle (str): The handle for the new bot which should be unique.
             prompt (str): The prompt for the new bot.
@@ -436,31 +416,31 @@
         # after creating, get the chatId (bot chat_data contains chatId) for using
         # when creating bot,the url_botname equals handle
         logger.info(f"Succeed to create a bot:{handle}")
         await self.save_botdata(url_botname=handle)
         return
 
     async def edit_bot(
-            self,
-            url_botname: str,
-            handle: str = None,
-            prompt: Optional[str] = None,
-            display_name=None,
-            base_model="chinchilla",
-            description="",
-            intro_message="",
-            api_key=None,
-            api_url=None,
-            is_private_bot=None,
-            prompt_public=None,
-            profile_picture_url=None,
-            linkification=None,
-            markdown_rendering=None,
-            suggested_replies=None,
-            temperature=None,
+        self,
+        url_botname: str,
+        handle: str = None,
+        prompt: Optional[str] = None,
+        display_name=None,
+        base_model="chinchilla",
+        description="",
+        intro_message="",
+        api_key=None,
+        api_url=None,
+        is_private_bot=None,
+        prompt_public=None,
+        profile_picture_url=None,
+        linkification=None,
+        markdown_rendering=None,
+        suggested_replies=None,
+        temperature=None,
     ) -> None:
         """
         This function is used to edit the configuration of an existing bot.
 
         Args:
             url_botname (str): The URL name of the bot to be edited.
             handle (str, optional): The new handle for the bot. If not provided, it will remain unchanged.
@@ -504,27 +484,25 @@
                 "introduction": intro_message or botinfo["introduction"],
                 "description": description or botinfo["description"],
                 "profilePictureUrl": profile_picture_url or botinfo["profilePicture"],
                 "apiUrl": api_url or botinfo["apiUrl"],
                 "apiKey": api_key or botinfo["apiKey"],
                 "hasLinkification": linkification or botinfo["hasLinkification"],
                 "hasMarkdownRendering": markdown_rendering
-                                        or botinfo["hasMarkdownRendering"],
+                or botinfo["hasMarkdownRendering"],
                 "hasSuggestedReplies": suggested_replies
-                                       or botinfo["hasSuggestedReplies"],
+                or botinfo["hasSuggestedReplies"],
                 "isPrivateBot": is_private_bot or botinfo["isPrivateBot"],
                 "temperature": temperature or botinfo["temperature"],
             },
         )
 
         data = result["data"]["poeBotEdit"]
         if data["status"] != "success":
-            raise RuntimeError(
-                f"Failed to create a bot: {data['status']}"
-            )
+            raise RuntimeError(f"Failed to create a bot: {data['status']}")
         logger.info(f"Succeed to edit {url_botname}")
         return data
 
     async def delete_bot(self, url_botname: str) -> None:
         """
         This function is used to edit the configuration of an existing bot.
 
@@ -554,15 +532,15 @@
         if response["data"] is None and response["errors"]:
             raise ValueError(
                 f"Failed to delete bot {url_botname} :{response['errors'][0]['message']}"  # noqa: E501
             )
         logger.info(f"Succeed to delete bot {url_botname}")
 
     async def explore_bots(
-            self, count: int = 50, explore_all: bool = False
+        self, count: int = 50, explore_all: bool = False
     ) -> List[dict]:
         """
         Asynchronously explore and fetch a specified number of third party bots.
 
         Args:
             count (int, optional): The number of bots to explore. Defaults to 50.
             explore_all (bool, optional): Whether to explore all third party bots. Defaults to False
@@ -604,15 +582,15 @@
                 for each in result["data"]["exploreBotsConnection"]["edges"]
             ]
             bots += new_bots
         logger.info("Succeed to explore bots")
         return bots[:count]
 
     async def send_message(
-            self, url_botname: str, question: str, with_chat_break: bool = False
+        self, url_botname: str, question: str, with_chat_break: bool = False
     ) -> int:
         """
         Sends a message to a specified bot and retrieves the message ID of the sent message.
 
         Parameters:
             url_botname (str): The unique identifier of the bot to which the message is to be sent.
             question (str): The message to be sent to the bot.
@@ -656,19 +634,19 @@
             return human_message_id
         except TypeError:
             raise RuntimeError(
                 "Failed to extract human_message and human_message_id from response when asking: Unknown Error"
             )
 
     async def send_recv(
-            self,
-            url_botname: str,
-            last_text: str,
-            bot_message_id: str,
-            human_message_id: int,
+        self,
+        url_botname: str,
+        last_text: str,
+        bot_message_id: str,
+        human_message_id: int,
     ) -> None:
         """
         A function to mimic the behavior of a human user interacting with a webpage.
 
         Parameters:
             url_botname (str): The unique identifier of the bot involved in the interaction.
             last_text (str): The last message text received from the bot.
@@ -699,18 +677,18 @@
                 "bot_message_id": bot_message_id,
                 "chat_id": self.bots[url_botname]["chatId"],
                 "bot_response_status": "success",
             },
         )
 
     async def ask(
-            self,
-            url_botname: str,
-            question: str,
-            with_chat_break: bool = False,
+        self,
+        url_botname: str,
+        question: str,
+        with_chat_break: bool = False,
     ) -> str:
         """
         Sends a question to a specified bot and retrieves the bot's response via HTTP.
 
         Parameters:
             url_botname (str): The unique identifier of the bot to which the question is to be sent.
             question (str): The question to be sent to the bot.
@@ -760,98 +738,129 @@
             except Exception as e:
                 logger.error(
                     f"Failed to getting message from {url_botname}, error:{str(e)}"
                 )
         raise ValueError(f"Failed to getting message from {url_botname} too many times")
 
     async def ask_stream(
-            self,
-            url_botname: str,
-            question: str,
-            with_chat_break: bool = False,
-            suggest_able: bool = True,
+        self,
+        url_botname: str,
+        question: str,
+        with_chat_break: bool = False,
+        suggest_able: bool = True,
     ) -> AsyncGenerator:
         """
         Asynchronously sends a question to a specified bot and yields the bot's responses as they arrive.
 
         Args:
             url_botname (str): The unique identifier of the bot to which the question is to be sent.
             question (str): The question to be sent to the bot.
             with_chat_break (bool, optional): If set to True, a chat break will be sent before the question, clearing the bot's conversation memory. Default is False.
             suggest_able (bool, optional): If set to True, suggested replies from the bot will be included in the responses. Default is False.
 
         Returns:
             AsyncGenerator[str]: An asynchronous generator that yields the bot's responses as they arrive.
 
         Raises:
-            Exception: If there is a failure in receiving messages from the bot through websockets.
-
-        Note:
-            This function opens a websocket connection to the bot, sends the question, and then listens for responses. It should be used within an 'async for' loop.
+            Exception: If there is a failure in receiving messages from the bots.
 
         """
-        ua = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36 Edg/117.0.0.0'
-        async with aiohttp.ClientSession(headers={'User-Agent': ua}) as session:
-            async with session.ws_connect(self.get_websocket_url(), timeout=3, proxy=self.proxy) as ws:
-                await self.subscribe()
-                human_message_id = await self.send_message(
-                    url_botname, question, with_chat_break
-                )
-                last_text = ""
-                message = None
-                yield_header = False
-                suggestion_list = []
-                retry = 5
-                while retry >= 0:
-                    try:
-                        raw_data = await ws.receive_json()
-                        if "messages" not in raw_data:
-                            retry -= 1
-                            if retry == 0:
-                                raise Exception("Failed to get answer form poe too many times.")
-                            continue
-                        message = json.loads(raw_data["messages"][-1])["payload"]["data"]["messageAdded"]  # noqa: E501
-                        if message["messageId"] > human_message_id:
-                            plain_text = message["text"][len(last_text):]
-                            last_text = message["text"]
-                            if (
-                                    self.bots[url_botname]["defaultBotObject"][
-                                        "hasSuggestedReplies"
-                                    ]
-                                    and suggest_able
-                            ):
-                                suggestion_num = len(message["suggestedReplies"])
-                                if 0 < suggestion_num < 3:
-                                    if not yield_header:
-                                        yield_header = True
-                                        yield "\n\nSuggested Reply:"
-                                    suggestion_list.append(message['suggestedReplies'][-1])
-                                    yield f"\n{str(suggestion_num)}:{message['suggestedReplies'][-1]}"
-                                elif suggestion_num >= 3:
-                                    suggestion_list.append(message['suggestedReplies'][-1])
-                                    self.bots[url_botname]["Suggestion"] = suggestion_list
-                                    yield f"\n{str(suggestion_num)}:{message['suggestedReplies'][-1]}"
+        async with aiohttp.ClientSession(**self.session_args) as client:
+            human_message_id = await self.send_message(
+                url_botname, question, with_chat_break
+            )
+            last_text = ""
+            yield_header = False
+            suggestion_list = []
+            self.bots[url_botname]["Suggestion"] = []
+            retry = 5
+            suggestion_lost = 5
+            while retry >= 0:
+                try:
+                    response = await client.get(self.channel_url)
+                    raw_data = await response.json()
+                    if "messages" not in raw_data:
+                        retry -= 1
+                        if retry == 0:
+                            raise Exception(
+                                "Failed to get answer form poe too many times:No Reply!"
+                            )
+                        continue
+                    message = json.loads(raw_data["messages"][-1])["payload"]["data"][
+                        "messageAdded"
+                    ]  # noqa: E501
+                    if message["messageId"] > human_message_id:
+                        plain_text = message["text"][len(last_text) :]
+                        last_text = message["text"]
+                        if (
+                            self.bots[url_botname]["defaultBotObject"][
+                                "hasSuggestedReplies"
+                            ]
+                            and suggest_able
+                            and message["state"] == "complete"
+                        ):
+                            if len(message["suggestedReplies"]) == 0:
+                                suggestion_lost -= 1
+                                if suggestion_lost <= 0:
+                                    logger.error(
+                                        "Failed to get suggestions:Poe didn't send suggestions"
+                                    )
                                     break
-                                else:
-                                    yield plain_text
+                            if 0 < len(message["suggestedReplies"]) < 3:
+                                if len(message["suggestedReplies"]) == len(
+                                    suggestion_list
+                                ):
+                                    suggestion_lost -= 1
+                                    if suggestion_lost <= 0:
+                                        logger.error(
+                                            "Failed to get suggestions:Poe didn't send enough suggestions"
+                                        )
+                                        break
+                                if not yield_header:
+                                    yield_header = True
+                                    yield "\n\nSuggested Reply:"
+                                for suggest in message["suggestedReplies"]:
+                                    if suggest not in suggestion_list:
+                                        suggestion_list.append(
+                                            message["suggestedReplies"][-1]
+                                        )
+                                        yield f"\n{str(len(message['suggestedReplies']))}:{message['suggestedReplies'][-1]}"  # noqa: E501
+                            elif len(message["suggestedReplies"]) >= 3:
+                                suggestion_list.append(message["suggestedReplies"][-1])
+                                self.bots[url_botname]["Suggestion"] = suggestion_list
+                                yield f"\n{str(len(message['suggestedReplies']))}:{message['suggestedReplies'][-1]}"
+                                break
                             else:
-                                if message["state"] == "complete":
-                                    yield plain_text
-                                    break
-                                else:
-                                    yield plain_text
-                    except asyncio.exceptions.TimeoutError as e:
-                        raise Exception(f"Failed to get message from {url_botname} through websocket:{str(e)}") from e
-                    except Exception as e:
-                        raise Exception(
-                            f"Failed to get message from {url_botname} through websocket:{str(e)}"
-                        ) from e
-                await self.send_recv(
-                    url_botname, last_text, message["messageId"], human_message_id
-                )
+                                yield plain_text
+                        else:
+                            if message["state"] == "complete":
+                                yield plain_text
+                                break
+                            else:
+                                yield plain_text
+                    else:
+                        retry -= 1
+                        if retry == 0:
+                            if retry == 0:
+                                raise Exception(
+                                    "Failed to get answer form poe too many times."
+                                )
+                            continue
+                except asyncio.exceptions.TimeoutError as e:
+                    raise Exception(
+                        f"Failed to get message from {url_botname}:{str(e)}"
+                    ) from e
+                except Exception as e:
+                    raise Exception(
+                        f"Failed to get message from {url_botname}:{str(e)}"
+                    ) from e
+            await self.send_recv(
+                url_botname, last_text, message["messageId"], human_message_id
+            )
+            return
 
     async def send_chat_break(self, url_botname: str) -> None:
         """
         Asynchronously sends a chat break to a specified bot, effectively clearing the bot's conversation memory.
 
         Parameters:
             url_botname (str): The unique identifier of the bot to which the chat break is to be sent.
@@ -864,17 +873,15 @@
 
         """
         if url_botname not in self.bots.keys():
             self.bots[url_botname] = await self.get_botdata(url_botname)
         await self.send_query(
             "AddMessageBreakMutation", {"chatId": self.bots[url_botname]["chatId"]}
         )
-        logger.info(
-            f'Succeed to chat break to {url_botname}'
-        )
+        logger.info(f"Succeed to chat break to {url_botname}")
         return
 
     async def delete_messages(self, message_ids: Union[list, int]):
         """
         Asynchronously deletes messages based on provided message IDs.
 
         Parameters:
@@ -893,15 +900,15 @@
         if isinstance(message_ids, int):
             message_ids = [int(message_ids)]
 
         await self.send_query("DeleteMessageMutation", {"messageIds": message_ids})
         logger.info(f"Succeed to deleting messages: {message_ids}")
 
     async def get_message_history(
-            self, url_botname, count: Optional[int] = None, get_all: Optional[bool] = False
+        self, url_botname, count: Optional[int] = None, get_all: Optional[bool] = False
     ):
         """
         Asynchronously fetches the message history for a specified bot.
 
         Parameters:
             url_botname (str): The url name of the bot whose message history is to be fetched.
             count (int, optional): The number of most recent messages to fetch. If not provided, either 'get_all' must be set to True or else a TypeError will be raised.
@@ -947,18 +954,18 @@
         logger.info(f"Succeed to get messages from {url_botname}")
         if count:
             return messages[-count:]
         else:
             return messages
 
     async def delete_bot_conversation(
-            self,
-            url_botname: str,
-            count: Optional[int] = None,
-            del_all: Optional[bool] = False,
+        self,
+        url_botname: str,
+        count: Optional[int] = None,
+        del_all: Optional[bool] = False,
     ):
         """
         Deletes the conversation history with the specified bot.
 
         Args:
             url_botname (str): The url name of the bot to delete the conversation history for.
             count (int, optional): The number of messages to delete. If not provided, all messages will be deleted.
@@ -981,15 +988,15 @@
                 "Please provide at least one of the following parameters: del_all=<bool>, count=<int>"
             )
         message_ids = [message["node"]["messageId"] for message in messages]
         await self.delete_messages(message_ids)
         logger.info(f"Succeed to delete {arg} messages with {url_botname}")
 
     async def get_available_bots(
-            self, count: Optional[int] = 25, get_all: Optional[bool] = False
+        self, count: Optional[int] = 25, get_all: Optional[bool] = False
     ) -> List[dict]:  # noqa: E501
         """
         Get own available bots .
 
         Args:
             count (int, optional): The number of bots to get.
             get_all (bool, optional): Whether to get all bots.
@@ -1036,15 +1043,15 @@
                 else:
                     logger.info("Succeed to get all available bots")
                 return bots
         logger.info("Succeed to get available bots")
         return bots[:count]
 
     async def delete_available_bots(
-            self, count: Optional[int] = 2, del_all: Optional[bool] = False
+        self, count: Optional[int] = 2, del_all: Optional[bool] = False
     ):
         """
         Asynchronously deletes some or all user available bots.
 
         Args:
             count (int, optional): The number of bots to delete.
             del_all (bool, optional): Whether to delete all bots.
@@ -1064,15 +1071,17 @@
             )
         bots = await self.get_available_bots(count, del_all)
         for bot in bots:
             if not bot["isSystemBot"]:
                 try:
                     await self.delete_bot(bot["handle"])
                 except Exception as e:
-                    logger.error(f"Failed to delete {bot['handle']} : {str(e)}. Make sure the bot belong to you.")
+                    logger.error(
+                        f"Failed to delete {bot['handle']} : {str(e)}. Make sure the bot belong to you."
+                    )
             else:
                 logger.info("Can't delete SystemBot, skipped")
         logger.info("Succeed to delete bots")
 
     async def delete_all_conversations(self):
         """
         Asynchronously deletes all user messages in the conversations.
```

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/ChatPaginationQuery.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/MessageAddedSubscription.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/PoeBotEditMutation.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/PoeBotEditMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/SendMessageMutation.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/ViewerStateFragment.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/async_poe_client/util.py` & `async_poe_client-0.1.9/async_poe_client/util.py`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/README.md` & `async_poe_client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.8/PKG-INFO` & `async_poe_client-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-poe-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: A stable, fast and convenient async client for poe.com
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

