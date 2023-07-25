# Comparing `tmp/raspisump-1.8.2.tar.gz` & `tmp/raspisump-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.8.2.tar", last modified: Tue Jul  4 19:20:47 2023, max compression
+gzip compressed data, was "raspisump-1.9.tar", last modified: Tue Jul 25 12:42:26 2023, max compression
```

## Comparing `raspisump-1.8.2.tar` & `raspisump-1.9.tar`

### file list

```diff
@@ -1,57 +1,63 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.939979 raspisump-1.8.2/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.8.2/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      284 2023-06-15 16:24:24.000000 raspisump-1.8.2/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3971 2023-07-04 19:20:47.939979 raspisump-1.8.2/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     3197 2023-06-15 16:24:24.000000 raspisump-1.8.2/README.md
--rw-r--r--   0 al        (1000) users      (984)       13 2023-07-04 19:19:39.000000 raspisump-1.8.2/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/bin/
--rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.8.2/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)      884 2023-07-04 19:19:39.000000 raspisump-1.8.2/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      638 2023-06-07 16:45:05.000000 raspisump-1.8.2/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      538 2023-06-07 16:45:05.000000 raspisump-1.8.2/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.8.2/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/csv/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     5937 2023-06-28 18:51:37.000000 raspisump-1.8.2/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.929979 raspisump-1.8.2/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.933313 raspisump-1.8.2/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.8.2/conf/web/css/includes.js
--rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      472 2023-06-15 16:24:24.000000 raspisump-1.8.2/conf/web/css/raspi.css
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.933313 raspisump-1.8.2/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.8.2/conf/web/images/logo.png
--rw-r--r--   0 al        (1000) users      (984)     2940 2023-06-15 16:24:24.000000 raspisump-1.8.2/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.933313 raspisump-1.8.2/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.8.2/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.8.2/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.933313 raspisump-1.8.2/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.8.2/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)    10745 2023-06-02 22:51:18.000000 raspisump-1.8.2/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.8.2/docs/install.pdf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.936646 raspisump-1.8.2/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.8.2/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     3781 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     2068 2023-06-02 22:51:18.000000 raspisump-1.8.2/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     2413 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/config_values.py
--rw-r--r--   0 al        (1000) users      (984)     1449 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     3543 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)      892 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2012 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     1864 2023-07-04 19:19:39.000000 raspisump-1.8.2/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.8.2/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.939979 raspisump-1.8.2/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3971 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      836 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       18 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-07-04 19:20:47.000000 raspisump-1.8.2/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-07-04 19:20:47.939979 raspisump-1.8.2/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2409 2023-07-04 19:19:39.000000 raspisump-1.8.2/setup.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-04 19:20:47.939979 raspisump-1.8.2/tests/
--rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.8.2/tests/tests_logging.py
--rw-r--r--   0 al        (1000) users      (984)     3904 2023-07-04 19:19:39.000000 raspisump-1.8.2/tests/tests_sump.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.501028 raspisump-1.9/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.9/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      407 2023-07-25 12:40:07.000000 raspisump-1.9/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3549 2023-07-25 12:42:26.501028 raspisump-1.9/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     2777 2023-07-25 12:40:07.000000 raspisump-1.9/README.md
+-rw-r--r--   0 al        (1000) users      (984)       11 2023-07-25 12:40:07.000000 raspisump-1.9/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.9/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)     1253 2023-07-25 12:40:07.000000 raspisump-1.9/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      719 2023-07-25 12:40:07.000000 raspisump-1.9/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      821 2023-07-25 12:40:07.000000 raspisump-1.9/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.9/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.9/conf/csv/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.9/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5756 2023-07-25 12:40:07.000000 raspisump-1.9/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.491028 raspisump-1.9/conf/systemd/
+-rw-r--r--   0 al        (1000) users      (984)      135 2023-07-25 12:40:07.000000 raspisump-1.9/conf/systemd/raspisump.service
+-rw-r--r--   0 al        (1000) users      (984)      137 2023-07-25 12:40:07.000000 raspisump-1.9/conf/systemd/rsumpwebchart.service
+-rw-r--r--   0 al        (1000) users      (984)      130 2023-07-25 12:40:07.000000 raspisump-1.9/conf/systemd/rsumpwebchart.timer
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.494361 raspisump-1.9/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.494361 raspisump-1.9/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)      379 2023-06-15 16:24:24.000000 raspisump-1.9/conf/web/css/includes.js
+-rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      526 2023-07-25 12:40:07.000000 raspisump-1.9/conf/web/css/raspi.css
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.494361 raspisump-1.9/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.9/conf/web/images/logo.png
+-rw-r--r--   0 al        (1000) users      (984)     3682 2023-07-25 12:40:07.000000 raspisump-1.9/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.494361 raspisump-1.9/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.9/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.9/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.497695 raspisump-1.9/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.9/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     8735 2023-07-25 12:40:07.000000 raspisump-1.9/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.9/docs/install.pdf
+-rw-r--r--   0 al        (1000) users      (984)     4397 2023-07-25 12:40:07.000000 raspisump-1.9/docs/upgrade_systemd.md
+-rw-r--r--   0 al        (1000) users      (984)     4937 2023-07-25 12:40:07.000000 raspisump-1.9/docs/upgrade_to_version_1.9.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.501028 raspisump-1.9/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.9/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     3781 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     1959 2023-07-25 12:40:07.000000 raspisump-1.9/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     2413 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/config_values.py
+-rw-r--r--   0 al        (1000) users      (984)     1449 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     3543 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      892 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2012 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     1864 2023-07-04 19:19:39.000000 raspisump-1.9/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.9/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.501028 raspisump-1.9/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3549 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      990 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       18 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-07-25 12:42:26.000000 raspisump-1.9/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-07-25 12:42:26.501028 raspisump-1.9/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2804 2023-07-25 12:40:07.000000 raspisump-1.9/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-07-25 12:42:26.501028 raspisump-1.9/tests/
+-rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.9/tests/tests_logging.py
+-rw-r--r--   0 al        (1000) users      (984)     3904 2023-07-04 19:19:39.000000 raspisump-1.9/tests/tests_sump.py
```

### Comparing `raspisump-1.8.2/LICENSE` & `raspisump-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/PKG-INFO` & `raspisump-1.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.8.2
+Version: 1.9
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,95 +15,70 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
-
-![MobileScreenshot](https://www.linuxnorth.org/raspi-sump/images/rsump_mobile.jpg)
+Raspi-sump is a sump pit water level monitoring system that uses a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
 
+![MobileScreenshot](https://www.linuxnorth.org/raspi-sump/images/rsump_mobile_1.9.jpg)
 
 Currently the system monitors the water level in your pit at defined intervals. It sends
 email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
 
 # What's New
 
+Version 1.9 - `Systemd` now replaces `rsumpmonitor.py`/`checkpid.py`. Control all Raspi-Sump services and Chart creation timers with `Systemd`.
+
 See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
 
 # Supported Versions of Raspbian / Raspberry Pi OS
 
 Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster)
 
 # Discord Group
 
 Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
 
-
-# Install Dependencies
-
-    sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
-
 # Install Raspi-Sump
 
-Pip installs default to Wheels which omits some folder setup in setup.py.
-Always use the '--no-binary :all:' option when installing or upgrading Raspi-Sump with pip.
-
-    sudo pip3 install --no-binary :all: raspisump
+Full install instructions are located at https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
+# Upgrade Raspi-Sump
 
-# Upgrading Raspi-Sump 
-
-Upgrading an existing version
+Upgrade an existing version
 
     sudo pip3 install -U --no-binary :all: raspisump
 
-This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
-
-
-Read the configuration docs copied during setup on your pi at the following location;
-
-    /home/username/raspi-sump/docs
-
-They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
-
-
-# Python2 (End of Life was January 1, 2020)
-
-Python2 installs of Raspi-Sump are no longer supported.
-
+If upgrading from version 1.8 or lower to version 1.9 see the [1.9 Upgrade Instructions](https://github.com/alaudet/raspi-sump/blob/master/docs/upgrade_to_version_1.9.md)
 
 # More Info
 
 Further details provided at https://www.linuxnorth.org/raspi-sump/
 
-An example hourly updating graph is available for view.
-https://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
-
 # Disclaimer
 
 You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
 
 This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
 
 Best practices should include:
 
-* A backup pump that triggers at a slightly higher water level than your main pump.
-* The secondary pump should be connected to a seperate dedicated electrical breaker. 
-* You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
-* if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you.  That would be the best approach with a backup pump for added protection.
+- A backup pump that triggers at a slightly higher water level than your main pump.
+- The secondary pump should be connected to a seperate dedicated electrical breaker.
+- You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
+- if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you. That would be the best approach with a backup pump for added protection.
 
 Once you have done all of these things, then consider using a monitoring system like Raspi-Sump.
 
 # License
 
-MIT License.  I want you to do whatever you want with Raspi-Sump.  If you
-improve it please let me know.
+Raspi-Sump is released under the [MIT License](https://github.com/alaudet/raspi-sump/blob/master/LICENSE).
 
-# Contributing
+# Contribute
 
 Please refer to the [Contributing Guidelines](https://github.com/alaudet/raspi-sump/blob/master/CONTRIBUTING.md) before issuing a pull request.
 
 # Donate
 
 [Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
```

### Comparing `raspisump-1.8.2/README.md` & `raspisump-1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,63 @@
-Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
-
-![MobileScreenshot](https://www.linuxnorth.org/raspi-sump/images/rsump_mobile.jpg)
+Raspi-sump is a sump pit water level monitoring system that uses a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
 
+![MobileScreenshot](https://www.linuxnorth.org/raspi-sump/images/rsump_mobile_1.9.jpg)
 
 Currently the system monitors the water level in your pit at defined intervals. It sends
 email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
 
 # What's New
 
+Version 1.9 - `Systemd` now replaces `rsumpmonitor.py`/`checkpid.py`. Control all Raspi-Sump services and Chart creation timers with `Systemd`.
+
 See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
 
 # Supported Versions of Raspbian / Raspberry Pi OS
 
 Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster)
 
 # Discord Group
 
 Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
 
-
-# Install Dependencies
-
-    sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
-
 # Install Raspi-Sump
 
-Pip installs default to Wheels which omits some folder setup in setup.py.
-Always use the '--no-binary :all:' option when installing or upgrading Raspi-Sump with pip.
-
-    sudo pip3 install --no-binary :all: raspisump
+Full install instructions are located at https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
+# Upgrade Raspi-Sump
 
-# Upgrading Raspi-Sump 
-
-Upgrading an existing version
+Upgrade an existing version
 
     sudo pip3 install -U --no-binary :all: raspisump
 
-This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
-
-
-Read the configuration docs copied during setup on your pi at the following location;
-
-    /home/username/raspi-sump/docs
-
-They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
-
-
-# Python2 (End of Life was January 1, 2020)
-
-Python2 installs of Raspi-Sump are no longer supported.
-
+If upgrading from version 1.8 or lower to version 1.9 see the [1.9 Upgrade Instructions](https://github.com/alaudet/raspi-sump/blob/master/docs/upgrade_to_version_1.9.md)
 
 # More Info
 
 Further details provided at https://www.linuxnorth.org/raspi-sump/
 
-An example hourly updating graph is available for view.
-https://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
-
 # Disclaimer
 
 You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
 
 This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
 
 Best practices should include:
 
-* A backup pump that triggers at a slightly higher water level than your main pump.
-* The secondary pump should be connected to a seperate dedicated electrical breaker. 
-* You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
-* if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you.  That would be the best approach with a backup pump for added protection.
+- A backup pump that triggers at a slightly higher water level than your main pump.
+- The secondary pump should be connected to a seperate dedicated electrical breaker.
+- You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
+- if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you. That would be the best approach with a backup pump for added protection.
 
 Once you have done all of these things, then consider using a monitoring system like Raspi-Sump.
 
 # License
 
-MIT License.  I want you to do whatever you want with Raspi-Sump.  If you
-improve it please let me know.
+Raspi-Sump is released under the [MIT License](https://github.com/alaudet/raspi-sump/blob/master/LICENSE).
 
-# Contributing
+# Contribute
 
 Please refer to the [Contributing Guidelines](https://github.com/alaudet/raspi-sump/blob/master/CONTRIBUTING.md) before issuing a pull request.
 
 # Donate
 
 [Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
```

### Comparing `raspisump-1.8.2/bin/rsumpchart.py` & `raspisump-1.9/bin/rsumpchart.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,8 +18,9 @@
     """Initiate todaychart.py module to graph sump pit activity."""
     csv_file = f"/home/{user}/raspi-sump/csv/waterlevel-{time.strftime('%Y%m%d')}.csv"
     filename = f"/home/{user}/raspi-sump/charts/today.png"
     todaychart.graph(csv_file, filename)
 
 
 if __name__ == "__main__":
+    print("Creating one time chart reading in the charts directory - today.png")
     main()
```

### Comparing `raspisump-1.8.2/bin/rsumpwebchart.py` & `raspisump-1.9/bin/rsumpwebchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/conf/raspisump.conf` & `raspisump-1.9/conf/raspisump.conf`

 * *Files 12% similar despite different names*

```diff
@@ -31,24 +31,21 @@
 
 # The pit_depth is the distance between the sensor and the bottom of the 
 # sump pit.
 # Like critical_water_level, enter centimeters for metric and inches for
 # imperial
 pit_depth = 72
 
-# rsump.py should be run with a cron job.  However cron is limited to
-# 1 minute as its minimum interval. If you need to monitor the sump level
-# more frequently you can set reading_interval to the desired time in seconds.
-# Default is 0 meaning only one reading will occur and the program will exit.
-# If set to 0 call the script with a cron job and select your interval there.
-# If setting to a value other than 0 you should run rsumpmonitor.py from a cron
-# job at a regularly interval to monitor the health of the rsump.py process.
-# rsumpmonitor.py is part of the raspisump software.  See documentation for
-# details.
-reading_interval = 0
+# Set the number of seconds between readings.
+# rsump.py is called from with systemd. See the install instructions (Systemd section).
+# If the rsump.py process fails for any reason systemd will restart the process
+# It is possible to take one reading only and have raspisump exit.  To do this make sure
+# you stop the raspisump.service and set the reading_interval to 0
+# When set to 0 raspisump takes one reading only and exits gracefully.
+reading_interval = 60
 
 # The temperature variable will adjust the speed of sound to reflect 
 # the normal temperature of your basement.  
 # If unit = metric then enter the temperature in Degrees Celcius.
 # If unit = imperial then enter the temperature in Degrees Fahrenheit.
 temperature = 20
```

### Comparing `raspisump-1.8.2/conf/web/images/logo.png` & `raspisump-1.9/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/conf/web/index.html` & `raspisump-1.9/conf/web/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 <!DOCTYPE html>
 <html>
+
 <head>
-    <title>Raspi-Sump Current Water Level</title>
-    <meta name="author" content="Al Audet" >
-    <meta charset="utf-8">
-    <meta name="viewport" content="width=device-width, initial-scale=1">
-    <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
-    <link rel="stylesheet" type="text/css" href="css/raspi.css">
-    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
-    <script src="css/includes.js"></script>
+  <title>Raspi-Sump Current Water Level</title>
+  <meta name="author" content="Al Audet">
+  <meta charset="utf-8">
+  <meta name="viewport" content="width=device-width, initial-scale=1">
+  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/css/bootstrap.min.css" rel="stylesheet"
+    integrity="sha384-uWxY/CJNBR+1zjPWmfnSnVxwRheevXITnMqoEIeG1LJrdI0GlVs/9cVSyPYXdcSF" crossorigin="anonymous">
+  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/js/bootstrap.bundle.min.js"
+    integrity="sha384-kQtW33rZJAHjgefvhyyzcGF3C5TFyBQBA13V1RKPf4uH+bwyzQxZ6CmMZHmNBEfJ"
+    crossorigin="anonymous"></script>
+  <link rel="stylesheet" type="text/css" href="css/raspi.css">
+  <script src="css/includes.js"></script>
 </head>
+
 <body>
-    <div class="container-fluid p-3 text-center topContainer">
-        <h1>Raspi-Sump</h1>
-        <p>Water Level Monitoring System</p> 
-      </div>
-    
-      <div class="container">
-        <div class="text-center">
-            <br><br>
-            
-            <div class="btn-group" role="group" aria-label="Button group">               
-                
-                <a href="charts/" class="btn btn-secondary">Historical Readings</a>
-            </div>
-            <div class="btn-group">    
-                <button type="button" class="btn btn-secondary dropdown-toggle" data-bs-toggle="dropdown">Raspi-Sump</button>
-                <ul class="dropdown-menu">
-                  <li><a class="dropdown-item" href="https://www.linuxnorth.org/raspi-sump/">Home</a></li>
-                  <li><a class="dropdown-item" href="https://www.linuxnorth.org/raspi-sump/faq.html">FAQ</a></li>
-                  <li><a class="dropdown-item" href="https://www.linuxnorth.org/raspi-sump/changelog.txt">Changelog</a></li>
-                  <li><a class="dropdown-item" href="https://www.linuxnorth.org/raspi-sump/license.html">License</a></li>
-                </ul>
-            </div>
-            <div class="btn-group">    
-                <button type="button" class="btn btn-secondary dropdown-toggle" data-bs-toggle="dropdown">Source Code</button>
-                <ul class="dropdown-menu">
-                  <li><a class="dropdown-item" href="https://github.com/alaudet/raspi-sump/">Raspi-Sump</a></li>
-                  <li><a class="dropdown-item" href="https://github.com/alaudet/hcsr04sensor/"">HCSR04Sensor</a></li>
-                </ul>
-            </div> 
-            <div class="btn-group" role="group" aria-label="Button group">               
-                
-                <a href="https://www.linuxnorth.org/donate/" class="btn btn-secondary">Donate</a>
-            </div>
-            
-        </div>
-        <div class="container pt-5">
-            <div class="text-center">
-            <img class="img-fluid" src="charts/today.png" alt="Today's Water Level" longdesc="Generated with Matplotlib">
-            </div>
+
+  <!-- begin navbar -->
+  <div class="container-fluid p-1 text-center topContainer">
+
+    <nav class="navbar p-3 navbar-expand-lg bg-body-tertiary navbar-dark">
+      <div class="container-fluid">
+        <a class="navbar-brand" href="#">Raspi-Sump</a>
+        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
+          aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
+          <span class="navbar-toggler-icon"></span>
+        </button>
+        <div class="collapse navbar-collapse" id="navbarSupportedContent">
+          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
+            <li class="nav-item">
+              <a class="nav-link" href="charts/">Historical Readings</a>
+            </li>
+            <li class="nav-item dropdown">
+              <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
+                aria-expanded="false">
+                Project
+              </a>
+              <ul class="dropdown-menu">
+                <li><a class="dropdown-item" href="https://www.linuxnorth.org/raspi-sump/">Home</a></li>
+                <li><a class="dropdown-item" href="https://www.linuxnorth.org/raspi-sump/faq.html">FAQ</a></li>
+                <li><a class="dropdown-item" href="https://www.linuxnorth.org/raspi-sump/changelog.txt">Changelog</a>
+                </li>
+                <li><a class="dropdown-item" href="https://www.linuxnorth.org/raspi-sump/license.html">License</a></li>
+              </ul>
+            </li>
+            <li class="nav-item dropdown">
+              <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown"
+                aria-expanded="false">
+                Source Code
+              </a>
+              <ul class="dropdown-menu">
+                <li><a class="dropdown-item" href="https://github.com/alaudet/raspi-sump/">Raspi-Sump</a></li>
+                <li><a class="dropdown-item" href="https://github.com/alaudet/hcsr04sensor/">HCSR04Sensor</a></li>
+              </ul>
+            </li>
+          </ul>
+          <a class="btn btn-secondary" href="https://www.linuxnorth.org/donate/" role="button">Donate</a>
         </div>
+      </div>
+    </nav>
+  </div>
+  <!-- end navbar -->
+
+  <div class="container-fluid p-0 text-center">
+    <p>Water Level Monitoring System</p>
+  </div>
+
+  <div class="container-fluid p-2">
+    <div class="text-center">
+      <img class="img-fluid" src="charts/today.png" alt="Today's Water Level" longdesc="Generated with Matplotlib">
     </div>
-    <div class="container-fluid p-0 bottomContainer">
-        <div id="VERSION"></div>
+  </div>
+
+  <!-- begin footer -->
+  <div class="container-fluid pt-3 p-1 text-center">
+    <div class="footer small p-1">
+      <div id="VERSION">
         <script>
-            fetchInclude("css/inc/VERSION", "VERSION");
+          fetchInclude("css/inc/VERSION", "VERSION");
         </script>
+      </div>
     </div>
+  </div>
+  <!-- end footer -->
+
 </body>
-</html>
+
+</html>
```

#### html2text {}

```diff
@@ -1,19 +1,17 @@
 
 
 
 
-****** Raspi-Sump ******
-Water Level Monitoring System
-
-
-Historical_Readings
 Raspi-Sump
-    * Home
-    * FAQ
-    * Changelog
-    * License
-Source Code
-    * Raspi-Sump
-    * >HCSR04Sensor
+    * Historical_Readings
+    * Project
+          o Home
+          o FAQ
+          o Changelog
+          o License
+    * Source_Code
+          o Raspi-Sump
+          o HCSR04Sensor
 Donate
+Water Level Monitoring System
 [Today's Water Level]
```

### Comparing `raspisump-1.8.2/docs/install.md` & `raspisump-1.9/docs/install.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,235 +1,182 @@
-Install
-=======
-Disclaimer: You could damage your raspberry pi if you do not insert a voltage divider between the echo pin on the sensor and the GPIO pin on the Raspberry Pi.
-If you choose to do this you do it at your own risk.
+# Raspi-Sump Installation Instructions
 
 Installation instructions assume Python3 on Raspberry Pi OS 11 (Bullseye) or Raspbian version 10 (Buster).
 
-Supported OS Versions
-=====================
+# Supported OS Versions
+
 Raspberry Pi OS 11 (Bullseye)
 
 Raspbian OS 10 (Buster)
 
-Raspbian OS 9 (Stretch) - Support ended on June 30, 2022.  Upgrade to Bullseye.
+Raspbian OS 9 (Stretch) - Support ended on June 30, 2022. Upgrade to Bullseye.
+
+# Hardware
+
+_Disclaimer: You could damage your raspberry pi if you do not insert a voltage divider between the echo pin on the sensor and the GPIO pin on the Raspberry Pi.
+If you choose to do this you do it at your own risk. Please make sure you understand GPIO information on your pi._
+
+Before installing Raspi-Sump you must setup your hardware.
+
+Use two resistors to create a voltage divider from the Sensor to the
+Pi. There are various combinations of resistors that you can use, a google
+search for Voltage Divider Calculator will allow you to calculate which
+combination you can use to bring the voltage down from the echo pin to 3.3V. I
+used a 470 Ohm and 1K Ohm resistor to bring the voltage down on the GPIO pin to
+3.4 which is within a tolerable 5% level. I could have also used a 1K and 2K resistor to give me 3.333V.
+
+Four wires connected as follows from the sensor to the pi (note, this will
+require some soldering). A floppy disk power connector fits nicely on the
+sensor. If you are just testing then a breadboard works great for quick and easy
+connections.
+
+- VCC pin to 5V pin on Pi (pin 2)
+
+- Ground pin to Ground on Pi (pin 6)
 
+- Trig pin to GPIO
 
-Install Dependencies
-====================
+- Echo pin to GPIO (need 470R resistor and 1K resistor to create a voltage divider.) In short, the 470 Ohm and 1K Ohm resistor are connected to one another with the Echo wire soldered between both of them to the GPIO pin. The other end of the 1K resistor is then soldered to the Ground wire.
 
-**Note**:  Your account must have sudo access to install Raspi-Sump.
+see https://www.linuxnorth.org/raspi-sump/ for information on pins I used and more details about the hardware setup.
+
+Google soldering resistors for good information on how to do this if you have never done it.
 
-Login to your Raspberry Pi running Raspberry Pi OS.
+# Install Dependencies
 
-Check that your user account is a member of the gpio group.  This is needed for accessing the gpio pins.
+**Note**: Your account must have sudo access to install Raspi-Sump.
+
+Now that your hardware is setup and properly connected to the gpio pins, login to your Raspberry Pi.
+
+Check that your user account is a member of the gpio group. This is needed for accessing the gpio pins.
 
     groups
 
-You should see all groups your account belongs to.  If gpio is not listed run the following command (where 'username' is your account name);
+You should see all groups your account belongs to. If gpio is not listed run the following command (where `username` is your account name);
 
-    sudo usermod -aG gpio username
+    sudo usermod -aG gpio `username`
 
 Logout and log back into your account for the groups to take effect.
 
 Install Pip, RPi.GPIO and Matplotlib
 
     sudo apt update && sudo apt -y upgrade
     sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
 
-RPi.GPIO is the library that controls the sensor.  
+RPi.GPIO is the library that controls the sensor.
 
 Matplotlib is used to generate charts.
 
-
 The Pip package manager is required to install Raspi-Sump in the next step.
 
-
-
-Install Raspi-Sump
-==================
+# Install Raspi-Sump
 
 The following will automatically install hcsr04sensor if it is not already installed on your Pi.
 
     sudo pip3 install --no-binary :all: raspisump
 
-
-Navigate to /home/username/raspi-sump/ and move the sample config file
+Navigate to /home/`username`/raspi-sump/ and move the sample config file
 to this directory.
 
-    cd /home/username/raspi-sump
+    cd /home/`username`/raspi-sump
     mv sample_config/raspisump.conf .
 
-The /home/username/raspi-sump folder is setup as follows on install;
-
-* raspi-sump/sample_config/raspisump.conf (all configurations for raspisump).
-* raspi-sump/csv (location of waterlevel readings to csv file)
-* raspi-sump/charts (location of charts if using rsumpchart.py)
-* raspi-sump/logs (location of rsumpmonitor.py logs if using raspisump as a continuous process)
-* raspi-sump/web (all files needed for the optional pi webserver install)
-* raspi-sump/cron (example crontab for scheduling readings)
+The /home/`username`/raspi-sump folder is setup as follows on install;
 
-
-**Note take care with your raspisump.conf file if you are using Gmail or any
-other mail system that requires authentication.  Your username and password
-will be viewable in the file. You should have a strong password on your account..  The installer also tightens file security on
+- raspi-sump/sample_config/raspisump.conf (all configurations for raspisump).
+- raspi-sump/csv (location of waterlevel readings to csv file)
+- raspi-sump/charts (location of charts if using rsumpchart.py)
+- raspi-sump/logs (location of rsumpmonitor.py logs if using raspisump as a continuous process)
+- raspi-sump/web (all files needed for the optional pi webserver install)
+- "depracated" raspi-sump/cron (example crontab for scheduling readings)
+
+  - NOTE that cron has been replaced with systemd.
+
+\*\*Note take care with your raspisump.conf file if you are using Gmail or any
+other mail system that requires authentication. Your `username` and password
+will be viewable in the file. You should have a strong password on your account.. The installer also tightens file security on
 the file automatically.
 
+# Edit raspisump.conf
 
-Edit raspisump.conf 
-====================
-
-All configurations are recorded in /home/username/raspi-sump/raspisump.conf
+All configurations are recorded in /home/`username`/raspi-sump/raspisump.conf
 
-See the configuration file for explanations of variables.  You can choose to
+See the configuration file for explanations of variables. You can choose to
 take imperial (inches) or metric (centimetres) water level readings.
 
+# Start Raspi-Sump with Systemd
 
-Hardware
-========
-
-Setup hardware (Please make sure you understand GPIO information on your pi).
-
-You must use two resistors to create a voltage divider from the Sensor to the
-Pi.  There are various combinations of resistors that you can use, a google
-search for Voltage Divider Calculator will allow you to calculate which
-combination you can use to bring the voltage down from the echo pin to 3.3V.  I
-used a 470 Ohm and 1K Ohm resistor to bring the voltage down on the GPIO pin to
-3.4 which is within a tolerable 5% level. I could have also used a 1K and 2K resistor to give me 3.333V. 
-
-
-Four wires connected as follows from the sensor to the pi (note, this will
-require some soldering).  A floppy disk power connector fits nicely on the
-sensor. If you are just testing then a breadboard works great for quick and easy
-connections. 
-
-1-VCC pin to 5V pin on Pi (pin 2)
-
-2-Ground pin to Ground on Pi (pin 6) 
-
-3-Trig pin to GPIO
-
-4-Echo pin to GPIO (need 470R resistor and 1K resistor to create a voltage divider.) In short, the 470 Ohm and 1K Ohm resistor are connected to one another with the Echo wire soldered between both of them to the GPIO pin.  The other end of the 1K resistor is then soldered to the Ground wire.
+To start Raspi-Sump you will need to enable it with systemd. The first time you install Raspi-Sump you will need to run this command for systemd to find the service files located in /home/`username`/.config/systemd/user
 
-see https://www.linuxnorth.org/raspi-sump/ for information on pins I used.
+    systemctl --user daemon-reload
 
-Google soldering resistors for good information on how to do this if you have never done it.
-
-
-Starting Raspi-Sump
-===================
-To start raspi-sump manually and take your first waterlevel reading issue the command;
-
-    rsump.py
-
-To run raspisump at 1 minute intervals enter the following line in crontab as follows;
-
-1 - crontab -e
-
-2 - enter line at the end of the crontab as follows;
-
-    */1 * * * * /usr/local/bin/rsump.py &> /dev/null
-
-
-3 - Save crontab
-
-(See cron documentation for questions on configuring crontab)
-
-
-1) To monitor the log file in the csv folder while raspi-sump is running;
-
-    e.g.   tail -f 'waterlevel-20230523.csv'
-
-If running as a continuous process 
-==================================
-
-There may be times where you want to run Raspi-Sump more than once every
-minute.  The default setting is 0 which will run rsump.py for one reading and
-then exit. This allows you to use the linux Cron scheduler to run at a specific
-interval.  Unfortunately cron allows one minute as its minimum interval.  
-
-To take readings at shorter intervals you can specify the amount of seconds
-between readings in the raspisump.conf file.
-
-1) set reading_interval in raspisump.conf to desired interval in seconds (e.g.
-reading_interval = 30).
+Start the raspisump service
 
-2) Add rsumpmonitor.py to crontab (see next section)
+    systemctl --user start raspisump
 
-3) To start Raspi-Sump on bootup add the following line at the end of /etc/rc.local just before the line 'exit 0'
+Configure raspisump to start after reboots
 
-    /usr/local/bin/rsump.py &
+    systemctl --user enable raspisump
 
-5) Reboot your Raspberry Pi or run the following command.  Your pi will run
-Raspi-Sump on boot from now on.
+To monitor the log file in the csv folder while raspi-sump is running;
 
-    rsump.py &
+    tail -f 'waterlevel-20230523.csv'
 
-Note*** Do not forget the ampersand '&' as this will run the script as a background process.
+## Extra systemd commands
 
-6) To stop Raspi-Sump:
+If you ever need to stop raspisump
 
-    sudo killall 09 rsump.py
+    systemctl --user stop raspisump
 
-7) To monitor the log file in the csv folder while raspi-sump is running;
+Prevent Raspi-Sump from running at boot time
 
-    e.g.    tail -f 'waterlevel-20230523.csv'
+    systemctl --user disable raspisump
 
-Health check with rsumpmonitor.py. If checking level more than once per minute only.
-================================================================================
+If you make a change to the raspisump.conf file, you must restart raspisump
 
-To check for the health of the rsump.py process run the rsumpmonitor.py script as
-root. 
-Add to pi user crontab as follows;
+    systemctl --user restart raspisump
 
-1 - crontab -e
+View the current status of the raspisump process
 
-2 - enter line at the end of the crontab as follows;
+    systemctl --user status raspisump
 
-    */5 * * * * /usr/local/bin/rsumpmonitor.py &> /dev/null
+# Generate Line Charts of Sump Activity
 
-3 - Save crontab
+You can automate the creation of charts at 15 minute intervals with systemd for later viewing on the pi webserver which will be configured later in this document. The first time it runs your webchart folder directory will be automatically created.
 
-This will check the rsump.py process every 5 minutes and restart it if it is stopped.
+    systemctl --user start rsumpwebchart.timer
+    systemctl --user enable rsumpwebchart.timer
 
+## Extra systemd commands
 
-Making Line Charts of Sump Activity
-===================================
+Prevent charts from being automatically created
 
-You can make a daily chart of sump pump activity by using rsumpchart.py.
+    systemctl --user stop rsumwebchart.timer
 
-1 - From the command line run;
+Prevent charts from being activated at boot time
 
-    rsumpchart.py
+    systemctl --user disable rsumpwebchart.timer
 
+View the current status of the chart timer
 
-This will create a line chart of sump pump activity.  You can easily modify the file to save to a different location with another name.
-Combined with a scheduled cron job it is an easy way to see the latest activity graphically.
+    systemctl --user status rsumpwebchart.timer
 
-**Note that this requires matplotlib on your RaspberryPi which can be
-installed with the apt command.  See the Install Dependencies section at the
-beginning of this file.
-
-You can also use the move_file.sh script provided as an example of how you
-transfer files offsite to a webserver or save historical chart information.
-
-Test Email Alerts
-=================
+# Test Email Alerts
 
 ### On Demand Email Test
 
 To test that emails are working run the command 'emailtest';
 
     emailtest
 
 ### Heartbeat Alerts
 
-Raspi-Sump can send email tests at predefined intervals.  See the raspisump.conf file option 'heartbeat' and 'heartbeat_interval'.
+Raspi-Sump can send email tests at predefined intervals. See the raspisump.conf file option 'heartbeat' and 'heartbeat_interval'.
 
-In /home/username/raspi-sump/raspisump.conf, this section configures the email heartbeat once per week.
+In /home/`username`/raspi-sump/raspisump.conf, this section configures the email heartbeat once per week.
 
     # Set a heartbeat sms or email interval in order to regularly test that your
     # notifications are working as intended.
     # 0 = No notifications
     # 1 = Send notifications
     heartbeat = 1
 
@@ -237,95 +184,62 @@
     # Values can be set to any number and are in minutes.
     # For reference;
     # daily   = 1439 minutes
     # weekly  = 10079 minutes
     # Monthly = 43199 minutes
     heartbeat_interval = 10079
 
-Optional - Setting Up a Local Web Server for easy Charts Viewing
-=================================================================
-
+# Set Up a Local Web Server for easy Charts Viewing
 
-Setting Up The Local Webserver on the Pi
+## Purpose
 
-Purpose
-=======
-
-The following instructions allow you to configure your raspberry pi to view graphs of sump pit activity through your web browser.  This is accomplished by configuring a local webserver on your pi.
+The following instructions allow you to configure your raspberry pi to view graphs of sump pit activity through your web browser. This is accomplished by configuring a local webserver on your pi.
 
 Once complete you will be able to view sump pump activity by connecting to
 http://ip_address_of_your_pi
 
-Preparation
-===========
+# Preparation
 
 If you have not done so in a while run the following command to update your Pi.
 This command updates repository information and then upgrades packages that are
-installed on your Pi.  If you did this already earlier in the instructions then
+installed on your Pi. If you did this already earlier in the instructions then
 it is not necessary to do again.
 
     sudo apt update && sudo apt -y upgrade
 
+# Getting Started
 
-Getting Started
-===============
-
-These instructions will do the following
-- install the Lighttpd webserver on your Pi
-- create your webcharts folder structure
-- configure cron to run the script to create for graphs of sump pump activity
-
+These instructions will install the Lighttpd webserver on your Pi
 
 Install the Lighttpd webserver on your
 Raspberry Pi as follows.
 
     sudo apt install lighttpd
 
-Create your first webcharts. This will create the needed folder under '/home/username/raspi-sump/charts/
-
-    rsumpwebchart.py
-
-    
-Change to the web server root folder at /var/www/html    
+Change to the web server root folder at /var/www/html
 
     cd /var/www/html
 
+Create the symlinks for your folders to be viewable with the web server. Replace `username` with your account name.
 
-Create the symlinks for your folders to be viewable with the web server. Replace 'username' with your account name.
-
-    sudo ln -s /home/username/raspi-sump/web/index.html index.html
-    sudo ln -s /home/username/raspi-sump/web/css css
-    sudo ln -s /home/username/raspi-sump/web/images images
-    sudo ln -s /home/username/raspi-sump/charts charts
-
+    sudo ln -s /home/`username`/raspi-sump/web/index.html index.html
+    sudo ln -s /home/`username`/raspi-sump/web/css css
+    sudo ln -s /home/`username`/raspi-sump/web/images images
+    sudo ln -s /home/`username`/raspi-sump/charts charts
 
 Enable directory listing for historical charts
 
     sudo lighttpd-enable-mod dir-listing
 
 Restart the web server
 
     sudo systemctl restart lighttpd
 
-
-Create a cron job to generate an hourly graph of your sump pit activity for viewing on your pi webserver.
-
-    1 - crontab -e
-
-    2 - enter line at the end of the crontab as follows;
-
-    59 * * * * /usr/local/bin/rsumpwebchart.py &> /dev/null
-
-    3 - Save crontab
-
-
-Open a web browser to http://ip_of_your_pi.  At the 59th minute of every hour
-you will create a chart of sump pit activity for the day which will be viewable
-on this page.  It will also copy historical information that you can access
+Open a web browser to http://ip_of_your_pi. Having configured the rsumpwebchart.timer earlier, a new webchart will be created every 15 minutes for viewing.
+This will also copy historical information that you can access
 from the link in the web page.
 
-Support
-==========
+# Support
 
-For support open an issue on the Github Issue Tracker or consider joining our discord server.  
+For support open an issue on the Github Issue Tracker or consider joining our discord server.
 
 For Discord simply send an email to alaudet@linuxnorth.org and request an invite link.
```

### Comparing `raspisump-1.8.2/docs/install.pdf` & `raspisump-1.9/docs/install.pdf`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/raspisump/alerts.py` & `raspisump-1.9/raspisump/alerts.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/raspisump/checkpid.py` & `raspisump-1.9/raspisump/checkpid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,61 @@
-'''Monitor the health of a process and restart it if it has stopped
-or if it has spawned multiple processes.'''
+"""Monitor the health of a process and restart it if it has stopped
+or if it has spawned multiple processes.
+
+This module is now deprecated in favour of systemd for restarting services."""
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import subprocess
 from raspisump import log
 
 
 def check_pid(process):
-    '''Check status of process.'''
-    cmdp1 = 'ps aux'
-    cmdp2 = 'grep -v grep'
-    cmdp3 = 'grep -v sudo'
-    cmdp4 = 'grep -c ' + process
-    cmdp1list = cmdp1.split(' ')
-    cmdp2list = cmdp2.split(' ')
-    cmdp3list = cmdp3.split(' ')
-    cmdp4list = cmdp4.split(' ')
+    """Check status of process."""
+    cmdp1 = "ps aux"
+    cmdp2 = "grep -v grep"
+    cmdp3 = "grep -v sudo"
+    cmdp4 = "grep -c " + process
+    cmdp1list = cmdp1.split(" ")
+    cmdp2list = cmdp2.split(" ")
+    cmdp3list = cmdp3.split(" ")
+    cmdp4list = cmdp4.split(" ")
     part1 = subprocess.Popen(cmdp1list, stdout=subprocess.PIPE)
-    part2 = subprocess.Popen(cmdp2list, stdin=part1.stdout,
-                             stdout=subprocess.PIPE
-                             )
+    part2 = subprocess.Popen(cmdp2list, stdin=part1.stdout, stdout=subprocess.PIPE)
     part1.stdout.close()
-    part3 = subprocess.Popen(cmdp3list, stdin=part2.stdout,
-                             stdout=subprocess.PIPE
-                             )
+    part3 = subprocess.Popen(cmdp3list, stdin=part2.stdout, stdout=subprocess.PIPE)
     part2.stdout.close()
-    part4 = subprocess.Popen(cmdp4list, stdin=part3.stdout,
-                             stdout=subprocess.PIPE
-                             )
+    part4 = subprocess.Popen(cmdp4list, stdin=part3.stdout, stdout=subprocess.PIPE)
     part3.stdout.close()
     number_of_processes = int(part4.communicate()[0])
     if number_of_processes == 0:
-        log.log_event('error_log',
-                      'ERROR - rsump.py process stopped, restarting')
+        log.log_event("error_log", "ERROR - rsump.py process stopped, restarting")
         restart(process)
     elif number_of_processes == 1:
         exit(0)
     else:
-        log.log_event('error_log',
-                      'ERROR - Multiple rsump.py processes...killing all and restarting')
+        log.log_event(
+            "error_log",
+            "ERROR - Multiple rsump.py processes...killing all and restarting",
+        )
         kill_start(process)
 
 
 def restart(process):
-    '''Restart process'''
-    restart_cmd = process + ' &'
-    restart_now = restart_cmd.split(' ')
+    """Restart process"""
+    restart_cmd = process + " &"
+    restart_now = restart_cmd.split(" ")
     subprocess.Popen(restart_now)
     exit(0)
 
 
 def kill_start(process):
-    '''Kill all instances of process and initiate restart.'''
-    kill_cmd = 'killall 09 ' + process
-    kill_it = kill_cmd.split(' ')
+    """Kill all instances of process and initiate restart."""
+    kill_cmd = "killall 09 " + process
+    kill_it = kill_cmd.split(" ")
     subprocess.call(kill_it)
     restart(process)
```

### Comparing `raspisump-1.8.2/raspisump/config_values.py` & `raspisump-1.9/raspisump/config_values.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/raspisump/emailtest.py` & `raspisump-1.9/raspisump/emailtest.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/raspisump/heartbeat.py` & `raspisump-1.9/raspisump/heartbeat.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/raspisump/log.py` & `raspisump-1.9/raspisump/log.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/raspisump/reading.py` & `raspisump-1.9/raspisump/reading.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/raspisump/todaychart.py` & `raspisump-1.9/raspisump/todaychart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/raspisump/webchart.py` & `raspisump-1.9/raspisump/webchart.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/raspisump.egg-info/PKG-INFO` & `raspisump-1.9/raspisump.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.8.2
+Version: 1.9
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,95 +15,70 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Raspi-sump is a sump pit water level monitoring system using a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
-
-![MobileScreenshot](https://www.linuxnorth.org/raspi-sump/images/rsump_mobile.jpg)
+Raspi-sump is a sump pit water level monitoring system that uses a Raspberry Pi and an Ultrasonic Sensor (HC-SR04).
 
+![MobileScreenshot](https://www.linuxnorth.org/raspi-sump/images/rsump_mobile_1.9.jpg)
 
 Currently the system monitors the water level in your pit at defined intervals. It sends
 email sms alerts if the water reaches a critical level, indicating a possible sump pump failure.
 
 # What's New
 
+Version 1.9 - `Systemd` now replaces `rsumpmonitor.py`/`checkpid.py`. Control all Raspi-Sump services and Chart creation timers with `Systemd`.
+
 See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
 
 # Supported Versions of Raspbian / Raspberry Pi OS
 
 Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster)
 
 # Discord Group
 
 Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
 
-
-# Install Dependencies
-
-    sudo apt install python3-pip python3-rpi.gpio python3-matplotlib
-
 # Install Raspi-Sump
 
-Pip installs default to Wheels which omits some folder setup in setup.py.
-Always use the '--no-binary :all:' option when installing or upgrading Raspi-Sump with pip.
-
-    sudo pip3 install --no-binary :all: raspisump
+Full install instructions are located at https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
+# Upgrade Raspi-Sump
 
-# Upgrading Raspi-Sump 
-
-Upgrading an existing version
+Upgrade an existing version
 
     sudo pip3 install -U --no-binary :all: raspisump
 
-This will also install the [HCSR04sensor](https://github.com/alaudet/hcsr04sensor) 
-
-
-Read the configuration docs copied during setup on your pi at the following location;
-
-    /home/username/raspi-sump/docs
-
-They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
-
-
-# Python2 (End of Life was January 1, 2020)
-
-Python2 installs of Raspi-Sump are no longer supported.
-
+If upgrading from version 1.8 or lower to version 1.9 see the [1.9 Upgrade Instructions](https://github.com/alaudet/raspi-sump/blob/master/docs/upgrade_to_version_1.9.md)
 
 # More Info
 
 Further details provided at https://www.linuxnorth.org/raspi-sump/
 
-An example hourly updating graph is available for view.
-https://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
-
 # Disclaimer
 
 You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
 
 This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
 
 Best practices should include:
 
-* A backup pump that triggers at a slightly higher water level than your main pump.
-* The secondary pump should be connected to a seperate dedicated electrical breaker. 
-* You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
-* if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you.  That would be the best approach with a backup pump for added protection.
+- A backup pump that triggers at a slightly higher water level than your main pump.
+- The secondary pump should be connected to a seperate dedicated electrical breaker.
+- You should also have a generator that can provide power should you have an extended outage during the spring or other unseasonally wet time of year.
+- if you are building a new home, pay attention to the grade of your property, as you may be able to let gravity empty your pit for you. That would be the best approach with a backup pump for added protection.
 
 Once you have done all of these things, then consider using a monitoring system like Raspi-Sump.
 
 # License
 
-MIT License.  I want you to do whatever you want with Raspi-Sump.  If you
-improve it please let me know.
+Raspi-Sump is released under the [MIT License](https://github.com/alaudet/raspi-sump/blob/master/LICENSE).
 
-# Contributing
+# Contribute
 
 Please refer to the [Contributing Guidelines](https://github.com/alaudet/raspi-sump/blob/master/CONTRIBUTING.md) before issuing a pull request.
 
 # Donate
 
 [Your Donation is Appreciated](https://www.linuxnorth.org/donate/)
```

### Comparing `raspisump-1.8.2/setup.py` & `raspisump-1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from setuptools import setup
 import os
 
-version = "1.8.2"
+version = "1.9"
 user = os.getlogin()
 
+
 homedir = "/home/" + user + "/raspi-sump/"
+systemd_configdir = "/home/" + user + "/.config/systemd/user/"
+
 
 if os.path.isfile(homedir + "raspisump.conf"):
     cmd = "cp -u " + homedir + "raspisump.conf " + homedir + "raspisump.conf.save"
     os.system(cmd)
 
+
 raspi_sump_files = [
     "bin/rsump.py",
     "bin/rsumpchart.py",
     "bin/rsumpmonitor.py",
     "bin/rsumpwebchart.py",
     "bin/emailtest",
 ]
@@ -30,14 +34,17 @@
     (homedir + "web", ["conf/web/index.html"]),
     (homedir + "web/images", ["conf/web/images/logo.png"]),
     (homedir + "web/css", ["conf/web/css/index.html"]),
     (homedir + "web/css", ["conf/web/css/raspi.css"]),
     (homedir + "web/css", ["conf/web/css/includes.js"]),
     (homedir, ["VERSION"]),
     (homedir + "web/css/inc", ["VERSION"]),
+    (systemd_configdir, ["conf/systemd/rsumpwebchart.service"]),
+    (systemd_configdir, ["conf/systemd/raspisump.service"]),
+    (systemd_configdir, ["conf/systemd/rsumpwebchart.timer"]),
 ]
 
 setup(
     name="raspisump",
     version=version,
     description="A sump pit monitoring system for Raspberry Pi",
     long_description_content_type="text/markdown",
@@ -67,7 +74,11 @@
 if os.path.isdir(homedir):
     cmd = "chown -R " + user + " " + homedir
     os.system(cmd)
     cmd = "chmod 600 " + homedir + "raspisump.conf"
     os.system(cmd)
     cmd = "chmod 600 " + homedir + "sample_config/raspisump.conf"
     os.system(cmd)
+
+if os.path.isdir("/home/" + user + "/.config/systemd"):
+    cmd = "chown -R " + user + " " + "/home/" + user + "/.config"
+    os.system(cmd)
```

### Comparing `raspisump-1.8.2/tests/tests_logging.py` & `raspisump-1.9/tests/tests_logging.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.8.2/tests/tests_sump.py` & `raspisump-1.9/tests/tests_sump.py`

 * *Files identical despite different names*

