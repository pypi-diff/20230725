# Comparing `tmp/inspursmsdk-2.1.0.tar.gz` & `tmp/inspursmsdk-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inspursmsdk-2.1.0.tar", last modified: Mon May 29 03:09:04 2023, max compression
+gzip compressed data, was "dist/inspursmsdk-2.1.1.tar", last modified: Tue Jul 25 09:31:32 2023, max compression
```

## Comparing `inspursmsdk-2.1.0.tar` & `inspursmsdk-2.1.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/
--rw-r--r--   0 root         (0) root         (0)      991 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      888 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspur_sm_sdk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/
--rw-r--r--   0 root         (0) root         (0)    49818 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/IpmiFunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
--rw-r--r--   0 root         (0) root         (0)    16391 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/commonInfoStr.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/eventLogString.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/sensorEventStr.py
--rw-r--r--   0 root         (0) root         (0)    51098 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
--rw-r--r--   0 root         (0) root         (0)     5698 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/showSensorDesc.py
--rw-r--r--   0 root         (0) root         (0)    21216 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/RedfishFunc.py
--rw-r--r--   0 root         (0) root         (0)   306808 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/RestFunc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12152 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/backup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/
--rw-r--r--   0 root         (0) root         (0)    44672 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/A7.xml
--rw-r--r--   0 root         (0) root         (0)    18131 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M4.xml
--rw-r--r--   0 root         (0) root         (0)    54444 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M5.xml
--rw-r--r--   0 root         (0) root         (0)    84520 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M6-N.xml
--rw-r--r--   0 root         (0) root         (0)    81800 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M6.xml
--rw-r--r--   0 root         (0) root         (0)    46175 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M7.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF3180A6.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF3280A6.xml
--rw-r--r--   0 root         (0) root         (0)   360127 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5180M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5280M5.xml
--rw-r--r--   0 root         (0) root         (0)    36922 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5468A5.xml
--rw-r--r--   0 root         (0) root         (0)    29961 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5488A5.xml
--rw-r--r--   0 root         (0) root         (0)   360290 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/SA5112M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/SA5212M5.xml
--rw-r--r--   0 root         (0) root         (0)    66019 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/command/restore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/
--rw-r--r--   0 root         (0) root         (0)     1613 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/NF5180M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/NF5280M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/SA5112M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/SA5212M5.yml
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/conf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/
--rw-r--r--   0 root         (0) root         (0)    44074 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/Base.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA5.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA6.py
--rw-r--r--   0 root         (0) root         (0)     6333 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA7.py
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA7_11308.py
--rw-r--r--   0 root         (0) root         (0)   744015 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM5.py
--rw-r--r--   0 root         (0) root         (0)   598814 2023-05-29 03:08:36.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6.py
--rw-r--r--   0 root         (0) root         (0)    17358 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6_41401.py
--rw-r--r--   0 root         (0) root         (0)    16476 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6_4140a.py
--rw-r--r--   0 root         (0) root         (0)   276843 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM7.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM7_13505.py
--rw-r--r--   0 root         (0) root         (0)    45791 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/I24M6.py
--rw-r--r--   0 root         (0) root         (0)     8475 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/IBase.py
--rw-r--r--   0 root         (0) root         (0)    14826 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5180M5.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5180M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    15217 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    59696 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5_435.py
--rw-r--r--   0 root         (0) root         (0)     2193 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5_436.py
--rw-r--r--   0 root         (0) root         (0)    47115 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/NS5160M6.py
--rw-r--r--   0 root         (0) root         (0)   120002 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/ResEntity.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/SA5212M5Impl.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:35.000000 inspursmsdk-2.1.0/inspur_sm_sdk/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/route/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/route/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3004 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/route/route.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/
--rw-r--r--   0 root         (0) root         (0)     4718 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/HostTypeJudge.py
--rw-r--r--   0 root         (0) root         (0)     4788 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/RedfishClient.py
--rw-r--r--   0 root         (0) root         (0)    10339 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/RegularCheckUtil.py
--rw-r--r--   0 root         (0) root         (0)     7686 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/RequestClient.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7550 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/configUtil.py
--rw-r--r--   0 root         (0) root         (0)     1812 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/fileUtil.py
--rw-r--r--   0 root         (0) root         (0)     7590 2023-05-29 03:08:34.000000 inspursmsdk-2.1.0/inspur_sm_sdk/util/parameterConversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      888 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2682 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 03:09:03.000000 inspursmsdk-2.1.0/inspursmsdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5216 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/ism.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 03:09:04.000000 inspursmsdk-2.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2023-05-29 03:08:37.000000 inspursmsdk-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)      991 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      888 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:24.000000 inspursmsdk-2.1.1/inspur_sm_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/
+-rw-r--r--   0 root         (0) root         (0)    49818 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/IpmiFunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    16391 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/commonInfoStr.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/eventLogString.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/sensorEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    51098 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/showSensorDesc.py
+-rw-r--r--   0 root         (0) root         (0)    21216 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/RedfishFunc.py
+-rw-r--r--   0 root         (0) root         (0)   299718 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/RestFunc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12152 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/backup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/
+-rw-r--r--   0 root         (0) root         (0)    44672 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/A7.xml
+-rw-r--r--   0 root         (0) root         (0)    18131 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M4.xml
+-rw-r--r--   0 root         (0) root         (0)    54444 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M5.xml
+-rw-r--r--   0 root         (0) root         (0)    84520 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M6-N.xml
+-rw-r--r--   0 root         (0) root         (0)    81800 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M6.xml
+-rw-r--r--   0 root         (0) root         (0)    46178 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M7.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2023-07-25 09:29:30.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF3180A6.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF3280A6.xml
+-rw-r--r--   0 root         (0) root         (0)   360127 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5180M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5280M5.xml
+-rw-r--r--   0 root         (0) root         (0)    36922 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5468A5.xml
+-rw-r--r--   0 root         (0) root         (0)    29961 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5488A5.xml
+-rw-r--r--   0 root         (0) root         (0)   360290 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/SA5112M5.xml
+-rw-r--r--   0 root         (0) root         (0)   360210 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/SA5212M5.xml
+-rw-r--r--   0 root         (0) root         (0)    66019 2023-07-25 09:29:29.000000 inspursmsdk-2.1.1/inspur_sm_sdk/command/restore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/NF5180M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/NF5280M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/SA5112M5.yml
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/SA5212M5.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/conf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)    44074 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/Base.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA5.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA6.py
+-rw-r--r--   0 root         (0) root         (0)     6333 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA7.py
+-rw-r--r--   0 root         (0) root         (0)      316 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA7_11308.py
+-rw-r--r--   0 root         (0) root         (0)   744015 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM5.py
+-rw-r--r--   0 root         (0) root         (0)   602520 2023-07-25 09:29:28.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6.py
+-rw-r--r--   0 root         (0) root         (0)    18029 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6_41401.py
+-rw-r--r--   0 root         (0) root         (0)    16476 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6_4140a.py
+-rw-r--r--   0 root         (0) root         (0)   288628 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM7.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM7_13505.py
+-rw-r--r--   0 root         (0) root         (0)    45791 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/I24M6.py
+-rw-r--r--   0 root         (0) root         (0)     8475 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/IBase.py
+-rw-r--r--   0 root         (0) root         (0)    14826 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5180M5.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5180M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    15217 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    59696 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5_435.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5_436.py
+-rw-r--r--   0 root         (0) root         (0)    47115 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/NS5160M6.py
+-rw-r--r--   0 root         (0) root         (0)   120116 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/ResEntity.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/SA5212M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:27.000000 inspursmsdk-2.1.1/inspur_sm_sdk/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/route/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/route/route.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/
+-rw-r--r--   0 root         (0) root         (0)     4718 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/HostTypeJudge.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/RedfishClient.py
+-rw-r--r--   0 root         (0) root         (0)    10339 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/RegularCheckUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/RequestClient.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 09:29:25.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7550 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/configUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/fileUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2023-07-25 09:29:26.000000 inspursmsdk-2.1.1/inspur_sm_sdk/util/parameterConversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      888 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/inspursmsdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/ism.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:31:32.000000 inspursmsdk-2.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-07-25 08:32:21.000000 inspursmsdk-2.1.1/setup.py
```

### Comparing `inspursmsdk-2.1.0/MANIFEST.in` & `inspursmsdk-2.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/PKG-INFO` & `inspursmsdk-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.1.0
+Version: 2.1.1
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/IpmiFunc.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/IpmiFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/biosPostEventStr.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/biosPostEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/commonInfoStr.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/commonInfoStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/eventLogString.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/eventLogString.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/sensorEventStr.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/sensorEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/M5Log/showSensorDesc.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/M5Log/showSensorDesc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/RedfishFunc.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/RedfishFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/RestFunc.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/RestFunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -6991,149 +6991,14 @@
             JSON['data'] = formatError("api/setallpolicy", response)
     except Exception as e:
         JSON['code'] = 1
         JSON['data'] = "exception into: " + str(e)
     return JSON
 
 
-# storage
-def getRaidCtrlInfo(client):
-    JSON = {}
-    URL = "api/raid/getraidCtrlInfo"
-    response = client.request("GET", URL, client.getHearder())
-    if response is None:
-        JSON['code'] = 1
-        JSON['data'] = 'Failed to call BMC interface [GET]' + URL + ', response is none'
-    elif response.status_code == 200:
-        result = response.json()
-        JSON['code'] = 0
-        JSON['data'] = result
-    else:
-        JSON['code'] = 1
-        JSON['data'] = formatError("[GET]" + URL, response)
-    return JSON
-
-
-def getPhysicalDiskInfo(client):
-    JSON = {}
-    URL = "api/raid/getphysicalDiskInfo"
-    response = client.request("GET", URL, client.getHearder())
-    if response is None:
-        JSON['code'] = 1
-        JSON['data'] = 'Failed to call BMC interface [GET]' + URL + ', response is none'
-    elif response.status_code == 200:
-        result = response.json()
-        JSON['code'] = 0
-        JSON['data'] = result
-    else:
-        JSON['code'] = 1
-        JSON['data'] = formatError("[GET]" + URL, response)
-    return JSON
-
-
-def getLogicalDiskInfo(client):
-    JSON = {}
-    URL = "api/raid/getlogicalDiskInfo"
-    response = client.request("GET", URL, client.getHearder())
-    if response is None:
-        JSON['code'] = 1
-        JSON['data'] = 'Failed to call BMC interface [GET]' + URL + ', response is none'
-    elif response.status_code == 200:
-        result = response.json()
-        JSON['code'] = 0
-        JSON['data'] = result
-    else:
-        JSON['code'] = 1
-        JSON['data'] = formatError("[GET]" + URL, response)
-    return JSON
-
-
-# EraseStop
-# EraseSimple
-# EraseNormal
-# EraseThrough
-def erasePhysicalDisk(client, ctrlId, diskid, option):
-    data = {
-        'ctrlId': ctrlId,
-        'deviceId': diskid,
-        'data': option
-    }
-    JSON = {}
-    header = client.getHearder()
-    # header["X-Requested-With"] = "XMLHttpRequest"
-    # header["Content-Type"] = "application/json;charset=UTF-8"
-    # header["Cookie"] = "" + header["Cookie"] + ";refresh_disable=1"
-    r = client.request("POST", "api/raid/erasePD", data=None, json=data, headers=header)
-    if r is None:
-        JSON["code"] = 1
-        JSON["data"] = 'Failed to call BMC interface api/raid/erasePD, response is none'
-    elif r.status_code == 200:
-        JSON["code"] = 0
-        JSON["data"] = "erase pysical disk success."
-    else:
-        JSON['code'] = 1
-        JSON['data'] = formatError("api/raid/erasePD", r)
-    return JSON
-
-
-def setPhysicalDisk(client, ctrlId, diskid, status):
-    data = {
-        'ctrlId': ctrlId,
-        'deviceId': diskid,
-        'data': status
-    }
-    JSON = {}
-    header = client.getHearder()
-    # header["X-Requested-With"] = "XMLHttpRequest"
-    # header["Content-Type"] = "application/json;charset=UTF-8"
-    # header["Cookie"] = "" + header["Cookie"] + ";refresh_disable=1"
-    r = client.request("POST", "api/raid/setPDState", data=None, json=data, headers=header)
-    if r is None:
-        JSON["code"] = 1
-        JSON["data"] = 'Failed to call BMC interface api/raid/setPDState, response is none'
-    elif r.status_code == 200:
-        JSON["code"] = 0
-        JSON["data"] = "set pysical disk success."
-    else:
-        JSON['code'] = 1
-        JSON['data'] = formatError("api/raid/setPDState", r)
-    return JSON
-
-
-def locateLogicalDisk(client, ctrlId, diskid, ledstate):
-    '''
-    locate disk
-    :param client:
-    :param ctrlId:
-    :param diskid:
-    :param ledstate:
-    :return:
-    '''
-    data = {
-        'ctrlId': ctrlId,
-        'deviceId': diskid,
-        'data': ledstate
-    }
-    JSON = {}
-    header = client.getHearder()
-    # header["X-Requested-With"] = "XMLHttpRequest"
-    # header["Content-Type"] = "application/json;charset=UTF-8"
-    # header["Cookie"] = "" + header["Cookie"] + ";refresh_disable=1"
-    r = client.request("POST", "api/raid/locateLD", data=None, json=data, headers=header)
-    if r is None:
-        JSON["code"] = 1
-        JSON["data"] = 'Failed to call BMC interface api/raid/locateLD, response is none'
-    elif r.status_code == 200:
-        JSON["code"] = 0
-        JSON["data"] = ledstate
-    else:
-        JSON['code'] = 1
-        JSON['data'] = formatError("api/raid/locateLD", r)
-    return JSON
-
 def locateLogicalDiskPMC(client, ctrlId, diskid, ledstate, duration):
     location_dict = {
         "StartLocate": 0,
         "StopLocate": 1
     }
     if ledstate == "StopLocate":
         duration = 1
