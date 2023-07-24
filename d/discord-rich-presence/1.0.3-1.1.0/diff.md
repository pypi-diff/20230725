# Comparing `tmp/discord-rich-presence-1.0.3.tar.gz` & `tmp/discord-rich-presence-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-rich-presence-1.0.3.tar", last modified: Mon Jun 12 18:47:02 2023, max compression
+gzip compressed data, was "discord-rich-presence-1.1.0.tar", last modified: Mon Jul 24 22:11:28 2023, max compression
```

## Comparing `discord-rich-presence-1.0.3.tar` & `discord-rich-presence-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-06-12 18:47:02.323424 discord-rich-presence-1.0.3/
--rw-r--r--   0 maxwe      (501) staff       (20)     1064 2022-06-14 05:49:12.000000 discord-rich-presence-1.0.3/LICENSE
--rw-r--r--   0 maxwe      (501) staff       (20)     2806 2023-06-12 18:47:02.321466 discord-rich-presence-1.0.3/PKG-INFO
--rw-r--r--   0 maxwe      (501) staff       (20)     2120 2023-06-05 02:59:38.000000 discord-rich-presence-1.0.3/README.md
-drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-06-12 18:47:02.316584 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/
--rw-r--r--   0 maxwe      (501) staff       (20)     2806 2023-06-12 18:47:02.000000 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/PKG-INFO
--rw-r--r--   0 maxwe      (501) staff       (20)      269 2023-06-12 18:47:02.000000 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/SOURCES.txt
--rw-r--r--   0 maxwe      (501) staff       (20)        1 2023-06-12 18:47:02.000000 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/dependency_links.txt
--rw-r--r--   0 maxwe      (501) staff       (20)       10 2023-06-12 18:47:02.000000 discord-rich-presence-1.0.3/discord_rich_presence.egg-info/top_level.txt
-drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-06-12 18:47:02.320583 discord-rich-presence-1.0.3/discordrp/
--rw-r--r--   0 maxwe      (501) staff       (20)      315 2023-06-12 18:44:46.000000 discord-rich-presence-1.0.3/discordrp/__init__.py
--rw-r--r--   0 maxwe      (501) staff       (20)     5804 2023-06-05 02:58:18.000000 discord-rich-presence-1.0.3/discordrp/presence.py
--rw-r--r--   0 maxwe      (501) staff       (20)        0 2023-06-05 02:46:28.000000 discord-rich-presence-1.0.3/discordrp/py.typed
--rw-r--r--   0 maxwe      (501) staff       (20)       38 2023-06-12 18:47:02.323570 discord-rich-presence-1.0.3/setup.cfg
--rw-r--r--   0 maxwe      (501) staff       (20)      978 2023-06-05 02:58:18.000000 discord-rich-presence-1.0.3/setup.py
+drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-07-24 22:11:28.435093 discord-rich-presence-1.1.0/
+-rw-r--r--   0 maxwe      (501) staff       (20)     1069 2023-07-24 22:02:11.000000 discord-rich-presence-1.1.0/LICENSE
+-rw-r--r--   0 maxwe      (501) staff       (20)     3267 2023-07-24 22:11:28.433937 discord-rich-presence-1.1.0/PKG-INFO
+-rw-r--r--   0 maxwe      (501) staff       (20)     2581 2023-07-24 21:35:49.000000 discord-rich-presence-1.1.0/README.md
+drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-07-24 22:11:28.425137 discord-rich-presence-1.1.0/discord_rich_presence.egg-info/
+-rw-r--r--   0 maxwe      (501) staff       (20)     3267 2023-07-24 22:11:28.000000 discord-rich-presence-1.1.0/discord_rich_presence.egg-info/PKG-INFO
+-rw-r--r--   0 maxwe      (501) staff       (20)      269 2023-07-24 22:11:28.000000 discord-rich-presence-1.1.0/discord_rich_presence.egg-info/SOURCES.txt
+-rw-r--r--   0 maxwe      (501) staff       (20)        1 2023-07-24 22:11:28.000000 discord-rich-presence-1.1.0/discord_rich_presence.egg-info/dependency_links.txt
+-rw-r--r--   0 maxwe      (501) staff       (20)       10 2023-07-24 22:11:28.000000 discord-rich-presence-1.1.0/discord_rich_presence.egg-info/top_level.txt
+drwxr-xr-x   0 maxwe      (501) staff       (20)        0 2023-07-24 22:11:28.432484 discord-rich-presence-1.1.0/discordrp/
+-rw-r--r--   0 maxwe      (501) staff       (20)      384 2023-07-24 22:04:15.000000 discord-rich-presence-1.1.0/discordrp/__init__.py
+-rw-r--r--   0 maxwe      (501) staff       (20)     6818 2023-07-24 21:45:46.000000 discord-rich-presence-1.1.0/discordrp/presence.py
+-rw-r--r--   0 maxwe      (501) staff       (20)        0 2023-06-05 02:46:28.000000 discord-rich-presence-1.1.0/discordrp/py.typed
+-rw-r--r--   0 maxwe      (501) staff       (20)       38 2023-07-24 22:11:28.435352 discord-rich-presence-1.1.0/setup.cfg
+-rw-r--r--   0 maxwe      (501) staff       (20)      978 2023-06-05 02:58:18.000000 discord-rich-presence-1.1.0/setup.py
```

### Comparing `discord-rich-presence-1.0.3/LICENSE` & `discord-rich-presence-1.1.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 TenType
+Copyright (c) 2022-2023 TenType
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `discord-rich-presence-1.0.3/PKG-INFO` & `discord-rich-presence-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-rich-presence
-Version: 1.0.3
+Version: 1.1.0
 Summary: A lightweight and safe module for creating custom rich presences on Discord.
 Home-page: https://github.com/TenType/discord-rich-presence
 Author: TenType
 License: MIT
 Keywords: discord,presence,rich presence,activity,rpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Unix
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # discord-rich-presence
-A lightweight and safe module for creating custom rich presences on Discord.
+A lightweight and safe package for creating custom rich presences on Discord.
 
 ## Example
 ![Discord Rich Presence Example](/examples/example.jpg)
 
 ## How to Use
 
 ### Making a Discord App
@@ -44,27 +44,31 @@
 ```py
 from discordrp import Presence
 import time
 
 client_id = "000000000000000000"  # Replace this with your own client id
 
 with Presence(client_id) as presence:
