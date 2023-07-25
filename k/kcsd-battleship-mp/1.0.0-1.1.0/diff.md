# Comparing `tmp/kcsd-battleship-mp-1.0.0.tar.gz` & `tmp/kcsd-battleship-mp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kcsd-battleship-mp-1.0.0.tar", last modified: Tue Jul 11 12:36:45 2023, max compression
+gzip compressed data, was "kcsd-battleship-mp-1.1.0.tar", last modified: Tue Jul 25 08:44:28 2023, max compression
```

## Comparing `kcsd-battleship-mp-1.0.0.tar` & `kcsd-battleship-mp-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2023-07-11 12:36:45.546454 kcsd-battleship-mp-1.0.0/
--rw-r--r--   0 mfischer   (501) staff       (20)     1196 2023-07-10 19:35:21.000000 kcsd-battleship-mp-1.0.0/LICENSE
--rw-r--r--   0 mfischer   (501) staff       (20)     2927 2023-07-11 12:36:45.546582 kcsd-battleship-mp-1.0.0/PKG-INFO
--rw-r--r--   0 mfischer   (501) staff       (20)     2341 2023-07-10 19:51:36.000000 kcsd-battleship-mp-1.0.0/README.rst
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2023-07-11 12:36:45.544143 kcsd-battleship-mp-1.0.0/battleship_mp/
--rw-r--r--   0 mfischer   (501) staff       (20)      174 2023-07-09 14:07:14.000000 kcsd-battleship-mp-1.0.0/battleship_mp/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     5708 2023-07-11 12:34:18.000000 kcsd-battleship-mp-1.0.0/battleship_mp/client.py
--rw-r--r--   0 mfischer   (501) staff       (20)      467 2023-07-10 19:18:58.000000 kcsd-battleship-mp-1.0.0/battleship_mp/exceptions.py
--rw-r--r--   0 mfischer   (501) staff       (20)     2073 2023-07-11 07:14:25.000000 kcsd-battleship-mp-1.0.0/battleship_mp/messages.py
--rw-r--r--   0 mfischer   (501) staff       (20)     6813 2023-07-11 07:14:25.000000 kcsd-battleship-mp-1.0.0/battleship_mp/server.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2023-07-11 12:36:45.546204 kcsd-battleship-mp-1.0.0/kcsd_battleship_mp.egg-info/
--rw-r--r--   0 mfischer   (501) staff       (20)     2927 2023-07-11 12:36:45.000000 kcsd-battleship-mp-1.0.0/kcsd_battleship_mp.egg-info/PKG-INFO
--rw-r--r--   0 mfischer   (501) staff       (20)      380 2023-07-11 12:36:45.000000 kcsd-battleship-mp-1.0.0/kcsd_battleship_mp.egg-info/SOURCES.txt
--rw-r--r--   0 mfischer   (501) staff       (20)        1 2023-07-11 12:36:45.000000 kcsd-battleship-mp-1.0.0/kcsd_battleship_mp.egg-info/dependency_links.txt
--rw-r--r--   0 mfischer   (501) staff       (20)      125 2023-07-11 12:36:45.000000 kcsd-battleship-mp-1.0.0/kcsd_battleship_mp.egg-info/requires.txt
--rw-r--r--   0 mfischer   (501) staff       (20)       14 2023-07-11 12:36:45.000000 kcsd-battleship-mp-1.0.0/kcsd_battleship_mp.egg-info/top_level.txt
--rw-r--r--   0 mfischer   (501) staff       (20)     1393 2023-07-11 12:34:47.000000 kcsd-battleship-mp-1.0.0/pyproject.toml
--rw-r--r--   0 mfischer   (501) staff       (20)      214 2023-07-11 12:36:45.547034 kcsd-battleship-mp-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:44:28.363259 kcsd-battleship-mp-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-25 08:44:15.000000 kcsd-battleship-mp-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-25 08:44:28.363259 kcsd-battleship-mp-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 08:44:15.000000 kcsd-battleship-mp-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:44:28.363259 kcsd-battleship-mp-1.1.0/battleship_mp/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-25 08:44:15.000000 kcsd-battleship-mp-1.1.0/battleship_mp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-25 08:44:15.000000 kcsd-battleship-mp-1.1.0/battleship_mp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-25 08:44:15.000000 kcsd-battleship-mp-1.1.0/battleship_mp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-25 08:44:15.000000 kcsd-battleship-mp-1.1.0/battleship_mp/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-25 08:44:15.000000 kcsd-battleship-mp-1.1.0/battleship_mp/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:44:28.363259 kcsd-battleship-mp-1.1.0/kcsd_battleship_mp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-25 08:44:28.000000 kcsd-battleship-mp-1.1.0/kcsd_battleship_mp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-25 08:44:28.000000 kcsd-battleship-mp-1.1.0/kcsd_battleship_mp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:44:28.000000 kcsd-battleship-mp-1.1.0/kcsd_battleship_mp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 08:44:28.000000 kcsd-battleship-mp-1.1.0/kcsd_battleship_mp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 08:44:28.000000 kcsd-battleship-mp-1.1.0/kcsd_battleship_mp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-25 08:44:15.000000 kcsd-battleship-mp-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-25 08:44:28.363259 kcsd-battleship-mp-1.1.0/setup.cfg
```

### Comparing `kcsd-battleship-mp-1.0.0/LICENSE` & `kcsd-battleship-mp-1.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 MIT License
 
