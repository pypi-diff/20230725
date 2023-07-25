# Comparing `tmp/yxr_codeforces_core-0.0.2.1.tar.gz` & `tmp/yxr_codeforces_core-0.0.2.2.tar.gz`

## Comparing `yxr_codeforces_core-0.0.2.1.tar` & `yxr_codeforces_core-0.0.2.2.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/__init__.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/account.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/constants.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/contest_list.py
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/contest_meta.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/contest_register.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/contest_standing.py
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/httphelper.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/language.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/problem.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/problems.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/py.typed
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/submit.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/url.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/util.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/websocket.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/interfaces/AioHttpHelper.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/codeforces_core/interfaces/__init__.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/LICENSE
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/README.md
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/__init__.py
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/account.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/constants.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/contest_list.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/contest_meta.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/contest_register.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/contest_standing.py
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/httphelper.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/kwargs.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/language.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/logging.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/problem.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/problems.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/py.typed
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/submit.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/url.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/util.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/websocket.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/interfaces/AioHttpHelper.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/codeforces_core/interfaces/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/LICENSE
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/README.md
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 yxr_codeforces_core-0.0.2.2/PKG-INFO
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/account.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/account.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
-from typing import Tuple
+from typing import Optional, Tuple
 from random import choice
 from lxml import html
 from lxml.html import HtmlElement
 import logging
 
-from codeforces_core.util import typedxpath
-
+from .kwargs import extract_common_kwargs
+from .util import typedxpath
 from .interfaces.AioHttpHelper import AioHttpHelperInterface
 
 default_login_url = "/enter?back=%2F"
 
 
 @dataclass
 class LoginResult:
@@ -30,64 +30,65 @@
   links = typedxpath(doc, './/div[@class="lang-chooser"]/div[not(@style)]/a[@href]')
   for m in links:
     if m.text.strip() in ["Register", "Enter"]:
       return False
   return True
 
 
-async def async_fetch_logged_in(http: AioHttpHelperInterface, login_url=default_login_url) -> Tuple[bool, str]:
+async def async_fetch_logged_in(http: AioHttpHelperInterface, login_url=default_login_url, **kw) -> Tuple[bool, str]:
   """
     auto update token 
     return bool(is_logged_in), html_data
   """
+  logger = extract_common_kwargs(**kw).logger
+
   html_data = await http.async_get(login_url)
-  try:
-    uc, usmc, cc, pc, csrf_token, ftaa, bfaa = extract_channel(html_data)
-  except Exception as e:
-    uc, usmc, cc, pc, csrf_token, ftaa, bfaa = '', '', '', '', '', '', ''
-    logging.error(str(e))
+  uc, usmc, cc, pc, csrf_token, ftaa, bfaa = extract_channel(html_data, logger=logger)
 
   if is_user_logged_in(html_data=html_data):
     http.update_tokens(csrf=csrf_token, ftaa=ftaa, bfaa=bfaa, uc=uc, usmc=usmc)
     return True, html_data
   return False, ''
 
 
-def extract_channel(html_data: str) -> Tuple[str, str, str, str, str, str, str]:
+# No exception, handler inside
+def extract_channel(html_data: str,
+                    logger: Optional[logging.Logger] = None) -> Tuple[str, str, str, str, str, str, str]:
   doc = html.fromstring(html_data)
 
   def xpath_content(el: HtmlElement, s: str) -> str:
     try:
       l = typedxpath(el, s)
       return l[0].get('content') if len(l) > 0 else ''
     except Exception as e:
-      logging.exception(e)
+      if logger: logger.exception(e)
       return ''
 
   uc = xpath_content(doc, './/meta[@name="uc"]')
   usmc = xpath_content(doc, './/meta[@name="usmc"]')
   cc = xpath_content(doc, './/meta[@name="cc"]')
   pc = xpath_content(doc, './/meta[@name="pc"]')
   try:
     csrf_token = typedxpath(doc, './/span[@class="csrf-token"]')[0].get('data-csrf')
     assert len(csrf_token) == 32, "Invalid CSRF token"
   except Exception as e:
