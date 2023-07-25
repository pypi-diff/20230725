# Comparing `tmp/pibooth_fire_remote-0.2.0-py3-none-any.whl.zip` & `tmp/pibooth_fire_remote-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4193 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4830 b- defN 23-Jul-24 08:43 pibooth_fire_remote.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1539 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-24 08:43 pibooth_fire_remote-0.2.0.dist-info/RECORD
-7 files, 8232 bytes uncompressed, 3053 bytes compressed:  62.9%
+Zip file size: 4237 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     5310 b- defN 23-Jul-25 07:15 pibooth_fire_remote.py
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-25 07:15 pibooth_fire_remote-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1539 b- defN 23-Jul-25 07:15 pibooth_fire_remote-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 07:15 pibooth_fire_remote-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Jul-25 07:15 pibooth_fire_remote-0.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-25 07:15 pibooth_fire_remote-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      632 b- defN 23-Jul-25 07:15 pibooth_fire_remote-0.2.2.dist-info/RECORD
+7 files, 8712 bytes uncompressed, 3097 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pibooth_fire_remote.py
 Comment: 
 
-Filename: pibooth_fire_remote-0.2.0.dist-info/LICENSE
+Filename: pibooth_fire_remote-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: pibooth_fire_remote-0.2.0.dist-info/METADATA
+Filename: pibooth_fire_remote-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: pibooth_fire_remote-0.2.0.dist-info/WHEEL
+Filename: pibooth_fire_remote-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: pibooth_fire_remote-0.2.0.dist-info/entry_points.txt
+Filename: pibooth_fire_remote-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.2.0.dist-info/top_level.txt
+Filename: pibooth_fire_remote-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pibooth_fire_remote-0.2.0.dist-info/RECORD
+Filename: pibooth_fire_remote-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pibooth_fire_remote.py