-Copyright 2023, Copyright Owner: Karlsruhe Institute of Technology (KIT).
-Authors: Collaborative Software Design Dozenten, Contact: csd-dozenten@lists.kit.edu
+Copyright 2023, Copyright Owner: Karlsruhe Institute of Technology (KIT). Authors: Collaborative Software Design Dozenten, Contact: csd-dozenten@lists.kit.edu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `kcsd-battleship-mp-1.0.0/PKG-INFO` & `kcsd-battleship-mp-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kcsd-battleship-mp
-Version: 1.0.0
+Version: 1.1.0
 Summary: Multiplayer client/server for CSD BattleShip
 Author-email: Max Fischer <max.fischer@kit.edu>
 Project-URL: Homepage, https://github.com/kit-colsoftdes/battleship_mp
 Project-URL: Bug Tracker, https://github.com/kit-colsoftdes/battleship_mp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,26 @@
 Provides-Extra: doc
 License-File: LICENSE
 
 ##########################################################
 ``battleship_mp`` - Multiplayer Support for CSD Battleship
 ##########################################################
 
+.. image:: https://readthedocs.org/projects/battleship-mp/badge/?version=latest
+    :target: https://battleship-mp.readthedocs.io/en/latest
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/kcsd-battleship-mp.svg
+    :alt: Available on PyPI
+    :target: https://pypi.python.org/pypi/kcsd-battleship-mp/
+
+.. image:: https://img.shields.io/github/license/kit-colsoftdes/battleship_mp.svg
+    :alt: License
+    :target: https://github.com/kit-colsoftdes/battleship_mp/blob/main/LICENSE
+
 This package provides a simple client and server for the Battleship game.
 It tries to be roughly compatible with the Collaborative Software Design implementation.
 Behind the scenes, it uses `WebSocket`_ for communication between client and server.
 
 Client Usage
 ------------
 
@@ -51,29 +63,16 @@
     ~ $ python3 -m battleship_mp.server 8765 localhost
 
 See the ``--help`` flag for options.
 
 Installation
 ------------
 
-You can install the package directly from the repository;
+You can install the package directly via ``pip``;
 only Python >= 3.8 is required.
-Using a `venv`_ is strongly recommended!
 
 .. code:: bash
 
-    ~ $ git clone https://github.com/kit-colsoftdes/battleship_mp.git
-    Cloning into 'battleship_mp'...
-    ...
-    ~ $ python3 -m venv venv
-    ~ $ source venv/bin/activate
-    (venv) ~ $ python3 -m pip install ./battleship_mp
-    Processing path/to/repo
-        ...
-    Successfully installed battleship_mp-1.0.0
-
-**Note**:
-If you want to develop in the repo, also pass the ``-e`` flag to pip.
-This allows you to make changes without having to re-install the package.
+    ~ $ python3 -m pip install kcsd-battleship-mp
 
 .. _WebSocket: https://en.wikipedia.org/wiki/WebSocket
 .. _venv: https://docs.python.org/3/library/venv.html
```

