# Comparing `tmp/danielutils-0.9.0.tar.gz` & `tmp/danielutils-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.9.0.tar", last modified: Sat Jun  3 13:04:23 2023, max compression
+gzip compressed data, was "danielutils-0.9.5.tar", last modified: Mon Jul 24 23:01:36 2023, max compression
```

## Comparing `danielutils-0.9.0.tar` & `danielutils-0.9.5.tar`

### file list

```diff
@@ -1,108 +1,120 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.673278 danielutils-0.9.0/
--rw-rw-rw-   0        0        0     3313 2023-06-03 13:04:23.673278 danielutils-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2542 2023-06-03 13:04:22.000000 danielutils-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.607473 danielutils-0.9.0/danielutils/
--rw-rw-rw-   0        0        0     4551 2023-06-03 11:02:15.000000 danielutils-0.9.0/danielutils/Aliases.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.620674 danielutils-0.9.0/danielutils/Classes/
--rw-rw-rw-   0        0        0      210 2023-04-20 17:59:42.000000 danielutils-0.9.0/danielutils/Classes/Convenience.py
--rw-rw-rw-   0        0        0     1144 2023-06-01 23:36:28.000000 danielutils-0.9.0/danielutils/Classes/Counter.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.626266 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/
--rw-rw-rw-   0        0        0       94 2023-06-02 22:44:50.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/__init__.py
--rw-rw-rw-   0        0        0      507 2023-06-03 11:23:40.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/tbase.py
--rw-rw-rw-   0        0        0     2086 2023-06-03 11:18:53.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/tdict.py
--rw-rw-rw-   0        0        0     4201 2023-06-03 11:21:46.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/tlist.py
--rw-rw-rw-   0        0        0      876 2023-06-03 11:23:36.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/tset.py
--rw-rw-rw-   0        0        0      151 2023-06-03 11:23:41.000000 danielutils-0.9.0/danielutils/Classes/TypedBuiltins/ttuple.py
--rw-rw-rw-   0        0        0      126 2023-05-01 13:01:32.000000 danielutils-0.9.0/danielutils/Classes/__init__.py
--rw-rw-rw-   0        0        0     1047 2023-06-01 21:36:49.000000 danielutils-0.9.0/danielutils/Classes/frange.py
--rw-rw-rw-   0        0        0     5440 2023-06-02 20:00:18.000000 danielutils-0.9.0/danielutils/Colors.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.627529 danielutils-0.9.0/danielutils/Conversions/
--rw-rw-rw-   0        0        0     2227 2023-04-20 19:56:42.000000 danielutils-0.9.0/danielutils/Conversions/MainConversions.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.629539 danielutils-0.9.0/danielutils/Conversions/SpecializedConversions/
--rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.9.0/danielutils/Conversions/SpecializedConversions/__init__.py
--rw-rw-rw-   0        0        0      505 2023-06-03 11:19:44.000000 danielutils-0.9.0/danielutils/Conversions/SpecializedConversions/to_hex.py
--rw-rw-rw-   0        0        0      407 2023-04-20 17:57:46.000000 danielutils-0.9.0/danielutils/Conversions/SpecializedConversions/to_int.py
--rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.9.0/danielutils/Conversions/__init__.py
--rw-rw-rw-   0        0        0      631 2023-04-20 17:15:00.000000 danielutils-0.9.0/danielutils/Data.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.636064 danielutils-0.9.0/danielutils/DataStructures/
--rw-rw-rw-   0        0        0     1056 2023-06-02 08:41:44.000000 danielutils-0.9.0/danielutils/DataStructures/Comparer.py
--rw-rw-rw-   0        0        0     2282 2023-06-02 21:03:54.000000 danielutils-0.9.0/danielutils/DataStructures/Graph.py
--rw-rw-rw-   0        0        0     3372 2023-06-02 08:43:49.000000 danielutils-0.9.0/danielutils/DataStructures/Heap.py
--rw-rw-rw-   0        0        0     2620 2023-06-02 08:58:56.000000 danielutils-0.9.0/danielutils/DataStructures/Node.py
--rw-rw-rw-   0        0        0     5065 2023-06-02 08:59:09.000000 danielutils-0.9.0/danielutils/DataStructures/Queue.py
--rw-rw-rw-   0        0        0     1507 2023-06-01 23:41:53.000000 danielutils-0.9.0/danielutils/DataStructures/Stack.py
--rw-rw-rw-   0        0        0      133 2023-05-10 19:33:24.000000 danielutils-0.9.0/danielutils/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      616 2023-06-03 11:02:22.000000 danielutils-0.9.0/danielutils/DataStructures/functions.py
--rw-rw-rw-   0        0        0      135 2023-04-21 22:43:20.000000 danielutils-0.9.0/danielutils/DateTime.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.648553 danielutils-0.9.0/danielutils/Decorators/
--rw-rw-rw-   0        0        0      696 2023-04-29 17:38:05.000000 danielutils-0.9.0/danielutils/Decorators/PartiallyImplemented.py
--rw-rw-rw-   0        0        0      361 2023-06-01 10:32:05.000000 danielutils-0.9.0/danielutils/Decorators/__init__.py
--rw-rw-rw-   0        0        0      613 2023-06-01 23:35:30.000000 danielutils-0.9.0/danielutils/Decorators/atomic.py
--rw-rw-rw-   0        0        0     1213 2023-06-01 22:03:38.000000 danielutils-0.9.0/danielutils/Decorators/attach.py
--rw-rw-rw-   0        0        0      730 2023-04-29 17:58:20.000000 danielutils-0.9.0/danielutils/Decorators/chain_decorators.py
--rw-rw-rw-   0        0        0      853 2023-06-01 23:23:43.000000 danielutils-0.9.0/danielutils/Decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0      817 2023-04-29 18:02:16.000000 danielutils-0.9.0/danielutils/Decorators/delay_call.py
--rw-rw-rw-   0        0        0     1082 2023-06-02 20:21:38.000000 danielutils-0.9.0/danielutils/Decorators/deprecate.py
--rw-rw-rw-   0        0        0     1552 2023-06-02 20:36:42.000000 danielutils-0.9.0/danielutils/Decorators/limit_recursion.py
--rw-rw-rw-   0        0        0      622 2023-04-29 17:38:26.000000 danielutils-0.9.0/danielutils/Decorators/memo.py
--rw-rw-rw-   0        0        0     7232 2023-06-03 11:24:52.000000 danielutils-0.9.0/danielutils/Decorators/overload.py
--rw-rw-rw-   0        0        0      661 2023-05-21 20:38:07.000000 danielutils-0.9.0/danielutils/Decorators/property.py
--rw-rw-rw-   0        0        0      595 2023-04-29 17:59:44.000000 danielutils-0.9.0/danielutils/Decorators/threadify.py
--rw-rw-rw-   0        0        0     1730 2023-06-01 23:20:48.000000 danielutils-0.9.0/danielutils/Decorators/timeout.py
--rw-rw-rw-   0        0        0     9685 2023-06-03 11:06:39.000000 danielutils-0.9.0/danielutils/Decorators/validate.py
--rw-rw-rw-   0        0        0     2130 2023-04-30 19:46:55.000000 danielutils-0.9.0/danielutils/Exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.653613 danielutils-0.9.0/danielutils/Functions/
--rw-rw-rw-   0        0        0      135 2023-06-03 10:48:20.000000 danielutils-0.9.0/danielutils/Functions/__init__.py
--rw-rw-rw-   0        0        0      875 2023-06-03 10:58:55.000000 danielutils-0.9.0/danielutils/Functions/areoneof.py
--rw-rw-rw-   0        0        0      638 2023-06-03 10:45:50.000000 danielutils-0.9.0/danielutils/Functions/check_foreach.py
--rw-rw-rw-   0        0        0     5498 2023-06-03 10:48:37.000000 danielutils-0.9.0/danielutils/Functions/isoftype.py
--rw-rw-rw-   0        0        0     1372 2023-06-03 10:47:36.000000 danielutils-0.9.0/danielutils/Functions/isoneof.py
--rw-rw-rw-   0        0        0      582 2023-06-03 10:45:17.000000 danielutils-0.9.0/danielutils/Functions/types_subseteq.py
--rw-rw-rw-   0        0        0        0 2023-06-03 10:50:20.000000 danielutils-0.9.0/danielutils/Functions.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.656121 danielutils-0.9.0/danielutils/Generators/
--rw-rw-rw-   0        0        0       70 2023-06-01 11:44:02.000000 danielutils-0.9.0/danielutils/Generators/__init__.py
--rw-rw-rw-   0        0        0      450 2023-06-01 12:22:56.000000 danielutils-0.9.0/danielutils/Generators/generator_from_stream.py
--rw-rw-rw-   0        0        0     2638 2023-06-01 23:35:56.000000 danielutils-0.9.0/danielutils/Generators/join_generators.py
--rw-rw-rw-   0        0        0     9490 2023-06-02 20:25:10.000000 danielutils-0.9.0/danielutils/IO.py
--rw-rw-rw-   0        0        0     1852 2023-06-02 19:50:25.000000 danielutils-0.9.0/danielutils/Internet.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.660501 danielutils-0.9.0/danielutils/Math/
--rw-rw-rw-   0        0        0     7682 2023-04-20 20:14:55.000000 danielutils-0.9.0/danielutils/Math/Constants.py
--rw-rw-rw-   0        0        0      341 2023-06-01 22:46:15.000000 danielutils-0.9.0/danielutils/Math/Functions.py
--rw-rw-rw-   0        0        0     1061 2023-06-01 23:34:42.000000 danielutils-0.9.0/danielutils/Math/MathPrint.py
--rw-rw-rw-   0        0        0     3815 2023-06-01 22:45:35.000000 danielutils-0.9.0/danielutils/Math/MathSymbols.py
--rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.9.0/danielutils/Math/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.664675 danielutils-0.9.0/danielutils/MetaClasses/
--rw-rw-rw-   0        0        0      724 2023-06-01 23:27:38.000000 danielutils-0.9.0/danielutils/MetaClasses/AtomicClassMeta.py
--rw-rw-rw-   0        0        0     1950 2023-06-01 23:27:26.000000 danielutils-0.9.0/danielutils/MetaClasses/ImplicitDataDeleterMeta.py
--rw-rw-rw-   0        0        0     1499 2023-05-01 12:50:48.000000 danielutils-0.9.0/danielutils/MetaClasses/InstanceCacheMeta.py
--rw-rw-rw-   0        0        0    10521 2023-06-02 08:37:49.000000 danielutils-0.9.0/danielutils/MetaClasses/Interface.py
--rw-rw-rw-   0        0        0     1422 2023-06-03 11:22:02.000000 danielutils-0.9.0/danielutils/MetaClasses/OverloadMeta.py
--rw-rw-rw-   0        0        0       98 2023-04-30 22:02:36.000000 danielutils-0.9.0/danielutils/MetaClasses/__init__.py
--rw-rw-rw-   0        0        0     1032 2023-06-02 20:14:53.000000 danielutils-0.9.0/danielutils/Path.py
--rw-rw-rw-   0        0        0     2799 2023-06-03 11:03:50.000000 danielutils-0.9.0/danielutils/Print.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.670229 danielutils-0.9.0/danielutils/Reflection/
--rw-rw-rw-   0        0        0      945 2023-06-03 10:53:31.000000 danielutils-0.9.0/danielutils/Reflection/File.py
--rw-rw-rw-   0        0        0     4042 2023-06-03 11:13:30.000000 danielutils-0.9.0/danielutils/Reflection/Function.py
--rw-rw-rw-   0        0        0      507 2023-06-03 10:56:16.000000 danielutils-0.9.0/danielutils/Reflection/Module.py
--rw-rw-rw-   0        0        0      876 2023-06-03 10:55:25.000000 danielutils-0.9.0/danielutils/Reflection/System.py
--rw-rw-rw-   0        0        0     1476 2023-06-03 10:56:58.000000 danielutils-0.9.0/danielutils/Reflection/__init__.py
--rw-rw-rw-   0        0        0      352 2023-06-03 10:51:21.000000 danielutils-0.9.0/danielutils/Reflection/_get_prev_frame.py
--rw-rw-rw-   0        0        0      275 2023-06-03 10:42:46.000000 danielutils-0.9.0/danielutils/Reflection/get_traceback.py
--rw-rw-rw-   0        0        0      117 2023-06-02 22:45:41.000000 danielutils-0.9.0/danielutils/Relations.py
--rw-rw-rw-   0        0        0      489 2023-06-02 19:49:07.000000 danielutils-0.9.0/danielutils/Signals.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.672235 danielutils-0.9.0/danielutils/Snippets/
--rw-rw-rw-   0        0        0       24 2023-06-01 14:01:33.000000 danielutils-0.9.0/danielutils/Snippets/__init__.py
--rw-rw-rw-   0        0        0      433 2023-06-02 19:32:42.000000 danielutils-0.9.0/danielutils/Snippets/try_get.py
--rw-rw-rw-   0        0        0     6456 2023-06-02 20:14:24.000000 danielutils-0.9.0/danielutils/System.py
--rw-rw-rw-   0        0        0     4224 2023-06-03 11:04:13.000000 danielutils-0.9.0/danielutils/Text.py
--rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.9.0/danielutils/Time.py
--rw-rw-rw-   0        0        0     2254 2023-04-21 15:17:41.000000 danielutils-0.9.0/danielutils/Windows.py
--rw-rw-rw-   0        0        0      712 2023-06-03 10:43:48.000000 danielutils-0.9.0/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 13:04:23.617256 danielutils-0.9.0/danielutils.egg-info/
--rw-rw-rw-   0        0        0     3313 2023-06-03 13:04:23.000000 danielutils-0.9.0/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3107 2023-06-03 13:04:23.000000 danielutils-0.9.0/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 13:04:23.000000 danielutils-0.9.0/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-03 13:04:23.000000 danielutils-0.9.0/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      767 2023-06-03 13:04:22.000000 danielutils-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-03 13:04:23.673278 danielutils-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1343 2023-06-03 13:04:22.000000 danielutils-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.218385 danielutils-0.9.5/
+-rw-rw-rw-   0        0        0     3313 2023-07-24 23:01:36.218385 danielutils-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2542 2023-07-24 23:01:33.000000 danielutils-0.9.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.100335 danielutils-0.9.5/danielutils/
+-rw-rw-rw-   0        0        0     5663 2023-07-24 18:54:52.000000 danielutils-0.9.5/danielutils/Aliases.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.130054 danielutils-0.9.5/danielutils/Classes/
+-rw-rw-rw-   0        0        0      210 2023-04-20 17:59:42.000000 danielutils-0.9.5/danielutils/Classes/Convenience.py
+-rw-rw-rw-   0        0        0     1221 2023-07-24 18:47:17.000000 danielutils-0.9.5/danielutils/Classes/Counter.py
+-rw-rw-rw-   0        0        0     3047 2023-07-24 22:31:02.000000 danielutils-0.9.5/danielutils/Classes/Shell.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.132879 danielutils-0.9.5/danielutils/Classes/SortedBuiltins/
+-rw-rw-rw-   0        0        0        0 2023-06-16 22:05:18.000000 danielutils-0.9.5/danielutils/Classes/SortedBuiltins/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-07-24 21:01:48.000000 danielutils-0.9.5/danielutils/Classes/SortedBuiltins/sset.py
+-rw-rw-rw-   0        0        0        0 2023-06-16 22:06:37.000000 danielutils-0.9.5/danielutils/Classes/Tree.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.140422 danielutils-0.9.5/danielutils/Classes/TypedBuiltins/
+-rw-rw-rw-   0        0        0       88 2023-06-07 20:42:15.000000 danielutils-0.9.5/danielutils/Classes/TypedBuiltins/__init__.py
+-rw-rw-rw-   0        0        0     4730 2023-07-24 22:31:19.000000 danielutils-0.9.5/danielutils/Classes/TypedBuiltins/factory.py
+-rw-rw-rw-   0        0        0      913 2023-07-24 20:26:44.000000 danielutils-0.9.5/danielutils/Classes/TypedBuiltins/tdict.py
+-rw-rw-rw-   0        0        0     7214 2023-07-24 21:19:08.000000 danielutils-0.9.5/danielutils/Classes/TypedBuiltins/tlist.py
+-rw-rw-rw-   0        0        0     2031 2023-07-24 21:19:33.000000 danielutils-0.9.5/danielutils/Classes/TypedBuiltins/tset.py
+-rw-rw-rw-   0        0        0      294 2023-07-24 21:19:49.000000 danielutils-0.9.5/danielutils/Classes/TypedBuiltins/ttuple.py
+-rw-rw-rw-   0        0        0      158 2023-07-24 17:40:53.000000 danielutils-0.9.5/danielutils/Classes/__init__.py
+-rw-rw-rw-   0        0        0     1639 2023-07-24 21:16:57.000000 danielutils-0.9.5/danielutils/Classes/frange.py
+-rw-rw-rw-   0        0        0     5440 2023-07-24 21:45:50.000000 danielutils-0.9.5/danielutils/Colors.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.142923 danielutils-0.9.5/danielutils/Conversions/
+-rw-rw-rw-   0        0        0     2227 2023-04-20 19:56:42.000000 danielutils-0.9.5/danielutils/Conversions/MainConversions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.146044 danielutils-0.9.5/danielutils/Conversions/SpecializedConversions/
+-rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.9.5/danielutils/Conversions/SpecializedConversions/__init__.py
+-rw-rw-rw-   0        0        0      505 2023-06-03 11:19:44.000000 danielutils-0.9.5/danielutils/Conversions/SpecializedConversions/to_hex.py
+-rw-rw-rw-   0        0        0      548 2023-07-24 22:31:47.000000 danielutils-0.9.5/danielutils/Conversions/SpecializedConversions/to_int.py
+-rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.9.5/danielutils/Conversions/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-04-20 17:15:00.000000 danielutils-0.9.5/danielutils/Data.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.156575 danielutils-0.9.5/danielutils/DataStructures/
+-rw-rw-rw-   0        0        0     1081 2023-07-24 18:47:25.000000 danielutils-0.9.5/danielutils/DataStructures/Comparer.py
+-rw-rw-rw-   0        0        0     4872 2023-07-24 22:31:56.000000 danielutils-0.9.5/danielutils/DataStructures/Graph.py
+-rw-rw-rw-   0        0        0     3385 2023-07-24 21:05:08.000000 danielutils-0.9.5/danielutils/DataStructures/Heap.py
+-rw-rw-rw-   0        0        0     2968 2023-07-24 21:37:40.000000 danielutils-0.9.5/danielutils/DataStructures/Node.py
+-rw-rw-rw-   0        0        0     5129 2023-07-24 21:35:32.000000 danielutils-0.9.5/danielutils/DataStructures/Queue.py
+-rw-rw-rw-   0        0        0     1774 2023-07-24 21:07:43.000000 danielutils-0.9.5/danielutils/DataStructures/Stack.py
+-rw-rw-rw-   0        0        0      133 2023-05-10 19:33:24.000000 danielutils-0.9.5/danielutils/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-07-24 18:47:17.000000 danielutils-0.9.5/danielutils/DataStructures/functions.py
+-rw-rw-rw-   0        0        0      232 2023-07-24 20:19:56.000000 danielutils-0.9.5/danielutils/DateTime.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.174872 danielutils-0.9.5/danielutils/Decorators/
+-rw-rw-rw-   0        0        0     1012 2023-07-24 22:39:00.000000 danielutils-0.9.5/danielutils/Decorators/PartiallyImplemented.py
+-rw-rw-rw-   0        0        0      361 2023-06-01 10:32:05.000000 danielutils-0.9.5/danielutils/Decorators/__init__.py
+-rw-rw-rw-   0        0        0      912 2023-07-24 22:39:07.000000 danielutils-0.9.5/danielutils/Decorators/atomic.py
+-rw-rw-rw-   0        0        0     1555 2023-07-24 22:39:02.000000 danielutils-0.9.5/danielutils/Decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2023-07-04 09:01:54.000000 danielutils-0.9.5/danielutils/Decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0     1016 2023-07-24 21:08:20.000000 danielutils-0.9.5/danielutils/Decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0     1192 2023-07-24 22:39:02.000000 danielutils-0.9.5/danielutils/Decorators/delay_call.py
+-rw-rw-rw-   0        0        0     1469 2023-07-24 22:39:01.000000 danielutils-0.9.5/danielutils/Decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1877 2023-07-24 22:39:01.000000 danielutils-0.9.5/danielutils/Decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0      997 2023-07-24 22:39:01.000000 danielutils-0.9.5/danielutils/Decorators/memo.py
+-rw-rw-rw-   0        0        0     7511 2023-07-24 22:39:00.000000 danielutils-0.9.5/danielutils/Decorators/overload.py
+-rw-rw-rw-   0        0        0     1095 2023-07-24 21:22:41.000000 danielutils-0.9.5/danielutils/Decorators/property.py
+-rw-rw-rw-   0        0        0      916 2023-07-24 22:39:00.000000 danielutils-0.9.5/danielutils/Decorators/threadify.py
+-rw-rw-rw-   0        0        0     2088 2023-07-24 22:39:01.000000 danielutils-0.9.5/danielutils/Decorators/timeout.py
+-rw-rw-rw-   0        0        0    10013 2023-07-24 22:39:01.000000 danielutils-0.9.5/danielutils/Decorators/validate.py
+-rw-rw-rw-   0        0        0     2163 2023-07-24 21:56:15.000000 danielutils-0.9.5/danielutils/Exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.183812 danielutils-0.9.5/danielutils/Functions/
+-rw-rw-rw-   0        0        0      160 2023-06-17 21:44:01.000000 danielutils-0.9.5/danielutils/Functions/__init__.py
+-rw-rw-rw-   0        0        0     1097 2023-07-24 22:43:12.000000 danielutils-0.9.5/danielutils/Functions/areoneof.py
+-rw-rw-rw-   0        0        0      638 2023-06-03 10:45:50.000000 danielutils-0.9.5/danielutils/Functions/check_foreach.py
+-rw-rw-rw-   0        0        0     8978 2023-07-24 22:38:19.000000 danielutils-0.9.5/danielutils/Functions/isoftype.py
+-rw-rw-rw-   0        0        0     1598 2023-07-24 22:42:53.000000 danielutils-0.9.5/danielutils/Functions/isoneof.py
+-rw-rw-rw-   0        0        0      639 2023-07-24 21:13:39.000000 danielutils-0.9.5/danielutils/Functions/powerset.py
+-rw-rw-rw-   0        0        0     1016 2023-07-24 22:32:06.000000 danielutils-0.9.5/danielutils/Functions/types_subseteq.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.188174 danielutils-0.9.5/danielutils/Generators/
+-rw-rw-rw-   0        0        0      108 2023-06-17 21:54:52.000000 danielutils-0.9.5/danielutils/Generators/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-07-24 21:25:37.000000 danielutils-0.9.5/danielutils/Generators/conditional_generator.py
+-rw-rw-rw-   0        0        0      463 2023-07-24 18:50:47.000000 danielutils-0.9.5/danielutils/Generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2826 2023-07-24 22:32:15.000000 danielutils-0.9.5/danielutils/Generators/join_generators.py
+-rw-rw-rw-   0        0        0     9685 2023-07-24 22:30:43.000000 danielutils-0.9.5/danielutils/IO.py
+-rw-rw-rw-   0        0        0     2051 2023-07-24 22:30:25.000000 danielutils-0.9.5/danielutils/Internet.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.194725 danielutils-0.9.5/danielutils/Math/
+-rw-rw-rw-   0        0        0     7682 2023-04-20 20:14:55.000000 danielutils-0.9.5/danielutils/Math/Constants.py
+-rw-rw-rw-   0        0        0      627 2023-07-24 21:26:23.000000 danielutils-0.9.5/danielutils/Math/Functions.py
+-rw-rw-rw-   0        0        0     1061 2023-06-01 23:34:42.000000 danielutils-0.9.5/danielutils/Math/MathPrint.py
+-rw-rw-rw-   0        0        0     4051 2023-07-24 22:32:23.000000 danielutils-0.9.5/danielutils/Math/MathSymbols.py
+-rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.9.5/danielutils/Math/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.202841 danielutils-0.9.5/danielutils/MetaClasses/
+-rw-rw-rw-   0        0        0      695 2023-07-24 21:38:19.000000 danielutils-0.9.5/danielutils/MetaClasses/AtomicClassMeta.py
+-rw-rw-rw-   0        0        0     2511 2023-07-24 21:27:30.000000 danielutils-0.9.5/danielutils/MetaClasses/ImplicitDataDeleterMeta.py
+-rw-rw-rw-   0        0        0     1487 2023-07-24 21:14:44.000000 danielutils-0.9.5/danielutils/MetaClasses/InstanceCacheMeta.py
+-rw-rw-rw-   0        0        0    10944 2023-07-24 22:32:31.000000 danielutils-0.9.5/danielutils/MetaClasses/Interface.py
+-rw-rw-rw-   0        0        0     1754 2023-07-24 21:35:54.000000 danielutils-0.9.5/danielutils/MetaClasses/OverloadMeta.py
+-rw-rw-rw-   0        0        0      161 2023-06-07 20:50:39.000000 danielutils-0.9.5/danielutils/MetaClasses/__init__.py
+-rw-rw-rw-   0        0        0     1032 2023-06-02 20:14:53.000000 danielutils-0.9.5/danielutils/Path.py
+-rw-rw-rw-   0        0        0     2799 2023-06-03 11:03:50.000000 danielutils-0.9.5/danielutils/Print.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.211064 danielutils-0.9.5/danielutils/Reflection/
+-rw-rw-rw-   0        0        0      940 2023-07-24 20:48:54.000000 danielutils-0.9.5/danielutils/Reflection/File.py
+-rw-rw-rw-   0        0        0     4614 2023-07-24 22:38:46.000000 danielutils-0.9.5/danielutils/Reflection/Function.py
+-rw-rw-rw-   0        0        0      507 2023-06-03 10:56:16.000000 danielutils-0.9.5/danielutils/Reflection/Module.py
+-rw-rw-rw-   0        0        0     1229 2023-07-24 22:47:29.000000 danielutils-0.9.5/danielutils/Reflection/System.py
+-rw-rw-rw-   0        0        0     1520 2023-07-24 22:42:25.000000 danielutils-0.9.5/danielutils/Reflection/__init__.py
+-rw-rw-rw-   0        0        0      848 2023-07-24 20:51:00.000000 danielutils-0.9.5/danielutils/Reflection/get_prev_frame.py
+-rw-rw-rw-   0        0        0      444 2023-07-24 22:40:09.000000 danielutils-0.9.5/danielutils/Reflection/get_traceback.py
+-rw-rw-rw-   0        0        0      288 2023-07-24 20:58:33.000000 danielutils-0.9.5/danielutils/Relations.py
+-rw-rw-rw-   0        0        0      489 2023-06-02 19:49:07.000000 danielutils-0.9.5/danielutils/Signals.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.212569 danielutils-0.9.5/danielutils/Snippets/
+-rw-rw-rw-   0        0        0       24 2023-06-01 14:01:33.000000 danielutils-0.9.5/danielutils/Snippets/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-06-02 19:32:42.000000 danielutils-0.9.5/danielutils/Snippets/try_get.py
+-rw-rw-rw-   0        0        0     6840 2023-07-24 22:30:51.000000 danielutils-0.9.5/danielutils/System.py
+-rw-rw-rw-   0        0        0     4093 2023-07-24 18:54:01.000000 danielutils-0.9.5/danielutils/Text.py
+-rw-rw-rw-   0        0        0      531 2023-06-19 06:55:45.000000 danielutils-0.9.5/danielutils/Time.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.214980 danielutils-0.9.5/danielutils/University/
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.217135 danielutils-0.9.5/danielutils/University/Databases/
+-rw-rw-rw-   0        0        0       20 2023-07-24 21:15:17.000000 danielutils-0.9.5/danielutils/University/Databases/__init__.py
+-rw-rw-rw-   0        0        0    24911 2023-07-24 22:32:44.000000 danielutils-0.9.5/danielutils/University/Databases/all.py
+-rw-rw-rw-   0        0        0       26 2023-06-16 21:44:58.000000 danielutils-0.9.5/danielutils/University/__init__.py
+-rw-rw-rw-   0        0        0     2253 2023-07-24 20:59:14.000000 danielutils-0.9.5/danielutils/Windows.py
+-rw-rw-rw-   0        0        0      739 2023-06-18 20:27:36.000000 danielutils-0.9.5/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 23:01:36.123758 danielutils-0.9.5/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     3313 2023-07-24 23:01:35.000000 danielutils-0.9.5/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3466 2023-07-24 23:01:36.000000 danielutils-0.9.5/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 23:01:35.000000 danielutils-0.9.5/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-24 23:01:35.000000 danielutils-0.9.5/danielutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-24 23:01:35.000000 danielutils-0.9.5/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      767 2023-07-24 23:01:33.000000 danielutils-0.9.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 23:01:36.219468 danielutils-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1349 2023-07-24 23:01:33.000000 danielutils-0.9.5/setup.py
```

### Comparing `danielutils-0.9.0/PKG-INFO` & `danielutils-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.0
+Version: 0.9.5
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
 Keywords: functions,decorators,methods,classes,metaclasses
 Platform: All
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.10.5
+Requires-Python: >=3.8.17
 Description-Content-Type: text/markdown
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.0
+# danielutils v=0.9.5
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 # Showcase
 In [this](./READMES/) folder you can check out some more in depth showcase of some of the topics I have covered in this package
