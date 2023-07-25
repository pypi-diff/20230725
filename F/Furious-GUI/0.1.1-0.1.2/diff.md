# Comparing `tmp/Furious-GUI-0.1.1.tar.gz` & `tmp/Furious-GUI-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.1.1.tar", last modified: Mon Jul 24 12:49:20 2023, max compression
+gzip compressed data, was "Furious-GUI-0.1.2.tar", last modified: Tue Jul 25 08:59:32 2023, max compression
```

## Comparing `Furious-GUI-0.1.1.tar` & `Furious-GUI-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.414536 Furious-GUI-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.070903 Furious-GUI-0.1.1/Furious/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.133483 Furious-GUI-0.1.1/Furious/Action/
--rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Connect.py
--rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/EditConfiguration.py
--rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Exit.py
--rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Export.py
--rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Import.py
--rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Language.py
--rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Routing.py
--rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/Settings.py
--rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Action/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.164902 Furious-GUI-0.1.1/Furious/Core/
--rw-rw-rw-   0        0        0    19804 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Core/Configuration.py
--rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Core/Core.py
--rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Core/Intellisense.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.180019 Furious-GUI-0.1.1/Furious/Gui/
--rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Gui/Action.py
--rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Gui/Icon.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.258603 Furious-GUI-0.1.1/Furious/Utility/
--rw-rw-rw-   0        0        0     1011 2023-07-24 12:48:19.000000 Furious-GUI-0.1.1/Furious/Utility/Constants.py
--rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Process.py
--rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Proxy.py
--rw-rw-rw-   0        0        0    42815 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Resources.py
--rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Settings.py
--rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/StartupOnBoot.py
--rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Theme.py
--rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Translator.py
--rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/Utility.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Utility/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-24 12:48:46.000000 Furious-GUI-0.1.1/Furious/Version.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.320942 Furious-GUI-0.1.1/Furious/Widget/
--rw-rw-rw-   0        0        0     8812 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/Application.py
--rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/ConnectingProgressBar.py
--rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/EditConfiguration.py
--rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/ExportQRCode.py
--rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/IndentSpinBox.py
--rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/LogViewer.py
--rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/SystemTrayIcon.py
--rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/Widget.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/Widget/__init__.py
--rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/__init__.py
--rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.039841 Furious-GUI-0.1.1/Furious/data/
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.336384 Furious-GUI-0.1.1/Furious/data/font/
--rw-rw-rw-   0        0        0   624892 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/font/CascadiaMono
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.352817 Furious-GUI-0.1.1/Furious/data/hysteria/
--rw-rw-rw-   0        0        0  1427940 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/hysteria/bypass-mainland-China.acl
--rw-rw-rw-   0        0        0  5872899 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/hysteria/country.mmdb
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.383423 Furious-GUI-0.1.1/Furious/data/xray/
--rw-rw-rw-   0        0        0 10006207 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/xray/geoip.dat
--rw-rw-rw-   0        0        0  1512983 2023-07-24 11:35:24.000000 Furious-GUI-0.1.1/Furious/data/xray/geosite.dat
-drwxrwxrwx   0        0        0        0 2023-07-24 12:49:20.414536 Furious-GUI-0.1.1/Furious_GUI.egg-info/
--rw-rw-rw-   0        0        0     6568 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-24 12:49:19.000000 Furious-GUI-0.1.1/Furious_GUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-07-24 11:48:32.000000 Furious-GUI-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     6568 2023-07-24 12:49:20.414536 Furious-GUI-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5566 2023-07-24 12:41:32.000000 Furious-GUI-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 12:49:20.414536 Furious-GUI-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1998 2023-07-24 11:58:03.000000 Furious-GUI-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.172365 Furious-GUI-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.094029 Furious-GUI-0.1.2/Furious/
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.109577 Furious-GUI-0.1.2/Furious/Action/
+-rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Connect.py
+-rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/EditConfiguration.py
+-rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Exit.py
+-rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Export.py
+-rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Import.py
+-rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Language.py
+-rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Routing.py
+-rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Settings.py
+-rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.109577 Furious-GUI-0.1.2/Furious/Core/
+-rw-rw-rw-   0        0        0    19756 2023-07-25 08:47:36.000000 Furious-GUI-0.1.2/Furious/Core/Configuration.py
+-rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Core/Core.py
+-rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Core/Intellisense.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.094029 Furious-GUI-0.1.2/Furious/Data/
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.109577 Furious-GUI-0.1.2/Furious/Data/font/
+-rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/font/CascadiaMono
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.109577 Furious-GUI-0.1.2/Furious/Data/hysteria/
+-rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/hysteria/country.mmdb
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.125627 Furious-GUI-0.1.2/Furious/Data/xray/
+-rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/xray/geoip.dat
+-rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/xray/geosite.dat
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.141309 Furious-GUI-0.1.2/Furious/Gui/
+-rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Gui/Action.py
+-rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Gui/Icon.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.141309 Furious-GUI-0.1.2/Furious/Utility/
+-rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.2/Furious/Utility/Constants.py
+-rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Process.py
+-rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Proxy.py
+-rw-rw-rw-   0        0        0    42815 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Resources.py
+-rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Settings.py
+-rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/StartupOnBoot.py
+-rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Theme.py
+-rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Translator.py
+-rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Utility.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-25 08:47:36.000000 Furious-GUI-0.1.2/Furious/Version.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.156808 Furious-GUI-0.1.2/Furious/Widget/
+-rw-rw-rw-   0        0        0     8812 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/Application.py
+-rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/ConnectingProgressBar.py
+-rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/EditConfiguration.py
+-rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/ExportQRCode.py
+-rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/IndentSpinBox.py
+-rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/LogViewer.py
+-rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/SystemTrayIcon.py
+-rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/Widget.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/__init__.py
+-rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.172365 Furious-GUI-0.1.2/Furious_GUI.egg-info/
+-rw-rw-rw-   0        0        0     6773 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6773 2023-07-25 08:59:32.172365 Furious-GUI-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5760 2023-07-25 08:55:22.000000 Furious-GUI-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 08:59:32.172365 Furious-GUI-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2009 2023-07-25 08:58:53.000000 Furious-GUI-0.1.2/setup.py
```

### Comparing `Furious-GUI-0.1.1/Furious/Action/Connect.py` & `Furious-GUI-0.1.2/Furious/Action/Connect.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Action/Export.py` & `Furious-GUI-0.1.2/Furious/Action/Export.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Action/Import.py` & `Furious-GUI-0.1.2/Furious/Action/Import.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Action/Language.py` & `Furious-GUI-0.1.2/Furious/Action/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Action/Routing.py` & `Furious-GUI-0.1.2/Furious/Action/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Action/Settings.py` & `Furious-GUI-0.1.2/Furious/Action/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Core/Configuration.py` & `Furious-GUI-0.1.2/Furious/Core/Configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,31 +428,29 @@
 
     def getUserObject(self):
         if self.protocol == 'vmess':
             UserObject = {
                 'id': self.uuid_,
                 'security': self.encryption,
                 # Extension
-                # TODO
-                'email': 'user@furious.com',
+                'email': 'user@Furious.GUI',
             }
 
             # For VMess(V2rayN share standard) only.
             if self.kwargs.get('aid') is not None:
                 UserObject['alterId'] = self.kwargs.get('aid')
 
             return UserObject
 
         if self.protocol == 'vless':
             UserObject = {
                 'id': self.uuid_,
                 'encryption': self.encryption,
                 # Extension
-                # TODO
-                'email': 'user@furious.com',
+                'email': 'user@Furious.GUI',
             }
 
             if self.kwargs.get('flow'):
                 # flow is empty, TLS. Otherwise, XTLS.
                 UserObject['flow'] = self.kwargs.get('flow')
 
             return UserObject
