# Comparing `tmp/crossposter-0.5.2.tar.gz` & `tmp/crossposter-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossposter-0.5.2.tar", last modified: Mon Oct 24 10:35:05 2022, max compression
+gzip compressed data, was "crossposter-0.6.0.tar", last modified: Tue Jul 25 15:37:34 2023, max compression
```

## Comparing `crossposter-0.5.2.tar` & `crossposter-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2022-10-24 10:35:05.021643 crossposter-0.5.2/
--rw-rw-r--   0 meet      (1000) meet      (1000)     6058 2022-10-24 10:35:05.021643 crossposter-0.5.2/PKG-INFO
--rw-rw-r--   0 meet      (1000) meet      (1000)     5732 2022-10-24 10:29:02.000000 crossposter-0.5.2/README.md
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2022-10-24 10:35:04.997641 crossposter-0.5.2/crossposter/
--rw-rw-r--   0 meet      (1000) meet      (1000)       26 2022-10-24 10:29:02.000000 crossposter-0.5.2/crossposter/__init__.py
--rw-rw-r--   0 meet      (1000) meet      (1000)        0 2022-10-24 10:29:02.000000 crossposter-0.5.2/crossposter/__main__.py
--rw-rw-r--   0 meet      (1000) meet      (1000)     3902 2022-10-24 10:29:58.000000 crossposter-0.5.2/crossposter/app.py
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2022-10-24 10:35:05.021643 crossposter-0.5.2/crossposter/publications/
--rw-rw-r--   0 meet      (1000) meet      (1000)        0 2022-10-24 10:29:03.000000 crossposter-0.5.2/crossposter/publications/__init__.py
--rw-rw-r--   0 meet      (1000) meet      (1000)     2675 2022-10-24 10:31:33.000000 crossposter-0.5.2/crossposter/publications/codenewbie.py
--rw-rw-r--   0 meet      (1000) meet      (1000)     2922 2022-10-24 10:31:33.000000 crossposter-0.5.2/crossposter/publications/dev.py
--rw-rw-r--   0 meet      (1000) meet      (1000)     2262 2022-10-24 10:29:03.000000 crossposter-0.5.2/crossposter/publications/hashnode.py
--rw-rw-r--   0 meet      (1000) meet      (1000)     1895 2022-10-24 10:29:03.000000 crossposter-0.5.2/crossposter/publications/medium.py
--rw-rw-r--   0 meet      (1000) meet      (1000)     1738 2022-10-24 10:31:24.000000 crossposter-0.5.2/crossposter/utils.py
-drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2022-10-24 10:35:05.021643 crossposter-0.5.2/crossposter.egg-info/
--rw-rw-r--   0 meet      (1000) meet      (1000)     6058 2022-10-24 10:35:03.000000 crossposter-0.5.2/crossposter.egg-info/PKG-INFO
--rw-rw-r--   0 meet      (1000) meet      (1000)      498 2022-10-24 10:35:03.000000 crossposter-0.5.2/crossposter.egg-info/SOURCES.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)        1 2022-10-24 10:35:03.000000 crossposter-0.5.2/crossposter.egg-info/dependency_links.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)       52 2022-10-24 10:35:03.000000 crossposter-0.5.2/crossposter.egg-info/entry_points.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)       40 2022-10-24 10:35:03.000000 crossposter-0.5.2/crossposter.egg-info/requires.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)       12 2022-10-24 10:35:03.000000 crossposter-0.5.2/crossposter.egg-info/top_level.txt
--rw-rw-r--   0 meet      (1000) meet      (1000)       38 2022-10-24 10:35:05.021643 crossposter-0.5.2/setup.cfg
--rw-rw-r--   0 meet      (1000) meet      (1000)      903 2022-10-24 10:32:18.000000 crossposter-0.5.2/setup.py
+drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2023-07-25 15:37:34.459487 crossposter-0.6.0/
+-rw-rw-r--   0 meet      (1000) meet      (1000)     6021 2023-07-25 15:37:34.459487 crossposter-0.6.0/PKG-INFO
+-rw-rw-r--   0 meet      (1000) meet      (1000)     5732 2023-07-25 15:29:57.000000 crossposter-0.6.0/README.md
+drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2023-07-25 15:37:34.451487 crossposter-0.6.0/crossposter/
+-rw-rw-r--   0 meet      (1000) meet      (1000)       26 2023-07-25 15:29:57.000000 crossposter-0.6.0/crossposter/__init__.py
+-rw-rw-r--   0 meet      (1000) meet      (1000)        0 2023-07-25 15:29:57.000000 crossposter-0.6.0/crossposter/__main__.py
+-rw-rw-r--   0 meet      (1000) meet      (1000)     4036 2023-07-25 15:30:43.000000 crossposter-0.6.0/crossposter/app.py
+drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2023-07-25 15:37:34.459487 crossposter-0.6.0/crossposter/publications/
+-rw-rw-r--   0 meet      (1000) meet      (1000)        0 2023-07-25 15:29:57.000000 crossposter-0.6.0/crossposter/publications/__init__.py
+-rw-rw-r--   0 meet      (1000) meet      (1000)     2872 2023-07-25 15:31:25.000000 crossposter-0.6.0/crossposter/publications/codenewbie.py
+-rw-rw-r--   0 meet      (1000) meet      (1000)     3042 2023-07-25 15:31:36.000000 crossposter-0.6.0/crossposter/publications/dev.py
+-rw-rw-r--   0 meet      (1000) meet      (1000)     2262 2023-07-25 15:29:57.000000 crossposter-0.6.0/crossposter/publications/hashnode.py
+-rw-rw-r--   0 meet      (1000) meet      (1000)     1895 2023-07-25 15:29:57.000000 crossposter-0.6.0/crossposter/publications/medium.py
+-rw-rw-r--   0 meet      (1000) meet      (1000)     2364 2023-07-25 15:31:00.000000 crossposter-0.6.0/crossposter/utils.py
+drwxrwxr-x   0 meet      (1000) meet      (1000)        0 2023-07-25 15:37:34.455487 crossposter-0.6.0/crossposter.egg-info/
+-rw-rw-r--   0 meet      (1000) meet      (1000)     6021 2023-07-25 15:37:32.000000 crossposter-0.6.0/crossposter.egg-info/PKG-INFO
+-rw-rw-r--   0 meet      (1000) meet      (1000)      498 2023-07-25 15:37:33.000000 crossposter-0.6.0/crossposter.egg-info/SOURCES.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)        1 2023-07-25 15:37:32.000000 crossposter-0.6.0/crossposter.egg-info/dependency_links.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)       51 2023-07-25 15:37:33.000000 crossposter-0.6.0/crossposter.egg-info/entry_points.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)       40 2023-07-25 15:37:33.000000 crossposter-0.6.0/crossposter.egg-info/requires.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)       12 2023-07-25 15:37:33.000000 crossposter-0.6.0/crossposter.egg-info/top_level.txt
+-rw-rw-r--   0 meet      (1000) meet      (1000)       38 2023-07-25 15:37:34.459487 crossposter-0.6.0/setup.cfg
+-rw-rw-r--   0 meet      (1000) meet      (1000)      903 2023-07-25 15:30:23.000000 crossposter-0.6.0/setup.py
```

### Comparing `crossposter-0.5.2/PKG-INFO` & `crossposter-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: crossposter
-Version: 0.5.2
+Version: 0.6.0
 Summary: Crosspost your markdown articles to devto, medium, codenewbie and hashnode
 Home-page: https://github.com/Mr-Destructive/crossposter
 Author: Meet Gor
 Author-email: gormeet711@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ## Crossposter
 
 > Crosspost your articles to dev.to/medium.com/hashnode.com from the command line
 
 - Crossposter is a script(Python/BASH) to automate crossposting to platforms like dev.to, medium.com and hashnode.com. The script takes in markdown version of your post with a few inputs from you and posts it to those platforms. You would require a token/key for each of those platforms to post it from the command line.