-    logging.exception(e)
+    if logger: logger.exception(e)
     csrf_token = ''
   ftaa = ''.join([choice('abcdefghijklmnopqrstuvwxyz0123456789') for x in range(18)])
   # bfaa : Fingerprint2.x64hash128
   bfaa = ''.join([choice('0123456789abcdef') for x in range(32)])
   return uc, usmc, cc, pc, csrf_token, ftaa, bfaa
 
 
 # TODO 已经登陆账号A, 再调用登陆账号B是不行的, 这个逻辑应该是由外部控制，调用时应该确保未登录状态
 async def async_login(http: AioHttpHelperInterface,
                       handle: str,
                       password: str,
-                      login_url=default_login_url) -> LoginResult:
+                      login_url=default_login_url,
+                      **kw) -> LoginResult:
   """
     This method will use ``http`` for login request, and  :py:func:`is_user_logged_in()` for login check
 
     :param handle: Codeforces handle
     :param password: Codeforces password
 
     :returns: if it is successful post and logged
@@ -110,28 +111,29 @@
           html_data = await http.async_get('https://codeforces.com')
           assert(is_user_logged_in(html_data))
 
           await http.close_session()
 
         asyncio.run(demo())
   """
+  logger = extract_common_kwargs(**kw).logger
   html_data = await http.async_get(login_url)
-  csrf_token, ftaa, bfaa = extract_channel(html_data)[4:7]
+  csrf_token, ftaa, bfaa = extract_channel(html_data, logger=logger)[4:7]
   login_data = {
       'csrf_token': csrf_token,
       'action': 'enter',
       'ftaa': ftaa,
       'bfaa': bfaa,
       'handleOrEmail': handle,
       'password': password,
       'remember': 'on',
   }
   html_data = await http.async_post(login_url, login_data)
   # uc, usmc, cc, pc, csrf_token, ftaa, bfaa = extract_channel(html_data)
-  uc, usmc, cc, pc = extract_channel(html_data)[0:4]
+  uc, usmc, cc, pc = extract_channel(html_data, logger=logger)[0:4]
 
   success = False
   # if check_login(result.html):
   if is_user_logged_in(html_data=html_data):
     http.update_tokens(csrf=csrf_token, ftaa=ftaa, bfaa=bfaa, uc=uc, usmc=usmc)
     success = True
   else:
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/contest_list.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/contest_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from dataclasses import dataclass
 import json
-import logging
 import re
 from typing import List
 from lxml import html
 from lxml.etree import ElementBase
 from datetime import datetime, timedelta
 
-from codeforces_core.interfaces.AioHttpHelper import AioHttpHelperInterface
-from codeforces_core.util import typedxpath
-
-logger = logging.getLogger(__name__)
+from .interfaces.AioHttpHelper import AioHttpHelperInterface
+from .kwargs import extract_common_kwargs
+from .util import typedxpath
 
 
 @dataclass
 class CodeforcesUser:
   name: str
   title: str
   class__: str
@@ -73,15 +71,16 @@
 
 @dataclass
 class ContestList:
   upcomming: List[ContestListItem]
   history: List[ContestListItem]
 
 
-def parse_contest_list(raw_contests: ElementBase, upcoming: bool) -> List[ContestListItem]:
+def parse_contest_list(raw_contests: ElementBase, upcoming: bool, **kw) -> List[ContestListItem]:
+  logger = extract_common_kwargs(**kw).logger
   contests: List[ContestListItem] = []
 
   for c in typedxpath(raw_contests, './/tr[@data-contestid]'):
     try:
       cid = int(c.get('data-contestid'))
       td = typedxpath(c, './/td')
       title = td[0].text.lstrip().splitlines()[0]
@@ -119,15 +118,15 @@
                           Div=parse_div(title)))
     except Exception as e:
       logger.exception(e)
   return contests
 
 
 # This function is to simulate web request, do not do the cache
