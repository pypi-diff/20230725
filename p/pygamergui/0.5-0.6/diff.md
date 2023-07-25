# Comparing `tmp/pygamergui-0.5.tar.gz` & `tmp/pygamergui-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygamergui-0.5.tar", last modified: Fri Mar  3 11:48:46 2023, max compression
+gzip compressed data, was "pygamergui-0.6.tar", last modified: Tue Jul 25 05:36:07 2023, max compression
```

## Comparing `pygamergui-0.5.tar` & `pygamergui-0.6.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 11:48:46.467249 pygamergui-0.5/
--rw-rw-rw-   0        0        0        0 2023-02-03 08:17:13.000000 pygamergui-0.5/LICENSE
--rw-rw-rw-   0        0        0     2964 2023-03-03 11:48:46.469252 pygamergui-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2439 2023-03-03 11:43:14.000000 pygamergui-0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-02-03 08:17:11.000000 pygamergui-0.5/pyproject.toml
--rw-rw-rw-   0        0        0      662 2023-03-03 11:48:46.478251 pygamergui-0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-03 11:48:46.242250 pygamergui-0.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-03 11:48:46.349251 pygamergui-0.5/src/pygamergui/
--rw-rw-rw-   0        0        0      648 2023-02-27 07:38:05.000000 pygamergui-0.5/src/pygamergui/__init__.py
--rw-rw-rw-   0        0        0     9011 2023-03-03 11:28:03.000000 pygamergui-0.5/src/pygamergui/tools.py
--rw-rw-rw-   0        0        0     1224 2023-02-27 07:38:37.000000 pygamergui-0.5/src/pygamergui/window.py
-drwxrwxrwx   0        0        0        0 2023-03-03 11:48:46.457253 pygamergui-0.5/src/pygamergui.egg-info/
--rw-rw-rw-   0        0        0     2964 2023-03-03 11:48:46.000000 pygamergui-0.5/src/pygamergui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-03-03 11:48:46.000000 pygamergui-0.5/src/pygamergui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 11:48:46.000000 pygamergui-0.5/src/pygamergui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-03 11:48:46.000000 pygamergui-0.5/src/pygamergui.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-03 11:48:46.462250 pygamergui-0.5/tests/
--rw-rw-rw-   0        0        0     1267 2023-03-03 11:32:14.000000 pygamergui-0.5/tests/test.py
+drwxr-xr-x   0 vishnu    (1000) vishnu    (1000)        0 2023-07-25 05:36:07.767021 pygamergui-0.6/
+-rw-rw-rw-   0 vishnu    (1000) vishnu    (1000)     1065 2023-07-25 05:25:25.000000 pygamergui-0.6/LICENSE
+-rw-r--r--   0 vishnu    (1000) vishnu    (1000)     3857 2023-07-25 05:36:07.767021 pygamergui-0.6/PKG-INFO
+-rw-rw-rw-   0 vishnu    (1000) vishnu    (1000)     3349 2023-07-25 05:16:06.000000 pygamergui-0.6/README.md
+-rw-rw-rw-   0 vishnu    (1000) vishnu    (1000)      110 2023-07-07 11:01:54.000000 pygamergui-0.6/pyproject.toml
+-rw-rw-rw-   0 vishnu    (1000) vishnu    (1000)      633 2023-07-25 05:36:07.775020 pygamergui-0.6/setup.cfg
+drwxr-xr-x   0 vishnu    (1000) vishnu    (1000)        0 2023-07-25 05:36:07.759021 pygamergui-0.6/src/
+drwxr-xr-x   0 vishnu    (1000) vishnu    (1000)        0 2023-07-25 05:36:07.763021 pygamergui-0.6/src/pygamergui/
+-rw-rw-rw-   0 vishnu    (1000) vishnu    (1000)      183 2023-07-07 10:15:29.000000 pygamergui-0.6/src/pygamergui/__init__.py
+-rw-r--r--   0 vishnu    (1000) vishnu    (1000)     3811 2023-07-25 03:42:16.000000 pygamergui-0.6/src/pygamergui/buttons.py
+-rw-rw-rw-   0 vishnu    (1000) vishnu    (1000)     5282 2023-07-25 03:42:47.000000 pygamergui-0.6/src/pygamergui/slider.py
+-rw-r--r--   0 vishnu    (1000) vishnu    (1000)     5680 2023-07-25 05:32:09.000000 pygamergui-0.6/src/pygamergui/text.py
+-rw-rw-rw-   0 vishnu    (1000) vishnu    (1000)     2307 2023-07-25 05:32:04.000000 pygamergui-0.6/src/pygamergui/window.py
+drwxr-xr-x   0 vishnu    (1000) vishnu    (1000)        0 2023-07-25 05:36:07.767021 pygamergui-0.6/src/pygamergui.egg-info/
+-rw-r--r--   0 vishnu    (1000) vishnu    (1000)     3857 2023-07-25 05:36:07.000000 pygamergui-0.6/src/pygamergui.egg-info/PKG-INFO
+-rw-r--r--   0 vishnu    (1000) vishnu    (1000)      334 2023-07-25 05:36:07.000000 pygamergui-0.6/src/pygamergui.egg-info/SOURCES.txt
+-rw-r--r--   0 vishnu    (1000) vishnu    (1000)        1 2023-07-25 05:36:07.000000 pygamergui-0.6/src/pygamergui.egg-info/dependency_links.txt
+-rw-r--r--   0 vishnu    (1000) vishnu    (1000)       11 2023-07-25 05:36:07.000000 pygamergui-0.6/src/pygamergui.egg-info/top_level.txt
+drwxr-xr-x   0 vishnu    (1000) vishnu    (1000)        0 2023-07-25 05:36:07.767021 pygamergui-0.6/tests/
+-rw-r--r--   0 vishnu    (1000) vishnu    (1000)     1695 2023-07-25 05:27:09.000000 pygamergui-0.6/tests/test.py
```

### Comparing `pygamergui-0.5/setup.cfg` & `pygamergui-0.6/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2070 7967 616d 6572 6775 690d 0a76   = pygamergui..v
-00000020: 6572 7369 6f6e 203d 2030 2e35 0d0a 6175  ersion = 0.5..au
-00000030: 7468 6f72 203d 2076 6973 686e 7530 310d  thor = vishnu01.
-00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-00000050: 6b6f 6861 7272 7570 6573 6840 676d 6169  koharrupesh@gmai
-00000060: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
-00000070: 6f6e 203d 2041 2070 616b 6167 6520 746f  on = A pakage to
-00000080: 2063 7265 6174 6520 6561 7379 2067 7569   create easy gui
-00000090: 2069 6e20 5079 7468 6f6e 0d0a 6c6f 6e67   in Python..long
-000000a0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000b0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000d0: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-000000e0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
-000000f0: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000100: 6875 622e 636f 6d2f 4269 7368 6e75 2d63  hub.com/Bishnu-c
-00000110: 6f64 6572 2f70 7967 616d 6572 6775 690d  oder/pygamergui.
-00000120: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-00000130: 0d0a 0942 7567 2054 7261 636b 6572 203d  ...Bug Tracker =
-00000140: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000150: 636f 6d2f 4269 7368 6e75 2d63 6f64 6572  com/Bishnu-coder
-00000160: 2f70 7967 616d 6572 6775 690d 0a63 6c61  /pygamergui..cla
-00000170: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-00000180: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000190: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001a0: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
-000001b0: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-000001c0: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-000001d0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-000001e0: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
-000001f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000200: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
-00000210: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
-00000220: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
-00000230: 6571 7569 7265 7320 3d20 3e3d 332e 3130  equires = >=3.10
-00000240: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000250: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000260: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
-00000270: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000280: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000290: 2030 0d0a 0d0a                            0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 7079 6761 6d65 7267 7569 0a76 6572  = pygamergui.ver
+00000020: 7369 6f6e 203d 2030 2e36 0a61 7574 686f  sion = 0.6.autho
+00000030: 7220 3d20 7669 7368 6e75 3031 0a61 7574  r = vishnu01.aut
+00000040: 686f 725f 656d 6169 6c20 3d20 6b6f 6861  hor_email = koha
+00000050: 7272 7570 6573 6840 676d 6169 6c2e 636f  rrupesh@gmail.co
+00000060: 6d0a 6465 7363 7269 7074 696f 6e20 3d20  m.description = 
+00000070: 4120 7061 6b61 6765 2074 6f20 6372 6561  A pakage to crea
+00000080: 7465 2065 6173 7920 6775 6920 696e 2050  te easy gui in P
+00000090: 7974 686f 6e0a 6c6f 6e67 5f64 6573 6372  ython.long_descr
+000000a0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+000000b0: 4541 444d 452e 6d64 0a6c 6f6e 675f 6465  EADME.md.long_de
+000000c0: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
+000000d0: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
+000000e0: 726b 646f 776e 0a75 726c 203d 2068 7474  rkdown.url = htt
+000000f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000100: 4269 7368 6e75 2d63 6f64 6572 2f70 7967  Bishnu-coder/pyg
+00000110: 616d 6572 6775 690a 7072 6f6a 6563 745f  amergui.project_
+00000120: 7572 6c73 203d 200a 0942 7567 2054 7261  urls = ..Bug Tra
+00000130: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
+00000140: 6974 6875 622e 636f 6d2f 4269 7368 6e75  ithub.com/Bishnu
+00000150: 2d63 6f64 6572 2f70 7967 616d 6572 6775  -coder/pygamergu
+00000160: 690a 636c 6173 7369 6669 6572 7320 3d20  i.classifiers = 
+00000170: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000180: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000190: 203a 3a20 330a 094c 6963 656e 7365 203a   :: 3..License :
+000001a0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+000001b0: 3a20 4d49 5420 4c69 6365 6e73 650a 094f  : MIT License..O
+000001c0: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000001d0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000001e0: 740a 0a5b 6f70 7469 6f6e 735d 0a70 6163  t..[options].pac
+000001f0: 6b61 6765 5f64 6972 203d 200a 093d 2073  kage_dir = ..= s
+00000200: 7263 0a70 6163 6b61 6765 7320 3d20 6669  rc.packages = fi
+00000210: 6e64 3a0a 7079 7468 6f6e 5f72 6571 7569  nd:.python_requi
+00000220: 7265 7320 3d20 3e3d 332e 3130 0a0a 5b6f  res = >=3.10..[o
+00000230: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+00000240: 6669 6e64 5d0a 7768 6572 6520 3d20 7372  find].where = sr
+00000250: 630a 0a5b 6567 675f 696e 666f 5d0a 7461  c..[egg_info].ta
+00000260: 675f 6275 696c 6420 3d20 0a74 6167 5f64  g_build = .tag_d
+00000270: 6174 6520 3d20 300a 0a                   ate = 0..
```

### Comparing `pygamergui-0.5/src/pygamergui/tools.py` & `pygamergui-0.6/src/pygamergui/slider.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,231 +1,131 @@
+#imports
 import pygame
