# Comparing `tmp/httpimport-1.3.0.tar.gz` & `tmp/httpimport-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpimport-1.3.0.tar", last modified: Sun Jan 29 22:55:44 2023, max compression
+gzip compressed data, was "httpimport-1.3.1.tar", last modified: Tue Jul 25 12:15:35 2023, max compression
```

## Comparing `httpimport-1.3.0.tar` & `httpimport-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:55:44.787693 httpimport-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-29 22:55:35.000000 httpimport-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-01-29 22:55:44.787693 httpimport-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-01-29 22:55:35.000000 httpimport-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 22:55:44.787693 httpimport-1.3.0/httpimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-01-29 22:55:44.000000 httpimport-1.3.0/httpimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-29 22:55:44.000000 httpimport-1.3.0/httpimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 22:55:44.000000 httpimport-1.3.0/httpimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-29 22:55:44.000000 httpimport-1.3.0/httpimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30974 2023-01-29 22:55:35.000000 httpimport-1.3.0/httpimport.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-29 22:55:44.787693 httpimport-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-01-29 22:55:35.000000 httpimport-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:15:35.226021 httpimport-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 12:15:20.000000 httpimport-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-07-25 12:15:35.226021 httpimport-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-07-25 12:15:20.000000 httpimport-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:15:35.222021 httpimport-1.3.1/httpimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-07-25 12:15:35.000000 httpimport-1.3.1/httpimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-25 12:15:35.000000 httpimport-1.3.1/httpimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 12:15:35.000000 httpimport-1.3.1/httpimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 12:15:35.000000 httpimport-1.3.1/httpimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31117 2023-07-25 12:15:20.000000 httpimport-1.3.1/httpimport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 12:15:35.226021 httpimport-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-25 12:15:20.000000 httpimport-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 12:15:35.226021 httpimport-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-25 12:15:20.000000 httpimport-1.3.1/tests/test_archives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-25 12:15:20.000000 httpimport-1.3.1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-25 12:15:20.000000 httpimport-1.3.1/tests/test_basicauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-25 12:15:20.000000 httpimport-1.3.1/tests/test_load_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-25 12:15:20.000000 httpimport-1.3.1/tests/test_load_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-25 12:15:20.000000 httpimport-1.3.1/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-25 12:15:20.000000 httpimport-1.3.1/tests/test_pypi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-25 12:15:20.000000 httpimport-1.3.1/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-25 12:15:20.000000 httpimport-1.3.1/tests/test_tls.py
```

### Comparing `httpimport-1.3.0/LICENSE` & `httpimport-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `httpimport-1.3.0/PKG-INFO` & `httpimport-1.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: httpimport
-Version: 1.3.0
-Summary: Module for remote in-memory Python package/module loading through HTTP
-Home-page: https://github.com/operatorequals/httpimport
-Author: John Torakis - operatorequals
-Author-email: john.torakis@gmail.com
-License: Apache2
-Keywords: import,loader,memory,http,network
-Classifier: Development Status :: 6 - Mature
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Testing
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # httpimport
 ## *Python's missing feature!*
 ##### [The feature has been suggested in Python Mailing List](https://lwn.net/Articles/732194/)
 
 _Remote_, _in-memory_ Python _package/module_ `import`ing **through HTTP/S**
 
 [![Downloads](https://img.shields.io/pypi/dm/httpimport)](https://pypi.org/project/httpimport/)
@@ -94,15 +69,15 @@
 
 ### Load Python packages from archives served through HTTP/S
 *No file is touching the disk in the process*
 ```python
 # with httpimport.remote_repo('https://example.com/packages.tar'):
 # with httpimport.remote_repo('https://example.com/packages.tar.bz2'):
 # with httpimport.remote_repo('https://example.com/packages.tar.gz'):
-# with httpimport.remote_repo('https://example.com/packages.tar.xz'): <-- Python3 Only
+# with httpimport.remote_repo('https://example.com/packages.tar.xz'):
 with httpimport.remote_repo('https://example.com/packages.zip'):
   import test_package
 ```
 
 ## Serving a package through HTTP/S
 Any package can be served for `httpimport` using a simple HTTP/S Server:
 ```bash
@@ -153,14 +128,16 @@
 And the above can be used as follows:
 
 ```python
 with httpimport.github_repo('operatorequals','httpimport-private-test', profile='github'):
   import secret_module
 ```
 