### Comparing `kcsd-battleship-mp-1.0.0/README.rst` & `kcsd-battleship-mp-1.1.0/kcsd_battleship_mp.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,39 @@
+Metadata-Version: 2.1
+Name: kcsd-battleship-mp
+Version: 1.1.0
+Summary: Multiplayer client/server for CSD BattleShip
+Author-email: Max Fischer <max.fischer@kit.edu>
+Project-URL: Homepage, https://github.com/kit-colsoftdes/battleship_mp
+Project-URL: Bug Tracker, https://github.com/kit-colsoftdes/battleship_mp/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: doc
+License-File: LICENSE
+
 ##########################################################
 ``battleship_mp`` - Multiplayer Support for CSD Battleship
 ##########################################################
 
+.. image:: https://readthedocs.org/projects/battleship-mp/badge/?version=latest
+    :target: https://battleship-mp.readthedocs.io/en/latest
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/pypi/v/kcsd-battleship-mp.svg
+    :alt: Available on PyPI
+    :target: https://pypi.python.org/pypi/kcsd-battleship-mp/
+
+.. image:: https://img.shields.io/github/license/kit-colsoftdes/battleship_mp.svg
+    :alt: License
+    :target: https://github.com/kit-colsoftdes/battleship_mp/blob/main/LICENSE
+
 This package provides a simple client and server for the Battleship game.
 It tries to be roughly compatible with the Collaborative Software Design implementation.
 Behind the scenes, it uses `WebSocket`_ for communication between client and server.
 
 Client Usage
 ------------
 
@@ -35,29 +63,16 @@
     ~ $ python3 -m battleship_mp.server 8765 localhost
 
 See the ``--help`` flag for options.
 
 Installation
 ------------
 
-You can install the package directly from the repository;
+You can install the package directly via ``pip``;
 only Python >= 3.8 is required.
-Using a `venv`_ is strongly recommended!
 
 .. code:: bash
 
-    ~ $ git clone https://github.com/kit-colsoftdes/battleship_mp.git
-    Cloning into 'battleship_mp'...
-    ...
-    ~ $ python3 -m venv venv
-    ~ $ source venv/bin/activate
-    (venv) ~ $ python3 -m pip install ./battleship_mp
-    Processing path/to/repo
-        ...
-    Successfully installed battleship_mp-1.0.0
-
-**Note**:
-If you want to develop in the repo, also pass the ``-e`` flag to pip.
-This allows you to make changes without having to re-install the package.
+    ~ $ python3 -m pip install kcsd-battleship-mp
 
 .. _WebSocket: https://en.wikipedia.org/wiki/WebSocket
 .. _venv: https://docs.python.org/3/library/venv.html
```

### Comparing `kcsd-battleship-mp-1.0.0/battleship_mp/client.py` & `kcsd-battleship-mp-1.1.0/battleship_mp/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Tuple, Generator
 from contextlib import contextmanager
 import random
 import os
 from enum import Enum, auto
 
+import websockets.exceptions
 from websockets.sync.client import connect, Connection  # type: ignore
 
 from . import SERVER_URL_ENV, PROTOCOL_VERSION
 from .messages import communicate, fail