```

### Comparing `Furious-GUI-0.1.1/Furious/Core/Core.py` & `Furious-GUI-0.1.2/Furious/Core/Core.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Core/Intellisense.py` & `Furious-GUI-0.1.2/Furious/Core/Intellisense.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Gui/Action.py` & `Furious-GUI-0.1.2/Furious/Gui/Action.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Utility/Constants.py` & `Furious-GUI-0.1.2/Furious/Utility/Constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 
 import math
 import pathlib
 import platform
 
 APPLICATION_NAME = 'Furious'
 APPLICATION_VERSION = __version__
-APPLICATION_MACOS_SIGNATURE = 'com.furious'
+APPLICATION_MACOS_SIGNATURE = 'com.Furious'
 APPLICATION_ABOUT_PAGE = 'https://github.com/LorenEteval/Furious/'
 APPLICATION_REPO_OWNER_NAME = 'LorenEteval'
 APPLICATION_REPO_NAME = 'Furious'
 
 ORGANIZATION_NAME = 'Furious'
-ORGANIZATION_DOMAIN = 'furious.network'
+ORGANIZATION_DOMAIN = 'Furious.GUI'
 
 PLATFORM = platform.system()
 
 LOCAL_SERVER_NAME = '891ad49d-8996-43cb-820c-d9baf42a04de'
 
 GOLDEN_RATIO = (math.sqrt(5) - 1) / 2
 
 SYSTEM_LANGUAGE = QtCore.QLocale().name()[:2].upper()
 
 ROOT_DIR = pathlib.Path(__file__).resolve().parent.parent
