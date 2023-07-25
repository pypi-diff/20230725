# Comparing `tmp/tally-token-0.3.0.tar.gz` & `tmp/tally-token-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tally-token-0.3.0.tar", last modified: Sat Jul 15 02:44:00 2023, max compression
+gzip compressed data, was "tally-token-0.3.1.tar", last modified: Tue Jul 25 09:03:15 2023, max compression
```

## Comparing `tally-token-0.3.0.tar` & `tally-token-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-15 02:43:40.000000 tally-token-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/renovate.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/workflows/happy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/workflows/spellcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-15 02:43:40.000000 tally-token-0.3.0/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-07-15 02:43:40.000000 tally-token-0.3.0/.gitignore.in
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-15 02:44:00.908723 tally-token-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-15 02:43:40.000000 tally-token-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    39018 2023-07-15 02:43:40.000000 tally-token-0.3.0/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-15 02:43:40.000000 tally-token-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-15 02:44:00.908723 tally-token-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/tally_token/
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-15 02:43:40.000000 tally-token-0.3.0/tally_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-15 02:43:40.000000 tally-token-0.3.0/tally_token/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/tally_token.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-15 02:43:40.000000 tally-token-0.3.0/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-15 02:43:40.000000 tally-token-0.3.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:15.075403 tally-token-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 09:02:51.000000 tally-token-0.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:15.071403 tally-token-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-25 09:02:51.000000 tally-token-0.3.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 09:02:51.000000 tally-token-0.3.1/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:15.075403 tally-token-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-25 09:02:51.000000 tally-token-0.3.1/.github/workflows/happy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-25 09:02:51.000000 tally-token-0.3.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-25 09:02:51.000000 tally-token-0.3.1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 09:02:51.000000 tally-token-0.3.1/.github/workflows/spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-25 09:02:51.000000 tally-token-0.3.1/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-07-25 09:02:51.000000 tally-token-0.3.1/.gitignore.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-25 09:03:15.075403 tally-token-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-25 09:02:51.000000 tally-token-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    39018 2023-07-25 09:02:51.000000 tally-token-0.3.1/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-25 09:02:51.000000 tally-token-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-25 09:03:15.075403 tally-token-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:15.075403 tally-token-0.3.1/tally_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-25 09:02:51.000000 tally-token-0.3.1/tally_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-25 09:02:51.000000 tally-token-0.3.1/tally_token/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 09:03:15.000000 tally-token-0.3.1/tally_token/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:15.075403 tally-token-0.3.1/tally_token.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-07-25 09:03:15.000000 tally-token-0.3.1/tally_token.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-25 09:03:15.000000 tally-token-0.3.1/tally_token.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:03:15.000000 tally-token-0.3.1/tally_token.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 09:03:15.000000 tally-token-0.3.1/tally_token.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 09:03:15.000000 tally-token-0.3.1/tally_token.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:03:15.075403 tally-token-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-25 09:02:51.000000 tally-token-0.3.1/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 09:02:51.000000 tally-token-0.3.1/tests/test_cli.py
```

### Comparing `tally-token-0.3.0/.github/workflows/pypi-publish.yml` & `tally-token-0.3.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `tally-token-0.3.0/.github/workflows/python-test.yml` & `tally-token-0.3.1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `tally-token-0.3.0/.gitignore` & `tally-token-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tally-token-0.3.0/PKG-INFO` & `tally-token-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tally-token
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library to split data into tokens
 Home-page: https://github.com/kitsuyui/python-tally-token
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -68,14 +68,28 @@
 
 You can use `merge` to merge multiple files into a file.
 
 ```sh
 $ tally-token merge merged.bin split-1.bin split-2.bin split-3.bin
 ```
 
