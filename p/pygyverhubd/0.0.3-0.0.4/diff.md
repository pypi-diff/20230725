# Comparing `tmp/pygyverhubd-0.0.3.tar.gz` & `tmp/pygyverhubd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygyverhubd-0.0.3.tar", last modified: Tue Jul 11 16:30:49 2023, max compression
+gzip compressed data, was "pygyverhubd-0.0.4.tar", last modified: Tue Jul 25 19:19:27 2023, max compression
```

## Comparing `pygyverhubd-0.0.3.tar` & `pygyverhubd-0.0.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/cli/new_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/cli/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/device_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/filesystem/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/mapped.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/mapped_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/union.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/vfspath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/virtual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/filesystem/virtual_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/proto/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/proto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/proto/ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.374907 pygyverhubd-0.0.3/gyverhubd/ui/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/gyverhubd/ui/components/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/controls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/prompt_confirm.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/components/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/ui/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/gyverhubd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/pygyverhubd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 16:30:49.000000 pygyverhubd-0.0.3/pygyverhubd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-11 16:30:39.000000 pygyverhubd-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:30:49.378908 pygyverhubd-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:19:27.734303 pygyverhubd-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-25 19:19:27.734303 pygyverhubd-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:19:27.730302 pygyverhubd-0.0.4/gyverhubd/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:19:27.730302 pygyverhubd-0.0.4/gyverhubd/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/cli/new_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/cli/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/device_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:19:27.734303 pygyverhubd-0.0.4/gyverhubd/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/filesystem/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/filesystem/mapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/filesystem/mapped_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/filesystem/union.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/filesystem/vfspath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/filesystem/virtual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/filesystem/virtual_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:19:27.734303 pygyverhubd-0.0.4/gyverhubd/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/proto/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/proto/proto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/proto/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/proto/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:19:27.734303 pygyverhubd-0.0.4/gyverhubd/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:19:27.734303 pygyverhubd-0.0.4/gyverhubd/ui/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/prompt_confirm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/components/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/ui/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/gyverhubd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:19:27.734303 pygyverhubd-0.0.4/pygyverhubd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-25 19:19:27.000000 pygyverhubd-0.0.4/pygyverhubd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-25 19:19:27.000000 pygyverhubd-0.0.4/pygyverhubd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:19:27.000000 pygyverhubd-0.0.4/pygyverhubd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-25 19:19:27.000000 pygyverhubd-0.0.4/pygyverhubd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 19:19:27.000000 pygyverhubd-0.0.4/pygyverhubd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-25 19:19:16.000000 pygyverhubd-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:19:27.734303 pygyverhubd-0.0.4/setup.cfg
```

### Comparing `pygyverhubd-0.0.3/LICENSE` & `pygyverhubd-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/PKG-INFO` & `pygyverhubd-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygyverhubd
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python implementation of GyverHub device
 Author-email: NekoNekoNyan <me@neko-dev.ru>
 License: MIT License
         
         Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pygyverhubd-0.0.3/README.md` & `pygyverhubd-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/cli/pack.py` & `pygyverhubd-0.0.4/gyverhubd/cli/pack.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     x = asn1.DerInteger().decode(x).value
     pub = asn1.DerSequence().decode(pub)
     p, q, g = list(pub)
     tup = (pow(g, x, p), g, p, q, x)
     return DSA.construct(tup)
 
 
