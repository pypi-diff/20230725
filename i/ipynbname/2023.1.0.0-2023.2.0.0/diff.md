# Comparing `tmp/ipynbname-2023.1.0.0.tar.gz` & `tmp/ipynbname-2023.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipynbname-2023.1.0.0.tar", last modified: Sun Apr  9 14:56:24 2023, max compression
+gzip compressed data, was "ipynbname-2023.2.0.0.tar", last modified: Tue Jul 25 06:44:58 2023, max compression
```

## Comparing `ipynbname-2023.1.0.0.tar` & `ipynbname-2023.2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 14:56:24.551340 ipynbname-2023.1.0.0/
--rw-rw-rw-   0        0        0     1092 2023-04-09 11:23:56.000000 ipynbname-2023.1.0.0/LICENSE
--rw-rw-rw-   0        0        0       19 2023-04-09 11:23:56.000000 ipynbname-2023.1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1788 2023-04-09 14:56:24.552340 ipynbname-2023.1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2023-04-09 11:23:56.000000 ipynbname-2023.1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 14:56:24.531798 ipynbname-2023.1.0.0/ipynbname/
--rw-rw-rw-   0        0        0     3749 2023-04-09 11:23:56.000000 ipynbname-2023.1.0.0/ipynbname/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 14:56:24.550374 ipynbname-2023.1.0.0/ipynbname.egg-info/
--rw-rw-rw-   0        0        0     1788 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-09 14:56:24.000000 ipynbname-2023.1.0.0/ipynbname.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-09 14:56:24.558175 ipynbname-2023.1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-04-09 14:41:04.000000 ipynbname-2023.1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:44:58.229221 ipynbname-2023.2.0.0/
+-rw-rw-rw-   0        0        0     1092 2023-04-09 11:23:56.000000 ipynbname-2023.2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       19 2023-04-09 11:23:56.000000 ipynbname-2023.2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1891 2023-07-25 06:44:58.229221 ipynbname-2023.2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-07-25 06:32:44.000000 ipynbname-2023.2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 06:44:58.213135 ipynbname-2023.2.0.0/ipynbname/
+-rw-rw-rw-   0        0        0     3749 2023-04-09 11:23:56.000000 ipynbname-2023.2.0.0/ipynbname/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 06:44:58.229221 ipynbname-2023.2.0.0/ipynbname.egg-info/
+-rw-rw-rw-   0        0        0     1891 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-25 06:44:58.000000 ipynbname-2023.2.0.0/ipynbname.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-25 06:44:58.244925 ipynbname-2023.2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-07-25 06:37:20.000000 ipynbname-2023.2.0.0/setup.py
```

### Comparing `ipynbname-2023.1.0.0/LICENSE` & `ipynbname-2023.2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipynbname-2023.1.0.0/PKG-INFO` & `ipynbname-2023.2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: ipynbname
-Version: 2023.1.0.0
+Version: 2023.2.0.0
 Summary: Simply returns either notebook filename or the full path to the notebook when run from Jupyter notebook in browser.
 Home-page: https://github.com/msm1089/ipynbname
 Author: Mark McPherson
 Author-email: msm1089@yahoo.co.uk
 License: MIT
 Keywords: jupyter,notebook,filename
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.4, <4
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipynbname
 
 When run in a Jupyter notebook, simply returns the notebook filename or the full path to the notebook.
 I created this to help with automating posting blog posts written in Jupyter notebooks directly to
