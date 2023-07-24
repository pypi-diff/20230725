# Comparing `tmp/redis-docker-harness-0.0.3.tar.gz` & `tmp/redis-docker-harness-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-docker-harness-0.0.3.tar", last modified: Sun Jul  9 22:46:06 2023, max compression
+gzip compressed data, was "redis-docker-harness-0.0.4.tar", last modified: Mon Jul 24 21:56:10 2023, max compression
```

## Comparing `redis-docker-harness-0.0.3.tar` & `redis-docker-harness-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-09 22:46:06.527516 redis-docker-harness-0.0.3/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      322 2023-07-09 22:44:55.000000 redis-docker-harness-0.0.3/CHANGES.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      125 2021-09-21 22:04:15.000000 redis-docker-harness-0.0.3/DESCRIPTION.rst
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 redis-docker-harness-0.0.3/MANIFEST.in
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1191 2023-07-09 22:46:06.527516 redis-docker-harness-0.0.3/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      478 2021-09-21 23:31:38.000000 redis-docker-harness-0.0.3/README.md
--rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-09 22:46:06.527516 redis-docker-harness-0.0.3/setup.cfg
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1045 2023-07-09 22:44:55.000000 redis-docker-harness-0.0.3/setup.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-09 22:46:06.523517 redis-docker-harness-0.0.3/src/
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-09 22:46:06.523517 redis-docker-harness-0.0.3/src/rdh/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      185 2023-07-06 23:08:08.000000 redis-docker-harness-0.0.3/src/rdh/__init__.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     3388 2023-07-09 22:42:14.000000 redis-docker-harness-0.0.3/src/rdh/_argparse.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      203 2021-09-21 22:33:02.000000 redis-docker-harness-0.0.3/src/rdh/_log.py
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     2502 2023-07-06 23:08:08.000000 redis-docker-harness-0.0.3/src/rdh/_redis.py
-drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-09 22:46:06.523517 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/
--rw-rw-r--   0 fracpete (62904) fracpete (62904)     1191 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/PKG-INFO
--rw-rw-r--   0 fracpete (62904) fracpete (62904)      372 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/SOURCES.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/dependency_links.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/requires.txt
--rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2023-07-09 22:46:06.000000 redis-docker-harness-0.0.3/src/redis_docker_harness.egg-info/top_level.txt
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-24 21:56:10.395900 redis-docker-harness-0.0.4/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      698 2023-07-24 21:55:37.000000 redis-docker-harness-0.0.4/CHANGES.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      125 2021-09-21 22:04:15.000000 redis-docker-harness-0.0.4/DESCRIPTION.rst
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       44 2021-08-14 06:44:26.000000 redis-docker-harness-0.0.4/MANIFEST.in
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1631 2023-07-24 21:56:10.395900 redis-docker-harness-0.0.4/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      478 2021-09-21 23:31:38.000000 redis-docker-harness-0.0.4/README.md
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)       38 2023-07-24 21:56:10.395900 redis-docker-harness-0.0.4/setup.cfg
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1045 2023-07-24 21:55:01.000000 redis-docker-harness-0.0.4/setup.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-24 21:56:10.391900 redis-docker-harness-0.0.4/src/
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-24 21:56:10.395900 redis-docker-harness-0.0.4/src/rdh/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      185 2023-07-06 23:08:08.000000 redis-docker-harness-0.0.4/src/rdh/__init__.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     4277 2023-07-24 21:54:00.000000 redis-docker-harness-0.0.4/src/rdh/_argparse.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      203 2021-09-21 22:33:02.000000 redis-docker-harness-0.0.4/src/rdh/_log.py
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     2658 2023-07-24 20:51:08.000000 redis-docker-harness-0.0.4/src/rdh/_redis.py
+drwxrwxr-x   0 fracpete (62904) fracpete (62904)        0 2023-07-24 21:56:10.395900 redis-docker-harness-0.0.4/src/redis_docker_harness.egg-info/
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)     1631 2023-07-24 21:56:10.000000 redis-docker-harness-0.0.4/src/redis_docker_harness.egg-info/PKG-INFO
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)      372 2023-07-24 21:56:10.000000 redis-docker-harness-0.0.4/src/redis_docker_harness.egg-info/SOURCES.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        1 2023-07-24 21:56:10.000000 redis-docker-harness-0.0.4/src/redis_docker_harness.egg-info/dependency_links.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        6 2023-07-24 21:56:10.000000 redis-docker-harness-0.0.4/src/redis_docker_harness.egg-info/requires.txt
+-rw-rw-r--   0 fracpete (62904) fracpete (62904)        4 2023-07-24 21:56:10.000000 redis-docker-harness-0.0.4/src/redis_docker_harness.egg-info/top_level.txt
```

### Comparing `redis-docker-harness-0.0.3/setup.py` & `redis-docker-harness-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,11 +31,11 @@
     },
     packages=[
         "rdh",
     ],
     install_requires=[
         "redis",
     ],