```

### Comparing `danielutils-0.9.0/README.md` & `danielutils-0.9.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.0
+# danielutils v=0.9.5
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 # Showcase
 In [this](./READMES/) folder you can check out some more in depth showcase of some of the topics I have covered in this package
```

### Comparing `danielutils-0.9.0/danielutils/Classes/Counter.py` & `danielutils-0.9.5/danielutils/Classes/Counter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,47 @@
+from typing import Union
 from ..MetaClasses import AtomicClassMeta
 
 
 class Counter:
     """A simple counter class
     """
 
-    def __init__(self, initial_value: int | float = 0, increment_amount: int | float = 1) -> None:
+    def __init__(self, initial_value: Union[int, float] = 0, increment_amount: Union[int, float] = 1) -> None:
         self.value = initial_value
         self.increment_value = increment_amount
 
     def increment(self) -> None:
         """increments the stored value by the increment amount
         """
         self.value += self.increment_value
 
     def decrement(self) -> None:
         """decrements the stored value by the increment amount
         """
         self.value -= self.increment_value
 
-    def get(self) -> int | float:
+    def get(self) -> Union[int, float]:
         """returns the current value of the counter
 
         Returns:
-            int | float: value
+            Union[int, float]: value
         """
         return self.value
 
-    def set(self, value: int | float):
+    def set(self, value: Union[int, float]):
         """sets the values of the counter
 
         Args:
-            value (int | float): value to set
+            value (Union[int, float]): value to set
         """
         self.value = value
 
 