-DATA_DIR = ROOT_DIR / 'data'
-CRASH_LOG_DIR = ROOT_DIR / 'crashLog'
+DATA_DIR = ROOT_DIR / 'Data'
+CRASH_LOG_DIR = ROOT_DIR / 'CrashLog'
 
 PROXY_SERVER_BYPASS = (
     'localhost;*.local;127.*;10.*;172.16.*;172.17.*;'
     '172.18.*;172.19.*;172.20.*;172.21.*;172.22.*;172.23.*;172.24.*;172.25.*;'
     '172.26.*;172.27.*;172.28.*;172.29.*;172.30.*;172.31.*;192.168.*'
 )
```

### Comparing `Furious-GUI-0.1.1/Furious/Utility/Process.py` & `Furious-GUI-0.1.2/Furious/Utility/Process.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Utility/Proxy.py` & `Furious-GUI-0.1.2/Furious/Utility/Proxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Utility/Resources.py` & `Furious-GUI-0.1.2/Furious/Utility/Resources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Utility/Settings.py` & `Furious-GUI-0.1.2/Furious/Utility/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.1.2/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Utility/Theme.py` & `Furious-GUI-0.1.2/Furious/Utility/Theme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Utility/Translator.py` & `Furious-GUI-0.1.2/Furious/Utility/Translator.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Utility/Utility.py` & `Furious-GUI-0.1.2/Furious/Utility/Utility.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Widget/Application.py` & `Furious-GUI-0.1.2/Furious/Widget/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Widget/ConnectingProgressBar.py` & `Furious-GUI-0.1.2/Furious/Widget/ConnectingProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Widget/EditConfiguration.py` & `Furious-GUI-0.1.2/Furious/Widget/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Widget/ExportQRCode.py` & `Furious-GUI-0.1.2/Furious/Widget/ExportQRCode.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.1.2/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Widget/LogViewer.py` & `Furious-GUI-0.1.2/Furious/Widget/LogViewer.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.1.2/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/Widget/Widget.py` & `Furious-GUI-0.1.2/Furious/Widget/Widget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/__main__.py` & `Furious-GUI-0.1.2/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/data/font/CascadiaMono` & `Furious-GUI-0.1.2/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.1.2/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/data/hysteria/country.mmdb` & `Furious-GUI-0.1.2/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/data/xray/geoip.dat` & `Furious-GUI-0.1.2/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious/data/xray/geosite.dat` & `Furious-GUI-0.1.2/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.1.2/Furious_GUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.1
-Summary: A cross-platform GUI client that launches your beloved GFW to outer space.
+Version: 0.1.2
+Summary: A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: End Users/Desktop
@@ -19,15 +19,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: Proxy Servers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Furious
 
