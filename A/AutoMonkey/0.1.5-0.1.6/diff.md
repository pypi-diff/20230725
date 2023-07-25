# Comparing `tmp/AutoMonkey-0.1.5.tar.gz` & `tmp/AutoMonkey-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoMonkey-0.1.5.tar", last modified: Wed Nov 16 22:05:57 2022, max compression
+gzip compressed data, was "AutoMonkey-0.1.6.tar", last modified: Tue Jul 25 19:50:47 2023, max compression
```

## Comparing `AutoMonkey-0.1.5.tar` & `AutoMonkey-0.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2022-11-16 22:05:57.350000 AutoMonkey-0.1.5/
--rw-rw-rw-   0        0        0      191 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/AUTHORS.rst
-drwxrwxrwx   0        0        0        0 2022-11-16 22:05:57.400000 AutoMonkey-0.1.5/AutoMonkey.egg-info/
--rw-rw-rw-   0        0        0    12462 2022-11-16 22:05:58.000000 AutoMonkey-0.1.5/AutoMonkey.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      729 2022-11-16 22:05:58.000000 AutoMonkey-0.1.5/AutoMonkey.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-16 22:05:58.000000 AutoMonkey-0.1.5/AutoMonkey.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-11-16 22:05:58.000000 AutoMonkey-0.1.5/AutoMonkey.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-16 22:05:58.000000 AutoMonkey-0.1.5/AutoMonkey.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      242 2022-11-16 22:05:58.000000 AutoMonkey-0.1.5/AutoMonkey.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-11-16 22:05:58.000000 AutoMonkey-0.1.5/AutoMonkey.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3684 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2022-11-06 14:59:42.000000 AutoMonkey-0.1.5/HISTORY.rst
--rw-rw-rw-   0        0        0     1615 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      291 2022-11-06 16:34:20.000000 AutoMonkey-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0    12462 2022-11-16 22:05:58.000000 AutoMonkey-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    11706 2022-11-16 18:43:04.000000 AutoMonkey-0.1.5/README.md
--rw-rw-rw-   0        0        0     1139 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-16 22:05:57.450000 AutoMonkey-0.1.5/automonkey/
--rw-rw-rw-   0        0        0      184 2022-11-16 22:05:02.000000 AutoMonkey-0.1.5/automonkey/__init__.py
--rw-rw-rw-   0        0        0     4241 2022-11-16 20:39:00.000000 AutoMonkey-0.1.5/automonkey/app_funcs.py
--rw-rw-rw-   0        0        0     9344 2022-11-16 22:02:36.000000 AutoMonkey-0.1.5/automonkey/automonkey.py
--rw-rw-rw-   0        0        0     1828 2022-11-15 18:06:26.000000 AutoMonkey-0.1.5/automonkey/constants.py
--rw-rw-rw-   0        0        0      604 2022-11-15 17:51:38.000000 AutoMonkey-0.1.5/automonkey/exceptions.py
--rw-rw-rw-   0        0        0    10253 2022-11-16 21:57:06.000000 AutoMonkey-0.1.5/automonkey/img_funcs.py
--rw-rw-rw-   0        0        0     4396 2022-11-16 21:43:32.000000 AutoMonkey-0.1.5/automonkey/mouse_tracker.py
--rw-rw-rw-   0        0        0     4869 2022-11-16 20:40:50.000000 AutoMonkey-0.1.5/automonkey/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-16 22:05:57.500000 AutoMonkey-0.1.5/docs/
--rw-rw-rw-   0        0        0      631 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/docs/Makefile
--rw-rw-rw-   0        0        0       29 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/docs/authors.rst
--rw-rw-rw-   0        0        0     5064 2022-11-16 18:16:42.000000 AutoMonkey-0.1.5/docs/conf.py
--rw-rw-rw-   0        0        0       34 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/docs/history.rst
--rw-rw-rw-   0        0        0      327 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/docs/index.rst
--rw-rw-rw-   0        0        0     1205 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/docs/installation.rst
--rwxrwxrwx   0        0        0      808 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/docs/make.bat
--rw-rw-rw-   0        0        0       28 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/docs/readme.rst
--rw-rw-rw-   0        0        0       82 2022-08-04 19:18:48.000000 AutoMonkey-0.1.5/docs/usage.rst
--rw-rw-rw-   0        0        0      974 2022-11-16 22:05:02.000000 AutoMonkey-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      275 2022-11-16 17:42:54.000000 AutoMonkey-0.1.5/requirements.txt
--rw-rw-rw-   0        0        0      451 2022-11-16 22:05:58.000000 AutoMonkey-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1602 2022-11-16 22:05:02.000000 AutoMonkey-0.1.5/setup.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      178 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/AUTHORS.rst
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 19:50:47.127348 AutoMonkey-0.1.6/AutoMonkey.egg-info/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      729 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       51 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/entry_points.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/not-zip-safe
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      242 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/requires.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       11 2023-07-25 19:50:47.000000 AutoMonkey-0.1.6/AutoMonkey.egg-info/top_level.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3556 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/CONTRIBUTING.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       89 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/HISTORY.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1582 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/LICENSE
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      279 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/MANIFEST.in
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    11362 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/README.md
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1098 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/README.rst
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/automonkey/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      177 2023-07-25 19:41:30.000000 AutoMonkey-0.1.6/automonkey/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4700 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/app_funcs.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     9336 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/automonkey.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1730 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/constants.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      589 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/exceptions.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    10013 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/img_funcs.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4263 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/mouse_tracker.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4706 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/automonkey/utils.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/docs/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      611 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/Makefile
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/authors.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4901 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/conf.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       33 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/contributing.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/history.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      307 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/index.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1154 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/installation.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      772 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/make.bat
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       27 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/readme.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       75 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/docs/usage.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      939 2023-07-25 19:41:30.000000 AutoMonkey-0.1.6/pyproject.toml
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      265 2023-07-25 19:36:00.000000 AutoMonkey-0.1.6/requirements.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      425 2023-07-25 19:50:47.131348 AutoMonkey-0.1.6/setup.cfg
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1578 2023-07-25 19:41:30.000000 AutoMonkey-0.1.6/setup.py
```

### Comparing `AutoMonkey-0.1.5/AutoMonkey.egg-info/PKG-INFO` & `AutoMonkey-0.1.6/AutoMonkey.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,342 +1,342 @@
-Metadata-Version: 2.1
-Name: AutoMonkey
-Version: 0.1.5
-Summary: Python Automation using Mouse and Keyboard, for the masses
-Home-page: https://github.com/MihailCosmin/automonkey
-Author: Mihail-Cosmin Munteanu
-Author-email: Mihail-Cosmin Munteanu <munteanumihailcosmin@gmail.com>
-License: GNU General Public License v3
-Project-URL: Homepage, https://github.com/MihailCosmin/AutoMonkey
-Project-URL: Bug Tracker, https://github.com/MihailCosmin/AutoMonkey/issues
-Keywords: automonkey
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4)
-[![Known Vulnerabilities](https://snyk.io/test/github/MihailCosmin/AutoMonkey/badge.svg)](https://snyk.io/test/github/MihailCosmin/AutoMonkey)
-[![HitCount](https://hits.dwyl.com/MihailCosmin/AutoMonkey.svg?style=flat-square&show=unique)](http://hits.dwyl.com/MihailCosmin/AutoMonkey)
-[![build](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml/badge.svg)](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml)
-[![Code Climate](https://codeclimate.com/github/MihailCosmin/AutoMonkey/badges/gpa.svg)](https://codeclimate.com/github/MihailCosmin/AutoMonkey)
-
-# AutoMonkey
-<img alt="AutoMonkey" src="https://github.com/MihailCosmin/AutoMonkey/raw/06181954fa23605583d61843226f5f3997157435/img/monkey.ico" width="100px" height="100px"/>
-
-Python Automation using Mouse and Keyboard, for the masses
-
-# Installation
-
-1. From <a href="https://pypi.org/project/AutoMonkey/">pypi</a>:
-
-```
-pip install AutoMonkey
-```
-
-2. From <a href="https://github.com/MihailCosmin/AutoMonkey">github</a>:
-
-```
-pip install git+https://github.com/MihailCosmin/AutoMonkey
-```
-
-# Dependencies
-#### Automonkey is based on:
-- <a href="https://github.com/asweigart/pyautogui">pyautogui</a>
-
-#### Other dependencies:
-- PyScreeze
-- pyperclip
-- clipboard
-- keyboard
-- screeninfo
-- pywin32
-- pillow
-- opencv-python
-- numpy
-- pytesseract
-
-# Usage
-Main function to be used is "chain"  
-
-This will allow you to "chain" together most of the other functions of automonkey.  
-Which in turn will enable you to create sequences of mouse and/or keyboard actions in order to automate any given task.
-
-A step can have this structure:
-
-```python
-
-dict(
-    <action> = <target>,  # action can be any of the automonkey functions, target on which the action will be performed
-    wait = 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
-    skip = False,  # if True, will skip this step
-    confidence = 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
-    v_offset = 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
-    h_offset = 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
-    offset = 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
-    monitor = 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
-)
-
-or 
-
-{
-    "<action>": "<target>",  # action can be any of the automonkey functions, target on which the action will be performed
-    "wait": 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
-    "skip": False,  # if True, will skip this step
-    "confidence": 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
-    "v_offset": 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
-    "h_offset": 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
-    "offset": 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
-    "monitor": 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
-}
-```
-
-1. You can connect multiple mouse actions together by using the "chain" function. Just by doing this you can generally automate most of the tasks you would do on a daily basis.
-
-    There are 2 main ways to click, either by giving the coordinates of the position where to click or by giving the filename of the image you want to click on
-
-    1.1. Clicking by coordinates
-        
-    
-    1.1.1. In order to find the coordinates of a position on the screen you can use the "track_mouse" function or the PositionTracker class
-
-    ```python
-        from automonkey import track_mouse
-        track_mouse()
-    ```
-
-    <img alt="track_mouse" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/track_mouse.gif" width="416px" height="304px"/>
-
-
-    ```python
-        from automonkey import PositionTracker
-        tracker = PositionTracker()
-        tracker.start()
-    ```
-
-    <img alt="PositionTracker" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/PositionTracker.gif" width="918px" height="574px"/>
-
-    1.2.1. Now that you have the coordinates of the position you want to click on, you can use the "chain" function to click on it
-
-
-    ```python
-        from automonkey import chain
-        chain(  
-            dict(click=(780, 1175), wait=1),  
-            dict(click=(444, 194), wait=1),  
-            dict(click=(1892, 110), wait=1),  
-            debug=True  
-        )
-    ```
-
-    <img alt="click" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click.gif" width="960px" height="576px"/>
-
-    1.2. Clicking by image
-
-    1.2.1. To click on an image you first need to make a screenshot of the area you want to click on and save it somewhere on your computer.
-        For this you can use any screenshot tool you want, or you could use monkeyshot: https://github.com/MihailCosmin/monkeyshot
-        For example you can make a screenshot of the Edge icon from your toolbar, then we can click on it by using the "chain" function.
-
-    <img alt="edge_toolbar" src="https://github.com/MihailCosmin/AutoMonkey/raw/25eaed263793bf548d42f616e241f435baa9d719/demo/edge_toolbar.jpg" width="33px" height="33px"/>
-
-    1.2.2. Now that we have the image we want to click on, we can use the "chain" function to click on it
-
-    ```python
-        chain(
-            dict(click="demo/edge_toolbar.jpg"),
-            dict(click="demo/google_create_account", wait=1),
-            dict(click="demo/personal_use", wait=1),
-            debug=True
-        )
-    ```
-
-    <img alt="click_image" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click_image.gif" width="918px" height="600px"/>
-
-    1.3. All mouse actions:
-
-        * click
-        * rightclick
-        * leftclick
-        * doubleclick
-        * tripleclick
-        * scrollup
-        * scrolldown
-        * scrollleft
-        * scrollright
-
-2. You can also connect multiple keyboard actions together by using the "chain" function.
-
-    2.1. Write text - This doesn't work well with non-english character. For this you can use the "pastetext" function.
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg"),
-            dict(write="Hello World!"),
-            debug=True
-        )
-    ```
-
-    <img alt="write" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/write.gif" width="918px" height="600px"/>
-
-    2.2. Paste text - This works well with non-english characters
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg"),
-            dict(pastetext="Straße"),
-            debug=True
-        )
-    ```
-
-    2.3. Key combinations
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(keys2="ctrl+a", wait=1),
-            dict(keys2="ctrl+x", wait=1),
-            dict(keys2="alt+f4", wait=1),  # close notepad
-            debug=True
-        )
-    ```
-
-    <img alt="keys" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/keys.gif" width="918px" height="600px"/>
-
-    2.4. All key actions:
-
-        * write
-        * pastetext
-        * keys
-        * keys2 - best option overall for key combinations
-        * keys3
-        * keys4
-        * copy
-        * paste
-
-3. Wait actions:
-
-    3.1. Wait until an image appears on the screen
-    This can used when you are waiting for a window to finish loading completely and you don't know exactly how long that would take.
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg"),
-            dict(waituntil="demo/notepad_opened.jpg", wait=1),
-            dict(write="Hello World!", wait=1),
-            debug=True
-        )
-    ```
-
-    3.2. Wait while an image is on the screen
-
-4. App (window) actions:
-
-    4.1. Open an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(waituntil="demo/notepad_opened.jpg", wait=1),
-            dict(write="Hello World!", wait=1),
-            debug=True
-        )
-    ```
-
-    4.2. Close an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(close="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.3. Minimize an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(minimize="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.4. Maximize an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(maximize="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.5. Restore an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(minimize="Notepad", wait=1),
-            dict(restore="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.6. All app actions:
-
-        * open_app
-        * close
-        * startfile
-        * focus
-        * minimize
-        * maximize
-        * restore
-        * msoffice_replace
-        * copy_from
-        * copy_from_to
-
-5. Image actions
-
-    5.1 count_img. With this function you can count how many times one image appears on the screen.
-
-    ```python
-        chain(
-            dict(count_img="demo/M.jpg", wait=1),  # The result will be copied to the clipboard
-            dict(open_app="notepad++.exe", wait=1),
-            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
-            debug=True
-        )
-    ```
-
-    5.2. get_text_from_region
-
-    ```python
-        chain(
-            dict(get_text_from_region=((136, 121), (189, 140)), wait=1),  # The text will be copied to the clipboard
-            dict(open_app="notepad++.exe", wait=1),
-            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
-            debug=True
-        )
-    ```
-
-# Roadmap
-1. Check if possible to add <a href="https://github.com/pywinauto/pywinauto">pyautowin</a> functionality
-
-# Frequently Asked Questions:
-
-1. I made an image but it doesn't click on it.
-
-    A: Make sure you have not changed resolution of your screen or the theme (dark/light) of the window.
-
-
-2. Keys combination using "keys" function doesn't work.
-
-    A: Try other keys functions. Preferably "keys2". Other options "keys3", "keys4".
+Metadata-Version: 2.1
+Name: AutoMonkey
+Version: 0.1.6
+Summary: Python Automation using Mouse and Keyboard, for the masses
+Home-page: https://github.com/MihailCosmin/automonkey
+Author: Mihail-Cosmin Munteanu
+Author-email: Mihail-Cosmin Munteanu <munteanumihailcosmin@gmail.com>
+License: GNU General Public License v3
+Project-URL: Homepage, https://github.com/MihailCosmin/AutoMonkey
+Project-URL: Bug Tracker, https://github.com/MihailCosmin/AutoMonkey/issues
+Keywords: automonkey
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4)
+[![](https://snyk.io/test/github/MihailCosmin/AutoMonkey/badge.svg)](https://snyk.io/test/github/MihailCosmin/AutoMonkey)
+[![HitCount](https://hits.dwyl.com/MihailCosmin/AutoMonkey.svg?style=flat-square&show=unique)](http://hits.dwyl.com/MihailCosmin/AutoMonkey)
+[![build](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml/badge.svg)](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml)
+[![Code Climate](https://codeclimate.com/github/MihailCosmin/AutoMonkey/badges/gpa.svg)](https://codeclimate.com/github/MihailCosmin/AutoMonkey)
+
+# AutoMonkey
+<img alt="AutoMonkey" src="https://github.com/MihailCosmin/AutoMonkey/raw/06181954fa23605583d61843226f5f3997157435/img/monkey.ico" width="100px" height="100px"/>
+
+Python Automation using Mouse and Keyboard, for the masses
+
+# Installation
+
+1. From <a href="https://pypi.org/project/AutoMonkey/">pypi</a>:
+
+```
+pip install AutoMonkey
+```
+
+2. From <a href="https://github.com/MihailCosmin/AutoMonkey">github</a>:
+
+```
+pip install git+https://github.com/MihailCosmin/AutoMonkey
+```
+
+# Dependencies
+#### Automonkey is based on:
+- <a href="https://github.com/asweigart/pyautogui">pyautogui</a>
+
+#### Other dependencies:
+- PyScreeze
+- pyperclip
+- clipboard
+- keyboard
+- screeninfo
+- pywin32
+- pillow
+- opencv-python
+- numpy
+- pytesseract
+
+# Usage
+Main function to be used is "chain"  
+
+This will allow you to "chain" together most of the other functions of automonkey.  
+Which in turn will enable you to create sequences of mouse and/or keyboard actions in order to automate any given task.
+
+A step can have this structure:
+
+```python
+
+dict(
+    <action> = <target>,  # action can be any of the automonkey functions, target on which the action will be performed
+    wait = 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
+    skip = False,  # if True, will skip this step
+    confidence = 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
+    v_offset = 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
+    h_offset = 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
+    offset = 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
+    monitor = 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
+)
+
+or 
+
+{
+    "<action>": "<target>",  # action can be any of the automonkey functions, target on which the action will be performed
+    "wait": 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
+    "skip": False,  # if True, will skip this step
+    "confidence": 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
+    "v_offset": 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
+    "h_offset": 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
+    "offset": 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
+    "monitor": 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
+}
+```
+
+1. You can connect multiple mouse actions together by using the "chain" function. Just by doing this you can generally automate most of the tasks you would do on a daily basis.
+
+    There are 2 main ways to click, either by giving the coordinates of the position where to click or by giving the filename of the image you want to click on
+
+    1.1. Clicking by coordinates
+        
+    
+    1.1.1. In order to find the coordinates of a position on the screen you can use the "track_mouse" function or the PositionTracker class
+
+    ```python
+        from automonkey import track_mouse
+        track_mouse()
+    ```
+
+    <img alt="track_mouse" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/track_mouse.gif" width="416px" height="304px"/>
+
+
+    ```python
+        from automonkey import PositionTracker
+        tracker = PositionTracker()
+        tracker.start()
+    ```
+
+    <img alt="PositionTracker" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/PositionTracker.gif" width="918px" height="574px"/>
+
+    1.2.1. Now that you have the coordinates of the position you want to click on, you can use the "chain" function to click on it
+
+
+    ```python
+        from automonkey import chain
+        chain(  
+            dict(click=(780, 1175), wait=1),  
+            dict(click=(444, 194), wait=1),  
+            dict(click=(1892, 110), wait=1),  
+            debug=True  
+        )
+    ```
+
+    <img alt="click" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click.gif" width="960px" height="576px"/>
+
+    1.2. Clicking by image
+
+    1.2.1. To click on an image you first need to make a screenshot of the area you want to click on and save it somewhere on your computer.
+        For this you can use any screenshot tool you want, or you could use monkeyshot: https://github.com/MihailCosmin/monkeyshot
+        For example you can make a screenshot of the Edge icon from your toolbar, then we can click on it by using the "chain" function.
+
+    <img alt="edge_toolbar" src="https://github.com/MihailCosmin/AutoMonkey/raw/25eaed263793bf548d42f616e241f435baa9d719/demo/edge_toolbar.jpg" width="33px" height="33px"/>
+
+    1.2.2. Now that we have the image we want to click on, we can use the "chain" function to click on it
+
+    ```python
+        chain(
+            dict(click="demo/edge_toolbar.jpg"),
+            dict(click="demo/google_create_account", wait=1),
+            dict(click="demo/personal_use", wait=1),
+            debug=True
+        )
+    ```
+
+    <img alt="click_image" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click_image.gif" width="918px" height="600px"/>
+
+    1.3. All mouse actions:
+
+        * click
+        * rightclick
+        * leftclick
+        * doubleclick
+        * tripleclick
+        * scrollup
+        * scrolldown
+        * scrollleft
+        * scrollright
+
+2. You can also connect multiple keyboard actions together by using the "chain" function.
+
+    2.1. Write text - This doesn't work well with non-english character. For this you can use the "pastetext" function.
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg"),
+            dict(write="Hello World!"),
+            debug=True
+        )
+    ```
+
+    <img alt="write" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/write.gif" width="918px" height="600px"/>
+
+    2.2. Paste text - This works well with non-english characters
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg"),
+            dict(pastetext="Straße"),
+            debug=True
+        )
+    ```
+
+    2.3. Key combinations
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(keys2="ctrl+a", wait=1),
+            dict(keys2="ctrl+x", wait=1),
+            dict(keys2="alt+f4", wait=1),  # close notepad
+            debug=True
+        )
+    ```
+
+    <img alt="keys" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/keys.gif" width="918px" height="600px"/>
+
+    2.4. All key actions:
+
+        * write
+        * pastetext
+        * keys
+        * keys2 - best option overall for key combinations
+        * keys3
+        * keys4
+        * copy
+        * paste
+
+3. Wait actions:
+
+    3.1. Wait until an image appears on the screen
+    This can used when you are waiting for a window to finish loading completely and you don't know exactly how long that would take.
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg"),
+            dict(waituntil="demo/notepad_opened.jpg", wait=1),
+            dict(write="Hello World!", wait=1),
+            debug=True
+        )
+    ```
+
+    3.2. Wait while an image is on the screen
+
+4. App (window) actions:
+
+    4.1. Open an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(waituntil="demo/notepad_opened.jpg", wait=1),
+            dict(write="Hello World!", wait=1),
+            debug=True
+        )
+    ```
+
+    4.2. Close an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(close="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.3. Minimize an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(minimize="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.4. Maximize an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(maximize="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.5. Restore an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(minimize="Notepad", wait=1),
+            dict(restore="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.6. All app actions:
+
+        * open_app
+        * close
+        * startfile
+        * focus
+        * minimize
+        * maximize
+        * restore
+        * msoffice_replace
+        * copy_from
+        * copy_from_to
+
+5. Image actions
+
+    5.1 count_img. With this function you can count how many times one image appears on the screen.
+
+    ```python
+        chain(
+            dict(count_img="demo/M.jpg", wait=1),  # The result will be copied to the clipboard
+            dict(open_app="notepad++.exe", wait=1),
+            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
+            debug=True
+        )
+    ```
+
+    5.2. get_text_from_region
+
+    ```python
+        chain(
+            dict(get_text_from_region=((136, 121), (189, 140)), wait=1),  # The text will be copied to the clipboard
+            dict(open_app="notepad++.exe", wait=1),
+            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
+            debug=True
+        )
+    ```
+
+# Roadmap
+1. Check if possible to add <a href="https://github.com/pywinauto/pywinauto">pyautowin</a> functionality
+
+# Frequently Asked Questions:
+
+1. I made an image but it doesn't click on it.
+
+    A: Make sure you have not changed resolution of your screen or the theme (dark/light) of the window.
+
+
+2. Keys combination using "keys" function doesn't work.
+
+    A: Try other keys functions. Preferably "keys2". Other options "keys3", "keys4".
```

#### html2text {}

```diff
@@ -1,92 +1,92 @@
-Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.5 Summary: Python
+Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.6 Summary: Python
 Automation using Mouse and Keyboard, for the masses Home-page: https://
 github.com/MihailCosmin/automonkey Author: Mihail-Cosmin Munteanu Author-email:
 Mihail-Cosmin Munteanu
 gmail.com> License: GNU General Public License v3 Project-URL: Homepage, https:
 //github.com/MihailCosmin/AutoMonkey Project-URL: Bug Tracker, https://
 github.com/MihailCosmin/AutoMonkey/issues Keywords: automonkey Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 AUTHORS.rst [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)]
-(https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4) [![Known
-Vulnerabilities](https://snyk.io/test/github/MihailCosmin/AutoMonkey/
-badge.svg)](https://snyk.io/test/github/MihailCosmin/AutoMonkey) [![HitCount]
-(https://hits.dwyl.com/MihailCosmin/AutoMonkey.svg?style=flat-
-square&show=unique)](http://hits.dwyl.com/MihailCosmin/AutoMonkey) [![build]
-(https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-
-package.yml/badge.svg)](https://github.com/MihailCosmin/AutoMonkey/actions/
-workflows/python-package.yml) [![Code Climate](https://codeclimate.com/github/
-MihailCosmin/AutoMonkey/badges/gpa.svg)](https://codeclimate.com/github/
-MihailCosmin/AutoMonkey) # AutoMonkey [AutoMonkey] Python Automation using
-Mouse and Keyboard, for the masses # Installation 1. From pypi: ``` pip install
-AutoMonkey ``` 2. From github: ``` pip install git+https://github.com/
-MihailCosmin/AutoMonkey ``` # Dependencies #### Automonkey is based on: -
-pyautogui #### Other dependencies: - PyScreeze - pyperclip - clipboard -
-keyboard - screeninfo - pywin32 - pillow - opencv-python - numpy - pytesseract
-# Usage Main function to be used is "chain" This will allow you to "chain"
-together most of the other functions of automonkey. Which in turn will enable
-you to create sequences of mouse and/or keyboard actions in order to automate
-any given task. A step can have this structure: ```python dict(  = , # action
-can be any of the automonkey functions, target on which the action will be
-performed wait = 1, # wait is an optional parameter, which will wait for the
-given amount of seconds before executing the next step skip = False, # if True,
-will skip this step confidence = 0.9, # confidence is an optional parameter,
-Used only for actions on images. Confidence on locating the image. v_offset =
-0, # v_offset is an optional parameter, Used only for actions on images.
-Vertical offset from the center of the image. h_offset = 0, # h_offset is an
-optional parameter, Used only for actions on images. Horizontal offset from the
-center of the image. offset = 0, # offset is an optional parameter, Used only
-for actions on images. Offset from the center of the image. monitor = 0, #
-monitor is an optional parameter, Used only for actions on images. Monitor on
-which to search for the image. ) or { "": "", # action can be any of the
-automonkey functions, target on which the action will be performed "wait": 1, #
-wait is an optional parameter, which will wait for the given amount of seconds
-before executing the next step "skip": False, # if True, will skip this step
-"confidence": 0.9, # confidence is an optional parameter, Used only for actions
-on images. Confidence on locating the image. "v_offset": 0, # v_offset is an
-optional parameter, Used only for actions on images. Vertical offset from the
-center of the image. "h_offset": 0, # h_offset is an optional parameter, Used
-only for actions on images. Horizontal offset from the center of the image.
-"offset": 0, # offset is an optional parameter, Used only for actions on
-images. Offset from the center of the image. "monitor": 0, # monitor is an
-optional parameter, Used only for actions on images. Monitor on which to search
-for the image. } ``` 1. You can connect multiple mouse actions together by
-using the "chain" function. Just by doing this you can generally automate most
-of the tasks you would do on a daily basis. There are 2 main ways to click,
-either by giving the coordinates of the position where to click or by giving
-the filename of the image you want to click on 1.1. Clicking by coordinates
-1.1.1. In order to find the coordinates of a position on the screen you can use
-the "track_mouse" function or the PositionTracker class ```python from
-automonkey import track_mouse track_mouse() ``` [track_mouse] ```python from
-automonkey import PositionTracker tracker = PositionTracker() tracker.start()
-``` [PositionTracker] 1.2.1. Now that you have the coordinates of the position
-you want to click on, you can use the "chain" function to click on it ```python
-from automonkey import chain chain( dict(click=(780, 1175), wait=1), dict
-(click=(444, 194), wait=1), dict(click=(1892, 110), wait=1), debug=True ) ```
-[click] 1.2. Clicking by image 1.2.1. To click on an image you first need to
-make a screenshot of the area you want to click on and save it somewhere on
-your computer. For this you can use any screenshot tool you want, or you could
-use monkeyshot: https://github.com/MihailCosmin/monkeyshot For example you can
-make a screenshot of the Edge icon from your toolbar, then we can click on it
-by using the "chain" function. [edge_toolbar] 1.2.2. Now that we have the image
-we want to click on, we can use the "chain" function to click on it ```python
-chain( dict(click="demo/edge_toolbar.jpg"), dict(click="demo/
-google_create_account", wait=1), dict(click="demo/personal_use", wait=1),
-debug=True ) ``` [click_image] 1.3. All mouse actions: * click * rightclick *
-leftclick * doubleclick * tripleclick * scrollup * scrolldown * scrollleft *
-scrollright 2. You can also connect multiple keyboard actions together by using
-the "chain" function. 2.1. Write text - This doesn't work well with non-english
-character. For this you can use the "pastetext" function. ```python chain( dict
-(click="demo/notepad.jpg"), dict(write="Hello World!"), debug=True ) ```
-[write] 2.2. Paste text - This works well with non-english characters ```python
-chain( dict(click="demo/notepad.jpg"), dict(pastetext="StraÃe"), debug=True )
-``` 2.3. Key combinations ```python chain( dict(click="demo/notepad.jpg",
-wait=1), dict(write="Hello World!", wait=1), dict(keys2="ctrl+a", wait=1), dict
+(https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4) [![](https://
+snyk.io/test/github/MihailCosmin/AutoMonkey/badge.svg)](https://snyk.io/test/
+github/MihailCosmin/AutoMonkey) [![HitCount](https://hits.dwyl.com/
+MihailCosmin/AutoMonkey.svg?style=flat-square&show=unique)](http://
+hits.dwyl.com/MihailCosmin/AutoMonkey) [![build](https://github.com/
+MihailCosmin/AutoMonkey/actions/workflows/python-package.yml/badge.svg)](https:
+//github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml) [!
+[Code Climate](https://codeclimate.com/github/MihailCosmin/AutoMonkey/badges/
+gpa.svg)](https://codeclimate.com/github/MihailCosmin/AutoMonkey) # AutoMonkey
+[AutoMonkey] Python Automation using Mouse and Keyboard, for the masses #
+Installation 1. From pypi: ``` pip install AutoMonkey ``` 2. From github: ```
+pip install git+https://github.com/MihailCosmin/AutoMonkey ``` # Dependencies
+#### Automonkey is based on: - pyautogui #### Other dependencies: - PyScreeze -
+pyperclip - clipboard - keyboard - screeninfo - pywin32 - pillow - opencv-
+python - numpy - pytesseract # Usage Main function to be used is "chain" This
+will allow you to "chain" together most of the other functions of automonkey.
+Which in turn will enable you to create sequences of mouse and/or keyboard
+actions in order to automate any given task. A step can have this structure:
+```python dict(  = , # action can be any of the automonkey functions, target on
+which the action will be performed wait = 1, # wait is an optional parameter,
+which will wait for the given amount of seconds before executing the next step
+skip = False, # if True, will skip this step confidence = 0.9, # confidence is
+an optional parameter, Used only for actions on images. Confidence on locating
+the image. v_offset = 0, # v_offset is an optional parameter, Used only for
+actions on images. Vertical offset from the center of the image. h_offset = 0,
+# h_offset is an optional parameter, Used only for actions on images.
+Horizontal offset from the center of the image. offset = 0, # offset is an
+optional parameter, Used only for actions on images. Offset from the center of
+the image. monitor = 0, # monitor is an optional parameter, Used only for
+actions on images. Monitor on which to search for the image. ) or { "": "", #
+action can be any of the automonkey functions, target on which the action will
+be performed "wait": 1, # wait is an optional parameter, which will wait for
+the given amount of seconds before executing the next step "skip": False, # if
+True, will skip this step "confidence": 0.9, # confidence is an optional
+parameter, Used only for actions on images. Confidence on locating the image.
+"v_offset": 0, # v_offset is an optional parameter, Used only for actions on
+images. Vertical offset from the center of the image. "h_offset": 0, # h_offset
+is an optional parameter, Used only for actions on images. Horizontal offset
+from the center of the image. "offset": 0, # offset is an optional parameter,
+Used only for actions on images. Offset from the center of the image.
+"monitor": 0, # monitor is an optional parameter, Used only for actions on
+images. Monitor on which to search for the image. } ``` 1. You can connect
+multiple mouse actions together by using the "chain" function. Just by doing
+this you can generally automate most of the tasks you would do on a daily
+basis. There are 2 main ways to click, either by giving the coordinates of the
+position where to click or by giving the filename of the image you want to
+click on 1.1. Clicking by coordinates 1.1.1. In order to find the coordinates
+of a position on the screen you can use the "track_mouse" function or the
+PositionTracker class ```python from automonkey import track_mouse track_mouse
+() ``` [track_mouse] ```python from automonkey import PositionTracker tracker =
+PositionTracker() tracker.start() ``` [PositionTracker] 1.2.1. Now that you
+have the coordinates of the position you want to click on, you can use the
+"chain" function to click on it ```python from automonkey import chain chain
+( dict(click=(780, 1175), wait=1), dict(click=(444, 194), wait=1), dict(click=
+(1892, 110), wait=1), debug=True ) ``` [click] 1.2. Clicking by image 1.2.1. To
+click on an image you first need to make a screenshot of the area you want to
+click on and save it somewhere on your computer. For this you can use any
+screenshot tool you want, or you could use monkeyshot: https://github.com/
+MihailCosmin/monkeyshot For example you can make a screenshot of the Edge icon
+from your toolbar, then we can click on it by using the "chain" function.
+[edge_toolbar] 1.2.2. Now that we have the image we want to click on, we can
+use the "chain" function to click on it ```python chain( dict(click="demo/
+edge_toolbar.jpg"), dict(click="demo/google_create_account", wait=1), dict
+(click="demo/personal_use", wait=1), debug=True ) ``` [click_image] 1.3. All
+mouse actions: * click * rightclick * leftclick * doubleclick * tripleclick *
+scrollup * scrolldown * scrollleft * scrollright 2. You can also connect
+multiple keyboard actions together by using the "chain" function. 2.1. Write
+text - This doesn't work well with non-english character. For this you can use
+the "pastetext" function. ```python chain( dict(click="demo/notepad.jpg"), dict
+(write="Hello World!"), debug=True ) ``` [write] 2.2. Paste text - This works
+well with non-english characters ```python chain( dict(click="demo/
+notepad.jpg"), dict(pastetext="StraÃe"), debug=True ) ``` 2.3. Key
+combinations ```python chain( dict(click="demo/notepad.jpg", wait=1), dict
+(write="Hello World!", wait=1), dict(keys2="ctrl+a", wait=1), dict
 (keys2="ctrl+x", wait=1), dict(keys2="alt+f4", wait=1), # close notepad
 debug=True ) ``` [keys] 2.4. All key actions: * write * pastetext * keys *
 keys2 - best option overall for key combinations * keys3 * keys4 * copy * paste
 3. Wait actions: 3.1. Wait until an image appears on the screen This can used
 when you are waiting for a window to finish loading completely and you don't
 know exactly how long that would take. ```python chain( dict(click="demo/
 notepad.jpg"), dict(waituntil="demo/notepad_opened.jpg", wait=1), dict
```

### Comparing `AutoMonkey-0.1.5/AutoMonkey.egg-info/SOURCES.txt` & `AutoMonkey-0.1.6/AutoMonkey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.5/CONTRIBUTING.rst` & `AutoMonkey-0.1.6/CONTRIBUTING.rst`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-.. highlight:: shell
-
-============
-Contributing
-============
-
-Contributions are welcome, and they are greatly appreciated! Every little bit
-helps, and credit will always be given.
-
-You can contribute in many ways:
-
-Types of Contributions
-----------------------
-
-Report Bugs
-~~~~~~~~~~~
-
-Report bugs at https://github.com/MihailCosmin/automonkey/issues.
-
-If you are reporting a bug, please include:
-
-* Your operating system name and version.
-* Any details about your local setup that might be helpful in troubleshooting.
-* Detailed steps to reproduce the bug.
-
-Fix Bugs
-~~~~~~~~
-
-Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
-wanted" is open to whoever wants to implement it.
-
-Implement Features
-~~~~~~~~~~~~~~~~~~
-
-Look through the GitHub issues for features. Anything tagged with "enhancement"
-and "help wanted" is open to whoever wants to implement it.
-
-Write Documentation
-~~~~~~~~~~~~~~~~~~~
-
-automonkey could always use more documentation, whether as part of the
-official automonkey docs, in docstrings, or even on the web in blog posts,
-articles, and such.
-
-Submit Feedback
-~~~~~~~~~~~~~~~
-
-The best way to send feedback is to file an issue at https://github.com/MihailCosmin/automonkey/issues.
-
-If you are proposing a feature:
-
-* Explain in detail how it would work.
-* Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that contributions
-  are welcome :)
-
-Get Started!
-------------
-
-Ready to contribute? Here's how to set up `automonkey` for local development.
-
-1. Fork the `automonkey` repo on GitHub.
-2. Clone your fork locally::
-
-    $ git clone git@github.com:your_name_here/automonkey.git
-
-3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
-
-    $ mkvirtualenv automonkey
-    $ cd automonkey/
-    $ python setup.py develop
-
-4. Create a branch for local development::
-
-    $ git checkout -b name-of-your-bugfix-or-feature
-
-   Now you can make your changes locally.
-
-5. When you're done making changes, check that your changes pass flake8 and the
-   tests, including testing other Python versions with tox::
-
-    $ flake8 automonkey tests
-    $ python setup.py test or pytest
-    $ tox
-
-   To get flake8 and tox, just pip install them into your virtualenv.
-
-6. Commit your changes and push your branch to GitHub::
-
-    $ git add .
-    $ git commit -m "Your detailed description of your changes."
-    $ git push origin name-of-your-bugfix-or-feature
-
-7. Submit a pull request through the GitHub website.
-
-Pull Request Guidelines
------------------------
-
-Before you submit a pull request, check that it meets these guidelines:
-
-1. The pull request should include tests.
-2. If the pull request adds functionality, the docs should be updated. Put
-   your new functionality into a function with a docstring, and add the
-   feature to the list in README.rst.
-3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
-   https://travis-ci.com/MihailCosmin/automonkey/pull_requests
-   and make sure that the tests pass for all supported Python versions.
-
-Tips
-----
-
-To run a subset of tests::
-
-$ pytest tests.test_automonkey
-
-
-Deploying
----------
-
-A reminder for the maintainers on how to deploy.
-Make sure all your changes are committed (including an entry in HISTORY.rst).
-Then run::
-
-$ bump2version patch # possible: major / minor / patch
-$ git push
-$ git push --tags
-
-Travis will then deploy to PyPI if tests pass.
+.. highlight:: shell
+
+============
+Contributing
+============
+
+Contributions are welcome, and they are greatly appreciated! Every little bit
+helps, and credit will always be given.
+
+You can contribute in many ways:
+
+Types of Contributions
+----------------------
+
+Report Bugs
+~~~~~~~~~~~
+
+Report bugs at https://github.com/MihailCosmin/automonkey/issues.
+
+If you are reporting a bug, please include:
+
+* Your operating system name and version.
+* Any details about your local setup that might be helpful in troubleshooting.
+* Detailed steps to reproduce the bug.
+
+Fix Bugs
+~~~~~~~~
+
+Look through the GitHub issues for bugs. Anything tagged with "bug" and "help
+wanted" is open to whoever wants to implement it.
+
+Implement Features
+~~~~~~~~~~~~~~~~~~
+
+Look through the GitHub issues for features. Anything tagged with "enhancement"
+and "help wanted" is open to whoever wants to implement it.
+
+Write Documentation
+~~~~~~~~~~~~~~~~~~~
+
+automonkey could always use more documentation, whether as part of the
+official automonkey docs, in docstrings, or even on the web in blog posts,
+articles, and such.
+
+Submit Feedback
+~~~~~~~~~~~~~~~
+
+The best way to send feedback is to file an issue at https://github.com/MihailCosmin/automonkey/issues.
+
+If you are proposing a feature:
+
+* Explain in detail how it would work.
+* Keep the scope as narrow as possible, to make it easier to implement.
+* Remember that this is a volunteer-driven project, and that contributions
+  are welcome :)
+
+Get Started!
+------------
+
+Ready to contribute? Here's how to set up `automonkey` for local development.
+
+1. Fork the `automonkey` repo on GitHub.
+2. Clone your fork locally::
+
+    $ git clone git@github.com:your_name_here/automonkey.git
+
+3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
+
+    $ mkvirtualenv automonkey
+    $ cd automonkey/
+    $ python setup.py develop
+
+4. Create a branch for local development::
+
+    $ git checkout -b name-of-your-bugfix-or-feature
+
+   Now you can make your changes locally.
+
+5. When you're done making changes, check that your changes pass flake8 and the
+   tests, including testing other Python versions with tox::
+
+    $ flake8 automonkey tests
+    $ python setup.py test or pytest
+    $ tox
+
+   To get flake8 and tox, just pip install them into your virtualenv.
+
+6. Commit your changes and push your branch to GitHub::
+
+    $ git add .
+    $ git commit -m "Your detailed description of your changes."
+    $ git push origin name-of-your-bugfix-or-feature
+
+7. Submit a pull request through the GitHub website.
+
+Pull Request Guidelines
+-----------------------
+
+Before you submit a pull request, check that it meets these guidelines:
+
+1. The pull request should include tests.
+2. If the pull request adds functionality, the docs should be updated. Put
+   your new functionality into a function with a docstring, and add the
+   feature to the list in README.rst.
+3. The pull request should work for Python 3.5, 3.6, 3.7 and 3.8, and for PyPy. Check
+   https://travis-ci.com/MihailCosmin/automonkey/pull_requests
+   and make sure that the tests pass for all supported Python versions.
+
+Tips
+----
+
+To run a subset of tests::
+
+$ pytest tests.test_automonkey
+
+
+Deploying
+---------
+
+A reminder for the maintainers on how to deploy.
+Make sure all your changes are committed (including an entry in HISTORY.rst).
+Then run::
+
+$ bump2version patch # possible: major / minor / patch
+$ git push
+$ git push --tags
+
+Travis will then deploy to PyPI if tests pass.
```

### Comparing `AutoMonkey-0.1.5/LICENSE` & `AutoMonkey-0.1.6/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-GNU GENERAL PUBLIC LICENSE
-                      Version 3, 29 June 2007
-
-    Python Automation using Mouse and Keyboard for the masses
-    Copyright (C) 2021  Mihail-Cosmin Munteanu
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
-
+GNU GENERAL PUBLIC LICENSE
+                      Version 3, 29 June 2007
+
+    Python Automation using Mouse and Keyboard for the masses
+    Copyright (C) 2021  Mihail-Cosmin Munteanu
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+
```

### Comparing `AutoMonkey-0.1.5/PKG-INFO` & `AutoMonkey-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,342 +1,342 @@
-Metadata-Version: 2.1
-Name: AutoMonkey
-Version: 0.1.5
-Summary: Python Automation using Mouse and Keyboard, for the masses
-Home-page: https://github.com/MihailCosmin/automonkey
-Author: Mihail-Cosmin Munteanu
-Author-email: Mihail-Cosmin Munteanu <munteanumihailcosmin@gmail.com>
-License: GNU General Public License v3
-Project-URL: Homepage, https://github.com/MihailCosmin/AutoMonkey
-Project-URL: Bug Tracker, https://github.com/MihailCosmin/AutoMonkey/issues
-Keywords: automonkey
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4)
-[![Known Vulnerabilities](https://snyk.io/test/github/MihailCosmin/AutoMonkey/badge.svg)](https://snyk.io/test/github/MihailCosmin/AutoMonkey)
-[![HitCount](https://hits.dwyl.com/MihailCosmin/AutoMonkey.svg?style=flat-square&show=unique)](http://hits.dwyl.com/MihailCosmin/AutoMonkey)
-[![build](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml/badge.svg)](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml)
-[![Code Climate](https://codeclimate.com/github/MihailCosmin/AutoMonkey/badges/gpa.svg)](https://codeclimate.com/github/MihailCosmin/AutoMonkey)
-
-# AutoMonkey
-<img alt="AutoMonkey" src="https://github.com/MihailCosmin/AutoMonkey/raw/06181954fa23605583d61843226f5f3997157435/img/monkey.ico" width="100px" height="100px"/>
-
-Python Automation using Mouse and Keyboard, for the masses
-
-# Installation
-
-1. From <a href="https://pypi.org/project/AutoMonkey/">pypi</a>:
-
-```
-pip install AutoMonkey
-```
-
-2. From <a href="https://github.com/MihailCosmin/AutoMonkey">github</a>:
-
-```
-pip install git+https://github.com/MihailCosmin/AutoMonkey
-```
-
-# Dependencies
-#### Automonkey is based on:
-- <a href="https://github.com/asweigart/pyautogui">pyautogui</a>
-
-#### Other dependencies:
-- PyScreeze
-- pyperclip
-- clipboard
-- keyboard
-- screeninfo
-- pywin32
-- pillow
-- opencv-python
-- numpy
-- pytesseract
-
-# Usage
-Main function to be used is "chain"  
-
-This will allow you to "chain" together most of the other functions of automonkey.  
-Which in turn will enable you to create sequences of mouse and/or keyboard actions in order to automate any given task.
-
-A step can have this structure:
-
-```python
-
-dict(
-    <action> = <target>,  # action can be any of the automonkey functions, target on which the action will be performed
-    wait = 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
-    skip = False,  # if True, will skip this step
-    confidence = 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
-    v_offset = 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
-    h_offset = 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
-    offset = 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
-    monitor = 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
-)
-
-or 
-
-{
-    "<action>": "<target>",  # action can be any of the automonkey functions, target on which the action will be performed
-    "wait": 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
-    "skip": False,  # if True, will skip this step
-    "confidence": 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
-    "v_offset": 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
-    "h_offset": 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
-    "offset": 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
-    "monitor": 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
-}
-```
-
-1. You can connect multiple mouse actions together by using the "chain" function. Just by doing this you can generally automate most of the tasks you would do on a daily basis.
-
-    There are 2 main ways to click, either by giving the coordinates of the position where to click or by giving the filename of the image you want to click on
-
-    1.1. Clicking by coordinates
-        
-    
-    1.1.1. In order to find the coordinates of a position on the screen you can use the "track_mouse" function or the PositionTracker class
-
-    ```python
-        from automonkey import track_mouse
-        track_mouse()
-    ```
-
-    <img alt="track_mouse" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/track_mouse.gif" width="416px" height="304px"/>
-
-
-    ```python
-        from automonkey import PositionTracker
-        tracker = PositionTracker()
-        tracker.start()
-    ```
-
-    <img alt="PositionTracker" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/PositionTracker.gif" width="918px" height="574px"/>
-
-    1.2.1. Now that you have the coordinates of the position you want to click on, you can use the "chain" function to click on it
-
-
-    ```python
-        from automonkey import chain
-        chain(  
-            dict(click=(780, 1175), wait=1),  
-            dict(click=(444, 194), wait=1),  
-            dict(click=(1892, 110), wait=1),  
-            debug=True  
-        )
-    ```
-
-    <img alt="click" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click.gif" width="960px" height="576px"/>
-
-    1.2. Clicking by image
-
-    1.2.1. To click on an image you first need to make a screenshot of the area you want to click on and save it somewhere on your computer.
-        For this you can use any screenshot tool you want, or you could use monkeyshot: https://github.com/MihailCosmin/monkeyshot
-        For example you can make a screenshot of the Edge icon from your toolbar, then we can click on it by using the "chain" function.
-
-    <img alt="edge_toolbar" src="https://github.com/MihailCosmin/AutoMonkey/raw/25eaed263793bf548d42f616e241f435baa9d719/demo/edge_toolbar.jpg" width="33px" height="33px"/>
-
-    1.2.2. Now that we have the image we want to click on, we can use the "chain" function to click on it
-
-    ```python
-        chain(
-            dict(click="demo/edge_toolbar.jpg"),
-            dict(click="demo/google_create_account", wait=1),
-            dict(click="demo/personal_use", wait=1),
-            debug=True
-        )
-    ```
-
-    <img alt="click_image" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click_image.gif" width="918px" height="600px"/>
-
-    1.3. All mouse actions:
-
-        * click
-        * rightclick
-        * leftclick
-        * doubleclick
-        * tripleclick
-        * scrollup
-        * scrolldown
-        * scrollleft
-        * scrollright
-
-2. You can also connect multiple keyboard actions together by using the "chain" function.
-
-    2.1. Write text - This doesn't work well with non-english character. For this you can use the "pastetext" function.
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg"),
-            dict(write="Hello World!"),
-            debug=True
-        )
-    ```
-
-    <img alt="write" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/write.gif" width="918px" height="600px"/>
-
-    2.2. Paste text - This works well with non-english characters
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg"),
-            dict(pastetext="Straße"),
-            debug=True
-        )
-    ```
-
-    2.3. Key combinations
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(keys2="ctrl+a", wait=1),
-            dict(keys2="ctrl+x", wait=1),
-            dict(keys2="alt+f4", wait=1),  # close notepad
-            debug=True
-        )
-    ```
-
-    <img alt="keys" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/keys.gif" width="918px" height="600px"/>
-
-    2.4. All key actions:
-
-        * write
-        * pastetext
-        * keys
-        * keys2 - best option overall for key combinations
-        * keys3
-        * keys4
-        * copy
-        * paste
-
-3. Wait actions:
-
-    3.1. Wait until an image appears on the screen
-    This can used when you are waiting for a window to finish loading completely and you don't know exactly how long that would take.
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg"),
-            dict(waituntil="demo/notepad_opened.jpg", wait=1),
-            dict(write="Hello World!", wait=1),
-            debug=True
-        )
-    ```
-
-    3.2. Wait while an image is on the screen
-
-4. App (window) actions:
-
-    4.1. Open an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(waituntil="demo/notepad_opened.jpg", wait=1),
-            dict(write="Hello World!", wait=1),
-            debug=True
-        )
-    ```
-
-    4.2. Close an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(close="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.3. Minimize an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(minimize="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.4. Maximize an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(maximize="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.5. Restore an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(minimize="Notepad", wait=1),
-            dict(restore="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.6. All app actions:
-
-        * open_app
-        * close
-        * startfile
-        * focus
-        * minimize
-        * maximize
-        * restore
-        * msoffice_replace
-        * copy_from
-        * copy_from_to
-
-5. Image actions
-
-    5.1 count_img. With this function you can count how many times one image appears on the screen.
-
-    ```python
-        chain(
-            dict(count_img="demo/M.jpg", wait=1),  # The result will be copied to the clipboard
-            dict(open_app="notepad++.exe", wait=1),
-            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
-            debug=True
-        )
-    ```
-
-    5.2. get_text_from_region
-
-    ```python
-        chain(
-            dict(get_text_from_region=((136, 121), (189, 140)), wait=1),  # The text will be copied to the clipboard
-            dict(open_app="notepad++.exe", wait=1),
-            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
-            debug=True
-        )
-    ```
-
-# Roadmap
-1. Check if possible to add <a href="https://github.com/pywinauto/pywinauto">pyautowin</a> functionality
-
-# Frequently Asked Questions:
-
-1. I made an image but it doesn't click on it.
-
-    A: Make sure you have not changed resolution of your screen or the theme (dark/light) of the window.
-
-
-2. Keys combination using "keys" function doesn't work.
-
-    A: Try other keys functions. Preferably "keys2". Other options "keys3", "keys4".
+Metadata-Version: 2.1
+Name: AutoMonkey
+Version: 0.1.6
+Summary: Python Automation using Mouse and Keyboard, for the masses
+Home-page: https://github.com/MihailCosmin/automonkey
+Author: Mihail-Cosmin Munteanu
+Author-email: Mihail-Cosmin Munteanu <munteanumihailcosmin@gmail.com>
+License: GNU General Public License v3
+Project-URL: Homepage, https://github.com/MihailCosmin/AutoMonkey
+Project-URL: Bug Tracker, https://github.com/MihailCosmin/AutoMonkey/issues
+Keywords: automonkey
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4)
+[![](https://snyk.io/test/github/MihailCosmin/AutoMonkey/badge.svg)](https://snyk.io/test/github/MihailCosmin/AutoMonkey)
+[![HitCount](https://hits.dwyl.com/MihailCosmin/AutoMonkey.svg?style=flat-square&show=unique)](http://hits.dwyl.com/MihailCosmin/AutoMonkey)
+[![build](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml/badge.svg)](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml)
+[![Code Climate](https://codeclimate.com/github/MihailCosmin/AutoMonkey/badges/gpa.svg)](https://codeclimate.com/github/MihailCosmin/AutoMonkey)
+
+# AutoMonkey
+<img alt="AutoMonkey" src="https://github.com/MihailCosmin/AutoMonkey/raw/06181954fa23605583d61843226f5f3997157435/img/monkey.ico" width="100px" height="100px"/>
+
+Python Automation using Mouse and Keyboard, for the masses
+
+# Installation
+
+1. From <a href="https://pypi.org/project/AutoMonkey/">pypi</a>:
+
+```
+pip install AutoMonkey
+```
+
+2. From <a href="https://github.com/MihailCosmin/AutoMonkey">github</a>:
+
+```
+pip install git+https://github.com/MihailCosmin/AutoMonkey
+```
+
+# Dependencies
+#### Automonkey is based on:
+- <a href="https://github.com/asweigart/pyautogui">pyautogui</a>
+
+#### Other dependencies:
+- PyScreeze
+- pyperclip
+- clipboard
+- keyboard
+- screeninfo
+- pywin32
+- pillow
+- opencv-python
+- numpy
+- pytesseract
+
+# Usage
+Main function to be used is "chain"  
+
+This will allow you to "chain" together most of the other functions of automonkey.  
+Which in turn will enable you to create sequences of mouse and/or keyboard actions in order to automate any given task.
+
+A step can have this structure:
+
+```python
+
+dict(
+    <action> = <target>,  # action can be any of the automonkey functions, target on which the action will be performed
+    wait = 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
+    skip = False,  # if True, will skip this step
+    confidence = 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
+    v_offset = 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
+    h_offset = 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
+    offset = 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
+    monitor = 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
+)
+
+or 
+
+{
+    "<action>": "<target>",  # action can be any of the automonkey functions, target on which the action will be performed
+    "wait": 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
+    "skip": False,  # if True, will skip this step
+    "confidence": 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
+    "v_offset": 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
+    "h_offset": 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
+    "offset": 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
+    "monitor": 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
+}
+```
+
+1. You can connect multiple mouse actions together by using the "chain" function. Just by doing this you can generally automate most of the tasks you would do on a daily basis.
+
+    There are 2 main ways to click, either by giving the coordinates of the position where to click or by giving the filename of the image you want to click on
+
+    1.1. Clicking by coordinates
+        
+    
+    1.1.1. In order to find the coordinates of a position on the screen you can use the "track_mouse" function or the PositionTracker class
+
+    ```python
+        from automonkey import track_mouse
+        track_mouse()
+    ```
+
+    <img alt="track_mouse" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/track_mouse.gif" width="416px" height="304px"/>
+
+
+    ```python
+        from automonkey import PositionTracker
+        tracker = PositionTracker()
+        tracker.start()
+    ```
+
+    <img alt="PositionTracker" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/PositionTracker.gif" width="918px" height="574px"/>
+
+    1.2.1. Now that you have the coordinates of the position you want to click on, you can use the "chain" function to click on it
+
+
+    ```python
+        from automonkey import chain
+        chain(  
+            dict(click=(780, 1175), wait=1),  
+            dict(click=(444, 194), wait=1),  
+            dict(click=(1892, 110), wait=1),  
+            debug=True  
+        )
+    ```
+
+    <img alt="click" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click.gif" width="960px" height="576px"/>
+
+    1.2. Clicking by image
+
+    1.2.1. To click on an image you first need to make a screenshot of the area you want to click on and save it somewhere on your computer.
+        For this you can use any screenshot tool you want, or you could use monkeyshot: https://github.com/MihailCosmin/monkeyshot
+        For example you can make a screenshot of the Edge icon from your toolbar, then we can click on it by using the "chain" function.
+
+    <img alt="edge_toolbar" src="https://github.com/MihailCosmin/AutoMonkey/raw/25eaed263793bf548d42f616e241f435baa9d719/demo/edge_toolbar.jpg" width="33px" height="33px"/>
+
+    1.2.2. Now that we have the image we want to click on, we can use the "chain" function to click on it
+
+    ```python
+        chain(
+            dict(click="demo/edge_toolbar.jpg"),
+            dict(click="demo/google_create_account", wait=1),
+            dict(click="demo/personal_use", wait=1),
+            debug=True
+        )
+    ```
+
+    <img alt="click_image" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click_image.gif" width="918px" height="600px"/>
+
+    1.3. All mouse actions:
+
+        * click
+        * rightclick
+        * leftclick
+        * doubleclick
+        * tripleclick
+        * scrollup
+        * scrolldown
+        * scrollleft
+        * scrollright
+
+2. You can also connect multiple keyboard actions together by using the "chain" function.
+
+    2.1. Write text - This doesn't work well with non-english character. For this you can use the "pastetext" function.
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg"),
+            dict(write="Hello World!"),
+            debug=True
+        )
+    ```
+
+    <img alt="write" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/write.gif" width="918px" height="600px"/>
+
+    2.2. Paste text - This works well with non-english characters
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg"),
+            dict(pastetext="Straße"),
+            debug=True
+        )
+    ```
+
+    2.3. Key combinations
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(keys2="ctrl+a", wait=1),
+            dict(keys2="ctrl+x", wait=1),
+            dict(keys2="alt+f4", wait=1),  # close notepad
+            debug=True
+        )
+    ```
+
+    <img alt="keys" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/keys.gif" width="918px" height="600px"/>
+
+    2.4. All key actions:
+
+        * write
+        * pastetext
+        * keys
+        * keys2 - best option overall for key combinations
+        * keys3
+        * keys4
+        * copy
+        * paste
+
+3. Wait actions:
+
+    3.1. Wait until an image appears on the screen
+    This can used when you are waiting for a window to finish loading completely and you don't know exactly how long that would take.
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg"),
+            dict(waituntil="demo/notepad_opened.jpg", wait=1),
+            dict(write="Hello World!", wait=1),
+            debug=True
+        )
+    ```
+
+    3.2. Wait while an image is on the screen
+
+4. App (window) actions:
+
+    4.1. Open an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(waituntil="demo/notepad_opened.jpg", wait=1),
+            dict(write="Hello World!", wait=1),
+            debug=True
+        )
+    ```
+
+    4.2. Close an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(close="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.3. Minimize an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(minimize="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.4. Maximize an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(maximize="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.5. Restore an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(minimize="Notepad", wait=1),
+            dict(restore="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.6. All app actions:
+
+        * open_app
+        * close
+        * startfile
+        * focus
+        * minimize
+        * maximize
+        * restore
+        * msoffice_replace
+        * copy_from
+        * copy_from_to
+
+5. Image actions
+
+    5.1 count_img. With this function you can count how many times one image appears on the screen.
+
+    ```python
+        chain(
+            dict(count_img="demo/M.jpg", wait=1),  # The result will be copied to the clipboard
+            dict(open_app="notepad++.exe", wait=1),
+            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
+            debug=True
+        )
+    ```
+
+    5.2. get_text_from_region
+
+    ```python
+        chain(
+            dict(get_text_from_region=((136, 121), (189, 140)), wait=1),  # The text will be copied to the clipboard
+            dict(open_app="notepad++.exe", wait=1),
+            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
+            debug=True
+        )
+    ```
+
+# Roadmap
+1. Check if possible to add <a href="https://github.com/pywinauto/pywinauto">pyautowin</a> functionality
+
+# Frequently Asked Questions:
+
+1. I made an image but it doesn't click on it.
+
+    A: Make sure you have not changed resolution of your screen or the theme (dark/light) of the window.
+
+
+2. Keys combination using "keys" function doesn't work.
+
+    A: Try other keys functions. Preferably "keys2". Other options "keys3", "keys4".
```

#### html2text {}

```diff
@@ -1,92 +1,92 @@
-Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.5 Summary: Python
+Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.6 Summary: Python
 Automation using Mouse and Keyboard, for the masses Home-page: https://
 github.com/MihailCosmin/automonkey Author: Mihail-Cosmin Munteanu Author-email:
 Mihail-Cosmin Munteanu
 gmail.com> License: GNU General Public License v3 Project-URL: Homepage, https:
 //github.com/MihailCosmin/AutoMonkey Project-URL: Bug Tracker, https://
 github.com/MihailCosmin/AutoMonkey/issues Keywords: automonkey Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE License-File:
 AUTHORS.rst [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)]
-(https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4) [![Known
-Vulnerabilities](https://snyk.io/test/github/MihailCosmin/AutoMonkey/
-badge.svg)](https://snyk.io/test/github/MihailCosmin/AutoMonkey) [![HitCount]
-(https://hits.dwyl.com/MihailCosmin/AutoMonkey.svg?style=flat-
-square&show=unique)](http://hits.dwyl.com/MihailCosmin/AutoMonkey) [![build]
-(https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-
-package.yml/badge.svg)](https://github.com/MihailCosmin/AutoMonkey/actions/
-workflows/python-package.yml) [![Code Climate](https://codeclimate.com/github/
-MihailCosmin/AutoMonkey/badges/gpa.svg)](https://codeclimate.com/github/
-MihailCosmin/AutoMonkey) # AutoMonkey [AutoMonkey] Python Automation using
-Mouse and Keyboard, for the masses # Installation 1. From pypi: ``` pip install
-AutoMonkey ``` 2. From github: ``` pip install git+https://github.com/
-MihailCosmin/AutoMonkey ``` # Dependencies #### Automonkey is based on: -
-pyautogui #### Other dependencies: - PyScreeze - pyperclip - clipboard -
-keyboard - screeninfo - pywin32 - pillow - opencv-python - numpy - pytesseract
-# Usage Main function to be used is "chain" This will allow you to "chain"
-together most of the other functions of automonkey. Which in turn will enable
-you to create sequences of mouse and/or keyboard actions in order to automate
-any given task. A step can have this structure: ```python dict(  = , # action
-can be any of the automonkey functions, target on which the action will be
-performed wait = 1, # wait is an optional parameter, which will wait for the
-given amount of seconds before executing the next step skip = False, # if True,
-will skip this step confidence = 0.9, # confidence is an optional parameter,
-Used only for actions on images. Confidence on locating the image. v_offset =
-0, # v_offset is an optional parameter, Used only for actions on images.
-Vertical offset from the center of the image. h_offset = 0, # h_offset is an
-optional parameter, Used only for actions on images. Horizontal offset from the
-center of the image. offset = 0, # offset is an optional parameter, Used only
-for actions on images. Offset from the center of the image. monitor = 0, #
-monitor is an optional parameter, Used only for actions on images. Monitor on
-which to search for the image. ) or { "": "", # action can be any of the
-automonkey functions, target on which the action will be performed "wait": 1, #
-wait is an optional parameter, which will wait for the given amount of seconds
-before executing the next step "skip": False, # if True, will skip this step
-"confidence": 0.9, # confidence is an optional parameter, Used only for actions
-on images. Confidence on locating the image. "v_offset": 0, # v_offset is an
-optional parameter, Used only for actions on images. Vertical offset from the
-center of the image. "h_offset": 0, # h_offset is an optional parameter, Used
-only for actions on images. Horizontal offset from the center of the image.
-"offset": 0, # offset is an optional parameter, Used only for actions on
-images. Offset from the center of the image. "monitor": 0, # monitor is an
-optional parameter, Used only for actions on images. Monitor on which to search
-for the image. } ``` 1. You can connect multiple mouse actions together by
-using the "chain" function. Just by doing this you can generally automate most
-of the tasks you would do on a daily basis. There are 2 main ways to click,
-either by giving the coordinates of the position where to click or by giving
-the filename of the image you want to click on 1.1. Clicking by coordinates
-1.1.1. In order to find the coordinates of a position on the screen you can use
-the "track_mouse" function or the PositionTracker class ```python from
-automonkey import track_mouse track_mouse() ``` [track_mouse] ```python from
-automonkey import PositionTracker tracker = PositionTracker() tracker.start()
-``` [PositionTracker] 1.2.1. Now that you have the coordinates of the position
-you want to click on, you can use the "chain" function to click on it ```python
-from automonkey import chain chain( dict(click=(780, 1175), wait=1), dict
-(click=(444, 194), wait=1), dict(click=(1892, 110), wait=1), debug=True ) ```
-[click] 1.2. Clicking by image 1.2.1. To click on an image you first need to
-make a screenshot of the area you want to click on and save it somewhere on
-your computer. For this you can use any screenshot tool you want, or you could
-use monkeyshot: https://github.com/MihailCosmin/monkeyshot For example you can
-make a screenshot of the Edge icon from your toolbar, then we can click on it
-by using the "chain" function. [edge_toolbar] 1.2.2. Now that we have the image
-we want to click on, we can use the "chain" function to click on it ```python
-chain( dict(click="demo/edge_toolbar.jpg"), dict(click="demo/
-google_create_account", wait=1), dict(click="demo/personal_use", wait=1),
-debug=True ) ``` [click_image] 1.3. All mouse actions: * click * rightclick *
-leftclick * doubleclick * tripleclick * scrollup * scrolldown * scrollleft *
-scrollright 2. You can also connect multiple keyboard actions together by using
-the "chain" function. 2.1. Write text - This doesn't work well with non-english
-character. For this you can use the "pastetext" function. ```python chain( dict
-(click="demo/notepad.jpg"), dict(write="Hello World!"), debug=True ) ```
-[write] 2.2. Paste text - This works well with non-english characters ```python
-chain( dict(click="demo/notepad.jpg"), dict(pastetext="StraÃe"), debug=True )
-``` 2.3. Key combinations ```python chain( dict(click="demo/notepad.jpg",
-wait=1), dict(write="Hello World!", wait=1), dict(keys2="ctrl+a", wait=1), dict
+(https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4) [![](https://
+snyk.io/test/github/MihailCosmin/AutoMonkey/badge.svg)](https://snyk.io/test/
+github/MihailCosmin/AutoMonkey) [![HitCount](https://hits.dwyl.com/
+MihailCosmin/AutoMonkey.svg?style=flat-square&show=unique)](http://
+hits.dwyl.com/MihailCosmin/AutoMonkey) [![build](https://github.com/
+MihailCosmin/AutoMonkey/actions/workflows/python-package.yml/badge.svg)](https:
+//github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml) [!
+[Code Climate](https://codeclimate.com/github/MihailCosmin/AutoMonkey/badges/
+gpa.svg)](https://codeclimate.com/github/MihailCosmin/AutoMonkey) # AutoMonkey
+[AutoMonkey] Python Automation using Mouse and Keyboard, for the masses #
+Installation 1. From pypi: ``` pip install AutoMonkey ``` 2. From github: ```
+pip install git+https://github.com/MihailCosmin/AutoMonkey ``` # Dependencies
+#### Automonkey is based on: - pyautogui #### Other dependencies: - PyScreeze -
+pyperclip - clipboard - keyboard - screeninfo - pywin32 - pillow - opencv-
+python - numpy - pytesseract # Usage Main function to be used is "chain" This
+will allow you to "chain" together most of the other functions of automonkey.
+Which in turn will enable you to create sequences of mouse and/or keyboard
+actions in order to automate any given task. A step can have this structure:
+```python dict(  = , # action can be any of the automonkey functions, target on
+which the action will be performed wait = 1, # wait is an optional parameter,
+which will wait for the given amount of seconds before executing the next step
+skip = False, # if True, will skip this step confidence = 0.9, # confidence is
+an optional parameter, Used only for actions on images. Confidence on locating
+the image. v_offset = 0, # v_offset is an optional parameter, Used only for
+actions on images. Vertical offset from the center of the image. h_offset = 0,
+# h_offset is an optional parameter, Used only for actions on images.
+Horizontal offset from the center of the image. offset = 0, # offset is an
+optional parameter, Used only for actions on images. Offset from the center of
+the image. monitor = 0, # monitor is an optional parameter, Used only for
+actions on images. Monitor on which to search for the image. ) or { "": "", #
+action can be any of the automonkey functions, target on which the action will
+be performed "wait": 1, # wait is an optional parameter, which will wait for
+the given amount of seconds before executing the next step "skip": False, # if
+True, will skip this step "confidence": 0.9, # confidence is an optional
+parameter, Used only for actions on images. Confidence on locating the image.
+"v_offset": 0, # v_offset is an optional parameter, Used only for actions on
+images. Vertical offset from the center of the image. "h_offset": 0, # h_offset
+is an optional parameter, Used only for actions on images. Horizontal offset
+from the center of the image. "offset": 0, # offset is an optional parameter,
+Used only for actions on images. Offset from the center of the image.
+"monitor": 0, # monitor is an optional parameter, Used only for actions on
+images. Monitor on which to search for the image. } ``` 1. You can connect
+multiple mouse actions together by using the "chain" function. Just by doing
+this you can generally automate most of the tasks you would do on a daily
+basis. There are 2 main ways to click, either by giving the coordinates of the
+position where to click or by giving the filename of the image you want to
+click on 1.1. Clicking by coordinates 1.1.1. In order to find the coordinates
+of a position on the screen you can use the "track_mouse" function or the
+PositionTracker class ```python from automonkey import track_mouse track_mouse
+() ``` [track_mouse] ```python from automonkey import PositionTracker tracker =
+PositionTracker() tracker.start() ``` [PositionTracker] 1.2.1. Now that you
+have the coordinates of the position you want to click on, you can use the
+"chain" function to click on it ```python from automonkey import chain chain
+( dict(click=(780, 1175), wait=1), dict(click=(444, 194), wait=1), dict(click=
+(1892, 110), wait=1), debug=True ) ``` [click] 1.2. Clicking by image 1.2.1. To
+click on an image you first need to make a screenshot of the area you want to
+click on and save it somewhere on your computer. For this you can use any
+screenshot tool you want, or you could use monkeyshot: https://github.com/
+MihailCosmin/monkeyshot For example you can make a screenshot of the Edge icon
+from your toolbar, then we can click on it by using the "chain" function.
+[edge_toolbar] 1.2.2. Now that we have the image we want to click on, we can
+use the "chain" function to click on it ```python chain( dict(click="demo/
+edge_toolbar.jpg"), dict(click="demo/google_create_account", wait=1), dict
+(click="demo/personal_use", wait=1), debug=True ) ``` [click_image] 1.3. All
+mouse actions: * click * rightclick * leftclick * doubleclick * tripleclick *
+scrollup * scrolldown * scrollleft * scrollright 2. You can also connect
+multiple keyboard actions together by using the "chain" function. 2.1. Write
+text - This doesn't work well with non-english character. For this you can use
+the "pastetext" function. ```python chain( dict(click="demo/notepad.jpg"), dict
+(write="Hello World!"), debug=True ) ``` [write] 2.2. Paste text - This works
+well with non-english characters ```python chain( dict(click="demo/
+notepad.jpg"), dict(pastetext="StraÃe"), debug=True ) ``` 2.3. Key
+combinations ```python chain( dict(click="demo/notepad.jpg", wait=1), dict
+(write="Hello World!", wait=1), dict(keys2="ctrl+a", wait=1), dict
 (keys2="ctrl+x", wait=1), dict(keys2="alt+f4", wait=1), # close notepad
 debug=True ) ``` [keys] 2.4. All key actions: * write * pastetext * keys *
 keys2 - best option overall for key combinations * keys3 * keys4 * copy * paste
 3. Wait actions: 3.1. Wait until an image appears on the screen This can used
 when you are waiting for a window to finish loading completely and you don't
 know exactly how long that would take. ```python chain( dict(click="demo/
 notepad.jpg"), dict(waituntil="demo/notepad_opened.jpg", wait=1), dict
```

### Comparing `AutoMonkey-0.1.5/README.md` & `AutoMonkey-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,323 +1,323 @@
-[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4)
-[![Known Vulnerabilities](https://snyk.io/test/github/MihailCosmin/AutoMonkey/badge.svg)](https://snyk.io/test/github/MihailCosmin/AutoMonkey)
-[![HitCount](https://hits.dwyl.com/MihailCosmin/AutoMonkey.svg?style=flat-square&show=unique)](http://hits.dwyl.com/MihailCosmin/AutoMonkey)
-[![build](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml/badge.svg)](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml)
-[![Code Climate](https://codeclimate.com/github/MihailCosmin/AutoMonkey/badges/gpa.svg)](https://codeclimate.com/github/MihailCosmin/AutoMonkey)
-
-# AutoMonkey
-<img alt="AutoMonkey" src="https://github.com/MihailCosmin/AutoMonkey/raw/06181954fa23605583d61843226f5f3997157435/img/monkey.ico" width="100px" height="100px"/>
-
-Python Automation using Mouse and Keyboard, for the masses
-
-# Installation
-
-1. From <a href="https://pypi.org/project/AutoMonkey/">pypi</a>:
-
-```
-pip install AutoMonkey
-```
-
-2. From <a href="https://github.com/MihailCosmin/AutoMonkey">github</a>:
-
-```
-pip install git+https://github.com/MihailCosmin/AutoMonkey
-```
-
-# Dependencies
-#### Automonkey is based on:
-- <a href="https://github.com/asweigart/pyautogui">pyautogui</a>
-
-#### Other dependencies:
-- PyScreeze
-- pyperclip
-- clipboard
-- keyboard
-- screeninfo
-- pywin32
-- pillow
-- opencv-python
-- numpy
-- pytesseract
-
-# Usage
-Main function to be used is "chain"  
-
-This will allow you to "chain" together most of the other functions of automonkey.  
-Which in turn will enable you to create sequences of mouse and/or keyboard actions in order to automate any given task.
-
-A step can have this structure:
-
-```python
-
-dict(
-    <action> = <target>,  # action can be any of the automonkey functions, target on which the action will be performed
-    wait = 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
-    skip = False,  # if True, will skip this step
-    confidence = 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
-    v_offset = 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
-    h_offset = 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
-    offset = 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
-    monitor = 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
-)
-
-or 
-
-{
-    "<action>": "<target>",  # action can be any of the automonkey functions, target on which the action will be performed
-    "wait": 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
-    "skip": False,  # if True, will skip this step
-    "confidence": 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
-    "v_offset": 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
-    "h_offset": 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
-    "offset": 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
-    "monitor": 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
-}
-```
-
-1. You can connect multiple mouse actions together by using the "chain" function. Just by doing this you can generally automate most of the tasks you would do on a daily basis.
-
-    There are 2 main ways to click, either by giving the coordinates of the position where to click or by giving the filename of the image you want to click on
-
-    1.1. Clicking by coordinates
-        
-    
-    1.1.1. In order to find the coordinates of a position on the screen you can use the "track_mouse" function or the PositionTracker class
-
-    ```python
-        from automonkey import track_mouse
-        track_mouse()
-    ```
-
-    <img alt="track_mouse" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/track_mouse.gif" width="416px" height="304px"/>
-
-
-    ```python
-        from automonkey import PositionTracker
-        tracker = PositionTracker()
-        tracker.start()
-    ```
-
-    <img alt="PositionTracker" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/PositionTracker.gif" width="918px" height="574px"/>
-
-    1.2.1. Now that you have the coordinates of the position you want to click on, you can use the "chain" function to click on it
-
-
-    ```python
-        from automonkey import chain
-        chain(  
-            dict(click=(780, 1175), wait=1),  
-            dict(click=(444, 194), wait=1),  
-            dict(click=(1892, 110), wait=1),  
-            debug=True  
-        )
-    ```
-
-    <img alt="click" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click.gif" width="960px" height="576px"/>
-
-    1.2. Clicking by image
-
-    1.2.1. To click on an image you first need to make a screenshot of the area you want to click on and save it somewhere on your computer.
-        For this you can use any screenshot tool you want, or you could use monkeyshot: https://github.com/MihailCosmin/monkeyshot
-        For example you can make a screenshot of the Edge icon from your toolbar, then we can click on it by using the "chain" function.
-
-    <img alt="edge_toolbar" src="https://github.com/MihailCosmin/AutoMonkey/raw/25eaed263793bf548d42f616e241f435baa9d719/demo/edge_toolbar.jpg" width="33px" height="33px"/>
-
-    1.2.2. Now that we have the image we want to click on, we can use the "chain" function to click on it
-
-    ```python
-        chain(
-            dict(click="demo/edge_toolbar.jpg"),
-            dict(click="demo/google_create_account", wait=1),
-            dict(click="demo/personal_use", wait=1),
-            debug=True
-        )
-    ```
-
-    <img alt="click_image" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click_image.gif" width="918px" height="600px"/>
-
-    1.3. All mouse actions:
-
-        * click
-        * rightclick
-        * leftclick
-        * doubleclick
-        * tripleclick
-        * scrollup
-        * scrolldown
-        * scrollleft
-        * scrollright
-
-2. You can also connect multiple keyboard actions together by using the "chain" function.
-
-    2.1. Write text - This doesn't work well with non-english character. For this you can use the "pastetext" function.
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg"),
-            dict(write="Hello World!"),
-            debug=True
-        )
-    ```
-
-    <img alt="write" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/write.gif" width="918px" height="600px"/>
-
-    2.2. Paste text - This works well with non-english characters
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg"),
-            dict(pastetext="Straße"),
-            debug=True
-        )
-    ```
-
-    2.3. Key combinations
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(keys2="ctrl+a", wait=1),
-            dict(keys2="ctrl+x", wait=1),
-            dict(keys2="alt+f4", wait=1),  # close notepad
-            debug=True
-        )
-    ```
-
-    <img alt="keys" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/keys.gif" width="918px" height="600px"/>
-
-    2.4. All key actions:
-
-        * write
-        * pastetext
-        * keys
-        * keys2 - best option overall for key combinations
-        * keys3
-        * keys4
-        * copy
-        * paste
-
-3. Wait actions:
-
-    3.1. Wait until an image appears on the screen
-    This can used when you are waiting for a window to finish loading completely and you don't know exactly how long that would take.
-
-    ```python
-        chain(
-            dict(click="demo/notepad.jpg"),
-            dict(waituntil="demo/notepad_opened.jpg", wait=1),
-            dict(write="Hello World!", wait=1),
-            debug=True
-        )
-    ```
-
-    3.2. Wait while an image is on the screen
-
-4. App (window) actions:
-
-    4.1. Open an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(waituntil="demo/notepad_opened.jpg", wait=1),
-            dict(write="Hello World!", wait=1),
-            debug=True
-        )
-    ```
-
-    4.2. Close an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(close="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.3. Minimize an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(minimize="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.4. Maximize an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(maximize="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.5. Restore an app
-
-    ```python
-        chain(
-            dict(open_app="notepad++.exe", wait=1),
-            dict(write="Hello World!", wait=1),
-            dict(minimize="Notepad", wait=1),
-            dict(restore="Notepad", wait=1),
-            debug=True
-        )
-    ```
-
-    4.6. All app actions:
-
-        * open_app
-        * close
-        * startfile
-        * focus
-        * minimize
-        * maximize
-        * restore
-        * msoffice_replace
-        * copy_from
-        * copy_from_to
-
-5. Image actions
-
-    5.1 count_img. With this function you can count how many times one image appears on the screen.
-
-    ```python
-        chain(
-            dict(count_img="demo/M.jpg", wait=1),  # The result will be copied to the clipboard
-            dict(open_app="notepad++.exe", wait=1),
-            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
-            debug=True
-        )
-    ```
-
-    5.2. get_text_from_region
-
-    ```python
-        chain(
-            dict(get_text_from_region=((136, 121), (189, 140)), wait=1),  # The text will be copied to the clipboard
-            dict(open_app="notepad++.exe", wait=1),
-            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
-            debug=True
-        )
-    ```
-
-# Roadmap
-1. Check if possible to add <a href="https://github.com/pywinauto/pywinauto">pyautowin</a> functionality
-
-# Frequently Asked Questions:
-
-1. I made an image but it doesn't click on it.
-
-    A: Make sure you have not changed resolution of your screen or the theme (dark/light) of the window.
-
-
-2. Keys combination using "keys" function doesn't work.
-
-    A: Try other keys functions. Preferably "keys2". Other options "keys3", "keys4".
+[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4)
+[![](https://snyk.io/test/github/MihailCosmin/AutoMonkey/badge.svg)](https://snyk.io/test/github/MihailCosmin/AutoMonkey)
+[![HitCount](https://hits.dwyl.com/MihailCosmin/AutoMonkey.svg?style=flat-square&show=unique)](http://hits.dwyl.com/MihailCosmin/AutoMonkey)
+[![build](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml/badge.svg)](https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-package.yml)
+[![Code Climate](https://codeclimate.com/github/MihailCosmin/AutoMonkey/badges/gpa.svg)](https://codeclimate.com/github/MihailCosmin/AutoMonkey)
+
+# AutoMonkey
+<img alt="AutoMonkey" src="https://github.com/MihailCosmin/AutoMonkey/raw/06181954fa23605583d61843226f5f3997157435/img/monkey.ico" width="100px" height="100px"/>
+
+Python Automation using Mouse and Keyboard, for the masses
+
+# Installation
+
+1. From <a href="https://pypi.org/project/AutoMonkey/">pypi</a>:
+
+```
+pip install AutoMonkey
+```
+
+2. From <a href="https://github.com/MihailCosmin/AutoMonkey">github</a>:
+
+```
+pip install git+https://github.com/MihailCosmin/AutoMonkey
+```
+
+# Dependencies
+#### Automonkey is based on:
+- <a href="https://github.com/asweigart/pyautogui">pyautogui</a>
+
+#### Other dependencies:
+- PyScreeze
+- pyperclip
+- clipboard
+- keyboard
+- screeninfo
+- pywin32
+- pillow
+- opencv-python
+- numpy
+- pytesseract
+
+# Usage
+Main function to be used is "chain"  
+
+This will allow you to "chain" together most of the other functions of automonkey.  
+Which in turn will enable you to create sequences of mouse and/or keyboard actions in order to automate any given task.
+
+A step can have this structure:
+
+```python
+
+dict(
+    <action> = <target>,  # action can be any of the automonkey functions, target on which the action will be performed
+    wait = 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
+    skip = False,  # if True, will skip this step
+    confidence = 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
+    v_offset = 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
+    h_offset = 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
+    offset = 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
+    monitor = 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
+)
+
+or 
+
+{
+    "<action>": "<target>",  # action can be any of the automonkey functions, target on which the action will be performed
+    "wait": 1,  # wait is an optional parameter, which will wait for the given amount of seconds before executing the next step
+    "skip": False,  # if True, will skip this step
+    "confidence": 0.9, # confidence is an optional parameter, Used only for actions on images. Confidence on locating the image.
+    "v_offset": 0,  # v_offset is an optional parameter, Used only for actions on images. Vertical offset from the center of the image.
+    "h_offset": 0,  # h_offset is an optional parameter, Used only for actions on images. Horizontal offset from the center of the image.
+    "offset": 0, # offset is an optional parameter, Used only for actions on images. Offset from the center of the image.
+    "monitor": 0,  # monitor is an optional parameter, Used only for actions on images. Monitor on which to search for the image.
+}
+```
+
+1. You can connect multiple mouse actions together by using the "chain" function. Just by doing this you can generally automate most of the tasks you would do on a daily basis.
+
+    There are 2 main ways to click, either by giving the coordinates of the position where to click or by giving the filename of the image you want to click on
+
+    1.1. Clicking by coordinates
+        
+    
+    1.1.1. In order to find the coordinates of a position on the screen you can use the "track_mouse" function or the PositionTracker class
+
+    ```python
+        from automonkey import track_mouse
+        track_mouse()
+    ```
+
+    <img alt="track_mouse" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/track_mouse.gif" width="416px" height="304px"/>
+
+
+    ```python
+        from automonkey import PositionTracker
+        tracker = PositionTracker()
+        tracker.start()
+    ```
+
+    <img alt="PositionTracker" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/PositionTracker.gif" width="918px" height="574px"/>
+
+    1.2.1. Now that you have the coordinates of the position you want to click on, you can use the "chain" function to click on it
+
+
+    ```python
+        from automonkey import chain
+        chain(  
+            dict(click=(780, 1175), wait=1),  
+            dict(click=(444, 194), wait=1),  
+            dict(click=(1892, 110), wait=1),  
+            debug=True  
+        )
+    ```
+
+    <img alt="click" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click.gif" width="960px" height="576px"/>
+
+    1.2. Clicking by image
+
+    1.2.1. To click on an image you first need to make a screenshot of the area you want to click on and save it somewhere on your computer.
+        For this you can use any screenshot tool you want, or you could use monkeyshot: https://github.com/MihailCosmin/monkeyshot
+        For example you can make a screenshot of the Edge icon from your toolbar, then we can click on it by using the "chain" function.
+
+    <img alt="edge_toolbar" src="https://github.com/MihailCosmin/AutoMonkey/raw/25eaed263793bf548d42f616e241f435baa9d719/demo/edge_toolbar.jpg" width="33px" height="33px"/>
+
+    1.2.2. Now that we have the image we want to click on, we can use the "chain" function to click on it
+
+    ```python
+        chain(
+            dict(click="demo/edge_toolbar.jpg"),
+            dict(click="demo/google_create_account", wait=1),
+            dict(click="demo/personal_use", wait=1),
+            debug=True
+        )
+    ```
+
+    <img alt="click_image" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/click_image.gif" width="918px" height="600px"/>
+
+    1.3. All mouse actions:
+
+        * click
+        * rightclick
+        * leftclick
+        * doubleclick
+        * tripleclick
+        * scrollup
+        * scrolldown
+        * scrollleft
+        * scrollright
+
+2. You can also connect multiple keyboard actions together by using the "chain" function.
+
+    2.1. Write text - This doesn't work well with non-english character. For this you can use the "pastetext" function.
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg"),
+            dict(write="Hello World!"),
+            debug=True
+        )
+    ```
+
+    <img alt="write" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/write.gif" width="918px" height="600px"/>
+
+    2.2. Paste text - This works well with non-english characters
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg"),
+            dict(pastetext="Straße"),
+            debug=True
+        )
+    ```
+
+    2.3. Key combinations
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(keys2="ctrl+a", wait=1),
+            dict(keys2="ctrl+x", wait=1),
+            dict(keys2="alt+f4", wait=1),  # close notepad
+            debug=True
+        )
+    ```
+
+    <img alt="keys" src="https://github.com/MihailCosmin/AutoMonkey/raw/1fa19ba4517875d00c08cf320e628669d60714dc/demo/keys.gif" width="918px" height="600px"/>
+
+    2.4. All key actions:
+
+        * write
+        * pastetext
+        * keys
+        * keys2 - best option overall for key combinations
+        * keys3
+        * keys4
+        * copy
+        * paste
+
+3. Wait actions:
+
+    3.1. Wait until an image appears on the screen
+    This can used when you are waiting for a window to finish loading completely and you don't know exactly how long that would take.
+
+    ```python
+        chain(
+            dict(click="demo/notepad.jpg"),
+            dict(waituntil="demo/notepad_opened.jpg", wait=1),
+            dict(write="Hello World!", wait=1),
+            debug=True
+        )
+    ```
+
+    3.2. Wait while an image is on the screen
+
+4. App (window) actions:
+
+    4.1. Open an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(waituntil="demo/notepad_opened.jpg", wait=1),
+            dict(write="Hello World!", wait=1),
+            debug=True
+        )
+    ```
+
+    4.2. Close an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(close="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.3. Minimize an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(minimize="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.4. Maximize an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(maximize="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.5. Restore an app
+
+    ```python
+        chain(
+            dict(open_app="notepad++.exe", wait=1),
+            dict(write="Hello World!", wait=1),
+            dict(minimize="Notepad", wait=1),
+            dict(restore="Notepad", wait=1),
+            debug=True
+        )
+    ```
+
+    4.6. All app actions:
+
+        * open_app
+        * close
+        * startfile
+        * focus
+        * minimize
+        * maximize
+        * restore
+        * msoffice_replace
+        * copy_from
+        * copy_from_to
+
+5. Image actions
+
+    5.1 count_img. With this function you can count how many times one image appears on the screen.
+
+    ```python
+        chain(
+            dict(count_img="demo/M.jpg", wait=1),  # The result will be copied to the clipboard
+            dict(open_app="notepad++.exe", wait=1),
+            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
+            debug=True
+        )
+    ```
+
+    5.2. get_text_from_region
+
+    ```python
+        chain(
+            dict(get_text_from_region=((136, 121), (189, 140)), wait=1),  # The text will be copied to the clipboard
+            dict(open_app="notepad++.exe", wait=1),
+            dict(paste="", wait=1),  # with paste we can paste the text from the clipboard
+            debug=True
+        )
+    ```
+
+# Roadmap
+1. Check if possible to add <a href="https://github.com/pywinauto/pywinauto">pyautowin</a> functionality
+
+# Frequently Asked Questions:
+
+1. I made an image but it doesn't click on it.
+
+    A: Make sure you have not changed resolution of your screen or the theme (dark/light) of the window.
+
+
+2. Keys combination using "keys" function doesn't work.
+
+    A: Try other keys functions. Preferably "keys2". Other options "keys3", "keys4".
```

#### html2text {}

```diff
@@ -1,82 +1,82 @@
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://
-www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4) [![Known
-Vulnerabilities](https://snyk.io/test/github/MihailCosmin/AutoMonkey/
-badge.svg)](https://snyk.io/test/github/MihailCosmin/AutoMonkey) [![HitCount]
-(https://hits.dwyl.com/MihailCosmin/AutoMonkey.svg?style=flat-
-square&show=unique)](http://hits.dwyl.com/MihailCosmin/AutoMonkey) [![build]
-(https://github.com/MihailCosmin/AutoMonkey/actions/workflows/python-
-package.yml/badge.svg)](https://github.com/MihailCosmin/AutoMonkey/actions/
-workflows/python-package.yml) [![Code Climate](https://codeclimate.com/github/
-MihailCosmin/AutoMonkey/badges/gpa.svg)](https://codeclimate.com/github/
-MihailCosmin/AutoMonkey) # AutoMonkey [AutoMonkey] Python Automation using
-Mouse and Keyboard, for the masses # Installation 1. From pypi: ``` pip install
-AutoMonkey ``` 2. From github: ``` pip install git+https://github.com/
-MihailCosmin/AutoMonkey ``` # Dependencies #### Automonkey is based on: -
-pyautogui #### Other dependencies: - PyScreeze - pyperclip - clipboard -
-keyboard - screeninfo - pywin32 - pillow - opencv-python - numpy - pytesseract
-# Usage Main function to be used is "chain" This will allow you to "chain"
-together most of the other functions of automonkey. Which in turn will enable
-you to create sequences of mouse and/or keyboard actions in order to automate
-any given task. A step can have this structure: ```python dict(  = , # action
-can be any of the automonkey functions, target on which the action will be
-performed wait = 1, # wait is an optional parameter, which will wait for the
-given amount of seconds before executing the next step skip = False, # if True,
-will skip this step confidence = 0.9, # confidence is an optional parameter,
-Used only for actions on images. Confidence on locating the image. v_offset =
-0, # v_offset is an optional parameter, Used only for actions on images.
-Vertical offset from the center of the image. h_offset = 0, # h_offset is an
-optional parameter, Used only for actions on images. Horizontal offset from the
-center of the image. offset = 0, # offset is an optional parameter, Used only
-for actions on images. Offset from the center of the image. monitor = 0, #
-monitor is an optional parameter, Used only for actions on images. Monitor on
-which to search for the image. ) or { "": "", # action can be any of the
-automonkey functions, target on which the action will be performed "wait": 1, #
-wait is an optional parameter, which will wait for the given amount of seconds
-before executing the next step "skip": False, # if True, will skip this step
-"confidence": 0.9, # confidence is an optional parameter, Used only for actions
-on images. Confidence on locating the image. "v_offset": 0, # v_offset is an
-optional parameter, Used only for actions on images. Vertical offset from the
-center of the image. "h_offset": 0, # h_offset is an optional parameter, Used
-only for actions on images. Horizontal offset from the center of the image.
-"offset": 0, # offset is an optional parameter, Used only for actions on
-images. Offset from the center of the image. "monitor": 0, # monitor is an
-optional parameter, Used only for actions on images. Monitor on which to search
-for the image. } ``` 1. You can connect multiple mouse actions together by
-using the "chain" function. Just by doing this you can generally automate most
-of the tasks you would do on a daily basis. There are 2 main ways to click,
-either by giving the coordinates of the position where to click or by giving
-the filename of the image you want to click on 1.1. Clicking by coordinates
-1.1.1. In order to find the coordinates of a position on the screen you can use
-the "track_mouse" function or the PositionTracker class ```python from
-automonkey import track_mouse track_mouse() ``` [track_mouse] ```python from
-automonkey import PositionTracker tracker = PositionTracker() tracker.start()
-``` [PositionTracker] 1.2.1. Now that you have the coordinates of the position
-you want to click on, you can use the "chain" function to click on it ```python
-from automonkey import chain chain( dict(click=(780, 1175), wait=1), dict
-(click=(444, 194), wait=1), dict(click=(1892, 110), wait=1), debug=True ) ```
-[click] 1.2. Clicking by image 1.2.1. To click on an image you first need to
-make a screenshot of the area you want to click on and save it somewhere on
-your computer. For this you can use any screenshot tool you want, or you could
-use monkeyshot: https://github.com/MihailCosmin/monkeyshot For example you can
-make a screenshot of the Edge icon from your toolbar, then we can click on it
-by using the "chain" function. [edge_toolbar] 1.2.2. Now that we have the image
-we want to click on, we can use the "chain" function to click on it ```python
-chain( dict(click="demo/edge_toolbar.jpg"), dict(click="demo/
-google_create_account", wait=1), dict(click="demo/personal_use", wait=1),
-debug=True ) ``` [click_image] 1.3. All mouse actions: * click * rightclick *
-leftclick * doubleclick * tripleclick * scrollup * scrolldown * scrollleft *
-scrollright 2. You can also connect multiple keyboard actions together by using
-the "chain" function. 2.1. Write text - This doesn't work well with non-english
-character. For this you can use the "pastetext" function. ```python chain( dict
-(click="demo/notepad.jpg"), dict(write="Hello World!"), debug=True ) ```
-[write] 2.2. Paste text - This works well with non-english characters ```python
-chain( dict(click="demo/notepad.jpg"), dict(pastetext="StraÃe"), debug=True )
-``` 2.3. Key combinations ```python chain( dict(click="demo/notepad.jpg",
-wait=1), dict(write="Hello World!", wait=1), dict(keys2="ctrl+a", wait=1), dict
+www.paypal.com/donate/?hosted_button_id=5Q6TUMXS2QJW4) [![](https://snyk.io/
+test/github/MihailCosmin/AutoMonkey/badge.svg)](https://snyk.io/test/github/
+MihailCosmin/AutoMonkey) [![HitCount](https://hits.dwyl.com/MihailCosmin/
+AutoMonkey.svg?style=flat-square&show=unique)](http://hits.dwyl.com/
+MihailCosmin/AutoMonkey) [![build](https://github.com/MihailCosmin/AutoMonkey/
+actions/workflows/python-package.yml/badge.svg)](https://github.com/
+MihailCosmin/AutoMonkey/actions/workflows/python-package.yml) [![Code Climate]
+(https://codeclimate.com/github/MihailCosmin/AutoMonkey/badges/gpa.svg)](https:
+//codeclimate.com/github/MihailCosmin/AutoMonkey) # AutoMonkey [AutoMonkey]
+Python Automation using Mouse and Keyboard, for the masses # Installation 1.
+From pypi: ``` pip install AutoMonkey ``` 2. From github: ``` pip install
+git+https://github.com/MihailCosmin/AutoMonkey ``` # Dependencies ####
+Automonkey is based on: - pyautogui #### Other dependencies: - PyScreeze -
+pyperclip - clipboard - keyboard - screeninfo - pywin32 - pillow - opencv-
+python - numpy - pytesseract # Usage Main function to be used is "chain" This
+will allow you to "chain" together most of the other functions of automonkey.
+Which in turn will enable you to create sequences of mouse and/or keyboard
+actions in order to automate any given task. A step can have this structure:
+```python dict(  = , # action can be any of the automonkey functions, target on
+which the action will be performed wait = 1, # wait is an optional parameter,
+which will wait for the given amount of seconds before executing the next step
+skip = False, # if True, will skip this step confidence = 0.9, # confidence is
+an optional parameter, Used only for actions on images. Confidence on locating
+the image. v_offset = 0, # v_offset is an optional parameter, Used only for
+actions on images. Vertical offset from the center of the image. h_offset = 0,
+# h_offset is an optional parameter, Used only for actions on images.
+Horizontal offset from the center of the image. offset = 0, # offset is an
+optional parameter, Used only for actions on images. Offset from the center of
+the image. monitor = 0, # monitor is an optional parameter, Used only for
+actions on images. Monitor on which to search for the image. ) or { "": "", #
+action can be any of the automonkey functions, target on which the action will
+be performed "wait": 1, # wait is an optional parameter, which will wait for
+the given amount of seconds before executing the next step "skip": False, # if
+True, will skip this step "confidence": 0.9, # confidence is an optional
+parameter, Used only for actions on images. Confidence on locating the image.
+"v_offset": 0, # v_offset is an optional parameter, Used only for actions on
+images. Vertical offset from the center of the image. "h_offset": 0, # h_offset
+is an optional parameter, Used only for actions on images. Horizontal offset
+from the center of the image. "offset": 0, # offset is an optional parameter,
+Used only for actions on images. Offset from the center of the image.
+"monitor": 0, # monitor is an optional parameter, Used only for actions on
+images. Monitor on which to search for the image. } ``` 1. You can connect
+multiple mouse actions together by using the "chain" function. Just by doing
+this you can generally automate most of the tasks you would do on a daily
+basis. There are 2 main ways to click, either by giving the coordinates of the
+position where to click or by giving the filename of the image you want to
+click on 1.1. Clicking by coordinates 1.1.1. In order to find the coordinates
+of a position on the screen you can use the "track_mouse" function or the
+PositionTracker class ```python from automonkey import track_mouse track_mouse
+() ``` [track_mouse] ```python from automonkey import PositionTracker tracker =
+PositionTracker() tracker.start() ``` [PositionTracker] 1.2.1. Now that you
+have the coordinates of the position you want to click on, you can use the
+"chain" function to click on it ```python from automonkey import chain chain
+( dict(click=(780, 1175), wait=1), dict(click=(444, 194), wait=1), dict(click=
+(1892, 110), wait=1), debug=True ) ``` [click] 1.2. Clicking by image 1.2.1. To
+click on an image you first need to make a screenshot of the area you want to
+click on and save it somewhere on your computer. For this you can use any
+screenshot tool you want, or you could use monkeyshot: https://github.com/
+MihailCosmin/monkeyshot For example you can make a screenshot of the Edge icon
+from your toolbar, then we can click on it by using the "chain" function.
+[edge_toolbar] 1.2.2. Now that we have the image we want to click on, we can
+use the "chain" function to click on it ```python chain( dict(click="demo/
+edge_toolbar.jpg"), dict(click="demo/google_create_account", wait=1), dict
+(click="demo/personal_use", wait=1), debug=True ) ``` [click_image] 1.3. All
+mouse actions: * click * rightclick * leftclick * doubleclick * tripleclick *
+scrollup * scrolldown * scrollleft * scrollright 2. You can also connect
+multiple keyboard actions together by using the "chain" function. 2.1. Write
+text - This doesn't work well with non-english character. For this you can use
+the "pastetext" function. ```python chain( dict(click="demo/notepad.jpg"), dict
+(write="Hello World!"), debug=True ) ``` [write] 2.2. Paste text - This works
+well with non-english characters ```python chain( dict(click="demo/
+notepad.jpg"), dict(pastetext="StraÃe"), debug=True ) ``` 2.3. Key
+combinations ```python chain( dict(click="demo/notepad.jpg", wait=1), dict
+(write="Hello World!", wait=1), dict(keys2="ctrl+a", wait=1), dict
 (keys2="ctrl+x", wait=1), dict(keys2="alt+f4", wait=1), # close notepad
 debug=True ) ``` [keys] 2.4. All key actions: * write * pastetext * keys *
 keys2 - best option overall for key combinations * keys3 * keys4 * copy * paste
 3. Wait actions: 3.1. Wait until an image appears on the screen This can used
 when you are waiting for a window to finish loading completely and you don't
 know exactly how long that would take. ```python chain( dict(click="demo/
 notepad.jpg"), dict(waituntil="demo/notepad_opened.jpg", wait=1), dict
```

### Comparing `AutoMonkey-0.1.5/README.rst` & `AutoMonkey-0.1.6/README.rst`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-============
-AutoMonkey
-============
-
-
-.. image:: https://img.shields.io/pypi/v/automonkey.svg
-        :target: https://pypi.python.org/pypi/automonkey
-
-.. image:: https://img.shields.io/travis/MihailCosmin/automonkey.svg
-        :target: https://travis-ci.com/MihailCosmin/automonkey
-
-.. image:: https://readthedocs.org/projects/automonkey/badge/?version=latest
-        :target: https://automonkey.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
-
-.. image:: https://pyup.io/repos/github/MihailCosmin/automonkey/shield.svg
-     :target: https://pyup.io/repos/github/MihailCosmin/automonkey/
-     :alt: Updates
-
-
-
-Python Automation using Mouse and Keyboard for the masses
-
-
-* Free software: GNU General Public License v3
-* Documentation: https://automonkey.readthedocs.io.
-
-
-Features
---------
-
-* TODO
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+============
+AutoMonkey
+============
+
+
+.. image:: https://img.shields.io/pypi/v/automonkey.svg
+        :target: https://pypi.python.org/pypi/automonkey
+
+.. image:: https://img.shields.io/travis/MihailCosmin/automonkey.svg
+        :target: https://travis-ci.com/MihailCosmin/automonkey
+
+.. image:: https://readthedocs.org/projects/automonkey/badge/?version=latest
+        :target: https://automonkey.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+
+.. image:: https://pyup.io/repos/github/MihailCosmin/automonkey/shield.svg
+     :target: https://pyup.io/repos/github/MihailCosmin/automonkey/
+     :alt: Updates
+
+
+
+Python Automation using Mouse and Keyboard for the masses
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://automonkey.readthedocs.io.
+
+
+Features
+--------
+
+* TODO
+
+Credits
+-------
+
+This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `AutoMonkey-0.1.5/automonkey/automonkey.py` & `AutoMonkey-0.1.6/automonkey/automonkey.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,234 +1,242 @@
-"""Python Automation using Mouse and Keyboard, for the masses
-"""
-from time import sleep
-from sys import exit as end
-
-from os import startfile  # It is used
-
-from clipboard import paste
-
-from pyautogui import click  # It is used
-from pyautogui import write  # It is used
-from pyautogui import moveTo  # It is used
-from pyautogui import mouseUp  # It is used
-from pyautogui import confirm
-from pyautogui import mouseDown  # It is used
-from pyautogui import press as keys  # this normally is to be used for same key left, left, left
-from pyautogui import hotkey as keys2  # this is best solution, pass list to be unpacked with *list
-from pyautogui import locateOnScreen
-from pyautogui import scroll as scrollup  # It is used
-from pyautogui import hscroll as scrollright  # It is used
-from pyautogui import leftClick as leftclick  # It is used
-from pyautogui import rightClick as rightclick  # It is used
-from pyautogui import middleClick as middleclick  # It is used
-from pyautogui import doubleClick as doubleclick  # It is used
-from pyautogui import tripleClick as tripleclick  # It is used
-from keyboard import send as keys3  # works mostly on windows - TODO: Check difference to below
-from keyboard import press_and_release as keys4  # works mostly on windows
-
-from screeninfo import get_monitors
-
-from .constants import MOUSE_ACTIONS
-from .constants import WAIT_ACTIONS
-from .constants import KEYBOARD_ACTIONS
-from .constants import APPS_ACTIONS
-from .constants import IMG_ACTIONS
-from .constants import COMMON_APPS
-
-from .exceptions import AutoMonkeyNoAction
-from .exceptions import AutoMonkeyNoTarget
-
-from .mouse_tracker import track_mouse
-from .mouse_tracker import PositionTracker
-
-from .app_funcs import open_app
-from .app_funcs import minimize
-from .app_funcs import maximize
-from .app_funcs import close
-from .app_funcs import restore
-from .app_funcs import focus
-from .app_funcs import msoffice_replace
-from .app_funcs import copy
-
-from .img_funcs import _add_ext
-from .img_funcs import is_on_screen
-from .img_funcs import get_center
-from .img_funcs import diagonal_point
-
-from .utils import waitwhile
-from .utils import waituntil
-from .utils import pastetext
-from .utils import copy_from
-from .utils import scrolldown
-from .utils import scrollleft
-from .utils import copy_from_to
-
-
-ALL_ACTIONS = MOUSE_ACTIONS + KEYBOARD_ACTIONS + WAIT_ACTIONS + APPS_ACTIONS + IMG_ACTIONS
-
-def _wait_for_target(target: any, skip: bool = False):
-    """Wait for a target to be available"""
-    slept = 0
-    while not is_on_screen(target) and not skip:
-        sleep(0.1)
-        slept += 0.1
-        if int(slept) == 30:  # For production make it 300
-            stop = confirm("Next target was not found for 5 minutes.\
-                           Would you like to continue or stop?",
-                           "Continue?",
-                           ["Continue", "Stop"])
-            if stop == "Stop":
-                end()
-
-
-def _prepare_step(raw_step: dict) -> dict:
-    """Transform the raw step into a step that can be used by the script
-
-    Args:
-        raw_step (dict): The raw step from the json file
-
-    Raises:
-        AutoMonkeyNoAction: If the action is not supported
-        AutoMonkeyNoTarget: If the target is not supported
-
-    Returns:
-        dict: The step that can be used by the script
-    """
-    step = dict(
-        action=None,
-        target=None,
-        skip=False,
-        wait=0,
-        confidence=0.9,
-        v_offset=0,
-        h_offset=0,
-        offset=None,
-        monitor=1,
-    )
-
-    for arg_pair in raw_step.items():
-        step["action"] = arg_pair[0] if arg_pair[0] in ALL_ACTIONS else step["action"]
-        step["target"] = arg_pair[1] if arg_pair[0] in ALL_ACTIONS else step["target"]
-        step["skip"] = bool(arg_pair[1]) if arg_pair[0] == 'skip' else step["skip"]
-        step["wait"] = float(arg_pair[1]) if arg_pair[0] == 'wait' else step["wait"]
-        step["confidence"] = float(arg_pair[1]) if arg_pair[0] == 'confidence' else step["confidence"]
-        step["v_offset"] = int(arg_pair[1]) if arg_pair[0] == 'v_offset' else step["v_offset"]
-        step["h_offset"] = int(arg_pair[1]) if arg_pair[0] == 'h_offset' else step["h_offset"]
-        step["offset"] = str(arg_pair[1]) if arg_pair[0] == 'offset' else step["offset"]
-        step["monitor"] = arg_pair[1] if arg_pair[0] == 'monitor' else step["monitor"]
-
-    if step["action"] not in ALL_ACTIONS:
-        raise AutoMonkeyNoAction(step["action"])
-
-    if step["target"] is None:
-        raise AutoMonkeyNoTarget(step["target"])
-    return step
-
-def __run_1(step: dict):
-    step["target"] = _add_ext(step["target"])
-    _wait_for_target(step["target"], step["skip"])
-
-    bullseye = locateOnScreen(step["target"], confidence=step["confidence"])
-    bullseye = get_center(bullseye)
-    bullseye = diagonal_point(bullseye, step["h_offset"], step["v_offset"])
-    if step["offset"] not in ("", None):
-        globals()["_offset_clicks"](bullseye, step["target"], step["offset"], step["action"])
-    else:
-        globals()[step["action"]](bullseye)
-
-def __run_2(step: dict):
-    if step["action"] in ("keys2", "msoffice_replace"):
-        globals()[step["action"]](*step["target"])
-    elif step["action"] == "paste":
-        pastetext(paste())
-    elif step["action"] == "open_app":
-        __run_3(step)
-    else:
-        globals()[step["action"]](step["target"])
-
-def __run_3(step: dict):
-    if step["target"].lower() in COMMON_APPS:
-        globals()[step["action"]](COMMON_APPS[step["target"].lower()])
-    else:
-        globals()[step["action"]](step["target"])
-
-def __monitors():
-    monitors = {}
-    for _, mon in enumerate(sorted([(mon.x, mon.y) for mon in get_monitors()], key=lambda tup: tup[0])):
-        monitors[_] = (mon[0], mon[1])
-    return monitors
-
-def __target_1(step: dict):
-    step["target"] = step["target"].split("+") if step["action"] in ("keys", "keys2") else step["target"]
-    return step
-
-def __target_2(step: dict):
-    monitors = __monitors()
-    try:
-        if step["action"] in ("keys", "keys2") and isinstance(step["target"], tuple):
-            step["target"] = (step["target"][0] + monitors[step["monitor"] - 1][0], step["target"][1]) if step["target"][0] < monitors[1][0] else step["target"]
-            return step
-    except IndexError:
-        pass
-    except KeyError:
-        pass
-    return step
-
-def __run_1_cond(step: dict):
-    return step["action"] in MOUSE_ACTIONS and not isinstance(step["target"], tuple) and not isinstance(step["target"], int)
-
-def __debug_1(debug: bool, step: dict):
-    if debug:
-        print(step)
-
-def chain(*steps: dict, debug=False):
-    """Chain together a series of automation steps
-
-    Args:
-        *steps (dict): Unlimitted number of automation steps as dictionaries.
-        Each automation step should be a dictionary with 1 or more pairs:
-            - First pair is the Action - Target pair. The only mandatory pair.
-              Example: dict(click: "image.jpg") or {"click": "image.jpg"}
-            - Next possible pairs are optional:
-                * skip (True/False) - optional. If True, the step will be skipped if the target is not found.
-                * wait - Seconds to wait after performing the action. Defaults to zero.
-                * confidence - optional. Used only for actions on images. Confidence on locating the image.
-                  Defaults to 0.9
-                * v_offset - optional. Vertical offset from the center of the target.
-                * h_offset - optional. Horizontal offset from the center of the target.
-                * offset - optional. Offset from the center of the target. Overrides v_offset and h_offset.
-                * monitor - optional. Monitor number to perform the action on. Defaults to 1.
-
-        Example of steps:
-            chain(
-                dict(write="this string", wait=0.5),
-                dict(write="this other string"),
-                dict(click="C:\\Folder1\\Folder2\\image.jpg", wait=2, confidence=0.8),
-                debug=True)
-
-        debug (bool, optional): Debug variable, if True will print each step. Defaults to False.
-
-        Notes:
-        1. To use the scroll functions you have to select the scrollable area first
-        2. Horizontal scroll (left, right) is not supported on Windows
-        3. write function cannot write special characters like German or Chinese characters.
-        4. startfile keeps the file opened only until the end of the chain.
-           If you want to keep the file opened you need to perform other operations on it.
-        5. When using startfile you are responsible for saving and closing the file.
-        6. For the app functions (start, close, minimize, maximize, restore, focus) you need to provide the title of the window.add()
-           You can also use regex to match the title.
-
-    """
-    for _ in steps:
-        step = _prepare_step(_)
-        __debug_1(debug, step)
-
-        step = __target_1(step)
-        step = __target_2(step)
-
-        if __run_1_cond(step):
-            __run_1(step)
-        else:
-            __run_2(step)
-
-        sleep(step["wait"])
+"""Python Automation using Mouse and Keyboard, for the masses
+"""
+from time import sleep
+from sys import exit as end
+
+from sys import platform
+
+if platform == "win32":
+    from os import startfile  # It is used
+elif platform == "linux":
+    from subprocess import call
+    def startfile(file):
+        call(["xdg-open", file])
+
+from clipboard import paste
+
+from pyautogui import click  # It is used
+from pyautogui import write  # It is used
+from pyautogui import moveTo  # It is used
+from pyautogui import mouseUp  # It is used
+from pyautogui import confirm
+from pyautogui import mouseDown  # It is used
+from pyautogui import press as keys  # this normally is to be used for same key left, left, left
+from pyautogui import hotkey as keys2  # this is best solution, pass list to be unpacked with *list
+from pyautogui import locateOnScreen
+from pyautogui import scroll as scrollup  # It is used
+from pyautogui import hscroll as scrollright  # It is used
+from pyautogui import leftClick as leftclick  # It is used
+from pyautogui import rightClick as rightclick  # It is used
+from pyautogui import middleClick as middleclick  # It is used
+from pyautogui import doubleClick as doubleclick  # It is used
+from pyautogui import tripleClick as tripleclick  # It is used
+from keyboard import send as keys3  # works mostly on windows - TODO: Check difference to below
+from keyboard import press_and_release as keys4  # works mostly on windows
+
+from screeninfo import get_monitors
+
+from .constants import MOUSE_ACTIONS
+from .constants import WAIT_ACTIONS
+from .constants import KEYBOARD_ACTIONS
+from .constants import APPS_ACTIONS
+from .constants import IMG_ACTIONS
+from .constants import COMMON_APPS
+
+from .exceptions import AutoMonkeyNoAction
+from .exceptions import AutoMonkeyNoTarget
+
+from .mouse_tracker import track_mouse
+from .mouse_tracker import PositionTracker
+
+if platform == "win32":
+    from .app_funcs import open_app
+    from .app_funcs import minimize
+    from .app_funcs import maximize
+    from .app_funcs import close
+    from .app_funcs import restore
+    from .app_funcs import focus
+    from .app_funcs import msoffice_replace
+    from .app_funcs import copy
+
+from .img_funcs import _add_ext
+from .img_funcs import is_on_screen
+from .img_funcs import get_center
+from .img_funcs import diagonal_point
+
+from .utils import waitwhile
+from .utils import waituntil
+from .utils import pastetext
+from .utils import copy_from
+from .utils import scrolldown
+from .utils import scrollleft
+from .utils import copy_from_to
+
+
+ALL_ACTIONS = MOUSE_ACTIONS + KEYBOARD_ACTIONS + WAIT_ACTIONS + APPS_ACTIONS + IMG_ACTIONS
+
+def _wait_for_target(target: any, skip: bool = False):
+    """Wait for a target to be available"""
+    slept = 0
+    while not is_on_screen(target) and not skip:
+        sleep(0.1)
+        slept += 0.1
+        if int(slept) == 30:  # For production make it 300
+            stop = confirm("Next target was not found for 5 minutes.\
+                           Would you like to continue or stop?",
+                           "Continue?",
+                           ["Continue", "Stop"])
+            if stop == "Stop":
+                end()
+
+
+def _prepare_step(raw_step: dict) -> dict:
+    """Transform the raw step into a step that can be used by the script
+
+    Args:
+        raw_step (dict): The raw step from the json file
+
+    Raises:
+        AutoMonkeyNoAction: If the action is not supported
+        AutoMonkeyNoTarget: If the target is not supported
+
+    Returns:
+        dict: The step that can be used by the script
+    """
+    step = dict(
+        action=None,
+        target=None,
+        skip=False,
+        wait=0,
+        confidence=0.9,
+        v_offset=0,
+        h_offset=0,
+        offset=None,
+        monitor=1,
+    )
+
+    for arg_pair in raw_step.items():
+        step["action"] = arg_pair[0] if arg_pair[0] in ALL_ACTIONS else step["action"]
+        step["target"] = arg_pair[1] if arg_pair[0] in ALL_ACTIONS else step["target"]
+        step["skip"] = bool(arg_pair[1]) if arg_pair[0] == 'skip' else step["skip"]
+        step["wait"] = float(arg_pair[1]) if arg_pair[0] == 'wait' else step["wait"]
+        step["confidence"] = float(arg_pair[1]) if arg_pair[0] == 'confidence' else step["confidence"]
+        step["v_offset"] = int(arg_pair[1]) if arg_pair[0] == 'v_offset' else step["v_offset"]
+        step["h_offset"] = int(arg_pair[1]) if arg_pair[0] == 'h_offset' else step["h_offset"]
+        step["offset"] = str(arg_pair[1]) if arg_pair[0] == 'offset' else step["offset"]
+        step["monitor"] = arg_pair[1] if arg_pair[0] == 'monitor' else step["monitor"]
+
+    if step["action"] not in ALL_ACTIONS:
+        raise AutoMonkeyNoAction(step["action"])
+
+    if step["target"] is None:
+        raise AutoMonkeyNoTarget(step["target"])
+    return step
+
+def __run_1(step: dict):
+    step["target"] = _add_ext(step["target"])
+    _wait_for_target(step["target"], step["skip"])
+
+    bullseye = locateOnScreen(step["target"], confidence=step["confidence"])
+    bullseye = get_center(bullseye)
+    bullseye = diagonal_point(bullseye, step["h_offset"], step["v_offset"])
+    if step["offset"] not in ("", None):
+        globals()["_offset_clicks"](bullseye, step["target"], step["offset"], step["action"])
+    else:
+        globals()[step["action"]](bullseye)
+
+def __run_2(step: dict):
+    if step["action"] in ("keys2", "msoffice_replace"):
+        globals()[step["action"]](*step["target"])
+    elif step["action"] == "paste":
+        pastetext(paste())
+    elif step["action"] == "open_app":
+        __run_3(step)
+    else:
+        globals()[step["action"]](step["target"])
+
+def __run_3(step: dict):
+    if step["target"].lower() in COMMON_APPS:
+        globals()[step["action"]](COMMON_APPS[step["target"].lower()])
+    else:
+        globals()[step["action"]](step["target"])
+
+def __monitors():
+    monitors = {}
+    for _, mon in enumerate(sorted([(mon.x, mon.y) for mon in get_monitors()], key=lambda tup: tup[0])):
+        monitors[_] = (mon[0], mon[1])
+    return monitors
+
+def __target_1(step: dict):
+    step["target"] = step["target"].split("+") if step["action"] in ("keys", "keys2") else step["target"]
+    return step
+
+def __target_2(step: dict):
+    monitors = __monitors()
+    try:
+        if step["action"] in ("keys", "keys2") and isinstance(step["target"], tuple):
+            step["target"] = (step["target"][0] + monitors[step["monitor"] - 1][0], step["target"][1]) if step["target"][0] < monitors[1][0] else step["target"]
+            return step
+    except IndexError:
+        pass
+    except KeyError:
+        pass
+    return step
+
+def __run_1_cond(step: dict):
+    return step["action"] in MOUSE_ACTIONS and not isinstance(step["target"], tuple) and not isinstance(step["target"], int)
+
+def __debug_1(debug: bool, step: dict):
+    if debug:
+        print(step)
+
+def chain(*steps: dict, debug=False):
+    """Chain together a series of automation steps
+
+    Args:
+        *steps (dict): Unlimitted number of automation steps as dictionaries.
+        Each automation step should be a dictionary with 1 or more pairs:
+            - First pair is the Action - Target pair. The only mandatory pair.
+              Example: dict(click: "image.jpg") or {"click": "image.jpg"}
+            - Next possible pairs are optional:
+                * skip (True/False) - optional. If True, the step will be skipped if the target is not found.
+                * wait - Seconds to wait after performing the action. Defaults to zero.
+                * confidence - optional. Used only for actions on images. Confidence on locating the image.
+                  Defaults to 0.9
+                * v_offset - optional. Vertical offset from the center of the target.
+                * h_offset - optional. Horizontal offset from the center of the target.
+                * offset - optional. Offset from the center of the target. Overrides v_offset and h_offset.
+                * monitor - optional. Monitor number to perform the action on. Defaults to 1.
+
+        Example of steps:
+            chain(
+                dict(write="this string", wait=0.5),
+                dict(write="this other string"),
+                dict(click="C:\\Folder1\\Folder2\\image.jpg", wait=2, confidence=0.8),
+                debug=True)
+
+        debug (bool, optional): Debug variable, if True will print each step. Defaults to False.
+
+        Notes:
+        1. To use the scroll functions you have to select the scrollable area first
+        2. Horizontal scroll (left, right) is not supported on Windows
+        3. write function cannot write special characters like German or Chinese characters.
+        4. startfile keeps the file opened only until the end of the chain.
+           If you want to keep the file opened you need to perform other operations on it.
+        5. When using startfile you are responsible for saving and closing the file.
+        6. For the app functions (start, close, minimize, maximize, restore, focus) you need to provide the title of the window.add()
+           You can also use regex to match the title.
+
+    """
+    for _ in steps:
+        step = _prepare_step(_)
+        __debug_1(debug, step)
+
+        step = __target_1(step)
+        step = __target_2(step)
+
+        if __run_1_cond(step):
+            __run_1(step)
+        else:
+            __run_2(step)
+
+        sleep(step["wait"])
```

### Comparing `AutoMonkey-0.1.5/automonkey/constants.py` & `AutoMonkey-0.1.6/automonkey/constants.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-IMG_EXT = (
-    ".png",
-    ".jpg",
-    ".jpeg",
-    ".tiff",
-    ".tif",
-    ".bmp",
-    ".gif",
-    ".pdf",
-    ".webp",
-    ".PNG",
-    ".JPG",
-    ".JPEG",
-    ".TIFF",
-    ".TIF",
-    ".BMP",
-    ".GIF",
-    ".PDF",
-    ".WEBP"
-)
-
-MOUSE_ACTIONS = (
-    "click",
-    "leftclick",
-    "rightclick",
-    "doubleclick",
-    "tripleclick",
-    "scrollup",
-    "scrolldown",
-    "scrollleft",
-    "scrollright",
-)
-
-WAIT_ACTIONS = (
-    "waitwhile",
-    "waituntil",
-)
-
-KEYBOARD_ACTIONS = (
-    "write",
-    "pastetext",
-    "keys",
-    "keys2",
-    "keys3",
-    "keys4",
-    "copy",
-    "paste",
-)
-
-APPS_ACTIONS = (
-    "close",
-    "focus",
-    "open_app",
-    "startfile",
-    "minimize",
-    "maximize",
-    "restore",
-    "copy_from",
-    "copy_from_to",
-    "msoffice_replace",
-)
-
-IMG_ACTIONS = (
-    "count_img",
-    "get_text_from_region",
-)
-
-COMMON_APPS = {
-    "edge": "msedge",
-    "msedge": "msedge",
-    "microsoft edge": "msedge",
-    "chrome": "chrome",
-    "google chrome": "chrome",
-    "firefox": "firefox",
-    "mozilla firefox": "firefox",
-    "notepad": "notepad",
-    "notepad++": "notepad++",
-    "excel": "excel",
-    "microsoft excel": "excel",
-    "word": "word",
-    "microsoft word": "word",
-    "powerpoint": "powerpoint",
-    "microsoft powerpoint": "powerpoint",
-    "outlook": "outlook",
-    "microsoft outlook": "outlook",
-    "onenote": "onenote",
-    "microsoft onenote": "onenote",
-    "vscode": "code",
-    "visual studio code": "code",
-    "explorer": "explorer",
-    "windows explorer": "explorer",
-    "files": "explorer",
-    "file explorer": "explorer",
-    "cmd": "cmd",
-    "command prompt": "cmd",
-    "terminal": "cmd",
-    "powershell": "powershell",
-    "power shell": "powershell",
+IMG_EXT = (
+    ".png",
+    ".jpg",
+    ".jpeg",
+    ".tiff",
+    ".tif",
+    ".bmp",
+    ".gif",
+    ".pdf",
+    ".webp",
+    ".PNG",
+    ".JPG",
+    ".JPEG",
+    ".TIFF",
+    ".TIF",
+    ".BMP",
+    ".GIF",
+    ".PDF",
+    ".WEBP"
+)
+
+MOUSE_ACTIONS = (
+    "click",
+    "leftclick",
+    "rightclick",
+    "doubleclick",
+    "tripleclick",
+    "scrollup",
+    "scrolldown",
+    "scrollleft",
+    "scrollright",
+)
+
+WAIT_ACTIONS = (
+    "waitwhile",
+    "waituntil",
+)
+
+KEYBOARD_ACTIONS = (
+    "write",
+    "pastetext",
+    "keys",
+    "keys2",
+    "keys3",
+    "keys4",
+    "copy",
+    "paste",
+)
+
+APPS_ACTIONS = (
+    "close",
+    "focus",
+    "open_app",
+    "startfile",
+    "minimize",
+    "maximize",
+    "restore",
+    "copy_from",
+    "copy_from_to",
+    "msoffice_replace",
+)
+
+IMG_ACTIONS = (
+    "count_img",
+    "get_text_from_region",
+)
+
+COMMON_APPS = {
+    "edge": "msedge",
+    "msedge": "msedge",
+    "microsoft edge": "msedge",
+    "chrome": "chrome",
+    "google chrome": "chrome",
+    "firefox": "firefox",
+    "mozilla firefox": "firefox",
+    "notepad": "notepad",
+    "notepad++": "notepad++",
+    "excel": "excel",
+    "microsoft excel": "excel",
+    "word": "word",
+    "microsoft word": "word",
+    "powerpoint": "powerpoint",
+    "microsoft powerpoint": "powerpoint",
+    "outlook": "outlook",
+    "microsoft outlook": "outlook",
+    "onenote": "onenote",
+    "microsoft onenote": "onenote",
+    "vscode": "code",
+    "visual studio code": "code",
+    "explorer": "explorer",
+    "windows explorer": "explorer",
+    "files": "explorer",
+    "file explorer": "explorer",
+    "cmd": "cmd",
+    "command prompt": "cmd",
+    "terminal": "cmd",
+    "powershell": "powershell",
+    "power shell": "powershell",
 }
```

### Comparing `AutoMonkey-0.1.5/automonkey/exceptions.py` & `AutoMonkey-0.1.6/automonkey/exceptions.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-class AutoMonkeyNoAction(Exception):
-    """
-    AutoMonkey chain function will raise this Exception if no valid action exists
-    in an automation step of the chain sequence.
-    """
-    def __init__(self, message):
-        super().__init__(f"The provided action is not supported: {message}")
-
-
-class AutoMonkeyNoTarget(Exception):
-    """
-    AutoMonkey chain function will raise this Exception if no valid target exists
-    in an automation step of the chain sequence.
-    """
-    def __init__(self, message):
+class AutoMonkeyNoAction(Exception):
+    """
+    AutoMonkey chain function will raise this Exception if no valid action exists
+    in an automation step of the chain sequence.
+    """
+    def __init__(self, message):
+        super().__init__(f"The provided action is not supported: {message}")
+
+
+class AutoMonkeyNoTarget(Exception):
+    """
+    AutoMonkey chain function will raise this Exception if no valid target exists
+    in an automation step of the chain sequence.
+    """
+    def __init__(self, message):
         super().__init__(f"The provided target is not supported: {message}")
```

### Comparing `AutoMonkey-0.1.5/automonkey/img_funcs.py` & `AutoMonkey-0.1.6/automonkey/img_funcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,299 +1,301 @@
-from os import remove
-from os.path import isfile
-
-from time import sleep
-
-from pyautogui import center
-from pyautogui import locateOnScreen
-
-from pyscreeze import Box
-from pytesseract import image_to_string
-
-from clipboard import copy as copy1
-from pyperclip import copy as copy2
-
-try:
-    from PIL import Image
-except ImportError:
-    import Image
-
-import cv2
-from cv2 import imread
-from numpy import where
-
-from pyautogui import screenshot
-
-from .constants import IMG_EXT
-
-def copy(text: str):
-    """Copy text to clipboard using two functions
-
-    Args:
-        text (str): text to be copied to clipboard
-    """
-    copy1(text)
-    copy2(text)
-
-def _add_ext(filename: str) -> str:
-    """Adds extension to an image filename if missing
-
-    Args:
-        filename (str): image filename (with or without extension)
-
-    Returns:
-        str: image filename with extension if was missing
-    """
-
-    for ext in IMG_EXT:
-        if isfile(f"{filename}{ext}"):
-            return f"{filename}{ext}"
-    return filename
-
-
-def is_on_screen(what: str) -> bool:
-    """Checks whether an image is found on screen
-    Args:
-        what (str): image to locate on screen
-    Returns:
-        bool: Returns True if image is found and False if not.
-    """
-
-    found = False
-    what = _add_ext(what)
-
-    if locateOnScreen(what, confidence=0.9) is not None:
-        found = True
-
-    return found
-
-
-def get_center(image: str) -> tuple:
-    """Find the center of an image on screen
-    Args:
-        image ([str]): image to be located
-    Returns:
-        [point]: Returns the center of the located image as a point or None
-    """
-
-    image = _add_ext(image)
-
-    try:
-        if not isinstance(image, Box):
-            return center(locateOnScreen(image, confidence=0.9))
-        return center(image)
-    except TypeError:
-        return None
-    except NameError:
-        return None
-
-
-def vertical_point(point, offset) -> tuple:
-    """Returns a PyAutoGUI point that is offset vertically
-    Args:
-        point (PyAutoGUI point): [A Tuple with an X and a Y]
-        offset (int): The offset. Can be positive or negative.
-                Positive = Above. Negative = Below
-    Returns:
-        [PyAutoGUI point]: The PyAutoGUI point offset vertically.
-    """
-    return point[0], point[1] - offset
-
-
-def horizontal_point(point, offset) -> tuple:
-    """Returns a PyAutoGUI point that is offset horizontally
-    Args:
-        point (PyAutoGUI point): [A Tuple with an X and a Y]
-        offset (int): The offset. Can be positive or negative.
-                Positive = Right. Negative = Left
-    Returns:
-        [PyAutoGUI point]: The PyAutoGUI point offset horizontally.
-    """
-    return point[0] + offset, point[1]
-
-
-def diagonal_point(point, x_point, y_point) -> tuple:
-    """Returns a PyAutoGUI point that is offset diagonally
-    Args:
-        point (PyAutoGUI point): [A Tuple with an X and a Y]
-        x_point (int): The horizontal offset. Can be positive or negative.
-                Positive = Right. Negative = Left
-        y_point (int): The vertical offset. Can be positive or negative.
-                Positive = Above. Negative = Below
-    Returns:
-        [PyAutoGUI point]: The PyAutoGUI point offset diagonally.
-    """
-    return point[0] + x_point, point[1] - y_point
-
-def get_img_height(image_file: str) -> int:
-    """Function that returns the height of an image.
-    Args:
-        image_file (path): path to an image file, including filename.
-    Returns:
-        int: Height of the image
-    """
-
-    image_file = _add_ext(image_file)
-
-    img = Image.open(image_file)
-    _, height = img.size
-
-    return height
-
-
-def get_img_width(image_file: str) -> int:
-    """Function that returns the width of an image.
-    Args:
-        image_file (path): path to an image file, including filename.
-    Returns:
-        int: Width of the image
-    """
-
-    image_file = _add_ext(image_file)
-
-    img = Image.open(image_file)
-    width, _ = img.size
-
-    return width
-
-def __transform_region_1(*args) -> tuple:
-    assert isinstance(args[0], tuple), "The argument must be a tuple of 4 integers: Left, Top, Width, Height"
-    if len(args[0]) == 4:
-        region = (args[0][0], args[0][1], args[0][2] - args[0][0], args[0][3] - args[0][1])
-    elif len(args[0]) == 2:
-        region = __transform_region_4(args)
-    else:
-        region = args[0]
-    return region
-
-# TODO: To have a function that can be called with different number and different types of arguments look into function overloading
-# https://stackoverflow.com/questions/6434482/python-function-overloading
-# This could be needed for:
-# 1. get_text_from_region
-# 2. copy_from_to
-
-def __transform_region_2(*args) -> tuple:
-    assert isinstance(args[0], tuple), "The first argument must be a tuple of 2 integers: X, Y coordinates of the top left corner"
-    assert isinstance(args[1], tuple), "The second argument must be a tuple of 2 integers: X, Y coordinates of the bottom right corner"
-    return (args[0][0], args[0][1], args[1][0] - args[0][0], args[1][1] - args[0][1])
-
-def __transform_region_3(*args) -> tuple:
-    assert isinstance(args[0], int), "The first argument must be an integer: X coordinate of the top left corner"
-    assert isinstance(args[1], int), "The second argument must be an integer: Y coordinate of the top left corner"
-    assert isinstance(args[2], int), "The third argument must be an integer: Width of the region"
-    assert isinstance(args[3], int), "The fourth argument must be an integer: Height of the region"
-    if args[2] > args[0] and args[3] > args[1]:
-        region = (args[0], args[1], args[2] - args[0], args[3] - args[1])
-    else:
-        region = (args[0], args[1], args[2], args[3])
-    return region
-
-def __transform_region_4(*args) -> tuple:
-    if args[0][1][1] > args[0][0][0] and args[0][1][1] > args[0][0][1]:
-        region = (args[0][0][0], args[0][0][1], args[0][1][0] - args[0][0][0], args[0][1][1] - args[0][0][1])
-    else:
-        region = (args[0][0][0], args[0][0][1], args[0][1][0], args[0][1][1])
-    return region
-
-def get_text_from_region(*args) -> str:
-    """Makes a screenshot of a screen region and performs OCR on it
-    Args:
-        Top left corner X, top left corner Y, bottom right corner X, bottom right corner Y
-        or
-        Top point (Tuple): (x, y) and Bottom point (Tuple): (x, y)
-        or
-        region (Tuple or PyAutoGUI region): (Left, Top, Width, Height)
-        or
-        Left (int), Top (int), Width (int), Height (int)
-    Returns:
-        str: The text from the region
-    """
-    if len(args) == 1:
-        region = __transform_region_1(args)
-    elif len(args) == 2:
-        region = __transform_region_2(args)
-    elif len(args) == 4:
-        region = __transform_region_3(args)
-
-    snap = screenshot(region=region)
-    snap.save("temp.jpg")
-    sleep(1)
-    img = imread('temp.jpg')
-
-    custom_config = r'--oem 3 --psm 6'
-    text = image_to_string(img, config=custom_config)
-    remove('temp.jpg')
-
-    copy(text)  # in order to make the text available in the clipboard
-    return text
-
-
-def count_img(needle: str, haystack: str = None) -> int:
-    """Counts how many times an image appears in a bigger image
-
-    Args:
-        needle (str): image filename to be counted
-        haystack (str): filename of image in which to search
-
-    Returns:
-        int: Count of occurrences of needle in the haystack
-    """
-
-    needle = _add_ext(needle)
-    if haystack:
-        haystack = _add_ext(haystack)
-        hay = imread(haystack)
-    else:
-        haystack = screenshot("temp.jpg")
-        hay = imread("temp.jpg")
-        remove("temp.jpg")
-
-    need = imread(needle)
-
-    res = cv2.cv2.matchTemplate(hay, need, cv2.cv2.TM_CCOEFF_NORMED)
-
-    threshold = .9  # 9 is more precise. 8 gives some false positives
-    loc = where(res >= threshold)
-
-    copy(len(loc[0]))  # in order to make the text available in the clipboard
-    return len(loc[0])
-
-
-def _offset_clicks(point: tuple, img: str, offset_value: str, click_type: str):
-    """Offset Clicks
-
-    Args:
-        point (tuple): PyAutoGUI Point as a (x, y) tuple
-        img (str): image path that was the source of the point
-        offset_value (str): Offset type:
-                                         - above
-                                         - bellow
-                                         - right
-                                         - left
-                                         - upper-left
-                                         - upper-right
-                                         - lower-left
-                                         - lower-right
-        click_type (str): click, rightClick, doubleClick, etc
-    """
-    __offset_clicks_1(point, img, offset_value, click_type)
-    __offset_clicks_2(point, img, offset_value, click_type)
-
-def __offset_clicks_1(point: tuple, img: str, offset_value: str, click_type: str):
-    if offset_value == "above":
-        globals()[click_type](vertical_point(point, get_img_height(img)))
-    if offset_value == "bellow":
-        globals()[click_type](vertical_point(point, 0 - get_img_height(img)))
-    if offset_value == "right":
-        globals()[click_type](horizontal_point(point, get_img_width(img)))
-    if offset_value == "left":
-        globals()[click_type](horizontal_point(point, 0 - get_img_width(img)))
-
-def __offset_clicks_2(point: tuple, img: str, offset_value: str, click_type: str):
-    if offset_value == "upper-left":
-        globals()[click_type](diagonal_point(point, 0 - get_img_width(img), get_img_height(img)))
-    if offset_value == "upper-right":
-        globals()[click_type](diagonal_point(point, get_img_width(img), get_img_height(img)))
-    if offset_value == "lower-left":
-        globals()[click_type](diagonal_point(point, 0 - get_img_width(img), 0 - get_img_height(img)))
-    if offset_value == "lower-right":
+from os import remove
+from os.path import isfile
+
+from time import sleep
+
+from pyautogui import center
+from pyautogui import locateOnScreen
+
+from pyscreeze import Box
+from pytesseract import image_to_string
+
+from clipboard import copy as copy1
+from pyperclip import copy as copy2
+
+try:
+    from PIL import Image
+except ImportError:
+    import Image
+
+import cv2
+from cv2 import imread
+from numpy import where
+
+from pyautogui import screenshot
+
+from .constants import IMG_EXT
+
+# TODO: Add mousedown, mouseup, drag, and drop functions
+
+def copy(text: str):
+    """Copy text to clipboard using two functions
+
+    Args:
+        text (str): text to be copied to clipboard
+    """
+    copy1(text)
+    copy2(text)
+
+def _add_ext(filename: str) -> str:
+    """Adds extension to an image filename if missing
+
+    Args:
+        filename (str): image filename (with or without extension)
+
+    Returns:
+        str: image filename with extension if was missing
+    """
+
+    for ext in IMG_EXT:
+        if isfile(f"{filename}{ext}"):
+            return f"{filename}{ext}"
+    return filename
+
+
+def is_on_screen(what: str) -> bool:
+    """Checks whether an image is found on screen
+    Args:
+        what (str): image to locate on screen
+    Returns:
+        bool: Returns True if image is found and False if not.
+    """
+
+    found = False
+    what = _add_ext(what)
+
+    if locateOnScreen(what, confidence=0.9) is not None:
+        found = True
+
+    return found
+
+
+def get_center(image: str) -> tuple:
+    """Find the center of an image on screen
+    Args:
+        image ([str]): image to be located
+    Returns:
+        [point]: Returns the center of the located image as a point or None
+    """
+
+    image = _add_ext(image)
+
+    try:
+        if not isinstance(image, Box):
+            return center(locateOnScreen(image, confidence=0.9))
+        return center(image)
+    except TypeError:
+        return None
+    except NameError:
+        return None
+
+
+def vertical_point(point, offset) -> tuple:
+    """Returns a PyAutoGUI point that is offset vertically
+    Args:
+        point (PyAutoGUI point): [A Tuple with an X and a Y]
+        offset (int): The offset. Can be positive or negative.
+                Positive = Above. Negative = Below
+    Returns:
+        [PyAutoGUI point]: The PyAutoGUI point offset vertically.
+    """
+    return point[0], point[1] - offset
+
+
+def horizontal_point(point, offset) -> tuple:
+    """Returns a PyAutoGUI point that is offset horizontally
+    Args:
+        point (PyAutoGUI point): [A Tuple with an X and a Y]
+        offset (int): The offset. Can be positive or negative.
+                Positive = Right. Negative = Left
+    Returns:
+        [PyAutoGUI point]: The PyAutoGUI point offset horizontally.
+    """
+    return point[0] + offset, point[1]
+
+
+def diagonal_point(point, x_point, y_point) -> tuple:
+    """Returns a PyAutoGUI point that is offset diagonally
+    Args:
+        point (PyAutoGUI point): [A Tuple with an X and a Y]
+        x_point (int): The horizontal offset. Can be positive or negative.
+                Positive = Right. Negative = Left
+        y_point (int): The vertical offset. Can be positive or negative.
+                Positive = Above. Negative = Below
+    Returns:
+        [PyAutoGUI point]: The PyAutoGUI point offset diagonally.
+    """
+    return point[0] + x_point, point[1] - y_point
+
+def get_img_height(image_file: str) -> int:
+    """Function that returns the height of an image.
+    Args:
+        image_file (path): path to an image file, including filename.
+    Returns:
+        int: Height of the image
+    """
+
+    image_file = _add_ext(image_file)
+
+    img = Image.open(image_file)
+    _, height = img.size
+
+    return height
+
+
+def get_img_width(image_file: str) -> int:
+    """Function that returns the width of an image.
+    Args:
+        image_file (path): path to an image file, including filename.
+    Returns:
+        int: Width of the image
+    """
+
+    image_file = _add_ext(image_file)
+
+    img = Image.open(image_file)
+    width, _ = img.size
+
+    return width
+
+def __transform_region_1(*args) -> tuple:
+    assert isinstance(args[0], tuple), "The argument must be a tuple of 4 integers: Left, Top, Width, Height"
+    if len(args[0]) == 4:
+        region = (args[0][0], args[0][1], args[0][2] - args[0][0], args[0][3] - args[0][1])
+    elif len(args[0]) == 2:
+        region = __transform_region_4(args)
+    else:
+        region = args[0]
+    return region
+
+# TODO: To have a function that can be called with different number and different types of arguments look into function overloading
+# https://stackoverflow.com/questions/6434482/python-function-overloading
+# This could be needed for:
+# 1. get_text_from_region
+# 2. copy_from_to
+
+def __transform_region_2(*args) -> tuple:
+    assert isinstance(args[0], tuple), "The first argument must be a tuple of 2 integers: X, Y coordinates of the top left corner"
+    assert isinstance(args[1], tuple), "The second argument must be a tuple of 2 integers: X, Y coordinates of the bottom right corner"
+    return (args[0][0], args[0][1], args[1][0] - args[0][0], args[1][1] - args[0][1])
+
+def __transform_region_3(*args) -> tuple:
+    assert isinstance(args[0], int), "The first argument must be an integer: X coordinate of the top left corner"
+    assert isinstance(args[1], int), "The second argument must be an integer: Y coordinate of the top left corner"
+    assert isinstance(args[2], int), "The third argument must be an integer: Width of the region"
+    assert isinstance(args[3], int), "The fourth argument must be an integer: Height of the region"
+    if args[2] > args[0] and args[3] > args[1]:
+        region = (args[0], args[1], args[2] - args[0], args[3] - args[1])
+    else:
+        region = (args[0], args[1], args[2], args[3])
+    return region
+
+def __transform_region_4(*args) -> tuple:
+    if args[0][1][1] > args[0][0][0] and args[0][1][1] > args[0][0][1]:
+        region = (args[0][0][0], args[0][0][1], args[0][1][0] - args[0][0][0], args[0][1][1] - args[0][0][1])
+    else:
+        region = (args[0][0][0], args[0][0][1], args[0][1][0], args[0][1][1])
+    return region
+
+def get_text_from_region(*args) -> str:
+    """Makes a screenshot of a screen region and performs OCR on it
+    Args:
+        Top left corner X, top left corner Y, bottom right corner X, bottom right corner Y
+        or
+        Top point (Tuple): (x, y) and Bottom point (Tuple): (x, y)
+        or
+        region (Tuple or PyAutoGUI region): (Left, Top, Width, Height)
+        or
+        Left (int), Top (int), Width (int), Height (int)
+    Returns:
+        str: The text from the region
+    """
+    if len(args) == 1:
+        region = __transform_region_1(args)
+    elif len(args) == 2:
+        region = __transform_region_2(args)
+    elif len(args) == 4:
+        region = __transform_region_3(args)
+
+    snap = screenshot(region=region)
+    snap.save("temp.jpg")
+    sleep(1)
+    img = imread('temp.jpg')
+
+    custom_config = r'--oem 3 --psm 6'
+    text = image_to_string(img, config=custom_config)
+    remove('temp.jpg')
+
+    copy(text)  # in order to make the text available in the clipboard
+    return text
+
+
+def count_img(needle: str, haystack: str = None) -> int:
+    """Counts how many times an image appears in a bigger image
+
+    Args:
+        needle (str): image filename to be counted
+        haystack (str): filename of image in which to search
+
+    Returns:
+        int: Count of occurrences of needle in the haystack
+    """
+
+    needle = _add_ext(needle)
+    if haystack:
+        haystack = _add_ext(haystack)
+        hay = imread(haystack)
+    else:
+        haystack = screenshot("temp.jpg")
+        hay = imread("temp.jpg")
+        remove("temp.jpg")
+
+    need = imread(needle)
+
+    res = cv2.cv2.matchTemplate(hay, need, cv2.cv2.TM_CCOEFF_NORMED)
+
+    threshold = .9  # 9 is more precise. 8 gives some false positives
+    loc = where(res >= threshold)
+
+    copy(len(loc[0]))  # in order to make the text available in the clipboard
+    return len(loc[0])
+
+
+def _offset_clicks(point: tuple, img: str, offset_value: str, click_type: str):
+    """Offset Clicks
+
+    Args:
+        point (tuple): PyAutoGUI Point as a (x, y) tuple
+        img (str): image path that was the source of the point
+        offset_value (str): Offset type:
+                                         - above
+                                         - bellow
+                                         - right
+                                         - left
+                                         - upper-left
+                                         - upper-right
+                                         - lower-left
+                                         - lower-right
+        click_type (str): click, rightClick, doubleClick, etc
+    """
+    __offset_clicks_1(point, img, offset_value, click_type)
+    __offset_clicks_2(point, img, offset_value, click_type)
+
+def __offset_clicks_1(point: tuple, img: str, offset_value: str, click_type: str):
+    if offset_value == "above":
+        globals()[click_type](vertical_point(point, get_img_height(img)))
+    if offset_value == "bellow":
+        globals()[click_type](vertical_point(point, 0 - get_img_height(img)))
+    if offset_value == "right":
+        globals()[click_type](horizontal_point(point, get_img_width(img)))
+    if offset_value == "left":
+        globals()[click_type](horizontal_point(point, 0 - get_img_width(img)))
+
+def __offset_clicks_2(point: tuple, img: str, offset_value: str, click_type: str):
+    if offset_value == "upper-left":
+        globals()[click_type](diagonal_point(point, 0 - get_img_width(img), get_img_height(img)))
+    if offset_value == "upper-right":
+        globals()[click_type](diagonal_point(point, get_img_width(img), get_img_height(img)))
+    if offset_value == "lower-left":
+        globals()[click_type](diagonal_point(point, 0 - get_img_width(img), 0 - get_img_height(img)))
+    if offset_value == "lower-right":
         globals()[click_type](diagonal_point(point, get_img_width(img), 0 - get_img_height(img)))
```

### Comparing `AutoMonkey-0.1.5/automonkey/utils.py` & `AutoMonkey-0.1.6/automonkey/utils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-from time import sleep
-
-from clipboard import copy as copy1
-from pyperclip import copy as copy2
-
-from clipboard import paste
-
-from pyautogui import click
-from pyautogui import moveTo
-from pyautogui import mouseUp
-from pyautogui import mouseDown
-from pyautogui import scroll as scrollup
-from pyautogui import hscroll as scrollright
-from pyautogui import hotkey as keys2  # this is best solution, pass list to be unpacked with *list
-
-from .img_funcs import is_on_screen
-
-def copy(text: str):
-    """Copy text to clipboard using two functions
-
-    Args:
-        text (str): text to be copied to clipboard
-    """
-    copy1(text)
-    copy2(text)
-
-
-def clear_clipboard():
-    """Try to clear the clipboard by copying an empty string
-    Might not work in all cases, for example: in environments
-    with shared/multiple clipboards.
-    """
-    for _ in range(0, 10):
-        copy('')
-
-
-def copy_from_to(*args) -> str:
-    """This function will copy text from one point to another.
-    Args:
-        point1 (PyAutoGUI point): PyAutoGUI start point (from)
-        point2 (PyAutoGUI point): PyAutoGUI end point (to)
-
-    Returns:
-        str: The copied text
-    """
-    if len(args) == 1:
-        assert isinstance(args[0][0], tuple), "The argument must be a tuple. First point tuple"
-        assert isinstance(args[0][1], tuple), "The argument must be a tuple. Second point tuple"
-        assert isinstance(args[0][0][0], int), "The argument must be an integer. First point X"
-        assert isinstance(args[0][0][1], int), "The argument must be an integer. First point Y"
-        assert isinstance(args[0][1][0], int), "The argument must be an integer. Second point X"
-        assert isinstance(args[0][1][1], int), "The argument must be an integer. Second point Y"
-        point1 = (args[0][0][0], args[0][0][1])
-        point2 = (args[0][1][0], args[0][1][1])
-    elif len(args) == 2:
-        assert isinstance(args[0], tuple), "The argument must be a tuple. First point tuple"
-        assert isinstance(args[1], tuple), "The argument must be a tuple. Second point tuple"
-        assert isinstance(args[0][0], int), "The argument must be an integer. First point X"
-        assert isinstance(args[0][1], int), "The argument must be an integer. First point Y"
-        assert isinstance(args[1][0], int), "The argument must be an integer. Second point X"
-        assert isinstance(args[1][1], int), "The argument must be an integer. Second point Y"
-        point1 = args[0]
-        point2 = args[1]
-
-    mouseDown(point1)
-    moveTo(point2)
-    mouseUp()
-    clear_clipboard()
-
-    while str(paste()) == '':
-        keys2('ctrl', 'c')
-
-    copied = paste()
-    print(copied)
-    copy(copied)
-    return copied
-
-
-def copy_from(point) -> str:
-    """This function will copy text from one point to the end of line.
-    This function uses select all functionality (ctrl+a) and as such
-    it should be used only when you are sure ctrl+a will select only
-    the content you want.
-    Args:
-        point (PyAutoGUI point): PyAutoGUI start point (from)
-    Returns:
-        [string]: The copied text.
-    """
-
-    clear_clipboard()
-    click(point)
-    sleep(0.2)
-    keys2('ctrl', 'a')
-    sleep(0.2)
-
-    while str(paste()) == '':
-        keys2('ctrl', 'c')
-
-    copied = paste()
-    copy(copied)
-
-    return copied
-
-def pastetext(text: str):
-    """Copy the text and paste it in the applicable place
-    This type of text output can be used when write or type are not capable
-    of writting special characters. For example German or Chinese characters.
-    In those cases a simple solution would be to copy the text and just paste it in the
-    where needed.
-
-    Args:
-        text (str): text to be output
-    """
-
-    temp_clipboard = paste()
-    while paste() != text:
-        copy(text)
-    keys2('ctrl', 'v')
-    copy(temp_clipboard)
-
-
-def scrolldown(clicks: int):
-    """Scroll down a given number of clicks
-    Note: You have to select the scrollable area first
-
-    Args:
-        clicks (int): number of clicks
-    """
-    scrollup(-clicks)
-
-
-def scrollleft(clicks: int):
-    """Scroll left a given number of clicks
-    Note: You have to select the scrollable area first
-
-    Args:
-        clicks (int): number of clicks
-    """
-    scrollright(-clicks)
-
-
-def waitwhile(img: str):
-    """While an image is on screen wait
-    For example a loading window.
-
-    Args:
-        img (str): image location path + name
-    """
-
-    while is_on_screen(img):
-        sleep(0.1)
-
-
-def waituntil(img: str):
-    """Wait until an image appears on screen
-    For example wait for a software to start
-
-    Args:
-        img (str): image location path + name
-    """
-
-    while not is_on_screen(img):
-        sleep(0.1)
+from time import sleep
+
+from clipboard import copy as copy1
+from pyperclip import copy as copy2
+
+from clipboard import paste
+
+from pyautogui import click
+from pyautogui import moveTo
+from pyautogui import mouseUp
+from pyautogui import mouseDown
+from pyautogui import scroll as scrollup
+from pyautogui import hscroll as scrollright
+from pyautogui import hotkey as keys2  # this is best solution, pass list to be unpacked with *list
+
+from .img_funcs import is_on_screen
+
+def copy(text: str):
+    """Copy text to clipboard using two functions
+
+    Args:
+        text (str): text to be copied to clipboard
+    """
+    copy1(text)
+    copy2(text)
+
+
+def clear_clipboard():
+    """Try to clear the clipboard by copying an empty string
+    Might not work in all cases, for example: in environments
+    with shared/multiple clipboards.
+    """
+    for _ in range(0, 10):
+        copy('')
+
+
+def copy_from_to(*args) -> str:
+    """This function will copy text from one point to another.
+    Args:
+        point1 (PyAutoGUI point): PyAutoGUI start point (from)
+        point2 (PyAutoGUI point): PyAutoGUI end point (to)
+
+    Returns:
+        str: The copied text
+    """
+    if len(args) == 1:
+        assert isinstance(args[0][0], tuple), "The argument must be a tuple. First point tuple"
+        assert isinstance(args[0][1], tuple), "The argument must be a tuple. Second point tuple"
+        assert isinstance(args[0][0][0], int), "The argument must be an integer. First point X"
+        assert isinstance(args[0][0][1], int), "The argument must be an integer. First point Y"
+        assert isinstance(args[0][1][0], int), "The argument must be an integer. Second point X"
+        assert isinstance(args[0][1][1], int), "The argument must be an integer. Second point Y"
+        point1 = (args[0][0][0], args[0][0][1])
+        point2 = (args[0][1][0], args[0][1][1])
+    elif len(args) == 2:
+        assert isinstance(args[0], tuple), "The argument must be a tuple. First point tuple"
+        assert isinstance(args[1], tuple), "The argument must be a tuple. Second point tuple"
+        assert isinstance(args[0][0], int), "The argument must be an integer. First point X"
+        assert isinstance(args[0][1], int), "The argument must be an integer. First point Y"
+        assert isinstance(args[1][0], int), "The argument must be an integer. Second point X"
+        assert isinstance(args[1][1], int), "The argument must be an integer. Second point Y"
+        point1 = args[0]
+        point2 = args[1]
+
+    mouseDown(point1)
+    moveTo(point2)
+    mouseUp()
+    clear_clipboard()
+
+    while str(paste()) == '':
+        keys2('ctrl', 'c')
+
+    copied = paste()
+    print(copied)
+    copy(copied)
+    return copied
+
+
+def copy_from(point) -> str:
+    """This function will copy text from one point to the end of line.
+    This function uses select all functionality (ctrl+a) and as such
+    it should be used only when you are sure ctrl+a will select only
+    the content you want.
+    Args:
+        point (PyAutoGUI point): PyAutoGUI start point (from)
+    Returns:
+        [string]: The copied text.
+    """
+
+    clear_clipboard()
+    click(point)
+    sleep(0.2)
+    keys2('ctrl', 'a')
+    sleep(0.2)
+
+    while str(paste()) == '':
+        keys2('ctrl', 'c')
+
+    copied = paste()
+    copy(copied)
+
+    return copied
+
+def pastetext(text: str):
+    """Copy the text and paste it in the applicable place
+    This type of text output can be used when write or type are not capable
+    of writting special characters. For example German or Chinese characters.
+    In those cases a simple solution would be to copy the text and just paste it in the
+    where needed.
+
+    Args:
+        text (str): text to be output
+    """
+
+    temp_clipboard = paste()
+    while paste() != text:
+        copy(text)
+    keys2('ctrl', 'v')
+    copy(temp_clipboard)
+
+
+def scrolldown(clicks: int):
+    """Scroll down a given number of clicks
+    Note: You have to select the scrollable area first
+
+    Args:
+        clicks (int): number of clicks
+    """
+    scrollup(-clicks)
+
+
+def scrollleft(clicks: int):
+    """Scroll left a given number of clicks
+    Note: You have to select the scrollable area first
+
+    Args:
+        clicks (int): number of clicks
+    """
+    scrollright(-clicks)
+
+
+def waitwhile(img: str):
+    """While an image is on screen wait
+    For example a loading window.
+
+    Args:
+        img (str): image location path + name
+    """
+
+    while is_on_screen(img):
+        sleep(0.1)
+
+
+def waituntil(img: str):
+    """Wait until an image appears on screen
+    For example wait for a software to start
+
+    Args:
+        img (str): image location path + name
+    """
+
+    while not is_on_screen(img):
+        sleep(0.1)
```

### Comparing `AutoMonkey-0.1.5/docs/Makefile` & `AutoMonkey-0.1.6/docs/Makefile`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line.
-SPHINXOPTS    =
-SPHINXBUILD   = python -msphinx
-SPHINXPROJ    = automonkey
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line.
+SPHINXOPTS    =
+SPHINXBUILD   = python -msphinx
+SPHINXPROJ    = automonkey
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `AutoMonkey-0.1.5/docs/conf.py` & `AutoMonkey-0.1.6/docs/conf.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-#!/usr/bin/env python
-#
-# automonkey documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
-#
-import os
-import sys
-sys.path.insert(0, os.path.abspath('..'))
-
-import automonkey
-
-# -- General configuration ---------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode', 'autoapi.extension']
-autoapi_dirs = ['../automonkey']
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-#
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
-
-# The master toctree document.
-master_doc = 'index'
-
-# General information about the project.
-project = 'automonkey'
-copyright = "2022, Mihail-Cosmin Munteanu"
-author = "Mihail-Cosmin Munteanu"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = automonkey.__version__
-# The full version, including alpha/beta/rc tags.
-release = automonkey.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = 'en'
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-
-# -- Options for HTML output -------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = 'alabaster'
-
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_theme_options = {}
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
-
-
-# -- Options for HTMLHelp output ---------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = 'automonkeydoc'
-
-
-# -- Options for LaTeX output ------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
-latex_documents = [
-    (master_doc, 'automonkey.tex',
-     'automonkey Documentation',
-     'Mihail-Cosmin Munteanu', 'manual'),
-]
-
-
-# -- Options for manual page output ------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'automonkey',
-     'automonkey Documentation',
-     [author], 1)
-]
-
-
-# -- Options for Texinfo output ----------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (master_doc, 'automonkey',
-     'automonkey Documentation',
-     author,
-     'automonkey',
-     'One line description of project.',
-     'Miscellaneous'),
-]
-
-
-
+#!/usr/bin/env python
+#
+# automonkey documentation build configuration file, created by
+# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+
+# If extensions (or modules to document with autodoc) are in another
+# directory, add these directories to sys.path here. If the directory is
+# relative to the documentation root, use os.path.abspath to make it
+# absolute, like shown here.
+#
+import os
+import sys
+sys.path.insert(0, os.path.abspath('..'))
+
+import automonkey
+
+# -- General configuration ---------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode', 'autoapi.extension']
+autoapi_dirs = ['../automonkey']
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ['_templates']
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+#
+# source_suffix = ['.rst', '.md']
+source_suffix = '.rst'
+
+# The master toctree document.
+master_doc = 'index'
+
+# General information about the project.
+project = 'automonkey'
+copyright = "2022, Mihail-Cosmin Munteanu"
+author = "Mihail-Cosmin Munteanu"
+
+# The version info for the project you're documenting, acts as replacement
+# for |version| and |release|, also used in various other places throughout
+# the built documents.
+#
+# The short X.Y version.
+version = automonkey.__version__
+# The full version, including alpha/beta/rc tags.
+release = automonkey.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = 'en'
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = 'sphinx'
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+
+# -- Options for HTML output -------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = 'alabaster'
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_theme_options = {}
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ['_static']
+
+
+# -- Options for HTMLHelp output ---------------------------------------
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = 'automonkeydoc'
+
+
+# -- Options for LaTeX output ------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass
+# [howto, manual, or own class]).
+latex_documents = [
+    (master_doc, 'automonkey.tex',
+     'automonkey Documentation',
+     'Mihail-Cosmin Munteanu', 'manual'),
+]
+
+
+# -- Options for manual page output ------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [
+    (master_doc, 'automonkey',
+     'automonkey Documentation',
+     [author], 1)
+]
+
+
+# -- Options for Texinfo output ----------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (master_doc, 'automonkey',
+     'automonkey Documentation',
+     author,
+     'automonkey',
+     'One line description of project.',
+     'Miscellaneous'),
+]
+
+
+
```

### Comparing `AutoMonkey-0.1.5/setup.py` & `AutoMonkey-0.1.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,49 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-with open('HISTORY.rst') as history_file:
-    history = history_file.read()
-
-with open("requirements.txt", "r", encoding="utf-8") as _:
-    requirements = _.read().splitlines()
-
-test_requirements = ['pytest>=3', ]
-
-setup(
-    author="Mihail-Cosmin Munteanu",
-    author_email='munteanumihailcosmin@gmail.com',
-    python_requires='>=3.6',
-    classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-    ],
-    description="Python Automation using Mouse and Keyboard for the masses",
-    entry_points={
-        'console_scripts': [
-            'automonkey=automonkey.cli:main',
-        ],
-    },
-    install_requires=requirements,
-    license="GNU General Public License v3",
-    long_description=readme + '\n\n' + history,
-    include_package_data=True,
-    keywords='automonkey',
-    name='automonkey',
-    packages=find_packages(include=['automonkey', 'automonkey.*']),
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/MihailCosmin/automonkey',
-    version="0.1.5",
-    zip_safe=False,
-)
+#!/usr/bin/env python
+"""The setup script."""
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+with open('HISTORY.rst') as history_file:
+    history = history_file.read()
+
+requirements = "requirements.txt"
+with open(requirements, "r", encoding="utf-8") as _:
+    requirements = _.read().splitlines()
+
+test_requirements = ['pytest>=3', ]
+
+setup(
+    author="Mihail-Cosmin Munteanu",
+    author_email='munteanumihailcosmin@gmail.com',
+    python_requires='>=3.6',
+    classifiers=[
+        'Development Status :: 2 - Pre-Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+    ],
+    description="Python Automation using Mouse and Keyboard for the masses",
+    entry_points={
+        'console_scripts': [
+            'automonkey=automonkey.cli:main',
+        ],
+    },
+    install_requires=requirements,
+    license="GNU General Public License v3",
+    long_description=readme + '\n\n' + history,
+    include_package_data=True,
+    keywords='automonkey',
+    name='automonkey',
+    packages=find_packages(include=['automonkey', 'automonkey.*']),
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/MihailCosmin/automonkey',
+    version="0.1.6",
+    zip_safe=False,
+)
```