-class AtomicCounter(Counter, metaclass=AtomicClassMeta):
+class AtomicCounter(Counter, metaclass=AtomicClassMeta):  # type:ignore
     """A Counter Class which is Atomic
     """
 
 
 __all__ = [
     "Counter",
     "AtomicCounter"
```

### Comparing `danielutils-0.9.0/danielutils/Colors.py` & `danielutils-0.9.5/danielutils/Colors.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.0/danielutils/Conversions/MainConversions.py` & `danielutils-0.9.5/danielutils/Conversions/MainConversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.0/danielutils/Data.py` & `danielutils-0.9.5/danielutils/Data.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.0/danielutils/DataStructures/Comparer.py` & `danielutils-0.9.5/danielutils/DataStructures/Comparer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Comparer class"""
-from typing import Callable, Any
+from typing import Callable, Any, Union
 from .functions import default_weight_function
 
 
 class Comparer():
     """a Comparer class to be used when comparing two objects
     """
 
-    def __init__(self, func: Callable[[Any, Any], int | float]):
+    def __init__(self, func: Callable[[Any, Any], Union[int, float]]):
         self.func = func
 
-    def compare(self, v1: Any, v2: Any) -> int | float:
+    def compare(self, v1: Any, v2: Any) -> Union[int, float]:
         """compares two objects
 
             Args:
                 v1 (Any): first object
                 v2 (Any): second object
 
             Returns:
                 int: a number specifying the order of the objects
             """
         return self.func(v1, v2)
 
-    def __call__(self, v1: Any, v2: Any) -> int | float:
+    def __call__(self, v1: Any, v2: Any) -> Union[int, float]:
         return self.compare(v1, v2)
 
 
 CompareGreater = Comparer(lambda a, b: default_weight_function(a) -
                           default_weight_function(b))
 CompareSmaller = Comparer(lambda a, b: default_weight_function(b) -
                           default_weight_function(a))
```

### Comparing `danielutils-0.9.0/danielutils/DataStructures/Graph.py` & `danielutils-0.9.5/danielutils/DataStructures/Node.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,106 @@
-from typing import Optional, Generator
-from .Queue import Queue
-from .Node import MultiNode
+from __future__ import annotations
+from typing import Any, Optional, Generator
+from ..MetaClasses import ImplicitDataDeleterMeta
 
 
-class Graph:
-    def __init__(self, nodes: Optional[list[MultiNode]] = None):
-        self.nodes: list[MultiNode] = nodes if nodes is not None else []
+class MultiNode:
+    """A node class with no limit to children amount
+    """
 
-    def add_node(self, node):
-        self.nodes.append(node)
+    def __init__(self, data: Any, children: Optional[list[Optional[MultiNode]]] = None):
+        self.data = data
+        self._children = children if children is not None else []
 
-    def _extended_dfs(self) -> Generator:
+    def __getitem__(self, index) -> Any:
+        return self._children[index]
+
+    def __setitem__(self, value, index) -> None:
+        self._children[index] = value
+
+    def __len__(self) -> int:
+        return len(self._children)
+
+    def __iter__(self) -> Generator:
+        yield from self._children
+
+    def __str__(self) -> str:
+        res = ""
         seen = set()
-        enter_times = dict()
-        exit_times = dict()
-        travel_index = 1
-        all_nodes = []
 
         def handle_node(node: MultiNode):
-            nonlocal travel_index
+            nonlocal res
+            # res += f"MultiNode({node.data}, ["
             seen.add(node)
-            all_nodes.append(node)
-            yield node
-            for subnode in node._children:
-                if subnode not in seen:
-                    travel_index += 1
-                    enter_times[subnode] = travel_index
-                    if subnode is not None:
-                        yield from handle_node(subnode)
-                    travel_index += 1
-                    exit_times[subnode] = travel_index
-
-        for node in self.nodes:
-            if node not in seen:
-                enter_times[node] = travel_index
-                travel_index += 1
-                yield from handle_node(node)
-                travel_index += 1
-                exit_times[node] = travel_index
-        topological_order = sorted(
-            all_nodes, key=lambda v: exit_times[v], reverse=True)
-        return topological_order
-
-    def dfs(self) -> Generator:
-        yield from self._extended_dfs()
-
-    def topological_sort(self) -> list:
-        g = self._extended_dfs()
-        try:
-            while True:
-                next(g)
-        except StopIteration as e:
-            return e.value
-
-    def bfs(self) -> Generator:
-        q = Queue()
-        for node in self.nodes:
-            q.push(node)
-        seen = set()
-        for node in q:
-            if node not in seen:
-                seen.add(node)
-                yield node
-                for child in node._children:
-                    q.push(child)
+            tmp = []
+            for child in node._children:  # pylint: disable=protected-access
+                if child in seen:
+                    tmp.append("...")
+                else:
+                    if child is not None:
+                        tmp.append(handle_node(child))
+            return f"{node.__class__.__name__}({node.data}, ["+", ".join(tmp)+"])"
+
+        return handle_node(self)
+
+    def __repr__(self):
+        return str(self)
+
+    def add_child(self, child):
+        """adds a child to current node
+        """
+        self._children.append(child)
+
+
+class Node(MultiNode, metaclass=ImplicitDataDeleterMeta):
+    """A 'classic' node class with only one child
+    """
+
+    def __init__(self, data, next: Optional[Node] = None):  # pylint: disable=redefined-builtin
+        super().__init__(data, [next])
+
+    @property
+    def next(self):
+        """return the next node after self
+        """
+        return self._children[0]
+
+    @next.setter
+    def next(self, value):
+        self._children[0] = value
+
+    def __str__(self):
+        # res = ""
+        # seen = set()
+
+        # def handle_node(node: Node):
+        #     nonlocal res
+        #     if node in seen:
+        #         res += "..."
+        #     else:
+        #         seen.add(node)
+        #         res += f"Node({node.data}, "
+        #         if node.next is None:
+        #             res += "None)"
+        #         elif node.next in seen:
+        #             res += "...)"
+
+        # curr = self
+        # while curr is not None:
+        #     handle_node(curr)
+        #     curr = curr.next
+        #     if curr in seen:
+        #         break
+        # return res+")"
+        return MultiNode.__str__(self).replace(
+            self.__class__.__mro__[1].__name__,
+            self.__class__.__name__
+        ).replace("[", "").replace("]", "")
 
-    def __str__(self) -> str:
-        tmp = []
-        for n in self.dfs():
-            tmp.append(f"\t{str(n)}")
-        return "Graph(\n"+",\n".join(tmp)+"\n)"
+    def __repr__(self):
+        return str(self)
 
 
 __all__ = [
-    "Graph"
+    "MultiNode",
+    "Node"
 ]
```

### Comparing `danielutils-0.9.0/danielutils/DataStructures/Heap.py` & `danielutils-0.9.5/danielutils/DataStructures/Heap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Union
 from .Comparer import Comparer, CompareGreater, CompareSmaller
 
 
 class Heap:
     """a Heap class which will do the sorting according to the supplied comparer object
     """
 
@@ -12,15 +12,15 @@
 
     def push(self, val: Any) -> None:
         """will add a new object to the heap
 
         Args:
             val (Any): the object to add to the heap
         """
-        res: int | float = -1
+        res: Union[int, float] = -1
         curr_index = len(self)
         self.arr.append(val)
         parent_index = curr_index//2 - (1 - curr_index % 2)
         while res < 0 and parent_index >= 0:
             res = self.comparer.compare(
                 self[parent_index], self[curr_index])
             if res < 0:
```

### Comparing `danielutils-0.9.0/danielutils/DataStructures/Queue.py` & `danielutils-0.9.5/danielutils/DataStructures/Queue.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Any
+from typing import Callable, Any, Union
 from .Heap import Heap
 from .Comparer import Comparer, CompareGreater
 from .functions import default_weight_function
 from ..MetaClasses import AtomicClassMeta
 
 
 class Queue:
@@ -21,15 +21,15 @@
 
     def push(self, value: Any) -> None:
         """adds a new element to the queue
 
         Args:
             value (Any): the value to add
         """
-        self.data.append(value)
+        self.data.insert(0, value)
 
     def peek(self) -> Any:
         """returns the oldest element in the queue 
         without removing it from the queue
 
         Returns:
             Any: result
@@ -44,19 +44,21 @@
 
         Returns:
             bool: result
         """
         return len(self) == 0
 
     def __str__(self) -> str:
+        return repr(self)
+
+    def __repr__(self) -> str:
         return str(self.data)
 
     def __iter__(self):
-        while not self.is_empty():
-            yield self.pop()
+        return iter(self.data)
 
     def push_many(self, arr: list):
         """will push many objects to the Queue
 
         Args:
             arr (list): the objects to push
         """
@@ -70,15 +72,15 @@
 
 
 class PriorityQueue(Queue):
     """
     A priority queue implementation based on a binary heap.
 
     Args:
-        weight_func (Callable[[T], int | float], optional): A function to calculate the weight of items added
+        weight_func (Callable[[T], Union[int, float]], optional): A function to calculate the weight of items added
             to the queue. Defaults to default_weight_function.
         comparer (Comparer, optional): The comparer to use when comparing weights of items in the queue.
             Defaults to Comparer.GREATER.
 
     Raises:
         ValueError: Raised if an item with the same weight value is added more than once.
 
@@ -98,19 +100,19 @@
         >>> pq.push(5)
         >>> pq.push(10)
         >>> pq.push(3)
         >>> pq.pop()
         10
     """
 
-    def __init__(self, weight_func: Callable[[Any], int | float] = default_weight_function):
+    def __init__(self, weight_func: Callable[[Any], Union[int, float]] = default_weight_function):
         super().__init__()
         comparer = CompareGreater if weight_func is default_weight_function else Comparer(
             lambda a, b: weight_func(a)-weight_func(b))
-        self.data: Heap = Heap(comparer)
+        self.data: Heap = Heap(comparer)  # type:ignore
         self.weight_func = weight_func
         self.dct: dict = {}
 
     def pop(self) -> Any:
         """
         Removes and returns the item with the highest priority (i.e., the lowest weight value) from the queue.
```

### Comparing `danielutils-0.9.0/danielutils/DataStructures/Stack.py` & `danielutils-0.9.5/danielutils/DataStructures/Stack.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,22 +7,32 @@
     """
 
     def __init__(self) -> None:
         self.head: Optional[Node] = None
         self.size = 0
 
     def push(self, value: Any):
+        """push an item to the stack
+
+        Args:
+            value (Any): item to push
+        """
         if self.head is None:
             self.head = Node(value)
         else:
             new_head = Node(value, self.head)
             self.head = new_head
         self.size += 1
 
     def pop(self) -> Any:
+        """pop an item from the stack
+
+        Returns:
+            Any: poped item
+        """
         if not self.is_empty():
             self.head = cast(Node, self.head)
             res = self.head.data
             self.size -= 1
             self.head = self.head.next
             return res
 
@@ -30,14 +40,16 @@
         return self.size
 
     def __iter__(self) -> Generator:
         while self:
             yield self.pop()
 
     def is_empty(self) -> bool:
+        """return whether the stack is empty
+        """
         return len(self) == 0
 
     def __bool__(self) -> bool:
         return not self.is_empty()
 
     def __contains__(self, value) -> bool:
         curr = self.head
```

### Comparing `danielutils-0.9.0/danielutils/Decorators/PartiallyImplemented.py` & `danielutils-0.9.5/danielutils/Decorators/PartiallyImplemented.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,25 @@
-from typing import Callable, Any
+from typing import Callable, Any, TypeVar
 import functools
+import platform
 from .validate import validate
 from ..Colors import warning
 
+from ..Reflection import get_python_version
+if get_python_version() < (3, 9):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+T = TypeVar("T")
+P = ParamSpec("P")
+FuncT = Callable[P, T]  # type:ignore
+
 
 @validate
-def PartiallyImplemented(func: Callable) -> Callable:
+def PartiallyImplemented(func: FuncT) -> FuncT:
     """decorator to mark function as not fully implemented for development purposes
 
     Args:
         func (Callable): the function to decorate
     """
 
     @ functools.wraps(func)
```

### Comparing `danielutils-0.9.0/danielutils/Decorators/chain_decorators.py` & `danielutils-0.9.5/danielutils/Decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.0/danielutils/Decorators/deprecate.py` & `danielutils-0.9.5/danielutils/Decorators/deprecate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,40 @@
-from typing import Callable
+import platform
+from typing import Callable, TypeVar
 from ..Colors import warning, ColoredText
 
+from ..Reflection import get_python_version
+if get_python_version() < (3, 9):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+T = TypeVar("T")
+P = ParamSpec("P")
+FuncT = Callable[P, T]  # type:ignore
 
-def deprecate_with(replacement_func) -> Callable[[Callable], Callable]:
+
+def deprecate_with(replacement_func) -> Callable[[FuncT], FuncT]:
     """will replace a deprecated function with the replacement func and will print a warning"""
-    def deco(func):
-        warning(f"{func.__module__}.{func.__qualname__} is deprecated, using {replacement_func.__module__}.{replacement_func.__qualname__} instead")
+    def deco(func: FuncT) -> FuncT:
+        warning(f"{func.__module__}.{func.__qualname__} is deprecated,"
+                f" using {replacement_func.__module__}.{replacement_func.__qualname__} instead")
 
         def wrapper(*args, **kwargs):
             return replacement_func(*args, **kwargs)
         return wrapper
     return deco
 
 
-def deprecate(deprecation_message: str):
+def deprecate(deprecation_message: str) -> Callable[[FuncT], FuncT]:
     """A decorator to print a deprecation message when using a deprecated function
 
     Args:
         deprecation_message (str): deprecation message
     """
-    def deco(func: Callable):
+    def deco(func: FuncT) -> FuncT:
         def wrapper(*args, **kwargs):
             print(ColoredText.orange("Deprecation Warning") +
                   ":", deprecation_message)
             return func(*args, **kwargs)
         return wrapper
     return deco
```

### Comparing `danielutils-0.9.0/danielutils/Decorators/limit_recursion.py` & `danielutils-0.9.5/danielutils/Decorators/limit_recursion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import functools
 import re
 import traceback
-from typing import Any, Callable
+import platform
+from typing import Any, Callable, TypeVar
 from .validate import validate
 from ..Colors import warning
 
+from ..Reflection import get_python_version
+if get_python_version() < (3, 9):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+T = TypeVar("T")
+P = ParamSpec("P")
+FuncT = Callable[P, T]  # type:ignore
+
 
 @validate
-def limit_recursion(max_depth: int, return_value: Any = None, quiet: bool = True) -> Callable:
+def limit_recursion(max_depth: int, return_value: Any = None, quiet: bool = True) -> Callable[[FuncT], FuncT]:
     """decorator to limit recursion of functions
 
     Args:
         max_depth (int): max recursion depth which is allowed for this function
         return_value (Any, optional): The value to return when the limit is reached. Defaults to None.
             if is None, will return the last a tuple for the last args, kwargs given
         quiet (bool, optional): whether to print a warning message. Defaults to True.
     """
 
-    def deco(func: Callable) -> Callable:
+    def deco(func: FuncT) -> FuncT:
         @ functools.wraps(func)
-        def wrapper(*args, **kwargs) -> Any:
+        def wrapper(*args, **kwargs):
             depth = functools.reduce(
                 lambda count, line:
                     count + 1 if re.search(rf"{func.__name__}\(.*\)$", line)
                     else count,
                 traceback.format_stack(), 0
             )
             if depth >= max_depth:
```

### Comparing `danielutils-0.9.0/danielutils/Decorators/overload.py` & `danielutils-0.9.5/danielutils/Decorators/overload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,29 @@
-from typing import Callable
+from typing import Callable, cast, Any, TypeVar, Dict as t_dict, List as t_list
 import inspect
+import platform
 import functools
-from ..Reflection.Function import is_function_annotated_properly
-from ..Functions.isoftype import isoftype
-from ..Functions.isoneof import isoneof, isoneof_strict
+from ..Reflection import is_function_annotated_properly
+from ..Functions import isoftype, isoneof, isoneof_strict
 from ..Exceptions import OverloadDuplication, OverloadNotFound
 from .deprecate import deprecate
-__overload_dict: dict[str, dict[tuple, Callable]] = {}
+from ..Reflection import get_python_version
+if get_python_version() < (3, 9):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec  # type:ignore# pylint: disable=ungrouped-imports
+    from builtins import dict as t_dict, list as t_list
+T = TypeVar("T")
+P = ParamSpec("P")
+FuncT = Callable[P, T]  # type:ignore
+T2 = TypeVar("T2")
+P2 = ParamSpec("P2")
+FuncT2 = Callable[P2, T2]  # type:ignore
+
+__overload_dict: t_dict[str, t_dict[tuple, Callable]] = {}
 
 
 @deprecate("'explicit_global_overload' is a legacy decorator please use 'overload' instead")
 def explicit_global_overload(*types) -> Callable:
     """decorator for overloading functions\n
     Usage\n-------\n
     @overload(str,str)\n
@@ -105,35 +118,36 @@
 class overload:
     """this class create an object to manage the overloads for a given function.\n
     will only match a specific resolution and won't infer best guess for types
     """
 
     __SKIP_SET = {"self", "cls", "args", "kwargs"}
 
-    def __init__(self, func: Callable):
+    def __init__(self, func: FuncT):
         overload._validate(func)
         self._qualname = func.__qualname__
         self._moudle = func.__module__
-        self._functions: dict[int, list[Callable]] = dict()
+        self._functions: t_dict[int, t_list[Callable]] = {}
         self._functions[overload._get_key(func)] = [func]
         functools.wraps(func)(self)
 
     @staticmethod
     def _get_key(func: Callable):
         return len(inspect.signature(func).parameters)
 
     @staticmethod
     def _validate(func: Callable):
         if not callable(func):
             raise ValueError("Can only overload functions")
         if not is_function_annotated_properly(func):
             raise ValueError(
-                f"{func.__module__}.{func.__qualname__} is not properly annotated.\nFunction must be fully annotated to be overloaded")
+                f"{func.__module__}.{func.__qualname__} is not properly annotated."
+                "\nFunction must be fully annotated to be overloaded")
 
