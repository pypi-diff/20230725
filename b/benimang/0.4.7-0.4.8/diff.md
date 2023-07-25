# Comparing `tmp/benimang-0.4.7.tar.gz` & `tmp/benimang-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benimang-0.4.7.tar", last modified: Mon Jul 24 06:34:29 2023, max compression
+gzip compressed data, was "benimang-0.4.8.tar", last modified: Tue Jul 25 08:34:07 2023, max compression
```

## Comparing `benimang-0.4.7.tar` & `benimang-0.4.8.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 06:34:29.204159 benimang-0.4.7/
--rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0      237 2023-07-24 06:34:29.203158 benimang-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 06:34:29.199158 benimang-0.4.7/beni/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/__init__.py
--rw-rw-rw-   0        0        0     6505 2023-07-20 01:41:22.000000 benimang-0.4.7/beni/bbyte.py
--rw-rw-rw-   0        0        0     6313 2023-07-24 06:29:19.000000 benimang-0.4.7/beni/bcache.py
--rw-rw-rw-   0        0        0     1906 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bcolor.py
--rw-rw-rw-   0        0        0     2460 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bexecute.py
--rw-rw-rw-   0        0        0     2762 2023-07-24 06:21:16.000000 benimang-0.4.7/beni/bfile.py
--rw-rw-rw-   0        0        0     5047 2023-07-20 03:23:07.000000 benimang-0.4.7/beni/bfunc.py
--rw-rw-rw-   0        0        0     5855 2023-07-22 08:10:55.000000 benimang-0.4.7/beni/bhttp.py
--rw-rw-rw-   0        0        0     2347 2023-07-20 02:15:15.000000 benimang-0.4.7/beni/binput.py
--rw-rw-rw-   0        0        0     5663 2023-07-20 03:23:14.000000 benimang-0.4.7/beni/block.py
--rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.7/beni/blog.py
--rw-rw-rw-   0        0        0     5664 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bpath.py
--rw-rw-rw-   0        0        0     2418 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bplaywright.py
--rw-rw-rw-   0        0        0     1086 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bprogress.py
--rw-rw-rw-   0        0        0     3845 2023-07-20 03:24:05.000000 benimang-0.4.7/beni/bqiniu.py
--rw-rw-rw-   0        0        0    10523 2023-07-20 01:45:35.000000 benimang-0.4.7/beni/bsqlite.py
--rw-rw-rw-   0        0        0      859 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/bstorage.py
--rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.7/beni/btable.py
--rw-rw-rw-   0        0        0     4705 2023-07-22 09:41:51.000000 benimang-0.4.7/beni/btask.py
--rw-rw-rw-   0        0        0     1574 2023-07-22 06:33:25.000000 benimang-0.4.7/beni/btime.py
--rw-rw-rw-   0        0        0      390 2023-07-20 02:53:02.000000 benimang-0.4.7/beni/btype.py
--rw-rw-rw-   0        0        0     2391 2023-07-20 02:15:15.000000 benimang-0.4.7/beni/bzip.py
-drwxrwxrwx   0        0        0        0 2023-07-24 06:34:29.202159 benimang-0.4.7/benimang.egg-info/
--rw-rw-rw-   0        0        0      237 2023-07-24 06:34:29.000000 benimang-0.4.7/benimang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-07-24 06:34:29.000000 benimang-0.4.7/benimang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 06:34:29.000000 benimang-0.4.7/benimang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-24 06:34:29.000000 benimang-0.4.7/benimang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      346 2023-07-24 06:30:49.000000 benimang-0.4.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-24 06:34:29.204159 benimang-0.4.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 08:34:07.046455 benimang-0.4.8/
+-rw-rw-rw-   0        0        0       29 2023-07-19 08:32:47.000000 benimang-0.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      237 2023-07-25 08:34:07.046455 benimang-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 08:34:07.041453 benimang-0.4.8/beni/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:32:47.000000 benimang-0.4.8/beni/__init__.py
+-rw-rw-rw-   0        0        0     6556 2023-07-25 07:39:02.000000 benimang-0.4.8/beni/bbyte.py
+-rw-rw-rw-   0        0        0     1866 2023-07-25 06:18:05.000000 benimang-0.4.8/beni/bcache.py
+-rw-rw-rw-   0        0        0     1816 2023-07-25 06:21:32.000000 benimang-0.4.8/beni/bcolor.py
+-rw-rw-rw-   0        0        0      436 2023-07-25 06:23:25.000000 benimang-0.4.8/beni/bdefine.py
+-rw-rw-rw-   0        0        0     1600 2023-07-25 07:11:17.000000 benimang-0.4.8/beni/bexecute.py
+-rw-rw-rw-   0        0        0     2661 2023-07-25 06:34:46.000000 benimang-0.4.8/beni/bfile.py
+-rw-rw-rw-   0        0        0     5090 2023-07-25 07:47:04.000000 benimang-0.4.8/beni/bfunc.py
+-rw-rw-rw-   0        0        0     5752 2023-07-25 07:01:09.000000 benimang-0.4.8/beni/bhttp.py
+-rw-rw-rw-   0        0        0     2242 2023-07-25 06:54:08.000000 benimang-0.4.8/beni/binput.py
+-rw-rw-rw-   0        0        0     5672 2023-07-25 07:25:27.000000 benimang-0.4.8/beni/block.py
+-rw-rw-rw-   0        0        0     4175 2023-07-20 02:15:15.000000 benimang-0.4.8/beni/blog.py
+-rw-rw-rw-   0        0        0     5413 2023-07-25 07:16:01.000000 benimang-0.4.8/beni/bpath.py
+-rw-rw-rw-   0        0        0     2415 2023-07-25 07:11:21.000000 benimang-0.4.8/beni/bplaywright.py
+-rw-rw-rw-   0        0        0     1083 2023-07-25 07:01:09.000000 benimang-0.4.8/beni/bprogress.py
+-rw-rw-rw-   0        0        0     3813 2023-07-25 07:15:16.000000 benimang-0.4.8/beni/bqiniu.py
+-rw-rw-rw-   0        0        0    10447 2023-07-25 08:21:55.000000 benimang-0.4.8/beni/bsqlite.py
+-rw-rw-rw-   0        0        0     3990 2023-07-25 08:13:07.000000 benimang-0.4.8/beni/bstore.py
+-rw-rw-rw-   0        0        0     1974 2023-07-19 08:32:47.000000 benimang-0.4.8/beni/btable.py
+-rw-rw-rw-   0        0        0     4705 2023-07-22 09:41:51.000000 benimang-0.4.8/beni/btask.py
+-rw-rw-rw-   0        0        0     1380 2023-07-25 07:06:47.000000 benimang-0.4.8/beni/btime.py
+-rw-rw-rw-   0        0        0      436 2023-07-25 02:06:35.000000 benimang-0.4.8/beni/btype.py
+-rw-rw-rw-   0        0        0     2366 2023-07-25 02:09:39.000000 benimang-0.4.8/beni/bzip.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:34:07.044454 benimang-0.4.8/benimang.egg-info/
+-rw-rw-rw-   0        0        0      237 2023-07-25 08:34:07.000000 benimang-0.4.8/benimang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2023-07-25 08:34:07.000000 benimang-0.4.8/benimang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:34:07.000000 benimang-0.4.8/benimang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-25 08:34:07.000000 benimang-0.4.8/benimang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      346 2023-07-25 08:33:37.000000 benimang-0.4.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:34:07.047455 benimang-0.4.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 08:34:07.045454 benimang-0.4.8/test/
+-rw-rw-rw-   0        0        0      398 2023-07-25 07:46:56.000000 benimang-0.4.8/test/test_bbyte.py
```

### Comparing `benimang-0.4.7/beni/bbyte.py` & `benimang-0.4.8/beni/bbyte.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,42 +7,42 @@
 def decode(value: bytes):
     import chardet
     data = chardet.detect(value)
     encoding = data['encoding'] or 'utf8'
     return value.decode(encoding)
 
 
