# Comparing `tmp/JAAEC-0.1.3.tar.gz` & `tmp/JAAEC-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JAAEC-0.1.3.tar", last modified: Mon Jul 24 12:45:36 2023, max compression
+gzip compressed data, was "JAAEC-0.1.4.tar", last modified: Tue Jul 25 14:41:50 2023, max compression
```

## Comparing `JAAEC-0.1.3.tar` & `JAAEC-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-24 12:45:36.165883 JAAEC-0.1.3/
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      155 2023-07-18 14:03:04.000000 JAAEC-0.1.3/AUTHORS.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     3551 2023-07-18 14:03:04.000000 JAAEC-0.1.3/CONTRIBUTING.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       89 2023-07-18 14:03:04.000000 JAAEC-0.1.3/HISTORY.rst
-drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-24 12:45:36.165883 JAAEC-0.1.3/JAAEC/
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     8554 2023-07-24 12:44:50.000000 JAAEC-0.1.3/JAAEC/JAAEC.py
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      214 2023-07-19 14:45:06.000000 JAAEC-0.1.3/JAAEC/__init__.py
-drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-24 12:45:36.165883 JAAEC-0.1.3/JAAEC.egg-info/
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1669 2023-07-24 12:45:36.000000 JAAEC-0.1.3/JAAEC.egg-info/PKG-INFO
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      605 2023-07-24 12:45:36.000000 JAAEC-0.1.3/JAAEC.egg-info/SOURCES.txt
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)        1 2023-07-24 12:45:36.000000 JAAEC-0.1.3/JAAEC.egg-info/dependency_links.txt
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)        1 2023-07-24 12:45:36.000000 JAAEC-0.1.3/JAAEC.egg-info/not-zip-safe
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)        6 2023-07-24 12:45:36.000000 JAAEC-0.1.3/JAAEC.egg-info/top_level.txt
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1069 2023-07-18 14:03:04.000000 JAAEC-0.1.3/LICENSE
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      262 2023-07-18 14:03:04.000000 JAAEC-0.1.3/MANIFEST.in
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1669 2023-07-24 12:45:36.165883 JAAEC-0.1.3/PKG-INFO
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      837 2023-07-19 15:12:50.000000 JAAEC-0.1.3/README.rst
-drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-24 12:45:36.165883 JAAEC-0.1.3/docs/
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      283 2023-07-19 15:33:44.000000 JAAEC-0.1.3/docs/JAAEC.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      606 2023-07-18 14:03:04.000000 JAAEC-0.1.3/docs/Makefile
-drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-24 12:45:36.161883 JAAEC-0.1.3/docs/_build/
-drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-24 12:45:36.161883 JAAEC-0.1.3/docs/_build/html/
-drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-24 12:45:36.165883 JAAEC-0.1.3/docs/_build/html/_static/
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      286 2023-07-19 15:22:59.000000 JAAEC-0.1.3/docs/_build/html/_static/file.png
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       90 2023-07-19 15:22:59.000000 JAAEC-0.1.3/docs/_build/html/_static/minus.png
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       90 2023-07-19 15:22:59.000000 JAAEC-0.1.3/docs/_build/html/_static/plus.png
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       28 2023-07-18 14:03:04.000000 JAAEC-0.1.3/docs/authors.rst
--rwxrwxr-x   0 bugsie    (1000) bugsie    (1000)     4830 2023-07-19 15:34:38.000000 JAAEC-0.1.3/docs/conf.py
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       33 2023-07-18 14:03:04.000000 JAAEC-0.1.3/docs/contributing.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       28 2023-07-18 14:03:04.000000 JAAEC-0.1.3/docs/history.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      323 2023-07-19 15:31:47.000000 JAAEC-0.1.3/docs/index.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1173 2023-07-18 14:03:04.000000 JAAEC-0.1.3/docs/installation.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      803 2023-07-18 14:03:04.000000 JAAEC-0.1.3/docs/make.bat
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       52 2023-07-19 15:33:44.000000 JAAEC-0.1.3/docs/modules.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       27 2023-07-18 14:03:04.000000 JAAEC-0.1.3/docs/readme.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       86 2023-07-18 14:03:04.000000 JAAEC-0.1.3/docs/usage.rst
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      377 2023-07-24 12:45:36.165883 JAAEC-0.1.3/setup.cfg
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1289 2023-07-24 12:45:33.000000 JAAEC-0.1.3/setup.py
-drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-24 12:45:36.165883 JAAEC-0.1.3/tests/
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       35 2023-07-18 14:03:04.000000 JAAEC-0.1.3/tests/__init__.py
--rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      312 2023-07-19 14:50:22.000000 JAAEC-0.1.3/tests/test_JAAEC.py
+drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-25 14:41:50.865280 JAAEC-0.1.4/
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      155 2023-07-18 14:03:04.000000 JAAEC-0.1.4/AUTHORS.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     3551 2023-07-18 14:03:04.000000 JAAEC-0.1.4/CONTRIBUTING.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       89 2023-07-18 14:03:04.000000 JAAEC-0.1.4/HISTORY.rst
+drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-25 14:41:50.865280 JAAEC-0.1.4/JAAEC/
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     8704 2023-07-25 14:40:42.000000 JAAEC-0.1.4/JAAEC/JAAEC.py
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      214 2023-07-19 14:45:06.000000 JAAEC-0.1.4/JAAEC/__init__.py
+drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-25 14:41:50.865280 JAAEC-0.1.4/JAAEC.egg-info/
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1669 2023-07-25 14:41:50.000000 JAAEC-0.1.4/JAAEC.egg-info/PKG-INFO
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      605 2023-07-25 14:41:50.000000 JAAEC-0.1.4/JAAEC.egg-info/SOURCES.txt
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)        1 2023-07-25 14:41:50.000000 JAAEC-0.1.4/JAAEC.egg-info/dependency_links.txt
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)        1 2023-07-25 14:41:50.000000 JAAEC-0.1.4/JAAEC.egg-info/not-zip-safe
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)        6 2023-07-25 14:41:50.000000 JAAEC-0.1.4/JAAEC.egg-info/top_level.txt
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1069 2023-07-18 14:03:04.000000 JAAEC-0.1.4/LICENSE
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      262 2023-07-18 14:03:04.000000 JAAEC-0.1.4/MANIFEST.in
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1669 2023-07-25 14:41:50.865280 JAAEC-0.1.4/PKG-INFO
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      837 2023-07-19 15:12:50.000000 JAAEC-0.1.4/README.rst
+drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-25 14:41:50.865280 JAAEC-0.1.4/docs/
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      283 2023-07-19 15:33:44.000000 JAAEC-0.1.4/docs/JAAEC.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      606 2023-07-18 14:03:04.000000 JAAEC-0.1.4/docs/Makefile
+drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-25 14:41:50.861279 JAAEC-0.1.4/docs/_build/
+drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-25 14:41:50.861279 JAAEC-0.1.4/docs/_build/html/
+drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-25 14:41:50.865280 JAAEC-0.1.4/docs/_build/html/_static/
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      286 2023-07-19 15:22:59.000000 JAAEC-0.1.4/docs/_build/html/_static/file.png
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       90 2023-07-19 15:22:59.000000 JAAEC-0.1.4/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       90 2023-07-19 15:22:59.000000 JAAEC-0.1.4/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       28 2023-07-18 14:03:04.000000 JAAEC-0.1.4/docs/authors.rst
+-rwxrwxr-x   0 bugsie    (1000) bugsie    (1000)     4830 2023-07-19 15:34:38.000000 JAAEC-0.1.4/docs/conf.py
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       33 2023-07-18 14:03:04.000000 JAAEC-0.1.4/docs/contributing.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       28 2023-07-18 14:03:04.000000 JAAEC-0.1.4/docs/history.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      323 2023-07-19 15:31:47.000000 JAAEC-0.1.4/docs/index.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1173 2023-07-18 14:03:04.000000 JAAEC-0.1.4/docs/installation.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      803 2023-07-18 14:03:04.000000 JAAEC-0.1.4/docs/make.bat
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       52 2023-07-19 15:33:44.000000 JAAEC-0.1.4/docs/modules.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       27 2023-07-18 14:03:04.000000 JAAEC-0.1.4/docs/readme.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       86 2023-07-18 14:03:04.000000 JAAEC-0.1.4/docs/usage.rst
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      377 2023-07-25 14:41:50.865280 JAAEC-0.1.4/setup.cfg
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)     1289 2023-07-25 14:41:49.000000 JAAEC-0.1.4/setup.py
+drwxrwxr-x   0 bugsie    (1000) bugsie    (1000)        0 2023-07-25 14:41:50.865280 JAAEC-0.1.4/tests/
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)       35 2023-07-18 14:03:04.000000 JAAEC-0.1.4/tests/__init__.py
+-rw-rw-r--   0 bugsie    (1000) bugsie    (1000)      312 2023-07-19 14:50:22.000000 JAAEC-0.1.4/tests/test_JAAEC.py
```

### Comparing `JAAEC-0.1.3/CONTRIBUTING.rst` & `JAAEC-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `JAAEC-0.1.3/JAAEC/JAAEC.py` & `JAAEC-0.1.4/JAAEC/JAAEC.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,16 @@
             Number of heads in the transformer encoder. Defaults to 8.
         """
 
         super(AmazingEncoder, self).__init__()
 
         self.save_hyperparameters()
 
-        self.input_shape = input_shape
-        self.embedding_shape = embedding_shape
+        self.hparams.input_shape = input_shape
+        self.hparams.embedding_shape = embedding_shape
 
         self.linear_expander = nn.Linear(input_shape[2], embedding_shape[1])
 
         self.linear_encoder = nn.Linear(input_shape[1], 1)
 
         encoder_layer = nn.TransformerEncoderLayer(d_model=embedding_shape[1],
                                                    nhead=num_heads, dim_feedforward=input_shape[1],
@@ -117,16 +117,16 @@
             Number of layers in the transformer decoder. Defaults to 3.
         num_heads : int, optional
             Number of heads in the transformer decoder. Defaults to 8.
         """
 
         super(AmazingDecoder, self).__init__()
 
-        self.input_shape = input_shape
-        self.embedding_shape = embedding_shape
+        self.hparams.input_shape = input_shape
+        self.hparams.embedding_shape = embedding_shape
 
         decoder_layer = nn.TransformerDecoderLayer(d_model=embedding_shape[1],
                                                    nhead=num_heads,
                                                    dim_feedforward=input_shape[1],
                                                    batch_first=True)
 
         self.decoder = nn.TransformerDecoder(decoder_layer, num_layers=num_layers)
@@ -198,15 +198,17 @@
 
         super(AmazingAutoEncoder, self).__init__()
 
         self.encoder = AmazingEncoder(input_shape, embedding_shape, num_layers, num_heads)
 
         self.decoder = AmazingDecoder(input_shape, embedding_shape, num_layers, num_heads)
 
-        self.learning_rate = learning_rate
+        self.hparams.input_shape = input_shape
+        self.hparams.embedding_shape = embedding_shape
+        self.hparams.learning_rate = learning_rate
 
     def forward(self, x: torch.Tensor):
         """
         Defines the computation performed at every call.
 
         Parameters
         ----------
@@ -309,8 +311,8 @@
 
         Returns
         -------
         Adam
             The Adam optimizer with the configured learning rate.
         """
 
-        return Adam(self.parameters(), lr=self.learning_rate)
+        return Adam(self.parameters(), lr=self.hparams.learning_rate)
```