-    def overload(self, func: Callable) -> "overload":
+    def overload(self, func: FuncT2) -> "overload":
         """will add another function to the list of available options
 
         Args:
             func (Callable): a new alternative function
 
         Returns:
             overload2: returns the overload object
@@ -142,23 +156,14 @@
         k = overload._get_key(func)
         if k not in self._functions:
             self._functions[k] = []
         self._functions[k].append(func)
         return self
 
     def __call__(self, *args, **kwargs):
-        """_summary_
-
-        Raises:
-            AttributeError: _description_
-            AttributeError: _description_
-
-        Returns:
-            _type_: _description_
-        """
         num_args = len(args)+len(kwargs.keys())
         if num_args not in self._functions:
             raise AttributeError(
                 f"No overload with {num_args} argument found for {self._moudle}.{self._qualname}")
         selected_func = None
         if len(self._functions[num_args]) == 1:
             selected_func = self._functions[num_args][0]
```

### Comparing `danielutils-0.9.0/danielutils/Decorators/timeout.py` & `danielutils-0.9.5/danielutils/Decorators/timeout.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 import threading
 import functools
-from typing import Callable
+import platform
+from typing import Callable, TypeVar, Union
 from .validate import validate
+from ..Reflection import get_python_version
+if get_python_version() < (3, 9):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+T = TypeVar("T")
+P = ParamSpec("P")
+FuncT = Callable[P, T]  # type:ignore
 
 
 @validate
-def timeout(duration: int | float, silent: bool = False) -> Callable:
+def timeout(duration: Union[int, float], silent: bool = False) -> Callable[[FuncT], FuncT]:
     """A decorator to limit runtime for a function
 
     Args:
-        duration (int | float): allowed runtime duration
-        silent (bool, optional): keyword only argument whether to pass the exception up the call stack. Defaults to False.
+        duration (Union[int, float]): allowed runtime duration
+        silent (bool, optional): keyword only argument whether
+        to pass the exception up the call stack. Defaults to False.
 
     Raises:
         ValueError: if a function is not provided to be decorated
         Exception: any exception from within the function
 
     Returns:
         Callable: the result decorated function
     """
     # https://stackoverflow.com/a/21861599/6416556
-    def timeout_deco(func: Callable) -> Callable:
+    def timeout_deco(func: FuncT) -> FuncT:
         if not callable(func):
             raise ValueError("timeout must decorate a function")
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             res: list = [
                 TimeoutError(f'{func.__module__}.{func.__qualname__} timed out after {duration} seconds!')]
```

### Comparing `danielutils-0.9.0/danielutils/Decorators/validate.py` & `danielutils-0.9.5/danielutils/Decorators/validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+import platform
 import functools
 import inspect
-from typing import Callable, get_type_hints, cast
+from typing import Callable, get_type_hints, cast, TypeVar, Union
 from ..Functions.isoftype import isoftype
-from ..Reflection.Function import get_function_return_type
+from ..Reflection import get_function_return_type
 from ..Exceptions import EmptyAnnotationException,\
     InvalidDefaultValueException, ValidationException, InvalidReturnValueException
+from ..Reflection import get_python_version
+if get_python_version() < (3, 9):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec  # type:ignore # pylint: disable=ungrouped-imports
+T = TypeVar("T")
+P = ParamSpec("P")
+FuncT = Callable[P, T]  # type:ignore
 
 
-def validate(strict: Callable | bool = True) -> Callable:
+def validate(strict: Union[FuncT, bool] = True) -> FuncT:
     """A decorator that validates the annotations and types of the arguments and return
     value of a function.
 
         * 'None' is allowed as default value for everything
         * Because of their wide known use, generally accepted keywords 'self', 'cls', 'args', 'kwargs'
         are not validated.
 
@@ -24,20 +33,19 @@
         InvalidDefaultValueException: If an argument's default value is not of the annotated type.
         ValidationException: If an argument's value is not of the expected type.
         InvalidReturnValueException: If the return value is not of the expected type.
 
     Returns:
         Callable: A wrapper function that performs the validation and calls the original function.
     """
-    if not isoftype(strict, bool | Callable):
+    if not isoftype(strict, Union[bool, Callable]):
         raise TypeError(
             "the argument for validate must be a Callable or a boolean to mark strict use")
 
-    def deco(func: Callable):
-
+    def deco(func: FuncT) -> FuncT:
         SKIP_SET = {"self", "cls", "args", "kwargs"}
         if not callable(func):
             raise TypeError(
                 "The validate decorator must only decorate a function")
         func_name = f"{func.__module__}.{func.__qualname__}"
         # get the signature of the function
         signature = inspect.signature(func)
```

### Comparing `danielutils-0.9.0/danielutils/Exceptions.py` & `danielutils-0.9.5/danielutils/Exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,11 +73,11 @@
     """
 
     def __enter__(self):
         return self
 
     def __exit__(self, cls, instance, traceback):
         if instance:
-            from .Colors import error
+            from .Colors import error  # pylint: disable=cyclic-import
             error(f"{cls} {instance}")
             return isinstance(instance, cls)
         return False
```

### Comparing `danielutils-0.9.0/danielutils/Functions/areoneof.py` & `danielutils-0.9.5/danielutils/Functions/areoneof.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from typing import Sequence, Any, Union
 from .isoneof import isoneof
+from ..Reflection import get_python_version
+if get_python_version() < (3, 9):
+    from typing import List as t_list, Tuple as t_tuple
+else:
+    from builtins import list as t_list, tuple as t_tuple  # type:ignore
 
 
-def areoneof(values: Sequence[Any], types: Union[list[type], tuple[type]]) -> bool:
+def areoneof(values: Sequence[Any], types: Union[t_list[type], t_tuple[type]]) -> bool:
     """performs 'isoneof(values[0],types) and ... and isoneof(values[...],types)'
 
     Args:
         values (Sequence[Any]): Sequence of values
         types (Sequence[Type]): Sequence of types
 
     Raises:
```

### Comparing `danielutils-0.9.0/danielutils/Functions/check_foreach.py` & `danielutils-0.9.5/danielutils/Functions/check_foreach.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.0/danielutils/Functions/isoneof.py` & `danielutils-0.9.5/danielutils/Functions/isoneof.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from typing import Any, Union, Sequence
 from .isoftype import isoftype
+from ..Reflection import get_python_version
+if get_python_version() < (3, 9):
+    from typing import List as t_list, Tuple as t_tuple
+else:
+    from builtins import list as t_list, tuple as t_tuple  # type:ignore
 
 
-def isoneof(v: Any, types: Union[list[type], tuple[type]]) -> bool:
+def isoneof(v: Any, types: Union[t_list[type], t_tuple[type]]) -> bool:
     """performs isoftype() or ... or isoftype()
 
     Args:
         v (Any): the value to check it's type
         types (Union[list[Type], tuple[Type]): A Sequence of approved types
 
     Raises:
@@ -19,15 +24,15 @@
         raise TypeError("'types' must be of type 'list' or 'tuple'")
     for T in types:
         if isoftype(v, T):
             return True
     return False
 
 
-def isoneof_strict(v: Any, types: Union[list[type], tuple[type]]) -> bool:
+def isoneof_strict(v: Any, types: Union[t_list[type], t_tuple[type]]) -> bool:
     """performs 'type(v) in types' efficiently
 
     Args:
         v (Any): value to check
         types (Sequence[Type]): sequence of approved types
 
     Raises:
```

### Comparing `danielutils-0.9.0/danielutils/Generators/join_generators.py` & `danielutils-0.9.5/danielutils/Generators/join_generators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from typing import Generator, Any
-from threading import Semaphore, Condition
+from typing import Generator, Any, Tuple as t_tuple
+from threading import Semaphore  # , Condition
 from ..Decorators import threadify
 from ..DataStructures import AtomicQueue, Queue
 from ..Classes import AtomicCounter
-from ..Print import aprint
+# from ..Print import aprint
+from ..Reflection import get_python_version
+if get_python_version() >= (3, 9):
+    from builtins import tuple as t_tuple  # type:ignore
 
 
-def join_generators_busy_waiting(*generators) -> Generator[tuple[int, Any], None, None]:
+def join_generators_busy_waiting(*generators) -> Generator[t_tuple[int, Any], None, None]:
     """joins an arbitrary amount of generators to yield objects as soon someone yield an object
 
     Yields:
         Generator[tuple[int, Any], None, None]: resulting generator
     """
     q = AtomicQueue()
     threads_status = [False for _ in range(len(generators))]
@@ -29,16 +32,17 @@
     while not all(threads_status):
         while not q.is_empty():
             yield q.pop()
     if not q.is_empty():
         yield from q
 
 
-def join_generators(*generators) -> Generator[tuple[int, Any], None, None]:
-    """will join generators to yield from all of them simultaneously without busy waiting, using semaphores and multithreading 
+def join_generators(*generators) -> Generator[t_tuple[int, Any], None, None]:
+    """will join generators to yield from all of them simultaneously 
+    without busy waiting, using semaphores and multithreading 
 
     Yields:
         Generator[Any, None, None]: one generator that combines all of the given ones
     """
     queue = Queue()
     edit_queue_semaphore = Semaphore(1)
     queue_status_semaphore = Semaphore(0)
@@ -49,15 +53,16 @@
         for value in generator:
             with edit_queue_semaphore:
                 queue.push((index, value))
             queue_status_semaphore.release()
         finished_threads_counter.increment()
 
         if finished_threads_counter.get() == len(generators):
-            # re-release the lock once from the last thread because it gets stuck in the main loop after the generation has stopped
+            # re-release the lock once from the last thread because it
+            # gets stuck in the main loop after the generation has stopped
             queue_status_semaphore.release()
 
     for i, generator in enumerate(generators):
         thread_entry_point(i, generator)
 
     while finished_threads_counter.get() < len(generators):
         queue_status_semaphore.acquire()
```

### Comparing `danielutils-0.9.0/danielutils/IO.py` & `danielutils-0.9.5/danielutils/IO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # -*- coding: utf-8 -*-
 import subprocess
-from typing import IO, Iterator, Generator, Optional, cast
+from typing import IO, Iterator, Generator, Optional, cast, Union, List as t_list
 import shutil
 from pathlib import Path
 import os
 from .Decorators import validate
+from .Reflection import get_python_version
+if get_python_version() >= (3, 9):
+    from builtins import list as t_list
 
 
 @validate
 def path_exists(path: str) -> bool:
     """checks whether a path exists
 
     Args:
@@ -54,15 +57,16 @@
         path (str): path of file
     """
     if file_exists(path):
         os.remove(path)
 
 
 @validate
-def read_file(path: str, read_bytes: bool = False) -> list[str] | list[bytes]:
+# type:ignore
+def read_file(path: str, read_bytes: bool = False) -> Union[t_list[str], t_list[bytes]]:
     """read all lines from a file
 
     Args:
         path (str): the path to the file
 
     Returns:
         list[str]: a list of all the lines in the file
@@ -98,43 +102,43 @@
     Args:
         path (str): path to check
     """
     return os.path.isdir(path)
 
 
 @validate
-def get_files(path: str) -> list[str]:
+def get_files(path: str) -> t_list[str]:
     """return a list of names of all files inside specified directory
 
     Args:
         path (str): directory
 
     Returns:
         list[str]: all files
     """
     files_and_directories = get_files_and_directories(path)
     return list(
         filter(lambda name: is_file(f"{path}\\{name}"), files_and_directories))
 
 
 @validate
-def get_files_and_directories(path: str) -> list[str]:
+def get_files_and_directories(path: str) -> t_list[str]:
     """get a list of all files and directories in specified path
 
     Args:
         path (str): path to check
 
     Returns:
         list[str]: all files and directories
     """
     return os.listdir(path)
 
 
 @validate
-def get_directories(path: str) -> list[str]:
+def get_directories(path: str) -> t_list[str]:
     """get all directories in specified path
 
     Args:
         path (str): path to check
 
     Returns:
         list[str]: all directories
@@ -315,15 +319,16 @@
             end (str, optional): the str to use as the final value. Defaults to "\n".
 
         Raises:
             ValueError: _description_
         """
         if self.output_stream is None:
             raise ValueError(
-                "Can't write to an empty stream. the stream must not be None: either by set_stream or by initialization")
+                "Can't write to an empty stream. the stream must not be None:"
+                " either by set_stream or by initialization")
         self.output_stream.write(
             str(self.indent_level*self.indent_value + sep.join(args)+end))
 
     def set_stream(self, stream: IO):
         """explicitly sets the stream
 
         Args:
```

### Comparing `danielutils-0.9.0/danielutils/Internet.py` & `danielutils-0.9.5/danielutils/Internet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import urllib.request
 import urllib.parse
 from urllib.parse import urlparse
 import urllib
+from typing import Tuple as t_tuple
 from .Decorators import validate
-
+from .Reflection import get_python_version
+if get_python_version() >= (3, 9):
+    from builtins import tuple as t_tuple  # type:ignore
 
 # def prettify_html(html: str) -> str:
 #     return html
 
 
 @validate
 def get_html(url: str) -> str:
@@ -18,28 +21,29 @@
 
     Returns:
         str: the html as a string
     """
     user_agent = 'Mozilla/5.0 (Windows; U; Windows NT 5.1; en-US; rv:1.9.0.7) Gecko/2009021910 Firefox/3.0.7'
     headers = {'User-Agent': user_agent, }
     req = urllib.request.Request(url, headers=headers)
