# Comparing `tmp/mystbin_py-6.0.0.tar.gz` & `tmp/mystbin_py-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystbin_py-6.0.0.tar", max compression
+gzip compressed data, was "mystbin_py-6.0.1.tar", max compression
```

## Comparing `mystbin_py-6.0.0.tar` & `mystbin_py-6.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1063 2023-07-21 11:45:52.554451 mystbin_py-6.0.0/LICENSE
--rwxr-xr-x   0        0        0     2854 2023-07-23 18:47:43.503227 mystbin_py-6.0.0/README.md
--rwxr-xr-x   0        0        0     1547 2023-07-23 18:59:34.053690 mystbin_py-6.0.0/mystbin/__init__.py
--rwxr-xr-x   0        0        0     6382 2023-07-23 18:36:56.781690 mystbin_py-6.0.0/mystbin/client.py
--rwxr-xr-x   0        0        0     1738 2023-07-21 11:50:11.686218 mystbin_py-6.0.0/mystbin/errors.py
--rwxr-xr-x   0        0        0    10885 2023-07-23 18:21:32.231992 mystbin_py-6.0.0/mystbin/http.py
--rwxr-xr-x   0        0        0     4715 2023-07-23 18:23:13.509501 mystbin_py-6.0.0/mystbin/paste.py
--rwxr-xr-x   0        0        0        0 2023-07-21 11:45:52.554451 mystbin_py-6.0.0/mystbin/py.typed
--rwxr-xr-x   0        0        0     1149 2023-07-21 11:45:52.554451 mystbin_py-6.0.0/mystbin/types/__init__.py
--rwxr-xr-x   0        0        0     1613 2023-07-21 11:50:11.694218 mystbin_py-6.0.0/mystbin/types/responses.py
--rwxr-xr-x   0        0        0     2263 2023-07-21 11:45:52.558451 mystbin_py-6.0.0/mystbin/utils.py
--rwxr-xr-x   0        0        0     2147 2023-07-23 18:59:22.461519 mystbin_py-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 mystbin_py-6.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1063 2023-07-21 11:45:52.554451 mystbin_py-6.0.1/LICENSE
+-rwxr-xr-x   0        0        0     2886 2023-07-25 03:47:26.738429 mystbin_py-6.0.1/README.md
+-rwxr-xr-x   0        0        0     1547 2023-07-25 03:53:45.475988 mystbin_py-6.0.1/mystbin/__init__.py
+-rwxr-xr-x   0        0        0     6403 2023-07-25 03:47:11.270202 mystbin_py-6.0.1/mystbin/client.py
+-rwxr-xr-x   0        0        0     1738 2023-07-21 11:50:11.686218 mystbin_py-6.0.1/mystbin/errors.py
+-rwxr-xr-x   0        0        0    10885 2023-07-23 18:21:32.231992 mystbin_py-6.0.1/mystbin/http.py
+-rwxr-xr-x   0        0        0     4787 2023-07-25 03:45:21.648593 mystbin_py-6.0.1/mystbin/paste.py
+-rwxr-xr-x   0        0        0        0 2023-07-21 11:45:52.554451 mystbin_py-6.0.1/mystbin/py.typed
+-rwxr-xr-x   0        0        0     1149 2023-07-21 11:45:52.554451 mystbin_py-6.0.1/mystbin/types/__init__.py
+-rwxr-xr-x   0        0        0     1689 2023-07-25 03:42:26.222018 mystbin_py-6.0.1/mystbin/types/responses.py
+-rwxr-xr-x   0        0        0     2263 2023-07-21 11:45:52.558451 mystbin_py-6.0.1/mystbin/utils.py
+-rwxr-xr-x   0        0        0     2147 2023-07-25 03:53:34.339825 mystbin_py-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4218 1970-01-01 00:00:00.000000 mystbin_py-6.0.1/PKG-INFO
```

### Comparing `mystbin_py-6.0.0/LICENSE` & `mystbin_py-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.0/README.md` & `mystbin_py-6.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 Documentation for this wrapper can be found [here](https://mystbinpy.readthedocs.io/en/stable/).
 If you want the docs for the `main` branch, those can be found [here](https://mystbinpy.readthedocs.io/en/latest/).
 
 ----------
 ### Features
 
 - [x] - Creating pastes.
+  - [ ] Supporting attachments.
 - [ ] - Editing pastes.
     - Pending design work.
 - [x] - Deleting pastes.
 - [x] - Getting pastes.
 - [ ] - User endpoints.
 - [ ] - Sync client.
   - This one will take some time as I have no motivation to do it, but PRs are welcome if others want to do it.
```

#### html2text {}

```diff
@@ -2,28 +2,28 @@
             [Documentation_Status] [Linting_status] [Build_status]
 
 A small simple wrapper around the [Mystb.in](https://mystb.in/) API. API docs
 can be found [here](https://api.mystb.in/docs). Documentation for this wrapper
 can be found [here](https://mystbinpy.readthedocs.io/en/stable/). If you want
 the docs for the `main` branch, those can be found [here](https://
 mystbinpy.readthedocs.io/en/latest/). ---------- ### Features - [x] - Creating
-pastes. - [ ] - Editing pastes. - Pending design work. - [x] - Deleting pastes.
-- [x] - Getting pastes. - [ ] - User endpoints. - [ ] - Sync client. - This one
-will take some time as I have no motivation to do it, but PRs are welcome if
-others want to do it. ### Installation This project will be on [PyPI](https://
-pypi.org/project/mystbin.py/) as a stable release, you can always find that
-there. Installing via `pip`: ```shell python -m pip install -U mystbin.py ```
-Installing from source: ```shell python -m pip install git+https://github.com/
-PythonistaGuild/mystbin.py.git ``` ### Usage examples ```py # async example -
-it will default to async import mystbin client = mystbin.Client() paste = await
-client.create_paste(filename="Hello.txt", content="Hello there!") # we also
-support passing a mystbin.File directly to the `file=` kwarg! str(paste) >>>
-'https://mystb.in/' get_paste = await client.get_paste("") get_paste.files
-[0].content >>> "Hello there!" get_paste.created_at >>> datetime.datetime(2020,
-10, 6, 10, 53, 57, 556741) ``` Or if you want to create a paste with multiple
-files... ```py import mystbin file = mystbin.File(filename="File1.txt",
-content="Hello there!") file2 = mystbin.File(filename="test.py", content="print
-('hello!')") paste = await client.create_paste(files=[file, file2]) for file in
-paste.files: print(file.content) >>> "Hello there!" >>> "print('hello!')" ```
-If you have any question please feel free to join the Pythonista Discord
-server:
+pastes. - [ ] Supporting attachments. - [ ] - Editing pastes. - Pending design
+work. - [x] - Deleting pastes. - [x] - Getting pastes. - [ ] - User endpoints.
+- [ ] - Sync client. - This one will take some time as I have no motivation to
+do it, but PRs are welcome if others want to do it. ### Installation This
+project will be on [PyPI](https://pypi.org/project/mystbin.py/) as a stable
+release, you can always find that there. Installing via `pip`: ```shell python
+-m pip install -U mystbin.py ``` Installing from source: ```shell python -m pip
+install git+https://github.com/PythonistaGuild/mystbin.py.git ``` ### Usage
+examples ```py # async example - it will default to async import mystbin client
+= mystbin.Client() paste = await client.create_paste(filename="Hello.txt",
+content="Hello there!") # we also support passing a mystbin.File directly to
+the `file=` kwarg! str(paste) >>> 'https://mystb.in/' get_paste = await
+client.get_paste("") get_paste.files[0].content >>> "Hello there!"
+get_paste.created_at >>> datetime.datetime(2020, 10, 6, 10, 53, 57, 556741) ```
+Or if you want to create a paste with multiple files... ```py import mystbin
+file = mystbin.File(filename="File1.txt", content="Hello there!") file2 =
+mystbin.File(filename="test.py", content="print('hello!')") paste = await
+client.create_paste(files=[file, file2]) for file in paste.files: print
+(file.content) >>> "Hello there!" >>> "print('hello!')" ``` If you have any
+question please feel free to join the Pythonista Discord server:
 [Discord_Server]
```

### Comparing `mystbin_py-6.0.0/mystbin/__init__.py` & `mystbin_py-6.0.1/mystbin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,8 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=6, minor=0, micro=0, releaselevel="final", serial=0)
+version_info: VersionInfo = VersionInfo(major=6, minor=0, micro=1, releaselevel="final", serial=0)
```

### Comparing `mystbin_py-6.0.0/mystbin/client.py` & `mystbin_py-6.0.1/mystbin/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             Internally the order of precesence is ``files`` > ``file`` > ``filename and content``.
         """
         if (filename and content) and file:
             raise ValueError("Cannot provide both `file` and `filename`/`content`")
 
         resolved_files: Sequence[File] = []
         if filename and content:
-            resolved_files = [File(filename=filename, content=content)]
+            resolved_files = [File(filename=filename, content=content, attachment_url=None)]
         elif file:
             resolved_files = [file]
 
         if resolved_files and files:
             raise ValueError("Cannot provide both singular and plural files.")
 
         resolved_files = files or resolved_files
```

### Comparing `mystbin_py-6.0.0/mystbin/errors.py` & `mystbin_py-6.0.1/mystbin/errors.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.0/mystbin/http.py` & `mystbin_py-6.0.1/mystbin/http.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.0/mystbin/paste.py` & `mystbin_py-6.0.1/mystbin/paste.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,41 +50,35 @@
     content: :class:`str`
         The file's contents.
     """
 
     __slots__ = (
         "filename",
         "content",
+        "attachment_url",
         "_lines_of_code",
         "_character_count",
     )
 
-    def __init__(
-        self,
-        *,
-        filename: str,
-        content: str,
-    ) -> None:
+    def __init__(self, *, filename: str, content: str, attachment_url: Optional[str]) -> None:
         self.filename: str = filename
         self.content: str = content
+        self.attachment_url: Optional[str] = attachment_url
 
     @property
     def lines_of_code(self) -> int:
         return self._lines_of_code
 
     @property
     def character_count(self) -> int:
         return self._character_count
 
     @classmethod
     def from_data(cls, payload: FileResponse, /) -> Self:
-        self = cls(
-            content=payload["content"],
-            filename=payload["filename"],
-        )
+        self = cls(content=payload["content"], filename=payload["filename"], attachment_url=payload["attachment"])
         self._lines_of_code = payload["loc"]
         self._character_count = payload["charcount"]
 
         return self
 
     def to_dict(self) -> Dict[str, Any]:
         ret: Dict[str, Any] = {"content": self.content, "filename": self.filename}
@@ -116,24 +110,19 @@
         "files",
         "notice",
         "_expires",
         "_views",
         "_last_edited",
     )
 
-    def __init__(
-        self,
-        *,
-        id: str,
-        created_at: str,
-        files: List[File],
-    ) -> None:
+    def __init__(self, *, id: str, created_at: str, files: List[File], notice: Optional[str]) -> None:
         self.id: str = id
         self.created_at: datetime.datetime = datetime.datetime.fromisoformat(created_at)
-        self.files: list[File] = files
+        self.files: List[File] = files
+        self.notice: Optional[str] = notice
 
     def __str__(self) -> str:
         return self.url
 
     def __repr__(self) -> str:
         return f"<Paste id={self.id!r} files={len(self.files)}>"
 
@@ -152,26 +141,22 @@
     @property
     def views(self) -> Optional[int]:
         return self._views
 
     @classmethod
     def from_data(cls, payload: PasteResponse, /) -> Self:
         files = [File.from_data(data) for data in payload["files"]]
-        self = cls(
-            id=payload["id"],
-            created_at=payload["created_at"],
-            files=files,
-        )
+        self = cls(id=payload["id"], created_at=payload["created_at"], files=files, notice=payload["notice"])
         self._views = payload.get("views")
-        last_edited = payload.get("last_edited")
+        last_edited = payload["last_edited"]
         if last_edited:
             self._last_edited = datetime.datetime.fromisoformat(last_edited)
         else:
             self._last_edited = None
 
-        expires = payload.get("expires")
+        expires = payload["expires"]
         if expires:
             self._expires = datetime.datetime.fromisoformat(expires)
         else:
             self._expires = None
 
         return self
```

### Comparing `mystbin_py-6.0.0/mystbin/types/__init__.py` & `mystbin_py-6.0.1/mystbin/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.0/mystbin/utils.py` & `mystbin_py-6.0.1/mystbin/utils.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.0.0/pyproject.toml` & `mystbin_py-6.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mystbin-py"
-version = "6.0.0"
+version = "6.0.1"
 description = "A small simple wrapper around the mystb.in API."
 authors = ["AbstractUmbra <Umbra@AbstractUmbra.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/PythonistaGuild/mystbin.py"
 repository = "https://github.com/PythonistaGuild/mystbin.py"
 keywords = ["mystbin",  "paste"]
```

### Comparing `mystbin_py-6.0.0/PKG-INFO` & `mystbin_py-6.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystbin-py
-Version: 6.0.0
+Version: 6.0.1
 Summary: A small simple wrapper around the mystb.in API.
 Home-page: https://github.com/PythonistaGuild/mystbin.py
 License: MIT
 Keywords: mystbin,paste
 Author: AbstractUmbra
 Author-email: Umbra@AbstractUmbra.dev
 Requires-Python: >=3.8,<4.0
@@ -50,14 +50,15 @@
 Documentation for this wrapper can be found [here](https://mystbinpy.readthedocs.io/en/stable/).
 If you want the docs for the `main` branch, those can be found [here](https://mystbinpy.readthedocs.io/en/latest/).
 
 ----------
 ### Features
 
 - [x] - Creating pastes.
+  - [ ] Supporting attachments.
 - [ ] - Editing pastes.
     - Pending design work.
 - [x] - Deleting pastes.
 - [x] - Getting pastes.
 - [ ] - User endpoints.
 - [ ] - Sync client.
   - This one will take some time as I have no motivation to do it, but PRs are welcome if others want to do it.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mystbin-py Version: 6.0.0 Summary: A small simple
+Metadata-Version: 2.1 Name: mystbin-py Version: 6.0.1 Summary: A small simple
 wrapper around the mystb.in API. Home-page: https://github.com/PythonistaGuild/
 mystbin.py License: MIT Keywords: mystbin,paste Author: AbstractUmbra Author-
 email: Umbra@AbstractUmbra.dev Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -20,28 +20,28 @@
             [Documentation_Status] [Linting_status] [Build_status]
 
 A small simple wrapper around the [Mystb.in](https://mystb.in/) API. API docs
 can be found [here](https://api.mystb.in/docs). Documentation for this wrapper
 can be found [here](https://mystbinpy.readthedocs.io/en/stable/). If you want
 the docs for the `main` branch, those can be found [here](https://
 mystbinpy.readthedocs.io/en/latest/). ---------- ### Features - [x] - Creating
-pastes. - [ ] - Editing pastes. - Pending design work. - [x] - Deleting pastes.
-- [x] - Getting pastes. - [ ] - User endpoints. - [ ] - Sync client. - This one
-will take some time as I have no motivation to do it, but PRs are welcome if
-others want to do it. ### Installation This project will be on [PyPI](https://
-pypi.org/project/mystbin.py/) as a stable release, you can always find that
-there. Installing via `pip`: ```shell python -m pip install -U mystbin.py ```
-Installing from source: ```shell python -m pip install git+https://github.com/
-PythonistaGuild/mystbin.py.git ``` ### Usage examples ```py # async example -
-it will default to async import mystbin client = mystbin.Client() paste = await
-client.create_paste(filename="Hello.txt", content="Hello there!") # we also
-support passing a mystbin.File directly to the `file=` kwarg! str(paste) >>>
-'https://mystb.in/' get_paste = await client.get_paste("") get_paste.files
-[0].content >>> "Hello there!" get_paste.created_at >>> datetime.datetime(2020,
-10, 6, 10, 53, 57, 556741) ``` Or if you want to create a paste with multiple
-files... ```py import mystbin file = mystbin.File(filename="File1.txt",
-content="Hello there!") file2 = mystbin.File(filename="test.py", content="print
-('hello!')") paste = await client.create_paste(files=[file, file2]) for file in
-paste.files: print(file.content) >>> "Hello there!" >>> "print('hello!')" ```
-If you have any question please feel free to join the Pythonista Discord
-server:
+pastes. - [ ] Supporting attachments. - [ ] - Editing pastes. - Pending design
+work. - [x] - Deleting pastes. - [x] - Getting pastes. - [ ] - User endpoints.
+- [ ] - Sync client. - This one will take some time as I have no motivation to
+do it, but PRs are welcome if others want to do it. ### Installation This
+project will be on [PyPI](https://pypi.org/project/mystbin.py/) as a stable
+release, you can always find that there. Installing via `pip`: ```shell python
+-m pip install -U mystbin.py ``` Installing from source: ```shell python -m pip
+install git+https://github.com/PythonistaGuild/mystbin.py.git ``` ### Usage
+examples ```py # async example - it will default to async import mystbin client
+= mystbin.Client() paste = await client.create_paste(filename="Hello.txt",
+content="Hello there!") # we also support passing a mystbin.File directly to
+the `file=` kwarg! str(paste) >>> 'https://mystb.in/' get_paste = await
+client.get_paste("") get_paste.files[0].content >>> "Hello there!"
+get_paste.created_at >>> datetime.datetime(2020, 10, 6, 10, 53, 57, 556741) ```
+Or if you want to create a paste with multiple files... ```py import mystbin
+file = mystbin.File(filename="File1.txt", content="Hello there!") file2 =
+mystbin.File(filename="test.py", content="print('hello!')") paste = await
+client.create_paste(files=[file, file2]) for file in paste.files: print
+(file.content) >>> "Hello there!" >>> "print('hello!')" ``` If you have any
+question please feel free to join the Pythonista Discord server:
 [Discord_Server]
```

