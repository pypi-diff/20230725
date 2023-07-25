# Comparing `tmp/fajrGPT-1.4.4.tar.gz` & `tmp/fajrGPT-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fajrGPT-1.4.4.tar", last modified: Mon Jul 24 12:09:09 2023, max compression
+gzip compressed data, was "fajrGPT-1.4.5.tar", last modified: Tue Jul 25 13:04:51 2023, max compression
```

## Comparing `fajrGPT-1.4.4.tar` & `fajrGPT-1.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 12:09:09.440852 fajrGPT-1.4.4/
--rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.4/LICENSE
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 12:09:09.440639 fajrGPT-1.4.4/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.4/README.md
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 12:09:09.438543 fajrGPT-1.4.4/fajrGPT/
--rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.4/fajrGPT/__init__.py
--rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.4/fajrGPT/quran_metadata.py
--rw-r--r--   0 malek8     (501) staff       (20)    18421 2023-07-24 12:08:27.000000 fajrGPT-1.4.4/fajrGPT/wake.py
-drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-24 12:09:09.440418 fajrGPT-1.4.4/fajrGPT.egg-info/
--rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/PKG-INFO
--rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/SOURCES.txt
--rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/dependency_links.txt
--rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/entry_points.txt
--rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/requires.txt
--rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-24 12:09:09.000000 fajrGPT-1.4.4/fajrGPT.egg-info/top_level.txt
--rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-24 12:09:09.440893 fajrGPT-1.4.4/setup.cfg
--rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-24 12:08:38.000000 fajrGPT-1.4.4/setup.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-25 13:04:51.058085 fajrGPT-1.4.5/
+-rw-r--r--   0 malek8     (501) staff       (20)     1062 2023-05-15 07:44:33.000000 fajrGPT-1.4.5/LICENSE
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-25 13:04:51.057912 fajrGPT-1.4.5/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)     2283 2023-06-12 00:59:24.000000 fajrGPT-1.4.5/README.md
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-25 13:04:51.056354 fajrGPT-1.4.5/fajrGPT/
+-rw-r--r--   0 malek8     (501) staff       (20)        0 2023-06-12 01:14:16.000000 fajrGPT-1.4.5/fajrGPT/__init__.py
+-rw-r--r--   0 malek8     (501) staff       (20)     1400 2023-07-03 14:08:35.000000 fajrGPT-1.4.5/fajrGPT/quran_metadata.py
+-rw-r--r--   0 malek8     (501) staff       (20)    18434 2023-07-25 10:13:28.000000 fajrGPT-1.4.5/fajrGPT/wake.py
+drwxr-xr-x   0 malek8     (501) staff       (20)        0 2023-07-25 13:04:51.057708 fajrGPT-1.4.5/fajrGPT.egg-info/
+-rw-r--r--   0 malek8     (501) staff       (20)     2946 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/PKG-INFO
+-rw-r--r--   0 malek8     (501) staff       (20)      276 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        1 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       46 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/entry_points.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       54 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/requires.txt
+-rw-r--r--   0 malek8     (501) staff       (20)        8 2023-07-25 13:04:51.000000 fajrGPT-1.4.5/fajrGPT.egg-info/top_level.txt
+-rw-r--r--   0 malek8     (501) staff       (20)       38 2023-07-25 13:04:51.058126 fajrGPT-1.4.5/setup.cfg
+-rw-r--r--   0 malek8     (501) staff       (20)     1129 2023-07-25 13:04:41.000000 fajrGPT-1.4.5/setup.py
```

### Comparing `fajrGPT-1.4.4/LICENSE` & `fajrGPT-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.4/PKG-INFO` & `fajrGPT-1.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.4
+Version: 1.4.5
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.4/README.md` & `fajrGPT-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.4/fajrGPT/quran_metadata.py` & `fajrGPT-1.4.5/fajrGPT/quran_metadata.py`

 * *Files identical despite different names*

### Comparing `fajrGPT-1.4.4/fajrGPT/wake.py` & `fajrGPT-1.4.5/fajrGPT/wake.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 COMPLETIONS_MODEL = "gpt-3.5-turbo"
 
 @click.command()
 @click.option('--url', required=True, help='YouTube URL containing desired audio data.')
 @click.option('--time', required=True, help='Countdown time in format [number][h/m/s], i.e. 1h would create a 1 hour timer.')
 @click.option('--output', required=True, help='Name of the output file.')
 @click.option('--names-flag', required=False, help='Whether or not to include a randomly selected name of Allah in the preamble.', default=True)
-@click.option('--transition-time', required=False, help='Time in seconds for the transition between the output audio and the Quran verses.')
+@click.option('--transition-time', required=False, help='Time in seconds for the transition between the output audio and the Quran verses.', default=600)
 @click.option('--surah', required=False, help='Specific Surah from the Quran. Should be given as integer.')
 
 def main(url, time, output, names_flag, transition_time=600, surah=None):
     # Check surah option
     if surah:
         # make the output file name the same as the surah
         output = 'quran-' + '{:03d}'.format(int(surah))
```

### Comparing `fajrGPT-1.4.4/fajrGPT.egg-info/PKG-INFO` & `fajrGPT-1.4.5/fajrGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fajrGPT
-Version: 1.4.4
+Version: 1.4.5
 Summary: A Python application to assist in waking up for Fajr prayer by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube.
 Home-page: https://github.com/malekinho8/quran-wake-up
 Author: Malek Ibrahim
 Author-email: shmeek8@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fajrGPT-1.4.4/setup.py` & `fajrGPT-1.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fajrGPT",
-    version="1.4.4",
+    version="1.4.5",
     author="Malek Ibrahim",
     author_email="shmeek8@gmail.com",
     description=("A Python application to assist in waking up for Fajr prayer "
                  "by providing 3 interactive verses/explanations from the Quran + ChatGPT explanations "
                  "accompanied by a soothing Islamic prayer fade-in and fade-out audio file from YouTube."),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