@@ -170,9 +168,7 @@
 
 Lets see the script in action 
 
 ![dev.to](https://gitlab.com/MR_DESTRUCTIVE/tblog-img/-/raw/main/devto.gif)
    
 If you want to add in more stuff to the post, you can check out the [DEV.to API docs](https://developers.forem.com/api#operation/createArticle) which is powered by [Forem](https://www.forem.com/), there a ton of options you can hook to the front-matter in the shellscript.
 
-
-
```

### Comparing `crossposter-0.5.2/README.md` & `crossposter-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `crossposter-0.5.2/crossposter/app.py` & `crossposter-0.6.0/crossposter/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 import sys
 import json
 import frontmatter
 import argparse
 from rich import print
 from pathlib import Path
-from .utils import generate_file
-from .publications.dev import devto
+from .publications.dev import devto, generate_devto_file
 from .publications.codenewbie import codenewbie
 from .publications.hashnode import hashnode
 from .publications.medium import medium
 
-
 def get_default_or_input(dictionary, keys):
     for key in keys:
         if key in dictionary.keys():
             return dictionary[key]
     return input(f"Enter the {keys[0]} for post: ")
 
 
 def main():
     print("[bold green]Crossposter[/ bold green]")
-    if len(sys.argv) < 2:
+    if len(sys.argv)<2:
         file_markdown = input("Enter the filename: ")
     else:
         file_markdown = sys.argv[1]
 
     while not file_markdown:
         print(f"No File Found with name {file_markdown}!")
         file_markdown = input("Enter the filename: ")
         if file_markdown:
             if Path(file_markdown).exists():
                 break
             else:
                 continue
 
     parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "Path",
-        metavar="path",
-        type=str,
-        nargs="?",
-        const=1,
-        default=file_markdown,
-        help="the path to file",
-    )
-    parser.add_argument("--dev", action="store_true", help="Post to dev.to")
-    parser.add_argument("--med", action="store_true", help="Post to medium.com")
-    parser.add_argument("--cdb", action="store_true", help="Post to codenewbie")
-    parser.add_argument("--opf", action="store_true", help="Save to a File")
+    parser.add_argument('Path', metavar='path', type=str, nargs='?', const=1, default=file_markdown, help='the path to file')
+    parser.add_argument("--dev", action="store_true", help='Post to dev.to')
+    parser.add_argument("--med", action="store_true", help='Post to medium.com')
+    parser.add_argument("--cdb", action="store_true", help='Post to codenewbie')
+    parser.add_argument("--output-file", action="store_true", help="Save to a File")
+    parser.add_argument("--embeds", action="store_true", help="Enable Embeds(only for devto/codenewbie)")
     args = parser.parse_args()
     post = frontmatter.load(file_markdown)
 
     with open("config.json", "r") as out:
         config = json.load(out)
 
     output_folder = config["output_folder"]
@@ -61,21 +52,22 @@
 
     blog_link = config["blog_link"]
 
     article = {}
     article["title"] = get_default_or_input(post, ["title"])
     article["description"] = get_default_or_input(post, ["subtitle", "description"])
     slug = get_default_or_input(post, ["slug", "canonical_url"])
-    # while True:
+    #while True:
     #    if validators.url(slug):
     #        break
     #    else:
     #        slug = input("Enter a valid URL: ")
 
-    if "slug" in post:
+    if "slug" in post.keys():
+        print(blog_link)
         slug = blog_link + str(slug)
     image_url = get_default_or_input(post, ["image_url", "cover_image"])
 
     article["canonical_url"] = slug
     article["cover_image"] = image_url
     article["tags"] = get_default_or_input(post, ["tags"])
     # article['date']=post['date']
@@ -84,34 +76,37 @@
         article["published"] = "true"
     else:
         article["published"] = "false"
     article["body_markdown"] = post.content
     if "series" in post:
         article["series"] = post["series"]
 
+
     key_file = Path("keys.txt")
     if not key_file.exists():
         key_file.touch(exist_ok=True)
         with open(key_file, "r+") as f:
             lines = f.readlines()
             lines.append("dev.to:\n")
             lines.append("medium.com:\n")
             lines.append("hashnode:\n")
             lines.append("hashnode_id:\n")
             lines.append("codenewbie:\n")
             f.writelines(lines)
 
+
+    allow_embeds = args.embeds
     if args.dev:
-        devto(article, output)
+        devto(article, output, allow_embeds)
     elif args.med:
         medium(article, output)
     elif args.cdb:
-        codenewbie(article, output)
+        codenewbie(article, output, allow_embeds)
     elif args.opf:
-        generate_file(article, output)
+        generate_devto_file(article, output)
     else:
         print(f"1. dev.to \n2. hashnode.com\n3. codenewbie\n4. medium.com\n")
         opt = input("Where you would like to post? (1/2/3/4) : ")
         if opt == "1":
             devto(article, output)
         elif opt == "2":
             hashnode(article, output)
```

### Comparing `crossposter-0.5.2/crossposter/publications/codenewbie.py` & `crossposter-0.6.0/crossposter/publications/codenewbie.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import requests
 import json
-import sys
-from crossposter.utils import hard_to_soft_wraps, replace_line
+from crossposter.utils import hard_to_soft_wraps, replace_line, embeds
 
 
 def codenewbie_file(article, output):
     codenewbie_frontmatter = "---\n"
     post = {}
     for key in article:
         post[key] = article[key]
@@ -14,51 +13,56 @@
         else:
             if post[key]:
                 if not key == "published":
                     codenewbie_frontmatter += f'{key}: "{post[key]}"\n'
                 else:
                     codenewbie_frontmatter += f"{key}: {post[key]}\n"
 
+
     lines = hard_to_soft_wraps(codenewbie_frontmatter)
 
     filename = post["title"].replace(" ", "_").lower()
     output_file = output / f"{filename}_codenewbie_post.md"
-    with open(output_file, "w") as f:
+    with open(output_file, 'w') as f:
         f.writelines(lines)
     print("The Codenewbie frontmatter is generated in the file -> ", output_file)
     return post
 
 
-def codenewbie(article, output):
+def codenewbie(article, output, allow_embeds=False):
 
     from rich.progress import Progress
-
     with Progress() as progress:
-        task = progress.add_task("Crossposting..", total=100)
+        task = progress.add_task("Crossposting..",  total=100)
         while not progress.finished:
             progress.update(task, advance=10)
 
     codenewbie_keys = []
     for line in open("keys.txt", "r"):
         if line.startswith("codenewbie:"):
             codenewbie_keys = line.split("codenewbie:")[1]
 
     if codenewbie_keys != "\n":
         codenewbie_keys = codenewbie_keys.strip()
     else:
         codenewbie_keys = input("Enter the Codenewbie API Key: ")
         replace_line("keys.txt", 4, f"dev.to: {codenewbie_keys}\n")
 
+
     post = codenewbie_file(article, output)
 
     post = {}
 
     for key in article:
         post[key] = article[key]
 
+    # replace github and other embed links
+    if allow_embeds:
+        post = embeds(post)
+
     API_ENDPOINT = "https://community.codenewbie.org/api/articles"
 
     data = {
         "Content-Type": "application/json",
         "article": post,
     }
     header = {"api-key": codenewbie_keys}
@@ -83,7 +87,10 @@
         response = requests.post(url=API_ENDPOINT, json=data, headers=header).json()
         if "url" in response:
             print("The article URL is: ", response["url"])
         else:
             print("The article URL is: ", response)
     else:
         print("Article already published")
+
+def generate_codenewbie_file(article, output):
+    codenewbie_file(article, output)
```

### Comparing `crossposter-0.5.2/crossposter/publications/dev.py` & `crossposter-0.6.0/crossposter/publications/dev.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 import json
-from crossposter.utils import hard_to_soft_wraps, replace_line
+from crossposter.utils import embeds, hard_to_soft_wraps, replace_line
 
 
 def devto_file(article, output):
     print("Cross-Posting on dev.to")
 
     dev_frontmatter = "---\n"
     post = {}
@@ -15,27 +15,26 @@
         else:
             if post[key]:
                 if not key == "published":
                     dev_frontmatter += f'{key}: "{post[key]}"\n'
                 else:
                     dev_frontmatter += f"{key}: {post[key]}\n"
 
+
     filename = post["title"].replace(" ", "_").lower()
     output_file = output / f"{filename}_dev_post.md"
 
-    import re
-
     lines = hard_to_soft_wraps(dev_frontmatter)
-    with open(output_file, "w") as f:
+    with open(output_file, 'w') as f:
         f.writelines(lines)
     print("The DEV frontmatter is generated in the file -> ", output_file)
     return post
 
 
-def devto(article, output):
+def devto(article, output, allow_embeds=False):
 
     post = devto_file(article, output)
 
     dev_keys = []
     for line in open("keys.txt", "r"):
         if line.startswith("dev.to:"):
             dev_keys = line.split("dev.to:")[1]
@@ -43,14 +42,17 @@
     if dev_keys != "\n":
         dev_keys = dev_keys.strip()
     else:
         dev_keys = input("Enter the DEV API Key: ")
         replace_line("keys.txt", 0, f"dev.to: {dev_keys}\n")
     API_ENDPOINT = "https://dev.to/api/articles"
 
+    if allow_embeds:
+        post = embeds(post)
+
     data = {
         "Content-Type": "application/json",
         "article": post,
     }
     """
     data = {
             'Content-Type': 'application/json',
@@ -66,28 +68,32 @@
             },
         }
     """
     header = {"api-key": dev_keys}
     flag = True
     # author_data = json.loads(requests.get("https://dev.to/api/users/me", headers=header).content)
     # author_username = author_data["username"]
+
+
     author_articles_list = json.loads(
         requests.get("https://dev.to/api/articles/me/published", headers=header).content
     )
     for article_data in author_articles_list:
         if article["body_markdown"] == article_data["body_markdown"]:
             flag = False
             print("ERRR!!!")
             break
         if article["title"] == article_data["title"]:
             flag = False
 
     if flag:
-        response = requests.post(
-            url=API_ENDPOINT, json=data, headers={"api-key": dev_keys}
-        ).json()
+        response = requests.post(url=API_ENDPOINT, json=data, headers={"api-key": dev_keys}).json()
         if "url" in response:
             print("The article URL is: ", response["url"])
         else:
             print("The article URL is: ", response)
     else:
         print("Article already published")
+
+
+def generate_devto_file(article, output):
+    devto_file(article, output)
```

### Comparing `crossposter-0.5.2/crossposter/publications/hashnode.py` & `crossposter-0.6.0/crossposter/publications/hashnode.py`

 * *Files identical despite different names*

### Comparing `crossposter-0.5.2/crossposter/publications/medium.py` & `crossposter-0.6.0/crossposter/publications/medium.py`

 * *Files identical despite different names*

### Comparing `crossposter-0.5.2/crossposter/utils.py` & `crossposter-0.6.0/crossposter/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import re
-from crossposter.publications.codenewbie import codenewbie_file
-
-from crossposter.publications.dev import devto_file
 
 
 def replace_line(file_name, line_num, text):
     with open(file_name, "r+") as f:
         lines = f.readlines()
         lines[line_num] = text
         f.truncate(0)
         f.seek(0)
         f.writelines(lines)
 
-
 def hard_to_soft_wraps(content):
-    # pre= re.findall(r'\n---\n(.*?)\n```.*$', content, re.DOTALL)
-    # mid = re.findall(r'\n```\n(.*?)\n```(.*?)',content, re.DOTALL)
-    # post = re.findall(r'\n```\n\n(.*$)', content, re.DOTALL)
+    #pre= re.findall(r'\n---\n(.*?)\n```.*$', content, re.DOTALL)
+    #mid = re.findall(r'\n```\n(.*?)\n```(.*?)',content, re.DOTALL)
+    #post = re.findall(r'\n```\n\n(.*$)', content, re.DOTALL)
 
     # get all fenced code block
-    fences = re.findall(r"\n```.*?```\n", content, re.DOTALL)
+    fences = re.findall(r'\n```.*?```\n', content, re.DOTALL)
 
     # get the frontmatter data
-    frontmatter = re.findall(r"---.*?---\n", content, re.DOTALL)
+    frontmatter = re.findall(r'---.*?---\n', content, re.DOTALL)
 
     for fence in fences:
         # set the new line character as some value //r to identify later
         content = content.replace(fence, fence.replace("\n", "\\r"))
     for attrib in frontmatter:
         content = content.replace(attrib, attrib.replace("\n", "\\r"))
 
@@ -37,16 +33,36 @@
     content = content.replace("\n#", "\\r\\r")
 
     # Split the text for iterating over the contents
     content = re.split("\\r\\r", content)
     for w in content:
         # replace the newline character which is a hard wrap into a whitespace
         # then replace the special character with new line character
-        content = w.replace("\n", " ").replace("\\r", "\n")
+        content = w.replace("\n", " ").replace('\\r', "\n")
 
     # returned soft wrapped content
     return content
 
 
-def generate_file(article, output):
-    devto_file(article, output)
-    codenewbie_file(article, output)
+def embeds(post):
+    github_regex = re.compile(r'\[([^\]]+)\]\(\s*(https?://github\.com/[^)]+)\s*\)')
+    twitter_regex = re.compile(r'\[([^\]]+)\]\(\s*https?://twitter\.com/([^)]+)\s*\)')
+
+    def embed_github_replace(match):
+        link_text = match.group(0)
+        github_link = match.group(2)
+        embeds = f'{link_text} {{% embed {github_link} %}}'
+        if len(github_link.split('/')) > 5:
+            return link_text
+        return embeds
+
+    def embed_twitter_replace(match):
+        link_text = match.group(0)
+        twitter_link = match.group(2)
+        embeds = f"{link_text} {{% embed https://twitter.com/{twitter_link} %}}"
+        return embeds
+
+    text = github_regex.sub(embed_github_replace, post["body_markdown"])
+    text = twitter_regex.sub(embed_twitter_replace, text)
+
+    post["body_markdown"] = text
+    return post
```

### Comparing `crossposter-0.5.2/crossposter.egg-info/PKG-INFO` & `crossposter-0.6.0/crossposter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: crossposter
-Version: 0.5.2
+Version: 0.6.0
 Summary: Crosspost your markdown articles to devto, medium, codenewbie and hashnode
 Home-page: https://github.com/Mr-Destructive/crossposter
 Author: Meet Gor
 Author-email: gormeet711@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ## Crossposter
 
 > Crosspost your articles to dev.to/medium.com/hashnode.com from the command line
 
 - Crossposter is a script(Python/BASH) to automate crossposting to platforms like dev.to, medium.com and hashnode.com. The script takes in markdown version of your post with a few inputs from you and posts it to those platforms. You would require a token/key for each of those platforms to post it from the command line.
@@ -170,9 +168,7 @@
 
 Lets see the script in action 
 
 ![dev.to](https://gitlab.com/MR_DESTRUCTIVE/tblog-img/-/raw/main/devto.gif)
    
 If you want to add in more stuff to the post, you can check out the [DEV.to API docs](https://developers.forem.com/api#operation/createArticle) which is powered by [Forem](https://www.forem.com/), there a ton of options you can hook to the front-matter in the shellscript.
 
-
-
```

### Comparing `crossposter-0.5.2/setup.py` & `crossposter-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = "0.5.2"
+VERSION = "0.6.0"
 PACKAGE_NAME = "crossposter"
 AUTHOR = "Meet Gor"
 AUTHOR_EMAIL = "gormeet711@gmail.com"
 URL = "https://github.com/Mr-Destructive/crossposter"
 
 DESCRIPTION = (
     "Crosspost your markdown articles to devto, medium, codenewbie and hashnode"
```