+### Large files
+
+Nothing special. You can split and merge large file.
+
+```sh
+$ dd if=/dev/urandom of=original.1g.bin bs=1G count=1
+$ tally-token split original.1g.bin split-1.bin split-2.bin split-3.bin
+$ shasum -a 256 original.1g.bin
+> 736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965 original.1g.bin
+$ tally-token merge recovery.1g.bin split-1.bin split-2.bin split-3.bin
+$ shasum -a 256 recovery.1g.bin
+> 736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965 recovery.1g.bin
+```
+
 ## Example
 
 ### split
 
 You can use `split_text` to split text into tokens. `split_text` returns list of random bytes.
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tally-token Version: 0.3.0 Summary: A library to
+Metadata-Version: 2.1 Name: tally-token Version: 0.3.1 Summary: A library to
 split data into tokens Home-page: https://github.com/kitsuyui/python-tally-
 token Author: Yui Kitsu Author-email: kitsuyui+github@kitsuyui.com License:
 BSD-3-Clause Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: BSD License Classifier: Topic :: Security :: Cryptography
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -28,18 +28,26 @@
 {split,merge} Commands: split: split a file into multiple files merge: merge
 multiple files into a fileExample: tally-token split example.bin example.bin.1
 example.bin.2 example.bin.3 tally-token merge example-merged.bin example.bin.1
 example.bin.2 example.bin.3 options: -h, --help show this help message and exit
 ``` ### split You can use `split` to split a file into multiple files. ```sh $
 tally-token split something.bin split-1.bin split-2.bin split-3.bin ``` ###
 merge You can use `merge` to merge multiple files into a file. ```sh $ tally-
