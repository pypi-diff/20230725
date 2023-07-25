# Comparing `tmp/dc3client-0.0.1.tar.gz` & `tmp/dc3client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dc3client-0.0.1.tar", last modified: Mon Jul 24 06:52:19 2023, max compression
+gzip compressed data, was "dc3client-0.0.2.tar", last modified: Tue Jul 25 05:29:28 2023, max compression
```

## Comparing `dc3client-0.0.1.tar` & `dc3client-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:19.466292 dc3client-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-24 06:52:05.000000 dc3client-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 06:52:19.466292 dc3client-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-24 06:52:05.000000 dc3client-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:19.462292 dc3client-0.0.1/dc3client/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 06:52:05.000000 dc3client-0.0.1/dc3client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39951 2023-07-24 06:52:05.000000 dc3client-0.0.1/dc3client/dc3client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-24 06:52:05.000000 dc3client-0.0.1/dc3client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:52:19.466292 dc3client-0.0.1/dc3client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-24 06:52:19.000000 dc3client-0.0.1/dc3client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-24 06:52:19.000000 dc3client-0.0.1/dc3client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:52:19.000000 dc3client-0.0.1/dc3client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 06:52:19.000000 dc3client-0.0.1/dc3client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 06:52:19.000000 dc3client-0.0.1/dc3client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:52:19.466292 dc3client-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-24 06:52:05.000000 dc3client-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:29:28.035265 dc3client-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-25 05:29:16.000000 dc3client-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 05:29:28.035265 dc3client-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 05:29:16.000000 dc3client-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:29:28.031265 dc3client-0.0.2/dc3client/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 05:29:16.000000 dc3client-0.0.2/dc3client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39929 2023-07-25 05:29:16.000000 dc3client-0.0.2/dc3client/dc3client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-25 05:29:16.000000 dc3client-0.0.2/dc3client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:29:28.035265 dc3client-0.0.2/dc3client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-25 05:29:28.000000 dc3client-0.0.2/dc3client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-25 05:29:28.000000 dc3client-0.0.2/dc3client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:29:28.000000 dc3client-0.0.2/dc3client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 05:29:28.000000 dc3client-0.0.2/dc3client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 05:29:28.000000 dc3client-0.0.2/dc3client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:29:28.035265 dc3client-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-25 05:29:16.000000 dc3client-0.0.2/setup.py
```

### Comparing `dc3client-0.0.1/LICENSE` & `dc3client-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dc3client-0.0.1/PKG-INFO` & `dc3client-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dc3client
-Version: 0.0.1
+Version: 0.0.2
 Summary: dc3client: Client of Digital Curing3.
 Home-page: https://github.com/being24/pypi-test
 Download-URL: https://github.com/being24/pypi-test
 Author: Ryosuke1218
 Author-email: 34680324+being24@users.noreply.github.com
 Maintainer: Ryosuke1218
 Maintainer-email: 34680324+being24@users.noreply.github.com
```

### Comparing `dc3client-0.0.1/dc3client/dc3client.py` & `dc3client-0.0.2/dc3client/dc3client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,29 +69,29 @@
 
         # Get current time for rate limit
         self.last_send = time.time()
 
         # Rate limit time interval
         self.rate_limit = 3.0
 
-    def __connect(self, address: tuple, family: int, typ: int, proto: int):
+    def _connect(self, address: tuple, family: int, typ: int, proto: int):
         self.logger.info(f"Connect to {address}")
         self.address = address  # address of server
         self.socket = socket.socket(family, typ, proto)  # create socket object
         self.socket.settimeout(self.timeout)  # set timeout
         self.socket.connect(self.address)  # connect to server
         self.logger.info(f"Connect to {address} success")
 
         if self.socket is None:
             self.logger.error("Socket is None")
             raise Exception("Socket is None")
         # Close socket on exit
         atexit.register(self.__shutdown)
 
-    def __send(self, message: str = ""):
+    def send(self, message: str = ""):
         """send message to server
 
         Args:
             message (str, optional): massage content. Defaults to "".
         """
 
         if message == "":
@@ -109,15 +109,15 @@
                     self.last_send = now
                     break
                 else:
                     self.logger.debug(f"Rate limit {self.rate_limit} seconds")
                     self.logger.debug(f"Please wait {wait_time + .5} seconds")
                     time.sleep(wait_time + 0.5)
 
-    def __receive(self) -> dict[str, Any]:
+    def receive(self) -> dict[str, Any]:
         """receive message from server until "\n"
 
         Returns:
             dict[str, Any]: received message
         """
 
         message = ""
