# Comparing `tmp/liteclashproman-0.3.0.tar.gz` & `tmp/liteclashproman-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liteclashproman-0.3.0.tar", last modified: Thu Jul 20 07:42:10 2023, max compression
+gzip compressed data, was "liteclashproman-0.4.0.tar", last modified: Tue Jul 25 17:21:30 2023, max compression
```

## Comparing `liteclashproman-0.3.0.tar` & `liteclashproman-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34523 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LICENSE
--rw-r--r--   0        0        0     1177 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/__init__.py
--rw-r--r--   0        0        0     3696 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/config.py
--rw-r--r--   0        0        0     1782 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/log.py
--rw-r--r--   0        0        0     2764 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/main.py
--rw-r--r--   0        0        0     2232 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/model/clash/__init__.py
--rw-r--r--   0        0        0     1863 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/model/clash/proxy.py
--rw-r--r--   0        0        0      400 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/model/clash/proxygroup.py
--rw-r--r--   0        0        0      166 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/model/clash/ruleprovider.py
--rw-r--r--   0        0        0     4046 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/static/config.exp.yaml
--rw-r--r--   0        0        0     3508 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/static/template/blacklist.yaml
--rw-r--r--   0        0        0     2607 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/static/template/whitelist.yaml
--rw-r--r--   0        0        0     2226 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/subscribe/__init__.py
--rw-r--r--   0        0        0     1239 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/subscribe/base64.py
--rw-r--r--   0        0        0      744 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/subscribe/clash.py
--rw-r--r--   0        0        0     1530 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/subscribe/jms.py
--rw-r--r--   0        0        0     1812 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/LiteClashProMan/utils.py
--rw-r--r--   0        0        0     3222 2023-07-20 07:42:00.626049 liteclashproman-0.3.0/README.md
--rw-r--r--   0        0        0      675 2023-07-20 07:42:10.250005 liteclashproman-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 liteclashproman-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LICENSE
+-rw-r--r--   0        0        0      958 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/__init__.py
+-rw-r--r--   0        0        0     3696 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/config.py
+-rw-r--r--   0        0        0     1782 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/log.py
+-rw-r--r--   0        0        0     2799 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/main.py
+-rw-r--r--   0        0        0     1948 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/model/clash/__init__.py
+-rw-r--r--   0        0        0     1863 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/model/clash/proxy.py
+-rw-r--r--   0        0        0      400 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/model/clash/proxygroup.py
+-rw-r--r--   0        0        0      166 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/model/clash/ruleprovider.py
+-rw-r--r--   0        0        0     4046 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/static/config.exp.yaml
+-rw-r--r--   0        0        0     3508 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/static/template/blacklist.yaml
+-rw-r--r--   0        0        0     2607 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/static/template/whitelist.yaml
+-rw-r--r--   0        0        0     2676 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/subscribe/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/subscribe/base64.py
+-rw-r--r--   0        0        0      744 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/subscribe/clash.py
+-rw-r--r--   0        0        0     1530 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/subscribe/jms.py
+-rw-r--r--   0        0        0     1812 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/LiteClashProMan/utils.py
+-rw-r--r--   0        0        0     3222 2023-07-25 17:21:19.945346 liteclashproman-0.4.0/README.md
+-rw-r--r--   0        0        0      675 2023-07-25 17:21:30.057334 liteclashproman-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3745 1970-01-01 00:00:00.000000 liteclashproman-0.4.0/PKG-INFO
```

### Comparing `liteclashproman-0.3.0/LICENSE` & `liteclashproman-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/__init__.py` & `liteclashproman-0.4.0/LiteClashProMan/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,31 +11,25 @@
 args = parser.parse_args()
 
 
 def main():
     # check dirs and files
     static_dir = Path(__file__).parent.joinpath("static")
     data_dir = Path("data")
-    profile_dir = data_dir.joinpath("profile")
     provider_dir = data_dir.joinpath("provider")
     template_dir = data_dir.joinpath("template")
 
-    for dir in [data_dir, profile_dir, provider_dir, template_dir]:
+    for dir in [data_dir, provider_dir, template_dir]:
         if not dir.exists():
             dir.mkdir(0o755, parents=True, exist_ok=True)
         assert dir.is_dir(), f"{dir.as_posix()} should be folder"
 
     if not any(template_dir.glob("*")):
         shutil.copytree(
             static_dir.joinpath("template"), template_dir, dirs_exist_ok=True
         )
 
-    # remove old profiles
-    if any(profile_dir.glob("*")):
-        shutil.rmtree(profile_dir)
-        profile_dir.mkdir(0o755, parents=True, exist_ok=True)
-
     Config.load(Path(args.config))
 
     from .main import main as run_main
 
     run_main()