@@ -7187,71 +7052,14 @@
         JSON["code"] = 0
         JSON["data"] = ledstate
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/raid/Locate_start_stop_LogicalDisk", r)
     return JSON
 
-# "StopInit"
-# "FastInit"
-# "SlowFullInit"
-def initLogicalDisk(client, ctrlId, diskid, ledstate):
-    '''
-    locate disk
-    :param client:
-    :param ctrlId:
-    :param diskid:
-    :param ledstate:
-    :return:
-    '''
-    data = {
-        'ctrlId': ctrlId,
-        'deviceId': diskid,
-        'data': ledstate
-    }
-    JSON = {}
-    header = client.getHearder()
-    # header["X-Requested-With"] = "XMLHttpRequest"
-    # header["Content-Type"] = "application/json;charset=UTF-8"
-    # header["Cookie"] = "" + header["Cookie"] + ";refresh_disable=1"
-    r = client.request("POST", "api/raid/initLD", data=None, json=data, headers=header)
-    if r is None:
-        JSON["code"] = 1
-        JSON["data"] = 'Failed to call BMC interface api/raid/initLD, response is none'
-    elif r.status_code == 200:
-        JSON["code"] = 0
-        JSON["data"] = ledstate
-    else:
-        JSON['code'] = 1
-        JSON['data'] = formatError("api/raid/initLD", r)
-    return JSON
-
-
-def deleteLogicalDisk(client, ctrlId, diskid):
-    data = {
-        'ctrlId': ctrlId,
-        'deviceId': diskid
-    }
-    JSON = {}
-    header = client.getHearder()
-    # header["X-Requested-With"] = "XMLHttpRequest"
-    # header["Content-Type"] = "application/json;charset=UTF-8"
-    # header["Cookie"] = "" + header["Cookie"] + ";refresh_disable=1"
-    r = client.request("POST", "api/raid/deleteLD", data=None, json=data, headers=header)
-    if r is None:
-        JSON["code"] = 1
-        JSON["data"] = 'Failed to call BMC interface api/raid/deleteLD, response is none'
-    elif r.status_code == 200:
-        JSON["code"] = 0
-        JSON["data"] = ""
-    else:
-        JSON['code'] = 1
-        JSON['data'] = formatError("api/raid/deleteLD", r)
-    return JSON
-
 
 def deleteLogicalDiskPMC(client, ctrlId, diskid):
     data = {
         'ctrlId': ctrlId,
         'deviceId': diskid,
         'vendor_type': 1
     }
@@ -7291,73 +7099,51 @@
         JSON["data"] = ""
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/raid/Delete_LogicalDisk", r)
     return JSON
 
 
-def setRaidCtrlProperties(client, ctrlId, jbod, smartEr):
-    data = {
-        'ctrlId': ctrlId,
-        'JBOD': jbod,
-        'smartEr': smartEr
-    }
+def createMVVirtualDrive(client, data):
     JSON = {}
     header = client.getHearder()
-    # header["X-Requested-With"] = "XMLHttpRequest"
-    # header["Content-Type"] = "application/json;charset=UTF-8"
-    # header["Cookie"] = "" + header["Cookie"] + ";refresh_disable=1"
-    r = client.request("POST", "api/raid/setRaidCtrlProperties", data=None, json=data, headers=header)
+    r = client.request("POST", "api/raid/setMVVDAdd", data=None, json=data, headers=header)
     if r is None:
         JSON["code"] = 1
-        JSON["data"] = 'Failed to call BMC interface api/raid/setRaidCtrlProperties, response is none'
+        JSON[
+            "data"] = 'Failed to call BMC interface api/raid/setMVVDAdd, response is none'
     elif r.status_code == 200:
         JSON["code"] = 0
         JSON["data"] = ""
     else:
         JSON['code'] = 1
-        JSON['data'] = formatError("api/raid/setRaidCtrlProperties", r)
+        JSON['data'] = formatError("api/raid/setMVVDAdd", r)
     return JSON
 
 
-def addLogicalDisk(client, data):
+def deleteMVLogicalDisk(client, ctrlId, diskid):
+    data = {
+        'ctrlId': ctrlId,
+        'deviceId': diskid
+    }
     JSON = {}
-    # print(data)
     header = client.getHearder()
     # header["X-Requested-With"] = "XMLHttpRequest"
     # header["Content-Type"] = "application/json;charset=UTF-8"
     # header["Cookie"] = "" + header["Cookie"] + ";refresh_disable=1"
-    r = client.request("POST", "api/raid/addLogicalDisk", data=None, json=data, headers=header)
-    if r is None:
-        JSON["code"] = 1
-        JSON["data"] = 'Failed to call BMC interface api/raid/addLogicalDisk, response is none'
-    elif r.status_code == 200:
-        JSON["code"] = 0
-        JSON["data"] = ""
-    else:
-        JSON['code'] = 1
-        JSON['data'] = formatError("api/raid/addLogicalDisk", r)
-    return JSON
-
-
-def createVirtualDrive(client, data):
-    JSON = {}
-    header = client.getHearder()
-    r = client.request("PUT", "api/settings/raid_management/create_virtual_drive", data=None, json=data,
-                       headers=header, timeout=600)
+    r = client.request("POST", "api/raid/setMVVDDel", data=None, json=data, headers=header)
     if r is None:
         JSON["code"] = 1
-        JSON[
-            "data"] = 'Failed to call BMC interface api/settings/raid_management/create_virtual_drive, response is none'
+        JSON["data"] = 'Failed to call BMC interface api/raid/deleteLD, response is none'
     elif r.status_code == 200:
         JSON["code"] = 0
         JSON["data"] = ""
     else:
         JSON['code'] = 1
