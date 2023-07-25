# Comparing `tmp/pip_services4_components-0.0.4.tar.gz` & `tmp/pip_services4_components-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_components-0.0.4.tar", last modified: Mon Jul 24 11:25:35 2023, max compression
+gzip compressed data, was "pip_services4_components-0.0.5.tar", last modified: Tue Jul 25 18:22:46 2023, max compression
```

## Comparing `pip_services4_components-0.0.4.tar` & `pip_services4_components-0.0.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:35.014365 pip_services4_components-0.0.4/
--rw-rw-rw-   0        0        0      297 2023-07-24 07:59:11.000000 pip_services4_components-0.0.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_components-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_components-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5480 2023-07-24 11:25:35.014365 pip_services4_components-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4472 2023-07-21 15:12:36.000000 pip_services4_components-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:34.941175 pip_services4_components-0.0.4/pip_services4_components/
--rw-rw-rw-   0        0        0      305 2023-07-21 14:51:22.000000 pip_services4_components-0.0.4/pip_services4_components/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:34.972180 pip_services4_components-0.0.4/pip_services4_components/build/
--rw-rw-rw-   0        0        0     3488 2023-07-21 14:51:22.000000 pip_services4_components-0.0.4/pip_services4_components/build/CompositeFactory.py
--rw-rw-rw-   0        0        0     1016 2023-07-21 15:39:24.000000 pip_services4_components-0.0.4/pip_services4_components/build/CreateException.py
--rw-rw-rw-   0        0        0     3679 2023-07-24 07:30:35.000000 pip_services4_components-0.0.4/pip_services4_components/build/Factory.py
--rw-rw-rw-   0        0        0     1610 2023-07-21 14:51:21.000000 pip_services4_components-0.0.4/pip_services4_components/build/IFactory.py
--rw-rw-rw-   0        0        0      622 2023-07-21 14:51:22.000000 pip_services4_components-0.0.4/pip_services4_components/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:34.977180 pip_services4_components-0.0.4/pip_services4_components/config/
--rw-rw-rw-   0        0        0     7492 2023-07-21 15:12:36.000000 pip_services4_components-0.0.4/pip_services4_components/config/ConfigParams.py
--rw-rw-rw-   0        0        0     1375 2023-07-21 15:12:36.000000 pip_services4_components-0.0.4/pip_services4_components/config/IConfigurable.py
--rw-rw-rw-   0        0        0      773 2023-07-21 15:12:36.000000 pip_services4_components-0.0.4/pip_services4_components/config/IReconfigurable.py
--rw-rw-rw-   0        0        0     1901 2023-07-24 07:34:38.000000 pip_services4_components-0.0.4/pip_services4_components/config/NameResolver.py
--rw-rw-rw-   0        0        0     1374 2023-07-21 15:12:36.000000 pip_services4_components-0.0.4/pip_services4_components/config/OptionsResolver.py
--rw-rw-rw-   0        0        0     1003 2023-07-24 07:29:26.000000 pip_services4_components-0.0.4/pip_services4_components/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:34.983180 pip_services4_components-0.0.4/pip_services4_components/context/
--rw-rw-rw-   0        0        0     2488 2023-07-24 11:24:52.000000 pip_services4_components-0.0.4/pip_services4_components/context/Context.py
--rw-rw-rw-   0        0        0     5753 2023-07-24 07:30:35.000000 pip_services4_components-0.0.4/pip_services4_components/context/ContextInfo.py
--rw-rw-rw-   0        0        0     1750 2023-07-21 15:37:39.000000 pip_services4_components-0.0.4/pip_services4_components/context/ContextResolver.py
--rw-rw-rw-   0        0        0     1211 2023-07-24 08:08:12.000000 pip_services4_components-0.0.4/pip_services4_components/context/DefaultInfoFactory.py
--rw-rw-rw-   0        0        0      405 2023-07-21 15:01:50.000000 pip_services4_components-0.0.4/pip_services4_components/context/IContext.py
--rw-rw-rw-   0        0        0      764 2023-07-24 11:19:27.000000 pip_services4_components-0.0.4/pip_services4_components/context/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:34.990179 pip_services4_components-0.0.4/pip_services4_components/exec/
--rw-rw-rw-   0        0        0     2168 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/exec/Executor.py
--rw-rw-rw-   0        0        0     6293 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/exec/FixedRateTimer.py
--rw-rw-rw-   0        0        0     1450 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/exec/IExecutable.py
--rw-rw-rw-   0        0        0     1371 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/exec/INotifiable.py
--rw-rw-rw-   0        0        0      721 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/exec/IParameterized.py
--rw-rw-rw-   0        0        0     2035 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/exec/Notifier.py
--rw-rw-rw-   0        0        0     9278 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/exec/Parameters.py
--rw-rw-rw-   0        0        0      873 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/exec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:34.999363 pip_services4_components-0.0.4/pip_services4_components/refer/
--rw-rw-rw-   0        0        0     8659 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/refer/DependencyResolver.py
--rw-rw-rw-   0        0        0     9021 2023-07-24 07:36:11.000000 pip_services4_components-0.0.4/pip_services4_components/refer/Descriptor.py
--rw-rw-rw-   0        0        0     1251 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/refer/IReferenceable.py
--rw-rw-rw-   0        0        0     6129 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/refer/IReferences.py
--rw-rw-rw-   0        0        0     1075 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/refer/IUnreferenceable.py
--rw-rw-rw-   0        0        0     1990 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/refer/Reference.py
--rw-rw-rw-   0        0        0     1196 2023-07-24 07:50:07.000000 pip_services4_components-0.0.4/pip_services4_components/refer/ReferenceException.py
--rw-rw-rw-   0        0        0     2909 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/refer/Referencer.py
--rw-rw-rw-   0        0        0     8407 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/refer/References.py
--rw-rw-rw-   0        0        0     1266 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/refer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:35.007364 pip_services4_components-0.0.4/pip_services4_components/run/
--rw-rw-rw-   0        0        0     1761 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/run/Cleaner.py
--rw-rw-rw-   0        0        0     1722 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/run/Closer.py
--rw-rw-rw-   0        0        0     1090 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/run/ICleanable.py
--rw-rw-rw-   0        0        0     1262 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/run/IClosable.py
--rw-rw-rw-   0        0        0     1690 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/run/IOpenable.py
--rw-rw-rw-   0        0        0     2960 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/run/Opener.py
--rw-rw-rw-   0        0        0      692 2023-07-24 08:14:53.000000 pip_services4_components-0.0.4/pip_services4_components/run/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:34.966180 pip_services4_components-0.0.4/pip_services4_components.egg-info/
--rw-rw-rw-   0        0        0     5480 2023-07-24 11:25:34.000000 pip_services4_components-0.0.4/pip_services4_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2470 2023-07-24 11:25:34.000000 pip_services4_components-0.0.4/pip_services4_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 11:25:34.000000 pip_services4_components-0.0.4/pip_services4_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-24 11:25:34.000000 pip_services4_components-0.0.4/pip_services4_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-07-24 11:25:34.000000 pip_services4_components-0.0.4/pip_services4_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 08:13:16.000000 pip_services4_components-0.0.4/pip_services4_components.egg-info/zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-24 11:25:35.021364 pip_services4_components-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1676 2023-07-24 11:25:09.000000 pip_services4_components-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:34.932507 pip_services4_components-0.0.4/test/
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:35.009364 pip_services4_components-0.0.4/test/context/
--rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_components-0.0.4/test/context/__init__.py
--rw-rw-rw-   0        0        0     2165 2023-07-24 07:54:28.000000 pip_services4_components-0.0.4/test/context/test_ContextInfo.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:25:35.013369 pip_services4_components-0.0.4/test/exec/
--rw-rw-rw-   0        0        0      300 2021-02-28 20:21:14.000000 pip_services4_components-0.0.4/test/exec/ClassTest.py
--rw-rw-rw-   0        0        0        0 2020-12-23 20:20:18.000000 pip_services4_components-0.0.4/test/exec/__init__.py
--rw-rw-rw-   0        0        0      726 2023-07-24 07:55:26.000000 pip_services4_components-0.0.4/test/exec/test_FixedRateTimer.py
--rw-rw-rw-   0        0        0     5016 2023-07-24 07:56:33.000000 pip_services4_components-0.0.4/test/exec/test_Parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.657989 pip_services4_components-0.0.5/
+-rw-rw-rw-   0        0        0      297 2023-07-24 07:59:11.000000 pip_services4_components-0.0.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1076 2020-12-11 04:21:14.000000 pip_services4_components-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-11 04:21:14.000000 pip_services4_components-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5480 2023-07-25 18:22:46.657989 pip_services4_components-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4472 2023-07-21 15:12:36.000000 pip_services4_components-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.573567 pip_services4_components-0.0.5/pip_services4_components/
+-rw-rw-rw-   0        0        0      305 2023-07-21 14:51:22.000000 pip_services4_components-0.0.5/pip_services4_components/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.594569 pip_services4_components-0.0.5/pip_services4_components/build/
+-rw-rw-rw-   0        0        0     3488 2023-07-21 14:51:22.000000 pip_services4_components-0.0.5/pip_services4_components/build/CompositeFactory.py
+-rw-rw-rw-   0        0        0     1016 2023-07-21 15:39:24.000000 pip_services4_components-0.0.5/pip_services4_components/build/CreateException.py
+-rw-rw-rw-   0        0        0     3679 2023-07-24 07:30:35.000000 pip_services4_components-0.0.5/pip_services4_components/build/Factory.py
+-rw-rw-rw-   0        0        0     1610 2023-07-21 14:51:21.000000 pip_services4_components-0.0.5/pip_services4_components/build/IFactory.py
+-rw-rw-rw-   0        0        0      622 2023-07-21 14:51:22.000000 pip_services4_components-0.0.5/pip_services4_components/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.602568 pip_services4_components-0.0.5/pip_services4_components/config/
+-rw-rw-rw-   0        0        0     7492 2023-07-21 15:12:36.000000 pip_services4_components-0.0.5/pip_services4_components/config/ConfigParams.py
+-rw-rw-rw-   0        0        0     1375 2023-07-21 15:12:36.000000 pip_services4_components-0.0.5/pip_services4_components/config/IConfigurable.py
+-rw-rw-rw-   0        0        0      773 2023-07-21 15:12:36.000000 pip_services4_components-0.0.5/pip_services4_components/config/IReconfigurable.py
+-rw-rw-rw-   0        0        0     1901 2023-07-24 07:34:38.000000 pip_services4_components-0.0.5/pip_services4_components/config/NameResolver.py
+-rw-rw-rw-   0        0        0     1374 2023-07-21 15:12:36.000000 pip_services4_components-0.0.5/pip_services4_components/config/OptionsResolver.py
+-rw-rw-rw-   0        0        0     1003 2023-07-24 07:29:26.000000 pip_services4_components-0.0.5/pip_services4_components/config/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.611869 pip_services4_components-0.0.5/pip_services4_components/context/
+-rw-rw-rw-   0        0        0     2488 2023-07-24 11:24:52.000000 pip_services4_components-0.0.5/pip_services4_components/context/Context.py
+-rw-rw-rw-   0        0        0     5753 2023-07-24 07:30:35.000000 pip_services4_components-0.0.5/pip_services4_components/context/ContextInfo.py
+-rw-rw-rw-   0        0        0     1750 2023-07-21 15:37:39.000000 pip_services4_components-0.0.5/pip_services4_components/context/ContextResolver.py
+-rw-rw-rw-   0        0        0     1214 2023-07-25 18:21:26.000000 pip_services4_components-0.0.5/pip_services4_components/context/DefaultContextFactory.py
+-rw-rw-rw-   0        0        0      405 2023-07-21 15:01:50.000000 pip_services4_components-0.0.5/pip_services4_components/context/IContext.py
+-rw-rw-rw-   0        0        0      773 2023-07-25 18:16:24.000000 pip_services4_components-0.0.5/pip_services4_components/context/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.622869 pip_services4_components-0.0.5/pip_services4_components/exec/
+-rw-rw-rw-   0        0        0     2168 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/exec/Executor.py
+-rw-rw-rw-   0        0        0     6293 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/exec/FixedRateTimer.py
+-rw-rw-rw-   0        0        0     1450 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/exec/IExecutable.py
+-rw-rw-rw-   0        0        0     1371 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/exec/INotifiable.py
+-rw-rw-rw-   0        0        0      721 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/exec/IParameterized.py
+-rw-rw-rw-   0        0        0     2035 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/exec/Notifier.py
+-rw-rw-rw-   0        0        0     9278 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/exec/Parameters.py
+-rw-rw-rw-   0        0        0      873 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/exec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.637987 pip_services4_components-0.0.5/pip_services4_components/refer/
+-rw-rw-rw-   0        0        0     8659 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/refer/DependencyResolver.py
+-rw-rw-rw-   0        0        0     9021 2023-07-24 07:36:11.000000 pip_services4_components-0.0.5/pip_services4_components/refer/Descriptor.py
+-rw-rw-rw-   0        0        0     1251 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/refer/IReferenceable.py
+-rw-rw-rw-   0        0        0     6129 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/refer/IReferences.py
+-rw-rw-rw-   0        0        0     1075 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/refer/IUnreferenceable.py
+-rw-rw-rw-   0        0        0     1990 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/refer/Reference.py
+-rw-rw-rw-   0        0        0     1196 2023-07-24 07:50:07.000000 pip_services4_components-0.0.5/pip_services4_components/refer/ReferenceException.py
+-rw-rw-rw-   0        0        0     2909 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/refer/Referencer.py
+-rw-rw-rw-   0        0        0     8407 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/refer/References.py
+-rw-rw-rw-   0        0        0     1266 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/refer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.647990 pip_services4_components-0.0.5/pip_services4_components/run/
+-rw-rw-rw-   0        0        0     1761 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/run/Cleaner.py
+-rw-rw-rw-   0        0        0     1722 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/run/Closer.py
+-rw-rw-rw-   0        0        0     1090 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/run/ICleanable.py
+-rw-rw-rw-   0        0        0     1262 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/run/IClosable.py
+-rw-rw-rw-   0        0        0     1690 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/run/IOpenable.py
+-rw-rw-rw-   0        0        0     2960 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/run/Opener.py
+-rw-rw-rw-   0        0        0      692 2023-07-24 08:14:53.000000 pip_services4_components-0.0.5/pip_services4_components/run/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.586591 pip_services4_components-0.0.5/pip_services4_components.egg-info/
+-rw-rw-rw-   0        0        0     5480 2023-07-25 18:22:46.000000 pip_services4_components-0.0.5/pip_services4_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2473 2023-07-25 18:22:46.000000 pip_services4_components-0.0.5/pip_services4_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:22:46.000000 pip_services4_components-0.0.5/pip_services4_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-25 18:22:46.000000 pip_services4_components-0.0.5/pip_services4_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-07-25 18:22:46.000000 pip_services4_components-0.0.5/pip_services4_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 08:13:16.000000 pip_services4_components-0.0.5/pip_services4_components.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-25 18:22:46.659992 pip_services4_components-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1676 2023-07-25 18:16:59.000000 pip_services4_components-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.563583 pip_services4_components-0.0.5/test/
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.650990 pip_services4_components-0.0.5/test/context/
+-rw-rw-rw-   0        0        0       25 2021-04-12 22:36:18.000000 pip_services4_components-0.0.5/test/context/__init__.py
+-rw-rw-rw-   0        0        0     2165 2023-07-24 07:54:28.000000 pip_services4_components-0.0.5/test/context/test_ContextInfo.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:22:46.656988 pip_services4_components-0.0.5/test/exec/
+-rw-rw-rw-   0        0        0      300 2021-02-28 20:21:14.000000 pip_services4_components-0.0.5/test/exec/ClassTest.py
+-rw-rw-rw-   0        0        0        0 2020-12-23 20:20:18.000000 pip_services4_components-0.0.5/test/exec/__init__.py
+-rw-rw-rw-   0        0        0      726 2023-07-24 07:55:26.000000 pip_services4_components-0.0.5/test/exec/test_FixedRateTimer.py
+-rw-rw-rw-   0        0        0     5016 2023-07-24 07:56:33.000000 pip_services4_components-0.0.5/test/exec/test_Parameters.py
```

### Comparing `pip_services4_components-0.0.4/LICENSE` & `pip_services4_components-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/PKG-INFO` & `pip_services4_components-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_components
-Version: 0.0.4
+Version: 0.0.5
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-components-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_components-0.0.4/README.md` & `pip_services4_components-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/build/CompositeFactory.py` & `pip_services4_components-0.0.5/pip_services4_components/build/CompositeFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/build/CreateException.py` & `pip_services4_components-0.0.5/pip_services4_components/build/CreateException.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/build/Factory.py` & `pip_services4_components-0.0.5/pip_services4_components/build/Factory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/build/IFactory.py` & `pip_services4_components-0.0.5/pip_services4_components/build/IFactory.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/build/__init__.py` & `pip_services4_components-0.0.5/pip_services4_components/build/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/config/ConfigParams.py` & `pip_services4_components-0.0.5/pip_services4_components/config/ConfigParams.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/config/IConfigurable.py` & `pip_services4_components-0.0.5/pip_services4_components/config/IConfigurable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/config/IReconfigurable.py` & `pip_services4_components-0.0.5/pip_services4_components/config/IReconfigurable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/config/NameResolver.py` & `pip_services4_components-0.0.5/pip_services4_components/config/NameResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/config/OptionsResolver.py` & `pip_services4_components-0.0.5/pip_services4_components/config/OptionsResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/config/__init__.py` & `pip_services4_components-0.0.5/pip_services4_components/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/context/Context.py` & `pip_services4_components-0.0.5/pip_services4_components/context/Context.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/context/ContextInfo.py` & `pip_services4_components-0.0.5/pip_services4_components/context/ContextInfo.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/context/ContextResolver.py` & `pip_services4_components-0.0.5/pip_services4_components/context/ContextResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/context/DefaultInfoFactory.py` & `pip_services4_components-0.0.5/pip_services4_components/context/DefaultContextFactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 """
 
 from .ContextInfo import ContextInfo
 from ..build.Factory import Factory
 from ..refer.Descriptor import Descriptor
 
 
-class DefaultInfoFactory(Factory):
+class DefaultContextFactory(Factory):
     """
     Creates information components by their descriptors.
 
     See :class:`IFactory <pip_services4_components.build.IFactory.IFactory>`,
     :class:`ContextInfo <pip_services4_components.context.ContextInfo.ContextInfo>`
     """
 
-    ContextInfoDescriptor = Descriptor("pip-services", "context-context", "default", "*", "1.0")
-    ContainerInfoDescriptor = Descriptor("pip-services", "container-context", "default", "*", "1.0")
+    ContextInfoDescriptor = Descriptor("pip-services", "context-info", "default", "*", "1.0")
+    ContainerInfoDescriptor = Descriptor("pip-services", "container-info", "default", "*", "1.0")
 
     def __init__(self):
         """
         Create a new instance of the factory.
         """
         super().__init__()
-        self.register_as_type(DefaultInfoFactory.ContextInfoDescriptor, ContextInfo)
-        self.register_as_type(DefaultInfoFactory.ContainerInfoDescriptor, ContextInfo)
+        self.register_as_type(DefaultContextFactory.ContextInfoDescriptor, ContextInfo)
+        self.register_as_type(DefaultContextFactory.ContainerInfoDescriptor, ContextInfo)
```

### Comparing `pip_services4_components-0.0.4/pip_services4_components/context/__init__.py` & `pip_services4_components-0.0.5/pip_services4_components/context/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     logging functions we need to know what source we are logging from – what is
     the processes name, what the process is/does.
     
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
 
-__all__ = ['ContextInfo', 'DefaultInfoFactory', 'IContext', 'Context', 'ContextResolver']
+__all__ = ['ContextInfo', 'DefaultContextFactory', 'IContext', 'Context', 'ContextResolver']
 
 from .ContextInfo import ContextInfo
-from .DefaultInfoFactory import DefaultInfoFactory
+from .DefaultContextFactory import DefaultContextFactory
 from .IContext import IContext
 from .Context import Context
 from .ContextResolver import ContextResolver
```

### Comparing `pip_services4_components-0.0.4/pip_services4_components/exec/Executor.py` & `pip_services4_components-0.0.5/pip_services4_components/exec/Executor.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/exec/FixedRateTimer.py` & `pip_services4_components-0.0.5/pip_services4_components/exec/FixedRateTimer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/exec/IExecutable.py` & `pip_services4_components-0.0.5/pip_services4_components/exec/IExecutable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/exec/INotifiable.py` & `pip_services4_components-0.0.5/pip_services4_components/exec/INotifiable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/exec/IParameterized.py` & `pip_services4_components-0.0.5/pip_services4_components/exec/IParameterized.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/exec/Notifier.py` & `pip_services4_components-0.0.5/pip_services4_components/exec/Notifier.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/exec/Parameters.py` & `pip_services4_components-0.0.5/pip_services4_components/exec/Parameters.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/exec/__init__.py` & `pip_services4_components-0.0.5/pip_services4_components/exec/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/DependencyResolver.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/DependencyResolver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/Descriptor.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/Descriptor.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/IReferenceable.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/IReferenceable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/IReferences.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/IReferences.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/IUnreferenceable.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/IUnreferenceable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/Reference.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/Reference.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/ReferenceException.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/ReferenceException.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/Referencer.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/Referencer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/References.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/References.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/refer/__init__.py` & `pip_services4_components-0.0.5/pip_services4_components/refer/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/run/Cleaner.py` & `pip_services4_components-0.0.5/pip_services4_components/run/Cleaner.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/run/Closer.py` & `pip_services4_components-0.0.5/pip_services4_components/run/Closer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/run/ICleanable.py` & `pip_services4_components-0.0.5/pip_services4_components/run/ICleanable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/run/IClosable.py` & `pip_services4_components-0.0.5/pip_services4_components/run/IClosable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/run/IOpenable.py` & `pip_services4_components-0.0.5/pip_services4_components/run/IOpenable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/run/Opener.py` & `pip_services4_components-0.0.5/pip_services4_components/run/Opener.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components/run/__init__.py` & `pip_services4_components-0.0.5/pip_services4_components/run/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/pip_services4_components.egg-info/PKG-INFO` & `pip_services4_components-0.0.5/pip_services4_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-components
-Version: 0.0.4
+Version: 0.0.5
 Summary: Component definitions for Pip.Services in Python
 Home-page: https://github.com/pip-services4/pip-services4-python/pip-services4-components-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_components-0.0.4/pip_services4_components.egg-info/SOURCES.txt` & `pip_services4_components-0.0.5/pip_services4_components.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 pip_services4_components/config/IReconfigurable.py
 pip_services4_components/config/NameResolver.py
 pip_services4_components/config/OptionsResolver.py
 pip_services4_components/config/__init__.py
 pip_services4_components/context/Context.py
 pip_services4_components/context/ContextInfo.py
 pip_services4_components/context/ContextResolver.py
-pip_services4_components/context/DefaultInfoFactory.py
+pip_services4_components/context/DefaultContextFactory.py
 pip_services4_components/context/IContext.py
 pip_services4_components/context/__init__.py
 pip_services4_components/exec/Executor.py
 pip_services4_components/exec/FixedRateTimer.py
 pip_services4_components/exec/IExecutable.py
 pip_services4_components/exec/INotifiable.py
 pip_services4_components/exec/IParameterized.py
```

### Comparing `pip_services4_components-0.0.4/setup.py` & `pip_services4_components-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 try:
     readme = open('README.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_components',
-    version='0.0.4',
+    version='0.0.5',
     url='https://github.com/pip-services4/pip-services4-python/pip-services4-components-python',
     license='MIT',
     description='Component definitions for Pip.Services in Python',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     long_description=readme,
     long_description_content_type="text/markdown",
```

### Comparing `pip_services4_components-0.0.4/test/context/test_ContextInfo.py` & `pip_services4_components-0.0.5/test/context/test_ContextInfo.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/test/exec/test_FixedRateTimer.py` & `pip_services4_components-0.0.5/test/exec/test_FixedRateTimer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_components-0.0.4/test/exec/test_Parameters.py` & `pip_services4_components-0.0.5/test/exec/test_Parameters.py`

 * *Files identical despite different names*