-async def async_contest_list(http: AioHttpHelperInterface, page: int = 1) -> ContestList:
+async def async_contest_list(http: AioHttpHelperInterface, page: int = 1, **kw) -> ContestList:
   """
     This method will use ``http`` for get contests page, you can both login or not login
 
     :param page: the page in url
 
     :returns: the result
 
@@ -149,14 +148,15 @@
               print(c)
           for c in result.history[:5]:
               print(c)
           await http.close_session()
 
         asyncio.run(demo())
   """
+  logger = extract_common_kwargs(**kw).logger
   doc = html.fromstring(await http.async_get(f'/contests/page/{page}?complete=true'))
   table = typedxpath(doc, './/div[@class="datatable"]')
   upcoming = parse_contest_list(table[0], upcoming=True)
 
   # count contests
   if len(table[1].xpath('.//tr[@data-contestid]')) == 0:
     logger.error("[!] Contest is running or countdown")
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/contest_meta.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/contest_meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import List, cast
 from bs4 import BeautifulSoup
 import bs4
 from lxml import html
 from lxml.etree import _Element
 from lxml.html import HtmlMixin
 
-from codeforces_core.interfaces.AioHttpHelper import AioHttpHelperInterface
-from codeforces_core.util import soup_find_bs4Tag
+from .interfaces.AioHttpHelper import AioHttpHelperInterface
+from .util import soup_find_bs4Tag
 
 
 class E_STATUS(str, Enum):
   NOT_SUBMITTED = ""
   AC = "AC"
   ERROR = "ERROR"
 
@@ -107,15 +107,15 @@
     links = cast(List[_Element], c.getparent().xpath('.//a[@href]'))
     for a in links:
       title_text = str(cast(HtmlMixin, html.fromstring(a.get('title'))).text_content())
       ret.append(Materials(text=title_text, url=a.get('href')))
   return ret
 
 
-async def async_contest_meta(http: AioHttpHelperInterface, contest_id: str) -> ContestPage:
+async def async_contest_meta(http: AioHttpHelperInterface, contest_id: str, **kw) -> ContestPage:
   """
     This method will use ``http`` to request ``/contest/<contest_id>``, and parse to struct result
 
     :param http: AioHttpHelperInterface 
     :param contest_id: contest id in url
 
     :returns: parsed structured result
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/contest_register.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/contest_register.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import List, cast
 from lxml import html
 from lxml.etree import _Element
 
-from codeforces_core.interfaces.AioHttpHelper import AioHttpHelperInterface
+from .interfaces.AioHttpHelper import AioHttpHelperInterface
 from . import util
 
 
 class RegisterResultMsg(str, Enum):
   HaveBeenRegistered = 'You have been successfully registered'  # first time message
   AlreadyRegistered = 'You are already registered for the contest'
   NoRegistrationIsOpenedNow = 'No registration is opened now'
@@ -19,15 +19,15 @@
 class RegisterResult:
   title: str = ''
   msg: RegisterResultMsg = RegisterResultMsg.Empty  # example: already register, TODO 有些比赛会 None
 
 
 # TODO 统一参数命名
 # Take part as individual participant
-async def async_register(http: AioHttpHelperInterface, contest_id: str) -> RegisterResult:
+async def async_register(http: AioHttpHelperInterface, contest_id: str, **kw) -> RegisterResult:
   """
     This method will use ``http`` for register request, you need login before
 
     :param contest_id: Codeforces contest_id in url
 
     :returns: the result
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/contest_standing.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/contest_standing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field
 import re
 from typing import List, Optional
 from bs4 import BeautifulSoup
 import bs4
 
-from codeforces_core.interfaces.AioHttpHelper import AioHttpHelperInterface
+from .interfaces.AioHttpHelper import AioHttpHelperInterface
 
 # TODO post toggle showunofficial
 
 
 @dataclass
 class StandingProblem:
   id: str = ''
@@ -88,15 +88,15 @@
         row.problems.append(problem)
     rows.append(row)
 
   # TODO add pagenation
   return Standing(head=h, rows=rows)
 
 