+from pygamergui import text
+text=text.text
 
-#@class fot button---------------
-class simple_button():
-    """ this is to crete a simple button either with color change OR with no color change """
-    def __init__(self,w=70,h=70,color=(0,0,255),color1=(0,255,0),target=None,text=None,fg="white",text_size=40,args=[],font=None):
-        self.h=h
-        self.w=w
-        self.color=color
-        self.color1=color1
-        self.target=target
-        self.text=text
-        self.text_size=text_size
-        self.fg=fg
-        self.args=args
-        pygame.font.init()
-        if font == None:
-            self.font = pygame.font.Font("freesansbold.ttf", text_size)
-        else:
-            self.font = pygame.font.Font(font, text_size)
-    def show_no_anemi(self,x,y,window,boder_width=0,corner_round_level=0):
-        
-        #--------for target-----------
-        mouse=pygame.mouse.get_pos()
-        rect=pygame.Rect(x,y,self.w,self.h)
-        if self.target!=None:
-            if rect.collidepoint(mouse):
-                if window.eve.type == pygame.MOUSEBUTTONDOWN:
-                    self.target(self.args)
-        #------------------------------
-
-        #---------draw rect-----------------
-        pygame.draw.rect(window.scren,self.color,rect,boder_width,corner_round_level)
-        #------------------------------------
-        
-        #-------for text----------------
-        if self.text!=None:
-            txt=self.font.render(self.text,True,self.fg)
-            window.scren.blit(txt,(x+(rect.h/20),rect.midleft[1]-18))
-        #--------------------------------
-        
-    def show_color_change(self,x,y,window,boder_width=0,corner_round_level=0):
-        #-------------some variables------------
-        color=self.color
-        mouse=pygame.mouse.get_pos()
-        rect=pygame.Rect(x,y,self.w,self.h)
-        #----------------------------------------
-        
-        #---------for target---------------------
-        if self.target!=None:
-            if rect.collidepoint(mouse):
-                if window.eve.type == pygame.MOUSEBUTTONDOWN:
-                    self.target(self.args)
-        #---------------------------------------
-
-        #-------------for color change----------
-        if rect.collidepoint(mouse):
-                if window.eve.type == pygame.MOUSEBUTTONDOWN:
-                    color=self.color1
-        #---------------------------------------
-
-        #-------draw rect-------------
-        pygame.draw.rect(window.scren,color,rect,boder_width,corner_round_level)
-        #------------------------------
-
-        #-------for text----------------
-        if self.text!=None:
-            txt=self.font.render(self.text,True,self.fg)
-            window.scren.blit(txt,(x+(rect.h/20),rect.midleft[1]-18))
-#--------------------------------
-
-#@class for text------------
-class text:
-    def __init__(self,text,color='white',size=38,font=None):
-        self.text=text
-        self.color=color
-        self.size=size
-        pygame.font.init()
-        if font == None:
-            self.font = pygame.font.Font("freesansbold.ttf", size)
-        else:
-            self.font = pygame.font.Font(font, size)
-    def show(self,window,x,y):
-        txt_surface=self.font.render(self.text,True,self.color)
-        window.scren.blit(txt_surface,(x,y))
-#---------------------------
-
-#@class for radio-button-----
-class button_radio():
-    def __init__(self,radius=10,color='black',target=None):
-        self.r=radius
-        self.color=color
-        self.active=False
-    def show(self,window,x,y):
-        mouse=pygame.mouse.get_pos()
-        pygame.draw.circle(window.scren,self.color,(x,y),self.r,3)
-        rect_circle=pygame.Rect(x,y,self.r*2,self.r*2)
-        rect_circle.center=(x,y)
-        if window.eve.type == pygame.MOUSEBUTTONDOWN:
-            if rect_circle.collidepoint(mouse):
-                if self.active==False:
-                    self.active=True
-                else:self.active=False
-        if self.active:
-            pygame.draw.circle(window.scren,self.color,(x,y),self.r/1.5)
-            return True
-        else:return False
-#----------------------------
+# @class for slider-----------
 
