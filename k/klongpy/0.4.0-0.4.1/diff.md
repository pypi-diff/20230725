# Comparing `tmp/klongpy-0.4.0.tar.gz` & `tmp/klongpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.4.0.tar", last modified: Sat Jul 22 00:22:54 2023, max compression
+gzip compressed data, was "klongpy-0.4.1.tar", last modified: Mon Jul 24 23:21:40 2023, max compression
```

## Comparing `klongpy-0.4.0.tar` & `klongpy-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.4.0/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    19806 2023-07-22 00:22:54.762551 klongpy-0.4.0/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    19252 2023-07-22 00:22:29.000000 klongpy-0.4.0/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.4.0/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.4.0/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.4.0/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    26102 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    30678 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20527 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.4.0/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    16759 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    15722 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/sys_fn_ipc.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.4.0/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     1558 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/klongpy/web/
--rw-rw-r--   0 brian     (1000) brian     (1000)       99 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/web/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4721 2023-07-22 00:22:29.000000 klongpy-0.4.0/klongpy/web/sys_fn_web.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    19806 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      687 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      231 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-22 00:22:54.000000 klongpy-0.4.0/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     7493 2023-07-22 00:22:29.000000 klongpy-0.4.0/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-22 00:22:54.762551 klongpy-0.4.0/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1136 2023-07-22 00:22:29.000000 klongpy-0.4.0/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-22 00:22:54.762551 klongpy-0.4.0/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.4.0/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.4.0/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    24124 2023-07-22 00:22:29.000000 klongpy-0.4.0/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.4.0/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2780 2023-06-29 18:49:02.000000 klongpy-0.4.0/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.4.0/tests/test_join_over.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.4.0/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.4.0/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.4.0/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14714 2023-07-22 00:22:29.000000 klongpy-0.4.0/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.4.0/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.4.1/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    22574 2023-07-24 23:21:40.399690 klongpy-0.4.1/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    21981 2023-07-24 23:20:23.000000 klongpy-0.4.1/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.4.1/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    12566 2023-06-29 19:31:08.000000 klongpy-0.4.1/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2897 2023-06-29 19:31:08.000000 klongpy-0.4.1/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    26102 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/core.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30678 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20648 2023-07-24 23:20:23.000000 klongpy-0.4.1/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14185 2023-06-29 19:31:08.000000 klongpy-0.4.1/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    16759 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    15723 2023-07-24 23:20:23.000000 klongpy-0.4.1/klongpy/sys_fn_ipc.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2781 2023-07-24 23:20:23.000000 klongpy-0.4.1/klongpy/sys_fn_timer.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.4.1/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1558 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/klongpy/web/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       99 2023-07-22 00:22:29.000000 klongpy-0.4.1/klongpy/web/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4947 2023-07-24 23:20:23.000000 klongpy-0.4.1/klongpy/web/sys_fn_web.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    22574 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      711 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      231 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-07-24 23:21:40.000000 klongpy-0.4.1/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7493 2023-07-22 00:22:29.000000 klongpy-0.4.1/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-07-24 23:21:40.399690 klongpy-0.4.1/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1136 2023-07-24 23:20:23.000000 klongpy-0.4.1/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-07-24 23:21:40.399690 klongpy-0.4.1/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6305 2023-06-29 18:49:02.000000 klongpy-0.4.1/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.4.1/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    24124 2023-07-22 00:22:29.000000 klongpy-0.4.1/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2088 2023-06-29 18:49:02.000000 klongpy-0.4.1/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2780 2023-06-29 18:49:02.000000 klongpy-0.4.1/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3831 2023-06-30 23:35:49.000000 klongpy-0.4.1/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.4.1/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.4.1/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.4.1/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14714 2023-07-22 00:22:29.000000 klongpy-0.4.1/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7942 2023-06-29 18:49:02.000000 klongpy-0.4.1/tests/test_util.py
```

### Comparing `klongpy-0.4.0/LICENSE` & `klongpy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/PKG-INFO` & `klongpy-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: klongpy
-Version: 0.4.0
-Summary: Python implementation of Klong language.
-Author: Brian Guarraci
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: cupy
-Provides-Extra: cuda12x
-Provides-Extra: cuda11x
-Provides-Extra: cuda111
-Provides-Extra: cuda110
-Provides-Extra: cuda102
-Provides-Extra: rocm-5-0
-Provides-Extra: rocm-4-3
-Provides-Extra: repl
-Provides-Extra: web
-License-File: LICENSE
-
 
 ![Unit Tests](https://github.com/briangu/klongpy/workflows/Unit%20Tests/badge.svg)
 
 # KlongPy
 
 If you're intrigued by the world of [array languages](https://en.wikipedia.org/wiki/Array_programming) and love Python's versatility, meet KlongPy. This project marries the two, bringing Klong's elegant, terse syntax and the computational power of array programming to Python.
 
@@ -33,19 +11,21 @@
 
 The project builds upon the work of [Nils M Holm](https://t3x.org), the creator of the Klong language, who has written a comprehensive [Klong Book](https://t3x.org/klong/book.html) for anyone interested in diving deeper. In short, if you're a data scientist, researcher, or just a programming language enthusiast, KlongPy may just be the next thing you want to check out.
 
 # Overview
 
 KlongPy is a powerful language for high performance data analysis and distributed computing. Some of its main features include:
 
-* Simplicity: KlongPy is based on Klong, a concise, expressive, and easy-to-understand array programming language. Its simple syntax and rich feature set make it an excellent tool for data scientists and engineers.
-* Speed: KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
-* Inter-Process Communication (IPC): KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
-* Array Programming: KlongPy supports array programming, which makes it a great tool for mathematical and scientific computing. You can manipulate entire arrays of data at once, enabling efficient data analysis and manipulation.
-* Compatibility: KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
+* __Simplicity__: KlongPy is based on Klong, a concise, expressive, and easy-to-understand array programming language. Its simple syntax and rich feature set make it an excellent tool for data scientists and engineers.
+* __Speed__: KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
+* __Inter-Process Communication (IPC)__: KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
+* __Array Programming__: KlongPy supports array programming, which makes it a great tool for mathematical and scientific computing. You can manipulate entire arrays of data at once, enabling efficient data analysis and manipulation.
+* __Compatibility__: KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
+* __Web server__: Includes a web server, making it easy to build sites backed by KlongPy capabilities.
+* __Timers__: Includes periodic timer facility to periodically perform tasks.
 
 At its heart, KlongPy is about infusing Python's flexibility with the compact Klong array language, allowing you to tap into the performance of NumPy while writing code that's concise and powerful. 
 
 Consider this simple Klong expression that computes an array's average: (+/a)%#a. Decoded, it means "sum of 'a' divided by the length of 'a'", as read from right to left.
 
 Below, we define the function 'avg' and apply it to the array of 1 million integers (as defined by !1000000)
 
@@ -335,41 +315,83 @@
 
 ## The .cli() Function
 
 The .cli() function creates an IPC client. You can pass it either an integer (interpreted as a port on "localhost:<port>"), a string (interpreted as a host address "<host>:<port>"), or a remote dictionary (which shares the network connection and returns a remote function).
 
 Use .cli() to evaluate commands on a remote KlongPy server, define functions, perform calculations, or retrieve values. You can also pass it a symbol to retrieve a value or a function from the remote server.
 
-Here are some examples:
+Start the IPC server:
+
+```bash
+$ kgpy -s 8888
+Welcome to KlongPy REPL v0.4.0
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-d or ]q to quit
 
+Running IPC server at 8888
+
+?>
 ```
-?> f = .cli(8888)
-?> f("avg::{(+/x)%#x}")   
-?> f("avg(!100)")        
+
+In a different terminal:
+
+```bash
+$ kgpy
+
+?> f::.cli(8888)
+remote[localhost:8888]:fn
+?> f("avg::{(+/x)%#x}")
+:monad
+?> f("avg(!100)")
+49.5
+?> :" Call a remote function and pass a local value (!100)
+?> data::!100
+[ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
+ 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47
+ 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71
+ 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95
+ 96 97 98 99]
+?> f(:avg,,data)
+49.5
 ```
 
 Using remote function proxies, you can reference a remotely defined function and call it as if it were local:
 
 ```
 ?> q::f(:avg)
+remote[localhost:8888]:avg:monad
 ?> q(!100)
 49.5 
 ```
 
 ## The .clid() Function
 
 As seen in Python interop examples, the KlongPy context is effectively a dictionary.  The .clid() function creates an IPC client that treats the remote KlongPy context as a dictionary, allowing you to set/get values on the remote instance.  Combined with the remote function capabilities, the remote dictionary makes it easy to interact with remote KlongPy instances.
 
 Here are some examples:
 
 ```
-?> d = .clid(8888)
-?> d,[:foo 2]             
-?> d,[:bar "hello"]       
-?> d,:fn,{x+1}            
+?> :" Open a remote dictionary using the same connection as f "
+?> d::.clid(f)
+remote[localhost:8888]:dict
+?> :" Add key/value pair :foo -> 2 to remote context "
+?> d,[:foo 2]
+?> :" Get the value for :foo key from the remote context "
+?> d?:foo
+2
+?> d,[:bar "hello"]
+?> d?:bar
+hello
+?> :" Assign a remote function to :fn "
+?> d,:fn,{x+1}
+?> t::d?:fn
+remote[localhost:8888]:fn:monad
+?> t(10)
+11
 ```
 
 These powerful capabilities allow for more effective use of distributed computing resources. Please be aware of potential security issues, as you are allowing a remote server to execute potentially arbitrary commands from your client. Always secure your connections and validate your commands to avoid potential attacks.
 
 ## Remote Function Proxies and Enumeration
 
 Another powerful feature of KlongPy's IPC capabilities is the use of remote function proxies. These function proxies behave as if they were local functions, but are actually executed on a remote server. You can easily create these function proxies using .cli() or .clid(), and then use them as you would any other function.
@@ -409,14 +431,105 @@
 1
 ```
 
 ## Synchronization
 
 While the IPC server I/O is async, the KlongPy interpreter is single-threaded.  All remote operations are synchronous to make it easy to use remote operations as part of a normal workflow.  Of course, when calling over to another KlongPy instance, you have no idea what state that instance is in, but within the calling instance operations will be sequential.
 
+# Web server
+
+KlongPy includes a simple web server module.  It's optional so you need to install the dependencies:
+
+```bash
+$ pip3 install klongpy[web]
+```
+
+The web server allows you to implement KlongPy functions as GET/POST handlers for registered routes.
+
+
+Here's a simple example that lets you fetch and update a data array:
+
+```
+:" Import the Klongpy web module.  Requires pip3 install klongpy[web] first"
+.py("klongpy.web")
+
+:" Array of data to display"
+data::[]
+
+:" Return the data for a GET method at /"
+index::{x;data}
+
+:" Create the GET route handlers"
+get:::{}
+get,"/",index
+
+:" Append the query param q value to data"
+update::{[p];p::x?"p";.p(p);data::data,p}
+
+:" Create the POST route handlers"
+post:::{}
+post,"/p",update
+
+:" Start the web server with the GET and POST handlers"
+.web(8888;get;post)
+
+.p("curl -X POST -d""p=100"" ""http://localhost:8888/p""")
+.p("curl ""http://localhost:8888""")
+
+data
+```
+
+Test it out:
+
+```bash
+$ curl "http://localhost:8888"
+[]
+$ curl -X POST -d"p=100" "http://localhost:8888/p"
+[100]
+$ curl "http://localhost:8888"
+[100]
+```
+
+# Timer
+
+KlongPy includes periodic timer capabilities:
+
+```
+cb::{.p("hello")}
+th::.timer("greeting";1;cb)
+```
+
+To stop the timer, it can be closed via:
+
+```
+.timerc(th)
+```
+
+The following example will create a timer which counts to 5 and then 
+terminates the timer by return 0 from the callback.
+
+```
+counter::0
+u::{counter::counter+1;.p(counter);1}
+c::{.p("stopping timer");0}
+cb::{:[counter<5;u();c()]}
+th::.timer("count";1;cb)
+```
+
+which displays:
+
+```
+1
+2
+3
+4
+5
+stopping timer
+``
+
 
 # Performance
 
 The Klong language is simple, so the overhead is low.  The bulk of the compute time will likely be spent in NumPy doing actual work.
 
 Here's a contrived rough benchmark to show the magnitude differences between Python, KlongPy (CPU + GPU) and Numpy (CPU).
```

### Comparing `klongpy-0.4.0/klongpy/adverbs.py` & `klongpy-0.4.1/klongpy/adverbs.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/klongpy/backend.py` & `klongpy-0.4.1/klongpy/backend.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/klongpy/core.py` & `klongpy-0.4.1/klongpy/core.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/klongpy/dyads.py` & `klongpy-0.4.1/klongpy/dyads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/klongpy/interpreter.py` & `klongpy-0.4.1/klongpy/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from .adverbs import get_adverb_fn
 from .core import *
 from .dyads import create_dyad_functions
 from .monads import create_monad_functions
 from .sys_fn import create_system_functions
 from .sys_fn_ipc import create_system_functions_ipc
+from .sys_fn_timer import create_system_functions_timer
 from .sys_var import *
 from .utils import ReadonlyDict
 
 
 def set_context_var(d, sym, v):
     """
     Sets a context variable, wrapping Python lambda/functions as appropriate.
@@ -121,14 +122,15 @@
     cin = eval_sys_var_cin()
     cout = eval_sys_var_cout()
     cerr = eval_sys_var_cerr()
 
     sys_d = {}
     add_system_functions(sys_d, create_system_functions())
     add_system_functions(sys_d, create_system_functions_ipc())
+    add_system_functions(sys_d, create_system_functions_timer())
     set_context_var(sys_d, KGSym('.e'), eval_sys_var_epsilon()) # TODO: this is probably a bug that this can't be a lambda
     set_context_var(sys_d, KGSym('.cin'), cin)
     set_context_var(sys_d, KGSym('.cout'), cout)
     set_context_var(sys_d, KGSym('.cerr'), cerr)
 
     sys_var = {}
     set_context_var(sys_var, KGSym('.sys.cin'), cin)
```

### Comparing `klongpy-0.4.0/klongpy/monads.py` & `klongpy-0.4.1/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/klongpy/sys_fn.py` & `klongpy-0.4.1/klongpy/sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/klongpy/sys_fn_ipc.py` & `klongpy-0.4.1/klongpy/sys_fn_ipc.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
     def __str__(self):
         return f"{self.nc.__str__()}:dict"
 
 
 def eval_sys_fn_create_client(x):
     """
 
-        .cli(x)                                       [Create IPC client]
+        .cli(x)                                      [Create-IPC-client]
 
         Return a function which evaluates commands on a remote KlongPy server.
 
         If "x" is an integer, then it is interpreted as a port in "localhost:<port>".
         if "x" is a string, then it is interpreted as a host address "<host>:<port>"
 
         If "x" is a remote dictionary, the underlying network connection 
@@ -380,15 +380,15 @@
     nc = x.nc if isinstance(x,NetworkClientDictHandle) else NetworkClient.create_from_addr(x)
     return NetworkClientHandle(nc)
 
 
 def eval_sys_fn_create_dict_client(x):
     """
 
-        .clid(x)                                 [Create IPC dict client]
+        .clid(x)                                [Create-IPC-dict-client]
 
         Return a dictionary which evaluates set/get operations on a remote KlongPy server.
 
         If "x" is an integer, then it is interpreted as a port in "localhost:<port>".
         if "x" is a string, then it is interpreted as a host address "<host>:<port>"
 
         If "x" is a remote function, the underlying network connection 
@@ -433,15 +433,15 @@
     nc = x.nc if isinstance(x,NetworkClientHandle) else NetworkClient.create_from_addr(x)
     return NetworkClientDictHandle(nc)
 
 
 def eval_sys_fn_shutdown_client(x):
     """
 
-        .clic(x)                                      [Close IPC client]
+        .clic(x)                                      [Close-IPC-client]
 
         Close a remote dictionary or function opened by .cli or .clid.
 
         Returns 1 if closed, 0 if already closed.
 
         When a connection is closed, all remote proxies / functions tied to this connection
         will also close and will fail if called.
@@ -454,18 +454,18 @@
             return 1
     return 0
 
 
 _ipc_tcp_server = TcpServerHandler()
 
 
-def eval_sys_create_ipc_server(klong, x):
+def eval_sys_fn_create_ipc_server(klong, x):
     """
 
-        .srv(x)                                       [Start IPC server]
+        .srv(x)                                       [Start-IPC-server]
 
         Open a server port to accept IPC connections.
 
         If "x" is an integer, then it is interpreted as a port in "<all>:<port>".
         if "x" is a string, then it is interpreted as a bind address "<bind>:<port>"
 
         if "x" is 0, then the server is closed and existing client connections are dropped.
```

### Comparing `klongpy-0.4.0/klongpy/sys_var.py` & `klongpy-0.4.1/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/klongpy/utils.py` & `klongpy-0.4.1/klongpy/utils.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/klongpy/web/sys_fn_web.py` & `klongpy-0.4.1/klongpy/web/sys_fn_web.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,15 +60,21 @@
             > curl http://localhost:8080/
             hello, world!
 
     """
     global _main_loop
     global _main_tid
     app = web.Application()
+
+    logging.info("web server start @ ", x)
+    logging.info("GET: ", y)
+    logging.info("POST: ", z)
+
     assert threading.current_thread().ident == _main_tid
+    
     for route, fn in y.items():
         arity = fn.arity if isinstance(fn, KGFn) else fn.get_arity() if issubclass(type(fn), KGLambda) else 0
         if arity != 1:
             logging.info(f"GET route {route} handler function requires arity 1, got {arity}")
             continue
         fn = fn if isinstance(fn, KGCall) else KGFnWrapper(klong, fn) if isinstance(fn, KGFn) else fn
 
@@ -76,32 +82,36 @@
             try:
                 assert request.method == "GET"
                 return web.Response(text=str(fn(dict(request.rel_url.query))))
             except Exception as e:
                 logging.info(f"failed web request: {route} with error {e}")
                 return web.Response(text="Invalid request", status=400)
 
+        logging.info("adding GET route: ", route)
+
         app.router.add_get(route, _get)
 
     for route, fn in z.items():
         arity = fn.arity if isinstance(fn, KGFn) else fn.get_arity() if issubclass(type(fn), KGLambda) else 0
         if arity != 1:
             logging.info(f"POST route {route} handler function requires arity 1, got {arity}")
             continue
         fn = fn if isinstance(fn, KGCall) else KGFnWrapper(klong, fn) if isinstance(fn, KGFn) else fn
 
         async def _post(request: web.Request, fn=fn):
             try:
                 assert request.method == "POST"
-                parameters = await request.post()
+                parameters = dict(await request.post())
                 return web.Response(text=str(fn(parameters)))
             except Exception as e:
-                print(e)
+                logging.error(e)
                 return web.Response(text="Invalid request", status=400)
 
+        logging.info("adding POST route: ", route)
+
         app.router.add_post(route, _post)
 
     runner = web.AppRunner(app)
 
     x = str(x)
     parts = x.split(":")
     bind = parts[0] if len(parts) > 1 else None
```

### Comparing `klongpy-0.4.0/klongpy.egg-info/PKG-INFO` & `klongpy-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python implementation of Klong language.
+Home-page: UNKNOWN
 Author: Brian Guarraci
 License: MIT
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: cupy
-Provides-Extra: cuda12x
-Provides-Extra: cuda11x
-Provides-Extra: cuda111
-Provides-Extra: cuda110
 Provides-Extra: cuda102
-Provides-Extra: rocm-5-0
-Provides-Extra: rocm-4-3
+Provides-Extra: cuda110
+Provides-Extra: cuda111
+Provides-Extra: cuda11x
+Provides-Extra: cuda12x
+Provides-Extra: cupy
 Provides-Extra: repl
+Provides-Extra: rocm-4-3
+Provides-Extra: rocm-5-0
 Provides-Extra: web
 License-File: LICENSE
 
 
 ![Unit Tests](https://github.com/briangu/klongpy/workflows/Unit%20Tests/badge.svg)
 
 # KlongPy
@@ -33,19 +35,21 @@
 
 The project builds upon the work of [Nils M Holm](https://t3x.org), the creator of the Klong language, who has written a comprehensive [Klong Book](https://t3x.org/klong/book.html) for anyone interested in diving deeper. In short, if you're a data scientist, researcher, or just a programming language enthusiast, KlongPy may just be the next thing you want to check out.
 
 # Overview
 
 KlongPy is a powerful language for high performance data analysis and distributed computing. Some of its main features include:
 
-* Simplicity: KlongPy is based on Klong, a concise, expressive, and easy-to-understand array programming language. Its simple syntax and rich feature set make it an excellent tool for data scientists and engineers.
-* Speed: KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
-* Inter-Process Communication (IPC): KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
-* Array Programming: KlongPy supports array programming, which makes it a great tool for mathematical and scientific computing. You can manipulate entire arrays of data at once, enabling efficient data analysis and manipulation.
-* Compatibility: KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
+* __Simplicity__: KlongPy is based on Klong, a concise, expressive, and easy-to-understand array programming language. Its simple syntax and rich feature set make it an excellent tool for data scientists and engineers.
+* __Speed__: KlongPy is designed for high-speed computing, enabling you to process large data sets quickly and efficiently. Its efficient internal mechanisms allow for rapid execution of operations on arrays of data.
+* __Inter-Process Communication (IPC)__: KlongPy has built-in support for IPC, enabling easy communication between different processes and systems. You can create remote function proxies, allowing you to execute functions on a remote server as if they were local functions. This powerful feature facilitates distributed computing tasks.
+* __Array Programming__: KlongPy supports array programming, which makes it a great tool for mathematical and scientific computing. You can manipulate entire arrays of data at once, enabling efficient data analysis and manipulation.
+* __Compatibility__: KlongPy is designed to be compatible with Python, allowing you to leverage existing Python libraries and frameworks in conjunction with KlongPy. This seamless integration enhances KlongPy's usability and adaptability.
+* __Web server__: Includes a web server, making it easy to build sites backed by KlongPy capabilities.
+* __Timers__: Includes periodic timer facility to periodically perform tasks.
 
 At its heart, KlongPy is about infusing Python's flexibility with the compact Klong array language, allowing you to tap into the performance of NumPy while writing code that's concise and powerful. 
 
 Consider this simple Klong expression that computes an array's average: (+/a)%#a. Decoded, it means "sum of 'a' divided by the length of 'a'", as read from right to left.
 
 Below, we define the function 'avg' and apply it to the array of 1 million integers (as defined by !1000000)
 
@@ -335,41 +339,83 @@
 
 ## The .cli() Function
 
 The .cli() function creates an IPC client. You can pass it either an integer (interpreted as a port on "localhost:<port>"), a string (interpreted as a host address "<host>:<port>"), or a remote dictionary (which shares the network connection and returns a remote function).
 
 Use .cli() to evaluate commands on a remote KlongPy server, define functions, perform calculations, or retrieve values. You can also pass it a symbol to retrieve a value or a function from the remote server.
 
-Here are some examples:
+Start the IPC server:
+
+```bash
+$ kgpy -s 8888
+Welcome to KlongPy REPL v0.4.0
+author: Brian Guarraci
+repo  : https://github.com/briangu/klongpy
+crtl-d or ]q to quit
+
+Running IPC server at 8888
 
+?>
 ```
-?> f = .cli(8888)
-?> f("avg::{(+/x)%#x}")   
-?> f("avg(!100)")        
+
+In a different terminal:
+
+```bash
+$ kgpy
+
+?> f::.cli(8888)
+remote[localhost:8888]:fn
+?> f("avg::{(+/x)%#x}")
+:monad
+?> f("avg(!100)")
+49.5
+?> :" Call a remote function and pass a local value (!100)
+?> data::!100
+[ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23
+ 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41 42 43 44 45 46 47
+ 48 49 50 51 52 53 54 55 56 57 58 59 60 61 62 63 64 65 66 67 68 69 70 71
+ 72 73 74 75 76 77 78 79 80 81 82 83 84 85 86 87 88 89 90 91 92 93 94 95
+ 96 97 98 99]
+?> f(:avg,,data)
+49.5
 ```
 
 Using remote function proxies, you can reference a remotely defined function and call it as if it were local:
 
 ```
 ?> q::f(:avg)
+remote[localhost:8888]:avg:monad
 ?> q(!100)
 49.5 
 ```
 
 ## The .clid() Function
 
 As seen in Python interop examples, the KlongPy context is effectively a dictionary.  The .clid() function creates an IPC client that treats the remote KlongPy context as a dictionary, allowing you to set/get values on the remote instance.  Combined with the remote function capabilities, the remote dictionary makes it easy to interact with remote KlongPy instances.
 
 Here are some examples:
 
 ```
-?> d = .clid(8888)
-?> d,[:foo 2]             
-?> d,[:bar "hello"]       
-?> d,:fn,{x+1}            
+?> :" Open a remote dictionary using the same connection as f "
+?> d::.clid(f)
+remote[localhost:8888]:dict
+?> :" Add key/value pair :foo -> 2 to remote context "
+?> d,[:foo 2]
+?> :" Get the value for :foo key from the remote context "
+?> d?:foo
+2
+?> d,[:bar "hello"]
+?> d?:bar
+hello
+?> :" Assign a remote function to :fn "
+?> d,:fn,{x+1}
+?> t::d?:fn
+remote[localhost:8888]:fn:monad
+?> t(10)
+11
 ```
 
 These powerful capabilities allow for more effective use of distributed computing resources. Please be aware of potential security issues, as you are allowing a remote server to execute potentially arbitrary commands from your client. Always secure your connections and validate your commands to avoid potential attacks.
 
 ## Remote Function Proxies and Enumeration
 
 Another powerful feature of KlongPy's IPC capabilities is the use of remote function proxies. These function proxies behave as if they were local functions, but are actually executed on a remote server. You can easily create these function proxies using .cli() or .clid(), and then use them as you would any other function.
@@ -409,14 +455,105 @@
 1
 ```
 
 ## Synchronization
 
 While the IPC server I/O is async, the KlongPy interpreter is single-threaded.  All remote operations are synchronous to make it easy to use remote operations as part of a normal workflow.  Of course, when calling over to another KlongPy instance, you have no idea what state that instance is in, but within the calling instance operations will be sequential.
 
+# Web server
+
+KlongPy includes a simple web server module.  It's optional so you need to install the dependencies:
+
+```bash
+$ pip3 install klongpy[web]
+```
+
+The web server allows you to implement KlongPy functions as GET/POST handlers for registered routes.
+
+
+Here's a simple example that lets you fetch and update a data array:
+
+```
+:" Import the Klongpy web module.  Requires pip3 install klongpy[web] first"
+.py("klongpy.web")
+
+:" Array of data to display"
+data::[]
+
+:" Return the data for a GET method at /"
+index::{x;data}
+
+:" Create the GET route handlers"
+get:::{}
+get,"/",index
+
+:" Append the query param q value to data"
+update::{[p];p::x?"p";.p(p);data::data,p}
+
+:" Create the POST route handlers"
+post:::{}
+post,"/p",update
+
+:" Start the web server with the GET and POST handlers"
+.web(8888;get;post)
+
+.p("curl -X POST -d""p=100"" ""http://localhost:8888/p""")
+.p("curl ""http://localhost:8888""")
+
+data
+```
+
+Test it out:
+
+```bash
+$ curl "http://localhost:8888"
+[]
+$ curl -X POST -d"p=100" "http://localhost:8888/p"
+[100]
+$ curl "http://localhost:8888"
+[100]
+```
+
+# Timer
+
+KlongPy includes periodic timer capabilities:
+
+```
+cb::{.p("hello")}
+th::.timer("greeting";1;cb)
+```
+
+To stop the timer, it can be closed via:
+
+```
+.timerc(th)
+```
+
+The following example will create a timer which counts to 5 and then 
+terminates the timer by return 0 from the callback.
+
+```
+counter::0
+u::{counter::counter+1;.p(counter);1}
+c::{.p("stopping timer");0}
+cb::{:[counter<5;u();c()]}
+th::.timer("count";1;cb)
+```
+
+which displays:
+
+```
+1
+2
+3
+4
+5
+stopping timer
+``
+
 
 # Performance
 
 The Klong language is simple, so the overhead is low.  The bulk of the compute time will likely be spent in NumPy doing actual work.
 
 Here's a contrived rough benchmark to show the magnitude differences between Python, KlongPy (CPU + GPU) and Numpy (CPU).
 
@@ -578,7 +715,9 @@
 :! :& :, :< :> :?
 ```
 
 # Acknowledgement
 
 HUGE thanks to Nils M Holm for his work on Klong and providing the foundations for this interesting project.
 
+
+
```

### Comparing `klongpy-0.4.0/klongpy.egg-info/SOURCES.txt` & `klongpy-0.4.1/klongpy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 klongpy/backend.py
 klongpy/core.py
 klongpy/dyads.py
 klongpy/interpreter.py
 klongpy/monads.py
 klongpy/sys_fn.py
 klongpy/sys_fn_ipc.py
+klongpy/sys_fn_timer.py
 klongpy/sys_var.py
 klongpy/utils.py
 klongpy.egg-info/PKG-INFO
 klongpy.egg-info/SOURCES.txt
 klongpy.egg-info/dependency_links.txt
 klongpy.egg-info/requires.txt
 klongpy.egg-info/top_level.txt
```

### Comparing `klongpy-0.4.0/scripts/kgpy` & `klongpy-0.4.1/scripts/kgpy`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/setup.py` & `klongpy-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
     packages=['klongpy', 'klongpy.web'],
-    version='0.4.0',
+    version='0.4.1',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `klongpy-0.4.0/tests/test_accel.py` & `klongpy-0.4.1/tests/test_accel.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_examples.py` & `klongpy-0.4.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_extra_suite.py` & `klongpy-0.4.1/tests/test_extra_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_fn.py` & `klongpy-0.4.1/tests/test_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_interop.py` & `klongpy-0.4.1/tests/test_interop.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_join_over.py` & `klongpy-0.4.1/tests/test_join_over.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_prog.py` & `klongpy-0.4.1/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_suite.py` & `klongpy-0.4.1/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_suite_file.py` & `klongpy-0.4.1/tests/test_suite_file.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_sys_fn.py` & `klongpy-0.4.1/tests/test_sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.4.0/tests/test_util.py` & `klongpy-0.4.1/tests/test_util.py`

 * *Files identical despite different names*