-    html = urllib.request.urlopen(req).read().decode('UTF-8')
+    with urllib.request.urlopen(req) as f:
+        html = f.read().decode('UTF-8')
     # return bs4(html, 'html.parser').prettify()
     return html
 
 
 @validate
-def get_url_details(url: str) -> tuple[str, str, str, str, str, str]:
+def get_url_details(url: str) -> "t_tuple[str, str, str, str, str, str]":
     """returns details about a url
 
     Args:
         url (str): url
 
     Returns:
-        tuple[str, str, str, str, str]: scheme, nteloc, path, params, query, fragment
+        tuple[str, str, str, str, str]: scheme, netloc, path, params, query, fragment
     """
     scheme, netloc, path, params, query, fragment = urlparse(url)
     return scheme, netloc, path, params, query, fragment
 
 
 @validate
 def url_encode(s: str) -> str:
```

### Comparing `danielutils-0.9.0/danielutils/Math/Constants.py` & `danielutils-0.9.5/danielutils/Math/Constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.0/danielutils/Math/MathPrint.py` & `danielutils-0.9.5/danielutils/Math/MathPrint.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.0/danielutils/Math/MathSymbols.py` & `danielutils-0.9.5/danielutils/Math/MathSymbols.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 """file with math symbols constants"""
+from typing import Union, Dict as t_dict
+from ..Reflection import get_python_version
+if get_python_version() >= (3, 9):
+    from builtins import dict as t_dict
 # https://unicode-table.com/en/sets/mathematical-signs/
 SPECIAL_DOUBLE_N = "ℕ"
 SPECIAL_DOUBLE_Q = "ℚ"
 SPECIAL_DOUBLE_R = "ℝ"
 SPECIAL_DOUBLE_Z = "ℤ"
 SPECIAL_DOUBLE_C = "ℂ"
 SPECIAL_RPAB = "〉"  # right pointing angle bracket
@@ -17,16 +21,16 @@
 SPECIAL_EQUIV = "≡"
 SPECIAL_LAMBDA = "λ"
 SPECIAL_SQRT = "√"
 SPECIAL_CUBE_ROOT = "∛"
 SPECIAL_4TH_ROOT = "∜"
 
 
-SUPERSCRIPT_SMALL_LETTERS = ['ᵃ','ᵇ','ᶜ','ᵈ','ᵉ','ᶠ','ᵍ','ʰ','ⁱ','ʲ','ᵏ','ˡ','ᵐ','ⁿ',
-                             'ᵒ','ᵖ','𐞥','ʳ','ˢ','ᵗ','ᵘ','ᵛ','ʷ','ˣ','ʸ','ᶻ']
+SUPERSCRIPT_SMALL_LETTERS = ['ᵃ', 'ᵇ', 'ᶜ', 'ᵈ', 'ᵉ', 'ᶠ', 'ᵍ', 'ʰ', 'ⁱ', 'ʲ', 'ᵏ', 'ˡ', 'ᵐ', 'ⁿ',
+                             'ᵒ', 'ᵖ', '𐞥', 'ʳ', 'ˢ', 'ᵗ', 'ᵘ', 'ᵛ', 'ʷ', 'ˣ', 'ʸ', 'ᶻ']
 
 # superscript_big_case_a = 'ⁱ'
 # superscript_big_case_b = 'ⁱ'
 # superscript_big_case_c = 'ⁱ'
 # superscript_big_case_d = 'ⁱ'
 # superscript_big_case_e = 'ⁱ'
 # superscript_big_case_f = 'ⁱ'
@@ -48,15 +52,15 @@
 # superscript_big_case_v = 'ⁱ'
 # superscript_big_case_w = 'ⁱ'
 # superscript_big_case_x = 'ⁱ'
 # superscript_big_case_y = 'ⁱ'
 # superscript_big_case_z = 'ⁱ'
 
 
-superscript_dict :dict[str|int,str]= {}
+superscript_dict: t_dict[Union[str, int], str] = {}
 superscript_dict.update(
     {chr(i+ord('a')): SUPERSCRIPT_SMALL_LETTERS[i] for i in range(26)}
 )
 superscript_digits = ["⁰", "¹", "²", "³",
                       "⁴", "⁵", "⁶", "⁷", "⁸", "⁹"]
 superscript_dict.update(
     {i: superscript_digits[i] for i in range(len(superscript_digits))}
@@ -65,16 +69,16 @@
     "+": "⁺",
     "-": "⁻",
     "=": "⁼",
     "(": "⁽",
     ")": "⁾",
 })
 
-SUBSCRIPT_SMALL_LETTERS = ['ₐ','','','','ₑ','','','ₕ','ᵢ','ⱼ','ₖ','ₗ','ₘ',
-                           'ₙ','ₒ','ₚ','','ᵣ','ₛ','ₜ','ᵤ','ᵥ','','ₓ','','']
+SUBSCRIPT_SMALL_LETTERS = ['ₐ', '', '', '', 'ₑ', '', '', 'ₕ', 'ᵢ', 'ⱼ', 'ₖ', 'ₗ', 'ₘ',
+                           'ₙ', 'ₒ', 'ₚ', '', 'ᵣ', 'ₛ', 'ₜ', 'ᵤ', 'ᵥ', '', 'ₓ', '', '']
 # subscript_big_case_a = 'ⁱ'
 # subscript_big_case_b = 'ⁱ'
 # subscript_big_case_c = 'ⁱ'
 # subscript_big_case_d = 'ⁱ'
 # subscript_big_case_e = 'ⁱ'
 # subscript_big_case_f = 'ⁱ'
 # subscript_big_case_g = 'ⁱ'
@@ -93,15 +97,15 @@
 # subscript_big_case_t = 'ⁱ'
 # subscript_big_case_u = 'ⁱ'
 # subscript_big_case_v = 'ⁱ'
 # subscript_big_case_w = 'ⁱ'
 # subscript_big_case_x = 'ⁱ'
 # subscript_big_case_y = 'ⁱ'
 # subscript_big_case_z = 'ⁱ'
-subscript_dict:dict[str|int,str] = {}
+subscript_dict: t_dict[Union[str, int], str] = {}
 subscript_dict.update(
     {chr(i+ord('a')): SUBSCRIPT_SMALL_LETTERS[i]
      for i in range(len(SUBSCRIPT_SMALL_LETTERS))}
 )
 
 subscript_digits = ["\u2080", "\u2081", "\u2082", "\u2083",
                     "\u2084", "\u2085", "\u2086", "\u2087", "\u2088", "\u2089"]
```

### Comparing `danielutils-0.9.0/danielutils/MetaClasses/AtomicClassMeta.py` & `danielutils-0.9.5/danielutils/MetaClasses/AtomicClassMeta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Callable
 from ..Decorators import atomic
 
 
 class AtomicClassMeta(type):
     """will make all of the class's function atomic
     """
     def __new__(mcs, name, bases, namespace):
```

### Comparing `danielutils-0.9.0/danielutils/MetaClasses/ImplicitDataDeleterMeta.py` & `danielutils-0.9.5/danielutils/MetaClasses/ImplicitDataDeleterMeta.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 from typing import Optional
 
 
 class DeletedException(AttributeError):
-    pass
+    """an exception to be raised if a function is deleted
+    """
 
 
 def deleted(func, cls_name: Optional[str] = None):
+    """replaces a function with a pre-scripted deleted function
+
+    Args:
+        func (_type_): _description_
+        cls_name (Optional[str], optional): _description_. Defaults to None.
+
+    Raises:
+        DeletedException: _description_
+
+    Returns:
+        _type_: _description_
+    """
     msg = f"'{func.__qualname__}' has been marked as deleted"
     if cls_name:
         msg = f"'{cls_name}.{func.__name__}' has been marked as deleted"
 
-    def new_func(*args, **kwargs):
+    def new_func(*args, **kwargs):  # pylint: disable=unused-argument
         nonlocal func
         raise DeletedException(msg)
     return new_func
 
 
 class ImplicitDataDeleterMeta(type):
+    """Inheriting from this metaclass will 'delete' all non builtin function 
+    and will replace them with a new function which will raise and error
+    """
     def __new__(mcs, name, bases, namespace):
         cls_functions = set()
         for k, v in namespace.items():
             if callable(v):
                 if hasattr(v, "__objclass__"):
                     if v.__objclass__ in {object}:
                         continue
```

### Comparing `danielutils-0.9.0/danielutils/MetaClasses/InstanceCacheMeta.py` & `danielutils-0.9.5/danielutils/MetaClasses/InstanceCacheMeta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..Classes import Counter
+from ..Classes.Counter import Counter
 
 
 class InstanceCacheMeta(type):
     """Adds automatic caching of all instances of the class
 
         Adds the following API to the class
         @staticmethod
@@ -13,39 +13,36 @@
 
         @staticmethod
         get_instance(id) -> return the id of an instance
 
     """
     def __new__(mcs, name, bases, namespace):
         INIT = "__init__"
-        instance_2_id = dict()
-        id_2_instance = dict()
+        instance_2_id: dict = {}
+        id_2_instance: dict = {}
         counter = Counter()
         original_init = None
         if INIT in namespace:
             original_init = namespace[INIT]
 
         def new_init(*args, **kwargs):
             id_2_instance[counter.get()] = args[0]
             instance_2_id[args[0]] = counter.get()
             counter.increment()
             if original_init:
                 original_init(*args, **kwargs)
 
-        @staticmethod
         def get_id(instance):
-            yield from instance_2_id[instance]
+            return instance_2_id[instance]
 
-        @staticmethod
-        def get_instance(id):
-            return id_2_instance[id]
+        def get_instance(id_: int):
+            return id_2_instance[id_]
 
-        @staticmethod
         def instances():
             return instance_2_id.keys()
 
-        namespace["instances"] = instances
-        namespace["get_id"] = get_id
-        namespace["get_instance"] = get_instance
+        namespace["instances"] = staticmethod(instances)
+        namespace["get_id"] = staticmethod(get_id)
+        namespace["get_instance"] = staticmethod(get_instance)
         namespace[INIT] = new_init
 
         return super().__new__(mcs, name, bases, namespace)
```

### Comparing `danielutils-0.9.0/danielutils/MetaClasses/Interface.py` & `danielutils-0.9.5/danielutils/MetaClasses/Interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from typing import Callable, Iterable, Any, Generator, Optional, cast
 import inspect
 import re
 import traceback
 import functools
+from typing import Callable, Iterable, Any, Generator, Optional, Union,\
+    List as t_list, Set as t_set, Type as t_type, Dict as t_dict
+from ..Reflection import get_python_version
+if get_python_version() >= (3, 9):
+    from builtins import list as t_list, set as t_set, type as t_type, dict as t_dict  # type:ignore
 # from ..Decorators.decorate_conditionally import decorate_conditionally
 
 
 class InterfaceHelper:
     """a helper class for Interface metaclass
     """
     ORIGINAL_INIT = "__original_init__"
@@ -79,24 +83,28 @@
     @staticmethod
     def get_declared_function_names(cls) -> Generator[str, None, None]:
         """will yield the names of all the functions declared inside a class
 
         Yields:
             Generator[str, None, None]: yields str values which are names of declared functions
         """
+        # In python 3.8 this function always return the first occurrence so some tests fail
         src = inspect.getsource(cls).splitlines()
+        print(src)
         for line in src:
             if re.match(r".*def \w+\(.*\).*:", line):
                 func_name = re.findall(r".*def (\w+)\(.*", line)[0]
                 yield func_name
 
     @staticmethod
-    def create_init_handler(cls_name, missing: Optional[list[str] | set[str]] = None, original: Optional[Callable] = None):
+    def create_init_handler(cls_name, missing: Optional[Union[t_list[str],
+                            t_set[str]]] = None, original: Optional[Callable] = None):
         """this function will create the default interface __init__ function with the wanted behavior"""
-        # @decorate_conditionally(functools.wraps, original is not None, [original])  # TODO implement this decorator
+        # @decorate_conditionally(functools.wraps, original
+        # is not None, [original])  # TODO implement this decorator
         def __interface_init__(*args, **kwargs):
             instance = args[0]
             caller_frame = traceback.format_stack()[-2]
             is_super_call = bool(re.match(
                 fr"\s+File \".*\", line \d+, in __init__\n\s+(?:super\(\)|{cls_name})\.__init__\(.*\)\n", caller_frame))
             if is_super_call:
                 mro = instance.__class__.mro()
@@ -145,35 +153,35 @@
 
     @staticmethod
     def abstractmethod(func):
         """will explicitly mark a method as an abstract method"""
         setattr(func, Interface.FUNC_KEY, True)
         return func
 