-#@class for slider-----------
 class slider:
-    def __init__(self,x,y,w=150,h=5,color='white',color_circle='white',start=1,end=10,radius=10,corner_round=0,text_size=38,t1_align='side',t2_align='up',t3_align='side',show_text=True,font=None):
-        self.t1=t1_align
-        self.t2=t2_align
-        self.t3=t3_align
-        self.text_show=show_text
-
-        self.x=x
-        self.y=y
-
-        self.color=color
-        self.cc=color_circle
-
-        self.start=start
-        self.end=end
-
-        self.h=h
-        self.w=w
-        self.r=radius
-        self.corner=corner_round
-
-        self.rect=pygame.Rect(self.x,self.y,self.w,self.h)
-
-        self.circleposx=self.rect.centerx
-        self.circleposy=self.rect.centery
-        
-        self.circle_rect=pygame.Rect(self.circleposx,self.circleposy,self.r*2,self.r*2)     
-        self.circle_rect.center=[self.circleposx,self.circleposy]
-
-        self.ts=text_size
-        if font==None:
-            self.text1=text(f'{self.start}',size=text_size)
-            self.text2=text(f'{self.end//2}',size=text_size)
-            self.text3=text(f'{self.end}',size=text_size)
+    def __init__(self, x, y, w=150, h=5, color='white', color_circle='white', start=1, end=10, radius=10,
+                 corner_round=0, text_size=38, t1_align='side', t2_align='up', t3_align='side', show_text=True,
+                 font=None, text_color="white"):
+        self.t1 = t1_align
+        self.t2 = t2_align
+        self.t3 = t3_align
+        self.text_show = show_text
+
+        self.x = x
+        self.y = y
+
+        self.color = color
+        self.cc = color_circle
+
+        self.start = start
+        self.end = end
+
+        self.h = h
+        self.w = w
+        self.r = radius
+        self.corner = corner_round
+
+        self.rect = pygame.Rect(self.x, self.y, self.w, self.h)
+
+        self.circleposx = self.rect.centerx
+        self.circleposy = self.rect.centery
+
+        self.circle_rect = pygame.Rect(self.circleposx, self.circleposy, self.r * 2, self.r * 2)
+        self.circle_rect.center = [self.circleposx, self.circleposy]
+
+        self.ts = text_size
+        if font is None:
+            self.text1 = text(f'{self.start}', size=text_size, color=text_color)
+            self.text2 = text(f'{self.end // 2}', size=text_size, color=text_color)
+            self.text3 = text(f'{self.end}', size=text_size, color=text_color)
         else:
-            self.text1=text(f'{self.start}',size=text_size,font=font)
-            self.text2=text(f'{self.end//2}',size=text_size,font=font)
-            self.text3=text(f'{self.end}',size=text_size,font=font)      
-        
-    def show(self,window):
-        
-        mouse_pressed=False
+            self.text1 = text(f'{self.start}', size=text_size, font=font, color=text_color)
+            self.text2 = text(f'{self.end // 2}', size=text_size, font=font, color=text_color)
+            self.text3 = text(f'{self.end}', size=text_size, font=font, color=text_color)
+
+    def show(self, window):
+
+        mouse_pressed = False
 
         if window.eve.type == pygame.MOUSEBUTTONDOWN:
-            mouse_pressed=True
+            mouse_pressed = True
         if window.eve.type == pygame.MOUSEBUTTONUP and mouse_pressed == True:
-            mouse_pressed=False
+            mouse_pressed = False
 
-        self.circle_rect.center=[self.circleposx,self.circleposy]
-        
-        mouse=pygame.mouse.get_pos()
-        pygame.draw.rect(window.scren,self.color,self.rect,0,self.corner)
-        pygame.draw.circle(window.scren,self.cc,(self.circleposx,self.circleposy),self.r)
-     
-        if mouse_pressed==True:
+        self.circle_rect.center = [self.circleposx, self.circleposy]
+
+        mouse = pygame.mouse.get_pos()
+        pygame.draw.rect(window.scren, self.color, self.rect, 0, self.corner)
+        pygame.draw.circle(window.scren, self.cc, (self.circleposx, self.circleposy), self.r)
+
+        if mouse_pressed == True:
             if self.rect.collidepoint(mouse):
