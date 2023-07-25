# Comparing `tmp/lifr-0.0.6.tar.gz` & `tmp/lifr-0.0.7.tar.gz`

## Comparing `lifr-0.0.6.tar` & `lifr-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lifr-0.0.6/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.6/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.6/src/LIFR/.DS_Store
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 lifr-0.0.6/src/LIFR/LIFR.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifr-0.0.6/src/LIFR/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lifr-0.0.6/LICENSE
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 lifr-0.0.6/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lifr-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 lifr-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lifr-0.0.7/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.7/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lifr-0.0.7/src/LIFR/.DS_Store
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 lifr-0.0.7/src/LIFR/LIFR.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifr-0.0.7/src/LIFR/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lifr-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 lifr-0.0.7/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lifr-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 lifr-0.0.7/PKG-INFO
```

### Comparing `lifr-0.0.6/.DS_Store` & `lifr-0.0.7/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -267,21 +267,21 @@
 000010a0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
 000010b0: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
 000010c0: 3130 342c 2034 3336 7d2c 207b 3932 302c  104, 436}, {920,
 000010d0: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
 000010e0: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
 000010f0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
 00001100: 0000 008b 0000 0004 0064 0069 0073 0074  .........d.i.s.t
-00001110: 6c67 3153 636f 6d70 0000 0000 0000 3e84  lg1Scomp......>.
+00001110: 6c67 3153 636f 6d70 0000 0000 0000 5b97  lg1Scomp......[.
 00001120: 0000 0004 0064 0069 0073 0074 6d6f 4444  .....d.i.s.tmoDD
-00001130: 626c 6f62 0000 0008 0000 804d 7e31 c541  blob.......M~1.A
+00001130: 626c 6f62 0000 0008 0000 80b3 2238 c541  blob........"8.A
 00001140: 0000 0004 0064 0069 0073 0074 6d6f 6444  .....d.i.s.tmodD
-00001150: 626c 6f62 0000 0008 0000 804d 7e31 c541  blob.......M~1.A
+00001150: 626c 6f62 0000 0008 0000 80b3 2238 c541  blob........"8.A
 00001160: 0000 0004 0064 0069 0073 0074 7068 3153  .....d.i.s.tph1S
-00001170: 636f 6d70 0000 0000 0000 5000 0000 0004  comp......P.....
+00001170: 636f 6d70 0000 0000 0000 7000 0000 0004  comp......p.....
 00001180: 0064 0069 0073 0074 7653 726e 6c6f 6e67  .d.i.s.tvSrnlong
 00001190: 0000 0001 0000 0007 004c 0049 0043 0045  .........L.I.C.E
 000011a0: 004e 0053 0045 496c 6f63 626c 6f62 0000  .N.S.EIlocblob..
 000011b0: 0010 0000 018b 0000 002e ffff ffff ffff  ................
 000011c0: 0000 0000 000e 0070 0079 0070 0072 006f  .......p.y.p.r.o
 000011d0: 006a 0065 0063 0074 002e 0074 006f 006d  .j.e.c.t...t.o.m
 000011e0: 006c 496c 6f63 626c 6f62 0000 0010 0000  .lIlocblob......
@@ -301,17 +301,17 @@
 000012c0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
 000012d0: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
 000012e0: 3130 342c 2034 3336 7d2c 207b 3932 302c  104, 436}, {920,
 000012f0: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
 00001300: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
 00001310: 0000 000d 0000 0000 0000 0000 0000 0000  ................
 00001320: 0000 008b 0000 0003 0073 0072 0063 6c67  .........s.r.clg
-00001330: 3153 636f 6d70 0000 0000 0000 3337 0000  1Scomp......37..
+00001330: 3153 636f 6d70 0000 0000 0000 3343 0000  1Scomp......3C..
 00001340: 0003 0073 0072 0063 6d6f 4444 626c 6f62  ...s.r.cmoDDblob
-00001350: 0000 0008 0000 8045 2238 c541 0000 0003  .......E"8.A....
+00001350: 0000 0008 0000 804b 2238 c541 0000 0003  .......K"8.A....
 00001360: 0073 0072 0063 6d6f 6444 626c 6f62 0000  .s.r.cmodDblob..
 00001370: 0008 0000 00af 6031 c541 0000 0003 0073  ......`1.A.....s
 00001380: 0072 0063 7068 3153 636f 6d70 0000 0000  .r.cph1Scomp....
 00001390: 0000 5000 0000 0003 0073 0072 0063 7653  ..P......s.r.cvS
 000013a0: 726e 6c6f 6e67 0000 0001 0000 0005 0074  rnlong.........t
 000013b0: 0065 0073 0074 0073 496c 6f63 626c 6f62  .e.s.t.sIlocblob
 000013c0: 0000 0010 0000 00b4 0000 002e ffff ffff  ................
```

### Comparing `lifr-0.0.6/src/.DS_Store` & `lifr-0.0.7/src/.DS_Store`

 * *Files 26% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 000002c0: 3130 342c 2034 3336 7d2c 207b 3932 302c  104, 436}, {920,
 000002d0: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
 000002e0: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
 000002f0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
 00000300: 0000 008b 0000 0004 004c 0049 0046 0052  .........L.I.F.R
 00000310: 6473 636c 626f 6f6c 0100 0000 0400 4c00  dsclbool......L.
 00000320: 4900 4600 526c 6731 5363 6f6d 7000 0000  I.F.Rlg1Scomp...
-00000330: 0000 001b 3300 0000 0400 4c00 4900 4600  ....3.....L.I.F.
-00000340: 526d 6f44 4462 6c6f 6200 0000 0800 0080  RmoDDblob.......
-00000350: 4322 38c5 4100 0000 0400 4c00 4900 4600  C"8.A.....L.I.F.
+00000330: 0000 001b 3f00 0000 0400 4c00 4900 4600  ....?.....L.I.F.
+00000340: 526d 6f44 4462 6c6f 6200 0000 0800 0000  RmoDDblob.......
+00000350: 4622 38c5 4100 0000 0400 4c00 4900 4600  F"8.A.....L.I.F.
 00000360: 526d 6f64 4462 6c6f 6200 0000 0800 0000  RmodDblob.......
 00000370: 8060 31c5 4100 0000 0400 4c00 4900 4600  .`1.A.....L.I.F.
 00000380: 5270 6831 5363 6f6d 7000 0000 0000 0030  Rph1Scomp......0
 00000390: 0000 0000 0400 4c00 4900 4600 5276 5372  ......L.I.F.RvSr
 000003a0: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `lifr-0.0.6/src/LIFR/.DS_Store` & `lifr-0.0.7/src/LIFR/.DS_Store`

 * *Files identical despite different names*

### Comparing `lifr-0.0.6/src/LIFR/LIFR.py` & `lifr-0.0.7/src/LIFR/LIFR.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import websockets
+import json
 print("hello")
 
 async def send(content):
     async with websockets.connect('ws://quoi29.ddns.net:8765') as websocket:
         # Send a message to the server
        
         await websocket.send(str(content))
```

### Comparing `lifr-0.0.6/LICENSE` & `lifr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lifr-0.0.6/README.md` & `lifr-0.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 [nom de la variable]=a*b=[a]*[b]=#
 
 en premier lieu nous mettons la variable ou sera stocké la variable
 ensuite nous mettons les valeurs numérique
 ensuite le calcule avec les variables
 ensuite le hashtag sera remplacé par la valeur du calcule
 
-[x1]>[x2] permet de favoriser le text après, si cette condition si elle est juste
-[x1]<[x2] permet de favoriser le text après, si cette condition si elle est juste
-[novalue] si la chaine de charactère après cette expression n'est pas présente dans les valeurs données ou crées, favorise alors le texte après cette condition
-[novalue] si la chaine de charactère après cette expression est présente dans les valeurs données ou crées, favorise alors le texte après cette condition
-[break] pour arreter la generation d'un text
+## Quelques conditions que le module peut utiliser :
+- `[x1]>[x2]` : Cette condition permet de favoriser le texte qui suit si la valeur de `x1` est strictement supérieure à la valeur de `x2`.
+- `[x1]<[x2]` : Cette condition permet de favoriser le texte qui suit si la valeur de `x1` est strictement inférieure à la valeur de `x2`.
+- `[novalue]` : Si la chaîne de caractères qui suit cette expression n'est pas présente dans les valeurs données ou créées, le texte qui suit cette condition sera favorisé.
+- `[novalue]` : Si la chaîne de caractères qui suit cette expression est présente dans les valeurs données ou créées, le texte qui suit cette condition sera favorisé.
+- `[break]` : Cette condition permet d'arrêter la génération d'un texte, indiquant que le processus doit se terminer à cet endroit.
+
+
 
 exemple donnont à LIFR le text suivant:
-"""la valeur données [x1]>6 est donc plus grande que 6 [break]
-la valeur données [x1]<6 n'est donc pas plus grande que 6 [break]
-"""
-par exemple:
-print(LIFR.generate(({"data":"""la valeur données [x1]>6 est donc plus grande que 6 [break]\n la valeur données [x1]<6 nest donc pas plus grande que 6 [break]""","variable":{"[x1]":"2"}}))["text"])
+<p>```la valeur données [x1]>6 est donc plus grande que 6 [break]
+la valeur données [x1]<6 n'est donc pas plus grande que 6 [break]```
+<p>par exemple:</p>
+```print(LIFR.generate(({"data":"""la valeur données [x1]>6 est donc plus grande que 6 [break]\n la valeur données [x1]<6 nest donc pas plus grande que 6 [break]""","variable":{"[x1]":"2"}}))["text"])```
 
-la fonction generate renvoie un dictionnaire composé de:
+<p><b>la fonction generate renvoie un dictionnaire composé de:</b></p>
 	text: le text généré 
 	output: des informations sur le déroulement du procésus
 			divisé en 2 sous parties:
 				score_output:information sur le scorage des mots et de pourquoi ils ont étaient choisis
 				maths-compare:informations sur le changement des variables en nombre pour ensuite verifier une condition mathématique
```

### Comparing `lifr-0.0.6/pyproject.toml` & `lifr-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "LIFR"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Raphael Scott", email="raphael.scott06@gmail.com" },
 ]
 description = "this package allows the user to connect with the LIFR model"
 readme = "README.md"
 requires-python = ">=3.1"
 classifiers = [
```

### Comparing `lifr-0.0.6/PKG-INFO` & `lifr-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LIFR
-Version: 0.0.6
+Version: 0.0.7
 Summary: this package allows the user to connect with the LIFR model
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Raphael Scott <raphael.scott06@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,28 +21,30 @@
 [nom de la variable]=a*b=[a]*[b]=#
 
 en premier lieu nous mettons la variable ou sera stocké la variable
 ensuite nous mettons les valeurs numérique
 ensuite le calcule avec les variables
 ensuite le hashtag sera remplacé par la valeur du calcule
 
-[x1]>[x2] permet de favoriser le text après, si cette condition si elle est juste
-[x1]<[x2] permet de favoriser le text après, si cette condition si elle est juste
-[novalue] si la chaine de charactère après cette expression n'est pas présente dans les valeurs données ou crées, favorise alors le texte après cette condition
-[novalue] si la chaine de charactère après cette expression est présente dans les valeurs données ou crées, favorise alors le texte après cette condition
-[break] pour arreter la generation d'un text
+## Quelques conditions que le module peut utiliser :
+- `[x1]>[x2]` : Cette condition permet de favoriser le texte qui suit si la valeur de `x1` est strictement supérieure à la valeur de `x2`.
+- `[x1]<[x2]` : Cette condition permet de favoriser le texte qui suit si la valeur de `x1` est strictement inférieure à la valeur de `x2`.
+- `[novalue]` : Si la chaîne de caractères qui suit cette expression n'est pas présente dans les valeurs données ou créées, le texte qui suit cette condition sera favorisé.
+- `[novalue]` : Si la chaîne de caractères qui suit cette expression est présente dans les valeurs données ou créées, le texte qui suit cette condition sera favorisé.
+- `[break]` : Cette condition permet d'arrêter la génération d'un texte, indiquant que le processus doit se terminer à cet endroit.
+
+
 
 exemple donnont à LIFR le text suivant:
-"""la valeur données [x1]>6 est donc plus grande que 6 [break]
-la valeur données [x1]<6 n'est donc pas plus grande que 6 [break]
-"""
-par exemple:
-print(LIFR.generate(({"data":"""la valeur données [x1]>6 est donc plus grande que 6 [break]\n la valeur données [x1]<6 nest donc pas plus grande que 6 [break]""","variable":{"[x1]":"2"}}))["text"])
+<p>```la valeur données [x1]>6 est donc plus grande que 6 [break]
+la valeur données [x1]<6 n'est donc pas plus grande que 6 [break]```
+<p>par exemple:</p>
+```print(LIFR.generate(({"data":"""la valeur données [x1]>6 est donc plus grande que 6 [break]\n la valeur données [x1]<6 nest donc pas plus grande que 6 [break]""","variable":{"[x1]":"2"}}))["text"])```
 
-la fonction generate renvoie un dictionnaire composé de:
+<p><b>la fonction generate renvoie un dictionnaire composé de:</b></p>
 	text: le text généré 
 	output: des informations sur le déroulement du procésus
 			divisé en 2 sous parties:
 				score_output:information sur le scorage des mots et de pourquoi ils ont étaient choisis
 				maths-compare:informations sur le changement des variables en nombre pour ensuite verifier une condition mathématique
```

