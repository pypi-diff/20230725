# Comparing `tmp/fw_storage-2.1.9-py3-none-any.whl.zip` & `tmp/fw_storage-3.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,24 @@
-Zip file size: 38154 bytes, number of entries: 24
+Zip file size: 30706 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      511 b- defN 80-Jan-01 00:00 fw_storage/__init__.py
--rw-r--r--  2.0 unx    18182 b- defN 80-Jan-01 00:00 fw_storage/config.py
+-rw-r--r--  2.0 unx    14408 b- defN 80-Jan-01 00:00 fw_storage/config.py
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 fw_storage/errors.py
--rw-r--r--  2.0 unx     1737 b- defN 80-Jan-01 00:00 fw_storage/fileinfo.py
+-rw-r--r--  2.0 unx     2236 b- defN 80-Jan-01 00:00 fw_storage/fileinfo.py
 -rw-r--r--  2.0 unx     1016 b- defN 80-Jan-01 00:00 fw_storage/filters.py
--rw-r--r--  2.0 unx     1013 b- defN 80-Jan-01 00:00 fw_storage/future/__init__.py
--rw-r--r--  2.0 unx    11860 b- defN 80-Jan-01 00:00 fw_storage/future/base.py
+-rw-r--r--  2.0 unx      922 b- defN 80-Jan-01 00:00 fw_storage/future/__init__.py
+-rw-r--r--  2.0 unx    11279 b- defN 80-Jan-01 00:00 fw_storage/future/base.py
 -rw-r--r--  2.0 unx     4652 b- defN 80-Jan-01 00:00 fw_storage/future/errors.py
 -rw-r--r--  2.0 unx       36 b- defN 80-Jan-01 00:00 fw_storage/future/types/__init__.py
--rw-r--r--  2.0 unx    13027 b- defN 80-Jan-01 00:00 fw_storage/future/types/fs.py
+-rw-r--r--  2.0 unx    13019 b- defN 80-Jan-01 00:00 fw_storage/future/types/fs.py
 -rw-r--r--  2.0 unx     3934 b- defN 80-Jan-01 00:00 fw_storage/future/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_storage/py.typed
--rw-r--r--  2.0 unx     7611 b- defN 80-Jan-01 00:00 fw_storage/storage.py
+-rw-r--r--  2.0 unx     7446 b- defN 80-Jan-01 00:00 fw_storage/storage.py
 -rw-r--r--  2.0 unx       28 b- defN 80-Jan-01 00:00 fw_storage/types/__init__.py
 -rw-r--r--  2.0 unx     6950 b- defN 80-Jan-01 00:00 fw_storage/types/az.py
--rw-r--r--  2.0 unx    13364 b- defN 80-Jan-01 00:00 fw_storage/types/dicom.py
--rw-r--r--  2.0 unx     7996 b- defN 80-Jan-01 00:00 fw_storage/types/dicomweb.py
 -rw-r--r--  2.0 unx      140 b- defN 80-Jan-01 00:00 fw_storage/types/fs.py
 -rw-r--r--  2.0 unx     4987 b- defN 80-Jan-01 00:00 fw_storage/types/gs.py
 -rw-r--r--  2.0 unx     6504 b- defN 80-Jan-01 00:00 fw_storage/types/s3.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_storage-2.1.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     4013 b- defN 80-Jan-01 00:00 fw_storage-2.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_storage-2.1.9.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1925 b- defN 16-Jan-01 00:00 fw_storage-2.1.9.dist-info/RECORD
-24 files, 110765 bytes uncompressed, 35070 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_storage-3.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3642 b- defN 80-Jan-01 00:00 fw_storage-3.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_storage-3.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1756 b- defN 16-Jan-01 00:00 fw_storage-3.0.0.dist-info/RECORD
+22 files, 84745 bytes uncompressed, 27880 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -39,35 +39,29 @@
 
 Filename: fw_storage/types/__init__.py
 Comment: 
 
 Filename: fw_storage/types/az.py
 Comment: 
 
-Filename: fw_storage/types/dicom.py
-Comment: 
-
-Filename: fw_storage/types/dicomweb.py
-Comment: 
-
 Filename: fw_storage/types/fs.py
 Comment: 
 
 Filename: fw_storage/types/gs.py
 Comment: 
 
 Filename: fw_storage/types/s3.py
 Comment: 
 