-async def async_friends_standing(http: AioHttpHelperInterface, contest_id: str) -> Standing:
+async def async_friends_standing(http: AioHttpHelperInterface, contest_id: str, **kw) -> Standing:
   """
     This method will use ``http`` to request ``/contest/<contest_id>/standings/friends/true``, and parse to struct result
 
     :param contest_id: contest id in url
 
     :returns: parsed structured result 
 
@@ -126,15 +126,15 @@
   url = f'/contest/{contest_id}/standings/friends/true'
   resp = await http.async_get(url)
   result = parseStandingHtml(resp)
   result.url = url
   return result
 
 
-async def async_common_standing(http: AioHttpHelperInterface, contest_id: str, page: str = '1') -> Standing:
+async def async_common_standing(http: AioHttpHelperInterface, contest_id: str, page: str = '1', **kw) -> Standing:
   """
     This method will use ``http`` to request ``/contest/<contest_id>/standings/page/<page>``, and parse to struct result
 
     :param contest_id: contest id in url
     :param page: pagination 1-index
 
     :returns: parsed structured result
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/httphelper.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/httphelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,29 +7,24 @@
 import aiohttp
 import pyaes
 import json
 import re
 
 from .constants import CF_HOST
 from .interfaces.AioHttpHelper import AioHttpHelperInterface
+from .kwargs import extract_common_kwargs
 
 default_headers = {
     'Accept': '*/*',
     'Accept-Encoding': 'gzip',
     # 'User-Agent': config.conf['user_agent'], TODO
     'User-Agent':
     'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36'
 }
 
-# session: aiohttp.ClientSession = None
-# tokens = {}
-# cookie_jar = None
-
-logger = logging.getLogger(__name__)
-
 
 class RCPCRedirectionError(Exception):
 
   def __init__(self):
     super().__init__("RCPC redirection detected")
 
 
@@ -46,23 +41,30 @@
 class HttpHelper(AioHttpHelperInterface):
   session: Optional[aiohttp.ClientSession] = None
   cookie_jar_path = ''
   cookie_jar: Optional[aiohttp.CookieJar] = None
   token_path = ''
   tokens: Dict[str, str] = {}
   headers: Dict[str, str] = {}  # TODO
+  logger: logging.Logger
 
-  def __init__(self, cookie_jar_path: str = '', token_path: str = '', headers=default_headers, host=CF_HOST) -> None:
+  def __init__(self,
+               cookie_jar_path: str = '',
+               token_path: str = '',
+               headers=default_headers,
+               host=CF_HOST,
+               **kw) -> None:
     # if path is empty string then won't save to any file, just store in memory
     self.cookie_jar_path = cookie_jar_path
     # if path is empty string then won't save to any file, just store in memory
     self.token_path = token_path
     self.headers = headers
     # TODO support cf mirror site?
     self.host = host
+    self.logger = extract_common_kwargs(**kw).logger
 
   @staticmethod
   def load_tokens(token_path: str) -> Dict[str, Any]:
     if token_path and path.isfile(token_path):
       with open(token_path, 'r') as f:
         return json.load(f)
     return {}
@@ -114,15 +116,15 @@
     except RCPCRedirectionError:
       async with self.session.get(url, headers=headers) as response:
         assert response.status == 200
         if self.cookie_jar_path:
           self.cookie_jar.save(file_path=self.cookie_jar_path)
         return await response.text()
     except Exception as e:
-      logger.error(e)
+      self.logger.error(e)
 
   async def async_post(self, url, data, headers=default_headers, csrf=False, **kwargs: Any):
     if self.session is None:
       raise Exception('Please open_session() before async_get()')
     if headers == None: headers = default_headers
     if csrf and 'csrf' in self.tokens:
       headers = add_header({'X-Csrf-Token': self.tokens['csrf']}, headers=headers)
@@ -139,15 +141,15 @@
     except RCPCRedirectionError:
       async with self.session.post(url, headers=headers, data=data) as response:
         assert response.status == 200
         if self.cookie_jar_path:
           self.cookie_jar.save(file_path=self.cookie_jar_path)
         return await response.text()
     except Exception as e:
