# Comparing `tmp/nonebot-plugin-twitter-0.1.8.tar.gz` & `tmp/nonebot-plugin-twitter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-twitter-0.1.8.tar", last modified: Tue Jun 27 15:35:27 2023, max compression
+gzip compressed data, was "nonebot-plugin-twitter-0.1.9.tar", last modified: Thu Jul 20 05:36:15 2023, max compression
```

## Comparing `nonebot-plugin-twitter-0.1.8.tar` & `nonebot-plugin-twitter-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/LICENSE
--rw-r--r--   0        0        0     3154 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/README.md
--rw-r--r--   0        0        0    14821 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/__init__.py
--rw-r--r--   0        0        0     4914 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/api.py
--rw-r--r--   0        0        0     1582 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/config.py
--rw-r--r--   0        0        0      654 2023-06-27 15:35:19.752761 nonebot-plugin-twitter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-20 05:36:04.927052 nonebot-plugin-twitter-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3347 2023-07-20 05:36:04.927052 nonebot-plugin-twitter-0.1.9/README.md
+-rw-r--r--   0        0        0    16243 2023-07-20 05:36:04.927052 nonebot-plugin-twitter-0.1.9/nonebot_plugin_twitter/__init__.py
+-rw-r--r--   0        0        0     4914 2023-07-20 05:36:04.927052 nonebot-plugin-twitter-0.1.9/nonebot_plugin_twitter/api.py
+-rw-r--r--   0        0        0     1578 2023-07-20 05:36:04.927052 nonebot-plugin-twitter-0.1.9/nonebot_plugin_twitter/config.py
+-rw-r--r--   0        0        0      654 2023-07-20 05:36:04.927052 nonebot-plugin-twitter-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 nonebot-plugin-twitter-0.1.9/PKG-INFO
```

### Comparing `nonebot-plugin-twitter-0.1.8/LICENSE` & `nonebot-plugin-twitter-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.8/README.md` & `nonebot-plugin-twitter-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 <a href="https://pypi.python.org/pypi/nonebot-plugin-twitter">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-twitter.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
+~~## ⚠ 插件暂不可用~~
+
+~~因推特开启登录墙，该插件暂不可用~~
 
 ## 📖 介绍
 
 订阅推送 twitter 推文
 
 ## 💿 安装
 
@@ -79,28 +82,38 @@
 command_priority=10
 ```
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
-| 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18]” r18为可选参数，不开启和默认为不推送r18推文|
+| 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18] [媒体]”|
 | 取关推主 | 无 | 否 | 群聊/私聊 | 取关切割 |
 | 推主列表 | 无 | 否 | 群聊/私聊 | 展示列表 |
 | 推文推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
 | 推文推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
+[] 为可选参数，
+r18 : 开启r18推文推送
+媒体 : 仅推送媒体消息
+
 ### 效果图
 [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV)
 [![pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT)
 ### 注意事项
 1.推主id：
 [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
 
 2.消息为合并转发发送，存在延迟和发送失败的可能
 
 3.新的0.1.0版本为破坏性更新：代理配置格式更改，关注列表需重新关注。
 
 ### 更新记录
 
+2023.07.20
+
+1. 增加了仅媒体推送
+2. 修复了该插件与若干问题
+
+
 2023.06.27
 
 1. 临时解决回复原推文时，无法推送全部推文的问题
```

#### html2text {}