-Filename: fw_storage-2.1.9.dist-info/LICENSE
+Filename: fw_storage-3.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: fw_storage-2.1.9.dist-info/METADATA
+Filename: fw_storage-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: fw_storage-2.1.9.dist-info/WHEEL
+Filename: fw_storage-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: fw_storage-2.1.9.dist-info/RECORD
+Filename: fw_storage-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_storage/config.py

```diff
@@ -8,15 +8,14 @@
 import abc
 import json
 import os
 import re
 import typing as t
 from pathlib import Path
 
-from fw_http_client import AnyAuth
 from fw_utils import format_query_string as qs
 from fw_utils import format_url, parse_url
 from pydantic import BaseModel, Field, SecretStr, root_validator, validator
 
 from .future.types.fs import FSConfig, FSConfigOverride
 
 LOAD_ENV = True  # load creds from envvars (and read file for gs)
@@ -380,124 +379,11 @@
 
     type: t.Literal["az"] = Field("az", title="Azure Blob Storage type")
     prefix: t.Optional[str] = Field(
         None, title="Common object key prefix", example="prefix"
     )
 
 
-class DICOMConfig(StorageConfig):
-    """DICOM Storage config."""
-
-    type: t.Literal["dicom"] = Field("dicom", title="DICOM Storage type")
-    host: str = Field(title="DICOM SCP / PACS server host or IP")
-    port: str = Field(
-        title="DICOM SCP / PACS server port",
-        regex=r"^[0-9]+$",
-    )
-    aec: t.Optional[str] = Field(None, title="Called Application Entity Title")
-    aet: str = Field("FW-STORAGE", title="Calling Application Entity Title")
-    rport: t.Optional[str] = Field(None, title="Return port for moving images (C-MOVE)")
-
-    @classmethod
-    def from_url(cls, url: str) -> "DICOMConfig":
-        """Return DICOM config parsed from a URL."""
-        parsed = parse_url(url)
-        params = {
-            "type": parsed.pop("scheme"),
-            "host": parsed.pop("host"),
-            "port": parsed.pop("port"),
-            "rport": parsed.pop("password", None),
-            "aet": parsed.pop("username", "FW-STORAGE"),
-        }
-
-        aec = parsed.pop("path", None)
-        if aec:
-            params["aec"] = aec.strip("/")
-        assert not parsed, f"unexpected {','.join(parsed)} in url {url!r}"
-        return cls(**params)
-
-    @property
-    def safe_url(self) -> str:
-        """Return safe storage URL without credentials."""
-        return format_url(
-            scheme=self.type,
-            host=self.host,
-            port=int(self.port),
-            username=self.aet,
-            password=self.rport,
-            path=self.aec,
-        )
-
-    @property
-    def full_url(self) -> str:
-        """Return full storage URL with credentials."""
-        return self.safe_url
-
-
-class DICOMWebConfig(StorageConfig):
-    """DICOMweb Storage config."""
-
-    type: t.Literal["dicomweb"] = Field("dicomweb", title="DICOMWeb Storage type")
-    api_url: str = Field(title="API URL")
-    auth: t.Optional[AnyAuth] = Field(None, title="Authorization")
-
-    @classmethod
-    def from_url(cls, url: str) -> "DICOMWebConfig":
-        """Return DICOM config parsed from a URL."""
-        parsed = parse_url(url)
-
-        api_url = parsed.pop("host")
-        port = parsed.pop("port", None)
-        if port:
-            api_url = f"{api_url}:{port}"
-        path = parsed.pop("path", None)
-        if path:
-            api_url = f"{api_url}/{path}"
-        driver = parsed.pop("driver", None)
-        if not api_url.startswith("http"):
-            if driver:
-                api_url = f"{driver}://{api_url}"
-            else:
-                api_url = f"https://{api_url}"
-
-        username = parsed.pop("username", None)
-        password = parsed.pop("password", None)
-        auth: t.Any = None
-        if username:
-            auth = str(username)
-            if password:
-                auth = f"{auth}:{str(password)}"
-            if isinstance(auth, str) and ":" in auth:
-                auth = tuple(auth.split(":", 1))
-
-        params = {"type": parsed.pop("scheme"), "api_url": api_url, "auth": auth}
-
-        assert not parsed, f"unexpected {','.join(parsed)} in url {url!r}"
-        return cls(**params)
-
-    @property
-    def safe_url(self) -> str:
-        """Return safe storage URL without credentials."""
-        match = re.match(r"(.*)://(.*)", self.api_url)
-        assert match, f"could not parse {self.api_url!r}"
-        driver = match.groups()[0]
-        host = match.groups()[1]
-
-        if driver == "https":
-            driver = None
-
-        auth = self.auth
-        if isinstance(auth, tuple):
-            auth = ":".join(auth)
-
-        return format_url(scheme=self.type, host=host, username=auth, driver=driver)
-
-    @property
-    def full_url(self) -> str:
-        """Return full storage URL with credentials."""
-        return self.safe_url
-
-
-Config = t.Union[FSConfig, S3Config, GSConfig, AZConfig, DICOMConfig, DICOMWebConfig]
+Config = t.Union[FSConfig, S3Config, GSConfig, AZConfig]
 ConfigOverride = t.Union[
     FSConfigOverride, S3ConfigOverride, GSConfigOverride, AZConfigOverride
 ]
```