-                self.circleposx=mouse[0]
-        
-        if mouse_pressed==True:
+                self.circleposx = mouse[0]
+
+        if mouse_pressed == True:
             if self.circle_rect.collidepoint(mouse):
-                self.circleposx=mouse[0]
-     
-        if self.text_show==True:
+                self.circleposx = mouse[0]
+
+        if self.text_show == True:
             self.show_text(window)
 
-        pos=self.circleposx-self.rect.midleft[0]
-        return round((pos*self.end)/self.rect.width,2)
-    def show_text(self,window):
+        pos = self.circleposx - self.rect.midleft[0]
+        return round((pos * self.end) / self.rect.width, 2)
+
+    def show_text(self, window):
         # for@start text----------------------
         match self.t1:
             case 'side':
                 self.text1.show(window,
-                            self.rect.midleft[0]-self.ts+20,
-                            self.rect.midleft[1]-20
-                            )
+                                self.rect.midleft[0] - self.ts + 20,
+                                self.rect.midleft[1] - 20
+                                )
             case 'up':
                 self.text1.show(window,
-                            self.rect.topleft[0]-self.ts+25,
-                            self.rect.topleft[1]-self.ts
-                            )
+                                self.rect.topleft[0] - self.ts + 25,
+                                self.rect.topleft[1] - self.ts
+                                )
             case 'down':
                 self.text1.show(window,
-                            self.rect.bottomleft[0]-self.ts+25,
-                            self.rect.bottomleft[1]+self.ts-25
-                            )
+                                self.rect.bottomleft[0] - self.ts + 25,
+                                self.rect.bottomleft[1] + self.ts - 25
+                                )
             case _:
                 raise Exception(f'invalid align command -> {self.t1}. use up, down or side as command')
         # for@mid text---------------------------- 
         match self.t2:
             case 'up':
                 self.text2.show(window,
-                            self.rect.midtop[0]-self.ts+20,
-                            self.rect.midtop[1]-27
-                            )
+                                self.rect.midtop[0] - self.ts + 20,
+                                self.rect.midtop[1] - 27
+                                )
             case 'down':
                 self.text2.show(window,
-                            self.rect.midbottom[0]-self.ts+20,
-                            self.rect.midbottom[1]+self.ts-25
-                            )
+                                self.rect.midbottom[0] - self.ts + 20,
+                                self.rect.midbottom[1] + self.ts - 25
+                                )
             case _:
                 raise Exception(f'invalid align command -> {self.t2} . use up or down as command')
         # for@last text-------------------------------
         match self.t3:
             case 'side':
                 self.text3.show(window,
-                            self.rect.midright[0]-self.ts+20,
-                            self.rect.midleft[1]-20
-                            )
+                                self.rect.midright[0] - self.ts + 20,
+                                self.rect.midleft[1] - 20
+                                )
             case 'up':
                 self.text3.show(window,
-                            self.rect.topright[0]-self.ts+25,
-                            self.rect.topleft[1]-self.ts
-                            )
+                                self.rect.topright[0] - self.ts + 25,
+                                self.rect.topleft[1] - self.ts
+                                )
             case 'down':
                 self.text3.show(window,
-                            self.rect.bottomright[0]-self.ts+25,
-                            self.rect.bottomleft[1]+self.ts-25
-                            )
+                                self.rect.bottomright[0] - self.ts + 25,
+                                self.rect.bottomleft[1] + self.ts - 25
+                                )
             case _:
                 raise Exception(f'invalid align command -> {self.t3} . use up, down or side as command')
-#-----------------------------
+# -----------------------------
```