@@ -171,15 +171,15 @@
         self.move_info: list[ShotInfo] = []
 
         # Name of the client
         self.client_name = client_name
 
         if auto_start:
             self.rate_limit = rate_limit
-            super().__connect(self.server, socket.AF_INET, socket.SOCK_STREAM, 0)
+            super()._connect(self.server, socket.AF_INET, socket.SOCK_STREAM, 0)
             self.start_game()
         else:
             self.start_game()
 
     def start_game(self):
         """start game"""
         self.dc_recv()
@@ -211,15 +211,15 @@
                     )
                 )
 
         return team_stone
 
     def dc_recv(self):
         """receive dc"""
-        message_recv = self.__receive()
+        message_recv = self.receive()
 
         version = Version(
             major=message_recv["version"]["major"],
             minor=message_recv["version"]["minor"],
         )
 
         dc = ServerDC(
@@ -233,20 +233,20 @@
 
     def dc_ok(self) -> None:
         """send dc_ok"""
 
         message: dict = {"cmd": "dc_ok", "name": self.client_name}
         message_str: str = json.dumps(message)
         message_str: str = message_str + "\n"
-        self.__send(message_str)
+        self.send(message_str)
 
     def is_ready_recv(self):
         """receive is_ready"""
 
-        message_recv = self.__receive()
+        message_recv = self.receive()
 
         thinking_time = ThinkingTime(
             team0=message_recv["game"]["setting"]["thinking_time"]["team0"],
             team1=message_recv["game"]["setting"]["thinking_time"]["team1"],
         )
 
         extra_end_thinking_time = ExtraEndThinkingTime(
@@ -303,31 +303,31 @@
         self.match_data.is_ready = is_ready
 
     def ready_ok(self, player_order: list = [0, 1, 3, 2]) -> None:
         """send ready_ok"""
         ready = {"cmd": "ready_ok", "player_order": player_order}
         ready_str = json.dumps(ready)
         ready_str = ready_str + "\n"
-        self.__send(ready_str)
+        self.send(ready_str)
 
     def get_new_game(self):
         """receive new_game"""
 
-        message_recv = self.__receive()
+        message_recv = self.receive()
         self.match_data.new_game = NewGame(cmd=message_recv["cmd"], name=message_recv["name"])
         if self.match_data.new_game is not None:
             self.is_connected = True
 
     def update(self):
         """receive update"""
 
         if self.is_connected is False:
             raise Exception("Not connected to server")
         
-        message_recv = self.__receive()
+        message_recv = self.receive()
 
         start_team0_position = []
         start_team1_position = []
         finish_team0_position = []
         finish_team1_position = []
         frame_data = []
 
@@ -512,22 +512,22 @@
                 "type": "shot",
                 "velocity": {"x": x, "y": y},
                 "rotation": rotation,
             },
         }
         s = json.dumps(shot)
         s = s + "\n"
-        self.__send(s)
+        self.send(s)
 
     def concede(self) -> None:
         """Concede"""
         concede = {"cmd": "move", "move": {"type": "concede"}}
         s = json.dumps(concede)
         s = s + "\n"
-        self.__send(s)
+        self.send(s)
 
     def get_my_team(self) -> str:
         """get my team name
 
         Returns:
             str: my team name
         """
```

### Comparing `dc3client-0.0.1/dc3client/models.py` & `dc3client-0.0.2/dc3client/models.py`

 * *Files identical despite different names*

### Comparing `dc3client-0.0.1/dc3client.egg-info/PKG-INFO` & `dc3client-0.0.2/dc3client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dc3client
-Version: 0.0.1
+Version: 0.0.2
 Summary: dc3client: Client of Digital Curing3.
 Home-page: https://github.com/being24/pypi-test
 Download-URL: https://github.com/being24/pypi-test
 Author: Ryosuke1218
 Author-email: 34680324+being24@users.noreply.github.com
 Maintainer: Ryosuke1218
 Maintainer-email: 34680324+being24@users.noreply.github.com
```

### Comparing `dc3client-0.0.1/setup.py` & `dc3client-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = "dc3client: Client of Digital Curing3."
 NAME = "dc3client"
 AUTHOR = "Ryosuke1218"
 AUTHOR_EMAIL = "34680324+being24@users.noreply.github.com"
 URL = "https://github.com/being24/pypi-test"
 LICENSE = "MIT"
 DOWNLOAD_URL = URL
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 PYTHON_REQUIRES = ">=3.10"
 INSTALL_REQUIRES = ["numpy>=1.24.0"]
 PACKAGES = ["dc3client"]
 KEYWORDS = "digital-curing3 dc3client"
 CLASSIFIERS = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
```