-      logger.error(e)
+      self.logger.error(e)
 
   def get_tokens(self):
     return self.tokens
 
   def check_rcpc(self, html_data: str):
     doc = html.fromstring(html_data)
     aesmin = cast(List[_Element], doc.xpath(".//script[@type='text/javascript' and @src='/aes.min.js']"))
@@ -188,13 +190,13 @@
 
             endwatch, obj = callback(js)
             yield obj
             if endwatch:
               return
 
           else:
-            logger.error('wrong msg type?', msg.type)
+            self.logger.error('wrong msg type?', msg.type)
             break
         return
     except Exception as e:
-      logger.error(e)
+      self.logger.error(e)
       return
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/language.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/language.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from dataclasses import dataclass
 from typing import List
 from bs4 import BeautifulSoup
 import bs4
 
-from codeforces_core.interfaces.AioHttpHelper import AioHttpHelperInterface
+from .interfaces.AioHttpHelper import AioHttpHelperInterface
 
 
 @dataclass
 class Lang:
   text: str
   value: str
 
 
-async def async_language(http: AioHttpHelperInterface) -> List[Lang]:
+async def async_language(http: AioHttpHelperInterface, **kw) -> List[Lang]:
   """
     This method will use ``http`` to request ``/problemset/submit``, and parse language options
 
     :returns: parsed structured result 
 
     Examples:
 
@@ -44,8 +44,8 @@
   resp = await http.async_get(f'/problemset/submit')
   ret: List[Lang] = []
   soup = BeautifulSoup(resp, 'lxml')
   tags = soup.find('select', attrs={'name': 'programTypeId'})
   if isinstance(tags, bs4.Tag):
     for child in tags.find_all('option'):
       ret.append(Lang(value=child.get('value'), text=child.string))
-  return ret
+  return ret
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/problem.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/problem.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from typing import List
 from bs4 import BeautifulSoup
 import bs4
 
-from codeforces_core.interfaces.AioHttpHelper import AioHttpHelperInterface
+from .interfaces.AioHttpHelper import AioHttpHelperInterface
 
 
 @dataclass
 class TestCase:
   in_data: str
   out_data: str
 
@@ -43,15 +43,15 @@
   time_limit: str = ''
   mem_limit: str = ''
   url: str = ''
   html: str = ''
   file_path: str = ''
 
 
-async def async_problem(http: AioHttpHelperInterface, contest_id: str, level: str) -> ParseProblemResult:
+async def async_problem(http: AioHttpHelperInterface, contest_id: str, level: str, **kw) -> ParseProblemResult:
   """
     This method will use ``http`` to request ``/contest/<contest_id>/problems``, and parse to struct result
 
     :param http: AioHttpHelperInterface 
     :param contest_id: contest id in url
 
     :returns: parsed structured result 
@@ -104,8 +104,8 @@
     test_case_outputs = match_groups.find_all(name='div', attrs={'class': 'output'})
     assert (len(test_case_inputs) == len(test_case_outputs))  # may not? in April fool contest
     for i in range(len(test_case_inputs)):
       t_in = test_case_inputs[i].find(name='pre').get_text("\n").strip(" \r\n")
       t_out = test_case_outputs[i].find(name='pre').get_text("\n").strip(" \r\n")
       problem.test_cases.append(TestCase(t_in, t_out))
 
-  return problem
+  return problem
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/problems.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/problems.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 import logging
 from typing import Any, List, cast
 from lxml import html
 
-from codeforces_core.interfaces.AioHttpHelper import AioHttpHelperInterface
+from .interfaces.AioHttpHelper import AioHttpHelperInterface
+from .kwargs import extract_common_kwargs
 from .util import pop_element
 
 
 def extract_testcases(tags):
   ret = []
   for i in tags:
     pop_element(i.xpath('.//div[@class="title"]')[0])
@@ -45,15 +46,15 @@
   memory_limit_mb: str
   desc: str
   in_tc: List[str]
   out_tc: List[str]
   note: str
 
 