+##### Github Tokens look like `github_pat_<gibberish>` and can be issued here: https://github.com/settings/tokens/new
+
 ### Profiles for PyPI
 When importing from PyPI extra options can be used, as described in the profile below:
 
 ```ini
 [pypi]
 
 # The location of a 'requirements.txt' file
@@ -192,16 +169,14 @@
 # '0.3.5' <-- pinned in the profile 'requirements' option
 sample.__url__
 # 'https://files.pythonhosted.org/packages/ec/a8/5ec62d18adde798d33a170e7f72930357aa69a60839194c93eb0fb05e59c/sampleproject-3.0.0-py3-none-any.whl#sample/__init__.py' <-- loaded from 'sampleproject'
 ```
 
 Additionally, all other options cascade to PyPI profiles, such as HTTPS Proxy (HTTP proxies won't work, as PyPI is hosted with HTTPS), `headers`, etc.
 
-##### Github Tokens look like `github_pat_<gibberish>` and can be issued here: https://github.com/settings/tokens/new
-
 ##### NOTE: The values in Profiles MUST NOT be quoted (`'`,`"`)
 
 ### Profile Creation
 Profiles can be provided as INI strings to the `set_profile` function and used in all `httpimport` functions:
 ```python
 httpimport.set_profile("""
 [profile1]
@@ -262,24 +237,22 @@
 import httpimport
 import logging
 
 logging.getLogger('httpimport').setLevel(logging.DEBUG)
 ```
 
 ## Beware: **Huge Security Implications!**
-_Using the `httpimport` with **HTTP URLs** is highly discouraged_
+_Using the `httpimport` with plain **HTTP URLs** is highly discouraged_
   
-As HTTP traffic isn't encrypted and/or integrity checked (_unlike HTTPS_), it is trivial for a remote attacker to intercept the HTTP responses (via an _ARP MiTM_ probably), and add arbitrary _Python_ code to the downloaded _packages/modules_.
-This will directly result in _Remote Code Execution_ on your current user's context!
+As HTTP traffic can be read and changed from all intermediate hosts (_unlike HTTPS_), it is possible for a remote adversary to alter the HTTP responses consumed by `httpimport` and add arbitrary _Python_ code to the downloaded _packages/modules_. This directly results in arbitrary _Remote Code Execution_ on your current user's context of your host!
 
-In other words, you get **totally  compromised**...
+In other words, using plain HTTP through the Internet can compromise your host *without a way to notice it*.
 
 ##### You have been warned! Use only **HTTPS URLs** with `httpimport`!
 
-
 ## Contributors
 * [ldsink](https://github.com/ldsink) - The `RELOAD` flag and Bug Fixes
 * [lavvy](https://github.com/lavvy) - the `load()` function
 * [superloach](https://github.com/superloach) - Deprecation of `imp` module in Python3 in favour of `importlib`
 * [yanliakos](https://github.com/yanliakos) - Bug Fix
 * [rkbennett](https://github.com/rkbennett) - Relative Imports fix, Proxy support
```

### Comparing `httpimport-1.3.0/README.md` & `httpimport-1.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: httpimport
+Version: 1.3.1
+Summary: Module for remote in-memory Python package/module loading through HTTP
+Home-page: https://github.com/operatorequals/httpimport
+Author: John Torakis - operatorequals
+Author-email: john.torakis@gmail.com
+License: Apache2
+Keywords: import,loader,memory,http,network
+Classifier: Development Status :: 6 - Mature
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Testing
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # httpimport
 ## *Python's missing feature!*
 ##### [The feature has been suggested in Python Mailing List](https://lwn.net/Articles/732194/)
 
 _Remote_, _in-memory_ Python _package/module_ `import`ing **through HTTP/S**
 
 [![Downloads](https://img.shields.io/pypi/dm/httpimport)](https://pypi.org/project/httpimport/)
@@ -69,15 +94,15 @@
 
 ### Load Python packages from archives served through HTTP/S
 *No file is touching the disk in the process*
 ```python
 # with httpimport.remote_repo('https://example.com/packages.tar'):
 # with httpimport.remote_repo('https://example.com/packages.tar.bz2'):
 # with httpimport.remote_repo('https://example.com/packages.tar.gz'):
-# with httpimport.remote_repo('https://example.com/packages.tar.xz'): <-- Python3 Only
+# with httpimport.remote_repo('https://example.com/packages.tar.xz'):
 with httpimport.remote_repo('https://example.com/packages.zip'):
   import test_package
 ```
 
 ## Serving a package through HTTP/S
 Any package can be served for `httpimport` using a simple HTTP/S Server:
 ```bash
@@ -128,14 +153,16 @@
 And the above can be used as follows:
 
 ```python
 with httpimport.github_repo('operatorequals','httpimport-private-test', profile='github'):
   import secret_module
 ```
 
+##### Github Tokens look like `github_pat_<gibberish>` and can be issued here: https://github.com/settings/tokens/new
+
 ### Profiles for PyPI
 When importing from PyPI extra options can be used, as described in the profile below:
 
 ```ini
 [pypi]
 
 # The location of a 'requirements.txt' file
@@ -167,16 +194,14 @@
 # '0.3.5' <-- pinned in the profile 'requirements' option
 sample.__url__
 # 'https://files.pythonhosted.org/packages/ec/a8/5ec62d18adde798d33a170e7f72930357aa69a60839194c93eb0fb05e59c/sampleproject-3.0.0-py3-none-any.whl#sample/__init__.py' <-- loaded from 'sampleproject'
 ```
 
 Additionally, all other options cascade to PyPI profiles, such as HTTPS Proxy (HTTP proxies won't work, as PyPI is hosted with HTTPS), `headers`, etc.
 
-##### Github Tokens look like `github_pat_<gibberish>` and can be issued here: https://github.com/settings/tokens/new
-
 ##### NOTE: The values in Profiles MUST NOT be quoted (`'`,`"`)
 
 ### Profile Creation
 Profiles can be provided as INI strings to the `set_profile` function and used in all `httpimport` functions:
 ```python
 httpimport.set_profile("""
 [profile1]
@@ -237,24 +262,22 @@
 import httpimport
 import logging
 
 logging.getLogger('httpimport').setLevel(logging.DEBUG)
 ```
 
 ## Beware: **Huge Security Implications!**
-_Using the `httpimport` with **HTTP URLs** is highly discouraged_
+_Using the `httpimport` with plain **HTTP URLs** is highly discouraged_
   
-As HTTP traffic isn't encrypted and/or integrity checked (_unlike HTTPS_), it is trivial for a remote attacker to intercept the HTTP responses (via an _ARP MiTM_ probably), and add arbitrary _Python_ code to the downloaded _packages/modules_.
-This will directly result in _Remote Code Execution_ on your current user's context!
+As HTTP traffic can be read and changed from all intermediate hosts (_unlike HTTPS_), it is possible for a remote adversary to alter the HTTP responses consumed by `httpimport` and add arbitrary _Python_ code to the downloaded _packages/modules_. This directly results in arbitrary _Remote Code Execution_ on your current user's context of your host!
 
-In other words, you get **totally  compromised**...
+In other words, using plain HTTP through the Internet can compromise your host *without a way to notice it*.
 
 ##### You have been warned! Use only **HTTPS URLs** with `httpimport`!
 
-
 ## Contributors
 * [ldsink](https://github.com/ldsink) - The `RELOAD` flag and Bug Fixes
 * [lavvy](https://github.com/lavvy) - the `load()` function
 * [superloach](https://github.com/superloach) - Deprecation of `imp` module in Python3 in favour of `importlib`
 * [yanliakos](https://github.com/yanliakos) - Bug Fix
 * [rkbennett](https://github.com/rkbennett) - Relative Imports fix, Proxy support
```

### Comparing `httpimport-1.3.0/httpimport.egg-info/PKG-INFO` & `httpimport-1.3.1/httpimport.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpimport
-Version: 1.3.0
+Version: 1.3.1
 Summary: Module for remote in-memory Python package/module loading through HTTP
 Home-page: https://github.com/operatorequals/httpimport
 Author: John Torakis - operatorequals
 Author-email: john.torakis@gmail.com
 License: Apache2
 Keywords: import,loader,memory,http,network
 Classifier: Development Status :: 6 - Mature
@@ -94,15 +94,15 @@
 
 ### Load Python packages from archives served through HTTP/S
 *No file is touching the disk in the process*
 ```python
 # with httpimport.remote_repo('https://example.com/packages.tar'):
 # with httpimport.remote_repo('https://example.com/packages.tar.bz2'):
 # with httpimport.remote_repo('https://example.com/packages.tar.gz'):
-# with httpimport.remote_repo('https://example.com/packages.tar.xz'): <-- Python3 Only
+# with httpimport.remote_repo('https://example.com/packages.tar.xz'):
 with httpimport.remote_repo('https://example.com/packages.zip'):
   import test_package
 ```
 
 ## Serving a package through HTTP/S
 Any package can be served for `httpimport` using a simple HTTP/S Server:
 ```bash
@@ -153,14 +153,16 @@
 And the above can be used as follows:
 
 ```python
 with httpimport.github_repo('operatorequals','httpimport-private-test', profile='github'):
   import secret_module
 ```
 
+##### Github Tokens look like `github_pat_<gibberish>` and can be issued here: https://github.com/settings/tokens/new
+
 ### Profiles for PyPI
 When importing from PyPI extra options can be used, as described in the profile below:
 
 ```ini
 [pypi]
 
 # The location of a 'requirements.txt' file
@@ -192,16 +194,14 @@
 # '0.3.5' <-- pinned in the profile 'requirements' option
 sample.__url__
 # 'https://files.pythonhosted.org/packages/ec/a8/5ec62d18adde798d33a170e7f72930357aa69a60839194c93eb0fb05e59c/sampleproject-3.0.0-py3-none-any.whl#sample/__init__.py' <-- loaded from 'sampleproject'
 ```
 
 Additionally, all other options cascade to PyPI profiles, such as HTTPS Proxy (HTTP proxies won't work, as PyPI is hosted with HTTPS), `headers`, etc.
 
-##### Github Tokens look like `github_pat_<gibberish>` and can be issued here: https://github.com/settings/tokens/new
-
 ##### NOTE: The values in Profiles MUST NOT be quoted (`'`,`"`)
 
 ### Profile Creation
 Profiles can be provided as INI strings to the `set_profile` function and used in all `httpimport` functions:
 ```python
 httpimport.set_profile("""
 [profile1]
@@ -262,24 +262,22 @@
 import httpimport
 import logging
 
 logging.getLogger('httpimport').setLevel(logging.DEBUG)
 ```
 
 ## Beware: **Huge Security Implications!**
-_Using the `httpimport` with **HTTP URLs** is highly discouraged_
+_Using the `httpimport` with plain **HTTP URLs** is highly discouraged_
   
-As HTTP traffic isn't encrypted and/or integrity checked (_unlike HTTPS_), it is trivial for a remote attacker to intercept the HTTP responses (via an _ARP MiTM_ probably), and add arbitrary _Python_ code to the downloaded _packages/modules_.
-This will directly result in _Remote Code Execution_ on your current user's context!
+As HTTP traffic can be read and changed from all intermediate hosts (_unlike HTTPS_), it is possible for a remote adversary to alter the HTTP responses consumed by `httpimport` and add arbitrary _Python_ code to the downloaded _packages/modules_. This directly results in arbitrary _Remote Code Execution_ on your current user's context of your host!
 
-In other words, you get **totally  compromised**...
+In other words, using plain HTTP through the Internet can compromise your host *without a way to notice it*.
 
 ##### You have been warned! Use only **HTTPS URLs** with `httpimport`!
 
-
 ## Contributors
 * [ldsink](https://github.com/ldsink) - The `RELOAD` flag and Bug Fixes
 * [lavvy](https://github.com/lavvy) - the `load()` function
 * [superloach](https://github.com/superloach) - Deprecation of `imp` module in Python3 in favour of `importlib`
 * [yanliakos](https://github.com/yanliakos) - Bug Fix
 * [rkbennett](https://github.com/rkbennett) - Relative Imports fix, Proxy support
```

### Comparing `httpimport-1.3.0/httpimport.py` & `httpimport-1.3.1/httpimport.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from urllib.error import HTTPError, URLError
 from urllib.request import (ProxyHandler, Request, build_opener,
                             install_opener, urlopen)
 
 # ====================== Metadata ======================
 
 __author__ = 'John Torakis - operatorequals'
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 __github__ = 'https://github.com/operatorequals/httpimport'
 
 # ====================== Constants ======================
 
 INSECURE = False
 
 __GIT_SERVICE_URLS = {
@@ -432,20 +432,22 @@
         # Set module path - get filepath and keep only the path until filename
         mod.__path__ = ['/'.join(mod.__file__.split('/')[:-1]) + '/']
         mod.__url__ = self.modules[fullname]['filepath']
 
         mod.__package__ = fullname
 
         # Populate subpackage '__package__' metadata with parent package names
-        if len(fullname.split('.')[:-1]) > 1:
+        pkg_name = '.'.join(fullname.split('.')[:-1])
+        if len(fullname.split('.')[:-1]) > 1 and not self.modules[fullname]['package']:
             # recursively find the parent package
-            pkg_name = '.'.join(fullname.split('.')[:-1])
             while sys.modules[pkg_name].__package__ != pkg_name:
                 pkg_name = '.'.join(pkg_name.split('.')[:-1])
             mod.__package__ = pkg_name
+        elif not self.modules[fullname]['package']:
+            mod.__package__ = pkg_name.split('.')[0]
 
         logger.debug(
             "[*] Metadata (__package__) set to '%s' for %s '%s'" %
             (mod.__package__,
              'package' if self.modules[fullname]['package'] else 'module',
              fullname))
```

### Comparing `httpimport-1.3.0/setup.py` & `httpimport-1.3.1/setup.py`

 * *Files identical despite different names*

