# Comparing `tmp/easyencryption-0.1.7.tar.gz` & `tmp/easyencryption-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.1.7.tar", last modified: Tue Jul 25 00:05:52 2023, max compression
+gzip compressed data, was "easyencryption-0.1.7.1.tar", last modified: Tue Jul 25 21:28:19 2023, max compression
```

## Comparing `easyencryption-0.1.7.tar` & `easyencryption-0.1.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 00:05:52.335169 easyencryption-0.1.7/
--rw-rw-rw-   0        0        0     3512 2023-07-25 00:05:52.336168 easyencryption-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2256 2023-07-25 00:04:53.000000 easyencryption-0.1.7/README.md
--rw-rw-rw-   0        0        0      723 2023-07-25 00:05:52.340674 easyencryption-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1992 2023-07-25 00:02:24.000000 easyencryption-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 00:05:52.289066 easyencryption-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 00:05:52.317129 easyencryption-0.1.7/src/easyencryption/
--rw-rw-rw-   0        0        0      584 2023-07-23 21:19:08.000000 easyencryption-0.1.7/src/easyencryption/__init__.py
--rw-rw-rw-   0        0        0     1355 2023-07-25 00:01:43.000000 easyencryption-0.1.7/src/easyencryption/aes.py
--rw-rw-rw-   0        0        0     1679 2023-06-25 21:36:58.000000 easyencryption-0.1.7/src/easyencryption/custom.py
--rw-rw-rw-   0        0        0     1490 2023-07-25 00:00:48.000000 easyencryption-0.1.7/src/easyencryption/ecc.py
--rw-rw-rw-   0        0        0     1087 2023-06-24 15:16:52.000000 easyencryption-0.1.7/src/easyencryption/fernet.py
--rw-rw-rw-   0        0        0     1977 2023-07-25 00:01:03.000000 easyencryption-0.1.7/src/easyencryption/rsa.py
--rw-rw-rw-   0        0        0     2057 2023-06-24 15:16:52.000000 easyencryption-0.1.7/src/easyencryption/sha.py
-drwxrwxrwx   0        0        0        0 2023-07-25 00:05:52.335169 easyencryption-0.1.7/src/easyencryption.egg-info/
--rw-rw-rw-   0        0        0     3512 2023-07-25 00:05:52.000000 easyencryption-0.1.7/src/easyencryption.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-07-25 00:05:52.000000 easyencryption-0.1.7/src/easyencryption.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 00:05:52.000000 easyencryption-0.1.7/src/easyencryption.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-25 00:05:52.000000 easyencryption-0.1.7/src/easyencryption.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-25 00:05:52.000000 easyencryption-0.1.7/src/easyencryption.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 21:28:19.337709 easyencryption-0.1.7.1/
+-rw-rw-rw-   0        0        0     3516 2023-07-25 21:28:19.338710 easyencryption-0.1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2258 2023-07-25 21:22:54.000000 easyencryption-0.1.7.1/README.md
+-rw-rw-rw-   0        0        0      723 2023-07-25 21:28:19.339714 easyencryption-0.1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1994 2023-07-25 21:27:57.000000 easyencryption-0.1.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:28:19.301759 easyencryption-0.1.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 21:28:19.317145 easyencryption-0.1.7.1/src/easyencryption/
+-rw-rw-rw-   0        0        0      642 2023-07-25 21:27:50.000000 easyencryption-0.1.7.1/src/easyencryption/__init__.py
+-rw-rw-rw-   0        0        0     1355 2023-07-25 00:01:43.000000 easyencryption-0.1.7.1/src/easyencryption/aes.py
+-rw-rw-rw-   0        0        0     1679 2023-06-25 21:36:58.000000 easyencryption-0.1.7.1/src/easyencryption/custom.py
+-rw-rw-rw-   0        0        0     1490 2023-07-25 00:00:48.000000 easyencryption-0.1.7.1/src/easyencryption/ecc.py
+-rw-rw-rw-   0        0        0     1087 2023-06-24 15:16:52.000000 easyencryption-0.1.7.1/src/easyencryption/fernet.py
+-rw-rw-rw-   0        0        0     1977 2023-07-25 00:01:03.000000 easyencryption-0.1.7.1/src/easyencryption/rsa.py
+-rw-rw-rw-   0        0        0     2057 2023-06-24 15:16:52.000000 easyencryption-0.1.7.1/src/easyencryption/sha.py
+drwxrwxrwx   0        0        0        0 2023-07-25 21:28:19.337709 easyencryption-0.1.7.1/src/easyencryption.egg-info/
+-rw-rw-rw-   0        0        0     3516 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-25 21:28:19.000000 easyencryption-0.1.7.1/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.1.7/PKG-INFO` & `easyencryption-0.1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -34,14 +34,15 @@
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
 SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
 ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.
 Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