-    def __new__(mcs: type['Interface'], name: str, bases: tuple, namespace: dict):
+    def __new__(mcs: t_type['Interface'], name: str, bases: tuple, namespace: dict):
         if len(bases) == 0:
             return mcs._handle_new_interface(mcs, name, bases, namespace)
         return mcs._handle_new_subclass(mcs, name, bases, namespace)
 
     @staticmethod
-    def _handle_new_interface(mcs, name: str, bases: tuple, namespace: dict[str, Any]) -> type:
+    def _handle_new_interface(mcs, name: str, bases: tuple, namespace: t_dict[str, Any]) -> type:
         namespace[InterfaceHelper.ORIGINAL_INIT] = None
         if "__init__" in namespace:
             namespace[InterfaceHelper.ORIGINAL_INIT] = namespace["__init__"]
         namespace["__init__"] = InterfaceHelper.create_init_handler(
             name, original=namespace[InterfaceHelper.ORIGINAL_INIT])
         for k, v in namespace.items():
             if callable(v) and not k == "__init__":
                 if not InterfaceHelper.is_func_implemented(v):
                     namespace[k] = InterfaceHelper.create_generic_handler(k, v)
         namespace[Interface.KEY] = True
         return type.__new__(mcs, name, bases, namespace)
 
     @staticmethod
-    def _handle_new_subclass(mcs: type['Interface'], name: str, bases: tuple, namespace: dict[str, Any]) -> type:
+    def _handle_new_subclass(mcs: t_type['Interface'], name: str, bases: tuple, namespace: t_dict[str, Any]) -> type:
         need_to_be_implemented: set = set()
         ancestry = set()
         for base in bases:
             cls_tree = inspect.getclasstree([base], unique=True)
             ancestry.update(InterfaceHelper.flatten_iterables(cls_tree))
             for item in cls_tree:
                 if isinstance(item, tuple):
```

### Comparing `danielutils-0.9.0/danielutils/MetaClasses/OverloadMeta.py` & `danielutils-0.9.5/danielutils/MetaClasses/OverloadMeta.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,25 @@
+import functools
 from typing import Callable
 from ..Decorators import overload
 
 
 class OverloadMeta(type):
+    """A meta-class for overloading functions in a class
+    """
     @staticmethod
     def overload(func: Callable) -> overload:
+        """overloads a function
+
+        Args:
+            func (Callable): function ot overload
+
+        Returns:
+            overload: _description_
+        """
         return overload(func)
 
     def __new__(mcs, name, bases, namespace):
         # og_getattribute = None
         # if "__getattribute__" in namespace:
         #     og_getattribute = namespace["__getattribute__"]
 
@@ -24,18 +35,23 @@
         #     @functools.wraps(function_obj)
         #     def wrapper(*args, **kwargs):
         #         return function_obj(self, *args, **kwargs)
 
         #     return wrapper
 
         def create_wrapper(v: overload):
-            @functools.wraps(next(iter(v._functions.values()))[0])
+            @functools.wraps(next(iter(v._functions.values()))[0])  # pylint: disable=protected-access
             def wrapper(*args, **kwargs):
                 return v(*args, **kwargs)
             return wrapper
 
         for k, v in namespace.items():
             if isinstance(v, overload):
                 namespace[k] = create_wrapper(v)
         # namespace["__getattribute__"] = __getattribute__
 
         return super().__new__(mcs, name, bases, namespace)
+
+
+__all__ = [
+    "OverloadMeta"
+]
```

### Comparing `danielutils-0.9.0/danielutils/Path.py` & `danielutils-0.9.5/danielutils/Path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.0/danielutils/Print.py` & `danielutils-0.9.5/danielutils/Print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.9.0/danielutils/Reflection/File.py` & `danielutils-0.9.5/danielutils/Reflection/File.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import inspect
 from typing import Optional, cast
 from types import FrameType
-from ._get_prev_frame import _get_prev_frame
+from .get_prev_frame import get_prev_frame
 
 
 def get_filename() -> Optional[str]:
     """returns the name of the file that this functions is called from
 
     Returns:
         Optional[str]: name of file
     """
-    frame = _get_prev_frame(inspect.currentframe())
+    frame = get_prev_frame(inspect.currentframe())
     if frame is None:
         return None
     frame = cast(FrameType, frame)
     return frame.f_code.co_filename
 
 
 def get_caller_filename() -> Optional[str]:
     """return the name of the file that the caller of the 
     function that's using this function is in
 
     Returns:
         Optional[str]: name of file
     """