-GitHub Pages.  
-[Check it out](https://msm1089.github.io/2020/09/04/Automating-Jupyter-Notebook-Blog-Post-Deployment.html) if you're looking to use this method of blogging :metal:
+GitHub Pages.
 
 You would think there was already some built-in way to access the current notebook name, but it took many hours
 of searching for a way to do it. As it seems many others did, I tried using Javascript, but the async nature of
 JS meant that it was unreliable. Finally I stumbled on this [post](https://forums.fast.ai/t/jupyter-notebook-enhancements-tips-and-tricks/17064/39).
 I have refactored the code there so a user can get either the name or path, but credit for most of the code
 goes to the author of this post, thanks!
 
@@ -40,7 +39,12 @@
 
 Get the full path to the notebook:
 
 ```python
 import ipynbname
 nb_path = ipynbname.path()
 ```
+## Limitations
+
+Note that this only reliably works when running a notebook in a browser. So it does not currently work for things like nbconvert or papermill.
+
+For VS Code there is a [workaround](https://github.com/msm1089/ipynbname/issues/17#issuecomment-1293269863).
```

### Comparing `ipynbname-2023.1.0.0/README.md` & `ipynbname-2023.2.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # ipynbname
 
 When run in a Jupyter notebook, simply returns the notebook filename or the full path to the notebook.
 I created this to help with automating posting blog posts written in Jupyter notebooks directly to
-GitHub Pages.  
-[Check it out](https://msm1089.github.io/2020/09/04/Automating-Jupyter-Notebook-Blog-Post-Deployment.html) if you're looking to use this method of blogging :metal:
+GitHub Pages.
 
 You would think there was already some built-in way to access the current notebook name, but it took many hours
 of searching for a way to do it. As it seems many others did, I tried using Javascript, but the async nature of
 JS meant that it was unreliable. Finally I stumbled on this [post](https://forums.fast.ai/t/jupyter-notebook-enhancements-tips-and-tricks/17064/39).
 I have refactored the code there so a user can get either the name or path, but credit for most of the code
 goes to the author of this post, thanks!
 
@@ -22,7 +21,12 @@
 
 Get the full path to the notebook:
 
 ```python
 import ipynbname
 nb_path = ipynbname.path()
 ```
+## Limitations
+
+Note that this only reliably works when running a notebook in a browser. So it does not currently work for things like nbconvert or papermill.
+
+For VS Code there is a [workaround](https://github.com/msm1089/ipynbname/issues/17#issuecomment-1293269863).
```

### Comparing `ipynbname-2023.1.0.0/ipynbname/__init__.py` & `ipynbname-2023.2.0.0/ipynbname/__init__.py`

 * *Files identical despite different names*

### Comparing `ipynbname-2023.1.0.0/ipynbname.egg-info/PKG-INFO` & `ipynbname-2023.2.0.0/ipynbname.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: ipynbname
-Version: 2023.1.0.0
+Version: 2023.2.0.0
 Summary: Simply returns either notebook filename or the full path to the notebook when run from Jupyter notebook in browser.
 Home-page: https://github.com/msm1089/ipynbname
 Author: Mark McPherson
 Author-email: msm1089@yahoo.co.uk
 License: MIT
 Keywords: jupyter,notebook,filename
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.4, <4
+Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ipynbname
 
 When run in a Jupyter notebook, simply returns the notebook filename or the full path to the notebook.
 I created this to help with automating posting blog posts written in Jupyter notebooks directly to
-GitHub Pages.  
-[Check it out](https://msm1089.github.io/2020/09/04/Automating-Jupyter-Notebook-Blog-Post-Deployment.html) if you're looking to use this method of blogging :metal:
+GitHub Pages.
 
 You would think there was already some built-in way to access the current notebook name, but it took many hours
 of searching for a way to do it. As it seems many others did, I tried using Javascript, but the async nature of
 JS meant that it was unreliable. Finally I stumbled on this [post](https://forums.fast.ai/t/jupyter-notebook-enhancements-tips-and-tricks/17064/39).
 I have refactored the code there so a user can get either the name or path, but credit for most of the code
 goes to the author of this post, thanks!
 
@@ -40,7 +39,12 @@
 
 Get the full path to the notebook:
 
 ```python
 import ipynbname
 nb_path = ipynbname.path()
 ```
+## Limitations
+
+Note that this only reliably works when running a notebook in a browser. So it does not currently work for things like nbconvert or papermill.
+
+For VS Code there is a [workaround](https://github.com/msm1089/ipynbname/issues/17#issuecomment-1293269863).
```

### Comparing `ipynbname-2023.1.0.0/setup.py` & `ipynbname-2023.2.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from pathlib import Path
 
 here = Path(__file__).parent
 long_description = (here / 'README.md').read_text()
 
 setuptools.setup(
     name='ipynbname',
-    version='2023.1.0.0',
+    version='2023.2.0.0',
     author='Mark McPherson',
     author_email='msm1089@yahoo.co.uk',
     description='Simply returns either notebook filename or the full path to the notebook when run from Jupyter notebook in browser.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     keywords='jupyter notebook filename'.split(),
     url='https://github.com/msm1089/ipynbname',
     packages=setuptools.find_packages(),
     package_data={},
     install_requires=['ipykernel'],
-    python_requires='>=3.4, <4',
+    python_requires='>=3.4',
     classifiers=[
         'Operating System :: OS Independent',
         'Development Status :: 4 - Beta',
         'Framework :: Jupyter',
         'Topic :: Utilities',
         'License :: OSI Approved :: MIT License'
     ]
```