```diff
@@ -7,15 +7,15 @@
 
 keyboard = Controller()
 
 import pibooth
 from pibooth.utils import LOGGER
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.2"
 
 
 
 BUTTONDOWN = pygame.USEREVENT + 1
 
 SECTION = "FIRE-Remote"
 
@@ -25,14 +25,18 @@
         # creates object 'fire tv remote' to store the data
         device_name = str(cfg_in.get(SECTION, 'device'))
         dev = InputDevice(device_name)
     except FileNotFoundError:
         LOGGER.warning("Bluetooth device not Found.")
         dev = None
 
+    except PermissionError:
+        LOGGER.warning("Bluetooth device busy")
+        dev = None
+
     return dev
 @pibooth.hookimpl
 def pibooth_configure(cfg):
     #button code variables (change to suit your device)
     cfg.add_option(SECTION, 'device', '/dev/input/event2',
                    "Device Path")
     cfg.add_option(SECTION, 'pictureBtn', 96,
@@ -57,71 +61,73 @@
                    "printBtn Button Code")
     # cfg.add_option(SECTION, 'backward', 168,
     #                "Backward Button Code")
 
 
 @pibooth.hookimpl
 def pibooth_startup(cfg, app):
-    dev = get_device(cfg)
-    if dev is not None:
-        th = threading.Thread(target=run_event_monitor, args=(cfg, app))
-        th.daemon = True
-        th.start()
+    th = threading.Thread(target=run_event_monitor, args=(cfg, app))
+    th.daemon = True
+    th.start()
 
 def run_event_monitor(cfg, app):
     #loop and filter by event code and print the mapped label
-    dev = get_device(cfg)
-    if dev is not None:
+    while True:
+
+        dev = get_device(cfg)
+        if dev is not None:
 
-        pictureBtn = int(cfg.get(SECTION, 'pictureBtn'))
-        # backBtn = int(cfg.get(SECTION, 'backBtn'))
-        settingsBtn = int(cfg.get(SECTION, 'settingsBtn'))
-        # homeBtn = int(cfg.get(SECTION, 'homeBtn'))
-        # up = int(cfg.get(SECTION, 'up'))
-        # down = int(cfg.get(SECTION, 'down'))
-        left = int(cfg.get(SECTION, 'left'))
-        right = int(cfg.get(SECTION, 'right'))
-        # playpause = int(cfg.get(SECTION, 'playpause'))
-        printBtn = int(cfg.get(SECTION, 'printBtn'))
-        # backward = int(cfg.get(SECTION, 'backward'))
-
-        for event in dev.read_loop():
-
-            if event.type == ecodes.EV_KEY and hasattr(event, "code"):
-                if event.value == 1:
-                    if event.code == pictureBtn:
-                        pygame.event.post(pygame.event.Event(BUTTONDOWN, capture=1, printer=0,
-                                                   button=app.buttons.capture))
-
-                        LOGGER.info("pictureBtn")
-                    elif event.code == settingsBtn:
-                        pygame.event.post(pygame.event.Event(BUTTONDOWN, capture=1, printer=1,
-                                                             button=app.buttons))
-                        LOGGER.info("settingsBtn")
-                    # if event.code == homeBtn:
-                    #     LOGGER.info("homeBtn")
-                    # elif event.code == backBtn:
-                    #     LOGGER.info("backBtn")
-                    # elif event.code == playpause:
-                    #     LOGGER.info("Play/Pause")
-                    # elif event.code == up:
-                    #     keyboard.press(Key.up)
-                    #     keyboard.release(Key.up)
-                    #     LOGGER.info("up")
-                    # elif event.code == down:
-                    #     keyboard.press(Key.up)
-                    #     keyboard.release(Key.up)
-                    #     LOGGER.info("down")
-                    elif event.code == left:
-                        keyboard.press(Key.left)
-                        keyboard.release(Key.left)
-                        LOGGER.info("left")
-                    elif event.code == right:
-                        keyboard.press(Key.right)
-                        keyboard.release(Key.right)
-                        LOGGER.info("right")
-                    elif event.code == printBtn:
-                        pygame.event.post(pygame.event.Event(BUTTONDOWN, capture=0, printer=1,
-                                                             button=app.buttons.printer))
-                        LOGGER.info("printBtn")
-                    # elif event.code == backward:
-                    #     LOGGER.info("backward")
+            pictureBtn = int(cfg.get(SECTION, 'pictureBtn'))
+            # backBtn = int(cfg.get(SECTION, 'backBtn'))
+            settingsBtn = int(cfg.get(SECTION, 'settingsBtn'))
+            # homeBtn = int(cfg.get(SECTION, 'homeBtn'))
+            # up = int(cfg.get(SECTION, 'up'))
+            # down = int(cfg.get(SECTION, 'down'))
+            left = int(cfg.get(SECTION, 'left'))
+            right = int(cfg.get(SECTION, 'right'))
+            # playpause = int(cfg.get(SECTION, 'playpause'))
+            printBtn = int(cfg.get(SECTION, 'printBtn'))
+            # backward = int(cfg.get(SECTION, 'backward'))
+            try:
+                for event in dev.read_loop():
+
+                    if event.type == ecodes.EV_KEY and hasattr(event, "code"):
+                        if event.value == 1:
+                            if event.code == pictureBtn:
+                                pygame.event.post(pygame.event.Event(BUTTONDOWN, capture=1, printer=0,
+                                                           button=app.buttons.capture))
+
+                                LOGGER.info("pictureBtn")
+                            elif event.code == settingsBtn:
+                                pygame.event.post(pygame.event.Event(BUTTONDOWN, capture=1, printer=1,
+                                                                     button=app.buttons))
+                                LOGGER.info("settingsBtn")
+                            # if event.code == homeBtn:
+                            #     LOGGER.info("homeBtn")
+                            # elif event.code == backBtn:
+                            #     LOGGER.info("backBtn")
+                            # elif event.code == playpause:
+                            #     LOGGER.info("Play/Pause")
+                            # elif event.code == up:
+                            #     keyboard.press(Key.up)
+                            #     keyboard.release(Key.up)
+                            #     LOGGER.info("up")
+                            # elif event.code == down:
+                            #     keyboard.press(Key.up)
+                            #     keyboard.release(Key.up)
+                            #     LOGGER.info("down")
+                            elif event.code == left:
+                                keyboard.press(Key.left)
+                                keyboard.release(Key.left)
+                                LOGGER.info("left")
+                            elif event.code == right:
+                                keyboard.press(Key.right)
+                                keyboard.release(Key.right)
+                                LOGGER.info("right")
+                            elif event.code == printBtn:
+                                pygame.event.post(pygame.event.Event(BUTTONDOWN, capture=0, printer=1,
+                                                                     button=app.buttons.printer))
+                                LOGGER.info("printBtn")
+                            # elif event.code == backward:
+                            #     LOGGER.info("backward")
+            except OSError:
+                pass
```

