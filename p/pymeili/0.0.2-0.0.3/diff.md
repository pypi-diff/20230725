# Comparing `tmp/pymeili-0.0.2.tar.gz` & `tmp/pymeili-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeili-0.0.2.tar", last modified: Tue Jul 25 13:19:47 2023, max compression
+gzip compressed data, was "pymeili-0.0.3.tar", last modified: Tue Jul 25 14:19:34 2023, max compression
```

## Comparing `pymeili-0.0.2.tar` & `pymeili-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 13:19:47.316105 pymeili-0.0.2/
--rw-rw-rw-   0        0        0      104 2023-07-25 13:19:14.000000 pymeili-0.0.2/CHANGELOG.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 13:19:47.303141 pymeili-0.0.2/FONT/
--rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.2/FONT/Futura Extra Black font.ttf
--rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.2/FONT/Futura Heavy font.ttf
--rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.2/FONT/futura medium bt.ttf
--rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.2/LISCENCE.txt
--rw-rw-rw-   0        0        0       31 2023-07-25 13:18:21.000000 pymeili-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      626 2023-07-25 13:19:47.315109 pymeili-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       70 2023-07-25 13:14:45.000000 pymeili-0.0.2/README.txt
--rw-rw-rw-   0        0        0       14 2023-07-25 12:51:05.000000 pymeili-0.0.2/__init__.py
--rw-rw-rw-   0        0        0    20451 2023-07-25 12:21:39.000000 pymeili-0.0.2/beautifyplot.py
-drwxrwxrwx   0        0        0        0 2023-07-25 13:19:47.314111 pymeili-0.0.2/pymeili.egg-info/
--rw-rw-rw-   0        0        0      626 2023-07-25 13:19:47.000000 pymeili-0.0.2/pymeili.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-25 13:19:47.000000 pymeili-0.0.2/pymeili.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:19:47.000000 pymeili-0.0.2/pymeili.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 13:19:47.000000 pymeili-0.0.2/pymeili.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 13:19:47.316105 pymeili-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-07-25 13:18:46.000000 pymeili-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:19:34.156918 pymeili-0.0.3/
+-rw-rw-rw-   0        0        0      142 2023-07-25 14:16:45.000000 pymeili-0.0.3/CHANGELOG.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 14:19:34.140966 pymeili-0.0.3/FONT/
+-rw-rw-rw-   0        0        0    40028 2016-07-20 20:40:52.000000 pymeili-0.0.3/FONT/Futura Extra Black font.ttf
+-rw-rw-rw-   0        0        0    38980 2016-07-20 20:40:52.000000 pymeili-0.0.3/FONT/Futura Heavy font.ttf
+-rw-rw-rw-   0        0        0    38764 2016-07-20 20:40:54.000000 pymeili-0.0.3/FONT/futura medium bt.ttf
+-rw-rw-rw-   0        0        0     1057 2023-07-25 12:28:38.000000 pymeili-0.0.3/LISCENCE.txt
+-rw-rw-rw-   0        0        0       31 2023-07-25 13:18:21.000000 pymeili-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      819 2023-07-25 14:19:34.155926 pymeili-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-25 13:25:52.000000 pymeili-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 14:19:34.141957 pymeili-0.0.3/pymeili/
+-rw-rw-rw-   0        0        0      472 2023-07-25 14:18:09.000000 pymeili-0.0.3/pymeili/__init__.py
+-rw-rw-rw-   0        0        0    20601 2023-07-25 14:17:36.000000 pymeili-0.0.3/pymeili/beautifyplot.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:19:34.155926 pymeili-0.0.3/pymeili.egg-info/
+-rw-rw-rw-   0        0        0      819 2023-07-25 14:19:34.000000 pymeili-0.0.3/pymeili.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-25 14:19:34.000000 pymeili-0.0.3/pymeili.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:19:34.000000 pymeili-0.0.3/pymeili.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 14:19:34.000000 pymeili-0.0.3/pymeili.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:19:34.156918 pymeili-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-07-25 14:17:00.000000 pymeili-0.0.3/setup.py
```

### Comparing `pymeili-0.0.2/FONT/Futura Extra Black font.ttf` & `pymeili-0.0.3/FONT/Futura Extra Black font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.2/FONT/Futura Heavy font.ttf` & `pymeili-0.0.3/FONT/Futura Heavy font.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.2/FONT/futura medium bt.ttf` & `pymeili-0.0.3/FONT/futura medium bt.ttf`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.2/LISCENCE.txt` & `pymeili-0.0.3/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `pymeili-0.0.2/beautifyplot.py` & `pymeili-0.0.3/pymeili/beautifyplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,14 +316,19 @@
 
 # 畫指數
 def xscale(scale, **kwargs):
     plt.xscale(scale, **kwargs)
 def yscale(scale, **kwargs):
     plt.yscale(scale, **kwargs)
 
+def xlog(base=10, **kwargs):
+    plt.xscale('log', base=base, **kwargs)
+def ylog(base=10, **kwargs):
+    plt.yscale('log', base=base, **kwargs)
+
 # 畫網格
 def grid(b=None, which='major', axis='both', color='fg', linestyle=':', linewidth=0.5, **kwargs):
     plt.grid(b, which=which, axis=axis, color=colorlist(color), linestyle=linestyle, linewidth=linewidth, **kwargs)
 
 # spines
 def spines(top=True, right=True, bottom=True, left=True, color='fg', linewidth=3, **kwargs):
     plt.gca().spines['top'].set_visible(top)
```

### Comparing `pymeili-0.0.2/setup.py` & `pymeili-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='pymeili',
-    version='0.0.2',
+    version='0.0.3',
     description='a module to beautify your python plot.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='VVVictorZhou',
     author_email='vichouro@gmail.com',
     license='MIT',
     classifiers=classifiers,
```