## fw_storage/fileinfo.py

```diff
@@ -10,47 +10,64 @@
 
     Path is unique and relative to the storage prefix. Slots minimize memory
     usage to allow storing large number of FileInfo instances at once.
     """
 
     __slots__ = ("type", "path", "size", "hash", "created", "modified")
 
-    type: t.Literal["fs", "s3", "gs", "az", "dicom"]
+    type: t.Literal["fs", "s3", "gs", "az"]
     path: str
     size: int
     hash: t.Optional[str]
     created: t.Optional[t.Union[int, float]]
     modified: t.Optional[t.Union[int, float]]
 
+    def __str__(self) -> str:  # pragma: no cover
+        """Return the path string."""
+        return self.path
+
     def asdict(self) -> t.Dict:
         """Return as a dictionary."""
         # TODO performance-test this and improve as needed
         return dataclasses.asdict(self)  # pragma: no cover
 
+    # FUTURE COMPAT
+
     def dict(self) -> t.Dict:  # pragma: no cover
         """Future compatibility."""
         return self.asdict()
 
     @property
-    def dir(self) -> str:  # pragma: no cover
-        """Return the directory name of this path."""
-        dirname = str(Path(self.path).parent)
-        return "" if dirname == "." else dirname
-
-    @property
     def name(self) -> str:  # pragma: no cover
         """Return the base filename of this path."""
         return Path(self.path).name
 
     @property
     def stem(self) -> str:  # pragma: no cover
         """Return the filename stem without any extension suffix."""
         return Path(self.path).stem
 
     @property
     def ext(self) -> str:  # pragma: no cover
         """Return the extension of this path."""
         return Path(self.path).suffix.lstrip(".")
 
-    def __str__(self) -> str:  # pragma: no cover
-        """Return the path string."""
-        return self.path
+    @property
+    def dir(self) -> str:  # pragma: no cover
+        """Return the directory name of this path."""
+        dirname = str(Path(self.path).parent)
+        return "" if dirname == "." else dirname
+
+    @property
+    def depth(self) -> int:  # pragma: no cover
+        """Return the path's depth - starting at 1 for top-level files."""
+        return 1 + self.path.count("/")
+
+    @property
+    def ctime(self) -> t.Optional[t.Union[int, float]]:  # pragma: no cover
+        """Return file's ctime."""
+        return self.created
+
+    @property
+    def mtime(self) -> t.Optional[t.Union[int, float]]:  # pragma: no cover
+        """Return file's mtime."""
+        return self.modified
```

## fw_storage/future/__init__.py

```diff
@@ -5,16 +5,14 @@
 from .utils import URL
 
 STORAGE_CONFIGS = {
     "fs": ".types.fs.FSConfig",
     "gs": ".types.gs.GSConfig",
     "s3": ".types.s3.S3Config",
     "az": ".types.az.AZConfig",
-    "dicom": ".types.dicom.DICOMConfig",
-    "dicomweb": ".types.dicomweb.DICOMwebConfig",
 }
 
 
 def create_storage_client(url: str) -> Storage:
     """Return storage client from a URL."""
     return create_storage_config(url).create_client()
```

## fw_storage/future/base.py

