# Comparing `tmp/porn_cli-1.0.5.tar.gz` & `tmp/porn_cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "porn_cli-1.0.5.tar", max compression
+gzip compressed data, was "porn_cli-1.0.6.tar", max compression
```

## Comparing `porn_cli-1.0.5.tar` & `porn_cli-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-07-24 20:02:06.740492 porn_cli-1.0.5/LICENSE
--rw-r--r--   0        0        0     2653 2023-07-24 20:02:06.740492 porn_cli-1.0.5/README.md
--rw-r--r--   0        0        0       23 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/__init__.py
--rw-r--r--   0        0        0      169 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/__main__.py
--rw-r--r--   0        0        0        0 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/hentaimama.py
--rw-r--r--   0        0        0     3092 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/javct.py
--rw-r--r--   0        0        0     1400 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/pornhub.py
--rw-r--r--   0        0        0     1810 2023-07-24 20:02:06.740492 porn_cli-1.0.5/porn_cli/websites/porn/xxxmax.py
--rw-r--r--   0        0        0      564 2023-07-24 20:02:06.740492 porn_cli-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 porn_cli-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 00:59:55.915689 porn_cli-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1789 2023-07-25 00:59:55.915689 porn_cli-1.0.6/README.md
+-rw-r--r--   0        0        0       23 2023-07-25 00:59:55.915689 porn_cli-1.0.6/porn_cli/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-25 00:59:55.915689 porn_cli-1.0.6/porn_cli/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-25 00:59:55.915689 porn_cli-1.0.6/porn_cli/websites/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 00:59:55.915689 porn_cli-1.0.6/porn_cli/websites/porn/__init__.py
+-rw-r--r--   0        0        0     2158 2023-07-25 00:59:55.915689 porn_cli-1.0.6/porn_cli/websites/porn/hentaimama.py
+-rw-r--r--   0        0        0     2536 2023-07-25 00:59:55.915689 porn_cli-1.0.6/porn_cli/websites/porn/javct.py
+-rw-r--r--   0        0        0     1493 2023-07-25 00:59:55.915689 porn_cli-1.0.6/porn_cli/websites/porn/pornhub.py
+-rw-r--r--   0        0        0     1822 2023-07-25 00:59:55.915689 porn_cli-1.0.6/porn_cli/websites/porn/xxxmax.py
+-rw-r--r--   0        0        0      502 2023-07-25 00:59:55.915689 porn_cli-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 porn_cli-1.0.6/PKG-INFO
```

### Comparing `porn_cli-1.0.5/LICENSE` & `porn_cli-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `porn_cli-1.0.5/porn_cli/websites/porn/hentaimama.py` & `porn_cli-1.0.6/porn_cli/websites/porn/xxxmax.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,50 @@
-from mov_cli.utils.scraper import WebScraper
 from bs4 import BeautifulSoup as BS
+from mov_cli.utils.scraper import WebScraper
+from mov_cli.utils.props import SelectedNotAvailable
 import re
-
+from urllib.parse import unquote
+from base64 import b64decode
 
 class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
-
+    
     def search(self, q: str):
         q = (
             input("[!] Please Enter the name of the Porn: ")
             if q is None
             else q
         )
-        return q
+        return q.replace(" ", "+")
     
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/?s={data}").text
-        soup = BS(req, "lxml")
-        items = soup.findAll("div", {"class": "result-item"})
+        soup = BS(req, self.scraper)
+        items = soup.findAll("article", {"class": "thumb-block"})
         urls = [items[i].find("a")["href"] for i in range(len(items))]
-        title = [items[i].find("img")["alt"] for i in range(len(items))]
+        title = [items[i].find("a")["title"] for i in range(len(items))]
         ids = [i for i in range(len(items))]
-        mov_or_tv = ["Hentai" for i in range(len(items))]
+        mov_or_tv = ["Porn" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
-
-    def ask(self, url):
-        req = self.client.get(url).text
-        soup = BS(req, "lxml")
-        episodes = soup.findAll("article", {"class": "item se episodes"})
-        print(episodes)
-        episode = int(self.askepisode(len(episodes)))
-        episodes = episodes[::-1]
-        url = episodes[episode - 1].find("a")["href"]
-        return url, episode
-
+    
     def cdn_url(self, url):
-        req = self.client.get(url)
-        soup = BS(req, "lxml")
-        link = soup.find("div", {"id": "option-1"}).find("iframe")["src"]
-        q = self.client.get(link).text
-        regex1 = 'file: "(.*?)"'
-        regex2 = 'source src="(.*?)"'
+        req = self.client.get(url).text
+        soup = BS(req, self.scraper)
+        items = soup.find("div", {"class": "responsive-player"})
         try:
-            url = re.findall(regex1, q)[0]
-        except IndexError:
-            url = re.findall(regex2, q)[0]
-        print(url)
+            iframe = items.find("iframe")["src"]
+        except AttributeError:
+            raise SelectedNotAvailable
+        encrypted = re.findall('q=(.*)', iframe)[0]
+        decrypted = unquote(str(b64decode(encrypted)))
+        url = re.findall('src="(.*?)"', decrypted)[0]
         return url
     
-    def TV_PandDP(self, t: list, state: str = "d" or "p" or "sd"):
-        name = t[self.title]
-        url, episode = self.ask(t[self.url])
-        url = self.cdn_url(url)
+    def MOV_PandDP(self, m: list, state: str = "d" or "p"):
+        name = m[self.title]
+        url = self.cdn_url(m[self.url])
         if state == "d":
-            self.dl(url, name, season=".", episode=episode)
+            self.dl(url, name)
             return
-        self.play(url, name)
+        self.play(url, name, referrer=m[self.url])
```