-async def async_problems(http: AioHttpHelperInterface, contest_id: str) -> List[ProblemInfo]:
+async def async_problems(http: AioHttpHelperInterface, contest_id: str, **kw) -> List[ProblemInfo]:
   """
     This method will use ``http`` to request ``/contest/<contest_id>/problems``, and parse to struct result
 
     :param http: AioHttpHelperInterface 
     :param contest_id: contest id in url
 
     :returns: parsed structured result 
@@ -74,14 +75,15 @@
           result = await async_problems(http=http, contest_id='1779')
           print(len(result))
           print(result[0])
           await http.close_session()
 
         asyncio.run(demo())
   """
+  logger = extract_common_kwargs(**kw).logger
   url = "/contest/{}/problems".format(contest_id)
   resp = await http.async_get(url)
   doc = html.fromstring(resp)
   probs = cast(List[Any], doc.xpath('.//div[@class="problemindexholder"]'))
 
   ret: List[ProblemInfo] = []
   for p in probs:
@@ -126,9 +128,9 @@
                       time_limit_seconds=time_limit,
                       memory_limit_mb=memory_limit,
                       desc=desc,
                       in_tc=in_tc,
                       out_tc=out_tc,
                       note=note))
     except Exception as e:
-      logging.exception(e)
+      logger.exception(e)
   return ret
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/submit.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/submit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from collections import defaultdict
 from dataclasses import dataclass, field
-import logging
 from os import path
 from typing import Any, List, Tuple
 from lxml import html
 
-from codeforces_core.util import typedxpath
-
 # from .ui import BLUE, GREEN, RED, redraw
+from .util import typedxpath
 from .account import is_user_logged_in
 from .interfaces.AioHttpHelper import AioHttpHelperInterface
+from .kwargs import extract_common_kwargs
 from .url import problem_url_parse
 
-logger = logging.getLogger(__name__)
-
 
-async def async_submit(http: AioHttpHelperInterface, contest_id: str, level: str, file_path: str,
-                       lang_id: str) -> Tuple[str, str]:
+async def async_submit(http: AioHttpHelperInterface, contest_id: str, level: str, file_path: str, lang_id: str,
+                       **kw) -> Tuple[str, str]:
   """
     This method will use ``http`` to post submit
 
     :param http: AioHttpHelperInterface 
     :param ws_handler: function to handler messages 
 
     :returns: (submission_id, html_text of contest/<contest id>/my )
@@ -56,14 +53,15 @@
           except asyncio.TimeoutError:
             pass
           await http.close_session()
 
         asyncio.run(demo())
 
   """
+  logger = extract_common_kwargs(**kw).logger
 
   if not contest_id or not level:
     logger.error("[!] Invalid contestID or level")
     return '', ''
   if not path.isfile(file_path):
     logger.error("[!] File not found : {}".format(file_path))
     return '', ''
@@ -119,15 +117,16 @@
     verdict = ''.join(td[5].itertext()).strip()
     prog_time = td[6].text.strip().replace('\xa0', ' ').split()[0]
     prog_mem = td[7].text.strip().replace('\xa0', ' ').split()[0]
     ret.append(SubmissionPageResult(id=submission_id, url=url, verdict=verdict, time_ms=prog_time, mem_bytes=prog_mem))
   return ret
 
 
-async def async_fetch_submission_page(http: AioHttpHelperInterface, problem_url: str) -> List[SubmissionPageResult]:
+async def async_fetch_submission_page(http: AioHttpHelperInterface, problem_url: str,
+                                      **kw) -> List[SubmissionPageResult]:
   contest_id, problem_key = problem_url_parse(problem_url)
   # 正常是 302 -> https://codeforces.com/contest/<contest id>/my
   html_page = await http.async_get(f'/contest/{contest_id}/my')
   result = parse_submit_status(html_page)
   return list(filter(lambda o: o.url.endswith(problem_key), result))
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/url.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/url.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/util.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/util.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/websocket.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/websocket.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-import asyncio
-import logging
 from time import time
 from typing import Any, Callable, Tuple, AsyncIterator
 
