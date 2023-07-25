# Comparing `tmp/socketify-0.0.8.tar.gz` & `tmp/socketify-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketify-0.0.8.tar", last modified: Wed Jan 18 21:33:36 2023, max compression
+gzip compressed data, was "socketify-0.0.9.tar", last modified: Thu Jan 19 19:00:46 2023, max compression
```

## Comparing `socketify-0.0.8.tar` & `socketify-0.0.9.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.201635 socketify-0.0.8/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1070 2022-05-28 23:14:27.000000 socketify-0.0.8/LICENSE
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11055 2023-01-18 21:33:36.201635 socketify-0.0.8/PKG-INFO
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10390 2023-01-13 10:37:55.000000 socketify-0.0.8/README.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      658 2023-01-18 20:42:24.000000 socketify-0.0.8/pyproject.toml
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       38 2023-01-18 21:33:36.201635 socketify-0.0.8/setup.cfg
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2819 2023-01-18 20:42:32.000000 socketify-0.0.8/setup.py
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.121634 socketify-0.0.8/src/
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.149634 socketify-0.0.8/src/socketify/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      375 2023-01-18 19:35:29.000000 socketify-0.0.8/src/socketify/__init__.py
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       57 2023-01-07 14:55:58.000000 socketify-0.0.8/src/socketify/__main__.py
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    27408 2023-01-18 19:02:57.000000 socketify-0.0.8/src/socketify/asgi.py
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    14379 2023-01-18 19:03:03.000000 socketify-0.0.8/src/socketify/cli.py
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    13863 2023-01-18 20:07:15.000000 socketify-0.0.8/src/socketify/helpers.py
--rwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)  2920456 2023-01-18 21:32:59.000000 socketify-0.0.8/src/socketify/libsocketify_darwin_amd64.so
--rwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)  2751945 2023-01-18 21:32:59.000000 socketify-0.0.8/src/socketify/libsocketify_darwin_arm64.so
--rwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)  3922512 2023-01-18 20:17:24.000000 socketify-0.0.8/src/socketify/libsocketify_linux_amd64.so
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)  2053632 2023-01-18 21:32:59.000000 socketify-0.0.8/src/socketify/libsocketify_windows_amd64.dll
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6543 2023-01-18 19:02:50.000000 socketify-0.0.8/src/socketify/loop.py
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.149634 socketify-0.0.8/src/socketify/native/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1215 2022-11-23 14:18:51.000000 socketify-0.0.8/src/socketify/native/Make.bat
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9984 2023-01-18 19:45:18.000000 socketify-0.0.8/src/socketify/native/Makefile
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.153634 socketify-0.0.8/src/socketify/native/__pycache__/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      196 2022-06-05 21:02:35.000000 socketify-0.0.8/src/socketify/native/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      200 2022-06-02 18:34:51.000000 socketify-0.0.8/src/socketify/native/__pycache__/__init__.pypy38.pyc
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5847 2022-10-25 15:03:30.000000 socketify-0.0.8/src/socketify/native/__pycache__/uv.cpython-310.pyc
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     7624 2022-11-01 12:17:09.000000 socketify-0.0.8/src/socketify/native/__pycache__/uv.pypy38.pyc
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)   536640 2023-01-18 19:58:49.000000 socketify-0.0.8/src/socketify/native/libsocketify.o
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.153634 socketify-0.0.8/src/socketify/native/src/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    18875 2023-01-07 14:55:58.000000 socketify-0.0.8/src/socketify/native/src/libsocketify.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5096 2023-01-07 14:55:58.000000 socketify-0.0.8/src/socketify/native/src/libsocketify.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10978 2022-11-14 19:14:51.000000 socketify-0.0.8/src/socketify/native/uv_selector.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    18776 2023-01-18 19:03:06.000000 socketify-0.0.8/src/socketify/native.py
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)   118196 2023-01-18 19:02:42.000000 socketify-0.0.8/src/socketify/socketify.py
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    12505 2023-01-08 19:36:25.000000 socketify-0.0.8/src/socketify/ssgi.py
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2161 2023-01-18 19:03:13.000000 socketify-0.0.8/src/socketify/status_codes.py
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22669 2023-01-18 19:02:48.000000 socketify-0.0.8/src/socketify/tasks.py
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.153634 socketify-0.0.8/src/socketify/uWebSockets/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      377 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/GNUmakefile
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11357 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/LICENSE
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      640 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/Makefile
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6024 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/README.md
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.157634 socketify-0.0.8/src/socketify/uWebSockets/benchmarks/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      631 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/benchmarks/Makefile
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2421 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/benchmarks/README.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6413 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/benchmarks/broadcast_test.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9523 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/benchmarks/load_test.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8328 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/benchmarks/scale_test.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3619 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/build.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      552 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/build.h
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.157634 socketify-0.0.8/src/socketify/uWebSockets/capi/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1972 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/Makefile
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.157634 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4572 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/Broadcast.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5628 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/BroadcastEchoServer.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2257 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/EchoServer.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      901 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/HelloWorld.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3729 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/HelloWorldAsync.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9539 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/RustHelloWorld.rs
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1737 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/ServerName.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8409 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/UpgradeAsync.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4038 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/examples/UpgradeSync.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    52633 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/libuwebsockets.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16238 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/capi/libuwebsockets.h
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.157634 socketify-0.0.8/src/socketify/uWebSockets/cluster/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       14 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/cluster/README.md
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.161634 socketify-0.0.8/src/socketify/uWebSockets/examples/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2730 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/Broadcast.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2661 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/BroadcastingEchoServer.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      438 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/Client.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1874 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/Crc32.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2079 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/EchoServer.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1939 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/EchoServerThreaded.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      566 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/HelloWorld.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1444 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/HelloWorldThreaded.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3163 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/Http3Server.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2882 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/HttpServer.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      216 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/README.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      963 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/ServerName.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5882 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/UpgradeAsync.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3510 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/UpgradeSync.cpp
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.165634 socketify-0.0.8/src/socketify/uWebSockets/examples/helpers/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3892 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/helpers/AsyncFileReader.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3207 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/helpers/AsyncFileStreamer.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      578 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/helpers/Middleware.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    12228 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/examples/helpers/optparse.h
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.169634 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5402 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/EpollEchoServer.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      232 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/EpollEchoServer.dict
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3505 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/EpollEchoServerPubSub.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      232 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/EpollEchoServerPubSub.dict
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6595 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/EpollHelloWorld.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      232 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/EpollHelloWorld.dict
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1762 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/Extensions.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4387 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/Http.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3008 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/Makefile
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1744 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/MultipartParser.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2111 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/PerMessageDeflate.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      307 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/QueryParser.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       31 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/QueryParser.dict
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1401 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/README.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4593 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/TopicTree.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       46 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/TopicTree.dict
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1586 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/WebSocket.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1377 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/helpers.h
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.169634 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      565 2023-01-18 19:02:02.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/Makefile
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2354 2023-01-18 19:02:02.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/README.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    59449 2023-01-18 19:02:02.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/epollFuzzer.svg
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    15884 2023-01-18 19:02:02.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/epoll_fuzzer.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4130 2023-01-18 19:02:02.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/test.c
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.169634 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/seed-corpus/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       53 2023-01-18 19:02:05.000000 socketify-0.0.8/src/socketify/uWebSockets/fuzzing/seed-corpus/README.md
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.173634 socketify-0.0.8/src/socketify/uWebSockets/misc/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22909 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/misc/READMORE.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    17816 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/misc/bigshot_lineup.png
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1229 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/misc/cert.pem
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1704 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/misc/key.pem
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11945 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/misc/logo.svg
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22974 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/misc/websocket_lineup.png
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.181635 socketify-0.0.8/src/socketify/uWebSockets/src/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    24818 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/App.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    13739 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/AsyncSocket.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2360 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/AsyncSocketData.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2229 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/BloomFilter.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     7857 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/ChunkedEncoding.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      890 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/ClientApp.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5315 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/Http3App.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6436 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/Http3Context.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      378 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/Http3ContextData.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      665 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/Http3Request.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4419 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/Http3Response.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      600 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/Http3ResponseData.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    21712 2023-01-18 19:57:50.000000 socketify-0.0.8/src/socketify/uWebSockets/src/HttpContext.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1652 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/HttpContextData.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    26798 2023-01-18 19:58:29.000000 socketify-0.0.8/src/socketify/uWebSockets/src/HttpParser.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22782 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/HttpResponse.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2952 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/HttpResponseData.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    13124 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/HttpRouter.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6625 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/Loop.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2884 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/LoopData.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2703 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/MessageParser.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    14436 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/MoveOnlyFunction.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8611 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/Multipart.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10940 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/PerMessageDeflate.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4670 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/ProxyParser.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4831 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/QueryParser.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11523 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/TopicTree.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1436 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/Utilities.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16147 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/WebSocket.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22076 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketContext.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3611 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketContextData.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2781 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketData.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9148 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketExtensions.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5576 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketHandshake.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16858 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketProtocol.h
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.181635 socketify-0.0.8/src/socketify/uWebSockets/tests/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2775 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/tests/BloomFilter.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     7241 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/tests/ChunkedEncoding.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4287 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/tests/ExtensionsNegotiator.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1575 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/tests/HttpParser.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9610 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/tests/HttpRouter.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      626 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/tests/Makefile
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1094 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/tests/README.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6190 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/tests/TopicTree.cpp
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2809 2023-01-18 19:02:01.000000 socketify-0.0.8/src/socketify/uWebSockets/tests/smoke.mjs
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.185635 socketify-0.0.8/src/socketify/uWebSockets/uSockets/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11357 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/LICENSE
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3141 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/Makefile
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1678 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/README.md
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.189635 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11392 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/API-CONVENTIONS.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9018 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/BREAKING-CHANGES.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9298 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/BUILDING.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    26978 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/CMakeLists.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2734 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/CONTRIBUTING.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4444 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/FUZZING.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5116 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/INCORPORATING.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    12517 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/LICENSE
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1179 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/OpenSSLConfig.cmake
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16853 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/PORTING.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2350 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/README.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6673 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/SANDBOXING.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8608 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/STYLE.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      170 2023-01-18 19:02:12.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/codereview.settings
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      175 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/go.mod
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1319 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/go.sum
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11078 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/sources.cmake
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11448 2023-01-18 19:58:41.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/bsd.o
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10432 2023-01-18 19:58:41.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/context.o
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      672 2023-01-18 19:58:42.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/epoll_kqueue.o
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.193635 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4217 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/echo_server.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    15650 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/hammer_test.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16070 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/hammer_test_unix.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5517 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/http3_client.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3582 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/http3_server.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4759 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/http_load_test.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4219 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/http_server.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10941 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/peer_verify_test.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4847 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/udp_benchmark.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      664 2023-01-18 19:58:42.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/gcd.o
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     7696 2023-01-18 19:58:42.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/libuv.o
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8008 2023-01-18 19:58:41.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/loop.o
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.197635 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8187 2023-01-18 19:02:14.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/APIs.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4533 2023-01-18 19:02:14.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/BUILD-WINDOWS.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    64336 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/CHANGELOG
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16902 2023-01-18 19:45:16.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/CMakeCache.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11806 2023-01-18 19:02:14.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/CMakeLists.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      926 2023-01-18 19:02:14.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/CONTRIBUTORS.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      747 2023-01-18 19:02:14.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/Dockerfile
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9699 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/EXAMPLES.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1090 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/LICENSE
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1618 2023-01-18 19:02:14.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/LICENSE.chrome
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6725 2023-01-18 19:45:16.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/Makefile
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3920 2023-01-18 20:48:33.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/README.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      624 2023-01-18 19:02:14.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/appveyor-linux.yml
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      858 2023-01-18 19:02:14.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/appveyor-windows.cmd
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      513 2023-01-18 19:02:14.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/appveyor-windows.yml
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2451 2023-01-18 19:45:16.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/cmake_install.cmake
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.197635 socketify-0.0.8/src/socketify/uWebSockets/uSockets/misc/
--rwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)     1467 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/misc/gen_test_certs.sh
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10991 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/misc/layout.png
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9947 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/misc/manual.md
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       58 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/module.modulemap
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    18816 2023-01-18 19:58:42.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/openssl.o
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22824 2023-01-18 19:58:41.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/quic.o
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    17752 2023-01-18 19:58:42.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/sni_tree.o
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5680 2023-01-18 19:58:41.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/socket.o
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.197635 socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22659 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/bsd.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    19316 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/context.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16951 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/libusockets.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    15109 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/loop.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    34301 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/quic.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3214 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/quic.h
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6760 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/socket.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5094 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/udp.c
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.197635 socketify-0.0.8/src/socketify/uWebSockets/uSockets/tests/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1867 2023-01-18 19:02:07.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/tests/sni_test.c
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)   117616 2023-01-18 19:58:42.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/uSockets_linux_amd64.a
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4216 2023-01-18 19:58:41.000000 socketify-0.0.8/src/socketify/uWebSockets/uSockets/udp.o
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3138 2023-01-18 19:03:18.000000 socketify-0.0.8/src/socketify/uv.py
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    17710 2023-01-18 19:03:22.000000 socketify-0.0.8/src/socketify/wsgi.py
-drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-18 21:33:36.149634 socketify-0.0.8/src/socketify.egg-info/
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11055 2023-01-18 21:33:36.000000 socketify-0.0.8/src/socketify.egg-info/PKG-INFO
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10520 2023-01-18 21:33:36.000000 socketify-0.0.8/src/socketify.egg-info/SOURCES.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)        1 2023-01-18 21:33:36.000000 socketify-0.0.8/src/socketify.egg-info/dependency_links.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       29 2023-01-18 21:33:36.000000 socketify-0.0.8/src/socketify.egg-info/requires.txt
--rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       10 2023-01-18 21:33:36.000000 socketify-0.0.8/src/socketify.egg-info/top_level.txt
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.106839 socketify-0.0.9/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1070 2022-05-28 23:14:27.000000 socketify-0.0.9/LICENSE
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11055 2023-01-19 19:00:46.106839 socketify-0.0.9/PKG-INFO
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10390 2023-01-13 10:37:55.000000 socketify-0.0.9/README.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      658 2023-01-19 18:59:08.000000 socketify-0.0.9/pyproject.toml
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       38 2023-01-19 19:00:46.106839 socketify-0.0.9/setup.cfg
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2819 2023-01-19 18:59:04.000000 socketify-0.0.9/setup.py
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.030838 socketify-0.0.9/src/
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.058838 socketify-0.0.9/src/socketify/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      390 2023-01-19 18:57:23.000000 socketify-0.0.9/src/socketify/__init__.py
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       57 2023-01-07 14:55:58.000000 socketify-0.0.9/src/socketify/__main__.py
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    27408 2023-01-18 19:02:57.000000 socketify-0.0.9/src/socketify/asgi.py
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    14379 2023-01-18 19:03:03.000000 socketify-0.0.9/src/socketify/cli.py
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    13863 2023-01-18 20:07:15.000000 socketify-0.0.9/src/socketify/helpers.py
+-rwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)  2920456 2023-01-18 21:32:59.000000 socketify-0.0.9/src/socketify/libsocketify_darwin_amd64.so
+-rwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)  2751945 2023-01-18 21:32:59.000000 socketify-0.0.9/src/socketify/libsocketify_darwin_arm64.so
+-rwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)  3922512 2023-01-18 20:17:24.000000 socketify-0.0.9/src/socketify/libsocketify_linux_amd64.so
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)  2053632 2023-01-18 21:32:59.000000 socketify-0.0.9/src/socketify/libsocketify_windows_amd64.dll
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6543 2023-01-19 13:28:57.000000 socketify-0.0.9/src/socketify/loop.py
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.058838 socketify-0.0.9/src/socketify/native/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1215 2022-11-23 14:18:51.000000 socketify-0.0.9/src/socketify/native/Make.bat
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9984 2023-01-18 19:45:18.000000 socketify-0.0.9/src/socketify/native/Makefile
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.062838 socketify-0.0.9/src/socketify/native/__pycache__/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      196 2022-06-05 21:02:35.000000 socketify-0.0.9/src/socketify/native/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      200 2022-06-02 18:34:51.000000 socketify-0.0.9/src/socketify/native/__pycache__/__init__.pypy38.pyc
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5847 2022-10-25 15:03:30.000000 socketify-0.0.9/src/socketify/native/__pycache__/uv.cpython-310.pyc
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     7624 2022-11-01 12:17:09.000000 socketify-0.0.9/src/socketify/native/__pycache__/uv.pypy38.pyc
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)   536640 2023-01-18 19:58:49.000000 socketify-0.0.9/src/socketify/native/libsocketify.o
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.062838 socketify-0.0.9/src/socketify/native/src/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    18875 2023-01-07 14:55:58.000000 socketify-0.0.9/src/socketify/native/src/libsocketify.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5096 2023-01-07 14:55:58.000000 socketify-0.0.9/src/socketify/native/src/libsocketify.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10978 2022-11-14 19:14:51.000000 socketify-0.0.9/src/socketify/native/uv_selector.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    18776 2023-01-18 19:03:06.000000 socketify-0.0.9/src/socketify/native.py
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)   118334 2023-01-19 18:56:24.000000 socketify-0.0.9/src/socketify/socketify.py
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    12505 2023-01-08 19:36:25.000000 socketify-0.0.9/src/socketify/ssgi.py
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2161 2023-01-18 19:03:13.000000 socketify-0.0.9/src/socketify/status_codes.py
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22669 2023-01-18 19:02:48.000000 socketify-0.0.9/src/socketify/tasks.py
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.062838 socketify-0.0.9/src/socketify/uWebSockets/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      377 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/GNUmakefile
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11357 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/LICENSE
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      640 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/Makefile
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6024 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/README.md
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.062838 socketify-0.0.9/src/socketify/uWebSockets/benchmarks/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      631 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/benchmarks/Makefile
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2421 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/benchmarks/README.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6413 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/benchmarks/broadcast_test.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9523 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/benchmarks/load_test.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8328 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/benchmarks/scale_test.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3619 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/build.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      552 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/build.h
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.066839 socketify-0.0.9/src/socketify/uWebSockets/capi/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1972 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/Makefile
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.066839 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4572 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/Broadcast.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5628 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/BroadcastEchoServer.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2257 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/EchoServer.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      901 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/HelloWorld.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3729 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/HelloWorldAsync.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9539 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/RustHelloWorld.rs
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1737 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/ServerName.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8409 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/UpgradeAsync.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4038 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/examples/UpgradeSync.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    52633 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/libuwebsockets.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16238 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/capi/libuwebsockets.h
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.066839 socketify-0.0.9/src/socketify/uWebSockets/cluster/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       14 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/cluster/README.md
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.070839 socketify-0.0.9/src/socketify/uWebSockets/examples/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2730 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/Broadcast.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2661 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/BroadcastingEchoServer.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      438 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/Client.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1874 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/Crc32.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2079 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/EchoServer.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1939 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/EchoServerThreaded.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      566 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/HelloWorld.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1444 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/HelloWorldThreaded.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3163 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/Http3Server.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2882 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/HttpServer.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      216 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/README.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      963 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/ServerName.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5882 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/UpgradeAsync.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3510 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/UpgradeSync.cpp
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.070839 socketify-0.0.9/src/socketify/uWebSockets/examples/helpers/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3892 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/helpers/AsyncFileReader.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3207 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/helpers/AsyncFileStreamer.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      578 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/helpers/Middleware.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    12228 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/examples/helpers/optparse.h
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.074838 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5402 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/EpollEchoServer.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      232 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/EpollEchoServer.dict
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3505 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/EpollEchoServerPubSub.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      232 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/EpollEchoServerPubSub.dict
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6595 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/EpollHelloWorld.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      232 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/EpollHelloWorld.dict
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1762 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/Extensions.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4387 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/Http.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3008 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/Makefile
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1744 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/MultipartParser.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2111 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/PerMessageDeflate.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      307 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/QueryParser.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       31 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/QueryParser.dict
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1401 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/README.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4593 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/TopicTree.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       46 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/TopicTree.dict
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1586 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/WebSocket.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1377 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/helpers.h
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.074838 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      565 2023-01-18 19:02:02.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/Makefile
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2354 2023-01-18 19:02:02.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/README.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    59449 2023-01-18 19:02:02.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/epollFuzzer.svg
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    15884 2023-01-18 19:02:02.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/epoll_fuzzer.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4130 2023-01-18 19:02:02.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/test.c
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.074838 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/seed-corpus/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       53 2023-01-18 19:02:05.000000 socketify-0.0.9/src/socketify/uWebSockets/fuzzing/seed-corpus/README.md
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.078839 socketify-0.0.9/src/socketify/uWebSockets/misc/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22909 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/misc/READMORE.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    17816 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/misc/bigshot_lineup.png
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1229 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/misc/cert.pem
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1704 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/misc/key.pem
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11945 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/misc/logo.svg
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22974 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/misc/websocket_lineup.png
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.086839 socketify-0.0.9/src/socketify/uWebSockets/src/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    24818 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/App.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    13739 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/AsyncSocket.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2360 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/AsyncSocketData.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2229 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/BloomFilter.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     7857 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/ChunkedEncoding.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      890 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/ClientApp.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5315 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/Http3App.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6436 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/Http3Context.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      378 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/Http3ContextData.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      665 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/Http3Request.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4419 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/Http3Response.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      600 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/Http3ResponseData.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    21712 2023-01-18 19:57:50.000000 socketify-0.0.9/src/socketify/uWebSockets/src/HttpContext.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1652 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/HttpContextData.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    26798 2023-01-18 19:58:29.000000 socketify-0.0.9/src/socketify/uWebSockets/src/HttpParser.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22782 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/HttpResponse.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2952 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/HttpResponseData.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    13124 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/HttpRouter.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6625 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/Loop.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2884 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/LoopData.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2703 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/MessageParser.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    14436 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/MoveOnlyFunction.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8611 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/Multipart.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10940 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/PerMessageDeflate.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4670 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/ProxyParser.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4831 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/QueryParser.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11523 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/TopicTree.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1436 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/Utilities.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16147 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/WebSocket.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22076 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketContext.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3611 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketContextData.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2781 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketData.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9148 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketExtensions.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5576 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketHandshake.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16858 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketProtocol.h
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.086839 socketify-0.0.9/src/socketify/uWebSockets/tests/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2775 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/tests/BloomFilter.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     7241 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/tests/ChunkedEncoding.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4287 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/tests/ExtensionsNegotiator.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1575 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/tests/HttpParser.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9610 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/tests/HttpRouter.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      626 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/tests/Makefile
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1094 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/tests/README.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6190 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/tests/TopicTree.cpp
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2809 2023-01-18 19:02:01.000000 socketify-0.0.9/src/socketify/uWebSockets/tests/smoke.mjs
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.090839 socketify-0.0.9/src/socketify/uWebSockets/uSockets/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11357 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/LICENSE
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3141 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/Makefile
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1678 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/README.md
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.094839 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11392 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/API-CONVENTIONS.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9018 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/BREAKING-CHANGES.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9298 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/BUILDING.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    26978 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/CMakeLists.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2734 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/CONTRIBUTING.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4444 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/FUZZING.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5116 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/INCORPORATING.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    12517 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/LICENSE
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1179 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/OpenSSLConfig.cmake
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16853 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/PORTING.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2350 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/README.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6673 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/SANDBOXING.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8608 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/STYLE.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      170 2023-01-18 19:02:12.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/codereview.settings
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      175 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/go.mod
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1319 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/go.sum
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11078 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/sources.cmake
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11448 2023-01-18 19:58:41.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/bsd.o
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10432 2023-01-18 19:58:41.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/context.o
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      672 2023-01-18 19:58:42.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/epoll_kqueue.o
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.098839 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4217 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/echo_server.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    15650 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/hammer_test.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16070 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/hammer_test_unix.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5517 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/http3_client.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3582 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/http3_server.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4759 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/http_load_test.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4219 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/http_server.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10941 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/peer_verify_test.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4847 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/udp_benchmark.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      664 2023-01-18 19:58:42.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/gcd.o
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     7696 2023-01-18 19:58:42.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/libuv.o
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8008 2023-01-18 19:58:41.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/loop.o
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.102839 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     8187 2023-01-18 19:02:14.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/APIs.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4533 2023-01-18 19:02:14.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/BUILD-WINDOWS.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    64336 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/CHANGELOG
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16902 2023-01-18 19:45:16.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/CMakeCache.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11806 2023-01-18 19:02:14.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/CMakeLists.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      926 2023-01-18 19:02:14.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/CONTRIBUTORS.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      747 2023-01-18 19:02:14.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/Dockerfile
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9699 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/EXAMPLES.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1090 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/LICENSE
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1618 2023-01-18 19:02:14.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/LICENSE.chrome
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6725 2023-01-18 19:45:16.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/Makefile
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3920 2023-01-18 20:48:33.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/README.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      624 2023-01-18 19:02:14.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/appveyor-linux.yml
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      858 2023-01-18 19:02:14.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/appveyor-windows.cmd
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)      513 2023-01-18 19:02:14.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/appveyor-windows.yml
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     2451 2023-01-18 19:45:16.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/cmake_install.cmake
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.102839 socketify-0.0.9/src/socketify/uWebSockets/uSockets/misc/
+-rwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)     1467 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/misc/gen_test_certs.sh
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10991 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/misc/layout.png
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     9947 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/misc/manual.md
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       58 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/module.modulemap
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    18816 2023-01-18 19:58:42.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/openssl.o
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22824 2023-01-18 19:58:41.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/quic.o
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    17752 2023-01-18 19:58:42.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/sni_tree.o
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5680 2023-01-18 19:58:41.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/socket.o
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.106839 socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    22659 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/bsd.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    19316 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/context.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    16951 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/libusockets.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    15109 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/loop.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    34301 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/quic.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3214 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/quic.h
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     6760 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/socket.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     5094 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/udp.c
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.106839 socketify-0.0.9/src/socketify/uWebSockets/uSockets/tests/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     1867 2023-01-18 19:02:07.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/tests/sni_test.c
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)   117616 2023-01-18 19:58:42.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/uSockets_linux_amd64.a
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     4216 2023-01-18 19:58:41.000000 socketify-0.0.9/src/socketify/uWebSockets/uSockets/udp.o
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)     3138 2023-01-18 19:03:18.000000 socketify-0.0.9/src/socketify/uv.py
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    17710 2023-01-18 19:03:22.000000 socketify-0.0.9/src/socketify/wsgi.py
+drwxr-xr-x   0 cirospaciari  (1000) cirospaciari  (1000)        0 2023-01-19 19:00:46.058838 socketify-0.0.9/src/socketify.egg-info/
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    11055 2023-01-19 19:00:45.000000 socketify-0.0.9/src/socketify.egg-info/PKG-INFO
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)    10520 2023-01-19 19:00:45.000000 socketify-0.0.9/src/socketify.egg-info/SOURCES.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)        1 2023-01-19 19:00:45.000000 socketify-0.0.9/src/socketify.egg-info/dependency_links.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       29 2023-01-19 19:00:45.000000 socketify-0.0.9/src/socketify.egg-info/requires.txt
+-rw-r--r--   0 cirospaciari  (1000) cirospaciari  (1000)       10 2023-01-19 19:00:45.000000 socketify-0.0.9/src/socketify.egg-info/top_level.txt
```

### Comparing `socketify-0.0.8/LICENSE` & `socketify-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/PKG-INFO` & `socketify-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketify
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bringing WebSockets, Http/Https High Performance servers for PyPy3 and Python3
 Home-page: https://github.com/cirospaciari/socketify.py
 Author: Ciro Spaciari
 Author-email: Ciro Spaciari <ciro.spaciari@gmail.com>
 Project-URL: Homepage, https://github.com/cirospaciari/socketify.py
 Project-URL: Bug Tracker, https://github.com/cirospaciari/socketify.py/issues
 Platform: any