+    print("Connected")
     presence.set(
         {
             "state": "In Game",
             "details": "Summoner's Rift",
             "timestamps": {"start": int(time.time())},
         }
     )
+    print("Presence updated")
 
     while True:
         time.sleep(15)
 ```
 Make sure you replace the `client_id` variable with your app's id that you copied earlier.
 
 7. Run the program! You should now see that you have a rich presence on your profile that will be on until you stop the program! Feel free to change the code however you want by adding images, buttons, and more. Check out [examples/complex.py](examples/complex.py) for another example.
 
 ## Troubleshooting
-If you're having trouble using this module, it might be because of the following:
-- your Discord app is not open
-- you passed in an incorrect dictionary, which the Discord API rejected
-- something unexpected occurred while writing data, in which you should try running the program again
+Here are the most common errors:
+- **`ActivityError`**: An incorrect dictionary was passed to `Presence.set`. Make sure that it matches the [format expected by Discord](https://discord.com/developers/docs/topics/gateway-events#activity-object).
+- **`ClientIDError`**: Verify that your client ID is valid.
+- **`PresenceError`**: Read the [Discord docs](https://discord.com/developers/docs/topics/opcodes-and-status-codes#rpc) for more information.
+- **`ConnectionRefusedError` or `FileNotFoundError`**: Make sure that your Discord application is open and logged in.
+- **Program hangs for a long time and does not set the presence**: Wait for at least 10 seconds before closing and trying again.
```

### Comparing `discord-rich-presence-1.0.3/README.md` & `discord-rich-presence-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # discord-rich-presence
-A lightweight and safe module for creating custom rich presences on Discord.
+A lightweight and safe package for creating custom rich presences on Discord.
 
 ## Example
 ![Discord Rich Presence Example](/examples/example.jpg)
 
 ## How to Use
 
 ### Making a Discord App
@@ -25,27 +25,31 @@
 ```py
 from discordrp import Presence
 import time
 
 client_id = "000000000000000000"  # Replace this with your own client id
 
 with Presence(client_id) as presence:
+    print("Connected")
     presence.set(
         {
             "state": "In Game",
             "details": "Summoner's Rift",
             "timestamps": {"start": int(time.time())},
         }
     )
+    print("Presence updated")
 
     while True:
         time.sleep(15)
 ```
 Make sure you replace the `client_id` variable with your app's id that you copied earlier.
 
 7. Run the program! You should now see that you have a rich presence on your profile that will be on until you stop the program! Feel free to change the code however you want by adding images, buttons, and more. Check out [examples/complex.py](examples/complex.py) for another example.
 
 ## Troubleshooting