-from codeforces_core.account import extract_channel
-from codeforces_core.interfaces.AioHttpHelper import AioHttpHelperInterface
-from codeforces_core.submit import SubmissionWSResult
-
-logger = logging.getLogger(__name__)
+from .account import extract_channel
+from .interfaces.AioHttpHelper import AioHttpHelperInterface
+from .kwargs import extract_common_kwargs
+from .submit import SubmissionWSResult
 
 
 # return (end watch?, transform result)
 def display_ws(result: Any) -> Tuple[bool, Any]:
   print(result)
   return False, result
 
@@ -62,32 +59,36 @@
 #   print(ws_url)
 #   return asyncio.create_task(http.websockets(ws_url, ws_handler))
 
 
 # https://codeforces.com/contest/<contest_id>/my 会多出两个 meta
 #    <meta name="cc" content="xxx"/>
 #    <meta name="pc" content="yyy"/>
+#   TODO 设计上不太对, handler处理了数据, 结果也抛给了使用者, 应该handler 只关心是否停止, 而transform不应该在handler里处理
 # 这两个可以监听 题目测试时 的通过 百分比 变化
-async def create_contest_ws_task_yield(
-    http: AioHttpHelperInterface, contest_id: str,
-    ws_handler: Callable[[Any], Tuple[bool, Any]]) -> AsyncIterator[SubmissionWSResult]:
+async def create_contest_ws_task_yield(http: AioHttpHelperInterface, contest_id: str,
+                                       ws_handler: Callable[[Any], Tuple[bool, Any]],
+                                       **kw) -> AsyncIterator[SubmissionWSResult]:
   """
     This method will use ``http`` to create contest specific websocket, and ``ws_handler`` to handle each ws message
 
-    :param http: AioHttpHelperInterface 
+    :param http: AioHttpHelperInterface
     :param contest_id: contest id in the url
-    :param ws_handler: function to handler messages 
+    :param ws_handler: function to handler messages
 
     :returns: the task which run ws
 
     Examples:
 
     See docstring of :py:func:`codeforces_core.submit.async_submit()`
   """
+  logger = extract_common_kwargs(**kw).logger
   epoch = int(time() * 1000)  # s -> ms
   html_data = await http.async_get(f"/contest/{contest_id}/my")
-  cc, pc = extract_channel(html_data)[2:4]
+  cc, pc = extract_channel(html_data, logger)[2:4]
   assert cc and pc
   ws_url = f"wss://pubsub.codeforces.com/ws/s_{pc}/s_{cc}?_={epoch}&tag=&time=&eventid="
-  logger.info("ws_url:", ws_url)
+  logger.debug(f"pc = {pc}")  # 似乎和场次有关, 可能包含别人的?
+  logger.debug(f"cc = {cc}")  # 似乎只会包含自己的
+  logger.debug(f"ws_url = {ws_url}")
   async for data in http.websockets(ws_url, ws_handler):
     yield data
```

### Comparing `yxr_codeforces_core-0.0.2.1/codeforces_core/interfaces/AioHttpHelper.py` & `yxr_codeforces_core-0.0.2.2/codeforces_core/interfaces/AioHttpHelper.py`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.1/.gitignore` & `yxr_codeforces_core-0.0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.1/LICENSE` & `yxr_codeforces_core-0.0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.1/README.md` & `yxr_codeforces_core-0.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.1/pyproject.toml` & `yxr_codeforces_core-0.0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yxr_codeforces_core-0.0.2.1/PKG-INFO` & `yxr_codeforces_core-0.0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yxr-codeforces-core
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: Simple Codeforces core api
 Project-URL: Homepage, https://github.com/CroMarmot/yxr-codeforces-core
 Project-URL: Bug Tracker, https://github.com/CroMarmot/yxr-codeforces-core/issues
 Author-email: YeXiaoRain <yexiaorain@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 陈鼫RWHTYFZ
```