```diff
@@ -9,22 +9,79 @@
 from pydantic import BaseModel, Field, SecretStr
 from pydantic.generics import GenericModel
 
 from .. import filters  # TODO phase out usage
 from . import errors
 
 Mode = t.Literal["r", "w"]
-AnyPath = t.Union[str, Path, "Item"]
+AnyPath = t.Union[str, Path, "File"]
 ConfigT = t.TypeVar("ConfigT", bound="Config")
 CloudConfigT = t.TypeVar("CloudConfigT", bound="CloudConfig")
-ItemT = t.TypeVar("ItemT", bound="Item")
 FileT = t.TypeVar("FileT", bound="File")
 StorageT = t.TypeVar("StorageT", bound="Storage")
 
 
+class File(BaseModel):
+    """File model with common attrs of files or blobs."""
+
+    type: t.Literal["fs", "s3", "gs", "az"]
+    path: str
+    size: int
+    hash: str
+    ctime: t.Union[int, float, None]
+    mtime: t.Union[int, float, None]
+
+    def __str__(self) -> str:
+        """Return string representation."""
+        return self.path
+
+    @property
+    def name(self) -> str:
+        """Return the base filename of this path."""
+        return Path(self.path).name
+
+    @property
+    def stem(self) -> str:
+        """Return the filename stem without any extension suffix."""
+        return Path(self.path).stem
+
+    @property
+    def ext(self) -> str:
+        """Return the extension of this path."""
+        return Path(self.path).suffix.lstrip(".")
+
+    @property
+    def dir(self) -> str:
+        """Return the directory name of this path."""
+        dirname = str(Path(self.path).parent)
+        return "" if dirname == "." else dirname
+
+    @property
+    def depth(self) -> int:
+        """Return the path's depth - starting at 1 for top-level files."""
+        return 1 + self.path.count("/")  # pragma: no cover
+
+    # STORAGE FILEINFO INTERFACE BACKWARDS COMPATIBILITY
+    # TODO deprecation warning (when most of future is implemented)
+
+    @property
+    def created(self):
+        """Backwards compatibility only."""
+        return self.ctime
+
+    @property
+    def modified(self):
+        """Backwards compatibility only."""
+        return self.mtime
+
+    def asdict(self) -> dict:
+        """Backwards compatibility only."""
+        return self.dict()  # pragma: no cover
+
+
 class Config(ABC, GenericModel, t.Generic[ConfigT]):
     """Storage config interface."""
 
     class Config:
         """Forbid extra attrs and allow using cached_property on models."""
 
         # fail fast on unexpected input (eg. unknown URL query params)
@@ -92,33 +149,16 @@
         """Backwards compatibility only."""
         properties = self.schema()["properties"]
         for key, value in override.dict(exclude_unset=True).items():
             assert key in properties
             setattr(self, key, value)
 
 
-class Item(BaseModel):
-    """Storage item representing an individual file/blob/etc."""
-
-    path: str
-
-    def __str__(self) -> str:
-        """Return string representation."""
-        return self.path
-
-    # STORAGE FILEINFO INTERFACE BACKWARDS COMPATIBILITY
-    # TODO deprecation warning (when most of future is implemented)
-
-    def asdict(self) -> dict:
-        """Backwards compatibility only."""
-        return self.dict()  # pragma: no cover
-
-
-class Storage(ABC, t.Generic[ConfigT, ItemT]):
-    """Storage client interface."""
+class Storage(ABC, t.Generic[ConfigT, FileT]):
+    """File storage client interface."""
 
     @abstractmethod
     def __init__(self, config: ConfigT) -> None:
         """Init storage client with config."""
         self.config = config  # pragma: no cover
 
     @abstractmethod
@@ -137,26 +177,26 @@
             urlpath += "/"
         return f"{urlpath}{relpath}"
 
     @abstractmethod
     def ls(  # noqa: D417
         self,
         path: t.Optional[AnyPath] = None,
-        filt: t.Optional[t.Callable[[ItemT], bool]] = None,
+        filt: t.Optional[t.Callable[[FileT], bool]] = None,
         **kw,
-    ) -> t.Iterator[ItemT]:
+    ) -> t.Iterator[FileT]:
         """Yield sorted storage items, optionally filtered.
 
         Args:
             path: Path prefix to yield items from.
             filt: Callback to filter items with.
         """
 
     @abstractmethod
-    def stat(self, path: AnyPath) -> ItemT:
+    def stat(self, path: AnyPath) -> FileT:
         """Return a storage item from an str or Path."""
 
     @abstractmethod
     def open(self, path: AnyPath, mode: Mode = "r") -> t.BinaryIO:
         """Return an item opened for reading or writing."""
 
     @abstractmethod
@@ -165,21 +205,44 @@
 
         Args:
             path: Storage item path to remove / delete.
             recurse: Set to True remove all items with the given prefix.
                 Required when deleting fs:// directories, for example.
         """
 
-    @abstractmethod
     def test(self, mode: Mode = "r") -> None:
         """Test whether the storage can be read/written and raise if not.
 
         Args:
             mode: Set to "w" to check write/rm perms in addition to ls/read.
         """
+        # test open("w") and write() if mode=w
+        fw_test = "fw-test"
+        if mode == "w":
+            with self.open(fw_test, mode="w") as file:
+                file.write(fw_test.encode("ascii"))
+        # test ls() then stat() the first item
+        item: t.Any = None
+        for item in self.ls():
+            item = self.stat(item)
+            break
+        else:
+            # for/else: no items found - if "w", we expect the test file
+            if mode == "w":  # pragma: no cover
+                raise errors.StorageError(f"ls() did not yield {fw_test!r}")
+        # test open("r") and read() a single byte (whole file could be BIG)
+        # use the test file if "w", or the 1st ls() yield if available
+        item = fw_test if mode == "w" else item
+        if item:
+            with self.open(item) as file:
+                file.read(1)
+        # test rm() on the test file if mode=w
+        if mode == "w":
+            self.rm(fw_test)
+            self.cleanup()
 
     def cleanup(self) -> None:
         """Run any cleanup steps."""
 
     def __enter__(self: StorageT) -> StorageT:
         """Enter context to enable auto-cleanup on exit."""
         return self
@@ -228,109 +291,26 @@
 
     def set(self, path: AnyPath, file):
         """Backwards compatibility only."""
         with fw_utils.open_any(file) as rf, self.open(path, mode="w") as wf:
             shutil.copyfileobj(rf, wf)
 
 
-class File(Item):
-    """File item with common attrs of files or blobs."""
-
-    type: t.Literal["fs", "s3", "gs", "az"]
-    size: int
-    ctime: t.Union[int, float, None]
-    mtime: t.Union[int, float, None]
-    hash: str
-
-    @property
-    def dir(self) -> str:
-        """Return the directory name of this path."""
-        dirname = str(Path(self.path).parent)
-        return "" if dirname == "." else dirname
-
-    @property
-    def name(self) -> str:
-        """Return the base filename of this path."""
-        return Path(self.path).name
-
-    @property
-    def stem(self) -> str:
-        """Return the filename stem without any extension suffix."""
-        return Path(self.path).stem
-
-    @property
-    def ext(self) -> str:
-        """Return the extension of this path."""
-        return Path(self.path).suffix.lstrip(".")
-
-    # STORAGE ITEM (OLD FILEINFO) INTERFACE BACKWARDS COMPATIBILITY
-    # TODO deprecation warning (when most of future is implemented)
-
-    @property
-    def created(self):
-        """Backwards compatibility only."""
-        return self.ctime
-
-    @property
-    def modified(self):
-        """Backwards compatibility only."""
-        return self.mtime
-
-
-class FileStorage(Storage, t.Generic[FileT]):
-    """File storage client interface w/ extended item and implementing test()."""
-
-    @abstractmethod
-    def stat(self, path: AnyPath) -> FileT:
-        """Return a storage item from an str or Path."""
-
-    def test(self, mode: Mode = "r") -> None:
-        """Test whether the storage can be read/written and raise if not.
-
-        Args:
-            mode: Set to "w" to check write/rm perms in addition to ls/read.
-        """
-        # test open("w") and write() if mode=w
-        fw_test = "fw-test"
-        if mode == "w":
-            with self.open(fw_test, mode="w") as file:
-                file.write(fw_test.encode("ascii"))
-        # test ls() then stat() the first item
-        item: t.Any = None
-        for item in self.ls():
-            item = self.stat(item)
-            break
-        else:
-            # for/else: no items found - if "w", we expect the test file
-            if mode == "w":  # pragma: no cover
-                raise errors.StorageError(f"ls() did not yield {fw_test!r}")
-        # test open("r") and read() a single byte (whole file could be BIG)
-        # use the test file if "w", or the 1st ls() yield if available
-        item = fw_test if mode == "w" else item
-        if item:
-            with self.open(item) as file:
-                file.read(1)
-        # test rm() on the test file if mode=w
-        if mode == "w":
-            self.rm(fw_test)
-            self.cleanup()
-
-
 class CloudConfig(Config):
     """Cloud storage config interface w/ rm_batch_max."""
 
     rm_batch_max: t.Optional[int] = Field(
         100,
         title="Max no. of blobs to delete in a single bulk operation.",
         min=1,
         max=1000,
     )
 
 
-class CloudStorage(FileStorage, t.Generic[CloudConfigT]):  # pragma: no cover
+class CloudStorage(Storage, t.Generic[CloudConfigT]):  # pragma: no cover
     """Cloud storage client interface defining rm_bulk() / implementing rm()."""
 
     @abstractmethod
     def __init__(self, config: CloudConfigT) -> None:
         """Init cloud storage client with config and an empty rm_keys."""
         self.config = config
         self.rm_keys: t.List[str] = []
```

