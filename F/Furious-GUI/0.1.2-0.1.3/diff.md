# Comparing `tmp/Furious-GUI-0.1.2.tar.gz` & `tmp/Furious-GUI-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.1.2.tar", last modified: Tue Jul 25 08:59:32 2023, max compression
+gzip compressed data, was "Furious-GUI-0.1.3.tar", last modified: Tue Jul 25 09:11:56 2023, max compression
```

## Comparing `Furious-GUI-0.1.2.tar` & `Furious-GUI-0.1.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.172365 Furious-GUI-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.094029 Furious-GUI-0.1.2/Furious/
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.109577 Furious-GUI-0.1.2/Furious/Action/
--rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Connect.py
--rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/EditConfiguration.py
--rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Exit.py
--rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Export.py
--rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Import.py
--rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Language.py
--rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Routing.py
--rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/Settings.py
--rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Action/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.109577 Furious-GUI-0.1.2/Furious/Core/
--rw-rw-rw-   0        0        0    19756 2023-07-25 08:47:36.000000 Furious-GUI-0.1.2/Furious/Core/Configuration.py
--rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Core/Core.py
--rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Core/Intellisense.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.094029 Furious-GUI-0.1.2/Furious/Data/
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.109577 Furious-GUI-0.1.2/Furious/Data/font/
--rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/font/CascadiaMono
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.109577 Furious-GUI-0.1.2/Furious/Data/hysteria/
--rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/hysteria/bypass-mainland-China.acl
--rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/hysteria/country.mmdb
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.125627 Furious-GUI-0.1.2/Furious/Data/xray/
--rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/xray/geoip.dat
--rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/Furious/Data/xray/geosite.dat
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.141309 Furious-GUI-0.1.2/Furious/Gui/
--rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Gui/Action.py
--rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Gui/Icon.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.141309 Furious-GUI-0.1.2/Furious/Utility/
--rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.2/Furious/Utility/Constants.py
--rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Process.py
--rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Proxy.py
--rw-rw-rw-   0        0        0    42815 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Resources.py
--rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Settings.py
--rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/StartupOnBoot.py
--rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Theme.py
--rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Translator.py
--rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/Utility.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Utility/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-25 08:47:36.000000 Furious-GUI-0.1.2/Furious/Version.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.156808 Furious-GUI-0.1.2/Furious/Widget/
--rw-rw-rw-   0        0        0     8812 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/Application.py
--rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/ConnectingProgressBar.py
--rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/EditConfiguration.py
--rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/ExportQRCode.py
--rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/IndentSpinBox.py
--rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/LogViewer.py
--rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/SystemTrayIcon.py
--rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/Widget.py
--rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/Widget/__init__.py
--rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/__init__.py
--rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.2/Furious/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:59:32.172365 Furious-GUI-0.1.2/Furious_GUI.egg-info/
--rw-rw-rw-   0        0        0     6773 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 08:59:32.000000 Furious-GUI-0.1.2/Furious_GUI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6773 2023-07-25 08:59:32.172365 Furious-GUI-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5760 2023-07-25 08:55:22.000000 Furious-GUI-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-25 08:59:32.172365 Furious-GUI-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2009 2023-07-25 08:58:53.000000 Furious-GUI-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.846431 Furious-GUI-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.768631 Furious-GUI-0.1.3/Furious/
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.768631 Furious-GUI-0.1.3/Furious/Action/
+-rw-rw-rw-   0        0        0    23373 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Action/Connect.py
+-rw-rw-rw-   0        0        0      487 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Action/EditConfiguration.py
+-rw-rw-rw-   0        0        0      450 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Action/Exit.py
+-rw-rw-rw-   0        0        0     7140 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Action/Export.py
+-rw-rw-rw-   0        0        0    12949 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Action/Import.py
+-rw-rw-rw-   0        0        0     1514 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Action/Language.py
+-rw-rw-rw-   0        0        0     1724 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Action/Routing.py
+-rw-rw-rw-   0        0        0     2417 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Action/Settings.py
+-rw-rw-rw-   0        0        0      268 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Action/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.768631 Furious-GUI-0.1.3/Furious/Core/
+-rw-rw-rw-   0        0        0    19756 2023-07-25 08:47:36.000000 Furious-GUI-0.1.3/Furious/Core/Configuration.py
+-rw-rw-rw-   0        0        0     4755 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Core/Core.py
+-rw-rw-rw-   0        0        0     3499 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Core/Intellisense.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.752579 Furious-GUI-0.1.3/Furious/Data/
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.784240 Furious-GUI-0.1.3/Furious/Data/font/
+-rw-rw-rw-   0        0        0   624892 2023-07-25 08:47:27.000000 Furious-GUI-0.1.3/Furious/Data/font/CascadiaMono
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.784240 Furious-GUI-0.1.3/Furious/Data/hysteria/
+-rw-rw-rw-   0        0        0  1427940 2023-07-25 08:47:27.000000 Furious-GUI-0.1.3/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-rw-rw-   0        0        0  5872899 2023-07-25 08:47:27.000000 Furious-GUI-0.1.3/Furious/Data/hysteria/country.mmdb
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.799780 Furious-GUI-0.1.3/Furious/Data/xray/
+-rw-rw-rw-   0        0        0 10006207 2023-07-25 08:47:27.000000 Furious-GUI-0.1.3/Furious/Data/xray/geoip.dat
+-rw-rw-rw-   0        0        0  1512983 2023-07-25 08:47:27.000000 Furious-GUI-0.1.3/Furious/Data/xray/geosite.dat
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.799780 Furious-GUI-0.1.3/Furious/Gui/
+-rw-rw-rw-   0        0        0     4736 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Gui/Action.py
+-rw-rw-rw-   0        0        0      180 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Gui/Icon.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Gui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.815398 Furious-GUI-0.1.3/Furious/Utility/
+-rw-rw-rw-   0        0        0     1007 2023-07-25 08:47:36.000000 Furious-GUI-0.1.3/Furious/Utility/Constants.py
+-rw-rw-rw-   0        0        0     2535 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Utility/Process.py
+-rw-rw-rw-   0        0        0     7375 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Utility/Proxy.py
+-rw-rw-rw-   0        0        0    42815 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Utility/Resources.py
+-rw-rw-rw-   0        0        0     2494 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Utility/Settings.py
+-rw-rw-rw-   0        0        0     5829 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Utility/StartupOnBoot.py
+-rw-rw-rw-   0        0        0     2364 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Utility/Theme.py
+-rw-rw-rw-   0        0        0    24098 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Utility/Translator.py
+-rw-rw-rw-   0        0        0     5005 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Utility/Utility.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Utility/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-25 09:11:06.000000 Furious-GUI-0.1.3/Furious/Version.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.830879 Furious-GUI-0.1.3/Furious/Widget/
+-rw-rw-rw-   0        0        0     8812 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Widget/Application.py
+-rw-rw-rw-   0        0        0     1975 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Widget/ConnectingProgressBar.py
+-rw-rw-rw-   0        0        0    66998 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Widget/EditConfiguration.py
+-rw-rw-rw-   0        0        0     1733 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Widget/ExportQRCode.py
+-rw-rw-rw-   0        0        0     1946 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Widget/IndentSpinBox.py
+-rw-rw-rw-   0        0        0     6618 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Widget/LogViewer.py
+-rw-rw-rw-   0        0        0     2811 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Widget/SystemTrayIcon.py
+-rw-rw-rw-   0        0        0     3808 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Widget/Widget.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/Widget/__init__.py
+-rw-rw-rw-   0        0        0       32 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/__init__.py
+-rw-rw-rw-   0        0        0     4260 2023-07-24 11:35:24.000000 Furious-GUI-0.1.3/Furious/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 09:11:56.846431 Furious-GUI-0.1.3/Furious_GUI.egg-info/
+-rw-rw-rw-   0        0        0     6773 2023-07-25 09:11:56.000000 Furious-GUI-0.1.3/Furious_GUI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-07-25 09:11:56.000000 Furious-GUI-0.1.3/Furious_GUI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 09:11:56.000000 Furious-GUI-0.1.3/Furious_GUI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-25 09:11:56.000000 Furious-GUI-0.1.3/Furious_GUI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       82 2023-07-25 09:11:56.000000 Furious-GUI-0.1.3/Furious_GUI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 09:11:56.000000 Furious-GUI-0.1.3/Furious_GUI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-07-25 08:47:27.000000 Furious-GUI-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6773 2023-07-25 09:11:56.846431 Furious-GUI-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5760 2023-07-25 09:11:06.000000 Furious-GUI-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 09:11:56.846431 Furious-GUI-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2009 2023-07-25 08:58:53.000000 Furious-GUI-0.1.3/setup.py
```

### Comparing `Furious-GUI-0.1.2/Furious/Action/Connect.py` & `Furious-GUI-0.1.3/Furious/Action/Connect.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Action/Export.py` & `Furious-GUI-0.1.3/Furious/Action/Export.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Action/Import.py` & `Furious-GUI-0.1.3/Furious/Action/Import.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Action/Language.py` & `Furious-GUI-0.1.3/Furious/Action/Language.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Action/Routing.py` & `Furious-GUI-0.1.3/Furious/Action/Routing.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Action/Settings.py` & `Furious-GUI-0.1.3/Furious/Action/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Core/Configuration.py` & `Furious-GUI-0.1.3/Furious/Core/Configuration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Core/Core.py` & `Furious-GUI-0.1.3/Furious/Core/Core.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Core/Intellisense.py` & `Furious-GUI-0.1.3/Furious/Core/Intellisense.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Data/font/CascadiaMono` & `Furious-GUI-0.1.3/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.1.3/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Data/hysteria/country.mmdb` & `Furious-GUI-0.1.3/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Data/xray/geoip.dat` & `Furious-GUI-0.1.3/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Data/xray/geosite.dat` & `Furious-GUI-0.1.3/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Gui/Action.py` & `Furious-GUI-0.1.3/Furious/Gui/Action.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Utility/Constants.py` & `Furious-GUI-0.1.3/Furious/Utility/Constants.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Utility/Process.py` & `Furious-GUI-0.1.3/Furious/Utility/Process.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Utility/Proxy.py` & `Furious-GUI-0.1.3/Furious/Utility/Proxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Utility/Resources.py` & `Furious-GUI-0.1.3/Furious/Utility/Resources.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Utility/Settings.py` & `Furious-GUI-0.1.3/Furious/Utility/Settings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.1.3/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Utility/Theme.py` & `Furious-GUI-0.1.3/Furious/Utility/Theme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Utility/Translator.py` & `Furious-GUI-0.1.3/Furious/Utility/Translator.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Utility/Utility.py` & `Furious-GUI-0.1.3/Furious/Utility/Utility.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Widget/Application.py` & `Furious-GUI-0.1.3/Furious/Widget/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Widget/ConnectingProgressBar.py` & `Furious-GUI-0.1.3/Furious/Widget/ConnectingProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Widget/EditConfiguration.py` & `Furious-GUI-0.1.3/Furious/Widget/EditConfiguration.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Widget/ExportQRCode.py` & `Furious-GUI-0.1.3/Furious/Widget/ExportQRCode.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.1.3/Furious/Widget/IndentSpinBox.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Widget/LogViewer.py` & `Furious-GUI-0.1.3/Furious/Widget/LogViewer.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Widget/SystemTrayIcon.py` & `Furious-GUI-0.1.3/Furious/Widget/SystemTrayIcon.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/Widget/Widget.py` & `Furious-GUI-0.1.3/Furious/Widget/Widget.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious/__main__.py` & `Furious-GUI-0.1.3/Furious/__main__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.1.3/Furious_GUI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.2
+Version: 0.1.3
 Summary: A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -46,29 +46,29 @@
 * Built-in user-friendly feature.
 * ...
 
 ## Sreenshot
 
 ### Windows
 