### Comparing `porn_cli-1.0.5/porn_cli/websites/porn/javct.py` & `porn_cli-1.0.6/porn_cli/websites/porn/javct.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from bs4 import BeautifulSoup as BS
 from mov_cli.utils.scraper import WebScraper
+from mov_cli.extractors.doodstream import dood
 import re
 from base64 import b64encode
 
 class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
@@ -14,25 +15,25 @@
             if q is None
             else q
         )
         return q
     
     def results(self, data: str) -> list:
         req = self.client.get(f"{self.base_url}/search/{data}").text
-        soup = BS(req, "lxml")
+        soup = BS(req, self.scraper)
         items = soup.findAll("div", {"class": "card__content"})
         urls = [items[i].find("a")["href"] for i in range(len(items))]
         title = [items[i].find("span").find("a").text + " | " + items[i].find("h3").find("a").text  for i in range(len(items))]
         ids = [i for i in range(len(items))]
         mov_or_tv = ["Porn" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def doodext(self, url):
         req = self.client.get(url).text
-        soup = BS(req, "lxml")
+        soup = BS(req, self.scraper)
         search = soup.prettify()
         token = re.findall(r'name="_token" value="(.*?)"', search)[0]
         socket = re.findall(r'name="_socket" value="(.*?)"', search)[0]
         key = f"{token}:{socket}"
         key = key.encode('ascii')
         auth = b64encode(key).decode("UTF-8")
         serverlist = soup.findAll("li", {"class": "switch-source"})
@@ -45,30 +46,19 @@
         server = dood[0]
         datasource = server["data-source"]
         dataep = server["data-episode"]
         self.client.set_headers({"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/109.0", "Referer": url, "Authorization": f"Basic {auth}"})
         response = self.client.post(f"{self.base_url}/ajax/player", {"episode": dataep, "filmId": datasource}).text 
         url = re.findall(r"[a-z]+.[a-z]+\\\/e\\\/(.*?)\\", response)[0]
         return url
-    
-    def doodstream(self, suffix):
-        domain = "https://dood.wf"
-        req = self.client.get(f"{domain}/e/{suffix}").text
-        pass_md = re.findall(r"/pass_md5/[^']*", req)[0]
-        token = pass_md.split("/")[-1]
-        self.client.set_headers({"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0", "Referer": f"{domain}/e/{suffix}", "Accept-Language": "en-GB,en;q=0.5"})
-        drylink = self.client.get(f"{domain}{pass_md}").text
-        streamlink = f"{drylink}zUEJeL3mUN?token={token}"
-        print(streamlink)
-        return streamlink
         
     def MOV_PandDP(self, m: list, state: str = "d" or "p" or "sd"):
         name = m[self.title]
         suffix = self.doodext(m[self.url])
-        url = self.doodstream(suffix)
+        url = dood(suffix)
         if state == "d":
             self.dl(url, name)
             return
         self.play(url, name)
```

### Comparing `porn_cli-1.0.5/porn_cli/websites/porn/pornhub.py` & `porn_cli-1.0.6/porn_cli/websites/porn/pornhub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from bs4 import BeautifulSoup as BS
 from mov_cli.utils.scraper import WebScraper
+from time import sleep
 
 class Provider(WebScraper):
     def __init__(self, base_url):
         super().__init__(base_url)
         self.base_url = base_url
     
     def search(self, q: str):
@@ -11,16 +12,17 @@
             input("[!] Please Enter the name of the Porn: ")
             if q is None
             else q
         )
         return q.replace(" ", "+")
 
     def results(self, data: str) -> list:
+        self.client.set_cookies({"accessAgeDisclaimerPH": "1"})
         req = self.client.get(f"{self.base_url}/video/search?search={data}")
-        soup = BS(req, "lxml")
+        soup = BS(req, self.scraper)
         items = soup.findAll("li", {"class": "pcVideoListItem"})
         urls = [items[i].find("a")["href"] for i in range(len(items))]
         title = [items[i].find("div", {"class": "usernameWrap"}).find("a").text + " | " + items[i].find("a")["title"] + " | " for i in range(len(items))]
         ids = [items[i]["data-video-vkey"] for i in range(len(items))]
         mov_or_tv = ["Porn" for i in range(len(items))]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
```

### Comparing `porn_cli-1.0.5/PKG-INFO` & `porn_cli-1.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porn-cli
-Version: 1.0.5
+Version: 1.0.6
 Summary: An ani-cli like cli tool for porn
 Home-page: https://github.com/mov-cli/porn-cli
 License: GPLv3
 Author: mov-cli
 Author-email: mov-cli@protonmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -46,47 +46,20 @@
     <img src="https://user-images.githubusercontent.com/83706294/216816435-15cd8441-7a20-4f95-9024-d0d3ea96c2ba.png" alt="Logo" width="80" height="80">
   </a>
 
   <p align="center">
     A cli tool to browse and watch porn.
     <br />
     <br />
-    <a href="https://github.com/mov-cli/porn-cli/issues">Report Bug</a>
+    <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
     ·
-    <a href="https://github.com/mov-cli/porn-cli/issues">Request Feature</a>
+    <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
   </p>
 </div>
 
-<!-- TABLE OF CONTENTS -->
-<details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li>
-      <a href="#about-the-project">About The Project</a>
-    </li>
-    <li>
-      <a href="#getting-started">Getting Started</a>
-      <ul>
-        <li><a href="#prerequisites">Prerequisites</a></li>
-        <li><a href="#installation">Installation</a></li>
-        <ul>
-          <li><a href="#windows-/-linux">Windows / Linux</a></li>
-          <li><a href="#android">Android</a></li>
-        </ul>
-      </ul>
-    </li>
-    <li><a href="#usage">Usage</a></li>
-    <li><a href="#disclaimer">Disclaimer</a></li>
-    <li><a href="#roadmap">Roadmap</a></li>
-    <li><a href="#contributing">Contributing</a></li>
-    <li><a href="#license">License</a></li>
-    <li><a href="#contact">Contact</a></li>
-    <li><a href="#inspiration">inspiration</a></li>
-  </ol>
-</details>
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
 porn-cli is a addition for [mov-cli](https://github.com/mov-cli/mov-cli).
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p
```

#### html2text {}

```diff
@@ -1,33 +1,19 @@
-Metadata-Version: 2.1 Name: porn-cli Version: 1.0.5 Summary: An ani-cli like
+Metadata-Version: 2.1 Name: porn-cli Version: 1.0.6 Summary: An ani-cli like
 cli tool for porn Home-page: https://github.com/mov-cli/porn-cli License: GPLv3
 Author: mov-cli Author-email: mov-cli@protonmail.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: mov-cli (>=1.4.6,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/mov-cli/porn-cli/issues Project-
 URL: Repository, https://github.com/mov-cli/porn-cli Description-Content-Type:
 text/markdown
                                     [Logo]
                      A cli tool to browse and watch porn.
 
                          Report_Bug Â· Request_Feature
-  Table of Contents
-   1. About_The_Project
-   2. Getting_Started
-          o Prerequisites
-          o Installation
-                # Windows_/_Linux
-                # Android
-   3. Usage
-   4. Disclaimer
-   5. Roadmap
-   6. Contributing
-   7. License
-   8. Contact
-   9. inspiration
-  ## About The Project porn-cli is a addition for [mov-cli](https://github.com/
+ ## About The Project porn-cli is a addition for [mov-cli](https://github.com/
 mov-cli/mov-cli).
   (back_to_top)!-- GETTING STARTED --> ## Getting Started Firstly install [mov-
 cli](https://github.com/mov-cli/mov-cli) ``` pip install mov-cli ``` After that
                          you can install porn-cli ``` pip install porn-cli ```
```