## fw_storage/future/types/fs.py

```diff
@@ -7,15 +7,15 @@
 from functools import cached_property
 from pathlib import Path
 from stat import S_IMODE
 
 from pydantic import BaseModel, Field, root_validator, validator
 
 from .. import errors, utils
-from ..base import AnyPath, Config, File, FileStorage, Mode
+from ..base import AnyPath, Config, File, Mode, Storage
 
 ERRMAP: dict = {
     FileExistsError: errors.FileExists,
     FileNotFoundError: errors.FileNotFound,
     IsADirectoryError: errors.IsADirectory,
     NotADirectoryError: errors.NotADirectory,
     PermissionError: errors.PermError,
@@ -160,15 +160,15 @@
     """FS / local file-system file model."""
 
     type: t.Literal["fs"] = "fs"
     owner: str
     perms: str
 
 
-class FSStorage(FileStorage):
+class FSStorage(Storage):
     """FS / local file-system storage client."""
 
     def __init__(self, config: FSConfig) -> None:
         """Init FS / local file-system storage from a config."""
         self.config = config
         path = Path(config.path)
         if not path.exists():
@@ -246,15 +246,15 @@
         stat = path.stat()
         return FSFile(
             path=self.relpath(path),
             size=stat.st_size,
             ctime=stat.st_ctime,
             mtime=stat.st_mtime,
             hash=md5sum(path, stat, self.config.content_hash),
-            owner=f"{stat.st_gid}:{stat.st_uid}",
+            owner=f"{stat.st_uid}:{stat.st_gid}",
             perms=oct(S_IMODE(path.stat().st_mode))[-3:],
         )
 
     @errmap
     def open(self, path: AnyPath, mode: Mode = "r") -> t.BinaryIO:
         """Return a file opened for reading or writing."""
         path = Path(self.abspath(path))
```