```diff
@@ -1,34 +1,36 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
                                    [python]
-## ð ä»ç» è®¢éæ¨é twitter æ¨æ ## ð¿ å®è£
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
-poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
-twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
-[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
-âï¸ éç½® å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | twitter_website | å¦ |
-æ  | èªå®ä¹website | | twitter_proxy | å¦ | æ  | proxy | | twitter_qq |
-å¦ | 2854196310 | åå¹¶æ¶æ¯å¤´åæ¥æº | | command_priority | å¦ | 10 |
-å½ä»¤ä¼åçº§ | éç½®æ ¼å¼ç¤ºä¾ ```bash #twitter twitter_proxy="http://
-127.0.0.1:1090" twitter_qq=2854196306 command_priority=10 ``` ## ð ä½¿ç¨
-### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:
-----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
-å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
-r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
-æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
-ç§è | å±ç¤ºåè¡¨ | | æ¨ææ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
-å³é­æ¨é | | æ¨ææ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
-å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
-pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
-2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
-1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)]
-(https://imgse.com/i/pCPMu36)
+~~## â  æä»¶æä¸å¯ç¨~~
+~~å æ¨ç¹å¼å¯ç»å½å¢ï¼è¯¥æä»¶æä¸å¯ç¨~~ ## ð ä»ç»
+è®¢éæ¨é twitter æ¨æ ## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
+nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter   poetry poetry add
+nonebot-plugin-twitter   conda conda install nonebot-plugin-twitter  æå¼
+nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ## âï¸ éç½® å¨
+nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ |
+å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | twitter_website
+| å¦ | æ  | èªå®ä¹website | | twitter_proxy | å¦ | æ  | proxy | |
+twitter_qq | å¦ | 2854196310 | åå¹¶æ¶æ¯å¤´åæ¥æº | | command_priority |
+å¦ | 10 | å½ä»¤ä¼åçº§ | éç½®æ ¼å¼ç¤ºä¾ ```bash #twitter
+twitter_proxy="http://127.0.0.1:1090" twitter_qq=2854196306 command_priority=10
+``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ
+| |:-----:|:----:|:----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/
+ç§è | å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18] [åªä½]â|
+| åå³æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ |
+æ  | å¦ | ç¾¤è/ç§è | å±ç¤ºåè¡¨ | | æ¨ææ¨éå³é­ | ç¾¤ç®¡ | å¦
+| ç¾¤è/ç§è | å³é­æ¨é | | æ¨ææ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/
+ç§è | å¼å¯æ¨é | [] ä¸ºå¯éåæ°ï¼ r18 : å¼å¯r18æ¨ææ¨é
+åªä½ : ä»æ¨éåªä½æ¶æ¯ ### ææå¾ [![pCPuhWV.png](https://
+s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [!
+[pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/
+pCPu4zT) ### æ³¨æäºé¡¹ 1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/
+2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
 2.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
 3.æ°ç0.1.0çæ¬ä¸ºç ´åæ§æ´æ°ï¼ä»£çéç½®æ ¼å¼æ´æ¹ï¼å³æ³¨åè¡¨ééæ°å³æ³¨ã
-### æ´æ°è®°å½ 2023.06.27 1.
+### æ´æ°è®°å½ 2023.07.20 1. å¢å äºä»åªä½æ¨é 2.
+ä¿®å¤äºè¯¥æä»¶ä¸è¥å¹²é®é¢ 2023.06.27 1.
 ä¸´æ¶è§£å³åå¤åæ¨ææ¶ï¼æ æ³æ¨éå¨é¨æ¨æçé®é¢
```

### Comparing `nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/__init__.py` & `nonebot-plugin-twitter-0.1.9/nonebot_plugin_twitter/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     web_list.append(config_dev.twitter_website)
 web_list += website_list
 
 
 with Client(proxies=config_dev.twitter_proxy) as client:
     for url in web_list:
         try:
-            res = client.get(url)
+            res = client.get(f"{url}/elonmusk")
             if res.status_code == 200:
                 logger.info(f"website: {url} ok!")
                 config_dev.twitter_url = url
                 break
             else:
                 logger.info(f"website: {url} failed!")
         except Exception as e:
@@ -71,22 +71,24 @@
     dirpath.mkdir(parents=True, exist_ok=True)
     dirpath = Path() / "data" / "twitter" / "cache"
     dirpath.mkdir(parents=True, exist_ok=True)
     dirpath = Path() / "data" / "twitter" / "twitter_list.json"
     dirpath.touch()
     if not dirpath.stat().st_size:
         dirpath.write_text("{}")
-
-    @scheduler.scheduled_job("interval",minutes=3,id="twitter",misfire_grace_time=180)
-    async def now_twitter():
-        twitter_list = json.loads(dirpath.read_text("utf8"))
-        twitter_list_task = [
-            get_status(user_name, twitter_list) for user_name in twitter_list
-        ]
-        asyncio.gather(*twitter_list_task)
+    if not config_dev.twitter_url:
+        logger.debug(f"website 推文服务器为空，跳过推文定时检索")
+    else:
+        @scheduler.scheduled_job("interval",minutes=3,id="twitter",misfire_grace_time=180)
+        async def now_twitter():
+            twitter_list = json.loads(dirpath.read_text("utf8"))
+            twitter_list_task = [
+                get_status(user_name, twitter_list) for user_name in twitter_list
+            ]
+            asyncio.gather(*twitter_list_task)
 
         
 def msg_type(user_id:int, task: str,name: str):
     return MessageSegment.node_custom(user_id=user_id, nickname=name,
                                           content=Message(MessageSegment.video(f"file:///{task}")))        
         
 async def get_pic(url: str,user_name: str) -> MessageSegment:
@@ -144,14 +146,18 @@
                 bots = nonebot.get_adapter(Adapter).bots
                 for group_num in twitter_list[user_name]["group"]:
                     # 群聊
                     if twitter_list[user_name]["group"][group_num]["status"]:
                         if twitter_list[user_name]["group"][group_num]["r18"] == False and tweet_info["r18"] == True:
                             logger.info(f"根据r18设置，群 {group_num} 的推文 {user_name}/status/{line_new_tweet_id} 跳过发送")
                             continue
+                        if twitter_list[user_name]["group"][group_num]["media"] == True and tweet_info["media"] == False:
+                            logger.info(f"根据媒体设置，群 {group_num} 的推文 {user_name}/status/{line_new_tweet_id} 跳过发送")
+                            continue
+                        
                         for bot in bots:
                             try:
                                 await bots[bot].send_group_forward_msg(group_id=int(group_num), messages=task_res)
                                 logger.info(f"群 {group_num} 的推文 {user_name}/status/{line_new_tweet_id} 发送成功")
                             except Exception:
                                 pass
                     else:
@@ -159,14 +165,18 @@
                         
                 for qq in twitter_list[user_name]["private"]:
                     # 私聊
                     if twitter_list[user_name]["private"][qq]["status"]:
                         if twitter_list[user_name]["private"][qq]["r18"] == False and tweet_info["r18"] == True:
                             logger.info(f"根据r18设置，qq {qq} 的推文 {user_name}/status/{line_new_tweet_id} 跳过发送")   
                             continue
+                        if twitter_list[user_name]["private"][qq]["media"] == True and tweet_info["media"] == False:
+                            logger.info(f"根据媒体设置，qq {qq} 的推文 {user_name}/status/{line_new_tweet_id} 跳过发送")   
+                            continue
+                        
                         for bot in bots:
                             try:
                                 await bots[bot].send_private_forward_msg(user_id=int(qq), messages=task_res)
                                 logger.info(f"qq {qq} 的推文 {user_name}/status/{line_new_tweet_id} 发送成功")
                             except Exception:
                                 pass
                     else:
@@ -184,14 +194,16 @@
     except Exception as e:
         logger.debug(f"出现异常：{e}")
 
 
 save = on_command("关注推主",block=True,priority=config_dev.command_priority)
 @save.handle()
 async def save_handle(bot:Bot,event: MessageEvent,matcher: Matcher,arg: Message = CommandArg()):
+    if not config_dev.twitter_url:
+        await matcher.finish("website 推文服务器访问失败，请检查连通性或代理")
     data = []
     if " " in arg.extract_plain_text():
         data = arg.extract_plain_text().split(" ")
     else:
         data.append(arg.extract_plain_text())
         data.append("")
     user_info = await get_user_info(data[0])
@@ -204,39 +216,43 @@
     twitter_list = json.loads(dirpath.read_text("utf8"))
     if isinstance(event,GroupMessageEvent):
         if data[0] not in twitter_list:
             twitter_list[data[0]] = {
                 "group":{
                     str(event.group_id):{
                         "status":True,
-                        "r18":True if data[1]=='r18' else False
+                        "r18":True if 'r18' in data[1:] else False,
+                        "media":True if '媒体' in data[1:] else False
                     }
                 },
                 "private":{}
             }
         else:
             twitter_list[data[0]]["group"][str(event.group_id)] = {
                         "status":True,
-                        "r18":True if data[1]=='r18' else False
+                        "r18":True if 'r18' in data[1:] else False,
+                        "media":True if '媒体' in data[1:] else False
                     }
     else:
         if data[0] not in twitter_list:
             twitter_list[data[0]] = {
                 "group":{},
                 "private":{
                     str(event.user_id):{
                         "status":True,
-                        "r18":True if data[0]=='r18' else False
+                        "r18":True if 'r18' in data[1:] else False,
+                        "media":True if '媒体' in data[1:] else False
                     }
                 }
             }
         else:
             twitter_list[data[0]]["private"][str(event.user_id)] = {
                         "status":True,
-                        "r18":True if data[1]=='r18' else False
+                        "r18":True if 'r18' in data[1:] else False,
+                        "media":True if '媒体' in data[1:] else False
                     }
             
     twitter_list[data[0]]["since_id"] = tweet_id
     twitter_list[data[0]]["screen_name"] = user_info["screen_name"]
     dirpath.write_text(json.dumps(twitter_list))
     await matcher.finish(f"id:{data[0]}\nname:{user_info['screen_name']}\n{user_info['bio']}\n订阅成功")
         
@@ -280,26 +296,26 @@
     
     if isinstance(event,GroupMessageEvent):
         for user_name in twitter_list:
             if str(event.group_id) in twitter_list[user_name]["group"]:
                 msg += [
                     MessageSegment.node_custom(
                         user_id=config_dev.twitter_qq, nickname=twitter_list[user_name]["screen_name"], content=Message(
-                            f"{user_name}  {'r18' if twitter_list[user_name]['group'][str(event.group_id)]['r18'] else ''}"
+                            f"{user_name}  {'r18' if twitter_list[user_name]['group'][str(event.group_id)]['r18'] else ''}  {'媒体' if twitter_list[user_name]['group'][str(event.group_id)]['media'] else ''}"
                             )
                     )
                 ]
         await bot.send_group_forward_msg(group_id=event.group_id, messages=msg)
     else:
         for user_name in twitter_list:
             if str(event.user_id) in twitter_list[user_name]["private"]:
                 msg += [
                     MessageSegment.node_custom(
                         user_id=config_dev.twitter_qq, nickname=twitter_list[user_name]["screen_name"], content=Message(
-                            f"{user_name}  {'r18' if twitter_list[user_name]['private'][str(event.user_id)]['r18'] else ''}"
+                            f"{user_name}  {'r18' if twitter_list[user_name]['private'][str(event.user_id)]['r18'] else ''}  {'媒体' if twitter_list[user_name]['private'][str(event.user_id)]['media'] else ''}"
                             )
                     )
                 ]
         await bot.send_private_forward_msg(user_id=event.user_id, messages=msg)          
     
     await matcher.finish()
```

### Comparing `nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/api.py` & `nonebot-plugin-twitter-0.1.9/nonebot_plugin_twitter/api.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-twitter-0.1.8/nonebot_plugin_twitter/config.py` & `nonebot-plugin-twitter-0.1.9/nonebot_plugin_twitter/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,14 @@
         if isinstance(v,int) and v >= 1:
             logger.info("command_priority 读取成功")
             return v
         
 config_dev = Config.parse_obj(get_driver().config)
 
 website_list = [
-    "https://twitter.owacon.moe",
+    "https://nitter.1d4.us",
+    "https://bird.trom.tf",
+    "https://nitter.moomoo.me"
     "https://nitter.unixfox.eu",
-    "https://nitter.1d4.us/",
-    "https://nitter.it/",
-    "https://bird.trom.tf/",
-    "https://nitter.moomoo.me/"
+    "https://nitter.it",
+    "https://twitter.owacon.moe",
 ]
```

### Comparing `nonebot-plugin-twitter-0.1.8/pyproject.toml` & `nonebot-plugin-twitter-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-twitter"
-version = "0.1.8"
+version = "0.1.9"
 description = "NoneBot2 plugin for twitter"
 authors = [
     { name = "nek0us", email = "nekouss@gmail.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.1.3",
```

### Comparing `nonebot-plugin-twitter-0.1.8/PKG-INFO` & `nonebot-plugin-twitter-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-twitter
-Version: 0.1.8
+Version: 0.1.9
 Summary: NoneBot2 plugin for twitter
 License: MIT
 Author-email: nek0us <nekouss@gmail.com>
 Requires-Python: >=3.8
 Project-URL: Homepage, https://github.com/nek0us/nonebot-plugin-twitter
 Project-URL: Repository, https://github.com/nek0us/nonebot-plugin-twitter
 Description-Content-Type: text/markdown
@@ -28,14 +28,17 @@
 <a href="https://pypi.python.org/pypi/nonebot-plugin-twitter">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-twitter.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 
 </div>
 
+~~## ⚠ 插件暂不可用~~
+
+~~因推特开启登录墙，该插件暂不可用~~
 
 ## 📖 介绍
 
 订阅推送 twitter 推文
 
 ## 💿 安装
 
@@ -90,29 +93,39 @@
 command_priority=10
 ```
 
 ## 🎉 使用
 ### 指令表
 | 指令 | 权限 | 需要@ | 范围 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
-| 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18]” r18为可选参数，不开启和默认为不推送r18推文|
+| 关注推主 | 无 | 否 | 群聊/私聊 | 关注，指令格式：“关注推主 <推主id> [r18] [媒体]”|
 | 取关推主 | 无 | 否 | 群聊/私聊 | 取关切割 |
 | 推主列表 | 无 | 否 | 群聊/私聊 | 展示列表 |
 | 推文推送关闭 | 群管 | 否 | 群聊/私聊 | 关闭推送 |
 | 推文推送开启 | 群管 | 否 | 群聊/私聊 | 开启推送 |
+[] 为可选参数，
+r18 : 开启r18推文推送
+媒体 : 仅推送媒体消息
+
 ### 效果图
 [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV)
 [![pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT)
 ### 注意事项
 1.推主id：
 [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
 
 2.消息为合并转发发送，存在延迟和发送失败的可能
 
 3.新的0.1.0版本为破坏性更新：代理配置格式更改，关注列表需重新关注。
 
 ### 更新记录
 
+2023.07.20
+
+1. 增加了仅媒体推送
+2. 修复了该插件与若干问题
+
+
 2023.06.27
 
 1. 临时解决回复原推文时，无法推送全部推文的问题
```

#### html2text {}

```diff
@@ -1,39 +1,41 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-twitter Version: 0.1.9 Summary:
 NoneBot2 plugin for twitter License: MIT Author-email: nek0us
 gmail.com> Requires-Python: >=3.8 Project-URL: Homepage, https://github.com/
 nek0us/nonebot-plugin-twitter Project-URL: Repository, https://github.com/
 nek0us/nonebot-plugin-twitter Description-Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # nonebot-plugin-twitter _â¨ æ¨æè®¢éæ¨éæä»¶ â¨_ [license] [pypi]
                                    [python]
-## ð ä»ç» è®¢éæ¨é twitter æ¨æ ## ð¿ å®è£
-ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
-æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-pip pip install nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter
-poetry poetry add nonebot-plugin-twitter   conda conda install nonebot-plugin-
-twitter  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `
-[tool.nonebot]` é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ##
-âï¸ éç½® å¨ nonebot2
-é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
-é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | twitter_website | å¦ |
-æ  | èªå®ä¹website | | twitter_proxy | å¦ | æ  | proxy | | twitter_qq |
-å¦ | 2854196310 | åå¹¶æ¶æ¯å¤´åæ¥æº | | command_priority | å¦ | 10 |
-å½ä»¤ä¼åçº§ | éç½®æ ¼å¼ç¤ºä¾ ```bash #twitter twitter_proxy="http://
-127.0.0.1:1090" twitter_qq=2854196306 command_priority=10 ``` ## ð ä½¿ç¨
-### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:
-----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è |
-å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18]â
-r18ä¸ºå¯éåæ°ï¼ä¸å¼å¯åé»è®¤ä¸ºä¸æ¨ér18æ¨æ| | åå³æ¨ä¸» |
-æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ | æ  | å¦ | ç¾¤è/
-ç§è | å±ç¤ºåè¡¨ | | æ¨ææ¨éå³é­ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
-å³é­æ¨é | | æ¨ææ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/ç§è |
-å¼å¯æ¨é | ### ææå¾ [![pCPuhWV.png](https://s1.ax1x.com/2023/06/05/
-pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [![pCPu4zT.png](https://s1.ax1x.com/
-2023/06/05/pCPu4zT.png)](https://imgse.com/i/pCPu4zT) ### æ³¨æäºé¡¹
-1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/2023/06/05/pCPMu36.png)]
-(https://imgse.com/i/pCPMu36)
+~~## â  æä»¶æä¸å¯ç¨~~
+~~å æ¨ç¹å¼å¯ç»å½å¢ï¼è¯¥æä»¶æä¸å¯ç¨~~ ## ð ä»ç»
+è®¢éæ¨é twitter æ¨æ ## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨
+nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
+æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
+nonebot-plugin-twitter   pdm pdm add nonebot-plugin-twitter   poetry poetry add
+nonebot-plugin-twitter   conda conda install nonebot-plugin-twitter  æå¼
+nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
+é¨åè¿½å åå¥ plugins = ["nonebot_plugin_twitter"]  ## âï¸ éç½® å¨
+nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ |
+å¿å¡« | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | twitter_website
+| å¦ | æ  | èªå®ä¹website | | twitter_proxy | å¦ | æ  | proxy | |
+twitter_qq | å¦ | 2854196310 | åå¹¶æ¶æ¯å¤´åæ¥æº | | command_priority |
+å¦ | 10 | å½ä»¤ä¼åçº§ | éç½®æ ¼å¼ç¤ºä¾ ```bash #twitter
+twitter_proxy="http://127.0.0.1:1090" twitter_qq=2854196306 command_priority=10
+``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ
+| |:-----:|:----:|:----:|:----:|:----:| | å³æ³¨æ¨ä¸» | æ  | å¦ | ç¾¤è/
+ç§è | å³æ³¨ï¼æä»¤æ ¼å¼ï¼âå³æ³¨æ¨ä¸» <æ¨ä¸»id> [r18] [åªä½]â|
+| åå³æ¨ä¸» | æ  | å¦ | ç¾¤è/ç§è | åå³åå² | | æ¨ä¸»åè¡¨ |
+æ  | å¦ | ç¾¤è/ç§è | å±ç¤ºåè¡¨ | | æ¨ææ¨éå³é­ | ç¾¤ç®¡ | å¦
+| ç¾¤è/ç§è | å³é­æ¨é | | æ¨ææ¨éå¼å¯ | ç¾¤ç®¡ | å¦ | ç¾¤è/
+ç§è | å¼å¯æ¨é | [] ä¸ºå¯éåæ°ï¼ r18 : å¼å¯r18æ¨ææ¨é
+åªä½ : ä»æ¨éåªä½æ¶æ¯ ### ææå¾ [![pCPuhWV.png](https://
+s1.ax1x.com/2023/06/05/pCPuhWV.png)](https://imgse.com/i/pCPuhWV) [!
+[pCPu4zT.png](https://s1.ax1x.com/2023/06/05/pCPu4zT.png)](https://imgse.com/i/
+pCPu4zT) ### æ³¨æäºé¡¹ 1.æ¨ä¸»idï¼ [![pCPMu36.png](https://s1.ax1x.com/
+2023/06/05/pCPMu36.png)](https://imgse.com/i/pCPMu36)
 2.æ¶æ¯ä¸ºåå¹¶è½¬ååéï¼å­å¨å»¶è¿ååéå¤±è´¥çå¯è½
 3.æ°ç0.1.0çæ¬ä¸ºç ´åæ§æ´æ°ï¼ä»£çéç½®æ ¼å¼æ´æ¹ï¼å³æ³¨åè¡¨ééæ°å³æ³¨ã
-### æ´æ°è®°å½ 2023.06.27 1.
+### æ´æ°è®°å½ 2023.07.20 1. å¢å äºä»åªä½æ¨é 2.
+ä¿®å¤äºè¯¥æä»¶ä¸è¥å¹²é®é¢ 2023.06.27 1.
 ä¸´æ¶è§£å³åå¤åæ¨ææ¶ï¼æ æ³æ¨éå¨é¨æ¨æçé®é¢
```