-        JSON['data'] = formatError("api/settings/raid_management/create_virtual_drive", r)
+        JSON['data'] = formatError("api/raid/deleteLD", r)
     return JSON
 
 
 def createVirtualDrive_41401(client, data):
     JSON = {}
     header = client.getHearder()
     r = client.request("PUT", "api/raid/Create_LogicalDisk", data=None, json=data,
@@ -7396,14 +7182,15 @@
         JSON['code'] = 0
         JSON['data'] = {"Swtich_Mode": "disable"}
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/ncsi-interfaces-normal", response)
     return JSON
 
+
 # {"NIC_Name":"OCP","Swtich_Mode":"AutoFailover","Port_Status":0}
 # {"NIC_Name": "OCP", "Swtich_Mode": "AutoFailover", "Port_Status": 0 }
 # {"NIC_Name":"PCIE","Swtich_Mode":"Manual","Port_Status":3}
 # {"NIC_Name": "PCIE", "Swtich_Mode": "Manual", "Port_Status": 3 }
 def setNCSI4jd(client, mode, nicname, portstatus):
     data = {
         "NIC_Name": nicname,
```

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/backup.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/backup.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/A7.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/A7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M4.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M4.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M5.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M6-N.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M6-N.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M6.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M7.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M7.xml`

 * *Files identical despite different names*

#### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/M7.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/M7.xml`

```diff
@@ -256,15 +256,15 @@
     </cfgItem>
     <cfgItem>
       <name>
         <description>VT-d</description>
         <belongto>Processor</belongto>
         <location>Socket Configuration-IIO Configuration-Intel VT for Directed I/O (VT-d)</location>
       </name>
-      <parent>SocketIioConfig</parent>
+      <parent>SocketMpLinkConfig</parent>
       <getter>VTdSupport</getter>
       <conditions>
         <condition>
           <key>PowerProfile</key>
           <value>CUSTOM</value>
         </condition>
       </conditions>
```

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF3180A6.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF3180A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF3280A6.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF3280A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5180M5.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5180M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5280M5.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5280M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5468A5.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5468A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/NF5488A5.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/NF5488A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/SA5112M5.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/SA5112M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/bios/SA5212M5.xml` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/bios/SA5212M5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/command/restore.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/command/restore.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/conf/NF5180M5.yml` & `inspursmsdk-2.1.1/inspur_sm_sdk/conf/NF5180M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/conf/NF5280M5.yml` & `inspursmsdk-2.1.1/inspur_sm_sdk/conf/NF5280M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/conf/SA5112M5.yml` & `inspursmsdk-2.1.1/inspur_sm_sdk/conf/SA5112M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/conf/SA5212M5.yml` & `inspursmsdk-2.1.1/inspur_sm_sdk/conf/SA5212M5.yml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/Base.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/Base.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA5.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA6.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonA7.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonA7.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM5.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6.py`

 * *Files 1% similar despite different names*

```diff
@@ -6088,22 +6088,46 @@
                             float(temp) if (
                                 temp is not None and temp != 'na') else None)
                     else:
                         cpu_singe.Temperature(None)
                     cpu_singe.EnabledSetting(True)
                     cpu_singe.ProcessorType('CPU')
                     cpu_singe.ProcessorArchitecture('x86')
-                    cpu_singe.InstructionSet('x86-64')
-                    cpu_singe.MaxSpeedMHz(cpu.get('proc_speed', None))
+                    instructionSet = 'x86-64'
+                    if 'InstructionSet' in cpu:
+                        #M6 新版本
+                        instructionSet = cpu.get('InstructionSet')
+                    elif 'instruct_set' in cpu:
+                        #M7
+                        instructionSet = cpu.get('instruct_set')
+                    cpu_singe.InstructionSet(instructionSet)
+                    cpu_singe.ProSpeedMHz(cpu.get('proc_speed', None))
+
+                    maxspeed = None
+                    if 'MaxSpeedMHz' in cpu:
+                        #M6 新版本
+                        maxspeed = cpu.get('MaxSpeedMHz')
+                    elif 'max_speed' in cpu:
+                        #M7
+                        maxspeed = cpu.get('max_speed')
+                    cpu_singe.MaxSpeedMHz(maxspeed)
                     cpu_singe.TotalCores(cpu.get('proc_used_core_count', None))
                     cpu_singe.TotalThreads(cpu.get('proc_thread_count', None))
                     cpu_singe.Socket(cpu.get('proc_id', 0))
                     cpu_singe.PROCID(cpu.get('PROC_ID', None))
                     cpu_singe.PPIN(cpu.get('ppin', None))
                     cpu_singe.TDP(cpu.get('proc_tdp'))
+                    mc = None
+                    if 'micro_code' in cpu:
+                        #M6 新版本
+                        mc = cpu.get('micro_code')
+                    elif 'micro_code_ver' in cpu:
+                        #M7
+                        mc = cpu.get('micro_code_ver')
+                    cpu_singe.MicroCode(mc)
                     cpu_singe.State('Enabled')
                     cpu_singe.Health(cpu.get('status', None))
                 else:
                     cpu_singe.CommonName('CPU' + str(cpu.get('proc_id')))
                     cpu_singe.Location('mainboard')
                     cpu_singe.State('Absent')
 
@@ -6145,19 +6169,18 @@
         # get
         res = RestFunc.getMemoryInfoByRest(client)
         if res == {}:
             result.State('Failure')
             result.Message(['get memory info failed'])
         elif res.get('code') == 0 and res.get('data') is not None:
             overalhealth = RestFunc.getHealthSummaryByRest(client)
-            if overalhealth.get('code') == 0 and overalhealth.get(
-                    'data') is not None and 'memory' in overalhealth.get('data'):
-                if overalhealth.get('code') == 0 and overalhealth.get(
-                        'data') is not None and 'memory' in overalhealth.get(
-                        'data'):
+            if overalhealth.get('code') == 0 and overalhealth.get('data') is not None and \
+                    'memory' in overalhealth.get('data'):
+                if overalhealth.get('code') == 0 and overalhealth.get('data') is not None and \
+                        'memory' in overalhealth.get('data'):
                     if overalhealth.get('data').get('memory') == 'na':
                         memory_Info.OverallHealth('Absent')
                     elif overalhealth.get('data').get('memory').lower() == 'info':
                         memory_Info.OverallHealth('OK')
                     else:
                         memory_Info.OverallHealth(
                             overalhealth.get('data').get('memory').capitalize())
@@ -6217,14 +6240,20 @@
                         memory.get('mem_data_width', None))
                     memory_singe.RankCount(memory.get('mem_mod_ranks', None))
                     if 'mem_mod_part_num' in memory:
                         memory_singe.PartNumber(
                             memory.get('mem_mod_part_num').strip())
                     else:
                         memory_singe.PartNumber(None)
+                    if 'mem_base_module' in memory:
+                        # M7
+                        memory_singe.BaseModule(memory.get('mem_base_module', None))
+                    elif 'mem_mod_BaseModuleType' in memory:
+                        # M6新版本
+                        memory_singe.BaseModule(memory.get('mem_mod_BaseModuleType', None))
                     memory_singe.Technology(
                         memory.get('mem_mod_technology', None))
                     memory_singe.MinVoltageMillivolt(
                         memory.get('mem_mod_min_volt', None))
                     if 'mem_mod_size' in memory:
                         memoryGiB = memoryGiB + memory.get('mem_mod_size')
                     else:
@@ -6235,22 +6264,19 @@
                     elif 'mem_mod_status' in memory:
                         memory_singe.Health(
                             'OK' if int(
                                 memory.get('mem_mod_status')) == 1 else None)
                     else:
                         memory_singe.Health(None)
                 else:
-                    if memory.get(
-                        'mem_mod_slot',
-                            None) is None and 'mem_mod_cpu_num' in memory and 'mem_riser_num' in memory and 'mem_mod_socket_num' in memory:
-                        name = 'DIMM' + '{0}{1}{2}'.format(
-                            memory.get(
-                                'mem_mod_cpu_num', 0), memory.get(
-                                'mem_riser_num', 0), memory.get(
-                                'mem_mod_socket_num', 0))
+                    if memory.get('mem_mod_slot', None) is None and 'mem_mod_cpu_num' in memory and \
+                            'mem_riser_num' in memory and 'mem_mod_socket_num' in memory:
+                        name = 'DIMM' + '{0}{1}{2}'.format(memory.get('mem_mod_cpu_num', 0),
+                                                           memory.get('mem_riser_num', 0),
+                                                           memory.get('mem_mod_socket_num', 0))
                     else:
                         name = memory.get('mem_mod_slot', None)
                     memory_singe.CommonName(name)
                     memory_singe.Location('mainboard')
                     memory_singe.State('Absent')
 
                 list.append(memory_singe.dict)
@@ -8811,14 +8837,15 @@
             if (data['ntp_auto_date'] != "manual"):
                 res['1stNTP'] = data.get('primary_ntp', None)
                 res['2ndNTP'] = data.get('secondary_ntp', None)
                 res['3rdNTP'] = data.get('third_ntp', None)
                 res['4thNTP'] = data.get('fourth_ntp', None)
                 res['5thNTP'] = data.get('fifth_ntp', None)
                 res['6thNTP'] = data.get('sixth_ntp', None)
+                res['NTPSYNCycle'] = data.get('sync_cycle_ntp', None)
             else:
                 if data['ntp_dhcp4_date'] == 'enable':
                     res['DateAutoSyn'] = 'dhcp4'
                 elif data['ntp_dhcp6_date'] == 'enable':
                     res['DateAutoSyn'] = 'dhcp6'
                 else:
                     res['DateAutoSyn'] = data['ntp_auto_date']
@@ -8880,16 +8907,16 @@
             default_NTP_timestamp = data.get('timestamp', "")
             default_NTP_server1 = data.get('primary_ntp', "")
             default_NTP_server2 = data.get('secondary_ntp', "")
             default_NTP_server3 = data.get('third_ntp', "")
             default_NTP_server4 = data.get('fourth_ntp', "")
             default_NTP_server5 = data.get('fifth_ntp', "")
             default_NTP_server6 = data.get('sixth_ntp', "")
-            default_NTP_dhcp4 = data['ntp_dhcp4_date']
-            default_NTP_dhcp6 = data['ntp_dhcp6_date']
+            default_NTP_dhcp4 = data['ntp_dhcp4_date', ""]
+            default_NTP_dhcp6 = data['ntp_dhcp6_date', ""]
         else:
             timeinfo.State("Failure")
             timeinfo.Message(["get bmc time error"])
             RestFunc.logout(client)
             return timeinfo
 
         sync_res = RestFunc.getSynctimeByRest(client)
@@ -11841,24 +11868,27 @@
 
 def createVirtualDrive(client, args):
     result = ResultBean()
     ctrl_id_name_dict = {}
     ctrl_id_list = []
     ctrl_type_dict = {
         "LSI": [],
-        "PMC": []
+        "PMC": [],
+        "MV": []
     }
     res = RestFunc.getRaidCtrlInfo(client)
     if res.get('code') == 0 and res.get('data') is not None:
         ctrls = res.get('data')
         for ctrl in ctrls:
             if str(ctrl.get("RaidType")).upper() == "PMC":
                 ctrl_type_dict['PMC'].append(ctrl["Name"])
             elif str(ctrl.get("RaidType")).upper() == "LSI":
                 ctrl_type_dict['LSI'].append(ctrl["Name"])
+            elif str(ctrl.get("RaidType")).upper() == "MV":
+                ctrl_type_dict['MV'].append(ctrl["Name"])
             if "Index" in ctrl.keys():
                 ctrl_id_name_dict[ctrl["Index"]] = ctrl["Name"]
                 ctrl_id_list.append(str(ctrl["Index"]))
             elif "id" in ctrl.keys():
                 ctrl_id_name_dict[ctrl["id"]] = ctrl["Name"]
                 ctrl_id_list.append(str(ctrl["id"]))
     else:
@@ -11874,15 +11904,15 @@
     pds = {}
     res = RestFunc.getPhysicalDiskInfo(client)
     if res.get('code') == 0 and res.get('data') is not None:
         pds = res.get('data')
         for pd in pds:
             if pd['ControllerName'] not in ctrl_list_dict:
                 ctrl_list_dict[pd['ControllerName']] = []
-            ctrl_list_dict[pd['ControllerName']].append(pd['DeviceID'])
+            ctrl_list_dict[pd['ControllerName']].append(pd.get('DeviceID', pd.get('slotNum')))
     else:
         result.State("Failure")
         result.Message(['get physical disk information failed!' + res.get('data')])
         return result
     if args.Info is not None:
         for pd in ctrl_list_dict:
             ctrl_list_dict.get(pd).sort()
@@ -11890,41 +11920,43 @@
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             if str(ctrl_id_name_dict.get(ctrlid)) in ctrl_type_dict.get('LSI'):
                 raidDict['Controller Type'] = "LSI"
-            else:
+            elif str(ctrl_id_name_dict.get(ctrlid)) in ctrl_type_dict.get('PMC'):
                 raidDict['Controller Type'] = "PMC"
+            elif str(ctrl_id_name_dict.get(ctrlid)) in ctrl_type_dict.get('MV'):
+                raidDict['Controller Type'] = "MV"
             pdiskList = []
             for pd in pds:
                 if pd.get("ControllerName") == ctrl_id_name_dict.get(ctrlid):
                     LSI_flag = True
                     pdiskDict = collections.OrderedDict()
-                    pdiskDict['Slot Number'] = pd.get("SlotNum")
+                    pdiskDict['Slot Number'] = pd.get("SlotNum", pd.get("slotNum"))
                     pdiskDict['Drive Name'] = pd.get("Name")
                     if "InterfaceType" in pd:
                         pdiskDict['Interface'] = pd.get("InterfaceType")
                     elif "interface_type" in pd:
                         pdiskDict['Interface'] = pd.get("interface_type")
                     else:
                         pdiskDict['Interface'] = None
                     if "MediaType" in pd:
-                        pdiskDict['Media Type'] = pd.get("MediaType")
+                        pdiskDict['Media Type'] = pd.get("MediaType",)
                     elif "type" in pd:
                         pdiskDict['Media Type'] = pd.get("type")
                     else:
-                        pdiskDict['Media Type'] = None
+                        pdiskDict['Media Type'] = pd.get("mediaType")
                     if "NONCoercedSize" in pd:
                         pdiskDict['Capacity'] = pd.get("NONCoercedSize")
                     elif "size" in pd:
                         pdiskDict['Capacity'] = pd.get("size")
                     else:
-                        pdiskDict['Capacity'] = None
+                        pdiskDict['Capacity'] = pd.get("cap")
                     if "FWState" in pd:
                         pdiskDict['Firmware State'] = pd.get("FWState")
                     else:
                         pdiskDict['Firmware State'] = None
                     if "array_number" in pd:
                         pdiskDict['Array Number'] = pd.get("array_number")
                     else:
@@ -11943,14 +11975,16 @@
         result.State('Failure')
         result.Message(["Please input ctrlId parameter!"])
         return result
     elif str(ctrl_id_name_dict.get(args.ctrlId)) in ctrl_type_dict.get('LSI'):
         result = addLogicalDisk(client, args, pds, ctrl_id_name_dict)
     elif str(ctrl_id_name_dict.get(args.ctrlId)) in ctrl_type_dict.get('PMC'):
         result = addPMCLogicalDisk(client, args, pds, ctrl_id_name_dict)
+    elif str(ctrl_id_name_dict.get(args.ctrlId)) in ctrl_type_dict.get('MV'):
+        result = addMVLogicalDisk(client, args)
     else:
         result.State('Failure')
         result.Message(["No raid controller!"])
     return result
 
 
 def addLogicalDisk(client, args, pds, ctrl_id_name_dict):
@@ -12072,15 +12106,15 @@
         "accessPolicy": args.access,
         "readPolicy": args.r,
         "writePolicy": args.w,
         "cachePolicy": args.cache,
         "ioPolicy": args.io,
         "initState": args.init,
         "spanDepth": args.spanDepth,
-                "raidname": args.vname
+        "raidname": args.vname
     }
     for i in range(len(pd_dev_list)):
         data["pdDeviceIndex" + str(i)] = pd_dev_list[i]
 
     res = RestFunc.addLogicalDisk(client, data)
     if res == {}:
         result.State("Failure")
@@ -12163,30 +12197,67 @@
         result.Message(['create virtual drive successful.'])
     else:
         result.State("Failure")
         result.Message(['create virtual drive failed, ' + str(res.get('data'))])
     return result
 
 
+def addMVLogicalDisk(client, args):
+    result = ResultBean()
+    if args.size is None:
+        result.State('Failure')
+        result.Message(['some parameters are missing'])
+        return result
+
+    if args.vname is None:
+        args.vname = "logicName1"
+
+    stripsize_dict_mv = {0: 0, 1: 1}
+    args.size = stripsize_dict_mv.get(args.size, 0)
+    data = {
+        "ctrlId": args.ctrlId,
+        "numPD": 2,
+        "pd_deviceIndex0": 0,
+        "pd_deviceIndex1": 1,
+        "raidLevel": "1",
+        "stripSize": args.size,
+        "VDName": args.vname
+    }
+    res = RestFunc.createMVVirtualDrive(client, data)
+    if res == {}:
+        result.State("Failure")
+        result.Message(["create virtual drive failed"])
+    elif res.get('code') == 0 and res.get('data') is not None:
+        result.State('Success')
+        result.Message(['create virtual drive successful.'])
+    else:
+        result.State("Failure")
+        result.Message(['create virtual drive failed, ' + str(res.get('data'))])
+    return result
+
+
 def setVirtualDrive(client, args):
     result = ResultBean()
     ctrl_id_name_dict = {}
     ctrl_type_dict = {
         "LSI": [],
-        "PMC": []
+        "PMC": [],
+        "MV": []
     }
     ctrl_id_list = []
     res = RestFunc.getRaidCtrlInfo(client)
     if res.get('code') == 0 and res.get('data') is not None:
         ctrls = res.get('data')
         for ctrl in ctrls:
             if str(ctrl.get("RaidType")).upper() == "PMC":
                 ctrl_type_dict['PMC'].append(ctrl["Name"])
-            else:
+            elif str(ctrl.get("RaidType")).upper() == "LSI":
                 ctrl_type_dict['LSI'].append(ctrl["Name"])
+            elif str(ctrl.get("RaidType")).upper() == "MV":
+                ctrl_type_dict['MV'].append(ctrl["Name"])
             if "Index" in ctrl.keys():
                 ctrl_id_name_dict[ctrl["Index"]] = ctrl["Name"]
                 ctrl_id_list.append(str(ctrl["Index"]))
             elif "id" in ctrl.keys():
                 ctrl_id_name_dict[ctrl["id"]] = ctrl["Name"]
                 ctrl_id_list.append(str(ctrl["id"]))
     else:
@@ -12228,18 +12299,18 @@
             raidDict['Virtual Drive ID'] = ctrl_ld_list_dict.get(ctrl_id_name_dict.get(ctrlid))
             ldiskList = []
             for ld in lds:
                 if ld.get("ControllerName") == ctrl_id_name_dict.get(ctrlid):
                     LSI_flag = True
                     ldiskDict = collections.OrderedDict()
                     ldiskDict['Virtual Drive ID'] = ld.get("Index")
-                    ldiskDict['Capacity (GB)'] = ld.get("CAPACITY")
-                    ldiskDict['Raid Level'] = ld.get("VOLUME_RAID_LEVEL")
-                    ldiskDict['PhysicalDisks'] = ld.get("PhysicalDisks")
-                    ldiskDict['Firmware State'] = ld.get("State")
+                    ldiskDict['Capacity (GB)'] = ld.get("CAPACITY", ld.get("VDCap"))
+                    ldiskDict['Raid Level'] = ld.get("VOLUME_RAID_LEVEL", ld.get("raidMode"))
+                    ldiskDict['PhysicalDisks'] = ld.get("PhysicalDisks", ld.get("PDNums"))
+                    ldiskDict['Firmware State'] = ld.get("State", ld.get("VDStatus"))
                     ldiskList.append(ldiskDict)
             raidDict['ldisk'] = ldiskList
             raidList.append(raidDict)
         if not LSI_flag:
             result.State('Failure')
             result.Message(['No LSI raid controller'])
             return result
@@ -12268,14 +12339,20 @@
             result.State('Failure')
             result.Message(["Logical drive under PMC raid controller only support LOC, STL, DEL."])
             return result
         if args.option == "LOC" and args.duration is None:
             result.State('Failure')
             result.Message(["Please input duration parameter while setting LOC of logical drive under PMC raid controller."])
             return result
+    elif str(ctrl_id_name_dict.get(args.ctrlId)) in ctrl_type_dict.get('MV'):
+        ctrl_type = "MV"
+        if args.option != "DEL":
+            result.State('Failure')
+            result.Message(["Logical drive under MV raid controller only support DEL."])
+            return result
     else:
         ctrl_type = "LSI"
 
     args.ctrl_type = ctrl_type
     args.location = None
     args.init = None
     args.delete = None
@@ -12306,14 +12383,16 @@
                     return result
             res = RestFunc.locateLogicalDiskPMC(client, args.ctrlId, args.ldiskId, args.location, args.duration)
     elif args.init is not None:
         res = RestFunc.initLogicalDisk(client, args.ctrlId, args.ldiskId, args.init)
     elif args.delete is not None:
         if args.ctrl_type == "LSI":
             res = RestFunc.deleteLogicalDisk(client, args.ctrlId, args.ldiskId)
+        elif args.ctrl_type == "MV":
+            res = RestFunc.deleteMVLogicalDisk(client, args.ctrlId, args.ldiskId)
         else:
             res = RestFunc.deleteLogicalDiskPMC(client, args.ctrlId, args.ldiskId)
     if res == {}:
         result.State("Failure")
         result.Message(["disk operation failed"])
     elif res.get('code') == 0 and res.get('data') is not None:
         result.State('Success')
```

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6_41401.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6_41401.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,25 +209,28 @@
 
 
 def setVirtualDrive(client, args):
     result = ResultBean()
     ctrl_id_name_dict = {}
     ctrl_type_dict = {
         "LSI": [],
-        "PMC": []
+        "PMC": [],
+        "MV": []
     }
     ctrl_id_list = []
     res = RestFunc.getRaidCtrlInfo(client)
     if res.get('code') == 0 and res.get('data') is not None:
         ctrls = res.get('data')
         for ctrl in ctrls:
             if str(ctrl.get("RaidType")).upper() == "PMC":
                 ctrl_type_dict['PMC'].append(ctrl["Name"])
-            else:
+            elif str(ctrl.get("RaidType")).upper() == "LSI":
                 ctrl_type_dict['LSI'].append(ctrl["Name"])
+            elif str(ctrl.get("RaidType")).upper() == "MV":
+                ctrl_type_dict['MV'].append(ctrl["Name"])
             if "Index" in ctrl.keys():
                 ctrl_id_name_dict[ctrl["Index"]] = ctrl["Name"]
                 ctrl_id_list.append(str(ctrl["Index"]))
             elif "id" in ctrl.keys():
                 ctrl_id_name_dict[ctrl["id"]] = ctrl["Name"]
                 ctrl_id_list.append(str(ctrl["id"]))
     else:
@@ -269,18 +272,18 @@
             raidDict['Virtual Drive ID'] = ctrl_ld_list_dict.get(ctrl_id_name_dict.get(ctrlid))
             ldiskList = []
             for ld in lds:
                 if ld.get("ControllerName") == ctrl_id_name_dict.get(ctrlid):
                     LSI_flag = True
                     ldiskDict = collections.OrderedDict()
                     ldiskDict['Virtual Drive ID'] = ld.get("Index")
-                    ldiskDict['Capacity (GB)'] = ld.get("CAPACITY")
-                    ldiskDict['Raid Level'] = ld.get("VOLUME_RAID_LEVEL")
-                    ldiskDict['PhysicalDisks'] = ld.get("PhysicalDisks")
-                    ldiskDict['Firmware State'] = ld.get("State")
+                    ldiskDict['Capacity (GB)'] = ld.get("CAPACITY", ld.get("VDCap"))
+                    ldiskDict['Raid Level'] = ld.get("VOLUME_RAID_LEVEL", ld.get("raidMode"))
+                    ldiskDict['PhysicalDisks'] = ld.get("PhysicalDisks", ld.get("PDNums"))
+                    ldiskDict['Firmware State'] = ld.get("State", ld.get("VDStatus"))
                     ldiskList.append(ldiskDict)
             raidDict['ldisk'] = ldiskList
             raidList.append(raidDict)
         if not LSI_flag:
             result.State('Failure')
             result.Message(['No LSI raid controller'])
             return result
@@ -309,14 +312,20 @@
             result.State('Failure')
             result.Message(["Logical drive under PMC raid controller only support LOC, STL, DEL."])
             return result
         if args.option == "LOC" and args.duration is None:
             result.State('Failure')
             result.Message(["Please input duration parameter while setting LOC of logical drive under PMC raid controller."])
             return result
+    elif str(ctrl_id_name_dict.get(args.ctrlId)) in ctrl_type_dict.get('MV'):
+        ctrl_type = "MV"
+        if args.option != "DEL":
+            result.State('Failure')
+            result.Message(["Logical drive under MV raid controller only support DEL."])
+            return result
     else:
         ctrl_type = "LSI"
 
     args.ctrl_type = ctrl_type
     args.location = None
     args.init = None
     args.delete = None
@@ -347,14 +356,16 @@
                     return result
             res = RestFunc.locateLogicalDiskPMC(client, args.ctrlId, args.ldiskId, args.location, args.duration)
     elif args.init is not None:
         res = RestFunc.initLogicalDisk(client, args.ctrlId, args.ldiskId, args.init)
     elif args.delete is not None:
         if args.ctrl_type == "LSI":
             res = RestFunc.deleteLogicalDisk(client, args.ctrlId, args.ldiskId)
+        elif args.ctrl_type == "MV":
+            res = RestFunc.deleteMVLogicalDisk(client, args.ctrlId, args.ldiskId)
         else:
             res = RestFunc.deleteLogicalDiskPMC(client, args.ctrlId, args.ldiskId)
     if res == {}:
         result.State("Failure")
         result.Message(["disk operation failed"])
     elif res.get('code') == 0 and res.get('data') is not None:
         result.State('Success')
```

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM6_4140a.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM6_4140a.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/CommonM7.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/CommonM7.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,584 @@
 
 import os
 import re
 import collections
 
 from inspur_sm_sdk.util import RegularCheckUtil, RequestClient, fileUtil, configUtil
 from inspur_sm_sdk.command import RestFunc, IpmiFunc, RedfishFunc
-from inspur_sm_sdk.interface.CommonM6 import CommonM6, addPMCLogicalDisk
+from inspur_sm_sdk.interface.CommonM6 import CommonM6, addPMCLogicalDisk, addMVLogicalDisk
 from inspur_sm_sdk.interface.ResEntity import (
     ResultBean,
     SnmpBean,
     DestinationTXBean,
     HealthBean,
     ProductBean,
     CPUBean, Cpu,
     FanBean, Fan,
     MemoryBean, Memory,
-    PSUBean, PSUSingleBean
+    PSUBean, PSUSingleBean, NICBean, NicAllBean, NicPort, NICController
+
 )
 
 retry_count = 0
 
+PCI_IDS_LIST = {
+    0x1000: "LSI Logic / Symbios Logic",
+    0x1001: "Kolter Electronic",
+    0x1002: "Advanced Micro Devices, Inc",
+    0x1003: "ULSI Systems",
+    0x1004: "VLSI Technology Inc",
+    0x1005: "Avance Logic Inc",
+    0x1006: "Reply Group",
+    0x1007: "NetFrame Systems Inc",
+    0x1008: "Epson",
+    0x100a: "Phoenix Technologies",
+    0x100b: "National Semiconductor Corporation",
+    0x100c: "Tseng Labs Inc",
+    0x100d: "AST Research Inc",
+    0x100e: "Weitek",
+    0x1010: "Video Logic, Ltd",
+    0x1011: "Digital Equipment Corporation",
+    0x1012: "Micronics Computers Inc",
+    0x1013: "Cirrus Logic",
+    0x1014: "IBM",
+    0x1015: "LSI Logic Corp of Canada",
+    0x1016: "ICL Personal Systems",
+    0x1017: "SPEA Software AG",
+    0x1018: "Unisys Systems",
+    0x1019: "Elitegroup Computer Systems",
+    0x101a: "AT&T GIS (NCR)",
+    0x101b: "Vitesse Semiconductor",
+    0x101c: "Western Digital",
+    0x101d: "Maxim Integrated Products",
+    0x101e: "American Megatrends Inc",
+    0x101f: "PictureTel",
+    0x1020: "Hitachi Computer Products",
+    0x1021: "OKI Electric Industry Co. Ltd",
+    0x1022: "Advanced Micro Devices, Inc",
+    0x1023: "Trident Microsystems",
+    0x1024: "Zenith Data Systems",
+    0x1025: "Acer Incorporated",
+    0x1028: "Dell",
+    0x1029: "Siemens Nixdorf IS",
+    0x102a: "LSI Logic",
+    0x102b: "Matrox Electronics Systems Ltd",
+    0x102c: "Chips and Technologies",
+    0x102d: "Wyse Technology Inc",
+    0x102e: "Olivetti Advanced Technology",
+    0x102f: "Toshiba America",
+    0x1030: "TMC Research",
+    0x1031: "Miro Computer Products AG",
+    0x1032: "Compaq",
+    0x1033: "NEC Corporation",
+    0x1034: "Framatome Connectors USA Inc",
+    0x1035: "Comp. & Comm. Research Lab",
+    0x1036: "Future Domain Corp",
+    0x1037: "Hitachi Micro Systems",
+    0x1038: "AMP, Inc",
+    0x1039: "Silicon Integrated Systems",
+    0x103a: "Seiko Epson Corporation",
+    0x103b: "Tatung Corp. Of America",
+    0x103c: "Hewlett-Packard Company",
+    0x103e: "Solliday Engineering",
+    0x103f: "Synopsys/Logic Modeling Group",
+    0x1040: "Accelgraphics Inc",
+    0x1041: "Computrend",
+    0x1042: "Micron",
+    0x1043: "ASUSTeK Computer Inc",
+    0x1044: "Adaptec",
+    0x1045: "OPTi Inc",
+    0x1046: "IPC Corporation, Ltd",
+    0x1047: "Genoa Systems Corp",
+    0x1048: "Elsa AG",
+    0x1049: "Fountain Technologies, Inc",
+    0x104a: "STMicroelectronics",
+    0x104b: "BusLogic",
+    0x104c: "Texas Instruments",
+    0x104d: "Sony Corporation",
+    0x104e: "Oak Technology, Inc",
+    0x104f: "Co-time Computer Ltd",
+    0x1050: "Winbond Electronics Corp",
+    0x1051: "Anigma, Inc",
+    0x1052: "?Young Micro Systems",
+    0x1053: "Young Micro Systems",
+    0x1054: "Hitachi, Ltd",
+    0x1055: "Microchip Technology / SMSC",
+    0x1056: "ICL",
+    0x1057: "Motorola",
+    0x1058: "Electronics & Telecommunications RSH",
+    0x1059: "Kontron",
+    0x105a: "Promise Technology, Inc",
+    0x105b: "Foxconn International, Inc",
+    0x105c: "Wipro Infotech Limited",
+    0x105d: "Number 9 Computer Company",
+    0x105e: "Vtech Computers Ltd",
+    0x105f: "Infotronic America Inc",
+    0x1060: "United Microelectronics",
+    0x1061: "I.I.T.",
+    0x1062: "Maspar Computer Corp",
+    0x1063: "Ocean Office Automation",
+    0x1064: "Alcatel",
+    0x1065: "Texas Microsystems",
+    0x1066: "PicoPower Technology",
+    0x1067: "Mitsubishi Electric",
+    0x1068: "Diversified Technology",
+    0x1069: "Mylex Corporation",
+    0x106a: "Aten Research Inc",
+    0x106b: "United Microelectronics",
+    0x106c: "Hynix Semiconductor",
+    0x106d: "Sequent Computer Systems",
+    0x106e: "DFI, Inc",
+    0x106f: "City Gate Development Ltd",
+    0x1070: "Daewoo Telecom Ltd",
+    0x1071: "Mitac",
+    0x1072: "GIT Co Ltd",
+    0x1073: "Yamaha Corporation",
+    0x1074: "NexGen Microsystems",
+    0x1075: "Advanced Integrations Research",
+    0x1076: "Chaintech Computer Co. Ltd",
+    0x1077: "QLogic Corp",
+    0x1078: "Cyrix Corporation",
+    0x1079: "I-Bus",
+    0x107a: "NetWorth",
+    0x107b: "Gateway, Inc",
+    0x107c: "LG Electronics",
+    0x107d: "LeadTek Research Inc",
+    0x107e: "Interphase Corporation",
+    0x107f: "Data Technology Corporation",
+    0x1080: "Contaq Microsystems",
+    0x1081: "Supermac Technology",
+    0x1082: "EFA Corporation of America",
+    0x1083: "Forex Computer Corporation",
+    0x1084: "Parador",
+    0x1086: "J. Bond Computer Systems",
+    0x1087: "Cache Computer",
+    0x1088: "Microcomputer Systems (M) Son",
+    0x1089: "Data General Corporation",
+    0x108a: "SBS Technologies",
+    0x108c: "Oakleigh Systems Inc",
+    0x108d: "Olicom",
+    0x108e: "Oracle/SUN",
+    0x108f: "Systemsoft",
+    0x1090: "Compro Computer Services, Inc",
+    0x1091: "Intergraph Corporation",
+    0x1092: "Diamond Multimedia Systems",
+    0x1093: "National Instruments",
+    0x1094: "First International Computers",
+    0x1095: "Silicon Image, Inc",
+    0x1096: "Alacron",
+    0x1097: "Appian Technology",
+    0x1098: "Quantum Designs (H.K.) Ltd",
+    0x1099: "Samsung Electronics Co., Ltd",
+    0x109a: "Packard Bell",
+    0x109b: "Gemlight Computer Ltd",
+    0x109c: "Megachips Corporation",
+    0x109d: "Zida Technologies Ltd",
+    0x109e: "Brooktree Corporation",
+    0x109f: "Trigem Computer Inc",
+    0x123f: "LSI Logic",
+    0x11ca: "LSI Systems, Inc",
+    0x11c1: "LSI Corporation",
+    0x10db: "Rohm LSI Systems, Inc",
+    0x10df: "Emulex Corporation",
+    0x1166: "Broadcom",
+    0x10de: "NVIDIA Corporation",
+    0x11f8: "PMC-Sierra Inc.",
+    0x1344: "Micron Technology Inc.",
+    0x15b3: "Mellanox Technologies",
+    0x19a2: "Emulex Corporation",
+    0x1c5f: "Beijing Memblaze Technology Co. Ltd.",
+    0x1fc1: "QLogic, Corp.",
+    0x8086: "Intel Corporation",
+    0x9005: "Adaptec",
+    0x9004: "Adaptec",
+    0x14e4: "Brodcom Limited",
+    0x144d: "Samsung Electronics Co Ltd",
+    0x1924: "Solarflare Communications",
+    0xcabc: "Cambricon"
+}
+
 
 class CommonM7(CommonM6):
+
+    def setservice(self, client, args):
+        set_result = ResultBean()
+        if args.secureport is None and args.nonsecureport is None and args.state is None and args.timeout is None:
+            set_result.State("Failure")
+            set_result.Message(["please input a subcommand"])
+            return set_result
+        if args.servicename == 'fd-media' or args.servicename == 'telnet' or args.servicename == "solssh":
+            set_result.State("Not Support")
+            set_result.Message([])
+            return set_result
+        if args.servicename == 'ssh':
+            if args.nonsecureport is not None:
+                set_result.State("Failure")
+                set_result.Message(["ssh not support nonsecure port."])
+                return set_result
+        if args.state is not None and args.state == 'Disabled' and (
+                args.secureport is not None or args.nonsecureport is not None):
+            set_result.State("Failure")
+            set_result.Message(["Settings are not supported when -S is set to Disabled."])
+            return set_result
+        # WEB 服务使用IPMI命令，其他使用RESTFUL接口
+        if args.state is not None:
+            if args.servicename == "web":
+                if 'Enabled' in args.state:
+                    enabled = ' 0x01'
+                else:
+                    enabled = ' 0x00'
+            else:
+                if 'Enabled' in args.state:
+                    args.state = 1
+                else:
+                    args.state = 0
+        if args.secureport is not None:
+            if args.servicename == 'kvm' or args.servicename == "cdmedia" or args.servicename == "hdmedia" or args.servicename == "vnc":
+                set_result.State("Failure")
+                set_result.Message([str(args.servicename) + " not support setting secureport"])
+                return set_result
+            if args.secureport < 1 or args.secureport > 65535:
+                set_result.State("Failure")
+                set_result.Message(["secureport is in 1-65535."])
+                return set_result
+            else:
+                if args.servicename == "web":
+                    sp = '{:08x}'.format(args.secureport)
+                    sp_hex = hexReverse(sp)
+
+        if args.nonsecureport is not None:
+            if args.servicename == 'kvm' or args.servicename == "cdmedia" or args.servicename == "hdmedia" or args.servicename == "ssh":
+                set_result.State("Failure")
+                set_result.Message([str(args.service) + " not support setting nonsecureport"])
+                return set_result
+            if args.nonsecureport < 1 or args.nonsecureport > 65535:
+                set_result.State("Failure")
+                set_result.Message(["nonsecureport is in 1-65535."])
+                return set_result
+            else:
+                if args.servicename == "web":
+                    nsp = '{:08x}'.format(args.nonsecureport)
+                    nsp_hex = hexReverse(nsp)
+
+        if args.timeout is not None:
+            if args.servicename == 'ssh' or args.servicename == 'solssh':
+                if args.timeout % 60 == 0 and args.timeout >= 60 and args.timeout <= 1800:
+                    pass
+                    # t = '{:08x}'.format(args.timeout)
+                    # t_hex = hexReverse(t)
+                else:
+                    set_result.State("Failure")
+                    set_result.Message(
+                        ["This time is invalid, please enter a multiple of 60 and range from 60 to 1800."])
+                    return set_result
+            elif args.servicename == 'web':
+                if args.timeout % 60 == 0 and args.timeout >= 300 and args.timeout <= 1800:
+                    t = '{:08x}'.format(args.timeout)
+                    t_hex = hexReverse(t)
+                else:
+                    set_result.State("Failure")
+                    set_result.Message(
+                        ["This time is invalid, please enter a multiple of 60 and range from 300 to 1800."])
+                    return set_result
+            elif args.servicename == 'kvm' or args.servicename == 'vnc':
+                if args.timeout % 60 == 0 and args.timeout >= 300 and args.timeout <= 1800:
+                    pass
+                else:
+                    set_result.State("Failure")
+                    set_result.Message(
+                        ["This time is invalid, please enter a multiple of 60 and range from 300 to 1800."])
+                    return set_result
+            else:
+                set_result.State("Failure")
+                set_result.Message(["The timeout(-T) are not support to set."])
+                return set_result
+        # 获取信息
+        headers = RestFunc.login_M6(client)
+        if headers == {}:
+            login_res = ResultBean()
+            login_res.State("Failure")
+            login_res.Message(["login error, please check username/password/host/port"])
+            return login_res
+        client.setHearder(headers)
+        service_name = args.service.replace('-', '').title()
+        Info = None
+        try:
+            if args.servicename == 'web':
+                # IPMI命令获取web的service信息
+                Info_all = getattr(IpmiFunc, "getM5" + service_name + 'ByIpmi')(client)
+                if Info_all:
+                    if Info_all.get('code') == 0 and Info_all.get('data') is not None:
+                        Info = Info_all.get('data')  # web当前值
+                    else:
+                        set_result.State("Failure")
+                        set_result.Message(["failed to set service info " + Info_all.get('data', '')])
+                        RestFunc.logout(client)
+                        return set_result
+                else:
+                    set_result.State("Failure")
+                    set_result.Message(["failed to set service info"])
+                    RestFunc.logout(client)
+                    return set_result
+            else:
+                # restful方式获取service信息
+                rest_result = RestFunc.getServiceInfoByRest(client)
+                if rest_result.get('code') == 0 and rest_result.get('data') is not None:
+                    for item in rest_result.get('data'):
+                        if item['service_name'].replace('-', '') == args.service:
+                            Info = item
+                            break
+                else:
+                    set_result.State("Failure")
+                    set_result.Message(["failed to set service info"])
+                    RestFunc.logout(client)
+                    return set_result
+        except Exception as e:
+            set_result.State('Failure')
+            set_result.Message(['this command is incompatible with current server.'])
+            RestFunc.logout(client)
+            return set_result
+        if Info:
+            if args.enabled is None:
+                if args.servicename == 'web':
+                    status_dict = {'Disabled': '00', 'Enabled': '01'}
+                    if Info['Status'] == 'Disabled':
+                        set_result.State("Failure")
+                        set_result.Message(["please set status to Enabled firstly."])
+                        RestFunc.logout(client)
+                        return set_result
+                    enabled = hex(int(status_dict[Info['Status']]))
+                else:
+                    if Info['state'] == 0:
+                        set_result.State("Failure")
+                        set_result.Message(["please set status to Enabled firstly."])
+                        RestFunc.logout(client)
+                        return set_result
+                    args.state = 1
+
+            if args.nonsecureport is None:
+                if args.servicename == 'web':
+                    if Info['NonsecurePort'] == 'N/A':
+                        nsp_hex = "0xff " * 4
+                    else:
+                        nsp = '{:08x}'.format(Info['NonsecurePort'])
+                        nsp_hex = hexReverse(nsp)
+                else:
+                    args.nonsecureport = Info['non_secure_port']
+
+            if args.secureport is None:
+                if args.servicename == 'web':
+                    if Info['SecurePort'] == 'N/A':
+                        sp_hex = "0xff " * 4
+                    else:
+                        sp = '{:08x}'.format(Info['SecurePort'])
+                        sp_hex = hexReverse(sp)
+                else:
+                    args.secureport = Info['secure_port']
+
+            if args.timeout is None:
+                if args.servicename == 'web':
+                    if Info['Timeout'] == 'N/A':
+                        t_hex = "0xff " * 4
+                    else:
+                        t = '{:08x}'.format(Info['Timeout'])
+                        t_hex = hexReverse(t)
+                else:
+                    args.timeout = Info['time_out']
+
+            if args.servicename == 'web':
+                if Info['InterfaceName'] == 'N/A':
+                    interface_temp = "F" * 16
+                    interface = ascii2hex(interface_temp, 17)
+                else:
+                    interface = ascii2hex(Info['InterfaceName'], 17)
+            else:
+                args.activeSession = Info['active_session']
+                args.configurable = 1
+                args.id = Info['id']
+                args.maximumSessions = Info['maximum_sessions']
+                args.serviceId = Info['service_id']
+                args.serviceName = Info['service_name']
+                args.singleportStatus = Info['singleport_status']
+
+            if args.service == 'web':
+                set_Info = getattr(IpmiFunc, "setM5" + service_name + 'ByIpmi')(client, enabled, interface, nsp_hex,
+                                                                                sp_hex, t_hex)
+            else:
+                set_Info = RestFunc.setServiceInfoByRest(client, args, Info['id'])
+
+            if set_Info:
+                if set_Info.get('code') == 0:
+                    set_result.State("Success")
+                    set_result.Message(["set service success."])
+                    RestFunc.logout(client)
+                    return set_result
+                else:
+                    set_result.State("Failure")
+                    set_result.Message(["failed to set service: " + set_Info.get('data', '')])
+                    RestFunc.logout(client)
+                    return set_result
+            else:
+                set_result.State("Failure")
+                set_result.Message(["failed to set service, return None."])
+                RestFunc.logout(client)
+                return set_result
+        else:
+            set_result.State("Failure")
+            set_result.Message(["failed to set service info"])
+            RestFunc.logout(client)
+            return set_result
+
+    def getnic(self, client, args):
+        headers = RestFunc.login_M6(client)
+        if headers == {}:
+            login_res = ResultBean()
+            login_res.State("Failure")
+            login_res.Message(["login error, please check username/password/host/port"])
+            return login_res
+        client.setHearder(headers)
+        nicRes = ResultBean()
+
+        # health
+        overalhealth = RestFunc.getHealthSummaryByRest(client)
+        if overalhealth.get('code') == 0 and overalhealth.get('data') is not None and 'lan' in overalhealth.get('data'):
+            if overalhealth.get('data').get('lan') == 'na':
+                health = 'Absent'
+            elif overalhealth.get('data').get('lan').lower() == 'info':
+                health = 'OK'
+            else:
+                health = overalhealth.get('data').get('lan').capitalize()
+        else:
+            health = None
+        nicinfo = NicAllBean()
+        nicinfo.OverallHealth(health)
+        # get
+        # res=RestFunc.getAdapterByRest(client)
+        res = RestFunc.getAdapterByRest(client)
+        if res == {}:
+            nicRes.State("Failure")
+            nicRes.Message(["cannot get information"])
+        elif res.get('code') == 0 and res.get('data') is not None:
+            port_status_dict = {0: "Not Linked", 1: "Linked", 2: "NA", "Unknown": "NA", 255: "NA"}
+            nicRes.State("Success")
+            PCIElist = []
+            data = res.get('data')['sys_adapters']
+            for ada in data:
+                PCIEinfo = NICBean()
+                PCIEinfo.CommonName(ada['location'])
+                PCIEinfo.Location("mainboard")
+                adapterinfo = NICController()
+                adapterinfo.Id(ada['id'])
+                adapterinfo.Location(ada['location'])
+                if ada['vendor'] == "":
+                    adapterinfo.Manufacturer(None)
+                    PCIEinfo.Manufacturer(None)
+                else:
+                    if "0x" in ada['vendor']:
+                        maf = PCI_IDS_LIST.get(int(ada['vendor'], 16), ada['vendor'])
+                        adapterinfo.Manufacturer(maf)
+                        PCIEinfo.Manufacturer(maf)
+                    else:
+                        adapterinfo.Manufacturer(ada['vendor'])
+                        PCIEinfo.Manufacturer(ada['vendor'])
+                adapterinfo.Model(ada.get('model', None))
+                PCIEinfo.Model(ada.get('model', None))
+                # 青海湖没有该字段
+                # adapterinfo.Serialnumber(ada['serial_num'])
+                if 'serial_num' in ada:
+                    adapterinfo.Serialnumber(ada['serial_num'])
+                elif "sn" in ada:
+                    adapterinfo.Serialnumber(ada['sn'])
+                else:
+                    adapterinfo.Serialnumber(None)
+                if 'pn' in ada:
+                    adapterinfo.PN(ada['pn'])
+                else:
+                    adapterinfo.PN(None)
+                adapterinfo.FirmwareVersion(ada['fw_ver'])
+                ports = ada.get('ports', [])
+                adapterinfo.PortCount(len(ports))
+                portlist = []
+                for port in ports:
+                    portBean = NicPort()
+                    portBean.Id(port['id'])
+                    portBean.MACAddress(port['mac_addr'])
+                    portBean.LinkStatus(port_status_dict.get(port['status'], port['status']))
+                    portBean.MediaType(None)
+                    portlist.append(portBean.dict)
+                adapterinfo.Port(portlist)
+                controllerList = []
+                controllerList.append(adapterinfo.dict)
+                # PCIEinfo.Serialnumber(ada['serial_num'])
+                if 'serial_num' in ada:
+                    PCIEinfo.Serialnumber(ada['serial_num'])
+                else:
+                    PCIEinfo.Serialnumber(None)
+                PCIEinfo.State("Enabled")
+                if ada['present'] == 1 or ada['present'] == 'OK':
+                    PCIEinfo.Health('OK')
+                else:
+                    PCIEinfo.Health('Warning')
+                PCIEinfo.Controller(controllerList)
+                PCIElist.append(PCIEinfo.dict)
+            nicinfo.Maximum(len(data))
+            nicinfo.NIC(PCIElist)
+            nicRes.Message([nicinfo.dict])
+        elif res.get('code') != 0 and res.get('data') is not None:
+            nicRes.State("Failure")
+            nicRes.Message([res.get('data')])
+        else:
+            nicRes.State("Failure")
+            nicRes.Message(["get information error, error code " + str(res.get('code'))])
+
+        RestFunc.logout(client)
+        return nicRes
+
+    def getgpu(self, client, args):
+        res = ResultBean()
+        state = "Failure"
+        gpu_device_class_type = ["DisplayController", "ProcessingAccelerator"]
+        id_res = RedfishFunc.getChassisID(client)
+        if id_res.get('code') == 0 and id_res.get('data') is not None:
+            id_data = id_res.get('data')
+            id_url = None
+            for item in id_data:
+                id_url = item.get("@odata.id")
+                if id_url is not None:
+                    break
+            if id_url is not None:
+                pcie_res = RedfishFunc.getPCIEDevices(client, id_url)
+                if pcie_res.get('code') == 0 and pcie_res.get('data') is not None:
+                    pcie_data = pcie_res.get('data')
+                    gpu_list = []
+                    for item in pcie_data:
+                        gpu_url = item.get('@odata.id')
+                        if gpu_url is not None:
+                            gpu_res = RedfishFunc.getPCIEInfo(client, gpu_url)
+                            if gpu_res.get('code') == 0 and gpu_res.get('data') is not None:
+                                gpu_data = gpu_res.get('data')
+                                if gpu_data.get("Oem", {}).get("Public", {}).get("DeviceClass", "N/A") \
+                                        in gpu_device_class_type:
+                                    gpu_list.append(gpu_data)
+                    if len(gpu_list) > 0:
+                        state = "Success"
+                        message = gpu_list
+                    else:
+                        state = "Success"
+                        message = []
+                else:
+                    message = "Cannot get pcie info."
+            else:
+                message = "No chassis id."
+        else:
+            message = "Cannot get chassis id."
+        res.State(state)
+        res.Message([message])
+        return res
+
     def setpowerbudget(self, client, args):
         import collections
 
         def getSuspend(start, end, week_str):
             if start is not None and end is not None and week_str is not None:
                 if start > 24 or start < 0:
                     value = 'Invalid start, start range from 0-24'
@@ -324,94 +877,71 @@
             else:
                 bios_result.Message([mapper_result[1]])
                 bios_result.State('Failure')
                 return bios_result
 
             attr_request = []  # 统一处理-A指定的配置项或所有可获取的配置项
             if args.Attribute:  # 获取指定BIOS
-                if args.Attribute.strip().lower() not in attr_dict:
+                if args.Attribute.strip().lower().replace(" ", "") not in attr_dict:
                     bios_result.Message(["[{}] is invalid option.".format(args.Attribute)])
                     bios_result.State('Failure')
                     return bios_result
-                attr_request.append(args.Attribute.strip().lower())
+                attr_request.append(args.Attribute.strip().lower().replace(" ", ""))
             else:  # 获取全部BIOS项
                 attr_request = list(attr_dict.keys())
 
             bios = {}
             for attr_lower in attr_request:
                 attr = attr_dict[attr_lower]['getter']
                 attr_parent = attr_dict[attr_lower]['parent']
                 attr_desc = attr_dict[attr_lower]['description']
+                attr_desc_nospace = attr_desc.replace(" ", "")
                 if attr_parent not in server_bios:
 
                     # 根据指定的参数确定输出的提示信息
                     if args.Attribute:
                         bios_result.State('Failure')
                         bios_result.Message(["can't get the value of [{}].".format(attr_desc)])
                         return bios_result
                     else:
-                        bios[attr_desc] = None
+                        bios[attr_desc_nospace] = None
 
                 else:
                     l1_bios_value = server_bios[attr_parent]
                     if isinstance(l1_bios_value, dict):
                         if attr in l1_bios_value:
-                            bios[attr_desc] = self._transfer_value(l1_bios_value[attr], attr_dict[attr_lower]['setter'],
+                            bios[attr_desc_nospace] = self._transfer_value(l1_bios_value[attr], attr_dict[attr_lower]['setter'],
                                                                    attr_desc)
                         elif attr[:-1] in l1_bios_value:
-                            bios[attr_desc] = self._transfer_value(l1_bios_value[attr[:-1]][int(attr[-1])], attr_dict[attr_lower]['setter'],
+                            bios[attr_desc_nospace] = self._transfer_value(l1_bios_value[attr[:-1]][int(attr[-1])], attr_dict[attr_lower]['setter'],
                                                                    attr_desc)
                         else:
 
                             # 根据指定的参数确定输出的提示信息
                             if args.Attribute:
                                 bios_result.State('Failure')
                                 bios_result.Message(
                                     ["can't get value of [{}].".format(attr_desc)])
                                 return bios_result
                             else:
-                                bios[attr_desc] = None
+                                bios[attr_desc_nospace] = None
 
                     else:
 
                         # 根据指定的参数确定输出的提示信息
                         if args.Attribute:
                             bios_result.State('Failure')
                             bios_result.Message(
                                 ['not support getting value of [{}].'.format(attr_desc)])
                             return bios_result
                         else:
-                            bios[attr_desc] = None
-            if 'fileurl' not in args:
-                bios_result.State('Success')
-                bios_result.Message([bios])
-            elif args.fileurl is not None:
-                flag, file_path, file_name = fileUtil.parseUrl(args.fileurl)
-                if not flag:
-                    bios_result.State("Failure")
-                    bios_result.Message(['bios file path is not valid.'])
-                else:
-                    if file_name == "":
-                        file_name = "bios.json"
-                    if os.path.splitext(file_name)[1] != ".json":
-                        bios_result.State("Failure")
-                        bios_result.Message(['bios file should be xxx.json.'])
-                        return bios_result
-                    flag2, fileurl_last = fileUtil.checkUrl(os.path.join(file_path, file_name))
-                    if flag2:
-                        with open(fileurl_last, 'w') as f:
-                            f.write(json.dumps(bios, default=lambda o: o.__dict__, indent=4, ensure_ascii=True))
-                        bios_result.State('Success')
-                        bios_result.Message(["bios export to " + fileurl_last])
-                    else:
-                        bios_result.State("Failure")
-                        bios_result.Message([fileurl_last])
-            else:
-                bios_result.State('Success')
-                bios_result.Message([bios])
+                            bios[attr_desc_nospace] = None
+
+            bios_result.State('Success')
+            bios_result.Message([bios])
         else:
             bios_result.State('Failure')
             bios_result.Message([server_result.get('data')])
         return bios_result
 
     def _transfer_value(self, origin_value, value_map, user_key):
         """
@@ -440,15 +970,15 @@
         # 读取映射文件
         mapper_result = self._get_xml_mapper(args, 'value', 'cmd')
         # args.list = False
         if mapper_result[0]:
             if 'list' in args and args.list:  # 打印信息
                 help_list = []
                 for key, value in mapper_result[1].items():
-                    help_list.append('{:<35}: {}'.format(value['description'], list(value['setter'].keys())))
+                    help_list.append('{:<35}: {}'.format(value['description'].replace(" ", ""), list(value['setter'].keys())))
                 res.Message(help_list)
                 res.State('Success')
                 return res
             else:
                 attr_dict = mapper_result[1]
         else:
             res.Message([mapper_result[1]])
@@ -801,27 +1331,27 @@
                 bios_result.Message([server_bios])
             else:  # 获取指定BIOS项
                 bios = {}
                 attr = args.Attribute.lower()
                 for key, value in server_bios.items():
                     # 获取第一级BIOS项
                     if attr == key.lower():
-                        bios[key] = value
+                        bios[str(key).replace(" ", "")] = value
                         break
                     # 获取第二级BIOS项
                     if isinstance(value, dict):
                         for k, v in value.items():
                             if attr == k.lower():
-                                bios[key] = {k: v}
+                                bios[str(key).replace(" ", "")] = {k: v}
                                 break
                     elif isinstance(value, list) and value and isinstance(value[0], dict):
                         for i in value:
                             for k, v in i.items():
                                 if attr == k.lower():
-                                    bios.get(key, []).append({k: v})
+                                    bios.get(str(key).replace(" ", ""), []).append({k: v})
                                     break
                 if bios:
                     bios_result.State('Success')
                     bios_result.Message([bios])
                 else:
                     bios_result.State('Failure')
                     bios_result.Message(['Not support setting [{}] for now.'.format(args.Attribute)])
@@ -1857,131 +2387,14 @@
             product_Result.State('Success')
             product_Result.Message([product_Info.dict])
 
         # logout
         RestFunc.logout(client)
         return product_Result
 
-    def getcpu(self, client, args):
-        '''
-        get CPUs info
-        :param client:
-        :param args:
-        :return:
-        '''
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-        result = ResultBean()
-        cpu_Info = CPUBean()
-
-        # get
-        res = RestFunc.getCpuInfoByRest(client)
-        if res == {}:
-            result.State('Failure')
-            result.Message(['get cpu info failed'])
-        elif res.get('code') == 0 and res.get('data') is not None:
-            # getcpu
-            overalhealth = RestFunc.getHealthSummaryByRest(client)
-            if overalhealth.get('code') == 0 and overalhealth.get('data') is not None and 'cpu' in overalhealth.get(
-                    'data'):
-                if overalhealth.get('data').get('cpu') == 'na':
-                    cpu_Info.OverallHealth('Absent')
-                elif overalhealth.get('data').get('cpu').lower() == 'info':
-                    cpu_Info.OverallHealth('OK')
-                else:
-                    cpu_Info.OverallHealth(overalhealth.get('data').get('cpu').capitalize())
-            else:
-                cpu_Info.OverallHealth(None)
-            cpus = res.get('data').get('processors', [])
-            size = len(cpus)
-            Num = IpmiFunc.getM6DeviceNumByIpmi(client, '0x02')
-            if Num and Num.get('code') == 0:
-                DevConfNum = Num.get('data').get('DevNum')
-                cpu_Info.Maximum(DevConfNum)
-            else:
-                cpu_Info.Maximum(size)
-            # cpu_Info.Maximum(size)
-            # 通过sensor获取cpu_power
-            sensor = IpmiFunc.getSensorByNameByIpmi(client, 'CPU_Power')
-            if sensor and sensor.get('code') == 0:
-                temp = sensor.get('data')[0].get('value')
-                cpu_Info.TotalPowerWatts(float(temp) if (temp is not None and temp != 'na') else None)
-            else:
-                cpu_Info.TotalPowerWatts(None)
-            # cpu_Info.TotalPowerWatts(res.get('data').get('cpu_power',None))
-
-            list = []
-            i = 0
-            for cpu in cpus:
-                cpu_singe = Cpu()
-                if cpu.get('proc_status') == 1:
-                    # 在位
-                    name = 'CPU' + str(cpu.get('proc_id', 0))
-                    cpu_singe.CommonName(name)
-                    cpu_singe.Location('mainboard')
-                    if 'proc_name' in cpu:
-                        cpu_singe.Model(cpu.get('proc_name'))
-                        if 'Intel' in cpu.get('proc_name'):
-                            cpu_singe.Manufacturer('Intel')
-                        else:
-                            cpu_singe.Manufacturer(None)
-                    else:
-                        cpu_singe.Model(cpu.get(None))
-                        cpu_singe.Manufacturer(None)
-
-                    cpu_singe.L1CacheKiB(cpu.get('proc_l1cache_size', None))
-                    cpu_singe.L2CacheKiB(cpu.get('proc_l2cache_size', None))
-                    cpu_singe.L3CacheKiB(cpu.get('proc_l3cache_size', None))
-                    # 通过sensor获取cpu_DTS_Temp
-                    sensor = IpmiFunc.getSensorByNameByIpmi(client, 'CPU{0}_DTS'.format(i))
-                    if sensor and sensor.get('code') == 0:
-                        temp = sensor.get('data')[0].get('value')
-                        cpu_singe.Temperature(float(temp) if (temp is not None and temp != 'na') else None)
-                    else:
-                        cpu_singe.Temperature(None)
-                    cpu_singe.EnabledSetting(True)
-                    cpu_singe.ProcessorType('CPU')
-                    cpu_singe.ProcessorArchitecture('x86')
-                    cpu_singe.InstructionSet(cpu.get('instruct_set', 'x86-64'))
-                    cpu_singe.ProSpeedMHz(cpu.get('proc_speed', None))
-                    cpu_singe.MaxSpeedMHz(cpu.get('max_speed', None))
-                    cpu_singe.TotalCores(cpu.get('proc_used_core_count', None))
-                    cpu_singe.TotalThreads(cpu.get('proc_thread_count', None))
-                    cpu_singe.Socket(cpu.get('proc_id', 0))
-                    cpu_singe.PROCID(cpu.get('PROC_ID', None))
-                    cpu_singe.PPIN(cpu.get('ppin', None))
-                    cpu_singe.MicroCode(cpu.get('micro_code_ver', None))
-                    cpu_singe.TDP(cpu.get('proc_tdp'))
-                    cpu_singe.State('Enabled')
-                    cpu_singe.Health(cpu.get('status', None))
-                else:
-                    cpu_singe.CommonName('CPU' + str(cpu.get('proc_id')))
-                    cpu_singe.Location('mainboard')
-                    cpu_singe.State('Absent')
-
-                list.append(cpu_singe.dict)
-                i += 1
-            cpu_Info.CPU(list)
-            result.State('Success')
-            result.Message([cpu_Info.dict])
-        elif res.get('code') != 0 and res.get('data') is not None:
-            result.State("Failure")
-            result.Message(["get cpu information error, " + str(res.get('data'))])
-        else:
-            result.State("Failure")
-            result.Message(["get cpu information error, error code " + str(res.get('code'))])
-
-        RestFunc.logout(client)
-        return result
-
     def getfan(self, client, args):
         headers = RestFunc.login_M6(client)
         if headers == {}:
             login_res = ResultBean()
             login_res.State("Failure")
             login_res.Message(["login error, please check username/password/host/port"])
             return login_res
@@ -5025,130 +5438,14 @@
                     result.Message(['At least three options(CN/UL/LL/SC) must be chosen.'])
         else:
             result.State('Failure')
             result.Message(['get/set user rule failure!'])
         RestFunc.logout(client)
         return result
 
-    def getmemory(self, client, args):
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-        result = ResultBean()
-        memory_Info = MemoryBean()
-
-        # get
-        res = RestFunc.getMemoryInfoByRest(client)
-        if res == {}:
-            result.State('Failure')
-            result.Message(['get memory info failed'])
-        elif res.get('code') == 0 and res.get('data') is not None:
-            overalhealth = RestFunc.getHealthSummaryByRest(client)
-            if overalhealth.get('code') == 0 and overalhealth.get('data') is not None and \
-                    'memory' in overalhealth.get('data'):
-                if overalhealth.get('code') == 0 and overalhealth.get('data') is not None and \
-                        'memory' in overalhealth.get('data'):
-                    if overalhealth.get('data').get('memory') == 'na':
-                        memory_Info.OverallHealth('Absent')
-                    elif overalhealth.get('data').get('memory').lower() == 'info':
-                        memory_Info.OverallHealth('OK')
-                    else:
-                        memory_Info.OverallHealth(overalhealth.get('data').get('memory').capitalize())
-            else:
-                memory_Info.OverallHealth(None)
-            memorys = res.get('data').get('mem_modules', [])
-            size = len(memorys)
-            memory_Info.Maximum(res.get('data').get('total_memory_count', size))
-            memory_Info.Present(res.get('data').get('present_memory_count', None))
-            memory_Info.TotalSystemMemoryGiB(None)
-            # 通过sensor获取cpu_power
-            sensor = IpmiFunc.getSensorByNameByIpmi(client, 'Memory_Power')
-            if sensor and sensor.get('code') == 0:
-                temp = sensor.get('data')[0].get('value')
-                memory_Info.TotalPowerWatts(float(temp) if (temp is not None and temp != 'na') else None)
-            else:
-                memory_Info.TotalPowerWatts(None)
-
-            list = []
-            memoryGiB = 0
-            for memory in memorys:
-                memory_singe = Memory()
-                memory_singe.MemId(memory.get('mem_mod_id', 0))
-                if memory.get('mem_mod_status') == 1:
-                    # 在位
-                    if memory.get('mem_mod_slot', None) is None and 'mem_mod_cpu_num' in memory and \
-                            'mem_riser_num' in memory and 'mem_mod_socket_num' in memory:
-                        name = 'DIMM' + '{0}{1}{2}'.format(memory.get('mem_mod_cpu_num', 0),
-                                                           memory.get('mem_riser_num', 0),
-                                                           memory.get('mem_mod_socket_num', 0))
-                    else:
-                        name = memory.get('mem_mod_slot', None)
-                    memory_singe.CommonName(name)
-                    memory_singe.Location('mainboard')
-                    memory_singe.Manufacturer(memory.get('mem_mod_vendor', None))
-                    memory_singe.CapacityMiB(memory.get('mem_mod_size') * 1024 if 'mem_mod_size' in memory else None)
-                    memory_singe.OperatingSpeedMhz(memory.get('mem_mod_frequency', None))
-                    memory_singe.CurrentSpeedMhz(memory.get('mem_mod_current_frequency', None))
-                    memory_singe.AssetTag(memory.get('mem_mod_asset_tag', None))
-                    memory_singe.SerialNumber(memory.get('mem_mod_serial_num', None))
-                    memory_singe.MemoryDeviceType(memory.get('mem_mod_type', None))
-                    memory_singe.DataWidthBits(memory.get('mem_data_width', None))
-                    memory_singe.RankCount(memory.get('mem_mod_ranks', None))
-                    if 'mem_mod_part_num' in memory:
-                        memory_singe.PartNumber(memory.get('mem_mod_part_num').strip())
-                    else:
-                        memory_singe.PartNumber(None)
-                    if 'mem_base_module' in memory:
-                        memory_singe.BaseModule(memory.get('mem_base_module', None))
-
-                    memory_singe.Technology(memory.get('mem_mod_technology', None))
-                    memory_singe.MinVoltageMillivolt(memory.get('mem_mod_min_volt', None))
-                    if 'mem_mod_size' in memory:
-                        memoryGiB = memoryGiB + memory.get('mem_mod_size')
-                    else:
-                        memoryGiB = memoryGiB + 0
-                    memory_singe.State('Enabled')
-                    if 'status' in memory:
-                        memory_singe.Health(memory.get('status'))
-                    elif 'mem_mod_status' in memory:
-                        memory_singe.Health('OK' if int(memory.get('mem_mod_status')) == 1 else None)
-                    else:
-                        memory_singe.Health(None)
-                else:
-                    if memory.get('mem_mod_slot', None) is None and 'mem_mod_cpu_num' in memory and \
-                            'mem_riser_num' in memory and 'mem_mod_socket_num' in memory:
-                        name = 'DIMM' + '{0}{1}{2}'.format(memory.get('mem_mod_cpu_num', 0),
-                                                           memory.get('mem_riser_num', 0),
-                                                           memory.get('mem_mod_socket_num', 0))
-                    else:
-                        name = memory.get('mem_mod_slot', None)
-                    memory_singe.CommonName(name)
-                    memory_singe.Location('mainboard')
-                    memory_singe.State('Absent')
-
-                list.append(memory_singe.dict)
-            memory_Info.Memory(list)
-            memory_Info.TotalSystemMemoryGiB(memoryGiB)
-
-            result.State('Success')
-            result.Message([memory_Info.dict])
-        elif res.get('code') != 0 and res.get('data') is not None:
-            result.State("Failure")
-            result.Message(["get memory information error, " + res.get('data')])
-        else:
-            result.State("Failure")
-            result.Message(["get memory information error, error code " + str(res.get('code'))])
-
-        RestFunc.logout(client)
-        return result
-
     def getpsu(self, client, args):
         headers = RestFunc.login_M6(client)
         if headers == {}:
             login_res = ResultBean()
             login_res.State("Failure")
             login_res.Message(["login error, please check username/password/host/port"])
             return login_res
@@ -5207,18 +5504,20 @@
                     psu.OutputVoltage(temp[i].get('ps_out_volt') if 'ps_out_volt' in temp[i] else None)
                     psu.PowerInputWatts(temp[i].get('ps_in_power') if 'ps_in_power' in temp[i] else None)
                     psu.OutputAmperage(
                         temp[i].get('ps_out_current') if 'ps_out_current' in temp[i] else None)
                     psu.PartNumber(None if temp[i].get('part_num', None) == '' else temp[i].get('part_num', None))
                     psu.PowerSupplyType(temp[i].get('input_type', 'Unknown'))
                     psu.LineInputVoltage(temp[i].get('ps_in_volt') if 'ps_in_volt' in temp[i] else None)
-                    psu.PowerCapacityWatts(temp[i].get('ps_out_power_max', None))
+                    # psu.PowerCapacityWatts(temp[i].get('ps_out_power_max', None))
+                    # 2023年3月27日 
+                    psu.PowerCapacityWatts(temp[i].get('rated_power', None))
                     psu.FirmwareVersion(None if temp[i].get('fw_ver', None) == '' else temp[i].get('fw_ver', None))
                     psu.SerialNumber(temp[i].get('serial_num', None))
-                    psu.Temperature(temp[i].get('psu_max_temperature', None))
+                    psu.Temperature(temp[i].get('ambient_temperature', None))
                     if 'status' in temp[i]:
                         psu.Health(
                             'OK' if temp[i].get('status').upper() == 'OK' else temp[i].get('status').capitalize())
                     else:
                         if 'power_status' in temp[i]:
                             psu.Health('OK' if temp[i].get('power_status') == 0 else 'Critical')
                         else:
@@ -5558,24 +5857,27 @@
 
 def createVirtualDrive(client, args):
     result = ResultBean()
     ctrl_id_name_dict = {}
     ctrl_id_list = []
     ctrl_type_dict = {
         "LSI": [],
-        "PMC": []
+        "PMC": [],
+        "MV": []
     }
     res = RestFunc.getRaidCtrlInfo(client)
     if res.get('code') == 0 and res.get('data') is not None:
         ctrls = res.get('data')
         for ctrl in ctrls:
             if str(ctrl.get("RaidType")).upper() == "PMC":
                 ctrl_type_dict['PMC'].append(ctrl["Name"])
             elif str(ctrl.get("RaidType")).upper() == "LSI":
                 ctrl_type_dict['LSI'].append(ctrl["Name"])
+            elif str(ctrl.get("RaidType")).upper() == "MV":
+                ctrl_type_dict['MV'].append(ctrl["Name"])
             if "Index" in ctrl.keys():
                 ctrl_id_name_dict[ctrl["Index"]] = ctrl["Name"]
                 ctrl_id_list.append(str(ctrl["Index"]))
             elif "id" in ctrl.keys():
                 ctrl_id_name_dict[ctrl["id"]] = ctrl["Name"]
                 ctrl_id_list.append(str(ctrl["id"]))
     else:
@@ -5607,41 +5909,43 @@
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             if str(ctrl_id_name_dict.get(ctrlid)) in ctrl_type_dict.get('LSI'):
                 raidDict['Controller Type'] = "LSI"
-            else:
+            elif str(ctrl_id_name_dict.get(ctrlid)) in ctrl_type_dict.get('PMC'):
                 raidDict['Controller Type'] = "PMC"
+            elif str(ctrl_id_name_dict.get(ctrlid)) in ctrl_type_dict.get('MV'):
+                raidDict['Controller Type'] = "MV"
             pdiskList = []
             for pd in pds:
                 if pd.get("ControllerName") == ctrl_id_name_dict.get(ctrlid):
                     LSI_flag = True
                     pdiskDict = collections.OrderedDict()
-                    pdiskDict['Slot Number'] = pd.get("SlotNum")
+                    pdiskDict['Slot Number'] = pd.get("SlotNum", pd.get("slotNum"))
                     pdiskDict['Drive Name'] = pd.get("Name")
                     if "InterfaceType" in pd:
                         pdiskDict['Interface'] = pd.get("InterfaceType")
                     elif "interface_type" in pd:
                         pdiskDict['Interface'] = pd.get("interface_type")
                     else:
                         pdiskDict['Interface'] = None
                     if "MediaType" in pd:
-                        pdiskDict['Media Type'] = pd.get("MediaType")
+                        pdiskDict['Media Type'] = pd.get("MediaType",)
                     elif "type" in pd:
                         pdiskDict['Media Type'] = pd.get("type")
                     else:
-                        pdiskDict['Media Type'] = None
+                        pdiskDict['Media Type'] = pd.get("mediaType")
                     if "NONCoercedSize" in pd:
                         pdiskDict['Capacity'] = pd.get("NONCoercedSize")
                     elif "size" in pd:
                         pdiskDict['Capacity'] = pd.get("size")
                     else:
-                        pdiskDict['Capacity'] = None
+                        pdiskDict['Capacity'] = pd.get("cap")
                     if "FWState" in pd:
                         pdiskDict['Firmware State'] = pd.get("FWState")
                     else:
                         pdiskDict['Firmware State'] = None
                     if "array_number" in pd:
                         pdiskDict['Array Number'] = pd.get("array_number")
                     else:
@@ -5660,14 +5964,16 @@
         result.State('Failure')
         result.Message(["Please input ctrlId parameter!"])
         return result
     elif str(ctrl_id_name_dict.get(args.ctrlId)) in ctrl_type_dict.get('LSI'):
         result = addLogicalDisk(client, args, pds, ctrl_id_name_dict)
     elif str(ctrl_id_name_dict.get(args.ctrlId)) in ctrl_type_dict.get('PMC'):
         result = addPMCLogicalDisk(client, args, pds, ctrl_id_name_dict)
+    elif str(ctrl_id_name_dict.get(args.ctrlId)) in ctrl_type_dict.get('MV'):
+        result = addMVLogicalDisk(client, args)
     else:
         result.State('Failure')
         result.Message(["No raid controller!"])
     return result
 
 
 def addLogicalDisk(client, args, pds, ctrl_id_name_dict):
@@ -5803,8 +6109,28 @@
         result.Message(["create virtual drive failed"])
     elif res.get('code') == 0 and res.get('data') is not None:
         result.State('Success')
         result.Message(['create virtual drive successful.'])
     else:
         result.State("Failure")
         result.Message(['create virtual drive failed, ' + str(res.get('data'))])
-    return result
+    return result
+
+
+# Ascii转十六进制
+def ascii2hex(data, length):
+    count = length - len(data)
+    list_h = []
+    for c in data:
+        list_h.append(str(hex(ord(c))))
+    data = ' '.join(list_h) + ' 0x00' * count
+    return data
+
+
+# 十六进制字符串逆序
+def hexReverse(data):
+    pattern = re.compile('.{2}')
+    time_hex = ' '.join(pattern.findall(data))
+    seq = time_hex.split(' ')[::-1]
+    data = '0x' + ' 0x'.join(seq)
+    return data
+
```

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/I24M6.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/I24M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/IBase.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/IBase.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5180M5.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5180M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5_435.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5_435.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NF5280M5_436.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NF5280M5_436.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/NS5160M6.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/NS5160M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/ResEntity.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/ResEntity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1769,14 +1769,20 @@
 
     def Location(self):
         return self.dict['Location']
 
     def Location(self, value):
         self.dict['Location'] = value
 
+    def PN(self):
+        return self.dict['PN']
+
+    def PN(self, value):
+        self.dict['PN'] = value
+
 
 class NicPort():
     def __init__(self):
         self.dict = collections.OrderedDict()
 
     def Id(self):
         return self.dict['Id']
```

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/interface/SA5212M5Impl.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/interface/SA5212M5Impl.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/route/route.yml` & `inspursmsdk-2.1.1/inspur_sm_sdk/route/route.yml`

 * *Files 3% similar despite different names*

```diff
@@ -139,8 +139,17 @@
     common: CommonA7
     1.1308: CommonA7_11308
 NF5468A7:
     common: CommonA7
     1.1308: CommonA7_11308
 NF5688A7:
     common: CommonA7
-    1.1308: CommonA7_11308
+    1.1308: CommonA7_11308
+TS860-M7-A0-R0-00:
+    common: CommonM7
+    1.3505: CommonM7_13505
+TS860M7:
+    common: CommonM7
+    1.3505: CommonM7_13505
+NF8480M7:
+    common: CommonM7
+    1.3505: CommonM7_13505
```

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/util/HostTypeJudge.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/util/HostTypeJudge.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/util/RedfishClient.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/util/RedfishClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/util/RegularCheckUtil.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/util/RegularCheckUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/util/RequestClient.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/util/RequestClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/util/configUtil.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/util/configUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/util/fileUtil.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/util/fileUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspur_sm_sdk/util/parameterConversion.py` & `inspursmsdk-2.1.1/inspur_sm_sdk/util/parameterConversion.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/inspursmsdk.egg-info/PKG-INFO` & `inspursmsdk-2.1.1/inspursmsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.1.0
+Version: 2.1.1
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.1.0/inspursmsdk.egg-info/SOURCES.txt` & `inspursmsdk-2.1.1/inspursmsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.0/ism.py` & `inspursmsdk-2.1.1/ism.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     ISM_EXIST = False
 sys.path.append(os.path.join(sys.path[0], "interface"))
 current_time = time.strftime(
     '%Y-%m-%d   %H:%M:%S',
     time.localtime(
         time.time()))
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 
 ERR_dict = {
     'ERR_CODE_CMN_FAIL': 'data acquisition exception',
     'ERR_CODE_PARAM_NULL': 'parameter is null',
     'ERR_CODE_INPUT_ERROR': 'parameter error',
     'ERR_CODE_INTF_FAIL': 'create link exception',
```

### Comparing `inspursmsdk-2.1.0/setup.py` & `inspursmsdk-2.1.1/setup.py`

 * *Files identical despite different names*