-from .exceptions import GameError, GameEnd
+from .exceptions import GameError, GameEnd, ConnectionClosed
 
 
 #: Names used if none is provided
 DEFAULT_NAMES = [
     "Dog",
     "Cat",
     "Fox",
@@ -100,21 +101,24 @@
         The underlying websocket must be managed manually.
         """
         local_name = (
             local_name
             if local_name is not None
             else f"Anonymous {random.choice(DEFAULT_NAMES)}"
         )
-        identifier, first = communicate(
-            connection,
-            "identifier",
-            "first",
-            identifier=local_name,
-            version=PROTOCOL_VERSION,
-        )
+        try:
+            identifier, first = communicate(
+                connection,
+                "identifier",
+                "first",
+                identifier=local_name,
+                version=PROTOCOL_VERSION,
+            )
+        except websockets.exceptions.ConnectionClosed:
+            raise ConnectionClosed() from None
         return cls(identifier, first, connection)
 
     def place_ships(self, *ships: SHIP_PLACEMENT) -> "tuple[SHIP_PLACEMENT, ...]":
         """
         Exchange placement of all the players' ships
 
         :param ships: placement of the local player's ships
@@ -124,49 +128,57 @@
         For example, ``(4, (0, 2), False)`` encodes
         a) a Destroyer of size 4
         b) at the top three cells to the right
         c) oriented to the right.
         """
         self._check_transition(State.PLACED, State.STARTED)
         l_sizes, l_coords, l_vertical = zip(*ships)
-        ships = tuple(
-            zip(
-                *communicate(
-                    self._ws,
-                    "sizes",
-                    "coords",
-                    "vertical",
-                    sizes=l_sizes,
-                    coords=l_coords,
-                    vertical=l_vertical,
-                )
+        try:
+            zipped_ships = communicate(
+                self._ws,
+                "sizes",
+                "coords",
+                "vertical",
+                sizes=l_sizes,
+                coords=l_coords,
+                vertical=l_vertical,
             )
-        )
-        return ships
+        except websockets.exceptions.ConnectionClosed:
+            raise ConnectionClosed() from None
+        return tuple(zip(*zipped_ships))
 
     def announce_shot(self, coord: "tuple[int, int]") -> None:
         """Announce that a shot has been fired"""
         self._check_transition(State.FIRING, State.PLACED, State.FIRING)
-        communicate(self._ws, announce_shot=coord)
+        try:
+            communicate(self._ws, announce_shot=coord)
+        except websockets.exceptions.ConnectionClosed:
+            raise ConnectionClosed() from None
 
     def expect_shot(self) -> "tuple[int, int]":
         """Wait for a shot to be fired and return its coordinates"""
         self._check_transition(State.FIRING, State.PLACED, State.FIRING)
-        (coord,) = communicate(self._ws, "coord", expect_shot=True)
+        try:
+            (coord,) = communicate(self._ws, "coord", expect_shot=True)
+        except websockets.exceptions.ConnectionClosed:
+            raise ConnectionClosed() from None
         return tuple(coord)  # type: ignore
 
     def end_game(self, winner: "str | None", forfeit: bool = False) -> "str | None":
         """
         End the game, announcing a ``winner`` or ``forfeit``
 
         Returns the ``winner`` determined by the peer.
         If a game is ``forfeit``, the peer is the winner.