## Comparing `pibooth_fire_remote-0.2.0.dist-info/LICENSE` & `pibooth_fire_remote-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pibooth_fire_remote-0.2.0.dist-info/METADATA` & `pibooth_fire_remote-0.2.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibooth-fire-remote
-Version: 0.2.0
+Version: 0.2.2
 Summary: UNKNOWN
 Home-page: https://github.com/chilipp89/pibooth-qr-download
 Author: P. Junietz
 License: MIT
 Keywords: Raspberry Pi,camera,photobooth,Bluetooth,Remote
 Platform: unix
 Platform: linux
```

## Comparing `pibooth_fire_remote-0.2.0.dist-info/RECORD` & `pibooth_fire_remote-0.2.2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pibooth_fire_remote.py,sha256=MI_z_YITpBYUIsGjBZ8S-4BGe7UeegCA78v-uzvVOx4,4830
-pibooth_fire_remote-0.2.0.dist-info/LICENSE,sha256=8MhKKX4jcdh7M60uTWf4zk_cdmFXMxHe26HsSJyZphU,1066
-pibooth_fire_remote-0.2.0.dist-info/METADATA,sha256=FuF8TQ2pgrVvH11Pyg3HGyUZN-zGwEcte2efSTYIjJ8,1539
-pibooth_fire_remote-0.2.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pibooth_fire_remote-0.2.0.dist-info/entry_points.txt,sha256=ExheM_w4JJMaMeao7ARgseEwDMsCCzTXD0F170rgR0U,53
-pibooth_fire_remote-0.2.0.dist-info/top_level.txt,sha256=uzVg30QGLIeuYlAgFLl7efJyUgD2uoKL2lOpC9oJGeY,20
-pibooth_fire_remote-0.2.0.dist-info/RECORD,,
+pibooth_fire_remote.py,sha256=ofvpZbRMRHDZN8W2Fr5T7LlG1r5u_mPmC90wwV0zq80,5310
+pibooth_fire_remote-0.2.2.dist-info/LICENSE,sha256=8MhKKX4jcdh7M60uTWf4zk_cdmFXMxHe26HsSJyZphU,1066
+pibooth_fire_remote-0.2.2.dist-info/METADATA,sha256=DZmxvV6IlMcFuyE3j6NbWHC8ORrustheEje_VJCz76A,1539
+pibooth_fire_remote-0.2.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pibooth_fire_remote-0.2.2.dist-info/entry_points.txt,sha256=ExheM_w4JJMaMeao7ARgseEwDMsCCzTXD0F170rgR0U,53
+pibooth_fire_remote-0.2.2.dist-info/top_level.txt,sha256=uzVg30QGLIeuYlAgFLl7efJyUgD2uoKL2lOpC9oJGeY,20
+pibooth_fire_remote-0.2.2.dist-info/RECORD,,
```