-A cross-platform GUI client that launches your beloved GFW to outer space.
+A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.
 Support [Xray-core](https://github.com/XTLS/Xray-core)
 and [hysteria](https://github.com/apernet/hysteria).
 
 ## Features
 
 * Runs seamlessly on Windows, macOS and Linux.
 * Built-in support for [Xray-core](https://github.com/XTLS/Xray-core)
@@ -106,14 +106,28 @@
 
 ```
 Furious
 ```
 
 Furious will enable startup on boot by default if it's launched for the first time. Happy browsing!
 
+## Run From Source
+
+Clone this repository and enter the project folder. Install requirements:
+
+```
+pip install -r requirements.txt
+```
+
+Run:
+
+```
+python -m Furious
+```
+
 ## Core Installation Script
 
 Below are some one-click/automatic installation script that's been tested to work in Furious.
 
 | Project Address                                                   |  Supported Core Installation  | Share Link Import Support? | JSON Import Support? |
 |-------------------------------------------------------------------|:-----------------------------:|:--------------------------:|:--------------------:|
 | [233boy/v2ray](https://github.com/233boy/v2ray)                   |          v2ray-core           |            Yes             |          /           |
```

### Comparing `Furious-GUI-0.1.1/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.1.2/Furious_GUI.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 Furious/Action/Routing.py
 Furious/Action/Settings.py
 Furious/Action/__init__.py
 Furious/Core/Configuration.py
 Furious/Core/Core.py
 Furious/Core/Intellisense.py
 Furious/Core/__init__.py
+Furious/Data/font/CascadiaMono
+Furious/Data/hysteria/bypass-mainland-China.acl
+Furious/Data/hysteria/country.mmdb
+Furious/Data/xray/geoip.dat
+Furious/Data/xray/geosite.dat
 Furious/Gui/Action.py
 Furious/Gui/Icon.py
 Furious/Gui/__init__.py
 Furious/Utility/Constants.py
 Furious/Utility/Process.py
 Furious/Utility/Proxy.py
 Furious/Utility/Resources.py
@@ -35,18 +40,13 @@
 Furious/Widget/EditConfiguration.py
 Furious/Widget/ExportQRCode.py
 Furious/Widget/IndentSpinBox.py
 Furious/Widget/LogViewer.py
 Furious/Widget/SystemTrayIcon.py
 Furious/Widget/Widget.py
 Furious/Widget/__init__.py
-Furious/data/font/CascadiaMono
-Furious/data/hysteria/bypass-mainland-China.acl
-Furious/data/hysteria/country.mmdb
-Furious/data/xray/geoip.dat
-Furious/data/xray/geosite.dat
 Furious_GUI.egg-info/PKG-INFO
 Furious_GUI.egg-info/SOURCES.txt
 Furious_GUI.egg-info/dependency_links.txt
 Furious_GUI.egg-info/entry_points.txt
 Furious_GUI.egg-info/requires.txt
 Furious_GUI.egg-info/top_level.txt
```

### Comparing `Furious-GUI-0.1.1/LICENSE` & `Furious-GUI-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.1/PKG-INFO` & `Furious-GUI-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.1
-Summary: A cross-platform GUI client that launches your beloved GFW to outer space.
+Version: 0.1.2
+Summary: A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: End Users/Desktop
@@ -19,15 +19,15 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: Proxy Servers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Furious
 
-A cross-platform GUI client that launches your beloved GFW to outer space.
+A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.
 Support [Xray-core](https://github.com/XTLS/Xray-core)
 and [hysteria](https://github.com/apernet/hysteria).
 
 ## Features
 
 * Runs seamlessly on Windows, macOS and Linux.
 * Built-in support for [Xray-core](https://github.com/XTLS/Xray-core)
@@ -106,14 +106,28 @@
 
 ```
 Furious
 ```
 
 Furious will enable startup on boot by default if it's launched for the first time. Happy browsing!
 
+## Run From Source
+
+Clone this repository and enter the project folder. Install requirements:
+
+```
+pip install -r requirements.txt
+```
+
+Run:
+
+```
+python -m Furious
+```
+
 ## Core Installation Script
 
 Below are some one-click/automatic installation script that's been tested to work in Furious.
 
 | Project Address                                                   |  Supported Core Installation  | Share Link Import Support? | JSON Import Support? |
 |-------------------------------------------------------------------|:-----------------------------:|:--------------------------:|:--------------------:|
 | [233boy/v2ray](https://github.com/233boy/v2ray)                   |          v2ray-core           |            Yes             |          /           |
```

### Comparing `Furious-GUI-0.1.1/README.md` & `Furious-GUI-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Furious
 
-A cross-platform GUI client that launches your beloved GFW to outer space.
+A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.
 Support [Xray-core](https://github.com/XTLS/Xray-core)
 and [hysteria](https://github.com/apernet/hysteria).
 
 ## Features
 
 * Runs seamlessly on Windows, macOS and Linux.
 * Built-in support for [Xray-core](https://github.com/XTLS/Xray-core)
@@ -83,14 +83,28 @@
 
 ```
 Furious
 ```
 
 Furious will enable startup on boot by default if it's launched for the first time. Happy browsing!
 
+## Run From Source
+
+Clone this repository and enter the project folder. Install requirements:
+
+```
+pip install -r requirements.txt
+```
+
+Run:
+
+```
+python -m Furious
+```
+
 ## Core Installation Script
 
 Below are some one-click/automatic installation script that's been tested to work in Furious.
 
 | Project Address                                                   |  Supported Core Installation  | Share Link Import Support? | JSON Import Support? |
 |-------------------------------------------------------------------|:-----------------------------:|:--------------------------:|:--------------------:|
 | [233boy/v2ray](https://github.com/233boy/v2ray)                   |          v2ray-core           |            Yes             |          /           |
```

### Comparing `Furious-GUI-0.1.1/setup.py` & `Furious-GUI-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='Furious-GUI',
     version=__version__,
     license='GPL v3.0',
-    description='A cross-platform GUI client that launches your beloved GFW to outer space.',
+    description='A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Loren Eteval',
     author_email='loren.eteval@proton.me',
     url='https://github.com/LorenEteval/Furious',
     packages=find_packages(),
-    package_data={'Furious': ['data/**']},
+    package_data={'Furious': ['Data/**']},
     include_package_data=True,
     install_requires=get_install_requires(),
     entry_points={
         'gui_scripts': [
             'Furious = Furious.__main__:main',
         ],
     },
```