-    version="0.0.3",
+    version="0.0.4",
     author='Peter Reutemann',
     author_email='fracpete@waikato.ac.nz',
 )
```

### Comparing `redis-docker-harness-0.0.3/src/rdh/_argparse.py` & `redis-docker-harness-0.0.4/src/rdh/_argparse.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 import argparse
 import os
 
 
-def create_parser(description, prog=None, prefix=""):
+def create_parser(description, prog=None, prefix="", host="localhost", port=6379, db=0,
+                  channel_in=None, channel_out=None, sleep_time=0.01):
     """
     Configures a command-line parser with parameters for redis.
 
     :param description: the description that the parser outputs on the help screen
     :type description: str
     :param prog: the program name, when using entry_points, None to ignore
     :type prog: str
     :param prefix: the prefix to use for the command-line arguments
     :type prefix: str
+    :param host: the default redis host
+    :type host: str
+    :param port: the default redis port
+    :type port: int
+    :param db: the default redis database
+    :type db: int
+    :param channel_in: the default incoming redis channel
+    :type channel_in: str
+    :param channel_out: the default outgoing redis channel
+    :type channel_out: str
+    :param sleep_time: the default pubsub timeout parameter
+    :type sleep_time: float
     :return: the configured parser
     :rtype: argparse.ArgumentParser
     """
     parser = argparse.ArgumentParser(description=description,
                                      prog=prog,
                                      formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('--%shost' % prefix, metavar='HOST', required=False, default="localhost",
+    parser.add_argument('--%shost' % prefix, metavar='HOST', required=(host is None), default=host, type=str,
                         dest='redis_host', help='The redis server to connect to')
-    parser.add_argument('--%sport' % prefix, metavar='PORT', required=False, default=6379, type=int,
+    parser.add_argument('--%sport' % prefix, metavar='PORT', required=(port is None), default=port, type=int,
                         dest='redis_port', help='The port the redis server is listening on')
     parser.add_argument('--%spassword' % prefix, metavar='PASSWORD', required=False, default=None, type=str,
                         dest='redis_password', help='The password to use for connecting')
     parser.add_argument('--%spassword_env' % prefix, metavar='PASSWORD', required=False, default=None, type=str,
                         dest='redis_password_env', help='The environment variable to obtain the password from to use for connecting')
-    parser.add_argument('--%sdb' % prefix, metavar='DB', required=False, default=0, type=int,
+    parser.add_argument('--%sdb' % prefix, metavar='DB', required=(db is None), default=db, type=int,
                         dest='redis_db', help='The redis database to use')
-    parser.add_argument('--%sin' % prefix, metavar='CHANNEL', required=True, type=str,
+    parser.add_argument('--%sin' % prefix, metavar='CHANNEL', required=(channel_in is None), default=channel_in, type=str,
                         dest='redis_in', help='The redis channel to receive the data from')
-    parser.add_argument('--%sout' % prefix, metavar='CHANNEL', required=True, type=str,
+    parser.add_argument('--%sout' % prefix, metavar='CHANNEL', required=(channel_out is None), default=channel_out, type=str,
                         dest='redis_out', help='The redis channel to publish the processed data on')
+    parser.add_argument('--%stimeout' % prefix, metavar='NUM', required=(sleep_time is None), default=sleep_time, type=float,
+                        dest='redis_timeout', help='The timeout to use for the pubsub thread sleep_time parameter.')
     return parser
 
 
 def has_password(ns):
     """
     Checks the namespace whether a password has been supplied either directly or via environment variable.
     Direct password takes precedence over environment variable.
```

### Comparing `redis-docker-harness-0.0.3/src/rdh/_redis.py` & `redis-docker-harness-0.0.4/src/rdh/_redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
         self.channel_in = None
         """ The channel to receive the data from. """
 
         self.channel_out = None
         """ The channel to send the processed data to. """
 
+        self.timeout = 0.001
+        """ The timeout to use for the pubsub thread sleep_time parameter. """
+
         self.stopped = False
         """ Flag whether processing has been stopped. """
 
 
 class MessageContainer(Container):
     """
     Simple container to store message alongside parameter for handler.
@@ -57,14 +60,15 @@
     :rtype: ParameterContainer
     """
     result = ParameterContainer()
     result.redis = redis.Redis(host=ns.redis_host, port=ns.redis_port, db=ns.redis_db, password=get_password(ns))
     result.pubsub = result.redis.pubsub()
     result.channel_in = ns.redis_in
     result.channel_out = ns.redis_out
+    result.timeout = ns.redis_timeout
     if config is not None:
         result.config = config
     return result
 
 
 def run_harness(params, process_method):
     """
@@ -82,8 +86,8 @@
         try:
             msg_cont.message = message
             process_method(msg_cont)
         except KeyboardInterrupt:
             msg_cont.params.stopped = True
 
     params.pubsub.psubscribe(**{params.channel_in: anon_handler})
-    params.pubsub.run_in_thread(sleep_time=0.001)
+    params.pubsub.run_in_thread(sleep_time=params.timeout)
```