+        A draw corresponds to ``winner=None``.
         """
         self._check_transition(State.ENDED, State.PLACED, State.FIRING)
         if forfeit:
             winner = self.opponent
         try:
             communicate(self._ws, "winner", winner=winner, forfeit=forfeit)
+        except websockets.exceptions.ConnectionClosed:
+            raise ConnectionClosed() from None
         except GameEnd as ge:
             return ge.winner
         else:
             return winner
```

### Comparing `kcsd-battleship-mp-1.0.0/battleship_mp/messages.py` & `kcsd-battleship-mp-1.1.0/battleship_mp/messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Iterable, NoReturn
+from typing import Any, Iterable, NoReturn, Type
 import json
 
 from websockets.sync.connection import Connection
 
 from .exceptions import ProtocolError, GameEnd
 
 
 # We only support a few known errors to avoid arbitrary calls
 ERRORS = {
     e.__name__: e for e in (ValueError, TypeError, KeyError, ProtocolError, GameEnd)
 }
+SERIALIZABLE_EXCEPTIONS: "tuple[Type[Exception], ...]" = tuple(ERRORS.values())
 
 
 def pack(
     payload: "dict[str, Any] | None" = None, error: "Exception | None" = None
 ) -> str:
     """Pack an error or payload into a message"""
     if error is not None:
```

### Comparing `kcsd-battleship-mp-1.0.0/battleship_mp/server.py` & `kcsd-battleship-mp-1.1.0/battleship_mp/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import argparse
 import random
 import logging
 
 import websockets
 from websockets.server import WebSocketServerProtocol
 
-from .messages import pack, unpack, unpack_keys
-from .exceptions import Deadlock, GameEnd
+from .messages import pack, unpack, unpack_keys, SERIALIZABLE_EXCEPTIONS
+from .exceptions import Deadlock, GameEnd, ProtocolError
 
 
 logger = logging.getLogger("battleship_mp.server")
 
 
 def send(_ws: WebSocketServerProtocol, **payload: Any) -> Awaitable[None]:
     return _ws.send(pack(payload))
@@ -39,21 +39,40 @@
         logger.info("run %s", self.identifier)
         try:
             await self.handle_start()
             await self.handle_placement()
             await self.handle_shots()
         except GameEnd as ge:
             logger.info("end %s, winner %s", self.identifier, ge.winner)
-        except Exception as exc:
+        except websockets.exceptions.ConnectionClosed:
+            # the connection of at least one player is gone
+            # let those know that we can still reach
+            for client in self.clients:
+                if not client.websocket.open:
+                    logger.info("end %s, closed %s", self.identifier, client.identifier)
+                    continue
+                else:
+                    await client.websocket.send(pack(error=GameEnd(winner=None)))
+        except SERIALIZABLE_EXCEPTIONS as exc:
             message = pack(error=exc)
             await gather(
                 self.clients[0].websocket.send(message),
                 self.clients[1].websocket.send(message),
             )
             logger.exception("abort %s", self.identifier)
+        except Exception:
+            # something completely unexpected happened
+            # try to let clients know but otherwise just drop everything and get out
+            message = pack(error=ProtocolError("internal server error"))
+            for client in self.clients:
+                try:
+                    await client.websocket.send(message)
+                except Exception:
+                    pass
+            logger.exception("abort %s", self.identifier)
 
     async def handle_start(self) -> None:
         logger.debug("handle_start %s", self.identifier)
         for idx, client in enumerate(self.clients):
             await send(
                 client.websocket,
                 identifier=self.clients[(idx + 1) % 2].identifier,
@@ -94,15 +113,15 @@
                     buffer = None
             elif "announce_shot" in a_action and "expect_shot" in b_action:
                 await gather(
                     send(sock_b, coord=a_action["announce_shot"]), send(sock_a)
                 )
             elif "expect_shot" in a_action and "announce_shot" in b_action:
                 await gather(
-                    send(sock_a, coord=a_action["announce_shot"]), send(sock_b)
+                    send(sock_a, coord=b_action["announce_shot"]), send(sock_b)
                 )
             else:
                 buffer = a_action["announce_shot"], b_action["announce_shot"]
                 await gather(send(sock_a), send(sock_b))
 
     async def handle_end(
         self, a_payload: "dict[str, Any]", b_payload: "dict[str, Any]"
```

### Comparing `kcsd-battleship-mp-1.0.0/pyproject.toml` & `kcsd-battleship-mp-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kcsd-battleship-mp"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Max Fischer", email="max.fischer@kit.edu" },
 ]
 description = "Multiplayer client/server for CSD BattleShip"
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3",
```