-If you're having trouble using this module, it might be because of the following:
-- your Discord app is not open
-- you passed in an incorrect dictionary, which the Discord API rejected
-- something unexpected occurred while writing data, in which you should try running the program again
+Here are the most common errors:
+- **`ActivityError`**: An incorrect dictionary was passed to `Presence.set`. Make sure that it matches the [format expected by Discord](https://discord.com/developers/docs/topics/gateway-events#activity-object).
+- **`ClientIDError`**: Verify that your client ID is valid.
+- **`PresenceError`**: Read the [Discord docs](https://discord.com/developers/docs/topics/opcodes-and-status-codes#rpc) for more information.
+- **`ConnectionRefusedError` or `FileNotFoundError`**: Make sure that your Discord application is open and logged in.
+- **Program hangs for a long time and does not set the presence**: Wait for at least 10 seconds before closing and trying again.
```

### Comparing `discord-rich-presence-1.0.3/discord_rich_presence.egg-info/PKG-INFO` & `discord-rich-presence-1.1.0/discord_rich_presence.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-rich-presence
-Version: 1.0.3
+Version: 1.1.0
 Summary: A lightweight and safe module for creating custom rich presences on Discord.
 Home-page: https://github.com/TenType/discord-rich-presence
 Author: TenType
 License: MIT
 Keywords: discord,presence,rich presence,activity,rpc
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Unix
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # discord-rich-presence
-A lightweight and safe module for creating custom rich presences on Discord.
+A lightweight and safe package for creating custom rich presences on Discord.
 
 ## Example
 ![Discord Rich Presence Example](/examples/example.jpg)
 
 ## How to Use
 
 ### Making a Discord App
@@ -44,27 +44,31 @@
 ```py
 from discordrp import Presence
 import time
 
 client_id = "000000000000000000"  # Replace this with your own client id
 
 with Presence(client_id) as presence:
+    print("Connected")
     presence.set(
         {
             "state": "In Game",
             "details": "Summoner's Rift",
             "timestamps": {"start": int(time.time())},
         }
     )
+    print("Presence updated")
 
     while True:
         time.sleep(15)
 ```
 Make sure you replace the `client_id` variable with your app's id that you copied earlier.
 
 7. Run the program! You should now see that you have a rich presence on your profile that will be on until you stop the program! Feel free to change the code however you want by adding images, buttons, and more. Check out [examples/complex.py](examples/complex.py) for another example.
 
 ## Troubleshooting
-If you're having trouble using this module, it might be because of the following:
-- your Discord app is not open
-- you passed in an incorrect dictionary, which the Discord API rejected
-- something unexpected occurred while writing data, in which you should try running the program again
+Here are the most common errors:
+- **`ActivityError`**: An incorrect dictionary was passed to `Presence.set`. Make sure that it matches the [format expected by Discord](https://discord.com/developers/docs/topics/gateway-events#activity-object).
+- **`ClientIDError`**: Verify that your client ID is valid.
+- **`PresenceError`**: Read the [Discord docs](https://discord.com/developers/docs/topics/opcodes-and-status-codes#rpc) for more information.
+- **`ConnectionRefusedError` or `FileNotFoundError`**: Make sure that your Discord application is open and logged in.
+- **Program hangs for a long time and does not set the presence**: Wait for at least 10 seconds before closing and trying again.
```

### Comparing `discord-rich-presence-1.0.3/discordrp/presence.py` & `discord-rich-presence-1.1.0/discordrp/presence.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,21 +20,44 @@
     FRAME = 1
     CLOSE = 2
     PING = 3
     PONG = 4
 
 
 SOCKET_NAME = "discord-ipc-{}"
+INVALID_PAYLOAD = 4000
 
 
 class PresenceError(Exception):
     """
-    Errors emitted by the Presence class.
+    An error emitted from Discord. See the [docs](https://discord.com/developers/docs/topics/opcodes-and-status-codes#rpc) for more details.
     """
 
+    def __init__(self, message: object, code: int) -> None:
+        super().__init__(message)
+        self.code = code
+
+
+class ClientIDError(PresenceError):
+    """
+    Invalid client ID.
+    """
+
+    def __init__(self) -> None:
+        super().__init__("Client ID is invalid", INVALID_PAYLOAD)
+
+
+class ActivityError(PresenceError):
+    """
+    Discord rejected the payload because the activity was not in the [correct format](https://discord.com/developers/docs/topics/gateway-events#activity-object).
+    """
+
+    def __init__(self, message: object) -> None:
+        super().__init__(message, INVALID_PAYLOAD)
+
 
 class Presence:
     """
     The main class used to connect to Discord for its rich presence API.
     """
 
     def __init__(self, client_id: str):
@@ -46,93 +69,91 @@
         )
 
         # Send a handshake request
         self._handshake()
 
     def set(self, activity: Optional[dict[str, Any]]) -> None:
         """
-        Sends an activity payload to Discord.
-        :param activity: A dictionary of this format:
+        Sets the current activity using a dictionary representing a [Discord activity object](https://discord.com/developers/docs/topics/gateway-events#activity-object).
 
-        ```
-        {
-            'state': str,
-            'details': str,
-            'timestamps': {
-                'start': int,
-                'end': int,
-            },
-            'assets': {
-                'large_image': str,
-                'large_text': str,
-                'small_image': str,
-                'small_text': str,
-            },
-            'buttons': [
-                {
-                    'label': str,
-                    'url': str,
-                },
-                {
-                    'label': str,
-                    'url': str,
-                }
-            ],
-        }
-        ```
-        One field of either 'state', 'details', or 'timestamps.start' is required.
+        Raises a `PresenceError` if Discord rejected the payload.
         """
+
         payload = {
             "cmd": "SET_ACTIVITY",
             "args": {
                 "pid": os.getpid(),
                 "activity": activity,
             },
             "nonce": str(uuid4()),
         }
         self._send(payload, _OpCode.FRAME)
 
+        # Check for errors
+        reply = self._read()
+        if reply.get("evt") != "ERROR":
+            return
+
+        message: str = reply["data"]["message"]
+        code: int = reply["data"]["code"]
+
+        if code == INVALID_PAYLOAD:
+            # Improve readability of the error message if the dictionary is invalid
+            prefix = 'child "activity" fails because ['
+            if message.startswith(prefix):
+                message = message[len(prefix) : -1]
+            raise ActivityError(message)
+
+        raise PresenceError(message, code)
+
     def clear(self) -> None:
         """
         Clears the current activity.
         """
         self.set(None)
 
     def close(self) -> None:
         """
         Closes the current connection.
         This method is automatically called when the program exits using the 'with' statement.
         """
-        self._send({}, _OpCode.CLOSE)
-        self._socket._close()
+        try:
+            self._send({}, _OpCode.CLOSE)
+        finally:
+            self._socket._close()
 
     def _handshake(self) -> None:
         self._send({"v": 1, "client_id": self.client_id}, _OpCode.HANDSHAKE)
-        data = self._read()
+        payload = self._read()
 
-        if data.get("evt") != "READY":
-            raise PresenceError(
-                "Discord returned an error response after a handshake request"
-            )
+        if payload.get("evt") != "READY":
+            if payload["code"] == INVALID_PAYLOAD:
+                raise ClientIDError()
+            raise PresenceError(payload["message"], payload["code"])
 
     def _read(self) -> dict[str, Any]:
         op, length = self._read_header()
         decoded = self._read_bytes(length).decode("utf-8")
         data = json.loads(decoded)
         return cast(dict[str, Any], data)
 
     def _read_header(self) -> tuple[int, int]:
         return cast(tuple[int, int], struct.unpack("<ii", self._read_bytes(8)))
 
     def _read_bytes(self, size: int) -> bytes:
-        encoded = b""
+        data = b""
         while size > 0:
-            encoded += self._socket._read(size)
-            size -= len(encoded)
-        return encoded
+            chunk = self._socket._read(size)
+            if not chunk:
+                raise ConnectionAbortedError(
+                    "Connection closed before all bytes were read"
+                )
+            data += chunk
+            size -= len(chunk)
+        return data
 
     def _send(self, payload: dict[str, Any], op: _OpCode) -> None:
         encoded = json.dumps(payload).encode("utf-8")
         header = struct.pack("<ii", int(op), len(encoded))
         self._socket._write(header + encoded)
 
     def __enter__(self) -> "Presence":
@@ -174,15 +195,15 @@
             try:
                 self._sock = socket.socket(socket.AF_UNIX)  # type: ignore [attr-defined,unused-ignore]
                 self._sock.connect(pipe.format(i))
                 break
             except FileNotFoundError:
                 pass
         else:
-            raise PresenceError("Cannot find a Unix socket to connect to Discord")
+            raise FileNotFoundError("Cannot find a Unix socket to connect to Discord")
 
     def _get_pipe_path(self) -> str:
         for env in ("XDG_RUNTIME_DIR", "TMPDIR", "TMP", "TEMP"):
             path = os.environ.get(env)
             if path is not None:
                 return path
 
@@ -206,15 +227,17 @@
         for i in range(10):
             try:
                 self._buffer = open(pipe.format(i), "rb+")
                 break
             except FileNotFoundError:
                 pass
         else:
-            raise PresenceError("Cannot find a Windows socket to connect to Discord")
+            raise FileNotFoundError(
+                "Cannot find a Windows socket to connect to Discord"
+            )
 
     def _read(self, size: int) -> bytes:
         return self._buffer.read(size)
 
     def _write(self, data: bytes) -> None:
         self._buffer.write(data)
         self._buffer.flush()
```

### Comparing `discord-rich-presence-1.0.3/setup.py` & `discord-rich-presence-1.1.0/setup.py`

 * *Files identical despite different names*

