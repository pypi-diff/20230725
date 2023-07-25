# Comparing `tmp/cron-lite-1.0.tar.gz` & `tmp/cron-lite-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cron-lite-1.0.tar", last modified: Wed May 11 18:48:45 2022, max compression
+gzip compressed data, was "dist/cron-lite-1.1.tar", last modified: Tue Jul 25 07:37:46 2023, max compression
```

## Comparing `cron-lite-1.0.tar` & `cron-lite-1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxrwxrwx   0        0        0        0 2022-05-11 18:48:45.000000 cron-lite-1.0/
--rw-rw-rw-   0        0        0     3670 2022-05-11 18:30:45.000000 cron-lite-1.0/cron_lite.py
--rw-rw-rw-   0        0        0     1686 2022-05-11 18:48:45.000000 cron-lite-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      822 2022-05-11 18:43:23.000000 cron-lite-1.0/setup.py
+drwxr-xr-x   0 baozhenchen   (503) staff       (20)        0 2023-07-25 07:37:46.000000 cron-lite-1.1/
+-rw-r--r--   0 baozhenchen   (503) staff       (20)     1693 2023-07-25 07:37:46.000000 cron-lite-1.1/PKG-INFO
+-rw-r--r--   0 baozhenchen   (503) staff       (20)      841 2023-07-25 07:31:35.000000 cron-lite-1.1/setup.py
+-rw-r--r--   0 baozhenchen   (503) staff       (20)     4543 2023-07-25 07:03:21.000000 cron-lite-1.1/cron_lite.py
```

### Comparing `cron-lite-1.0/setup.py` & `cron-lite-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 # coding: utf-8
 from distutils.core import setup
 from os import path, system
 from sys import argv
 
 if "upload" in argv:
     print("running test")
-    assert system("python test_cron_lite.py") == 0
+    assert system("python3.6 test_cron_lite.py") == 0
 
 this_directory = path.abspath(path.dirname(__file__))
 
 try:
     import pypandoc
     long_description = pypandoc.convert('README.md', 'rst')
 except:
     long_description = ""
 
 setup(
     name='cron-lite',
-    version='1.0',
+    version='1.1',
     description='A very light library to run python functions like cron jobs do.',
     author='Rainy Chan',
     author_email='rainydew@qq.com',
     url='https://github.com/rainydew/cron_lite',
     py_modules=["cron_lite"],
-    install_requires=['croniter>=1.3.4'],
+    install_requires=['croniter>=1.3.4', 'pytz>=2022.7'],
     keywords='cron task decorator schedule',
     long_description=long_description,
     python_requires=">=3.6"
 )
```