### Comparing `JAAEC-0.1.3/JAAEC.egg-info/PKG-INFO` & `JAAEC-0.1.4/JAAEC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JAAEC
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jake's Amazing Autoencoder is an amazing autoencoder designed for time series applications.
 Home-page: https://github.com/bugsiesegal/JAAEC
 Author: Jake Segal
 Author-email: bugsie@segalnyc.com
 License: MIT license
 Keywords: JAAEC
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `JAAEC-0.1.3/JAAEC.egg-info/SOURCES.txt` & `JAAEC-0.1.4/JAAEC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JAAEC-0.1.3/LICENSE` & `JAAEC-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `JAAEC-0.1.3/PKG-INFO` & `JAAEC-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JAAEC
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jake's Amazing Autoencoder is an amazing autoencoder designed for time series applications.
 Home-page: https://github.com/bugsiesegal/JAAEC
 Author: Jake Segal
 Author-email: bugsie@segalnyc.com
 License: MIT license
 Keywords: JAAEC
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `JAAEC-0.1.3/README.rst` & `JAAEC-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `JAAEC-0.1.3/docs/Makefile` & `JAAEC-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `JAAEC-0.1.3/docs/conf.py` & `JAAEC-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `JAAEC-0.1.3/docs/installation.rst` & `JAAEC-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `JAAEC-0.1.3/docs/make.bat` & `JAAEC-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `JAAEC-0.1.3/setup.py` & `JAAEC-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='JAAEC',
     name='JAAEC',
     packages=find_packages(include=['JAAEC', 'JAAEC.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/bugsiesegal/JAAEC',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

