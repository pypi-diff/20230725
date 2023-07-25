# Comparing `tmp/async_poe_client-0.1.9.tar.gz` & `tmp/async_poe_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_poe_client-0.1.9.tar", max compression
+gzip compressed data, was "async_poe_client-0.2.0.tar", max compression
```

## Comparing `async_poe_client-0.1.9.tar` & `async_poe_client-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.1.9/async_poe_client/__init__.py
--rw-r--r--   0        0        0    48716 2023-07-25 01:15:45.644096 async_poe_client-0.1.9/async_poe_client/client.py
--rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.1.9/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.1.9/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.1.9/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.1.9/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
--rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.1.9/async_poe_client/poe_graphql/BioFragment.graphql
--rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.1.9/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
--rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatFragment.graphql
--rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.1.9/async_poe_client/poe_graphql/HandleFragment.graphql
--rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageFragment.graphql
--rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.1.9/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.1.9/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.1.9/async_poe_client/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.1.9/async_poe_client/requirements.txt
--rw-r--r--   0        0        0     1648 2023-07-24 06:33:37.590357 async_poe_client-0.1.9/async_poe_client/util.py
--rw-r--r--   0        0        0      445 2023-07-25 01:17:52.886038 async_poe_client-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    16836 2023-07-24 06:32:46.931339 async_poe_client-0.1.9/README.md
--rw-r--r--   0        0        0    17088 1970-01-01 00:00:00.000000 async_poe_client-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-07-22 14:46:24.800780 async_poe_client-0.2.0/async_poe_client/__init__.py
+-rw-r--r--   0        0        0    48782 2023-07-25 06:32:25.199349 async_poe_client-0.2.0/async_poe_client/client.py
+-rw-r--r--   0        0        0     1145 2023-07-19 06:18:30.461961 async_poe_client-0.2.0/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-07-19 06:18:30.461961 async_poe_client-0.2.0/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-07-19 06:18:30.461961 async_poe_client-0.2.0/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      701 2023-07-22 07:43:55.501987 async_poe_client-0.2.0/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
+-rw-r--r--   0        0        0      105 2023-07-19 06:18:30.461961 async_poe_client-0.2.0/async_poe_client/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0      169 2023-07-22 05:55:18.261809 async_poe_client-0.2.0/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
+-rw-r--r--   0        0        0       78 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-07-19 06:18:30.462960 async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-07-19 06:18:30.463987 async_poe_client-0.2.0/async_poe_client/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-07-19 06:18:30.464960 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-07-19 06:18:30.465959 async_poe_client-0.2.0/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-07-19 06:18:30.466959 async_poe_client-0.2.0/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-07-19 06:18:30.467959 async_poe_client-0.2.0/async_poe_client/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-07-19 06:18:30.467959 async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-07-19 06:18:30.467959 async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-07-19 06:18:30.467959 async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       53 2023-07-23 07:11:13.271223 async_poe_client-0.2.0/async_poe_client/requirements.txt
+-rw-r--r--   0        0        0     2459 2023-07-25 06:17:58.542713 async_poe_client-0.2.0/async_poe_client/util.py
+-rw-r--r--   0        0        0      467 2023-07-25 06:40:16.211595 async_poe_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17252 2023-07-25 06:41:01.974440 async_poe_client-0.2.0/README.md
+-rw-r--r--   0        0        0    17538 1970-01-01 00:00:00.000000 async_poe_client-0.2.0/PKG-INFO
```

### Comparing `async_poe_client-0.1.9/async_poe_client/client.py` & `async_poe_client-0.2.0/async_poe_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,22 @@
     GQL_URL,
     GQL_RECV_URL,
     SETTING_URL,
     CONST_NAMESPACE,
     generate_data,
     QUERIES,
     generate_nonce,
+    extract_formkey,
 )
 
-Last_Use_Time = time.time()
-
 
 class Poe_Client:
-    def __init__(self, p_b: str, formkey: str, proxy: str = ""):
+    def __init__(
+        self, p_b: str, formkey: Optional[str] = "", proxy: Optional[str] = ""
+    ):
         self.channel_url: str = ""
         self.bots: dict = {}
         self.bot_list_url: str = ""
         self.formkey: str = formkey
         self.home_bot_list: List[str] = []
         self.next_data: dict = {}
         self.p_b: str = p_b