## fw_storage/storage.py

```diff
@@ -1,34 +1,29 @@
 """Storage base class and factory."""
 import abc
 import importlib
 import typing as t
+from functools import lru_cache
 from pathlib import Path
 
 from fw_utils import AnyFile, BinFile, TempFile, parse_url
-from memoization import cached
 
 from .config import Config
 from .fileinfo import FileInfo
 
 SPOOLED_TMP_MAX_SIZE = 1 << 20  # 1MB
 # map of url schemes to storage class import paths (and user-registered classes)
 # TODO fw:// storage class
 ConfigType = t.Union[str, t.Type["Config"]]
 StorageType = t.Union[str, t.Type["Storage"]]
 STORAGE_CLASSES: t.Dict[str, t.Tuple[ConfigType, StorageType]] = {
     "fs": ("fw_storage.config.FSConfig", "fw_storage.types.fs.FSStorage"),
     "s3": ("fw_storage.config.S3Config", "fw_storage.types.s3.S3Storage"),
     "gs": ("fw_storage.config.GSConfig", "fw_storage.types.gs.GSStorage"),
     "az": ("fw_storage.config.AZConfig", "fw_storage.types.az.AZStorage"),
-    "dicom": ("fw_storage.config.DICOMConfig", "fw_storage.types.dicom.DICOMStorage"),
-    "dicomweb": (
-        "fw_storage.config.DICOMWebConfig",
-        "fw_storage.types.dicomweb.DICOMWebStorage",
-    ),
 }
 
 AnyPath = t.Union[str, FileInfo]
 
 
 class Storage(abc.ABC):
     """Abstract storage class defining the common interface."""
@@ -92,19 +87,19 @@
         self.cleanup()
 
     def cleanup(self) -> None:
         """Run any cleanup steps for the storage (eg. tempfiles, buffers)."""
 
     def __enter__(self):
         """Enter storage 'with' context to enable automatic cleanup()."""
-        return self
+        return self  # pragma: no cover
 
     def __exit__(self, exc_type, exc, traceback) -> None:
         """Invoke cleanup() when exiting the storage 'with' context."""
-        self.cleanup()
+        self.cleanup()  # pragma: no cover
 
     def __del__(self) -> None:
         """Invoke cleanup() when the storage is garbage-collected."""
         self.cleanup()
 
     def __str__(self) -> str:  # pragma: no cover
         """Return string representation of the storage."""
@@ -202,15 +197,15 @@
 
 
 def create_storage_client_cls(storage_cls_path: str) -> t.Type[Storage]:
     """Return the storage class for an import path (late import)."""
     return _get_cls(storage_cls_path)
 
 
-@cached
+@lru_cache
 def _get_cls(cls_path: str):
     """Return the class for an import path (late import)."""
     module_path, cls_name = cls_path.rsplit(".", maxsplit=1)
     try:
         module = importlib.import_module(module_path, cls_name)
         storage_cls = getattr(module, cls_name)
     except (ImportError, AttributeError) as exc:
```