```

### Comparing `socketify-0.0.8/README.md` & `socketify-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/pyproject.toml` & `socketify-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["cffi>=1.0","setuptools>=58.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketify"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Ciro Spaciari", email="ciro.spaciari@gmail.com" },
 ]
 description = "Bringing WebSockets, Http/Https High Performance servers for PyPy3 and Python3"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `socketify-0.0.8/setup.py` & `socketify-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="socketify",
-    version="0.0.8",
+    version="0.0.9",
     platforms=["any"],
     author="Ciro Spaciari",
     author_email="ciro.spaciari@gmail.com",
     description="Bringing WebSockets, Http/Https High Performance servers for PyPy3 and Python3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cirospaciari/socketify.py",
```

### Comparing `socketify-0.0.8/src/socketify/asgi.py` & `socketify-0.0.9/src/socketify/asgi.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/cli.py` & `socketify-0.0.9/src/socketify/cli.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/helpers.py` & `socketify-0.0.9/src/socketify/helpers.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/libsocketify_darwin_amd64.so` & `socketify-0.0.9/src/socketify/libsocketify_darwin_amd64.so`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/libsocketify_darwin_arm64.so` & `socketify-0.0.9/src/socketify/libsocketify_darwin_arm64.so`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/libsocketify_linux_amd64.so` & `socketify-0.0.9/src/socketify/libsocketify_linux_amd64.so`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/libsocketify_windows_amd64.dll` & `socketify-0.0.9/src/socketify/libsocketify_windows_amd64.dll`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/loop.py` & `socketify-0.0.9/src/socketify/loop.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/native/Make.bat` & `socketify-0.0.9/src/socketify/native/Make.bat`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/native/Makefile` & `socketify-0.0.9/src/socketify/native/Makefile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/native/__pycache__/uv.cpython-310.pyc` & `socketify-0.0.9/src/socketify/native/__pycache__/uv.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/native/__pycache__/uv.pypy38.pyc` & `socketify-0.0.9/src/socketify/native/__pycache__/uv.pypy38.pyc`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/native/libsocketify.o` & `socketify-0.0.9/src/socketify/native/libsocketify.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/native/src/libsocketify.cpp` & `socketify-0.0.9/src/socketify/native/src/libsocketify.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/native/src/libsocketify.h` & `socketify-0.0.9/src/socketify/native/src/libsocketify.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/native/uv_selector.txt` & `socketify-0.0.9/src/socketify/native/uv_selector.txt`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/native.py` & `socketify-0.0.9/src/socketify/native.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/socketify.py` & `socketify-0.0.9/src/socketify/socketify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1139,14 +1139,19 @@
         self.app = app
         self._cork_handler = None
         self._for_each_topic_handler = None
         self.socket_data_id = None
         self.socket_data = None
         self.got_socket_data = False
 