-EndianType = Literal[
+_EndianType = Literal[
     # https://docs.python.org/zh-cn/3/library/struct.html#byte-order-size-and-alignment
     '@',  # 按原字节
     '=',  # 按原字节
     '<',  # 小端
     '>',  # 大端
     '!',  # 网络（=大端）
 ]
 
 
 class BytesWriter():
 
-    def __init__(self, endian: EndianType):
+    def __init__(self, endian: _EndianType):
         self.endian = endian
-        self.formatAry: list[str] = []
-        self.valueAry: list[Any] = []
+        self.formats: list[str] = []
+        self.values: list[Any] = []
 
     def toBytes(self):
         return struct.pack(
-            f'{self.endian}{"".join(self.formatAry)}',
-            *self.valueAry
+            f'{self.endian}{"".join(self.formats)}',
+            *self.values
         )
 
     def _write(self, format: str, value: int | float | bool | str | bytes):
-        self.formatAry.append(format)
-        self.valueAry.append(value)
+        self.formats.append(format)
+        self.values.append(value)
 
-    def _writeAry(self, func: Any, ary: list[Any]):
+    def _writeList(self, func: Any, ary: list[Any]):
         self.writeUint(len(ary))
         for value in ary:
             func(value)
         return self
 
     # ---------------------------------------------------------------------------
 
@@ -93,67 +93,67 @@
         count = len(valueBytes)
         self.writeUshort(count)
         self._write(f'{count}s', valueBytes)
         return self
 
     # ---------------------------------------------------------------------------
 
-    def writeAryShort(self, ary: list[int]):
+    def writeListShort(self, ary: list[int]):
         'int16[]'
-        return self._writeAry(self.writeShort, ary)
+        return self._writeList(self.writeShort, ary)
 
-    def writeAryUshort(self, ary: list[int]):
+    def writeListUshort(self, ary: list[int]):
         'int16[]'
-        return self._writeAry(self.writeUshort, ary)
+        return self._writeList(self.writeUshort, ary)
 
-    def writeAryInt(self, ary: list[int]):
+    def writeListInt(self, ary: list[int]):
         'int32[]'
-        return self._writeAry(self.writeInt, ary)
+        return self._writeList(self.writeInt, ary)
 
-    def writeAryUint(self, ary: list[int]):
+    def writeListUint(self, ary: list[int]):
         'int32[]'
-        return self._writeAry(self.writeUint, ary)
+        return self._writeList(self.writeUint, ary)
 
-    def writeAryLong(self, ary: list[int]):
+    def writeListLong(self, ary: list[int]):
         'int64[]'
-        return self._writeAry(self.writeLong, ary)
+        return self._writeList(self.writeLong, ary)
 
-    def writeAryUlong(self, ary: list[int]):
+    def writeListUlong(self, ary: list[int]):
         'int64[]'
-        return self._writeAry(self.writeUlong, ary)
+        return self._writeList(self.writeUlong, ary)
 
-    def writeAryFloat(self, ary: list[float]):
-        return self._writeAry(self.writeFloat, ary)
+    def writeListFloat(self, ary: list[float]):
+        return self._writeList(self.writeFloat, ary)
 
-    def writeAryDouble(self, ary: list[float]):
-        return self._writeAry(self.writeDouble, ary)
+    def writeListDouble(self, ary: list[float]):
+        return self._writeList(self.writeDouble, ary)
 
-    def writeAryBool(self, ary: list[bool]):
-        return self._writeAry(self.writeBool, ary)
+    def writeListBool(self, ary: list[bool]):
+        return self._writeList(self.writeBool, ary)
 
-    def writeAryStr(self, ary: list[str]):
-        return self._writeAry(self.writeStr, ary)
+    def writeListStr(self, ary: list[str]):
+        return self._writeList(self.writeStr, ary)
 
 
 class BytesReader():
 
     offset: int
     data: bytes
 
-    def __init__(self, endian: EndianType, data: bytes):
+    def __init__(self, endian: _EndianType, data: bytes):
         self.endian = endian
         self.offset = 0
         self.data = data
 
     def _read(self, fmt: str):
-        result = struct.unpack_from(fmt, self.data, self.offset)[0]
+        result = struct.unpack_from(f'{self.endian}{fmt}', self.data, self.offset)[0]
         self.offset += struct.calcsize(fmt)
         return result
 
-    def _readAry(self, func: Any):
+    def _readList(self, func: Any):
         ary: list[Any] = []
         count = self.readUint()
         for _ in range(count):
             ary.append(func())
         return ary
 
     # ---------------------------------------------------------------------------
@@ -193,42 +193,42 @@
 
     def readStr(self):
         count = self.readUshort()
         return cast(str, self._read(f'{count}s').decode())
 
     # ---------------------------------------------------------------------------
 
-    def readAryShort(self):
+    def readListShort(self):
         'int16[]'
-        return cast(list[int], self._readAry(self.readShort))
+        return cast(list[int], self._readList(self.readShort))
 
-    def readAryUshort(self):
+    def readListUshort(self):
         'int16[]'
-        return cast(list[int], self._readAry(self.readUshort))
+        return cast(list[int], self._readList(self.readUshort))
 
-    def readAryInt(self):
+    def readListInt(self):
         'int32[]'
-        return cast(list[int], self._readAry(self.readInt))
+        return cast(list[int], self._readList(self.readInt))
 
-    def readAryUint(self):
+    def readListUint(self):
         'int32[]'
-        return cast(list[int], self._readAry(self.readUint))
+        return cast(list[int], self._readList(self.readUint))
 
-    def readAryLong(self):
+    def readListLong(self):
         'int64[]'
-        return cast(list[int], self._readAry(self.readLong))
+        return cast(list[int], self._readList(self.readLong))
 
-    def readAryUlong(self):
+    def readListUlong(self):
         'int64[]'
-        return cast(list[int], self._readAry(self.readUlong))
+        return cast(list[int], self._readList(self.readUlong))
 
-    def readAryFloat(self):
-        return cast(list[float], self._readAry(self.readFloat))
+    def readListFloat(self):
+        return cast(list[float], self._readList(self.readFloat))
 
-    def readAryDouble(self):
-        return cast(list[float], self._readAry(self.readDouble))
+    def readListDouble(self):
+        return cast(list[float], self._readList(self.readDouble))
 
-    def readAryBool(self):
-        return cast(list[bool], self._readAry(self.readBool))
+    def readListBool(self):
+        return cast(list[bool], self._readList(self.readBool))
 
-    def readAryStr(self):
-        return cast(list[str], self._readAry(self.readStr))
+    def readListStr(self):
+        return cast(list[str], self._readList(self.readStr))
```

### Comparing `benimang-0.4.7/beni/bcolor.py` & `benimang-0.4.8/beni/bcolor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 import sys
 from typing import IO, Any
 
 from colorama import Fore, Style, init
 
-_isInited = False
+init()
 
-if not _isInited:
-    _isInited = True
-    init()
 
-
-def printx(*values: Any, sep: str = ' ', end: str = '\n', file: IO[str] = sys.stdout, flush: bool = False, colorList: list[Any] | None):
+def printx(*values: Any, sep: str = ' ', end: str = '\n', file: IO[str] = sys.stdout, flush: bool = False, colors: list[Any] | None):
     '''color 数组参数 colorama.Fore / colorama.Back / colorama.Style 的常量'''
-    if colorList:
-        set(*colorList)
+    if colors:
+        set(*colors)
     print(*values, sep=sep, end=end, file=file, flush=flush)
     clear()
 
 
-def getStr(value: Any, *colorList: Any):
-    if colorList:
-        value = ''.join(colorList) + str(value) + Style.RESET_ALL
+def getStr(value: Any, *colors: Any):
+    if colors:
+        value = ''.join(colors) + str(value) + Style.RESET_ALL
     return value
 
 
-def set(*colorList: Any):
-    content = ''.join(colorList)
+def set(*colors: Any):
+    content = ''.join(colors)
     if content:
         sys.stdout.write(content)
         sys.stderr.write(content)
 
 
 def clear():
     sys.stdout.write(Style.RESET_ALL)
```

### Comparing `benimang-0.4.7/beni/bexecute.py` & `benimang-0.4.8/beni/bexecute.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
-from pathlib import Path
 from typing import Any
 
 from beni import bbyte, bpath
+from beni.btype import XPath
 
 
-async def winscp(winscp_exe: Path | str, key_file: str, server: str, cmd_list: list[str], show_cmd: bool = True):
-    logFile = bpath.getUser('executeWinScp.log')
+async def winscp(winscp_exe: XPath, key_file: str, server: str, cmd_list: list[str], show_cmd: bool = True):
+    logFile = bpath.user('executeWinScp.log')
     await bpath.remove(logFile)
     ary = [
         'option batch abort',
         'option transfer binary',
         f'open sftp://{server} -privatekey={key_file} -hostkey=*',
     ]
     ary += cmd_list
@@ -21,15 +21,15 @@
     # /console
     cmd = f'{winscp_exe} /log={logFile} /loglevel=0 /command ' + ' '.join("%s" % x for x in ary)
     if show_cmd:
         print(cmd)
     return await run(cmd)
 
 
-async def runTry(*args: Any, output: str = '', error: str = ''):
+async def runExpect(*args: Any, output: str = '', error: str = ''):
     outputBytes, errorBytes, _ = await runQuiet(*args)
     if output and output not in bbyte.decode(outputBytes):
         raise Exception(f'命令执行失败: {" ".join([str(x) for x in args])}')
     if error and error not in bbyte.decode(errorBytes):
         raise Exception(f'命令执行失败: {" ".join([str(x) for x in args])}')
 
 
@@ -44,32 +44,7 @@
 
 async def run(*args: Any):
     proc = await asyncio.create_subprocess_shell(
         ' '.join([str(x) for x in args]),
     )
     await proc.communicate()
     return proc.returncode or 0
-
-# -------------------------------------------------------
-
-# def execute(*pars: str, show_cmd: bool = True, show_output: bool = False, ignore_error: bool = False):
-#     cmd = ' '.join(pars)
-#     if show_cmd:
-#         info(cmd)
-#     p = subprocess.Popen(
-#         cmd,
-#         shell=True,
-#         stdout=subprocess.PIPE,
-#         stderr=subprocess.PIPE,
-#     )
-#     outBytes, errBytes = p.communicate()
-#     p.kill()
-#     if show_output:
-#         outStr = decode(outBytes).replace('\r\n', '\n')
-#         errStr = decode(errBytes).replace('\r\n', '\n')
-#         if outStr:
-#             info(f'output:\n{outStr}')
-#         if errStr:
-#             info(f'error:\n{errStr}')
-#     if not ignore_error and p.returncode != 0:
-#         raise Exception('执行命令出错')
-#     return p.returncode, outBytes, errBytes
```

### Comparing `benimang-0.4.7/beni/bfile.py` & `benimang-0.4.8/beni/bfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,91 @@
+import tomllib
+import orjson
+import json
+import yaml
 import os
+import pickle
 from pathlib import Path
 from typing import Any
 
 import aiofiles
 
-from beni import bcolor, bfile, bfunc, block, bpath
-from beni.btype import Null
+from beni import bcolor, bfile, bfunc, bpath
+from beni.btype import Null, XPath
 
-_limit = 50
 
-
-@block.useLimit(_limit)
-async def writeText(file: Path | str, content: str, encoding: str = 'utf8', newline: str = '\n'):
+async def writeText(file: XPath, content: str, encoding: str = 'utf8', newline: str = '\n'):
     file = bpath.get(file)
     await bpath.make(file.parent)
     async with aiofiles.open(file, 'w', encoding=encoding, newline=newline) as f:
         return await f.write(content)
 
 
-@block.useLimit(_limit)
-async def writeBytes(file: Path | str, data: bytes):
+async def writeBytes(file: XPath, data: bytes):
     file = bpath.get(file)
     await bpath.make(file.parent)
     async with aiofiles.open(file, 'wb') as f:
         return await f.write(data)
 
 
-@block.useLimit(_limit)
-async def writeYaml(file: Path | str, data: Any):
-    import yaml
+async def writeYaml(file: XPath, data: Any):
     await writeText(file, yaml.safe_dump(data))
 
 
-@block.useLimit(_limit)
-async def writeJson(file: Path | str, data: Any, mini: bool = True):
+async def writeJson(file: XPath, data: Any, mini: bool = True):
     if mini:
-        await writeText(file, bfunc.jsonDumpsMini(data))
+        content = bfunc.jsonDumpsMini(data)
     else:
-        import json
-        await writeText(file, json.dumps(data, ensure_ascii=False, sort_keys=True, indent=4))
+        content = json.dumps(data, ensure_ascii=False, sort_keys=True, indent=4)
+    await writeText(file, content)
+
 
+async def writePickle(file: XPath, data: Any):
+    await writeBytes(file, pickle.dumps(data))
 
-@block.useLimit(_limit)
-async def readText(file: Path | str, encoding: str = 'utf8', newline: str = '\n'):
+
+async def readText(file: XPath, encoding: str = 'utf8', newline: str = '\n'):
     async with aiofiles.open(file, 'r', encoding=encoding, newline=newline) as f:
         return await f.read()
 
 
-@block.useLimit(_limit)
-async def readBytes(file: Path | str):
+async def readBytes(file: XPath):
     async with aiofiles.open(file, 'rb') as f:
         return await f.read()
 
 
-@block.useLimit(_limit)
-async def readYaml(file: Path | str):
-    import yaml
+async def readYaml(file: XPath):
     return yaml.safe_load(
         await readText(file)
     )
 
 
-@block.useLimit(_limit)
-async def readJson(file: Path | str):
-    import orjson
+async def readJson(file: XPath):
     return orjson.loads(await readBytes(file))
 
 
-@block.useLimit(_limit)
-async def readToml(file: Path | str):
-    import tomllib
+async def readPickle(file: XPath):
+    return pickle.loads(
+        await readBytes(file)
+    )
+
+
+async def readToml(file: XPath):
     return tomllib.loads(
         await readText(file)
     )
 
 
-async def md5(file: Path | str):
+async def md5(file: XPath):
     return bfunc.md5Bytes(
         await readBytes(file)
     )
 
 
-async def crc(file: Path | str):
+async def crc(file: XPath):
     return bfunc.crcBytes(
         await readBytes(file)
     )
 
 
 async def makeFiles(content: str, output: Path = Null):
     if output is Null:
@@ -96,10 +96,11 @@
     ary.sort()
     for substr in ary:
         subAry = substr.replace('\r\n', '\n').split('\n')
         fileName = subAry.pop(0)
         if subAry:
             file = output / fileName
             bcolor.printYellow(file)
-            msg = '\n'.join(subAry).strip()
-            if msg:
-                await bfile.writeText(file, msg)
+            await bfile.writeText(
+                file,
+                '\n'.join(subAry).strip(),
+            )
```

### Comparing `benimang-0.4.7/beni/bfunc.py` & `benimang-0.4.8/beni/bfunc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 import asyncio
 import binascii
 import hashlib
 import json
 import os
+import pickle
 import random
 import sys
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import asynccontextmanager
 from functools import wraps
-from pathlib import Path
 from typing import Any, Callable, Coroutine, cast
 
 import async_timeout
 
-from beni.btype import AnyType, AsyncFuncType, IfsType, FuncType
+from beni.btype import AnyType, AsyncFuncType, FuncType, IfsType, Null, XPath
 
 
 def jsonDumpsMini(value: Any):
     return json.dumps(value, ensure_ascii=False, sort_keys=True, separators=(',', ':'))
 
 
 def md5Bytes(data: bytes):
     return hashlib.md5(data).hexdigest()
 
 
 def md5Str(content: str):
-    return md5Bytes(content.encode())
+    return md5Bytes(
+        content.encode()
+    )
 
 
 def md5Data(data: Any):
-    return md5Str(
-        jsonDumpsMini(data)
+    return md5Bytes(
+        pickle.dumps(data)
     )
 
 
 def crcBytes(data: bytes):
     return hex(binascii.crc32(data))[2:].zfill(8)
 
 
 def crcStr(content: str):
-    return crcBytes(content.encode())
+    return crcBytes(
+        content.encode()
+    )
 
 
 def crcData(data: Any):
-    return crcStr(
-        jsonDumpsMini(data)
+    return crcBytes(
+        pickle.dumps(data)
     )
 
 
 def sysUtf8():
     if sys.platform == 'win32':
         os.system('chcp 65001')
 
 
-def addEnvPath(p: Path | str):
+def addEnvPath(path: XPath):
     value = os.getenv('path') or ''
-    value = ';'.join([value, str(p)])
+    value = ';'.join([value, str(path)])
     os.putenv('path', value)
 
 
 def makeValidateCode(length: int):
     minValue = 10 ** (length - 1)
     maxValue = int('9' * length)
     return str(random.randrange(minValue, maxValue))
@@ -69,17 +73,15 @@
     '包括最小值和最大值'
     value = min(value, maxValue)
     value = max(value, minValue)
     return value
 
 
 def getPercentValue(targetValue: float, minValue: float, maxValue: float, minResult: float, maxResult: float):
-    '''
-    根据百分之计算指定数值
-    '''
+    '根据百分之计算指定数值'
     if targetValue >= maxValue:
         return maxResult
     elif targetValue <= minValue:
         return minResult
     else:
         percent = (targetValue - minValue) / (maxValue - minValue)
         return minResult + (maxResult - minResult) * percent
@@ -103,64 +105,68 @@
     try:
         result = int(value)
     except:
         pass
     return result
 
 
+def toAny(value: Any):
+    return cast(Any, value)
+
+
 def getSqlPlacement(ary: list[Any] | set[Any]):
     return '(' + ','.join(['?' for _ in range(len(ary))]) + ')'
 
 
 def getWrapped(data: Any):
     result = data
     while hasattr(result, '__wrapped__'):
         result = getattr(result, '__wrapped__')
     return result
 
 
 def retry(times: int):
-    def fun(func: AsyncFuncType) -> AsyncFuncType:
+    def func(func: AsyncFuncType) -> AsyncFuncType:
         @wraps(func)
         async def wrapper(*args: Any, **kwargs: Any):
             current = 0
             while True:
                 try:
                     return await func(*args, **kwargs)
                 except:
                     current += 1
                     if current >= times:
                         raise
-        return cast(AsyncFuncType, wrapper)
-    return fun
+        return toAny(wrapper)
+    return func
 
 
 @asynccontextmanager
 async def timeout(timeout: float):
     async with async_timeout.timeout(timeout):
         yield
 
 
 def syncCall(func: Callable[..., Coroutine[Any, Any, AnyType]]) -> Callable[..., AnyType]:
     @wraps(func)
     def wraper(*args: Any, **kwargs: Any):
         return asyncio.run(func(*args, **kwargs))
-    return cast(Any, wraper)
+    return toAny(wraper)
 
 
 _onceCallSet: set[int] = set()
 
 
 def onceCall(func: FuncType) -> Callable[..., FuncType]:
     @wraps(func)
     def wraper(*args: Any, **kwargs: Any):
         assert id(func) not in _onceCallSet, f'函数 {func.__module__}.{func.__name__} 只能调用一次'
         _onceCallSet.add(id(func))
         return func(*args, **kwargs)
-    return cast(Any, wraper)
+    return toAny(wraper)
 
 
 def initErrorFormat():
     import pretty_errors
     pretty_errors.configure(
         separator_character='*',
         filename_display=pretty_errors.FILENAME_COMPACT,
@@ -180,24 +186,24 @@
     def _(v: int = 1):
         nonlocal value
         value += v
         return value
     return _
 
 
-_threadPoolExector: ThreadPoolExecutor | None = None
+_threadPoolExector: ThreadPoolExecutor = Null
 _threadMaxNum: int = 4
 
 
 def setThreadMaxNum(value: int):
     global _threadPoolExector, _threadMaxNum
     if not _threadPoolExector:
         _threadMaxNum = value
     else:
         raise Exception('ThreadPoolExector实例化之后不能再设置maxWorkers')
 
 
-async def runInThread(lambdaFunc: Callable[..., AnyType]) -> AnyType:
+async def runThread(lambdaFunc: Callable[..., AnyType]) -> AnyType:
     global _threadPoolExector
     if _threadPoolExector is None:
         _threadPoolExector = ThreadPoolExecutor(max_workers=_threadMaxNum)
     return await asyncio.get_running_loop().run_in_executor(_threadPoolExector, lambdaFunc)
```

### Comparing `benimang-0.4.7/beni/bhttp.py` & `benimang-0.4.8/beni/bhttp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import asyncio
 from http.cookiejar import CookieJar
-from pathlib import Path
 from typing import Any, Final
 from urllib.parse import urlencode
 from urllib.request import HTTPCookieProcessor, build_opener, install_opener
 
 import aiofiles
 import aiohttp
 import orjson
 
 from beni import block, bpath
+from beni.btype import Null, XPath
 
 _limit: Final = 5
-_defaultRetry = 3
-
-_httpHeaders = {
+_retry = 3
+_headers = {
     'Connection': 'keep-alive',
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/76.0.3809.100 Safari/537.36',
     'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8',
     'Accept-Encoding': 'gzip',
     'Accept-Language': 'zh-CN,zh;q=0.8',
 }
 
 
 def _makeHttpHeaders(headers: dict[str, Any] | None = None):
     if headers:
-        return _httpHeaders | headers
+        return _headers | headers
     else:
-        return dict(_httpHeaders)
+        return dict(_headers)
 
 
-@block.useLimit(_limit)
+@block.limit(_limit)
 async def get(
     url: str,
     *,
-    headers: dict[str, Any] | None = None,
+    headers: dict[str, Any] = Null,
     timeout: int = 10,
-    retry: int | None = None,
+    retry: int = Null,
 ):
-    retry = retry or _defaultRetry
+    retry = retry or _retry
     while True:
         retry -= 1
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.get(url, headers=_makeHttpHeaders(headers), timeout=timeout) as response:
                     result = await response.read()
                     if not result:
@@ -53,59 +52,59 @@
             if retry <= 0:
                 raise
 
 
 async def getBytes(
     url: str,
     *,
-    headers: dict[str, Any] | None = None,
+    headers: dict[str, Any] = Null,
     timeout: int = 10,
-    retry: int | None = None,
+    retry: int = Null,
 ):
     resultBytes, _ = await get(
         url,
         headers=headers,
         timeout=timeout,
         retry=retry,
     )
     return resultBytes
 
 
 async def getStr(
     url: str,
     *,
-    headers: dict[str, Any] | None = None,
+    headers: dict[str, Any] = Null,
     timeout: int = 10,
-    retry: int | None = None,
+    retry: int = Null,
 ):
     result = await getBytes(url, headers=headers, timeout=timeout, retry=retry)
     return result.decode()
 
 
 async def getJson(
     url: str,
     *,
-    headers: dict[str, Any] | None = None,
+    headers: dict[str, Any] = Null,
     timeout: int = 10,
-    retry: int | None = None,
+    retry: int = Null,
 ):
     result = await getBytes(url, headers=headers, timeout=timeout, retry=retry)
     return orjson.loads(result)
 
 
-@block.useLimit(_limit)
+@block.limit(_limit)
 async def post(
     url: str,
     *,
-    data: bytes | dict[str, Any] | None = None,
-    headers: dict[str, Any] | None = None,
+    data: bytes | dict[str, Any] = Null,
+    headers: dict[str, Any] = Null,
     timeout: int = 10,
-    retry: int | None = None,
+    retry: int = Null,
 ):
-    retry = retry or _defaultRetry
+    retry = retry or _retry
     while True:
         retry -= 1
         try:
             postData = data
             if type(data) is dict:
                 postData = urlencode(data).encode()
             async with aiohttp.ClientSession() as session:
@@ -119,73 +118,73 @@
             if retry <= 0:
                 raise
 
 
 async def postBytes(
     url: str,
     *,
-    data: bytes | dict[str, Any] | None = None,
-    headers: dict[str, Any] | None = None,
+    data: bytes | dict[str, Any] = Null,
+    headers: dict[str, Any] = Null,
     timeout: int = 10,
-    retry: int | None = None,
+    retry: int = Null,
 ):
     resultBytes, _ = await post(
         url,
         data=data,
         headers=headers,
         timeout=timeout,
         retry=retry,
     )
     return resultBytes
 
 
 async def postStr(
     url: str,
     *,
-    data: bytes | dict[str, Any] | None = None,
-    headers: dict[str, Any] | None = None,
+    data: bytes | dict[str, Any] = Null,
+    headers: dict[str, Any] = Null,
     timeout: int = 10,
-    retry: int | None = None,
+    retry: int = Null,
 ):
     return (await postBytes(
         url,
         data=data,
         headers=headers,
         timeout=timeout,
         retry=retry,
     )).decode()
 
 
 async def postJson(
     url: str,
     *,
-    data: bytes | dict[str, Any] | None = None,
-    headers: dict[str, Any] | None = None,
+    data: bytes | dict[str, Any] = Null,
+    headers: dict[str, Any] = Null,
     timeout: int = 10,
-    retry: int | None = None,
+    retry: int = Null,
 ):
     return orjson.loads(
         await postBytes(
             url,
             data=data,
             headers=headers,
             timeout=timeout,
             retry=retry,
         )
     )
 
 
-@block.useLimit(_limit)
-async def download(url: str, file: Path | str, timeout: int = 300):
+@block.limit(_limit)
+async def download(url: str, file: XPath, timeout: int = 300):
     # total_size: int = 0
     # download_size: int = 0
     try:
         file = bpath.get(file)
         async with aiohttp.ClientSession() as session:
-            async with session.get(url, headers=_httpHeaders, timeout=timeout) as response:
+            async with session.get(url, headers=_headers, timeout=timeout) as response:
                 await bpath.make(file.parent)
                 assert response.content_length, '下载内容为空'
                 # total_size = response.content_length
                 async with aiofiles.open(file, 'wb') as f:
                     while True:
                         data = await response.content.read(1024 * 1024)
                         if data:
@@ -197,16 +196,21 @@
         # assert total_size and total_size == download_size, '下载为文件不完整'
     except:
         await bpath.remove(file)
         raise
 
 
 def setDefaultRetry(value: int):
-    global _defaultRetry
-    _defaultRetry = value
+    global _retry
+    _retry = value
+
+
+def setDefaultHeaders(value: dict[str, Any]):
+    global _headers
+    _headers = value
 
 
 # Cookie
 _cookie = CookieJar()
 _cookieProc = HTTPCookieProcessor(_cookie)
 _opener = build_opener(_cookieProc)
 install_opener(_opener)
```

### Comparing `benimang-0.4.7/beni/binput.py` & `benimang-0.4.8/beni/binput.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 import getpass
 import random
 from typing import Any, Callable, Coroutine, cast
 
+import aioconsole
+
 from beni import bcolor
 
 
-async def hold(msg: str | None = None, password: bool = False, *exitvalue_list: str):
+async def hold(msg: str | None = None, isShowInput: bool = True, *exits: str):
     msg = msg or '测试暂停，输入exit可以退出'
     msg = f'{msg}: '
-    exitvalue_list = exitvalue_list or ('exit',)
+    exits = exits or ('exit',)
     while True:
-        if password:
-            inputValue = getpass.getpass(msg)
+        if isShowInput:
+
+            result = cast(str, await aioconsole.ainput(msg))
         else:
-            import aioconsole
-            inputValue = cast(str, await aioconsole.ainput(msg))
-        if (inputValue in exitvalue_list) or ('*' in exitvalue_list):
-            return inputValue
+            result = getpass.getpass(msg)
+        if (result in exits) or ('*' in exits):
+            return result
 
 
 async def confirm(msg: str = '确认', isShowInput: bool = False):
     code = f'{random.randint(1, 999):03}'
     await hold(f'{msg} [ {_getRemindMsg(code)} ]', not isShowInput, code)
 
 
 async def select(*data: tuple[str, str, str | Callable[[str], Any] | None, Callable[[str], Coroutine[Any, Any, Any]] | None]):
     '''
-    value = goSelect(
+    value = binput.select(
         ('descA', 'confirmDescA', 'quanbuqueren', __handlerA),
         ('descB', 'confirmDescB', lambda x: ..., __handlerB),
     )
     '''
     print()
     print('-' * 30)
     print()
     for msg, inputDisplay, _, _ in data:
         if inputDisplay:
             msg += f' [ {_getRemindMsg(inputDisplay)} ]'
         print(msg)
     print()
-    import aioconsole
     while True:
         value = cast(str, await aioconsole.ainput('输入选择：'))
         isMatch = False
         result = None
         for msg, inputDisplay, inputValue, handler in data:
             inputValue = inputValue or inputDisplay or msg
             if type(inputValue) is str:
@@ -58,15 +59,14 @@
                     result = await handler(value)
                     break
         if isMatch and result is not False:
             return value
 
 
 async def inputCheck(msg: str, check: Callable[[str], Any]):
-    import aioconsole
     while True:
         try:
             value = cast(str, await aioconsole.ainput(f'{msg}：'))
             if check(value):
                 return value
         except:
             pass
```

### Comparing `benimang-0.4.7/beni/block.py` & `benimang-0.4.8/beni/block.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import asyncio
 import inspect
 from contextlib import asynccontextmanager
 from functools import wraps
 from pathlib import Path
-from typing import Any, Callable, cast
+from typing import Any
 
-from beni import bfunc, binput, bpath
+from beni import binput, bpath
+from beni.bfunc import crcStr, toAny
+from beni.btype import AsyncFuncType, Func
 
 
 @asynccontextmanager
 async def useFileLock(*keys: str, timeout: float = 0, quite: bool = False):
     import portalocker
     lock_list: list[portalocker.Lock] = []
     keyfile_list: list[Path] = []
@@ -29,15 +31,15 @@
                 await bpath.remove(keyfile)
             except:
                 pass
 
 
 async def _lock_acquire(key: str, timeout: float = 0, quite: bool = False):
     '''不对外部提供，只提供给 async_keylock 方法使用'''
-    keyfile = bpath.getWorkspace(f'.lock/{bfunc.crcStr(key)}.lock')
+    keyfile = bpath.workspace(f'.lock/{crcStr(key)}.lock')
     await bpath.make(keyfile.parent)
     import portalocker
     while True:
         try:
             lock = portalocker.Lock(keyfile, timeout=timeout, fail_when_locked=timeout == 0)
             f = lock.acquire()
             f.write(key)
@@ -61,38 +63,38 @@
                 )
     return lock, keyfile
 
 
 # ------------------------------------------------------------------------------------------------------------------------
 
 
-def useLimit(limit: int = 1):
-    def wraperfun(func: bfunc.AsyncFuncType) -> bfunc.AsyncFuncType:
+def limit(value: int = 1):
+    def wraperfun(func: AsyncFuncType) -> AsyncFuncType:
         @wraps(func)
         async def wraper(*args: Any, **kwargs: Any):
             funid = id(inspect.unwrap(func))
-            if funid not in _limit_dict:
-                _limit_dict[funid] = _Limit(limit)
+            if funid not in _limitDict:
+                _limitDict[funid] = _Limit(value)
             try:
-                await _limit_dict[funid].wait()
+                await _limitDict[funid].wait()
                 return await func(*args, **kwargs)
             finally:
-                await _limit_dict[funid].release()
-        return cast(Any, wraper)
+                await _limitDict[funid].release()
+        return toAny(wraper)
     return wraperfun
 
 
-async def setLimit(func: Callable[..., Any], limit: int):
+async def setLimit(func: Func, limit: int):
     funid = id(inspect.unwrap(func))
-    if funid not in _limit_dict:
-        _limit_dict[funid] = _Limit(limit)
-    await _limit_dict[funid].set_limit(limit)
+    if funid not in _limitDict:
+        _limitDict[funid] = _Limit(limit)
+    await _limitDict[funid].set_limit(limit)
 
 
-_limit_dict: dict[int, _Limit] = {}
+_limitDict: dict[int, _Limit] = {}
 
 
 class _Limit():
 
     _queue: asyncio.Queue[Any]
     _running: int
```

### Comparing `benimang-0.4.7/beni/blog.py` & `benimang-0.4.8/beni/blog.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.7/beni/bplaywright.py` & `benimang-0.4.8/beni/bplaywright.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     if url:
         page.goto(url)
     return page
 
 
 def testStorageState():
     if _testContext:
-        _testContext.storage_state(path=bpath.getDesktop('storage_state.dat'))
+        _testContext.storage_state(path=bpath.desktop('storage_state.dat'))
 
 
 @asynccontextmanager
 async def page(
     *,
     browser: dict[str, Any] = {},
     context: dict[str, Any] = {},
```

### Comparing `benimang-0.4.7/beni/bprogress.py` & `benimang-0.4.8/beni/bprogress.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     # 示例
     # await bprogress.run(
     #     [myfun() for _ in range(100)],
     #     10,
     # )
     print()
     with tqdm(total=len(taskList), ncols=70) as progress:
-        @block.useLimit(itemLimit)
+        @block.limit(itemLimit)
         async def task(x: Coroutine[Any, Any, _ReturnType]):
             result = await x
             progress.update()
             return result
         resultList = await asyncio.gather(*[task(x) for x in taskList])
     print()
     return resultList
```

### Comparing `benimang-0.4.7/beni/bqiniu.py` & `benimang-0.4.8/beni/bqiniu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from contextlib import asynccontextmanager
-from pathlib import Path
 from typing import Any, NamedTuple, Tuple, cast
 
 from qiniu import Auth, BucketManager, build_batch_delete, etag, put_file
 from qiniu.http import ResponseInfo
 
 from beni import bfunc, bhttp, bpath, bzip
+from beni.btype import XPath
 
 
 class QiniuItem(NamedTuple):
     key: str
     size: int
     qetag: str
     time: int
@@ -21,76 +21,76 @@
 class QiniuBucket():
 
     def __init__(self, bucket: str, baseUrl: str, ak: str, sk: str) -> None:
         self.q = Auth(ak, sk)
         self.bucket = bucket
         self.baseUrl = baseUrl
 
-    async def uploadFile(self, key: str, localFile: Path | str):
+    async def uploadFile(self, key: str, localFile: XPath):
         token = self.q.upload_token(self.bucket, key)
-        _, info = await bfunc.runInThread(
+        _, info = await bfunc.runThread(
             lambda: cast(Tuple[Any, ResponseInfo], put_file(token, key, localFile, version='v2'))
         )
         assert info.exception is None
         assert info.status_code == 200
 
     def getPrivateFileUrl(self, key: str):
         return self.q.private_download_url(f'{self.baseUrl}/{key}')
 
     @asynccontextmanager
     async def _downloadPrivateFile(self, key: str):
         url = self.getPrivateFileUrl(key)
         async with bpath.useTempFile() as tempFile:
-            tempFile = bpath.getTempFile()
+            tempFile = bpath.tempFile()
             await bhttp.download(url, tempFile)
             assert tempFile.exists()
             yield tempFile
 
-    async def downloadPrivateFile(self, key: str, localFile: Path | str):
+    async def downloadPrivateFile(self, key: str, localFile: XPath):
         async with self._downloadPrivateFile(key) as tempFile:
             await bpath.move(tempFile, localFile, True)
 
-    async def downloadPrivateFileUnzip(self, key: str, outputDir: Path | str):
+    async def downloadPrivateFileUnzip(self, key: str, outputDir: XPath):
         async with self._downloadPrivateFile(key) as tempFile:
-            async with bpath.useTempDir() as tempDir:
+            async with bpath.useTempPath() as tempDir:
                 await bzip.unzip(tempFile, tempDir)
                 for file in await bpath.listFile(tempDir, True):
                     toFile = bpath.changeRelative(file, tempDir, outputDir)
                     await bpath.move(file, toFile, True)
 
-    async def downloadPrivateFileSevenUnzip(self, key: str, outputDir: Path | str):
+    async def downloadPrivateFileSevenUnzip(self, key: str, outputDir: XPath):
         async with self._downloadPrivateFile(key) as tempFile:
-            async with bpath.useTempDir() as tempDir:
+            async with bpath.useTempPath() as tempDir:
                 await bzip.sevenUnzip(tempFile, tempDir)
                 for file in await bpath.listFile(tempDir, True):
                     toFile = bpath.changeRelative(file, tempDir, outputDir)
                     await bpath.move(file, toFile, True)
 
     async def getFileList(self, prefix: str, limit: int = 100) -> tuple[list[QiniuItem], str | None]:
         bucket = BucketManager(self.q)
-        result, _, _ = await bfunc.runInThread(
+        result, _, _ = await bfunc.runThread(
             lambda: cast(_FileListResult, bucket.list(self.bucket, prefix, None, limit))
         )
         assert type(result) is dict
         fileList = [QiniuItem(x['key'], x['fsize'], x['hash'], x['putTime']) for x in result['items']]
         return fileList, cast(str | None, result.get('marker', None))
 
     async def getFileListByMarker(self, marker: str, limit: int = 100):
         bucket = BucketManager(self.q)
-        result, _, _ = await bfunc.runInThread(
+        result, _, _ = await bfunc.runThread(
             lambda: cast(_FileListResult, bucket.list(self.bucket, None, marker, limit))
         )
         assert type(result) is dict
         fileList = [QiniuItem(x['key'], x['fsize'], x['hash'], x['putTime']) for x in result['items']]
         return fileList, cast(str | None, result.get('marker', None))
 
     async def deleteFiles(self, *keyList: str):
         bucket = BucketManager(self.q)
-        result, _ = await bfunc.runInThread(
+        result, _ = await bfunc.runThread(
             lambda: cast(tuple[Any, Any], bucket.batch(build_batch_delete(self.bucket, keyList)))
         )
         assert result
 
-    async def hashFile(self, file: Path | str):
-        return await bfunc.runInThread(
+    async def hashFile(self, file: XPath):
+        return await bfunc.runThread(
             lambda: etag(file)
         )
```

### Comparing `benimang-0.4.7/beni/bsqlite.py` & `benimang-0.4.8/beni/bsqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from typing import Any, Final, Sequence, cast
 
 import aiosqlite
 import orjson
 from pydantic import BaseModel
 
 from beni import block, bpath
-from beni.bfunc import getSqlPlacement
+from beni.bfunc import getSqlPlacement, toAny
+from beni.btype import Null, XPath
 
 sqlite3.register_converter(
     "bool",
     lambda x: x not in (
         b'',
         b'0',
         # None, # 如果是None根本就不会进来，这里判断也没有意义
@@ -27,15 +28,15 @@
 _ALIVE: Final = 5 * 60  # 数据库链接至少存活时间（因为清除不是实时执行）
 
 
 class SqliteDbPool:
 
     _isRunningClean = False
 
-    def __init__(self, dbFile: str | Path, maxConnections: int = 10):
+    def __init__(self, dbFile: XPath, maxConnections: int = 10):
         self._avaliableList: asyncio.Queue[_SqliteDbWrite] = asyncio.Queue()
         self.lock = block.RWLock(maxConnections)
         if type(dbFile) is Path:
             self._dbFile = dbFile
         else:
             self._dbFile = bpath.get(dbFile)
 
@@ -136,15 +137,15 @@
 
 
 class _SqliteDbRead:
 
     _db: aiosqlite.Connection
     _releaseTime = 0.0
 
-    async def connect(self, db_file: Path | str):
+    async def connect(self, db_file: XPath):
         self._db = await aiosqlite.connect(db_file, detect_types=sqlite3.PARSE_DECLTYPES)
         self._db.row_factory = sqlite3.Row
 
     async def close(self):
         await self._db.close()
 
     async def get(self, sql: str, *parameters: Any):
@@ -254,82 +255,80 @@
             result = ''.join(nameList)
             cls.__tableName__ = result
         return cls.__tableName__
 
     async def add(self):
         return await self._add()
 
-    async def _add(self, exclude: set[str] | None = None, include: set[str] | None = None):
+    async def _add(self, exclude: set[str] = Null, include: set[str] = Null):
         return await self._db.add(
             self.TableName,
             self.dict(
-                exclude=cast(Any, exclude),
-                include=cast(Any, include),
+                exclude=toAny(exclude),
+                include=toAny(include),
             )
         )
 
     @classmethod
     async def addList(cls, modelList: Sequence[SqliteDbModel]):
         return await cls._addList(modelList)
 
     @classmethod
-    async def _addList(cls, modelList: Sequence[SqliteDbModel], exclude: set[str] | None = None):
+    async def _addList(cls, modelList: Sequence[SqliteDbModel], exclude: set[str] = Null):
         if not modelList:
             return 0
         return await cls._db.addList(
             cls.TableName,
-            [x.dict(exclude=cast(Any, exclude)) for x in modelList],
+            [x.dict(exclude=toAny(exclude)) for x in modelList],
         )
 
-    async def _update(self, statement: str = '', *args: Any, exclude: set[str] | None = None, include: set[str] | None = None):
+    async def _update(self, statement: str = '', *args: Any, exclude: set[str] = Null, include: set[str] = Null):
         return await self._db.update(
             self.TableName,
             self.dict(
-                exclude=cast(Any, exclude),
-                include=cast(Any, include),
+                exclude=toAny(exclude),
+                include=toAny(include),
             ),
             statement,
             *args,
         )
 
     @classmethod
     async def removeAll(cls):
-        return await cls._db.execute(
-            f'DELETE FROM {cls.TableName}',
-        )
+        return await cls._remove()
 
     @classmethod
     async def _remove(cls, statement: str = '', *args: Any):
         return await cls._db.execute(
             f'DELETE FROM {cls.TableName} {statement}',
             *args,
         )
 
     @classmethod
-    async def _get(cls, statement: str = '', *args: Any, fields: set[str] | None = None):
+    async def _get(cls, statement: str = '', *args: Any, fields: set[str] = Null):
         row = await cls._db.get(
             f'''
-            SELECT
-                {fields and ', '.join(fields) or '*'}
+            SELECT                
+                {', '.join(fields) if fields else '*'}
             FROM
                 `{cls.TableName}`
             {statement}
             LIMIT 1
             ''',
             *args,
         )
         if row:
             return cls(**dict(row))
 
     @classmethod
-    async def _getList(cls, statement: str = '', *args: Any, fields: set[str] | None = None):
+    async def _getList(cls, statement: str = '', *args: Any, fields: set[str] = Null):
         rowList = await cls._db.getList(
             f'''
             SELECT
-                {fields and ', '.join(fields) or '*'}
+                {', '.join(fields) if fields else '*'}
             FROM
                 `{cls.TableName}`
             {statement}
             ''',
             *args,
         )
         return [cls(**dict(x)) for x in rowList]
```

### Comparing `benimang-0.4.7/beni/btable.py` & `benimang-0.4.8/beni/btable.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.7/beni/btask.py` & `benimang-0.4.8/beni/btask.py`

 * *Files identical despite different names*

### Comparing `benimang-0.4.7/beni/btime.py` & `benimang-0.4.8/beni/btime.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,18 +57,7 @@
 
 def makeDatetime(date_str: str, fmt: str = r'%Y-%m-%d %H:%M:%S'):
     return xdatetime.datetime.strptime(date_str, fmt)
 
 
 def makeDate(date_str: str, fmt: str = r'%Y-%m-%d'):
     return xdatetime.datetime.strptime(date_str, fmt).date()
-
-
-# def tomorrowDatetime():
-#     return datetime.datetime.combine(
-#         nowDate(),
-#         datetime.time(),
-#     )
-
-
-# def foreverDatetime():
-#     return datetime.datetime(9999, 1, 1)
```

### Comparing `benimang-0.4.7/beni/bzip.py` & `benimang-0.4.8/beni/bzip.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from pathlib import Path
 from typing import Any, Callable
 from zipfile import ZIP_DEFLATED, ZipFile
 
 from beni import bexecute, bpath
+from beni.btype import XPath
 
 
 async def _zip(zfile: Path, path_dict: dict[str, Path]):
     await bpath.make(zfile.parent)
     with ZipFile(zfile, 'w', ZIP_DEFLATED) as f:
         for fname in sorted(path_dict.keys()):
             file = path_dict[fname]
             if file.is_file():
                 f.write(file, fname)
 
 
-async def zipFile(zfile: Path | str, targetFile: Path | str, name: str | None = None):
+async def zipFile(zfile: XPath, targetFile: XPath, name: str | None = None):
     zfile = bpath.get(zfile)
     targetFile = bpath.get(targetFile)
     if name is None:
         name = targetFile.name
     await _zip(zfile, {name: targetFile})
 
 
-async def zipFolder(zfile: Path | str, targetDir: Path | str, filterFunc: Callable[[Path], bool] | None = None):
+async def zipFolder(zfile: XPath, targetDir: XPath, filterFunc: Callable[[Path], bool] | None = None):
     zfile = bpath.get(zfile)
     targetDir = bpath.get(targetDir)
     ary = await bpath.listPath(targetDir, True)
     if filterFunc:
         ary = list(filter(filterFunc, ary))
     await _zip(zfile, {str(x.relative_to(targetDir)): x for x in ary})
 
 
-async def unzip(file: Path | str, outputDir: Path | str | None = None):
+async def unzip(file: XPath, outputDir: XPath | None = None):
     file = bpath.get(file)
     outputDir = outputDir or file.parent
     with ZipFile(file) as f:
         for subFile in sorted(f.namelist()):
             try:
                 # zipfile 代码中指定了cp437，这里会导致中文乱码
                 encodeSubFile = subFile.encode('cp437').decode('gbk')
@@ -44,23 +45,23 @@
             f.extract(subFile, outputDir)
             # 处理压缩包中的中文文件名在windows下乱码
             if subFile != encodeSubFile:
                 toFile = bpath.get(outputDir, encodeSubFile)
                 bpath.get(outputDir, subFile).rename(toFile)
 
 
-async def sevenZip(zfile: Path | str, target: Path | str):
+async def sevenZip(zfile: XPath, target: XPath):
     await _runSeven('a', zfile, target)
 
 
-async def sevenUnzip(zfile: Path | str, output: Path | str):
+async def sevenUnzip(zfile: XPath, output: XPath):
     await _runSeven('x', f'-o{output}', zfile)
 
 
-async def sevenRename(zfile: Path | str, fromName: str, toName: str):
+async def sevenRename(zfile: XPath, fromName: str, toName: str):
     await _runSeven('rn', zfile, fromName, toName)
 
 
 async def _runSeven(*args: Any):
     resultBytes, errorBytes, _ = await bexecute.runQuiet('7zr', *args)
     assert not errorBytes, errorBytes.decode('gbk')
     assert b'Everything is Ok' in resultBytes, resultBytes.decode('gbk')
```

