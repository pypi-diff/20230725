# Comparing `tmp/pip_services4_observability-0.0.2.tar.gz` & `tmp/pip_services4_observability-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_observability-0.0.2.tar", last modified: Tue Jul 25 19:05:03 2023, max compression
+gzip compressed data, was "pip_services4_observability-0.0.3.tar", last modified: Tue Jul 25 19:35:44 2023, max compression
```

## Comparing `pip_services4_observability-0.0.2.tar` & `pip_services4_observability-0.0.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.255613 pip_services4_observability-0.0.2/
--rw-rw-rw-   0        0        0      297 2023-07-25 19:03:18.000000 pip_services4_observability-0.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_observability-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_observability-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4079 2023-07-25 19:05:03.255613 pip_services4_observability-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3066 2023-07-25 17:52:38.000000 pip_services4_observability-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.171504 pip_services4_observability-0.0.2/pip_services4_observability/
--rw-rw-rw-   0        0        0      308 2023-07-25 10:38:57.000000 pip_services4_observability-0.0.2/pip_services4_observability/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.209564 pip_services4_observability-0.0.2/pip_services4_observability/build/
--rw-rw-rw-   0        0        0     2680 2023-07-25 19:02:58.000000 pip_services4_observability-0.0.2/pip_services4_observability/build/DefaultObservabilityFactory.py
--rw-rw-rw-   0        0        0        0 2023-07-25 18:57:46.000000 pip_services4_observability-0.0.2/pip_services4_observability/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.221072 pip_services4_observability-0.0.2/pip_services4_observability/count/
--rw-rw-rw-   0        0        0     8414 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/CachedCounters.py
--rw-rw-rw-   0        0        0     5102 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/CompositeCounters.py
--rw-rw-rw-   0        0        0     1461 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/Counter.py
--rw-rw-rw-   0        0        0     1523 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/CounterTiming.py
--rw-rw-rw-   0        0        0     1165 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/CounterType.py
--rw-rw-rw-   0        0        0     1781 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/DefaultCountersFactory.py
--rw-rw-rw-   0        0        0      936 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/ICounterTimingCallback.py
--rw-rw-rw-   0        0        0     3223 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/ICounters.py
--rw-rw-rw-   0        0        0     3729 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/LogCounters.py
--rw-rw-rw-   0        0        0     2681 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/NullCounters.py
--rw-rw-rw-   0        0        0     1171 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/pip_services4_observability/count/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.232586 pip_services4_observability-0.0.2/pip_services4_observability/log/
--rw-rw-rw-   0        0        0     4548 2023-07-25 17:37:10.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/CachedLogger.py
--rw-rw-rw-   0        0        0     2908 2023-07-25 17:37:50.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/CompositeLogger.py
--rw-rw-rw-   0        0        0     2621 2023-07-25 17:41:00.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/ConsoleLogger.py
--rw-rw-rw-   0        0        0     1731 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/DefaultLoggerFactory.py
--rw-rw-rw-   0        0        0     5023 2023-07-25 17:36:05.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/ILogger.py
--rw-rw-rw-   0        0        0     1032 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/LogLevel.py
--rw-rw-rw-   0        0        0     2794 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/LogLevelConverter.py
--rw-rw-rw-   0        0        0     1771 2023-07-25 17:42:59.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/LogMessage.py
--rw-rw-rw-   0        0        0     9285 2023-07-25 17:42:17.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/Logger.py
--rw-rw-rw-   0        0        0     4611 2023-07-25 17:43:37.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/NullLogger.py
--rw-rw-rw-   0        0        0     1133 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/pip_services4_observability/log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.241100 pip_services4_observability-0.0.2/pip_services4_observability/trace/
--rw-rw-rw-   0        0        0     7643 2023-07-25 17:45:10.000000 pip_services4_observability-0.0.2/pip_services4_observability/trace/CachedTracer.py
--rw-rw-rw-   0        0        0     3983 2023-07-25 17:46:04.000000 pip_services4_observability-0.0.2/pip_services4_observability/trace/CompositeTracer.py
--rw-rw-rw-   0        0        0     1567 2023-07-25 10:55:44.000000 pip_services4_observability-0.0.2/pip_services4_observability/trace/DefaultTracerFactory.py
--rw-rw-rw-   0        0        0     1769 2023-07-25 17:46:30.000000 pip_services4_observability-0.0.2/pip_services4_observability/trace/ITracer.py
--rw-rw-rw-   0        0        0     4361 2023-07-25 17:47:54.000000 pip_services4_observability-0.0.2/pip_services4_observability/trace/LogTracer.py
--rw-rw-rw-   0        0        0     2177 2023-07-25 17:48:27.000000 pip_services4_observability-0.0.2/pip_services4_observability/trace/NullTracer.py
--rw-rw-rw-   0        0        0     1911 2023-07-25 17:49:04.000000 pip_services4_observability-0.0.2/pip_services4_observability/trace/OperationTrace.py
--rw-rw-rw-   0        0        0     1893 2023-07-25 17:50:15.000000 pip_services4_observability-0.0.2/pip_services4_observability/trace/TraceTiming.py
--rw-rw-rw-   0        0        0      508 2021-10-25 15:30:28.000000 pip_services4_observability-0.0.2/pip_services4_observability/trace/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.206559 pip_services4_observability-0.0.2/pip_services4_observability.egg-info/
--rw-rw-rw-   0        0        0     4079 2023-07-25 19:05:03.000000 pip_services4_observability-0.0.2/pip_services4_observability.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2418 2023-07-25 19:05:03.000000 pip_services4_observability-0.0.2/pip_services4_observability.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:05:03.000000 pip_services4_observability-0.0.2/pip_services4_observability.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-25 19:05:03.000000 pip_services4_observability-0.0.2/pip_services4_observability.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-07-25 19:05:03.000000 pip_services4_observability-0.0.2/pip_services4_observability.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 18:00:09.000000 pip_services4_observability-0.0.2/pip_services4_observability.egg-info/zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-25 19:05:03.261129 pip_services4_observability-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1754 2023-07-25 19:03:18.000000 pip_services4_observability-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.166504 pip_services4_observability-0.0.2/test/
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.245101 pip_services4_observability-0.0.2/test/count/
--rw-rw-rw-   0        0        0     2054 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/test/count/CountersFixture.py
--rw-rw-rw-   0        0        0        0 2020-12-11 04:21:14.000000 pip_services4_observability-0.0.2/test/count/__init__.py
--rw-rw-rw-   0        0        0     1049 2023-07-25 10:55:44.000000 pip_services4_observability-0.0.2/test/count/test_LogCounters.py
--rw-rw-rw-   0        0        0      750 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/test/count/test_NullCounters.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.250613 pip_services4_observability-0.0.2/test/log/
--rw-rw-rw-   0        0        0     1214 2023-07-25 17:58:33.000000 pip_services4_observability-0.0.2/test/log/LoggerFixture.py
--rw-rw-rw-   0        0        0        0 2020-12-11 04:21:14.000000 pip_services4_observability-0.0.2/test/log/__init__.py
--rw-rw-rw-   0        0        0     1094 2023-07-25 10:55:44.000000 pip_services4_observability-0.0.2/test/log/test_CompositeLogger.py
--rw-rw-rw-   0        0        0      668 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/test/log/test_ConsoleLogger.py
--rw-rw-rw-   0        0        0      767 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/test/log/test_LogLevelConverter.py
--rw-rw-rw-   0        0        0      665 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.2/test/log/test_NullLogger.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:05:03.253613 pip_services4_observability-0.0.2/test/trace/
--rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_observability-0.0.2/test/trace/__init__.py
--rw-rw-rw-   0        0        0     1121 2023-07-25 17:57:28.000000 pip_services4_observability-0.0.2/test/trace/test_LogTracer.py
--rw-rw-rw-   0        0        0      818 2023-07-25 17:57:28.000000 pip_services4_observability-0.0.2/test/trace/test_NullTracer.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.723214 pip_services4_observability-0.0.3/
+-rw-rw-rw-   0        0        0      297 2023-07-25 19:33:56.000000 pip_services4_observability-0.0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_observability-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_observability-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4079 2023-07-25 19:35:44.724214 pip_services4_observability-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3066 2023-07-25 17:52:38.000000 pip_services4_observability-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.654735 pip_services4_observability-0.0.3/pip_services4_observability/
+-rw-rw-rw-   0        0        0      308 2023-07-25 10:38:57.000000 pip_services4_observability-0.0.3/pip_services4_observability/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.671737 pip_services4_observability-0.0.3/pip_services4_observability/build/
+-rw-rw-rw-   0        0        0     2680 2023-07-25 19:02:58.000000 pip_services4_observability-0.0.3/pip_services4_observability/build/DefaultObservabilityFactory.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 18:57:46.000000 pip_services4_observability-0.0.3/pip_services4_observability/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.684737 pip_services4_observability-0.0.3/pip_services4_observability/count/
+-rw-rw-rw-   0        0        0     8414 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/CachedCounters.py
+-rw-rw-rw-   0        0        0     5102 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/CompositeCounters.py
+-rw-rw-rw-   0        0        0     1461 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/Counter.py
+-rw-rw-rw-   0        0        0     1523 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/CounterTiming.py
+-rw-rw-rw-   0        0        0     1165 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/CounterType.py
+-rw-rw-rw-   0        0        0     1781 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/DefaultCountersFactory.py
+-rw-rw-rw-   0        0        0      936 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/ICounterTimingCallback.py
+-rw-rw-rw-   0        0        0     3223 2023-07-25 10:45:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/ICounters.py
+-rw-rw-rw-   0        0        0     3729 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/LogCounters.py
+-rw-rw-rw-   0        0        0     2681 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/NullCounters.py
+-rw-rw-rw-   0        0        0     1171 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/pip_services4_observability/count/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.696737 pip_services4_observability-0.0.3/pip_services4_observability/log/
+-rw-rw-rw-   0        0        0     4548 2023-07-25 17:37:10.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/CachedLogger.py
+-rw-rw-rw-   0        0        0     2908 2023-07-25 17:37:50.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/CompositeLogger.py
+-rw-rw-rw-   0        0        0     2621 2023-07-25 17:41:00.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/ConsoleLogger.py
+-rw-rw-rw-   0        0        0     1731 2023-07-25 10:50:19.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/DefaultLoggerFactory.py
+-rw-rw-rw-   0        0        0     5023 2023-07-25 17:36:05.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/ILogger.py
+-rw-rw-rw-   0        0        0     1032 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/LogLevel.py
+-rw-rw-rw-   0        0        0     2794 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/LogLevelConverter.py
+-rw-rw-rw-   0        0        0     1771 2023-07-25 17:42:59.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/LogMessage.py
+-rw-rw-rw-   0        0        0     9285 2023-07-25 17:42:17.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/Logger.py
+-rw-rw-rw-   0        0        0     4611 2023-07-25 17:43:37.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/NullLogger.py
+-rw-rw-rw-   0        0        0     1133 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/pip_services4_observability/log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.707785 pip_services4_observability-0.0.3/pip_services4_observability/trace/
+-rw-rw-rw-   0        0        0     7643 2023-07-25 17:45:10.000000 pip_services4_observability-0.0.3/pip_services4_observability/trace/CachedTracer.py
+-rw-rw-rw-   0        0        0     3983 2023-07-25 17:46:04.000000 pip_services4_observability-0.0.3/pip_services4_observability/trace/CompositeTracer.py
+-rw-rw-rw-   0        0        0     1567 2023-07-25 10:55:44.000000 pip_services4_observability-0.0.3/pip_services4_observability/trace/DefaultTracerFactory.py
+-rw-rw-rw-   0        0        0     1769 2023-07-25 17:46:30.000000 pip_services4_observability-0.0.3/pip_services4_observability/trace/ITracer.py
+-rw-rw-rw-   0        0        0     4361 2023-07-25 17:47:54.000000 pip_services4_observability-0.0.3/pip_services4_observability/trace/LogTracer.py
+-rw-rw-rw-   0        0        0     2177 2023-07-25 17:48:27.000000 pip_services4_observability-0.0.3/pip_services4_observability/trace/NullTracer.py
+-rw-rw-rw-   0        0        0     1911 2023-07-25 17:49:04.000000 pip_services4_observability-0.0.3/pip_services4_observability/trace/OperationTrace.py
+-rw-rw-rw-   0        0        0     1893 2023-07-25 17:50:15.000000 pip_services4_observability-0.0.3/pip_services4_observability/trace/TraceTiming.py
+-rw-rw-rw-   0        0        0      508 2021-10-25 15:30:28.000000 pip_services4_observability-0.0.3/pip_services4_observability/trace/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.668735 pip_services4_observability-0.0.3/pip_services4_observability.egg-info/
+-rw-rw-rw-   0        0        0     4079 2023-07-25 19:35:44.000000 pip_services4_observability-0.0.3/pip_services4_observability.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2418 2023-07-25 19:35:44.000000 pip_services4_observability-0.0.3/pip_services4_observability.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 19:35:44.000000 pip_services4_observability-0.0.3/pip_services4_observability.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-25 19:35:44.000000 pip_services4_observability-0.0.3/pip_services4_observability.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-07-25 19:35:44.000000 pip_services4_observability-0.0.3/pip_services4_observability.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 18:00:09.000000 pip_services4_observability-0.0.3/pip_services4_observability.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-25 19:35:44.725214 pip_services4_observability-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1754 2023-07-25 19:35:40.000000 pip_services4_observability-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.646735 pip_services4_observability-0.0.3/test/
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.711790 pip_services4_observability-0.0.3/test/count/
+-rw-rw-rw-   0        0        0     2054 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/test/count/CountersFixture.py
+-rw-rw-rw-   0        0        0        0 2020-12-11 04:21:14.000000 pip_services4_observability-0.0.3/test/count/__init__.py
+-rw-rw-rw-   0        0        0     1049 2023-07-25 10:55:44.000000 pip_services4_observability-0.0.3/test/count/test_LogCounters.py
+-rw-rw-rw-   0        0        0      750 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/test/count/test_NullCounters.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.718826 pip_services4_observability-0.0.3/test/log/
+-rw-rw-rw-   0        0        0     1214 2023-07-25 17:58:33.000000 pip_services4_observability-0.0.3/test/log/LoggerFixture.py
+-rw-rw-rw-   0        0        0        0 2020-12-11 04:21:14.000000 pip_services4_observability-0.0.3/test/log/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-07-25 10:55:44.000000 pip_services4_observability-0.0.3/test/log/test_CompositeLogger.py
+-rw-rw-rw-   0        0        0      668 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/test/log/test_ConsoleLogger.py
+-rw-rw-rw-   0        0        0      767 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/test/log/test_LogLevelConverter.py
+-rw-rw-rw-   0        0        0      665 2023-07-25 10:45:00.000000 pip_services4_observability-0.0.3/test/log/test_NullLogger.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:35:44.722213 pip_services4_observability-0.0.3/test/trace/
+-rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_observability-0.0.3/test/trace/__init__.py
+-rw-rw-rw-   0        0        0     1121 2023-07-25 17:57:28.000000 pip_services4_observability-0.0.3/test/trace/test_LogTracer.py
+-rw-rw-rw-   0        0        0      818 2023-07-25 17:57:28.000000 pip_services4_observability-0.0.3/test/trace/test_NullTracer.py
```

### Comparing `pip_services4_observability-0.0.2/LICENSE` & `pip_services4_observability-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/PKG-INFO` & `pip_services4_observability-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_observability
-Version: 0.0.2
+Version: 0.0.3
 Summary: Observability components for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-observability-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_observability-0.0.2/README.md` & `pip_services4_observability-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/build/DefaultObservabilityFactory.py` & `pip_services4_observability-0.0.3/pip_services4_observability/build/DefaultObservabilityFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/CachedCounters.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/CachedCounters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/CompositeCounters.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/CompositeCounters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/Counter.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/Counter.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/CounterTiming.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/CounterTiming.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/CounterType.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/CounterType.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/DefaultCountersFactory.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/DefaultCountersFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/ICounterTimingCallback.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/ICounterTimingCallback.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/ICounters.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/ICounters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/LogCounters.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/LogCounters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/NullCounters.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/NullCounters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/count/__init__.py` & `pip_services4_observability-0.0.3/pip_services4_observability/count/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/CachedLogger.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/CachedLogger.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/CompositeLogger.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/CompositeLogger.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/ConsoleLogger.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/ConsoleLogger.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/DefaultLoggerFactory.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/DefaultLoggerFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/ILogger.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/ILogger.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/LogLevel.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/LogLevel.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/LogLevelConverter.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/LogLevelConverter.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/LogMessage.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/LogMessage.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/Logger.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/Logger.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/NullLogger.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/NullLogger.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/log/__init__.py` & `pip_services4_observability-0.0.3/pip_services4_observability/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/trace/CachedTracer.py` & `pip_services4_observability-0.0.3/pip_services4_observability/trace/CachedTracer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/trace/CompositeTracer.py` & `pip_services4_observability-0.0.3/pip_services4_observability/trace/CompositeTracer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/trace/DefaultTracerFactory.py` & `pip_services4_observability-0.0.3/pip_services4_observability/trace/DefaultTracerFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/trace/ITracer.py` & `pip_services4_observability-0.0.3/pip_services4_observability/trace/ITracer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/trace/LogTracer.py` & `pip_services4_observability-0.0.3/pip_services4_observability/trace/LogTracer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/trace/NullTracer.py` & `pip_services4_observability-0.0.3/pip_services4_observability/trace/NullTracer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/trace/OperationTrace.py` & `pip_services4_observability-0.0.3/pip_services4_observability/trace/OperationTrace.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability/trace/TraceTiming.py` & `pip_services4_observability-0.0.3/pip_services4_observability/trace/TraceTiming.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability.egg-info/PKG-INFO` & `pip_services4_observability-0.0.3/pip_services4_observability.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-observability
