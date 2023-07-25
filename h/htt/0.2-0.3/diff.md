# Comparing `tmp/htt-0.2.tar.gz` & `tmp/htt-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htt-0.2.tar", max compression
+gzip compressed data, was "htt-0.3.tar", max compression
```

## Comparing `htt-0.2.tar` & `htt-0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-20 03:56:04.979903 htt-0.2/README.md
--rw-r--r--   0        0        0       64 2023-07-24 04:58:15.082524 htt-0.2/htt/__init__.py
--rw-r--r--   0        0        0     7021 2023-07-24 04:57:57.594206 htt-0.2/htt/application.py
--rw-r--r--   0        0        0      304 2023-07-24 04:58:20.474622 htt-0.2/pyproject.toml
--rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 htt-0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-20 03:56:04.979903 htt-0.3/README.md
+-rw-r--r--   0        0        0       64 2023-07-24 04:58:15.082524 htt-0.3/htt/__init__.py
+-rw-r--r--   0        0        0     6862 2023-07-25 02:00:48.769043 htt-0.3/htt/application.py
+-rw-r--r--   0        0        0      304 2023-07-25 02:01:00.953206 htt-0.3/pyproject.toml
+-rw-r--r--   0        0        0      362 1970-01-01 00:00:00.000000 htt-0.3/PKG-INFO
```

### Comparing `htt-0.2/htt/application.py` & `htt-0.3/htt/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,46 +83,46 @@
             file_name (os.PathLike, optional): File name of file handler. Do not create a file handler if set to None. Defaults to None.
             file_size (int, optional): Rotation size of file handler in MB. Defaults to 10.
             file_count (int, optional): Rotation count of file handler. Defaults to 30.
             syslog_address (str, optional): Address of syslog server. Do not create a syslog handler if set to None. Defaults to None.
             syslog_sockettype (socket.SocketKind, optional): Socket type of syslog server. Defaults to socket.SOCK_DGRAM.
 
         Returns:
-            _type_: Return a logger with the specified handlers
+            Logger: Logger created with specified handlers
         """
         assert Application._logger is None
         Application._logger = logging.getLogger()
         Application._logger.setLevel(logging.DEBUG)
-        if file_name is not None:
+        if file_name:
             pathlib.Path(file_name).parent.mkdir(parents=True, exist_ok=True)
             file_handler = logging.handlers.RotatingFileHandler(
                 file_name,
                 maxBytes=1048756 * file_size,
                 backupCount=file_count,
                 encoding="UTF-8",
             )
             file_handler.setLevel(logging.NOTSET)
             file_formatter = _LevelFormatter()
             file_handler.setFormatter(file_formatter)
             Application._logger.addHandler(file_handler)
-        if syslog_address is not None:
+        if syslog_address:
             syslog_handler = logging.handlers.SysLogHandler(
                 Application._split_address(syslog_address),
                 socktype=syslog_sockettype,
             )
             syslog_handler.setLevel(logging.INFO)
             Application._logger.addHandler(syslog_handler)
         return Application._logger
 
     @staticmethod
     def get_logger():
         """Return the logger of current application. Logger must be created by create_logger() first.
 
         Returns:
-            _type_: Return the logger
+            Logger: Logger of current application
         """
         assert Application._logger is not None
         return Application._logger
 
     @staticmethod
     def _split_address(address: str):
         match = re.match(r"^(.+):(\d+)$", address)
@@ -133,24 +133,21 @@
             host = address
             port = None
         return (host, port)
 
 
 class _DateTimeFormatter(logging.Formatter):
     default_time_format = "%Y-%m-%dT%H:%M:%S.%f%z"
-    default_msec_format = "%s,%06d"
 
     def formatTime(self, record, datefmt=None) -> str:
         ct = datetime.datetime.fromtimestamp(record.created, datetime.datetime.now().astimezone().tzinfo)
         if datefmt:
             s = ct.strftime(datefmt)
         else:
             s = ct.strftime(self.default_time_format)
-            if self.default_msec_format:
-                s = self.default_msec_format % (s, record.msecs)
         return s
 
 
 class _LevelFormatter(logging.Formatter):
     default_formatter = _DateTimeFormatter
     default_notset_format = "%(levelname).1s %(asctime)s | %(message)s"
     default_debug_format = "%(levelname).1s %(asctime)s | %(message)s"
```