-![Windows-Light-EN](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Windows-Light-EN.png)
+![Windows-Light-EN](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Windows-Light-EN.png)
 
-![Windows-Light-CN](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Windows-Light-CN.png)
+![Windows-Light-CN](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Windows-Light-CN.png)
 
 ### macOS
 
-![macOS-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/macOS-Light.png)
+![macOS-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/macOS-Light.png)
 
-![macOS-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/macOS-Dark.png)
+![macOS-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/macOS-Dark.png)
 
 ### Ubuntu
 
-![Ubuntu-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Light.png)
+![Ubuntu-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Ubuntu-Light.png)
 
-![Ubuntu-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Dark.png)
+![Ubuntu-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Ubuntu-Dark.png)
 
 ## Install
 
 > Note: Due to better binary files compatibility on Windows platform, Windows users can skip this section and
 > download zip file in the [release](https://github.com/LorenEteval/Furious/releases) page that contains
 > pre-built binaries. Otherwise you need to follow the instructions below.
```

### Comparing `Furious-GUI-0.1.2/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.1.3/Furious_GUI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/LICENSE` & `Furious-GUI-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.1.2/PKG-INFO` & `Furious-GUI-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.1.2
+Version: 0.1.3
 Summary: A PyQt-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -46,29 +46,29 @@
 * Built-in user-friendly feature.
 * ...
 
 ## Sreenshot
 
 ### Windows
 
-![Windows-Light-EN](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Windows-Light-EN.png)
+![Windows-Light-EN](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Windows-Light-EN.png)
 
-![Windows-Light-CN](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Windows-Light-CN.png)
+![Windows-Light-CN](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Windows-Light-CN.png)
 
 ### macOS
 
-![macOS-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/macOS-Light.png)
+![macOS-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/macOS-Light.png)
 
-![macOS-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/macOS-Dark.png)
+![macOS-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/macOS-Dark.png)
 
 ### Ubuntu
 
-![Ubuntu-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Light.png)
+![Ubuntu-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Ubuntu-Light.png)
 
-![Ubuntu-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Dark.png)
+![Ubuntu-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Ubuntu-Dark.png)
 
 ## Install
 
 > Note: Due to better binary files compatibility on Windows platform, Windows users can skip this section and
 > download zip file in the [release](https://github.com/LorenEteval/Furious/releases) page that contains
 > pre-built binaries. Otherwise you need to follow the instructions below.
```

### Comparing `Furious-GUI-0.1.2/README.md` & `Furious-GUI-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 * Built-in user-friendly feature.
 * ...
 
 ## Sreenshot
 
 ### Windows
 
-![Windows-Light-EN](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Windows-Light-EN.png)
+![Windows-Light-EN](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Windows-Light-EN.png)
 
-![Windows-Light-CN](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Windows-Light-CN.png)
+![Windows-Light-CN](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Windows-Light-CN.png)
 
 ### macOS
 
-![macOS-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/macOS-Light.png)
+![macOS-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/macOS-Light.png)
 
-![macOS-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/macOS-Dark.png)
+![macOS-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/macOS-Dark.png)
 
 ### Ubuntu
 
-![Ubuntu-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Light.png)
+![Ubuntu-Light](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Ubuntu-Light.png)
 
-![Ubuntu-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/screenshot/Ubuntu-Dark.png)
+![Ubuntu-Dark](https://raw.githubusercontent.com/LorenEteval/Furious/main/Screenshot/Ubuntu-Dark.png)
 
 ## Install
 
 > Note: Due to better binary files compatibility on Windows platform, Windows users can skip this section and
 > download zip file in the [release](https://github.com/LorenEteval/Furious/releases) page that contains
 > pre-built binaries. Otherwise you need to follow the instructions below.
```

### Comparing `Furious-GUI-0.1.2/setup.py` & `Furious-GUI-0.1.3/setup.py`

 * *Files identical despite different names*