-token merge merged.bin split-1.bin split-2.bin split-3.bin ``` ## Example ###
-split You can use `split_text` to split text into tokens. `split_text` returns
-list of random bytes. ```python >>> from tally_token import split_text >>>
-split_text("Hello, World!") [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
+token merge merged.bin split-1.bin split-2.bin split-3.bin ``` ### Large files
+Nothing special. You can split and merge large file. ```sh $ dd if=/dev/urandom
+of=original.1g.bin bs=1G count=1 $ tally-token split original.1g.bin split-
+1.bin split-2.bin split-3.bin $ shasum -a 256 original.1g.bin >
+736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965
+original.1g.bin $ tally-token merge recovery.1g.bin split-1.bin split-2.bin
+split-3.bin $ shasum -a 256 recovery.1g.bin >
+736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965
+recovery.1g.bin ``` ## Example ### split You can use `split_text` to split text
+into tokens. `split_text` returns list of random bytes. ```python >>> from
+tally_token import split_text >>> split_text("Hello, World!")
+[b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80'] ``` ### merge You can use
 `merge_text` to merge tokens into text. `merge_text` returns cleartext.
 ```python >>> from tally_token import merge_text >>> merge_text(
 [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80']) 'Hello, World!' ``` ### split
 with custom length ```python >>> from tally_token import split_text, merge_text
 >>> split_text("Hello, World!", 5) [b'N&\xce\\\xbc6dxp\x87\xa8#z',
```

### Comparing `tally-token-0.3.0/README.md` & `tally-token-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -48,14 +48,28 @@
 
 You can use `merge` to merge multiple files into a file.
 
 ```sh
 $ tally-token merge merged.bin split-1.bin split-2.bin split-3.bin
 ```
 
+### Large files
+
+Nothing special. You can split and merge large file.
+
+```sh
+$ dd if=/dev/urandom of=original.1g.bin bs=1G count=1
+$ tally-token split original.1g.bin split-1.bin split-2.bin split-3.bin
+$ shasum -a 256 original.1g.bin
+> 736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965 original.1g.bin
+$ tally-token merge recovery.1g.bin split-1.bin split-2.bin split-3.bin
+$ shasum -a 256 recovery.1g.bin
+> 736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965 recovery.1g.bin
+```
+
 ## Example
 
 ### split
 
 You can use `split_text` to split text into tokens. `split_text` returns list of random bytes.
 
 ```python
```

#### html2text {}

```diff
@@ -18,18 +18,26 @@
 {split,merge} Commands: split: split a file into multiple files merge: merge
 multiple files into a fileExample: tally-token split example.bin example.bin.1
 example.bin.2 example.bin.3 tally-token merge example-merged.bin example.bin.1
 example.bin.2 example.bin.3 options: -h, --help show this help message and exit
 ``` ### split You can use `split` to split a file into multiple files. ```sh $
 tally-token split something.bin split-1.bin split-2.bin split-3.bin ``` ###
 merge You can use `merge` to merge multiple files into a file. ```sh $ tally-
-token merge merged.bin split-1.bin split-2.bin split-3.bin ``` ## Example ###
-split You can use `split_text` to split text into tokens. `split_text` returns
-list of random bytes. ```python >>> from tally_token import split_text >>>
-split_text("Hello, World!") [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
+token merge merged.bin split-1.bin split-2.bin split-3.bin ``` ### Large files
+Nothing special. You can split and merge large file. ```sh $ dd if=/dev/urandom
+of=original.1g.bin bs=1G count=1 $ tally-token split original.1g.bin split-
+1.bin split-2.bin split-3.bin $ shasum -a 256 original.1g.bin >
+736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965
+original.1g.bin $ tally-token merge recovery.1g.bin split-1.bin split-2.bin
+split-3.bin $ shasum -a 256 recovery.1g.bin >
+736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965
+recovery.1g.bin ``` ## Example ### split You can use `split_text` to split text
+into tokens. `split_text` returns list of random bytes. ```python >>> from
+tally_token import split_text >>> split_text("Hello, World!")
+[b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80'] ``` ### merge You can use
 `merge_text` to merge tokens into text. `merge_text` returns cleartext.
 ```python >>> from tally_token import merge_text >>> merge_text(
 [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80']) 'Hello, World!' ``` ### split
 with custom length ```python >>> from tally_token import split_text, merge_text
 >>> split_text("Hello, World!", 5) [b'N&\xce\\\xbc6dxp\x87\xa8#z',
```

### Comparing `tally-token-0.3.0/poetry.lock` & `tally-token-0.3.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `tally-token-0.3.0/pyproject.toml` & `tally-token-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tally-token-0.3.0/setup.cfg` & `tally-token-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tally-token-0.3.0/tally_token/__init__.py` & `tally-token-0.3.1/tally_token/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This module provides a simple way to split a secret into multiple tokens.
 The secret can be recovered only if all the tokens are merged together.
 """
 from __future__ import annotations
 
 import secrets
+from io import BufferedReader, BufferedWriter
 
 
 def split_text(
     clear_text: str, into: int = 2, *, encoding: str = "utf-8"
 ) -> list[bytes]:
     """Split a text into multiple tokens.
 
@@ -18,14 +19,38 @@
         into: The number of tokens to be generated.
         encoding: The encoding of the text.
     """
     clear_text_bytes = bytes(clear_text, encoding=encoding)
     return split_bytes_into(clear_text_bytes, into)
 
 
+def split_io(
+    infile: BufferedReader,
+    outfiles: list[BufferedWriter],
+    *,
+    bufsize: int = 1024,
+) -> None:
+    """Split a file into multiple tokens.
+
+    Args:
+        infile: The file to be split.
+        outfiles: The files to be written.
+        bufsize: The buffer size of reading and writing.
+    """
+    output_sizes = len(outfiles)
+    for buf in iter(lambda: infile.read(bufsize), b""):
+        token_bytes = split_bytes_into(buf, output_sizes)
+        for token, outfile in zip(token_bytes, outfiles):
+            outfile.write(token)
+
+    # flush all the files
+    for outfile in outfiles:
+        outfile.flush()
+
+
 def _split1(source: bytes) -> tuple[bytes, bytes]:
     token = _generate_random_token(len(source))
     cipher_text = bytearray()
     for i in range(len(source)):
         cipher_text.append(source[i] ^ token[i])
     return bytes(token), bytes(cipher_text)
 
@@ -72,9 +97,30 @@
         tokens: The tokens to be merged.
         encoding: The encoding of the text.
     """
     clear_text_bytes = merge_bytes_into(tokens)
     return clear_text_bytes.decode(encoding)
 
 
+def merge_io(
+    infiles: list[BufferedReader],
+    outfile: BufferedWriter,
+    *,
+    bufsize: int = 1024,
+) -> None:
+    """Merge tokens into a file.
+
+    Args:
+        infiles: The files to be read.
+        outfile: The file to be written.
+    """
+    token_bytes = []
+    while True:
+        token_bytes = [infile.read(bufsize) for infile in infiles]
+        clear_text_bytes = merge_bytes_into(token_bytes)
+        if not clear_text_bytes:
+            break
+        outfile.write(clear_text_bytes)
+
+
 def _generate_random_token(size: int) -> bytes:
     return secrets.token_bytes(size)
```

### Comparing `tally-token-0.3.0/tally_token.egg-info/PKG-INFO` & `tally-token-0.3.1/tally_token.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tally-token
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library to split data into tokens
 Home-page: https://github.com/kitsuyui/python-tally-token
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -68,14 +68,28 @@
 
 You can use `merge` to merge multiple files into a file.
 
 ```sh
 $ tally-token merge merged.bin split-1.bin split-2.bin split-3.bin
 ```
 
+### Large files
+
+Nothing special. You can split and merge large file.
+
+```sh
+$ dd if=/dev/urandom of=original.1g.bin bs=1G count=1
+$ tally-token split original.1g.bin split-1.bin split-2.bin split-3.bin
+$ shasum -a 256 original.1g.bin
+> 736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965 original.1g.bin
+$ tally-token merge recovery.1g.bin split-1.bin split-2.bin split-3.bin
+$ shasum -a 256 recovery.1g.bin
+> 736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965 recovery.1g.bin
+```
+
 ## Example
 
 ### split
 
 You can use `split_text` to split text into tokens. `split_text` returns list of random bytes.
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tally-token Version: 0.3.0 Summary: A library to
+Metadata-Version: 2.1 Name: tally-token Version: 0.3.1 Summary: A library to
 split data into tokens Home-page: https://github.com/kitsuyui/python-tally-
 token Author: Yui Kitsu Author-email: kitsuyui+github@kitsuyui.com License:
 BSD-3-Clause Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: BSD License Classifier: Topic :: Security :: Cryptography
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -28,18 +28,26 @@
 {split,merge} Commands: split: split a file into multiple files merge: merge
 multiple files into a fileExample: tally-token split example.bin example.bin.1
 example.bin.2 example.bin.3 tally-token merge example-merged.bin example.bin.1
 example.bin.2 example.bin.3 options: -h, --help show this help message and exit
 ``` ### split You can use `split` to split a file into multiple files. ```sh $
 tally-token split something.bin split-1.bin split-2.bin split-3.bin ``` ###
 merge You can use `merge` to merge multiple files into a file. ```sh $ tally-
-token merge merged.bin split-1.bin split-2.bin split-3.bin ``` ## Example ###
-split You can use `split_text` to split text into tokens. `split_text` returns
-list of random bytes. ```python >>> from tally_token import split_text >>>
-split_text("Hello, World!") [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
+token merge merged.bin split-1.bin split-2.bin split-3.bin ``` ### Large files
+Nothing special. You can split and merge large file. ```sh $ dd if=/dev/urandom
+of=original.1g.bin bs=1G count=1 $ tally-token split original.1g.bin split-
+1.bin split-2.bin split-3.bin $ shasum -a 256 original.1g.bin >
+736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965
+original.1g.bin $ tally-token merge recovery.1g.bin split-1.bin split-2.bin
+split-3.bin $ shasum -a 256 recovery.1g.bin >
+736a344d99d27e2dcdab8bc37ca94c83eda26f812a3dee87ac98989f89b3f965
+recovery.1g.bin ``` ## Example ### split You can use `split_text` to split text
+into tokens. `split_text` returns list of random bytes. ```python >>> from
+tally_token import split_text >>> split_text("Hello, World!")
+[b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80'] ``` ### merge You can use
 `merge_text` to merge tokens into text. `merge_text` returns cleartext.
 ```python >>> from tally_token import merge_text >>> merge_text(
 [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80']) 'Hello, World!' ``` ### split
 with custom length ```python >>> from tally_token import split_text, merge_text
 >>> split_text("Hello, World!", 5) [b'N&\xce\\\xbc6dxp\x87\xa8#z',
```

### Comparing `tally-token-0.3.0/tally_token.egg-info/SOURCES.txt` & `tally-token-0.3.1/tally_token.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tally-token-0.3.0/tests/test_basis.py` & `tally-token-0.3.1/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `tally-token-0.3.0/tests/test_cli.py` & `tally-token-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

