# Comparing `tmp/scratch-getdata-1.0.5.tar.gz` & `tmp/scratch-getdata-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratch-getdata-1.0.5.tar", last modified: Wed Jun 28 03:16:46 2023, max compression
+gzip compressed data, was "scratch-getdata-1.0.6.tar", last modified: Tue Jul 25 19:34:25 2023, max compression
```

## Comparing `scratch-getdata-1.0.5.tar` & `scratch-getdata-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-28 03:16:46.539081 scratch-getdata-1.0.5/
--rw-r--r--   0 runner    (1000) runner    (1000)     2822 2023-06-28 03:16:46.539081 scratch-getdata-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2261 2023-06-28 03:12:22.000000 scratch-getdata-1.0.5/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)      659 2023-06-28 03:16:33.000000 scratch-getdata-1.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-28 03:16:46.535080 scratch-getdata-1.0.5/scratch_getdata/
--rw-r--r--   0 runner    (1000) runner    (1000)      517 2023-06-23 18:37:46.000000 scratch-getdata-1.0.5/scratch_getdata/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3616 2023-06-28 02:59:54.000000 scratch-getdata-1.0.5/scratch_getdata/api_client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-28 03:16:46.539081 scratch-getdata-1.0.5/scratch_getdata.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2822 2023-06-28 03:16:46.000000 scratch-getdata-1.0.5/scratch_getdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-06-28 03:16:46.000000 scratch-getdata-1.0.5/scratch_getdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-28 03:16:46.000000 scratch-getdata-1.0.5/scratch_getdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-06-28 03:16:46.000000 scratch-getdata-1.0.5/scratch_getdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-06-28 03:16:46.000000 scratch-getdata-1.0.5/scratch_getdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-28 03:16:46.539081 scratch-getdata-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-28 02:32:47.000000 scratch-getdata-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2975 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2387 2023-07-25 19:32:03.000000 scratch-getdata-1.0.6/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)      686 2023-07-25 19:32:57.000000 scratch-getdata-1.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/scratch_getdata/
+-rw-r--r--   0 runner    (1000) runner    (1000)      517 2023-07-25 19:32:23.000000 scratch-getdata-1.0.6/scratch_getdata/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4214 2023-07-25 19:30:04.000000 scratch-getdata-1.0.6/scratch_getdata/api_client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/scratch_getdata.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2975 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      285 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        9 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       16 2023-07-25 19:34:24.000000 scratch-getdata-1.0.6/scratch_getdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-25 19:34:25.406927 scratch-getdata-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      404 2023-06-28 02:32:47.000000 scratch-getdata-1.0.6/setup.py
```

### Comparing `scratch-getdata-1.0.5/PKG-INFO` & `scratch-getdata-1.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
-Author-email: kokofixcomputers <none@none.com>
+Author-email: kokofixcomputers <kokocanfixit@kokofixcomputers.serv00.net>
 Project-URL: Github, https://github.com/kokofixcomputers/Scratch-getdata
 Project-URL: Bug Tracker, https://github.com/kokofixcomputers/Scratch-getdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -29,66 +29,66 @@
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
 
 
 2. Retrieving the follower count of a user:
-follower_count = client.get_follower_count(username)
+follower_count = client.get_follower_count(username, api_key)
 
 
 3. Checking if a user is a Scratcher:
-is_scratcher = client.is_scratcher(username)
+is_scratcher = client.is_scratcher(username, api_key)
 
 
 4. Retrieving the following count of a user:
-following_count = client.get_following_count(username)
+following_count = client.get_following_count(username, api_key)
 
 5. Retrieving the "What I'm Working On" (WIWO) status of a user:
-wiwo_status = client.get_wiwo(username)
+wiwo_status = client.get_wiwo(username, api_key)
 
 
 6. Retrieving the "About Me" information of a user:
-about_me = client.get_about_me(username)
+about_me = client.get_about_me(username, api_key)
 
 
 7. Retrieving the messages of a user:
-messages = client.get_messages(username)
+messages = client.get_messages(username, api_key)
 
 
 8. Retrieving the creator of a project:
-project_creator = client.get_project_creator(project_id)
+project_creator = client.get_project_creator(project_id, api_key)
 
 
 9. Retrieving the name of a project:
-project_name = client.get_project_name(project_id)
+project_name = client.get_project_name(project_id), api_key
 
 
 10. Retrieving the description of a project:
-project_description = client.get_project_description(project_id)
+project_description = client.get_project_description(project_id, api_key)
 
 
 11. Retrieving the instructions of a project:
-project_instructions = client.get_project_instructions(project_id)
+project_instructions = client.get_project_instructions(project_id, api_key)
 
 
 12. Retrieving the blocks of a project:
-project_blocks = client.get_project_blocks(project_id)
+project_blocks = client.get_project_blocks(project_id, api_key)
 
 
 13. Retrieving the title of a forum post:
-forum_title = client.get_forum_title(post_id)
+forum_title = client.get_forum_title(post_id, api_key)
 
 
 14. Retrieving the category of a forum post:
-forum_category = client.get_forum_category(post_id)
+forum_category = client.get_forum_category(post_id, api_key)
 
 
 15. Retrieving the country of a Scratch user:
-user_country = client.get_scratch_user_country(username)
+user_country = client.get_scratch_user_country(username, api_key)
 
 
 Note: Replace `username` with the desired Scratch username and `project_id` with the desired project ID.
 
 API website: https://scratch-get-data.kokoiscool.repl.co
 
 Credits
```

### Comparing `scratch-getdata-1.0.5/README.md` & `scratch-getdata-1.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,66 +15,66 @@
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
 
 
 2. Retrieving the follower count of a user:
-follower_count = client.get_follower_count(username)
+follower_count = client.get_follower_count(username, api_key)
 
 
 3. Checking if a user is a Scratcher:
-is_scratcher = client.is_scratcher(username)
+is_scratcher = client.is_scratcher(username, api_key)
 
 
 4. Retrieving the following count of a user:
-following_count = client.get_following_count(username)
+following_count = client.get_following_count(username, api_key)
 
 5. Retrieving the "What I'm Working On" (WIWO) status of a user:
-wiwo_status = client.get_wiwo(username)
+wiwo_status = client.get_wiwo(username, api_key)
 
 
 6. Retrieving the "About Me" information of a user:
-about_me = client.get_about_me(username)
+about_me = client.get_about_me(username, api_key)
 
 
 7. Retrieving the messages of a user:
-messages = client.get_messages(username)
+messages = client.get_messages(username, api_key)
 
 
 8. Retrieving the creator of a project:
-project_creator = client.get_project_creator(project_id)
+project_creator = client.get_project_creator(project_id, api_key)
 
 
 9. Retrieving the name of a project:
-project_name = client.get_project_name(project_id)
+project_name = client.get_project_name(project_id), api_key
 
 
 10. Retrieving the description of a project:
-project_description = client.get_project_description(project_id)
+project_description = client.get_project_description(project_id, api_key)
 
 
 11. Retrieving the instructions of a project:
-project_instructions = client.get_project_instructions(project_id)
+project_instructions = client.get_project_instructions(project_id, api_key)
 
 
 12. Retrieving the blocks of a project:
-project_blocks = client.get_project_blocks(project_id)
+project_blocks = client.get_project_blocks(project_id, api_key)
 
 
 13. Retrieving the title of a forum post:
-forum_title = client.get_forum_title(post_id)
+forum_title = client.get_forum_title(post_id, api_key)
 
 
 14. Retrieving the category of a forum post:
-forum_category = client.get_forum_category(post_id)
+forum_category = client.get_forum_category(post_id, api_key)
 
 
 15. Retrieving the country of a Scratch user:
-user_country = client.get_scratch_user_country(username)
+user_country = client.get_scratch_user_country(username, api_key)
 
 
 Note: Replace `username` with the desired Scratch username and `project_id` with the desired project ID.
 
 API website: https://scratch-get-data.kokoiscool.repl.co
 
 Credits
```

### Comparing `scratch-getdata-1.0.5/pyproject.toml` & `scratch-getdata-1.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scratch-getdata"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
-  { name="kokofixcomputers", email="none@none.com" },
+  { name="kokofixcomputers", email="kokocanfixit@kokofixcomputers.serv00.net" },
 ]
 dependencies = ['requests']
 description = "A Module to fetch scratch things from ScratchGetData"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `scratch-getdata-1.0.5/scratch_getdata/__init__.py` & `scratch-getdata-1.0.6/scratch_getdata/__init__.py`

 * *Files identical despite different names*

### Comparing `scratch-getdata-1.0.5/scratch_getdata/api_client.py` & `scratch-getdata-1.0.6/scratch_getdata/api_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,96 @@
 import requests
 
 class ScratchAPIClient:
     def __init__(self):
         print("It may take a while for ScratchForGetData to boot up like 3-10 seconds")
         self.base_url = "https://scratch-get-data.kokoiscool.repl.co"
 
-    def get_follower_count(self, username):
+    def get_follower_count(self, username, api_key):
         url = f"{self.base_url}/get/follower-count/{username}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the follower count as a string
 
-    def is_scratcher(self, username):
+    def is_scratcher(self, username, api_key):
         url = f"{self.base_url}/get/is_scratcher/{username}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip().lower() == "true"  # Return True or False based on the response
 
-    def get_following_count(self, username):
+    def get_following_count(self, username, api_key):
         url = f"{self.base_url}/get/following-count/{username}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the following count as a string
 
-    def get_wiwo(self, username):
+    def get_wiwo(self, username, api_key):
         url = f"{self.base_url}/get/wiwo/{username}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the WiWo as a string
 
-    def get_about_me(self, username):
+    def get_about_me(self, username, api_key):
         url = f"{self.base_url}/get/aboutme/{username}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the About Me text as a string
 
-    def get_messages(self, username):
+    def get_messages(self, username, api_key):
         url = f"{self.base_url}/get/messages/{username}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the Messages as a string
 
-    def get_project_creator(self, project_id):
+    def get_project_creator(self, project_id, api_key):
         url = f"{self.base_url}/get/project/creator/{project_id}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the project creator username as a string
 