```

### Comparing `liteclashproman-0.3.0/LiteClashProMan/config.py` & `liteclashproman-0.4.0/LiteClashProMan/config.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/log.py` & `liteclashproman-0.4.0/LiteClashProMan/log.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/main.py` & `liteclashproman-0.4.0/LiteClashProMan/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from apscheduler.schedulers.asyncio import AsyncIOScheduler
 from apscheduler.triggers.cron import CronTrigger
 from fastapi import FastAPI, HTTPException, Request
 from fastapi.staticfiles import StaticFiles
 from loguru import logger
-from starlette.responses import FileResponse
+from starlette.responses import PlainTextResponse
 from uvicorn import Config, Server
 
 from .config import config
 from .log import LOGGING_CONFIG
-from .subscribe import counter, update
+from .subscribe import counter, update_provider, generate_profile
 
 if config.sentry_dsn:
     import sentry_sdk
 
     sentry_sdk.init(
         dsn=config.sentry_dsn,
         traces_sample_rate=1.0,
@@ -40,50 +40,48 @@
 
     # logging id and ip
     user_ip = request.headers.get("X-Real-IP", request.client.host)
     logger.info(
         f"A request from {id}({user_ip}) to download profile {path} was received"
     )
 
-    resp = FileResponse(
-        path=f"data/profile/{path}",
+    resp = PlainTextResponse(
+        content=await generate_profile(path[:-5]), headers=config.headers.copy()
     )
     counter_info = await counter(path[:-5])
     if counter_info:
         resp.headers["subscription-userinfo"] = counter_info
-    for h in config.headers:
-        resp.headers[h] = config.headers[h]
     return resp
 
 
 # manual update trigger
 @app.get(f"/{config.urlprefix}/update")
 async def _():
     logger.info("Update is triggered manually")
-    error = await update()
+    error = await update_provider()
     return str(error) or "update complete"
 
 
 # test sentry debug
 @app.get("/sentry-debug")
 async def trigger_error():
     division_by_zero = 1 / 0
 
 
 @app.on_event("startup")
 async def startup_event():
-    error = await update()
+    error = await update_provider()
     if error:
         raise error
     logger.info(
         f"Starting up scheduler from crontab {config.update_cron} at timezone {config.update_tz}"
     )
     scheduler = AsyncIOScheduler()
     scheduler.add_job(
-        update, CronTrigger.from_crontab(config.update_cron, config.update_tz)
+        update_provider, CronTrigger.from_crontab(config.update_cron, config.update_tz)
     )
     scheduler.start()
     logger.info(
         f"Application startup complete, listening requests from {config.domian}/{config.urlprefix}/"
     )
```

### Comparing `liteclashproman-0.3.0/LiteClashProMan/model/clash/__init__.py` & `liteclashproman-0.4.0/LiteClashProMan/model/clash/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Dict, List, Literal, Optional, Union
+from typing import Dict, List, Literal, Optional, Union, Sequence
 
 import yaml
 from pydantic import BaseModel, Extra, Field, validator
 
 from .proxy import SS, SSR, Snell, Socks5, Trojan, Vmess
 from .proxygroup import ProxyGroup, ProxyGroupTemplate
 from .ruleprovider import RuleProvider
@@ -33,31 +33,23 @@
         if not proxies:
             return Clash(**self.dict(exclude_none=True, by_alias=True))
         proxies_name_list = [proxy.name for proxy in proxies]
         proxy_groups = []
         for group in self.proxy_groups:
             if group.proxies == "__proxies_name_list__":
                 group.proxies = proxies_name_list
-            if isinstance(group.proxies, list):
-                if "__proxies_name_list__" in group.proxies:
-                    group.proxies.remove("__proxies_name_list__")
-                    group.proxies += proxies_name_list
+            if (
+                isinstance(group.proxies, Sequence)
+                and "__proxies_name_list__" in group.proxies
+            ):
+                group.proxies.remove("__proxies_name_list__")
+                group.proxies += proxies_name_list
             proxy_groups.append(group)
 
         self.proxies = proxies
         self.proxy_groups = proxy_groups
         return Clash(**self.dict(exclude_none=True, by_alias=True))
 
 
 class Clash(ClashTemplate):
     proxies: List[Union[SS, SSR, Vmess, Socks5, Snell, Trojan]]
     proxy_groups: List[ProxyGroup] = Field(alias="proxy-groups")
-
-    def save(self, file: str) -> None:
-        Path(f"data/profile/{file}.yaml").write_text(
-            yaml.dump(
-                self.dict(exclude_none=True, by_alias=True, exclude_unset=True),
-                sort_keys=False,
-                allow_unicode=True,
-            ),
-            encoding="utf-8",
-        )
```

### Comparing `liteclashproman-0.3.0/LiteClashProMan/model/clash/proxy.py` & `liteclashproman-0.4.0/LiteClashProMan/model/clash/proxy.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/static/config.exp.yaml` & `liteclashproman-0.4.0/LiteClashProMan/static/config.exp.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/static/template/blacklist.yaml` & `liteclashproman-0.4.0/LiteClashProMan/static/template/blacklist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/static/template/whitelist.yaml` & `liteclashproman-0.4.0/LiteClashProMan/static/template/whitelist.yaml`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/subscribe/__init__.py` & `liteclashproman-0.4.0/LiteClashProMan/subscribe/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from pathlib import Path
 from typing import List, Union
 
+import yaml
 from loguru import logger
 
 from ..config import config
 from ..model.clash import SS, SSR, ClashTemplate, Snell, Socks5, Trojan, Vmess
 from ..utils import Download
 from . import clash, jms
 
@@ -19,37 +21,50 @@
         if sub.type == "ClashSub":
             proxies += await clash.get_sub(sub.url)
         if sub.type == "ClashFile":
             proxies += await clash.get_file(sub.file)
     return proxies
 
 
-async def update():
-    logger.info("Start update profiles")
+async def generate_profile(profile: str):
+    proxies = await _subs(config.profiles[profile].subs)
+    logger.debug(
+        f"Generating profile {profile} from template {config.profiles[profile].template}"
+    )
+    template = ClashTemplate.load(config.profiles[profile].template)
+    clash = template.render(proxies)
+    if clash.rule_providers:
+        for provider in clash.rule_providers:
+            # if provider is exists in local
+            # replace it with loacl file
+            if Path(f"data/provider/{provider}.yaml").exists():
+                clash.rule_providers[provider].url = "/".join(
+                    [
+                        config.domian,
+                        config.urlprefix,
+                        "provider",
+                        f"{provider}.yaml",
+                    ]
+                )
+    return yaml.dump(
+        clash.model_dump(exclude_none=True, by_alias=True, exclude_unset=True),
+        sort_keys=False,
+        allow_unicode=True,
+    )
+
+
+async def update_provider():
+    logger.info("Start update provider")
     try:
         rulesets = {}
         for profile in config.profiles:
-            proxies = await _subs(config.profiles[profile].subs)
-            logger.debug(
-                f"Generating profile {profile} from template {config.profiles[profile].template}"
-            )
             template = ClashTemplate.load(config.profiles[profile].template)
-            clash = template.render(proxies)
-            if clash.rule_providers:
-                for provider in clash.rule_providers:
-                    rulesets[provider] = clash.rule_providers[provider].url
-                    clash.rule_providers[provider].url = "/".join(
-                        [
-                            config.domian,
-                            config.urlprefix,
-                            "provider",
-                            f"{provider}.yaml",
-                        ]
-                    )
-            clash.save(profile)
+            if template.rule_providers:
+                for provider in template.rule_providers:
+                    rulesets[provider] = template.rule_providers[provider].url
         await Download.provider(rulesets)
         logger.success("Update complete")
 
     except Exception as e:
         logger.critical(e)
         return e
```

### Comparing `liteclashproman-0.3.0/LiteClashProMan/subscribe/base64.py` & `liteclashproman-0.4.0/LiteClashProMan/subscribe/base64.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/subscribe/clash.py` & `liteclashproman-0.4.0/LiteClashProMan/subscribe/clash.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/subscribe/jms.py` & `liteclashproman-0.4.0/LiteClashProMan/subscribe/jms.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/LiteClashProMan/utils.py` & `liteclashproman-0.4.0/LiteClashProMan/utils.py`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/README.md` & `liteclashproman-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `liteclashproman-0.3.0/pyproject.toml` & `liteclashproman-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "LiteClashProMan"
-version = "0.3.0"
+version = "0.4.0"
 description = "生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。"
 authors = [
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "pyyaml>=6.0",
     "fastapi[all]>=0.96.0",
```

### Comparing `liteclashproman-0.3.0/PKG-INFO` & `liteclashproman-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiteClashProMan
-Version: 0.3.0
+Version: 0.4.0
 Summary: 生成并更新 clash 配置文件，并提供 http 下载和规则文件镜像下载。
 Author-Email: Well404 <well_404@outlook.com>
 License: APGL-3.0
 Requires-Python: >=3.8
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: fastapi[all]>=0.96.0
 Requires-Dist: httpx>=0.24.1
```