## Comparing `fw_storage-2.1.9.dist-info/LICENSE` & `fw_storage-3.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_storage-2.1.9.dist-info/METADATA` & `fw_storage-3.0.0.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-storage
-Version: 2.1.9
+Version: 3.0.0
 Summary: Unified storage interface.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-storage
 License: MIT
 Keywords: Flywheel,file,object,storage
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
@@ -13,30 +13,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: az
-Provides-Extra: dicom
-Provides-Extra: dicomweb
 Provides-Extra: gs
 Provides-Extra: s3
 Requires-Dist: azure-identity (>=1.11.0,<2.0.0) ; extra == "all" or extra == "az"
 Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0) ; extra == "all" or extra == "az"
 Requires-Dist: boto3 (>=1.17.7,<2.0.0) ; extra == "all" or extra == "s3"
-Requires-Dist: diskcache (>=5.2.1,<6.0.0)
-Requires-Dist: fw-file (>=1,<3)
-Requires-Dist: fw-http-client (>=1.2.0,<2.0.0)
-Requires-Dist: fw-utils (>=4.2.2,<5.0.0)
+Requires-Dist: fw-utils (>=4.2.2)
 Requires-Dist: google-cloud-storage (>=2.2.1,<3.0.0) ; extra == "all" or extra == "gs"
-Requires-Dist: memoization (>=0,<1)
 Requires-Dist: pydantic (>=1.8.1,<2.0.0)
-Requires-Dist: pydicom (>=2.1.2,<3.0.0) ; extra == "all" or extra == "dicomweb"
-Requires-Dist: pynetdicom (>=1.5.7,<2.0.0) ; extra == "all" or extra == "dicom"
 Project-URL: Documentation, https://gitlab.com/flywheel-io/tools/lib/fw-storage
 Project-URL: Repository, https://gitlab.com/flywheel-io/tools/lib/fw-storage
 Description-Content-Type: text/markdown
 
 # fw-storage
 
 Unified file storage interface tuned for simple filtering, memory-efficiency and
```

## Comparing `fw_storage-2.1.9.dist-info/RECORD` & `fw_storage-3.0.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 fw_storage/__init__.py,sha256=v36QDeDLZJv7Sj2zXEZ6s0YIxuz42A9OA8boUEFnPvk,511
-fw_storage/config.py,sha256=VNKq8MNQ4dudrJqU6tBmEx8s5kmOdqKhliFvnvncx_s,18182
+fw_storage/config.py,sha256=K0Xc-Ao4OBQbgC_KnmLObQtFACX3XJmclX3Ik8lsLbk,14408
 fw_storage/errors.py,sha256=HD92V9ebpmsILbhf239XRSmwmO_-WHiOEuYdCUnL1V4,113