+
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
 
 [![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
```

### Comparing `easyencryption-0.1.7/README.md` & `easyencryption-0.1.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
 SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
 ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.
 Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
+
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
 
 [![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
```

### Comparing `easyencryption-0.1.7/setup.cfg` & `easyencryption-0.1.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.7/setup.py` & `easyencryption-0.1.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
 ##with open('src/easyencryption/__init__.py', 'r') as f:
     ##version = [line.split('=')[1].strip(" '\"") for line in f.read().splitlines() if line.startswith('__version__')][0]
-version = "0.1.7"
+version = "0.1.7.1"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `easyencryption-0.1.7/src/easyencryption/__init__.py` & `easyencryption-0.1.7.1/src/easyencryption/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,7 +12,9 @@
 from .sha import sha384check
 from .sha import sha512encrypt
 from .sha import sha512check
 from .custom import customencrypt
 from .custom import customdecrypt
 from .custom import customencrypttimes
 from .custom import customdecrypttimes
+from .ecc import eccencrypt
+from .ecc import eccdecrypt
```

### Comparing `easyencryption-0.1.7/src/easyencryption/aes.py` & `easyencryption-0.1.7.1/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.7/src/easyencryption/custom.py` & `easyencryption-0.1.7.1/src/easyencryption/custom.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.7/src/easyencryption/ecc.py` & `easyencryption-0.1.7.1/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.7/src/easyencryption/fernet.py` & `easyencryption-0.1.7.1/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.7/src/easyencryption/rsa.py` & `easyencryption-0.1.7.1/src/easyencryption/rsa.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.7/src/easyencryption/sha.py` & `easyencryption-0.1.7.1/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.1.7/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.1.7.1/src/easyencryption.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -34,14 +34,15 @@
 
 Fernet - Cryptographys algorithm that contains "symmetric ciphers, message digests, and key derivation functions" (pypi.org), this is pretty basic encryption.<br />
 AES256 - It is the "current encryption standard" (idera.com), it can slow down slower processors but should be fine on most systems.<br />
 RSA - It uses a pair of keys (public and private) to encrypt data. It encrypts the data with the public key, but the data can only be unencrypted with the private key.<br />
 SHA - Secure Hash Algorithm, used for cryptographic security. Cryptographic hash algorithms produce irreversible and unique hashes. The larger the number of possible hashes, the smaller the chance that two values will create the same hash. The higher number sha means more unique hashes.<br />
 ECC - Elliptic-curve cryptography is an approach to public-key cryptography based on the algebraic structure of elliptic curves over finite fields.
 Custom - A custom Ascii scrambler that I made. It is not the most secure so I wouldn't recommend using it alone, but using it in combination with some other methods provided by this package removes the possibility of the same thing being created. **WARNING** This cannot be used in combination with SHA hashing because of the checking methods.<br /><br />
+
 This is a very simple library that I made for one of my projects, so there might be bugs please report these in the github issues. Although it might be simple it is pretty powerful.<br />
 
 **WARNING** Don't delete the .key files or you cant unencrypt the data that you have encrypted with that key.<br />
 
 # Information
 
 [![Python](https://img.shields.io/pypi/pyversions/easyencryption.svg)](https://pypi.python.org/pypi/easyencryption)
```