-def make_package(base_path: pathlib.Path, key: typing.Optional[DSA.DsaKey],
+def make_package(base_path: pathlib.Path, key: typing.Optional[DSA.DsaKey], main_device: typing.Optional[str],
                  out_path: typing.Union[pathlib.Path, typing.IO[bytes]]):
     with zipfile.ZipFile(out_path, 'w') as zf:
         file_hashes = []
 
         for dir_path, dirs, files in os.walk(base_path):
             for i in tuple(dirs):
                 if i.startswith('.'):
@@ -69,19 +69,22 @@
             hasher.update(data_hash)
 
         if key is not None:
             signer = DSS.new(key, 'fips-186-3')
             signature = signer.sign(hasher)
             zf.writestr('SIGN', signature)
 
+        if main_device is not None:
+            zf.writestr('MAIN', main_device)
+
 
 def do_pack(args):
     output = args.output
     if output is None:
         output = args.directory.resolve()
         output = output.with_suffix(output.suffix + '.zip')
 
     key = None
     if args.sign is not None:
         key = import_private_key(args.sign.read())
 
-    make_package(args.directory, key, output)
+    make_package(args.directory, key, args.main, output)
```

### Comparing `pygyverhubd-0.0.3/gyverhubd/cli/run.py` & `pygyverhubd-0.0.4/gyverhubd/cli/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import importlib
 import os
 import sys
+import zipfile
 
 from gyverhubd import run_server
 from gyverhubd.proto.mqtt import MqttProtocol
-from gyverhubd.proto.ws import WSProtocol
+from gyverhubd.proto.serial import SerialProtocol
+from gyverhubd.proto.websocket import WebsocketProtocol
 
 
 def import_device(main: str):
     module, _, cls = main.rpartition('.')
     loaded = module in sys.modules
     mod = __import__(module)
     if loaded:
@@ -16,33 +18,62 @@
 
     for i in module.split('.')[1:]:
         mod = getattr(mod, i)
 
     return getattr(mod, cls)
 
 
+def get_main_device(path):
+    if path.is_dir():
+        main = path / 'MAIN'
+        if not main.exists():
+            print("No device to run specified and no MAIN file found!", file=sys.stderr)
+            sys.exit(1)
+
+        return main.read_text('utf-8')
+
+    else:
+        with zipfile.ZipFile(path) as zf:
+            try:
+                main = zf.getinfo('MAIN')
+            except KeyError:
+                print("No device to run specified and package has no MAIN device!", file=sys.stderr)
+                sys.exit(1)
+
+            return zf.read(main).decode('utf-8')
+
+
 def do_run2(args):
     protocols = []
     devices = []
 
-    if args.websocket:
-        protocols.append(WSProtocol(args.websocket_host, args.http_port, args.websocket_port))
+    if args.websocket is not None:
+        options = (i.partition('=') for i in args.websocket_option)
+        protocols.append(WebsocketProtocol(args.websocket, {k: v for k, _, v in options}))
+
     if args.mqtt is not None:
-        protocols.append(MqttProtocol(args.mqtt, args.mqtt_port, username=args.mqtt_username,
-                                      password=args.mqtt_password))
+        options = (i.partition('=') for i in args.mqtt_option)
+        protocols.append(MqttProtocol(args.mqtt, {k: v for k, _, v in options}))
+
+    if args.serial is not None:
+        options = (i.partition('=') for i in args.serial_option)
+        protocols.append(SerialProtocol(args.serial, {k: v for k, _, v in options}))
 
     path = str(args.path.resolve())
     if path not in sys.path:
         sys.path.append(path)
 
     cached = sys.path_importer_cache.get(path)
     if cached is not None:
         cached.invalidate_caches()
         del sys.path_importer_cache[path]
 
+    if args.device is None:
+        args.device = [get_main_device(args.path)]
+
     for i in args.device:
         dev_cls = import_device(i)
         devices.append(dev_cls())
 
     run_server(*devices, protocols=protocols)
```

### Comparing `pygyverhubd-0.0.3/gyverhubd/context.py` & `pygyverhubd-0.0.4/gyverhubd/context.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/device.py` & `pygyverhubd-0.0.4/gyverhubd/device.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/device_utils.py` & `pygyverhubd-0.0.4/gyverhubd/device_utils.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/errors.py` & `pygyverhubd-0.0.4/gyverhubd/errors.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/events.py` & `pygyverhubd-0.0.4/gyverhubd/events.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/filesystem/base.py` & `pygyverhubd-0.0.4/gyverhubd/filesystem/base.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/filesystem/mapped.py` & `pygyverhubd-0.0.4/gyverhubd/filesystem/mapped.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/filesystem/mapped_file.py` & `pygyverhubd-0.0.4/gyverhubd/filesystem/mapped_file.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/filesystem/union.py` & `pygyverhubd-0.0.4/gyverhubd/filesystem/union.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/filesystem/vfspath.py` & `pygyverhubd-0.0.4/gyverhubd/filesystem/vfspath.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/filesystem/virtual.py` & `pygyverhubd-0.0.4/gyverhubd/filesystem/virtual.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/filesystem/virtual_file.py` & `pygyverhubd-0.0.4/gyverhubd/filesystem/virtual_file.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/info.py` & `pygyverhubd-0.0.4/gyverhubd/info.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/local.py` & `pygyverhubd-0.0.4/gyverhubd/local.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/proto/mqtt.py` & `pygyverhubd-0.0.4/gyverhubd/proto/serial.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,101 +1,95 @@
 import asyncio
 import json
-import os
-import sys
 import typing
 
-import aiomqtt
+import serial_asyncio
 
 from . import Protocol, Request
 
-__all__ = ["MqttProtocol"]
+__all__ = ["SerialProtocol", "protocol_factory"]
 
 
-class MqttRequest(Request):
-    def __init__(self, protocol, message: aiomqtt.Message):
-        super().__init__(message.topic.value, message.payload.decode('ascii'))
-        self.protocol: MqttProtocol = protocol
+def _parse_options(options: typing.Dict[str, str]) -> dict:
+    if options is None:
+        return {}
+
+    res = {}
+    for option, value in options.items():
+        if option == 'baudrate':
+            res['baudrate'] = int(value)
+
+        elif option in {'timeout', 'write_timeout', 'inter_byte_timeout'}:
+            res[option] = float(value)
+
+        elif option in {'xonxoff', 'rtscts', 'dsrdtr', 'exclusive'}:
+            value = value.lower()
+            if value in {'yes', 'on', 'true'}:
+                res[option] = True
+            elif value in {'no', 'off', 'false'}:
+                res[option] = True
+            else:
+                raise ValueError(f"Invalid serial option ({option}) value: {value!r}")
+
+        elif option == 'config':
+            res['bytesize'] = int(value[0])
+            res['parity'] = value[1].upper()
+            if len(value) == 3:
+                res['stopbits'] = int(value[2:])
+            else:
+                res['stopbits'] = float(value[2:])
+
+        else:
+            raise ValueError(f"Invalid serial option {option!r}")
+
+    return res
 
-        if not self.value:
-            self.value = None
 
-        if self.cmd is None:
-            self.clid = self.value
-            self.value = None
+class SerialRequest(Request):
+    def __init__(self, protocol, data):
+        self.protocol: SerialProtocol = protocol
+
+        assert isinstance(data, str) and data and data[-1] == '\0'
+        url, eq, data = data[:-1].partition('=')
+        super().__init__(url, data if eq else None)
 
     async def respond(self, data: dict):
         if self.did is not None:
             data['id'] = self.did
-        data = '\n' + json.dumps(data) + '\n'
-        await self.protocol.send_to(self, data)
+        await self.protocol.send(data)
 
     def set_focused(self, value: bool):
-        pass
+        self.protocol.focused = value
 
 
-class MqttProtocol(Protocol):
-    def __init__(self, host: str, port=1883, **kwargs):
-        self._host = host
-        self._port = port
-        self._client_kwargs = kwargs
-
-        self._client: typing.Optional[aiomqtt.Client] = None
-        self._server = None
-        self._stopped = False
-        self._prefixes = []
-
-    @property
-    def focused(self) -> bool:
-        return False
+class SerialProtocol(Protocol):
+    def __init__(self, port: str, options: typing.Dict[str, str] = None):
+        self._reader = self._writer = None
+        self._kwargs = _parse_options(options)
+        self._kwargs['url'] = port
+        self.focused = False
 
     def bind(self, server):
         self._server = server
-        self._prefixes.clear()
         server.add_event_listener('start', self.__server_start)
         server.add_event_listener('stop', self.__server_stop)
 
     async def __server_start(self):
-        self._client = aiomqtt.Client(self._host, self._port, **self._client_kwargs)
-        await self._client.connect()
-        asyncio.ensure_future(self._messages())
-
-        for dev in self._server.devices:
-            await self._client.subscribe(dev.prefix)
-            await self._client.subscribe(f"{dev.prefix}/{dev.id}/#")
-            await self._client.publish(f"{dev.prefix}/hub/{dev.id}/status", b'online')
-            self._prefixes.append(dev.prefix)
-
-    async def _messages(self):
-        async with self._client.messages() as messages:
-            try:
-                async for message in messages:
-                    req = MqttRequest(self, message)
-                    asyncio.ensure_future(self._server.dispatch_event('request', req))
-            except aiomqtt.MqttError as e:
-                if not self._stopped:
-                    raise e
+        self._reader, self._writer = await serial_asyncio.open_serial_connection(**self._kwargs)
+        asyncio.ensure_future(self._read_requests())
 
-    async def __server_stop(self):
-        for dev in self._server.devices:
-            await self._client.publish(f"{dev.prefix}/hub/{dev.id}/status", b'offline')
+    async def _read_requests(self):
+        while not self._writer.is_closing():
+            data = await self._reader.readuntil(b'\x00')
+            data = data.decode()
+            req = SerialRequest(self, data)
+            asyncio.ensure_future(self._server.dispatch_event('request', req))
 
-        self._stopped = True
-        await self._client.disconnect()
+    async def __server_stop(self):
+        self._writer.close()
 
     async def send(self, data: dict):
         data = '\n' + json.dumps(data) + '\n'
-        for prefix in self._prefixes:
-            await self._client.publish(f"{prefix}/hub", data)
-
-    async def send_to(self, req: MqttRequest, data: str):
-        if req.did is None:
-            await self._client.publish(f"{req.prefix}/hub", data)
-        else:
-            await self._client.publish(f"{req.prefix}/hub/{req.clid}/{req.did}", data)
-
+        self._writer.write(data.encode())
 
-protocol_factory = MqttProtocol
 
-if sys.platform.lower() == "win32" or os.name.lower() == "nt":
-    # fix for aiomqtt
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
+protocol_factory = SerialProtocol
```

### Comparing `pygyverhubd-0.0.3/gyverhubd/proto/proto.py` & `pygyverhubd-0.0.4/gyverhubd/proto/proto.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     clid: typing.Optional[str]
     did: typing.Optional[str]
     cmd: typing.Optional[str]
     name: typing.Optional[str]
     value: typing.Optional[str]
     protocol: Protocol
 
-    def __init__(self, url: str, value: str):
+    def __init__(self, url: str, value: typing.Optional[str]):
         self.prefix, self.clid, self.did, self.cmd, self.name = parse_url(url)
         self.value = value
 
     async def respond(self, data: dict):
         raise NotImplementedError()
 
     def set_focused(self, value: bool):
```

### Comparing `pygyverhubd-0.0.3/gyverhubd/server.py` & `pygyverhubd-0.0.4/gyverhubd/server.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/ui/color.py` & `pygyverhubd-0.0.4/gyverhubd/ui/color.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/ui/component.py` & `pygyverhubd-0.0.4/gyverhubd/ui/component.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/ui/components/button.py` & `pygyverhubd-0.0.4/gyverhubd/ui/components/button.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/ui/components/controls.py` & `pygyverhubd-0.0.4/gyverhubd/ui/components/controls.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/ui/components/datetime.py` & `pygyverhubd-0.0.4/gyverhubd/ui/components/datetime.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/ui/components/tabs.py` & `pygyverhubd-0.0.4/gyverhubd/ui/components/tabs.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/ui/components/text.py` & `pygyverhubd-0.0.4/gyverhubd/ui/components/text.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/ui/layout.py` & `pygyverhubd-0.0.4/gyverhubd/ui/layout.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/gyverhubd/utils.py` & `pygyverhubd-0.0.4/gyverhubd/utils.py`

 * *Files identical despite different names*

### Comparing `pygyverhubd-0.0.3/pygyverhubd.egg-info/PKG-INFO` & `pygyverhubd-0.0.4/pygyverhubd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygyverhubd
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python implementation of GyverHub device
 Author-email: NekoNekoNyan <me@neko-dev.ru>
 License: MIT License
         
         Copyright (c) 2023 NekoNekoNyan <neko-dev.ru>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pygyverhubd-0.0.3/pygyverhubd.egg-info/SOURCES.txt` & `pygyverhubd-0.0.4/pygyverhubd.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 gyverhubd/filesystem/vfspath.py
 gyverhubd/filesystem/virtual.py
 gyverhubd/filesystem/virtual_file.py
 gyverhubd/proto/__init__.py
 gyverhubd/proto/mqtt.py
 gyverhubd/proto/proto.py
 gyverhubd/proto/serial.py
-gyverhubd/proto/ws.py
+gyverhubd/proto/websocket.py
 gyverhubd/ui/__init__.py
 gyverhubd/ui/base.py
 gyverhubd/ui/color.py
 gyverhubd/ui/component.py
 gyverhubd/ui/layout.py
 gyverhubd/ui/components/__init__.py
 gyverhubd/ui/components/button.py
```

### Comparing `pygyverhubd-0.0.3/pyproject.toml` & `pygyverhubd-0.0.4/pyproject.toml`

 * *Files identical despite different names*