-    frame = _get_prev_frame(_get_prev_frame(inspect.currentframe()))
+    frame = get_prev_frame(get_prev_frame(inspect.currentframe()))
     if frame is None:
         return None
     frame = cast(FrameType, frame)
     return frame.f_code.co_filename
 
 
 __all__ = [
```

### Comparing `danielutils-0.9.0/danielutils/Reflection/Function.py` & `danielutils-0.9.5/danielutils/Reflection/Function.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import inspect
-from typing import cast, Optional, Callable
+from typing import cast, Optional, Callable, Any
 from types import FrameType
-from ._get_prev_frame import _get_prev_frame
-from ..Functions.isoftype import isoftype
+from .get_prev_frame import get_prev_frame
+
+from ..Reflection import get_python_version
+if get_python_version() < (3, 9):
+    from typing import List as t_list, Set as t_set  # pylint: disable=ungrouped-imports
+else:
+    from builtins import list as t_list, set as t_set
 
 
 def get_caller_name(steps_back: int = 0) -> Optional[str]:
     """returns the name caller of the function
 
     Returns:
         str: name of caller
 
     USING THIS FUNCTION WHILE DEBUGGING WILL ADD ADDITIONAL FRAMES TO THE TRACEBACK
     """
     if not isinstance(steps_back, int):
         raise TypeError("steps_back must be an int")
-    if not (steps_back >= 0):
+    if steps_back < 0:
         raise ValueError("steps_back must be a non-negative integer")
     # different implementation:
 
     # RGX = r'File ".*", line \d+, in (.+)\n'
     # # traceback_list = get_traceback()
     # # callee_frame = traceback_list[-1]
     # # callee_name = re.search(RGX, callee_frame).group(1)
@@ -30,20 +35,20 @@
 
     # current_frame = inspect.currentframe()
     # callee_frame = current_frame.f_back
     # # callee_name = callee_frame.f_code.co_name
     # caller_frame = callee_frame.f_back
     # caller_name = caller_frame.f_code.co_name
     # return caller_name
-    frame = _get_prev_frame(_get_prev_frame(inspect.currentframe()))
+    frame = get_prev_frame(get_prev_frame(inspect.currentframe()))
     if frame is None:
         return None
     frame = cast(FrameType, frame)
     while steps_back > 0:
-        frame = _get_prev_frame(frame)
+        frame = get_prev_frame(frame)
         if frame is None:
             return None
         frame = cast(FrameType, frame)
         steps_back -= 1
     return frame.f_code.co_name
 
 
@@ -60,33 +65,34 @@
         signature = inspect.signature(func)
     if ("inspect._empty" in str(signature.return_annotation)) or (signature.return_annotation is None):
         return type(None)
     return signature.return_annotation
 
 
 def is_function_annotated_properly(func: Callable, ignore: Optional[set] = None, check_return: bool = True) -> bool:
-    """checks wheter a function is annotated properly
+    """checks whether a function is annotated properly
 
     Args:
         func (Callable): the function to check
-        ignore (set, optional): arguments to ignore when validating. when 'None' Defaults to {"self", "cls", "args", "kwargs"}.
+        ignore (set, optional): arguments to ignore when validating.
+        when 'None' Defaults to {"self", "cls", "args", "kwargs"}.
         check_return (bool, optional): whether to also check that the return value is annotated. Defaults to True
     Raises:
         ValueError: if any of the parameters is of the wrong type
 
     Returns:
         bool: result of validation
     """
-
+    from ..Functions.isoftype import isoftype
     if not inspect.isfunction(func):
         raise ValueError("param should be a function")
 
     if ignore is None:
         ignore = {"self", "cls", "args", "kwargs"}
-    if not isoftype(ignore, set[str]):
+    if not isoftype(ignore, t_set[str]):
         raise ValueError("ignore must be a set of str")
 
     # get the signature of the function
     signature = inspect.signature(func)
     for arg_name, arg_param in signature.parameters.items():
         if arg_name not in ignore:
             arg_type = arg_param.annotation
@@ -104,12 +110,27 @@
                 return False
 
     if check_return:
         pass
     return True
 
 
+def get_mro(obj: Any) -> t_list[type]:
+    """returns the mro of an object
+
+    Args:
+        obj (Any): any object, instance or class
+
+    Returns:
+        list[type]: the resulting mro for the object
+    """
+    if isinstance(obj, type):
+        return obj.mro()
+    return get_mro(obj.__class__)
+
+
 __all__ = [
     "get_caller_name",
     "get_function_return_type",
-    "is_function_annotated_properly"
+    "is_function_annotated_properly",
+    "get_mro"
 ]
```

### Comparing `danielutils-0.9.0/danielutils/Reflection/System.py` & `danielutils-0.9.5/danielutils/Reflection/System.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,30 +15,41 @@
 def get_os() -> OSType:
     """returns the type of operation system running this code
 
     Returns:
         OSType: enum result
     """
     p = sys.platform
-    if p == "linux" or p == "linux2":
+    if p in {"linux", "linux2"}:
         return OSType.LINUX
-    elif p == "darwin":
+    if p == "darwin":
         return OSType.OSX
-    elif p == "win32":
+    if p == "win32":
         return OSType.WINDOWS
     return OSType.UNKNOWN
 
 
-def get_python_version() -> str:
-    """returns the python version of the interpreter running this code
+def _get_python_version_untyped() -> tuple:
+    values = (int(v) for v in platform.python_version().split("."))
+    return tuple(values)  # type:ignore
+
+
+if _get_python_version_untyped() < (3, 9):
+    from typing import Tuple as t_tuple
+else:
+    from builtins import tuple as t_tuple  # type:ignore
+
+
+def get_python_version() -> t_tuple[int, int, int]:
+    """return the version of python that is currently running this code
 
     Returns:
-        str: version string
+        tuple[int, int, int]: version
     """
-    return platform.python_version()
+    return _get_python_version_untyped()  # type:ignore
 
 
 __all__ = [
     "OSType",
     "get_os",
     "get_python_version"
 ]
```

### Comparing `danielutils-0.9.0/danielutils/Reflection/__init__.py` & `danielutils-0.9.5/danielutils/Reflection/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from .System import *  # this has to be first, the order matters!
 from .File import *
 from .Function import *
 from .get_traceback import *
 from .Module import *
-from .System import *
 
 
 # def get_class(module_name: str, class_name: str) -> type:
 #     """dynammically loads the module and returns the class from this file
 
 #     Args:
 #         module_name (str): name of python module, (typically a file name without extention)
```

### Comparing `danielutils-0.9.0/danielutils/System.py` & `danielutils-0.9.5/danielutils/System.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Generator
-from typing import IO, Optional, cast
+from typing import IO, Optional, cast, Union, Generator, Tuple as t_tuple, List as t_list
 from pathlib import Path
 import subprocess
 import time
 from .Decorators import timeout, validate
 from .Conversions import str_to_bytes
 from .Generators import join_generators, generator_from_stream
+from .Reflection import get_python_version
+if get_python_version() >= (3, 9):
+    from builtins import tuple as t_tuple, list as t_list  # type:ignore
 
 
-def cm(*args, shell: bool = True) -> tuple[int, bytes, bytes]:
+def cm(*args, shell: bool = True) -> t_tuple[int, bytes, bytes]:
     """Execute windows shell command and return output
 
     Args:
         command or args:\n
         command (str): A string representation of the command to execute.
         args (list[str]): A list of all the command parts
         shell (bool, optional): whether to execute in shell. Defaults to True.
@@ -32,15 +34,15 @@
             args = (*args[:i], f"\"{arg}\"", *args[i+1:])
     res = subprocess.run(" ".join(args), shell=shell,
                          capture_output=True, check=False)
     return res.returncode, res.stdout, res.stderr
 
 
 @validate
-def sleep(seconds: int | float) -> None:
+def sleep(seconds: Union[int, float]) -> None:
     """make current thread sleep
 
     Args:
         seconds (float): number of seconds to sleep
 
     Returns:
         None
@@ -53,16 +55,17 @@
     b_args = str_to_bytes(sep).join(str_to_bytes(v) for v in args)
     b_end = str_to_bytes(end)
     p.stdin.write(b_args+b_end)
     p.stdin.flush()
 
 
 @validate
-def acm(command: str, inputs: Optional[list[str]] = None, i_timeout: float = 0.01,
-        shell: bool = False, use_write_helper: bool = True, cwd: Optional[str] = None) -> tuple[int, Optional[list[bytes]], Optional[list[bytes]]]:
+def acm(command: str, inputs: Optional[t_list[str]] = None, i_timeout: float = 0.01,
+        shell: bool = False, use_write_helper: bool = True, cwd: Optional[str] = None) \
+        -> t_tuple[int, Optional[t_list[bytes]], Optional[t_list[bytes]]]:
     """Advanced command
 
     Args:
         command (str): The command to execute\n
         inputs (list[str]): the inputs to give to the program from the command. Defaults to None.\n
         i_timeout (float, optional): An individual timeout for every step of the execution. Defaults to 0.01.\n
         cwd (?, optional): Current working directory. Defaults to None.\n
@@ -80,14 +83,16 @@
     """
 
     if inputs is None:
         inputs = []
 
     p = None
     try:
+        # with subprocess.Popen(command, stdout=subprocess.PIPE,
+        #                      stdin=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=cwd, shell=shell) as p:
         # TODO with ... as p:
         p = subprocess.Popen(command, stdout=subprocess.PIPE,
                              stdin=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=cwd, shell=shell)
         p.stdin = cast(IO[bytes], p.stdin)
         p.stdout = cast(IO[bytes], p.stdout)
         p.stderr = cast(IO[bytes], p.stderr)
 
@@ -102,16 +107,16 @@
                     # new_len = len(l)
                 except TimeoutError:
                     # break
                     pass
                 except BaseException as e1:
                     raise e1
 
-        stdout: list[bytes] = []
-        stderr: list[bytes] = []
+        stdout: t_list[bytes] = []
+        stderr: t_list[bytes] = []
         for curr_input in inputs:
             if p.stdin.writable():
                 if use_write_helper:
                     __acm_write(curr_input, p=p)
                 else:
                     __acm_write(curr_input, p=p, sep="", end="")
             extend_from_stream(p.stdout, stdout)
@@ -133,15 +138,15 @@
                 p.stdin.close()
             if p.stderr is not None:
                 p.stderr.close()
             if p.stdout is not None:
                 p.stdout.close()
 
 
-def cmrt(*args, shell: bool = True) -> Generator[tuple[int, bytes], None, None]:
+def cmrt(*args, shell: bool = True) -> Generator[t_tuple[int, bytes], None, None]:
     """Executes a command and yields stdout and stderr in real-time.
 
     Args:
         shell (bool, optional): If True, the command is executed through the shell. Defaults to True.
 
     Raises:
         TypeError: if 'shell' is not boolean
```

### Comparing `danielutils-0.9.0/danielutils/Text.py` & `danielutils-0.9.5/danielutils/Text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import Union, TypeGuard
+from typing import Union
 from .Decorators.validate import validate
 from .Functions.check_foreach import check_foreach
 HEBREW_LETTERS = ['\u05D0', '\u2135', '\uFB21', '\uFB2E', '\uFB2F',
                   '\uFB30', '\uFB4F', '\u05D1', '\u2136', '\uFB31',
                   '\uFB4C', '\u05D2', '\u2137', '\uFB32', '\u05D3',
                   '\u2138', '\uFB22', '\uFB33', '\u05D4', '\uFB23',
                   '\uFB34', '\u05D5', '\uFB4B', '\uFB35', '\u05F0',
@@ -25,81 +25,81 @@
 ENGLISH_LETTERS = [chr(v) for v in range(65, 91)]+[chr(v)
                                                    for v in range(97, 123)]
 ENGLISH_LETTERS_DEC = [ord(v) for v in ENGLISH_LETTERS]
 ENGLISH_LETTERS_HEX = [hex(v) for v in ENGLISH_LETTERS_DEC]
 
 
 @validate
-def is_english(s: str) -> TypeGuard[str]:
+def is_english(s: str) -> bool:
     """returns whether the specified string is in the english language
 
     Args:
         s (str): the string to check
 
     Returns:
-        TypeGuard[str]: returns true if the string is in english
+        bool: returns true if the string is in english
     """
     return check_foreach(s, lambda c: c in ENGLISH_LETTERS)
 
 
 @validate
-def is_number(s: str) -> TypeGuard[int | float]:
+def is_number(s: str) -> bool:
     """checks if a string is a number
 
     Args:
         text (str): string to check
 
     Returns:
-        TypeGuard[int | float]: true if string is a number
+        bool: true if string is a number
     """
     return s.isnumeric()
 
 
 @validate
-def is_int(num: Union[int, float]) -> TypeGuard[int]:
+def is_int(num: Union[int, float]) -> bool:
     """_summary_
 
     Args:
         num (Union[int, float]): is a number an int
 
     Returns:
-        TypeGuard[int]: return true if num is a while number
+        bool: return true if num is a while number
     """
     if isinstance(num, int):
         return True
 
     return int(num) == num
 
 
 @validate
-def is_float(s: str) -> TypeGuard[float]:
+def is_float(s: str) -> bool:
     """checks whether a string has a float value
 
     Args:
         s (str): string to check
 
     Returns:
-        TypeGuard[float]: result
+        bool: result
     """
     try:
         float(s)
         return True
     except ValueError:
         return False
 
 
 @validate
-def is_hebrew(s: str) -> TypeGuard[str]:
+def is_hebrew(s: str) -> bool:
     """checks if a string is in hebrew
 
     Args:
         text (str): string to check
 
     Returns:
-        TypeGuard[str]: true iff all chars are hebrew
+        bool: true iff all chars are hebrew
     """
     return check_foreach(s, lambda c: c in HEBREW_LETTERS)
 
 
 @validate
 def is_binary(s: str) -> bool:
     """checks if s string has a binary value
```

### Comparing `danielutils-0.9.0/danielutils/Windows.py` & `danielutils-0.9.5/danielutils/Windows.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 # def screenshot(xy: tuple[int, int] = (0, 0), wh: tuple[int, int] = None) -> Image:
 #     """creates a screenshot of the screen in an arbitrary location and size
 
 #     Args:
 #         xy (tuple[int, int], optional): the top left location of the screenshot. Defaults to (0, 0).
-#         wh (tuple[int, int], optional): the size of the screenshot in pixels. Defaults to None. if None will 
+#         wh (tuple[int, int], optional): the size of the screenshot in pixels. Defaults to None. if None will
 #         create a screen shot of all monitors
 #     Returns:
 #         Image: _description_
 #     """
 #     if wh is None:
 #         wh = (0, 0)
 #         for monitor_index in range(get_monitor_count()):
```

### Comparing `danielutils-0.9.0/danielutils/__init__.py` & `danielutils-0.9.5/danielutils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,13 +14,14 @@
 from .DataStructures import *
 from .Math import *
 from .Path import *
 from .Windows import *
 from .Print import *
 from .Exceptions import PrintCatchOne
 from .Reflection import *
-from .DateTime import *
 from .MetaClasses import *
+from .DateTime import *
 from .Generators import *
 from .Snippets import *
 from .Aliases import *
 from .Signals import *
+from .University import *
```

### Comparing `danielutils-0.9.0/danielutils.egg-info/PKG-INFO` & `danielutils-0.9.5/danielutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.9.0
+Version: 0.9.5
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
 Keywords: functions,decorators,methods,classes,metaclasses
 Platform: All
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.10.5
+Requires-Python: >=3.8.17
 Description-Content-Type: text/markdown
 
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.9.0
+# danielutils v=0.9.5
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 # Showcase
 In [this](./READMES/) folder you can check out some more in depth showcase of some of the topics I have covered in this package
```

### Comparing `danielutils-0.9.0/danielutils.egg-info/SOURCES.txt` & `danielutils-0.9.5/danielutils.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,40 @@
 pyproject.toml
 setup.py
 danielutils/Aliases.py
 danielutils/Colors.py
 danielutils/Data.py
 danielutils/DateTime.py
 danielutils/Exceptions.py
-danielutils/Functions.py
 danielutils/IO.py
 danielutils/Internet.py
 danielutils/Path.py
 danielutils/Print.py
 danielutils/Relations.py
 danielutils/Signals.py
 danielutils/System.py
 danielutils/Text.py
 danielutils/Time.py
 danielutils/Windows.py
 danielutils/__init__.py
 danielutils.egg-info/PKG-INFO
 danielutils.egg-info/SOURCES.txt
 danielutils.egg-info/dependency_links.txt
+danielutils.egg-info/requires.txt
 danielutils.egg-info/top_level.txt
 danielutils/Classes/Convenience.py
 danielutils/Classes/Counter.py
+danielutils/Classes/Shell.py
+danielutils/Classes/Tree.py
 danielutils/Classes/__init__.py
 danielutils/Classes/frange.py
+danielutils/Classes/SortedBuiltins/__init__.py
+danielutils/Classes/SortedBuiltins/sset.py
 danielutils/Classes/TypedBuiltins/__init__.py
-danielutils/Classes/TypedBuiltins/tbase.py
+danielutils/Classes/TypedBuiltins/factory.py
 danielutils/Classes/TypedBuiltins/tdict.py
 danielutils/Classes/TypedBuiltins/tlist.py
 danielutils/Classes/TypedBuiltins/tset.py
 danielutils/Classes/TypedBuiltins/ttuple.py
 danielutils/Conversions/MainConversions.py
 danielutils/Conversions/__init__.py
 danielutils/Conversions/SpecializedConversions/__init__.py
@@ -61,16 +65,18 @@
 danielutils/Decorators/timeout.py
 danielutils/Decorators/validate.py
 danielutils/Functions/__init__.py
 danielutils/Functions/areoneof.py
 danielutils/Functions/check_foreach.py
 danielutils/Functions/isoftype.py
 danielutils/Functions/isoneof.py
+danielutils/Functions/powerset.py
 danielutils/Functions/types_subseteq.py
 danielutils/Generators/__init__.py
+danielutils/Generators/conditional_generator.py
 danielutils/Generators/generator_from_stream.py
 danielutils/Generators/join_generators.py
 danielutils/Math/Constants.py
 danielutils/Math/Functions.py
 danielutils/Math/MathPrint.py
 danielutils/Math/MathSymbols.py
 danielutils/Math/__init__.py
@@ -81,11 +87,14 @@
 danielutils/MetaClasses/OverloadMeta.py
 danielutils/MetaClasses/__init__.py
 danielutils/Reflection/File.py
 danielutils/Reflection/Function.py
 danielutils/Reflection/Module.py
 danielutils/Reflection/System.py
 danielutils/Reflection/__init__.py
-danielutils/Reflection/_get_prev_frame.py
+danielutils/Reflection/get_prev_frame.py
 danielutils/Reflection/get_traceback.py
 danielutils/Snippets/__init__.py
-danielutils/Snippets/try_get.py
+danielutils/Snippets/try_get.py
+danielutils/University/__init__.py
+danielutils/University/Databases/__init__.py
+danielutils/University/Databases/all.py
```

### Comparing `danielutils-0.9.0/pyproject.toml` & `danielutils-0.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "danielutils"
-version = "0.9.0"
+version = "0.9.5"
 authors = [
   { name="danielnachumdev", email="danielnachumdev@gmail.com" },
 ]
 description = "A python utils library for things I find useful"
 readme = "README.md"
-requires-python = ">=3.10.5"
+requires-python = ">=3.8.17"
 classifiers = [
    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     # "Operating System :: Unix",
     # "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
```

### Comparing `danielutils-0.9.0/setup.py` & `danielutils-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 def read_file(path: str) -> "list[str]":
     with codecs.open(path, 'r', 'utf-8') as f:
         return [l.strip() for l in f.readlines()]
 
 
 README_PATH = 'README.md'
 DESCRIPTION = 'A python utils library for things I find useful'
-VERSION = "0.9.0"
+VERSION = "0.9.5"
 LONG_DESCRIPTION = '\n'.join(read_file(README_PATH))
 setup(
     name="danielutils",
     version=VERSION,
     author="danielnachumdev",
     author_email="<danielnachumdev@gmail.com>",
     description=DESCRIPTION,
     long_description=open('README.md', "r", encoding="utf8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/danielnachumdev/danielutils',
     license="MIT License",
     packages=find_packages(
         exclude=["*.tests", "*.tests.*", "tests.*", "tests", "archive/"]),
-    install_requires=[],
+    install_requires=["tqdm"],
     platforms=["All"],
     keywords=['functions', 'decorators', 'methods', 'classes', 'metaclasses'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         # "Operating System :: Unix",
```