-fw_storage/fileinfo.py,sha256=b2ZT8BBPm9Gppa-8R_UqmkUbxDdCnY5Fowrz6n71qHw,1737
+fw_storage/fileinfo.py,sha256=_F40bjc9ueStTV3Vqd_XGLZAiQ7h7VhFAGjbj5jtl1A,2236
 fw_storage/filters.py,sha256=P3C1oGw1q6UoNEbHiSr-xdi_jumosSKOQgsulZ2GGaA,1016
-fw_storage/future/__init__.py,sha256=TWyZ7CFeCDO4_uiiT6gLJhE-SP8Ie7bNsCB3vUSbv2U,1013
-fw_storage/future/base.py,sha256=UGl2BFhRCtJb-LZF3z3ayEX4nh1hDpkZNOhRbaIivpc,11860
+fw_storage/future/__init__.py,sha256=KAczcbIhq7Sjp6PBqpgR1ZB4LuwQPrVGLBx5h6mAYs0,922
+fw_storage/future/base.py,sha256=d_hQWTk7f3YZ0x4wd05SzBt_t0CkvPnU9t5RMlbJ8lM,11279
 fw_storage/future/errors.py,sha256=tE-wb4n_X8-v2zaU5KpoPlQVfDaDhazOpjLmNU45cw0,4652
 fw_storage/future/types/__init__.py,sha256=zOnfjDtMpINsVdYFikGbvjIf_FVnfPpm-DanhqDrLjo,36
-fw_storage/future/types/fs.py,sha256=-9V9_2oDzv82g250JqinRX3OBmoC6gfrEncxgIOLI8g,13027
+fw_storage/future/types/fs.py,sha256=Oz_1zBpW0m8gv3zyTHsfWYyl7Gg3qzCiERZonm-p6VE,13019
 fw_storage/future/utils.py,sha256=JLVhxqSsA0uyNMbhPKyEQoJ3FVYoqLyjyO3bfeO4OOk,3934
 fw_storage/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fw_storage/storage.py,sha256=1_KqVCRUzINhERpSygBNvZhdvIzYBw7V6FWk13DKJqA,7611
+fw_storage/storage.py,sha256=WsYtJwNgiFCq5Esc3WlDhbQC8KzvtAjsMuAcPpE4Jhk,7446
 fw_storage/types/__init__.py,sha256=TT2pfyY-AMuKb4FZduNbVbmWTBRyEC3autb1QbdHE24,28
 fw_storage/types/az.py,sha256=gv1dt_MWZNwUCxxAiiF9KHnlw6vhMNFIu85UtPyNnsQ,6950
-fw_storage/types/dicom.py,sha256=yMMmvV6PLuCkRORzgwVmS5u67PNsgw3LXE6PAvRRSfw,13364
-fw_storage/types/dicomweb.py,sha256=NR9E-csPgznASouwIdokukAxGPKCPRobhz80e4-z_v0,7996
 fw_storage/types/fs.py,sha256=Cz_GGrS_e11m9SvDgdjJkMf-VMI0s5DKUJZp0bWSegM,140
 fw_storage/types/gs.py,sha256=p4rVPsNgaVW4RStFvrrEM3BtNS6xcDBXNnIWFbT7lKA,4987
 fw_storage/types/s3.py,sha256=JNkvaidHR9hCYB1m859Bd8e7fqbkqLxAFa3Skmc3Plg,6504
-fw_storage-2.1.9.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
-fw_storage-2.1.9.dist-info/METADATA,sha256=onJLN7q3RDgfYoJi9BrXWoJxaq_NuyrlGFbcaE_LVb4,4013
-fw_storage-2.1.9.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-fw_storage-2.1.9.dist-info/RECORD,,
+fw_storage-3.0.0.dist-info/LICENSE,sha256=3QLwoJgDkLWRKwcyYzPn3vLqTHhbdltfjFYeBOZSlDY,1078
+fw_storage-3.0.0.dist-info/METADATA,sha256=Du33BRd9DwSkgj1ibVGCz4ojaGUK7rQl9D4a_MEI67I,3642
+fw_storage-3.0.0.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+fw_storage-3.0.0.dist-info/RECORD,,
```