-Version: 0.0.2
+Version: 0.0.3
 Summary: Observability components for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-observability-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_observability-0.0.2/pip_services4_observability.egg-info/SOURCES.txt` & `pip_services4_observability-0.0.3/pip_services4_observability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/setup.py` & `pip_services4_observability-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 try:
     readme = open('README.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_observability',
-    version='0.0.2',
+    version='0.0.3',
     url='https://github.com/pip-services4/pip-services4-python/pip-services4-observability-python',
     license='MIT',
     description='Observability components for Pip.Services in Python',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['config', 'data', 'test']),
     include_package_data=True,
     zip_safe=True,
     platforms='any',
     install_requires=[
-        'pip_services4_commons >= 0.0.2, < 4.0',
-        'pip_services4_components >= 0.0.2, < 4.0',
+        'pip_services4_commons >= 0.0.2, < 1.0',
+        'pip_services4_components >= 0.0.2, < 1.0',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

### Comparing `pip_services4_observability-0.0.2/test/count/CountersFixture.py` & `pip_services4_observability-0.0.3/test/count/CountersFixture.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/test/count/test_LogCounters.py` & `pip_services4_observability-0.0.3/test/count/test_LogCounters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/test/count/test_NullCounters.py` & `pip_services4_observability-0.0.3/test/count/test_NullCounters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/test/log/LoggerFixture.py` & `pip_services4_observability-0.0.3/test/log/LoggerFixture.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/test/log/test_CompositeLogger.py` & `pip_services4_observability-0.0.3/test/log/test_CompositeLogger.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/test/log/test_ConsoleLogger.py` & `pip_services4_observability-0.0.3/test/log/test_ConsoleLogger.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/test/log/test_LogLevelConverter.py` & `pip_services4_observability-0.0.3/test/log/test_LogLevelConverter.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/test/log/test_NullLogger.py` & `pip_services4_observability-0.0.3/test/log/test_NullLogger.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/test/trace/test_LogTracer.py` & `pip_services4_observability-0.0.3/test/trace/test_LogTracer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_observability-0.0.2/test/trace/test_NullTracer.py` & `pip_services4_observability-0.0.3/test/trace/test_NullTracer.py`

 * *Files identical despite different names*