-    def get_project_name(self, project_id):
+    def get_project_name(self, project_id, api_key):
         url = f"{self.base_url}/get/project/name/{project_id}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the project name as a string
 
-    def get_project_description(self, project_id):
+    def get_project_description(self, project_id, api_key):
         url = f"{self.base_url}/get/project/notes_and_credits/{project_id}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the project description as a string
 
-    def get_project_instructions(self, project_id):
+    def get_project_instructions(self, project_id, api_key):
         url = f"{self.base_url}/get/project/instructions/{project_id}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the project instructions as a string
 
-    def get_project_blocks(self, project_id):
+    def get_project_blocks(self, project_id, api_key):
         url = f"{self.base_url}/get/project/blocks/{project_id}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the project blocks as a string
 
-    def get_forum_title(self, post_id):
+    def get_forum_title(self, post_id, api_key):
         url = f"{self.base_url}/get/forum/title/{post_id}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the forum post title as a string
 
-    def get_forum_category(self, post_id):
+    def get_forum_category(self, post_id, api_key):
         url = f"{self.base_url}/get/forum/category/{post_id}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the forum post category as a string
 
-    def get_scratch_user_country(self, username):
+    def get_scratch_user_country(self, username, api_key):
         url = f"{self.base_url}/get/user/country/{username}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the Scratch user's country as a string
 
-    def get_studio_title(self, studio_id):
+    def get_studio_title(self, studio_id, api_key):
         url = f"{self.base_url}/get/studio/title/{studio_id}/"
-        response = requests.get(url)
+        response = requests.get(url, key=api_key)
         return response.text.strip()  # Return the Scratch studio title as string
 
+class TestConnection:
+
+  def test():
+    base_url = "https://scratch-get-data.kokoiscool.repl.co"
+    
+    url = f"{base_url}/ping/"
+
+    response = requests.get(url)
+    
+    if response.status_code == 200:
+      return 'ok'
+    else:
+      raise("ConnectionError")
+
```

### Comparing `scratch-getdata-1.0.5/scratch_getdata.egg-info/PKG-INFO` & `scratch-getdata-1.0.6/scratch_getdata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: scratch-getdata
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Module to fetch scratch things from ScratchGetData
 Author: kokofixcomputers
-Author-email: kokofixcomputers <none@none.com>
+Author-email: kokofixcomputers <kokocanfixit@kokofixcomputers.serv00.net>
 Project-URL: Github, https://github.com/kokofixcomputers/Scratch-getdata
 Project-URL: Bug Tracker, https://github.com/kokofixcomputers/Scratch-getdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -29,66 +29,66 @@
 Usage
 -----
 1. Instantiating the ScratchAPIClient class:
 client = ScratchAPIClient()
 
 
 2. Retrieving the follower count of a user:
-follower_count = client.get_follower_count(username)
+follower_count = client.get_follower_count(username, api_key)
 
 
 3. Checking if a user is a Scratcher:
-is_scratcher = client.is_scratcher(username)
+is_scratcher = client.is_scratcher(username, api_key)
 
 
 4. Retrieving the following count of a user:
-following_count = client.get_following_count(username)
+following_count = client.get_following_count(username, api_key)
 
 5. Retrieving the "What I'm Working On" (WIWO) status of a user:
-wiwo_status = client.get_wiwo(username)
+wiwo_status = client.get_wiwo(username, api_key)
 
 
 6. Retrieving the "About Me" information of a user:
-about_me = client.get_about_me(username)
+about_me = client.get_about_me(username, api_key)
 
 
 7. Retrieving the messages of a user:
-messages = client.get_messages(username)
+messages = client.get_messages(username, api_key)
 
 
 8. Retrieving the creator of a project:
-project_creator = client.get_project_creator(project_id)
+project_creator = client.get_project_creator(project_id, api_key)
 
 
 9. Retrieving the name of a project:
-project_name = client.get_project_name(project_id)
+project_name = client.get_project_name(project_id), api_key
 
 
 10. Retrieving the description of a project:
-project_description = client.get_project_description(project_id)
+project_description = client.get_project_description(project_id, api_key)
 
 
 11. Retrieving the instructions of a project:
-project_instructions = client.get_project_instructions(project_id)
+project_instructions = client.get_project_instructions(project_id, api_key)
 
 
 12. Retrieving the blocks of a project:
-project_blocks = client.get_project_blocks(project_id)
+project_blocks = client.get_project_blocks(project_id, api_key)
 
 
 13. Retrieving the title of a forum post:
-forum_title = client.get_forum_title(post_id)
+forum_title = client.get_forum_title(post_id, api_key)
 
 
 14. Retrieving the category of a forum post:
-forum_category = client.get_forum_category(post_id)
+forum_category = client.get_forum_category(post_id, api_key)
 
 
 15. Retrieving the country of a Scratch user:
-user_country = client.get_scratch_user_country(username)
+user_country = client.get_scratch_user_country(username, api_key)
 
 
 Note: Replace `username` with the desired Scratch username and `project_id` with the desired project ID.
 
 API website: https://scratch-get-data.kokoiscool.repl.co
 
 Credits
```