+
+    def clone(self):
+        # clone and preserve this websocket in another instance
+        return WebSocket(self.websocket, self.app)
+
     def trigger_for_each_topic_handler(self, topic):
         if hasattr(self, "_for_each_topic_handler") and hasattr(
             self._for_each_topic_handler, "__call__"
         ):
             try:
                 if inspect.iscoroutinefunction(self._for_each_topic_handler):
                     raise RuntimeError(
```

### Comparing `socketify-0.0.8/src/socketify/ssgi.py` & `socketify-0.0.9/src/socketify/ssgi.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/status_codes.py` & `socketify-0.0.9/src/socketify/status_codes.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/tasks.py` & `socketify-0.0.9/src/socketify/tasks.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/LICENSE` & `socketify-0.0.9/src/socketify/uWebSockets/LICENSE`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/Makefile` & `socketify-0.0.9/src/socketify/uWebSockets/Makefile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/README.md` & `socketify-0.0.9/src/socketify/uWebSockets/README.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/benchmarks/Makefile` & `socketify-0.0.9/src/socketify/uWebSockets/benchmarks/Makefile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/benchmarks/README.md` & `socketify-0.0.9/src/socketify/uWebSockets/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/benchmarks/broadcast_test.c` & `socketify-0.0.9/src/socketify/uWebSockets/benchmarks/broadcast_test.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/benchmarks/load_test.c` & `socketify-0.0.9/src/socketify/uWebSockets/benchmarks/load_test.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/benchmarks/scale_test.c` & `socketify-0.0.9/src/socketify/uWebSockets/benchmarks/scale_test.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/build.c` & `socketify-0.0.9/src/socketify/uWebSockets/build.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/build.h` & `socketify-0.0.9/src/socketify/uWebSockets/build.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/Makefile` & `socketify-0.0.9/src/socketify/uWebSockets/capi/Makefile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/examples/Broadcast.c` & `socketify-0.0.9/src/socketify/uWebSockets/capi/examples/Broadcast.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/examples/BroadcastEchoServer.c` & `socketify-0.0.9/src/socketify/uWebSockets/capi/examples/BroadcastEchoServer.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/examples/EchoServer.c` & `socketify-0.0.9/src/socketify/uWebSockets/capi/examples/EchoServer.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/examples/HelloWorld.c` & `socketify-0.0.9/src/socketify/uWebSockets/capi/examples/HelloWorld.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/examples/HelloWorldAsync.c` & `socketify-0.0.9/src/socketify/uWebSockets/capi/examples/HelloWorldAsync.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/examples/RustHelloWorld.rs` & `socketify-0.0.9/src/socketify/uWebSockets/capi/examples/RustHelloWorld.rs`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/examples/ServerName.c` & `socketify-0.0.9/src/socketify/uWebSockets/capi/examples/ServerName.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/examples/UpgradeAsync.c` & `socketify-0.0.9/src/socketify/uWebSockets/capi/examples/UpgradeAsync.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/examples/UpgradeSync.c` & `socketify-0.0.9/src/socketify/uWebSockets/capi/examples/UpgradeSync.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/libuwebsockets.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/capi/libuwebsockets.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/capi/libuwebsockets.h` & `socketify-0.0.9/src/socketify/uWebSockets/capi/libuwebsockets.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/Broadcast.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/Broadcast.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/BroadcastingEchoServer.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/BroadcastingEchoServer.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/Crc32.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/Crc32.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/EchoServer.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/EchoServer.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/EchoServerThreaded.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/EchoServerThreaded.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/HelloWorld.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/HelloWorld.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/HelloWorldThreaded.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/HelloWorldThreaded.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/Http3Server.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/Http3Server.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/HttpServer.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/HttpServer.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/ServerName.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/ServerName.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/UpgradeAsync.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/UpgradeAsync.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/UpgradeSync.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/examples/UpgradeSync.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/helpers/AsyncFileReader.h` & `socketify-0.0.9/src/socketify/uWebSockets/examples/helpers/AsyncFileReader.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/helpers/AsyncFileStreamer.h` & `socketify-0.0.9/src/socketify/uWebSockets/examples/helpers/AsyncFileStreamer.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/helpers/Middleware.h` & `socketify-0.0.9/src/socketify/uWebSockets/examples/helpers/Middleware.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/examples/helpers/optparse.h` & `socketify-0.0.9/src/socketify/uWebSockets/examples/helpers/optparse.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/EpollEchoServer.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/EpollEchoServer.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/EpollEchoServerPubSub.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/EpollEchoServerPubSub.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/EpollHelloWorld.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/EpollHelloWorld.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/Extensions.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/Extensions.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/Http.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/Http.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/Makefile` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/Makefile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/MultipartParser.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/MultipartParser.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/PerMessageDeflate.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/PerMessageDeflate.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/README.md` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/README.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/TopicTree.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/TopicTree.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/WebSocket.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/WebSocket.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/helpers.h` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/helpers.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/Makefile` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/Makefile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/README.md` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/README.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/epollFuzzer.svg` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/epollFuzzer.svg`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/epoll_fuzzer.h` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/epoll_fuzzer.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/test.c` & `socketify-0.0.9/src/socketify/uWebSockets/fuzzing/libEpollFuzzer/test.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/misc/READMORE.md` & `socketify-0.0.9/src/socketify/uWebSockets/misc/READMORE.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/misc/bigshot_lineup.png` & `socketify-0.0.9/src/socketify/uWebSockets/misc/bigshot_lineup.png`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/misc/cert.pem` & `socketify-0.0.9/src/socketify/uWebSockets/misc/cert.pem`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/misc/key.pem` & `socketify-0.0.9/src/socketify/uWebSockets/misc/key.pem`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/misc/logo.svg` & `socketify-0.0.9/src/socketify/uWebSockets/misc/logo.svg`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/misc/websocket_lineup.png` & `socketify-0.0.9/src/socketify/uWebSockets/misc/websocket_lineup.png`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/App.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/App.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/AsyncSocket.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/AsyncSocket.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/AsyncSocketData.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/AsyncSocketData.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/BloomFilter.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/BloomFilter.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/ChunkedEncoding.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/ChunkedEncoding.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/ClientApp.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/ClientApp.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/Http3App.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/Http3App.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/Http3Context.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/Http3Context.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/Http3Request.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/Http3Request.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/Http3Response.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/Http3Response.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/Http3ResponseData.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/Http3ResponseData.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/HttpContext.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/HttpContext.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/HttpContextData.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/HttpContextData.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/HttpParser.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/HttpParser.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/HttpResponse.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/HttpResponse.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/HttpResponseData.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/HttpResponseData.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/HttpRouter.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/HttpRouter.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/Loop.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/Loop.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/LoopData.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/LoopData.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/MessageParser.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/MessageParser.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/MoveOnlyFunction.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/MoveOnlyFunction.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/Multipart.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/Multipart.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/PerMessageDeflate.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/PerMessageDeflate.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/ProxyParser.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/ProxyParser.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/QueryParser.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/QueryParser.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/TopicTree.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/TopicTree.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/Utilities.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/Utilities.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/WebSocket.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/WebSocket.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketContext.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketContext.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketContextData.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketContextData.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketData.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketData.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketExtensions.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketExtensions.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketHandshake.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketHandshake.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/src/WebSocketProtocol.h` & `socketify-0.0.9/src/socketify/uWebSockets/src/WebSocketProtocol.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/tests/BloomFilter.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/tests/BloomFilter.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/tests/ChunkedEncoding.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/tests/ChunkedEncoding.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/tests/ExtensionsNegotiator.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/tests/ExtensionsNegotiator.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/tests/HttpParser.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/tests/HttpParser.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/tests/HttpRouter.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/tests/HttpRouter.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/tests/Makefile` & `socketify-0.0.9/src/socketify/uWebSockets/tests/Makefile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/tests/README.md` & `socketify-0.0.9/src/socketify/uWebSockets/tests/README.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/tests/TopicTree.cpp` & `socketify-0.0.9/src/socketify/uWebSockets/tests/TopicTree.cpp`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/tests/smoke.mjs` & `socketify-0.0.9/src/socketify/uWebSockets/tests/smoke.mjs`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/LICENSE` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/LICENSE`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/Makefile` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/Makefile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/README.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/README.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/API-CONVENTIONS.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/API-CONVENTIONS.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/BREAKING-CHANGES.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/BREAKING-CHANGES.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/BUILDING.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/BUILDING.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/CMakeLists.txt` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/CONTRIBUTING.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/FUZZING.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/FUZZING.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/INCORPORATING.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/INCORPORATING.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/LICENSE` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/LICENSE`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/OpenSSLConfig.cmake` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/OpenSSLConfig.cmake`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/PORTING.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/PORTING.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/README.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/README.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/SANDBOXING.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/SANDBOXING.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/STYLE.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/STYLE.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/go.sum` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/go.sum`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/boringssl/sources.cmake` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/boringssl/sources.cmake`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/bsd.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/bsd.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/context.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/context.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/epoll_kqueue.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/epoll_kqueue.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/echo_server.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/echo_server.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/hammer_test.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/hammer_test.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/hammer_test_unix.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/hammer_test_unix.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/http3_client.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/http3_client.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/http3_server.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/http3_server.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/http_load_test.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/http_load_test.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/http_server.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/http_server.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/peer_verify_test.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/peer_verify_test.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/examples/udp_benchmark.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/examples/udp_benchmark.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/gcd.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/gcd.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/libuv.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/libuv.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/loop.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/loop.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/APIs.txt` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/APIs.txt`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/BUILD-WINDOWS.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/BUILD-WINDOWS.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/CHANGELOG` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/CHANGELOG`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/CMakeCache.txt` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/CMakeLists.txt` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/CONTRIBUTORS.txt` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/CONTRIBUTORS.txt`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/Dockerfile` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/Dockerfile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/EXAMPLES.txt` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/EXAMPLES.txt`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/LICENSE` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/LICENSE`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/LICENSE.chrome` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/LICENSE.chrome`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/Makefile` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/Makefile`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/README.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/README.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/appveyor-linux.yml` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/appveyor-linux.yml`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/appveyor-windows.cmd` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/appveyor-windows.cmd`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/appveyor-windows.yml` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/appveyor-windows.yml`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/lsquic/cmake_install.cmake` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/lsquic/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/misc/gen_test_certs.sh` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/misc/gen_test_certs.sh`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/misc/layout.png` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/misc/layout.png`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/misc/manual.md` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/misc/manual.md`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/openssl.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/openssl.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/quic.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/quic.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/sni_tree.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/sni_tree.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/socket.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/socket.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/bsd.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/bsd.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/context.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/context.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/libusockets.h` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/libusockets.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/loop.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/loop.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/quic.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/quic.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/quic.h` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/quic.h`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/socket.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/socket.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/src/udp.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/src/udp.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/tests/sni_test.c` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/tests/sni_test.c`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/uSockets_linux_amd64.a` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/uSockets_linux_amd64.a`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uWebSockets/uSockets/udp.o` & `socketify-0.0.9/src/socketify/uWebSockets/uSockets/udp.o`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/uv.py` & `socketify-0.0.9/src/socketify/uv.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify/wsgi.py` & `socketify-0.0.9/src/socketify/wsgi.py`

 * *Files identical despite different names*

### Comparing `socketify-0.0.8/src/socketify.egg-info/PKG-INFO` & `socketify-0.0.9/src/socketify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketify
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bringing WebSockets, Http/Https High Performance servers for PyPy3 and Python3
 Home-page: https://github.com/cirospaciari/socketify.py
 Author: Ciro Spaciari
 Author-email: Ciro Spaciari <ciro.spaciari@gmail.com>
 Project-URL: Homepage, https://github.com/cirospaciari/socketify.py
 Project-URL: Bug Tracker, https://github.com/cirospaciari/socketify.py/issues
 Platform: any
```

### Comparing `socketify-0.0.8/src/socketify.egg-info/SOURCES.txt` & `socketify-0.0.9/src/socketify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