@@ -38,29 +39,24 @@
         self.subscription: dict = {}
         self.tchannel_data: dict = {}
         self.user_id: str = ""
         self.viewer: dict = {}
         self.ws_domain = f"tch{random.randint(1, int(1e6))}"[:8]
         self.proxy = proxy
         self.headers = {
-            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
             "Accept-Encoding": "gzip, deflate, br",
-            "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6",
-            "Cache-Control": "max-age=0",
-            "Cookie": f"p-b={self.p_b}; SL_G_WPT_TO=zh-CN; SL_GWPT_Show_Hide_tmp=1; SL_wptGlobTipTmp=1;",
+            "Accept-Language": "en-US,en;q=0.9",
+            "Cookie": f"p-b={self.p_b}",
             "poe-formkey": self.formkey,
-            "Sec-Ch-Ua": '"Microsoft Edge";v="117", "Not;A Brand";v="8", "Chromium";v="117"',
+            "Sec-Ch-Ua": '"Not.A/Brand";v="8", "Chromium";v="112"',
             "Sec-Ch-Ua-Mobile": "?0",
-            "Sec-Ch-Ua-Platform": '"Windows"',
-            "Sec-Fetch-Dest": "document",
-            "Sec-Fetch-Mode": "navigate",
-            "Sec-Fetch-Site": "same-origin",
-            "Sec-Fetch-User": "?1",
+            "Sec-Ch-Ua-Platform": '"Linux"',
             "Upgrade-Insecure-Requests": "1",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/117.0.0.0 Safari/537.36 Edg/117.0.0.0",
         }
 
     @property
     def session_args(self):
         args = {
             "headers": self.headers,
             "cookies": {"p-b": self.p_b},
@@ -106,14 +102,23 @@
             for bot in bot_list:
                 self.home_bot_list.append(bot["node"]["handle"])
             self.sdid = str(uuid.uuid5(CONST_NAMESPACE, self.viewer["poeUser"]["id"]))
         except KeyError as e:
             raise ValueError(
                 "Failed to extract 'viewer' or 'user_id' from 'next_data'."
             ) from e
+        if not self.formkey:
+            if not self.formkey:
+                script_url_regex = r'src="(https://psc2\.cf2\.poecdn\.net/[a-f0-9]{40}/_next/static/chunks/pages/_app-[a-f0-9]{16}\.js)"'
+                script_url = re.search(script_url_regex, text).group(1)
+                async with aiohttp.ClientSession(**self.session_args) as client:
+                    response = await client.get(script_url)
+                    script_text = await response.text()
+            self.formkey = extract_formkey(text, script_text)
+            self.headers["poe-formkey"] = self.formkey
 
     async def get_channel_data(self) -> None:
         """
         This function fetches the channel data from the SETTING_URL and sets the 'tchanneldata' attribute of the object.
 
         Raises:
             Raises a ValueError if it fails to extract the channel data from the response.
@@ -145,25 +150,15 @@
             try:
                 await self.get_basedata()
                 break
             except Exception as e:
                 retry -= 1
                 if retry == 0:
                     raise e
-        retry = 3
-        while retry >= 0:
-            try:
-                await self.get_channel_data()
-                break
-            except Exception as e:
-                retry -= 1
-                if retry == 0:
-                    raise e
         await self.get_bots()
-        await self.subscribe()
         logger.info("Succeed to create async_poe_client instance")
         return self
 
     async def get_botdata(self, url_botname: str) -> dict:
         """
         This function gets the chat data of the bot from the specified URL.
 
@@ -697,15 +692,15 @@
         Returns:
             Union[str, dict]: The bot's response. This will be a string if 'plain' is True, else it will be a dictionary.
 
         Raises:
             ValueError: If there's a timeout or failure in receiving the message from the bot.
 
         Note:
-            This function uses HTTPX to send and receive messages. It doesn't support streaming and is not recommended if 'ask_stream' can be used.
+            This function uses AIOHTTP to send and receive messages. It doesn't support streaming and is not recommended if 'ask_stream' can be used.
 
         """
         await self.subscribe()
         human_message_id = await self.send_message(
             url_botname, question, with_chat_break
         )
         retry = 3
@@ -761,14 +756,16 @@
             AsyncGenerator[str]: An asynchronous generator that yields the bot's responses as they arrive.
 
         Raises:
             Exception: If there is a failure in receiving messages from the bots.
 
         """
         async with aiohttp.ClientSession(**self.session_args) as client:
+            await self.get_channel_data()
+            await self.subscribe()
             human_message_id = await self.send_message(
                 url_botname, question, with_chat_break
             )
             last_text = ""
             yield_header = False
             suggestion_list = []
             self.bots[url_botname]["Suggestion"] = []
```

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/ChatPaginationQuery.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/MessageAddedSubscription.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/PoeBotEditMutation.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/PoeBotEditMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/SendMessageMutation.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerStateFragment.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `async_poe_client-0.2.0/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `async_poe_client-0.1.9/async_poe_client/util.py` & `async_poe_client-0.2.0/async_poe_client/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,103 +1,154 @@
 00000000: 696d 706f 7274 206a 736f 6e0d 0a69 6d70  import json..imp
 00000010: 6f72 7420 7261 6e64 6f6d 0d0a 696d 706f  ort random..impo
-00000020: 7274 2073 6563 7265 7473 0d0a 696d 706f  rt secrets..impo
-00000030: 7274 2075 7569 640d 0a66 726f 6d20 7061  rt uuid..from pa
-00000040: 7468 6c69 6220 696d 706f 7274 2050 6174  thlib import Pat
-00000050: 680d 0a0d 0a43 4f4e 5354 5f4e 414d 4553  h....CONST_NAMES
-00000060: 5041 4345 203d 2075 7569 642e 5555 4944  PACE = uuid.UUID
-00000070: 2822 3132 3334 3536 3738 3132 3334 3536  ("12345678123456
-00000080: 3738 3132 3334 3536 3738 3132 3334 3536  7812345678123456
-00000090: 3738 2229 0d0a 0d0a 5155 4552 4945 5320  78")....QUERIES 
-000000a0: 3d20 7b7d 0d0a 4751 4c5f 5552 4c20 3d20  = {}..GQL_URL = 
-000000b0: 2268 7474 7073 3a2f 2f70 6f65 2e63 6f6d  "https://poe.com
-000000c0: 2f61 7069 2f67 716c 5f50 4f53 5422 0d0a  /api/gql_POST"..
-000000d0: 4751 4c5f 5245 4356 5f55 524c 203d 2022  GQL_RECV_URL = "
-000000e0: 6874 7470 733a 2f2f 706f 652e 636f 6d2f  https://poe.com/
-000000f0: 6170 692f 7265 6365 6976 655f 504f 5354  api/receive_POST
-00000100: 220d 0a48 4f4d 455f 5552 4c20 3d20 2268  "..HOME_URL = "h
-00000110: 7474 7073 3a2f 2f70 6f65 2e63 6f6d 220d  ttps://poe.com".
-00000120: 0a53 4554 5449 4e47 5f55 524c 203d 2022  .SETTING_URL = "
-00000130: 6874 7470 733a 2f2f 706f 652e 636f 6d2f  https://poe.com/
-00000140: 6170 692f 7365 7474 696e 6773 220d 0a0d  api/settings"...
-00000150: 0a71 7565 7269 6573 5f70 6174 6820 3d20  .queries_path = 
-00000160: 5061 7468 285f 5f66 696c 655f 5f29 2e72  Path(__file__).r
-00000170: 6573 6f6c 7665 2829 2e70 6172 656e 7420  esolve().parent 
-00000180: 2f20 2270 6f65 5f67 7261 7068 716c 220d  / "poe_graphql".
-00000190: 0a0d 0a0d 0a64 6566 2067 656e 6572 6174  .....def generat
-000001a0: 655f 6461 7461 2871 7565 7279 5f6e 616d  e_data(query_nam
-000001b0: 652c 2076 6172 6961 626c 6573 2920 2d3e  e, variables) ->
-000001c0: 2073 7472 3a0d 0a20 2020 2069 6620 7175   str:..    if qu
-000001d0: 6572 795f 6e61 6d65 203d 3d20 2272 6563  ery_name == "rec
-000001e0: 7622 3a0d 0a20 2020 2020 2020 2064 6174  v":..        dat
-000001f0: 6120 3d20 5b0d 0a20 2020 2020 2020 2020  a = [..         
-00000200: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
-00000210: 2020 2020 2020 2263 6174 6567 6f72 7922        "category"
-00000220: 3a20 2270 6f65 2f62 6f74 5f72 6573 706f  : "poe/bot_respo
-00000230: 6e73 655f 7370 6565 6422 2c0d 0a20 2020  nse_speed",..   
-00000240: 2020 2020 2020 2020 2020 2020 2022 6461               "da
-00000250: 7461 223a 2076 6172 6961 626c 6573 2c0d  ta": variables,.
-00000260: 0a20 2020 2020 2020 2020 2020 207d 0d0a  .            }..
-00000270: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
-00000280: 2020 2069 6620 7261 6e64 6f6d 2e72 616e     if random.ran
-00000290: 646f 6d28 2920 3e20 302e 393a 0d0a 2020  dom() > 0.9:..  
-000002a0: 2020 2020 2020 2020 2020 6461 7461 2e61            data.a
-000002b0: 7070 656e 6428 0d0a 2020 2020 2020 2020  ppend(..        
-000002c0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-000002d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000002e0: 6361 7465 676f 7279 223a 2022 706f 652f  category": "poe/
-000002f0: 7374 6174 7364 5f65 7665 6e74 222c 0d0a  statsd_event",..
-00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000310: 2020 2020 2264 6174 6122 3a20 7b0d 0a20      "data": {.. 
+00000020: 7274 2072 650d 0a69 6d70 6f72 7420 7365  rt re..import se
+00000030: 6372 6574 730d 0a69 6d70 6f72 7420 7575  crets..import uu
+00000040: 6964 0d0a 6672 6f6d 2070 6174 686c 6962  id..from pathlib
+00000050: 2069 6d70 6f72 7420 5061 7468 0d0a 0d0a   import Path....
+00000060: 696d 706f 7274 2065 7865 636a 730d 0a0d  import execjs...
+00000070: 0a43 4f4e 5354 5f4e 414d 4553 5041 4345  .CONST_NAMESPACE
+00000080: 203d 2075 7569 642e 5555 4944 2822 3132   = uuid.UUID("12
+00000090: 3334 3536 3738 3132 3334 3536 3738 3132  3456781234567812
+000000a0: 3334 3536 3738 3132 3334 3536 3738 2229  34567812345678")
+000000b0: 0d0a 0d0a 5155 4552 4945 5320 3d20 7b7d  ....QUERIES = {}
+000000c0: 0d0a 4751 4c5f 5552 4c20 3d20 2268 7474  ..GQL_URL = "htt
+000000d0: 7073 3a2f 2f70 6f65 2e63 6f6d 2f61 7069  ps://poe.com/api
+000000e0: 2f67 716c 5f50 4f53 5422 0d0a 4751 4c5f  /gql_POST"..GQL_
+000000f0: 5245 4356 5f55 524c 203d 2022 6874 7470  RECV_URL = "http
+00000100: 733a 2f2f 706f 652e 636f 6d2f 6170 692f  s://poe.com/api/
+00000110: 7265 6365 6976 655f 504f 5354 220d 0a48  receive_POST"..H
+00000120: 4f4d 455f 5552 4c20 3d20 2268 7474 7073  OME_URL = "https
+00000130: 3a2f 2f70 6f65 2e63 6f6d 220d 0a53 4554  ://poe.com"..SET
+00000140: 5449 4e47 5f55 524c 203d 2022 6874 7470  TING_URL = "http
+00000150: 733a 2f2f 706f 652e 636f 6d2f 6170 692f  s://poe.com/api/
+00000160: 7365 7474 696e 6773 220d 0a0d 0a71 7565  settings"....que
+00000170: 7269 6573 5f70 6174 6820 3d20 5061 7468  ries_path = Path
+00000180: 285f 5f66 696c 655f 5f29 2e72 6573 6f6c  (__file__).resol
+00000190: 7665 2829 2e70 6172 656e 7420 2f20 2270  ve().parent / "p
+000001a0: 6f65 5f67 7261 7068 716c 220d 0a0d 0a0d  oe_graphql".....
+000001b0: 0a64 6566 2067 656e 6572 6174 655f 6461  .def generate_da
+000001c0: 7461 2871 7565 7279 5f6e 616d 652c 2076  ta(query_name, v
+000001d0: 6172 6961 626c 6573 2920 2d3e 2073 7472  ariables) -> str
+000001e0: 3a0d 0a20 2020 2069 6620 7175 6572 795f  :..    if query_
+000001f0: 6e61 6d65 203d 3d20 2272 6563 7622 3a0d  name == "recv":.
+00000200: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+00000210: 5b0d 0a20 2020 2020 2020 2020 2020 207b  [..            {
+00000220: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000230: 2020 2263 6174 6567 6f72 7922 3a20 2270    "category": "p
+00000240: 6f65 2f62 6f74 5f72 6573 706f 6e73 655f  oe/bot_response_
+00000250: 7370 6565 6422 2c0d 0a20 2020 2020 2020  speed",..       
+00000260: 2020 2020 2020 2020 2022 6461 7461 223a           "data":
+00000270: 2076 6172 6961 626c 6573 2c0d 0a20 2020   variables,..   
+00000280: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00000290: 2020 2020 5d0d 0a20 2020 2020 2020 2069      ]..        i
+000002a0: 6620 7261 6e64 6f6d 2e72 616e 646f 6d28  f random.random(
+000002b0: 2920 3e20 302e 393a 0d0a 2020 2020 2020  ) > 0.9:..      
+000002c0: 2020 2020 2020 6461 7461 2e61 7070 656e        data.appen
+000002d0: 6428 0d0a 2020 2020 2020 2020 2020 2020  d(..            
+000002e0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
+000002f0: 2020 2020 2020 2020 2020 2022 6361 7465             "cate
+00000300: 676f 7279 223a 2022 706f 652f 7374 6174  gory": "poe/stat
+00000310: 7364 5f65 7665 6e74 222c 0d0a 2020 2020  sd_event",..    
 00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000330: 2020 2020 2020 2022 6b65 7922 3a20 2270         "key": "p
-00000340: 6f65 2e73 7065 6564 2e77 6562 5f76 6974  oe.speed.web_vit
-00000350: 616c 732e 494e 5022 2c0d 0a20 2020 2020  als.INP",..     
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 2020 2022 7661 6c75 6522 3a20 7261 6e64     "value": rand
-00000380: 6f6d 2e72 616e 6469 6e74 2831 3030 2c20  om.randint(100, 
-00000390: 3132 3529 2c0d 0a20 2020 2020 2020 2020  125),..         
-000003a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000003b0: 6361 7465 676f 7279 223a 2022 7469 6d65  category": "time
-000003c0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000003d0: 2020 2020 2020 2020 2020 2020 2270 6174              "pat
-000003e0: 6822 3a20 222f 5b68 616e 646c 655d 222c  h": "/[handle]",
-000003f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000400: 2020 2020 2020 2020 2020 2265 7874 7261            "extra
-00000410: 5f64 6174 6122 3a20 7b7d 2c0d 0a20 2020  _data": {},..   
-00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000430: 207d 2c0d 0a20 2020 2020 2020 2020 2020   },..           
-00000440: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00000450: 2020 2020 290d 0a20 2020 2065 6c73 653a      )..    else:
-00000460: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-00000470: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00000480: 2271 7565 7279 223a 2051 5545 5249 4553  "query": QUERIES
-00000490: 5b71 7565 7279 5f6e 616d 655d 2c0d 0a20  [query_name],.. 
-000004a0: 2020 2020 2020 2020 2020 2022 7175 6572             "quer
-000004b0: 794e 616d 6522 3a20 7175 6572 795f 6e61  yName": query_na
-000004c0: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
-000004d0: 2022 7661 7269 6162 6c65 7322 3a20 7661   "variables": va
-000004e0: 7269 6162 6c65 732c 0d0a 2020 2020 2020  riables,..      
-000004f0: 2020 7d0d 0a20 2020 2072 6574 7572 6e20    }..    return 
-00000500: 6a73 6f6e 2e64 756d 7073 2864 6174 612c  json.dumps(data,
-00000510: 2073 6570 6172 6174 6f72 733d 2822 2c22   separators=(","
-00000520: 2c20 223a 2229 290d 0a0d 0a0d 0a64 6566  , ":"))......def
-00000530: 2067 656e 6572 6174 655f 6e6f 6e63 6528   generate_nonce(
-00000540: 6c65 6e67 7468 3a20 696e 7420 3d20 3136  length: int = 16
-00000550: 293a 0d0a 2020 2020 7265 7475 726e 2073  ):..    return s
-00000560: 6563 7265 7473 2e74 6f6b 656e 5f68 6578  ecrets.token_hex
-00000570: 286c 656e 6774 6820 2f2f 2032 290d 0a0d  (length // 2)...
-00000580: 0a0d 0a64 6566 206c 6f61 645f 7175 6572  ...def load_quer
-00000590: 6965 7328 293a 0d0a 2020 2020 676c 6f62  ies():..    glob
-000005a0: 616c 2051 5545 5249 4553 0d0a 2020 2020  al QUERIES..    
-000005b0: 666f 7220 7061 7468 2069 6e20 7175 6572  for path in quer
-000005c0: 6965 735f 7061 7468 2e69 7465 7264 6972  ies_path.iterdir
-000005d0: 2829 3a0d 0a20 2020 2020 2020 2069 6620  ():..        if 
-000005e0: 7061 7468 2e73 7566 6669 7820 213d 2022  path.suffix != "
-000005f0: 2e67 7261 7068 716c 223a 0d0a 2020 2020  .graphql":..    
-00000600: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00000610: 0d0a 2020 2020 2020 2020 7769 7468 206f  ..        with o
-00000620: 7065 6e28 7061 7468 2920 6173 2066 3a0d  pen(path) as f:.
-00000630: 0a20 2020 2020 2020 2020 2020 2051 5545  .            QUE
-00000640: 5249 4553 5b70 6174 682e 7374 656d 5d20  RIES[path.stem] 
-00000650: 3d20 662e 7265 6164 2829 0d0a 0d0a 0d0a  = f.read()......
-00000660: 6c6f 6164 5f71 7565 7269 6573 2829 0d0a  load_queries()..
+00000330: 2264 6174 6122 3a20 7b0d 0a20 2020 2020  "data": {..     
+00000340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000350: 2020 2022 6b65 7922 3a20 2270 6f65 2e73     "key": "poe.s
+00000360: 7065 6564 2e77 6562 5f76 6974 616c 732e  peed.web_vitals.
+00000370: 494e 5022 2c0d 0a20 2020 2020 2020 2020  INP",..         
+00000380: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000390: 7661 6c75 6522 3a20 7261 6e64 6f6d 2e72  value": random.r
+000003a0: 616e 6469 6e74 2831 3030 2c20 3132 3529  andint(100, 125)
+000003b0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+000003c0: 2020 2020 2020 2020 2020 2022 6361 7465             "cate
+000003d0: 676f 7279 223a 2022 7469 6d65 222c 0d0a  gory": "time",..
+000003e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003f0: 2020 2020 2020 2020 2270 6174 6822 3a20          "path": 
+00000400: 222f 5b68 616e 646c 655d 222c 0d0a 2020  "/[handle]",..  
+00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000420: 2020 2020 2020 2265 7874 7261 5f64 6174        "extra_dat
+00000430: 6122 3a20 7b7d 2c0d 0a20 2020 2020 2020  a": {},..       
+00000440: 2020 2020 2020 2020 2020 2020 207d 2c0d               },.
+00000450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000460: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+00000470: 290d 0a20 2020 2065 6c73 653a 0d0a 2020  )..    else:..  
+00000480: 2020 2020 2020 6461 7461 203d 207b 0d0a        data = {..
+00000490: 2020 2020 2020 2020 2020 2020 2271 7565              "que
+000004a0: 7279 223a 2051 5545 5249 4553 5b71 7565  ry": QUERIES[que
+000004b0: 7279 5f6e 616d 655d 2c0d 0a20 2020 2020  ry_name],..     
+000004c0: 2020 2020 2020 2022 7175 6572 794e 616d         "queryNam
+000004d0: 6522 3a20 7175 6572 795f 6e61 6d65 2c0d  e": query_name,.
+000004e0: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
+000004f0: 7269 6162 6c65 7322 3a20 7661 7269 6162  riables": variab
+00000500: 6c65 732c 0d0a 2020 2020 2020 2020 7d0d  les,..        }.
+00000510: 0a20 2020 2072 6574 7572 6e20 6a73 6f6e  .    return json
+00000520: 2e64 756d 7073 2864 6174 612c 2073 6570  .dumps(data, sep
+00000530: 6172 6174 6f72 733d 2822 2c22 2c20 223a  arators=(",", ":
+00000540: 2229 290d 0a0d 0a0d 0a64 6566 2067 656e  "))......def gen
+00000550: 6572 6174 655f 6e6f 6e63 6528 6c65 6e67  erate_nonce(leng
+00000560: 7468 3a20 696e 7420 3d20 3136 293a 0d0a  th: int = 16):..
+00000570: 2020 2020 7265 7475 726e 2073 6563 7265      return secre
+00000580: 7473 2e74 6f6b 656e 5f68 6578 286c 656e  ts.token_hex(len
+00000590: 6774 6820 2f2f 2032 290d 0a0d 0a0d 0a64  gth // 2)......d
+000005a0: 6566 2065 7874 7261 6374 5f66 6f72 6d6b  ef extract_formk
+000005b0: 6579 2868 746d 6c2c 2073 6372 6970 7429  ey(html, script)
+000005c0: 3a0d 0a20 2020 2073 6372 6970 745f 7265  :..    script_re
+000005d0: 6765 7820 3d20 7222 3c73 6372 6970 743e  gex = r"<script>
+000005e0: 282e 2b3f 293c 2f73 6372 6970 743e 220d  (.+?)</script>".
+000005f0: 0a20 2020 2076 6172 735f 7265 6765 7820  .    vars_regex 
+00000600: 3d20 7227 7769 6e64 6f77 5c2e 5f28 5b61  = r'window\._([a
+00000610: 2d7a 412d 5a30 2d39 5d7b 3130 7d29 3d22  -zA-Z0-9]{10})="
+00000620: 285b 612d 7a41 2d5a 302d 395d 7b31 307d  ([a-zA-Z0-9]{10}
+00000630: 2922 270d 0a20 2020 206b 6579 2c20 7661  )"'..    key, va
+00000640: 6c75 6520 3d20 7265 2e66 696e 6461 6c6c  lue = re.findall
+00000650: 2876 6172 735f 7265 6765 782c 2073 6372  (vars_regex, scr
+00000660: 6970 7429 5b30 5d0d 0a0d 0a20 2020 2073  ipt)[0]....    s
+00000670: 6372 6970 745f 7465 7874 203d 2022 2222  cript_text = """
+00000680: 0d0a 2020 2020 2020 6c65 7420 5175 6963  ..      let Quic
+00000690: 6b4a 5320 3d20 756e 6465 6669 6e65 642c  kJS = undefined,
+000006a0: 2070 726f 6365 7373 203d 2075 6e64 6566   process = undef
+000006b0: 696e 6564 3b0d 0a20 2020 2020 206c 6574  ined;..      let
+000006c0: 2077 696e 646f 7720 3d20 7b0d 0a20 2020   window = {..   
+000006d0: 2020 2020 2064 6f63 756d 656e 743a 207b       document: {
+000006e0: 613a 317d 2c0d 0a20 2020 2020 2020 206e  a:1},..        n
+000006f0: 6176 6967 6174 6f72 3a20 7b0d 0a20 2020  avigator: {..   
+00000700: 2020 2020 2020 2075 7365 7241 6765 6e74         userAgent
+00000710: 3a20 2261 220d 0a20 2020 2020 2020 207d  : "a"..        }
+00000720: 0d0a 2020 2020 2020 7d3b 0d0a 2020 2020  ..      };..    
+00000730: 2222 220d 0a20 2020 2073 6372 6970 745f  """..    script_
+00000740: 7465 7874 202b 3d20 6622 7769 6e64 6f77  text += f"window
+00000750: 2e5f 7b6b 6579 7d20 3d20 277b 7661 6c75  ._{key} = '{valu
+00000760: 657d 273b 220d 0a20 2020 2073 6372 6970  e}';"..    scrip
+00000770: 745f 7465 7874 202b 3d20 2222 2e6a 6f69  t_text += "".joi
+00000780: 6e28 7265 2e66 696e 6461 6c6c 2873 6372  n(re.findall(scr
+00000790: 6970 745f 7265 6765 782c 2068 746d 6c29  ipt_regex, html)
+000007a0: 290d 0a0d 0a20 2020 2066 756e 6374 696f  )....    functio
+000007b0: 6e5f 7265 6765 7820 3d20 7222 2877 696e  n_regex = r"(win
+000007c0: 646f 775c 2e5b 612d 7a41 2d5a 302d 395d  dow\.[a-zA-Z0-9]
+000007d0: 7b31 377d 293d 6675 6e63 7469 6f6e 220d  {17})=function".
+000007e0: 0a20 2020 2066 756e 6374 696f 6e5f 7465  .    function_te
+000007f0: 7874 203d 2072 652e 7365 6172 6368 2866  xt = re.search(f
+00000800: 756e 6374 696f 6e5f 7265 6765 782c 2073  unction_regex, s
+00000810: 6372 6970 745f 7465 7874 292e 6772 6f75  cript_text).grou
+00000820: 7028 3129 0d0a 2020 2020 6578 6563 203d  p(1)..    exec =
+00000830: 2066 227b 6675 6e63 7469 6f6e 5f74 6578   f"{function_tex
+00000840: 747d 2829 220d 0a0d 0a20 2020 2063 6f6e  t}()"....    con
+00000850: 7465 7874 203d 2065 7865 636a 732e 636f  text = execjs.co
+00000860: 6d70 696c 6528 7363 7269 7074 5f74 6578  mpile(script_tex
+00000870: 7429 0d0a 2020 2020 666f 726d 6b65 7920  t)..    formkey 
+00000880: 3d20 636f 6e74 6578 742e 6576 616c 2865  = context.eval(e
+00000890: 7865 6329 0d0a 2020 2020 7265 7475 726e  xec)..    return
+000008a0: 2066 6f72 6d6b 6579 0d0a 0d0a 0d0a 6465   formkey......de
+000008b0: 6620 6c6f 6164 5f71 7565 7269 6573 2829  f load_queries()
+000008c0: 3a0d 0a20 2020 2067 6c6f 6261 6c20 5155  :..    global QU
+000008d0: 4552 4945 530d 0a20 2020 2066 6f72 2070  ERIES..    for p
+000008e0: 6174 6820 696e 2071 7565 7269 6573 5f70  ath in queries_p
+000008f0: 6174 682e 6974 6572 6469 7228 293a 0d0a  ath.iterdir():..
+00000900: 2020 2020 2020 2020 6966 2070 6174 682e          if path.
+00000910: 7375 6666 6978 2021 3d20 222e 6772 6170  suffix != ".grap
+00000920: 6871 6c22 3a0d 0a20 2020 2020 2020 2020  hql":..         
+00000930: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
+00000940: 2020 2020 2077 6974 6820 6f70 656e 2870       with open(p
+00000950: 6174 6829 2061 7320 663a 0d0a 2020 2020  ath) as f:..    
+00000960: 2020 2020 2020 2020 5155 4552 4945 535b          QUERIES[
+00000970: 7061 7468 2e73 7465 6d5d 203d 2066 2e72  path.stem] = f.r
+00000980: 6561 6428 290d 0a0d 0a0d 0a6c 6f61 645f  ead()......load_
+00000990: 7175 6572 6965 7328 290d 0a              queries()..
```

### Comparing `async_poe_client-0.1.9/README.md` & `async_poe_client-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 - [Step 1: Import the library and create a Poe_Client object](#step-1-import-the-library-and-create-a-poeclient-object)
 - [Step 2: Use Poe_Client](#step-2-use-poeclient)
     - [1. Get Account Subscription Information](#1-get-the-subscription-information-of-the-account)
     - [2. Create a Bot](#2-create-a-bot)
     - [3. Edit a Bot’s Settings](#3-edit-a-bots-settings)
     - [4. Delete a Bot](#4-delete-a-bot)
     - [5. Chat with a Bot](#5-chat-with-a-bot)
-        - [(1). Use websockets and httpx supported functions for streaming output and suggested replies](#1-using-websockets-and-httpx-support-for-streaming-output-and-suggested-replies)
-        - [(2). Use httpx only supported functions without suggested replies and streaming output](#2-function-that-only-uses-httpx-and-does-not-support-suggested-replies-and-streaming-output)
+        - [(1). Use channel_url and aiohttp supported functions for streaming output and suggested replies](#1-using-channelurl-and-aiohttp-support-for-streaming-output-and-suggested-replies)
+        - [(2). Use data_url and aiohttp supported functions without suggested replies and streaming output](#2-using-dataurl-and-aiohttp-but-does-not-support-suggested-replies-and-streaming-output)
     - [6. Delete a Bot's Dialogue Memory, Reset Conversation (This won't delete messages in chat history)](#6-deleting-a-bots-dialogue-memory-resetting-the-dialogue-this-does-not-delete-messages-in-the-chat-history)
     - [7. Get your Available Bots](#7-get-your-own-available-bots)
     - [8. Bulk Delete your Available Bots](#8-bulk-delete-your-available-bots)
     - [9. Get partial data or full settings of a bot](#9-get-partial-data-or-full-settings-of-a-bot)
     - [10. Get Chat History (Chat Messages)](#10-get-chat-history-chat-messages)
     - [11. Delete Chat History (Chat Messages)](#11-delete-chat-history-chat-messages)
         - [(1). Delete Chat History with a Certain Bot](#1-delete-chat-history-with-a-certain-bot)
@@ -39,24 +39,32 @@
     2. For bots you create, url_botname = handle. If display_name is set, the name you see on the web page is display_name;
        if not set, you see url_botname (handle).
        However, there are special cases where the handle does not follow the above rules, such as the handle of all bots
        obtained using get_available_bots always equals url_botname.
 
 ## Step 1: Import the library and create a Poe_Client object
 
+If you don't formkey to the Poe_Client, you need to install node.js for generate form key.
+Here is the download link.[node.js](https://nodejs.org/en)
+
 Before you can use any functionality of the `Poe_Client` library, you first need to import the library and create
-a `Poe_Client` object. You need to pass the `p_b token` to the constructor of `Poe_Client`, and then call the `create`
+a `Poe_Client` object. You need to pass the `p_b token` and `formkey` to the constructor of `Poe_Client`, and then call the `create`
 method to initialize it. Here is an example:
 
 ```python
 from async_poe_client import Poe_Client
 
-poe_client = await Poe_Client("your p_b token", "your formkey").create()
+poe_client = await Poe_Client("your p_b token").create()
+# or with a proxy
+poe_client = await Poe_Client("your p_b token", proxy="socks5://127.0.0.1:7890").create()
+
+# if the formkey algorithm changes, please pass your formkey
+poe_client = await Poe_Client("your p_b token","your form key").create()
 # or with a proxy
-poe_client = await Poe_Client("your p_b token", "your formkey", proxy="socks5://127.0.0.1:7890").create()
+poe_client = await Poe_Client("your p_b token","your form key", proxy="socks5://127.0.0.1:7890").create()
 ```
 
 Here, `"your p_b token"` should be replaced with your actual p_b token.
 
 ## Step 2: Use Poe_Client
 
 After creating the `Poe_Client`, you can use it to perform a lot of operations.
@@ -190,15 +198,15 @@
 await poe_client.delete_bot(url_botname="test27gs2")
 ```
 
 ---
 
 ### 5. Chat with a Bot
 
-#### (1). Using websockets and httpx support for streaming output and suggested replies
+#### (1). Using channel_url and aiohttp support for streaming output and suggested replies
 
 Function: `ask_stream()`
 
 Parameters:
 
 - `url_botname: str` - The url_botname of the bot.
 - `question: str` - The content of the query.
@@ -208,22 +216,22 @@
   dialogue).
 
 Return value: `AsyncGenerator` of `str`
 
 ```python
 # The usage of get_available_bots() can be seen in section 8.
 bots = await poe_client.get_available_bots(count=2)
-async for message in poe_client.ask_stream(url_botname=bots[1]['handle'], question="introduce websockets"):
+async for message in poe_client.ask_stream(url_botname=bots[1]['handle'], question="introduce async and await"):
     print(message, end="")
 # If suggested replies are used and a list of suggested replies is desired, you can extract from the bots property.
 # It records the latest suggested replies of a bot.
 print(poe_client.bots[bots[1]['handle']]['Suggestion'])
 ```
 
-#### (2). Function that only uses httpx and does not support suggested replies and streaming output
+#### (2). Using data_url and aiohttp but does not support suggested replies and streaming output
 
 Function: `ask()`
 
 Parameters:
 
 - `url_botname: str` - The url_botname of the bot.
 - `question: str` - The content of the query.
```

### Comparing `async_poe_client-0.1.9/PKG-INFO` & `async_poe_client-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: async-poe-client
-Version: 0.1.9
+Version: 0.2.0
 Summary: A stable, fast and convenient async client for poe.com
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: pyexecjs2 (>=1.6.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # User Guide
 
 [中文版本](README_zh_CN.md)
 
 This is a guide on how to use the `async-poe-Client` library. Before starting, make sure you've installed this library.
@@ -32,16 +33,16 @@
 - [Step 1: Import the library and create a Poe_Client object](#step-1-import-the-library-and-create-a-poeclient-object)
 - [Step 2: Use Poe_Client](#step-2-use-poeclient)
     - [1. Get Account Subscription Information](#1-get-the-subscription-information-of-the-account)
     - [2. Create a Bot](#2-create-a-bot)
     - [3. Edit a Bot’s Settings](#3-edit-a-bots-settings)
     - [4. Delete a Bot](#4-delete-a-bot)
     - [5. Chat with a Bot](#5-chat-with-a-bot)
-        - [(1). Use websockets and httpx supported functions for streaming output and suggested replies](#1-using-websockets-and-httpx-support-for-streaming-output-and-suggested-replies)
-        - [(2). Use httpx only supported functions without suggested replies and streaming output](#2-function-that-only-uses-httpx-and-does-not-support-suggested-replies-and-streaming-output)
+        - [(1). Use channel_url and aiohttp supported functions for streaming output and suggested replies](#1-using-channelurl-and-aiohttp-support-for-streaming-output-and-suggested-replies)
+        - [(2). Use data_url and aiohttp supported functions without suggested replies and streaming output](#2-using-dataurl-and-aiohttp-but-does-not-support-suggested-replies-and-streaming-output)
     - [6. Delete a Bot's Dialogue Memory, Reset Conversation (This won't delete messages in chat history)](#6-deleting-a-bots-dialogue-memory-resetting-the-dialogue-this-does-not-delete-messages-in-the-chat-history)
     - [7. Get your Available Bots](#7-get-your-own-available-bots)
     - [8. Bulk Delete your Available Bots](#8-bulk-delete-your-available-bots)
     - [9. Get partial data or full settings of a bot](#9-get-partial-data-or-full-settings-of-a-bot)
     - [10. Get Chat History (Chat Messages)](#10-get-chat-history-chat-messages)
     - [11. Delete Chat History (Chat Messages)](#11-delete-chat-history-chat-messages)
         - [(1). Delete Chat History with a Certain Bot](#1-delete-chat-history-with-a-certain-bot)
@@ -57,24 +58,32 @@
     2. For bots you create, url_botname = handle. If display_name is set, the name you see on the web page is display_name;
        if not set, you see url_botname (handle).
        However, there are special cases where the handle does not follow the above rules, such as the handle of all bots
        obtained using get_available_bots always equals url_botname.
 
 ## Step 1: Import the library and create a Poe_Client object
 
+If you don't formkey to the Poe_Client, you need to install node.js for generate form key.
+Here is the download link.[node.js](https://nodejs.org/en)
+
 Before you can use any functionality of the `Poe_Client` library, you first need to import the library and create
-a `Poe_Client` object. You need to pass the `p_b token` to the constructor of `Poe_Client`, and then call the `create`
+a `Poe_Client` object. You need to pass the `p_b token` and `formkey` to the constructor of `Poe_Client`, and then call the `create`
 method to initialize it. Here is an example:
 
 ```python
 from async_poe_client import Poe_Client
 
-poe_client = await Poe_Client("your p_b token", "your formkey").create()
+poe_client = await Poe_Client("your p_b token").create()
+# or with a proxy
+poe_client = await Poe_Client("your p_b token", proxy="socks5://127.0.0.1:7890").create()
+
+# if the formkey algorithm changes, please pass your formkey
+poe_client = await Poe_Client("your p_b token","your form key").create()
 # or with a proxy
-poe_client = await Poe_Client("your p_b token", "your formkey", proxy="socks5://127.0.0.1:7890").create()
+poe_client = await Poe_Client("your p_b token","your form key", proxy="socks5://127.0.0.1:7890").create()
 ```
 
 Here, `"your p_b token"` should be replaced with your actual p_b token.
 
 ## Step 2: Use Poe_Client
 
 After creating the `Poe_Client`, you can use it to perform a lot of operations.
@@ -208,15 +217,15 @@
 await poe_client.delete_bot(url_botname="test27gs2")
 ```
 
 ---
 
 ### 5. Chat with a Bot
 
-#### (1). Using websockets and httpx support for streaming output and suggested replies
+#### (1). Using channel_url and aiohttp support for streaming output and suggested replies
 
 Function: `ask_stream()`
 
 Parameters:
 
 - `url_botname: str` - The url_botname of the bot.
 - `question: str` - The content of the query.
@@ -226,22 +235,22 @@
   dialogue).
 
 Return value: `AsyncGenerator` of `str`
 
 ```python
 # The usage of get_available_bots() can be seen in section 8.
 bots = await poe_client.get_available_bots(count=2)
-async for message in poe_client.ask_stream(url_botname=bots[1]['handle'], question="introduce websockets"):
+async for message in poe_client.ask_stream(url_botname=bots[1]['handle'], question="introduce async and await"):
     print(message, end="")
 # If suggested replies are used and a list of suggested replies is desired, you can extract from the bots property.
 # It records the latest suggested replies of a bot.
 print(poe_client.bots[bots[1]['handle']]['Suggestion'])
 ```
 
-#### (2). Function that only uses httpx and does not support suggested replies and streaming output
+#### (2). Using data_url and aiohttp but does not support suggested replies and streaming output
 
 Function: `ask()`
 
 Parameters:
 
 - `url_botname: str` - The url_botname of the bot.
 - `question: str` - The content of the query.
```

