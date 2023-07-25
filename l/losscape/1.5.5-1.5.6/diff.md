# Comparing `tmp/losscape-1.5.5.tar.gz` & `tmp/losscape-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "losscape-1.5.5.tar", last modified: Mon Jul 24 10:21:43 2023, max compression
+gzip compressed data, was "losscape-1.5.6.tar", last modified: Tue Jul 25 08:00:12 2023, max compression
```

## Comparing `losscape-1.5.5.tar` & `losscape-1.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 10:21:43.794081 losscape-1.5.5/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-24 10:21:43.794081 losscape-1.5.5/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.5.5/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 10:21:43.794081 losscape-1.5.5/losscape/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.5.5/losscape/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1715 2023-07-22 18:00:07.000000 losscape-1.5.5/losscape/compute_loss.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.5.5/losscape/create_directions.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16331 2023-07-24 10:21:25.000000 losscape-1.5.5/losscape/create_landscape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.5.5/losscape/train.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-24 10:21:43.794081 losscape-1.5.5/losscape.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-24 10:21:43.000000 losscape-1.5.5/losscape.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-24 10:21:43.000000 losscape-1.5.5/losscape.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-24 10:21:43.000000 losscape-1.5.5/losscape.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-07-24 10:21:43.000000 losscape-1.5.5/losscape.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-24 10:21:43.000000 losscape-1.5.5/losscape.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-24 10:21:43.794081 losscape-1.5.5/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)      596 2023-07-24 10:21:40.000000 losscape-1.5.5/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 08:00:12.026789 losscape-1.5.6/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-25 08:00:12.022789 losscape-1.5.6/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3312 2023-07-21 13:44:05.000000 losscape-1.5.6/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 08:00:12.022789 losscape-1.5.6/losscape/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-18 12:39:49.000000 losscape-1.5.6/losscape/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1715 2023-07-22 18:00:07.000000 losscape-1.5.6/losscape/compute_loss.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1816 2023-07-18 09:41:21.000000 losscape-1.5.6/losscape/create_directions.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16361 2023-07-25 07:58:49.000000 losscape-1.5.6/losscape/create_landscape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2099 2023-07-21 07:07:54.000000 losscape-1.5.6/losscape/train.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-25 08:00:12.022789 losscape-1.5.6/losscape.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3585 2023-07-25 08:00:11.000000 losscape-1.5.6/losscape.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)      300 2023-07-25 08:00:12.000000 losscape-1.5.6/losscape.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-25 08:00:11.000000 losscape-1.5.6/losscape.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       41 2023-07-25 08:00:11.000000 losscape-1.5.6/losscape.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-25 08:00:11.000000 losscape-1.5.6/losscape.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-25 08:00:12.026789 losscape-1.5.6/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)      596 2023-07-25 08:00:08.000000 losscape-1.5.6/setup.py
```

### Comparing `losscape-1.5.5/PKG-INFO` & `losscape-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.5.5
+Version: 1.5.6
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.5.5/README.md` & `losscape-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `losscape-1.5.5/losscape/compute_loss.py` & `losscape-1.5.6/losscape/compute_loss.py`

 * *Files identical despite different names*

### Comparing `losscape-1.5.5/losscape/create_directions.py` & `losscape-1.5.6/losscape/create_directions.py`

 * *Files identical despite different names*

### Comparing `losscape-1.5.5/losscape/create_landscape.py` & `losscape-1.5.6/losscape/create_landscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     init_weights = [p.data for p in model.parameters()]
 
     coords = np.linspace(x_min, x_max, num_points)
     losses = []
 
     for x in coords:
+        print(len(direction))
         _set_weights(model, init_weights, direction, x)
 
         loss = compute_loss(model, train_loader_unshuffled, get_batch, criterion, num_batches)
         losses.append(loss)
 
     _reset_weights(model, init_weights)
```

### Comparing `losscape-1.5.5/losscape/train.py` & `losscape-1.5.6/losscape/train.py`

 * *Files identical despite different names*

### Comparing `losscape-1.5.5/losscape.egg-info/PKG-INFO` & `losscape-1.5.6/losscape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: losscape
-Version: 1.5.5
+Version: 1.5.6
 Summary: Visualize easily the loss landscape of your neural networks
 Home-page: https://github.com/Procuste34/losscape
 Author: Alexandre TL
 Author-email: alexandretl3434@gmail.com
 Description-Content-Type: text/markdown
 
 # loss + landscape = `losscape` 🌄
```

### Comparing `losscape-1.5.5/setup.py` & `losscape-1.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 current_dir = Path(__file__).parent
 desc = (current_dir / "README.md").read_text()
 
 setup(
     name='losscape',
-    version='1.5.5',
+    version='1.5.6',
     url='https://github.com/Procuste34/losscape',
     author='Alexandre TL',
     author_email='alexandretl3434@gmail.com',
     description='Visualize easily the loss landscape of your neural networks',
     long_description=desc,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

