# Comparing `tmp/tkadw-0.3.3.tar.gz` & `tmp/tkadw-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkadw-0.3.3.tar", max compression
+gzip compressed data, was "tkadw-0.3.5.tar", max compression
```

## Comparing `tkadw-0.3.3.tar` & `tkadw-0.3.5.tar`

### file list

```diff
@@ -1,82 +1,92 @@
--rw-r--r--   0        0        0      421 2023-07-16 05:19:58.382178 tkadw-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2745 2023-07-16 05:19:27.945475 tkadw-0.3.3/README.md
--rw-r--r--   0        0        0      591 2023-07-14 05:18:03.595214 tkadw-0.3.3/tkadw/__init__.py
--rw-r--r--   0        0        0      729 2023-07-15 04:57:05.864349 tkadw-0.3.3/tkadw/__main__.py
--rw-r--r--   0        0        0    14254 2023-07-16 00:41:12.056850 tkadw-0.3.3/tkadw/doc.py
--rw-r--r--   0        0        0       82 2023-07-09 09:06:40.819424 tkadw-0.3.3/tkadw/game/__init__.py
--rw-r--r--   0        0        0      274 2023-07-09 10:06:51.337745 tkadw-0.3.3/tkadw/game/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1081 2023-07-09 09:05:04.428075 tkadw-0.3.3/tkadw/game/__pycache__/surface.cpython-311.pyc
--rw-r--r--   0        0        0     1486 2023-07-09 10:06:51.339744 tkadw-0.3.3/tkadw/game/__pycache__/window.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-07-09 09:06:15.869430 tkadw-0.3.3/tkadw/game/action.py
--rw-r--r--   0        0        0      302 2023-07-09 09:05:03.855776 tkadw-0.3.3/tkadw/game/surface.py
--rw-r--r--   0        0        0      503 2023-07-09 09:03:53.662343 tkadw-0.3.3/tkadw/game/window.py
--rw-r--r--   0        0        0        0 2023-07-05 02:47:22.168814 tkadw-0.3.3/tkadw/utility/__init__.py
--rw-r--r--   0        0        0      127 2023-07-05 03:10:22.091006 tkadw-0.3.3/tkadw/utility/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      143 2023-07-05 02:48:08.371100 tkadw-0.3.3/tkadw/utility/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      851 2023-07-05 03:10:22.094005 tkadw-0.3.3/tkadw/utility/__pycache__/appconfig.cpython-310.pyc
--rw-r--r--   0        0        0     1779 2023-07-05 02:48:08.372100 tkadw-0.3.3/tkadw/utility/__pycache__/appconfig.cpython-311.pyc
--rw-r--r--   0        0        0    10003 2023-07-15 00:06:35.798144 tkadw-0.3.3/tkadw/utility/__pycache__/dragtool.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.3.3/tkadw/utility/app.config
--rw-r--r--   0        0        0      944 2023-07-05 02:48:08.189796 tkadw-0.3.3/tkadw/utility/appconfig.py
--rw-r--r--   0        0        0     5435 2023-07-15 00:06:32.738325 tkadw-0.3.3/tkadw/utility/dragtool.py
--rw-r--r--   0        0        0      107 2023-07-05 01:34:36.098785 tkadw-0.3.3/tkadw/windows/__init__.py
--rw-r--r--   0        0        0      229 2023-07-05 03:10:20.021585 tkadw-0.3.3/tkadw/windows/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      273 2023-07-05 01:35:29.380630 tkadw-0.3.3/tkadw/windows/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6883 2023-07-05 03:12:28.822756 tkadw-0.3.3/tkadw/windows/__pycache__/theme.cpython-310.pyc
--rw-r--r--   0        0        0    15793 2023-07-16 02:32:48.335683 tkadw-0.3.3/tkadw/windows/__pycache__/theme.cpython-311.pyc
--rw-r--r--   0        0        0     1138 2023-07-14 23:55:33.173781 tkadw-0.3.3/tkadw/windows/canvas/__init__.py
--rw-r--r--   0        0        0     1263 2023-07-05 03:10:20.085734 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1945 2023-07-14 23:57:15.913264 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12827 2023-07-05 03:10:21.840626 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc
--rw-r--r--   0        0        0    23197 2023-07-15 12:30:24.901956 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0    38279 2023-07-05 03:10:20.174751 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc
--rw-r--r--   0        0        0    46492 2023-07-15 05:42:36.854511 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc
--rw-r--r--   0        0        0    11053 2023-07-05 03:10:21.911520 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc
--rw-r--r--   0        0        0    21085 2023-07-05 01:35:43.431699 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     6171 2023-07-05 03:10:22.086485 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc
--rw-r--r--   0        0        0    11993 2023-07-16 02:33:29.600856 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2694 2023-07-05 03:12:28.867163 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc
--rw-r--r--   0        0        0     4558 2023-07-05 01:36:52.241618 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc
--rw-r--r--   0        0        0    13219 2023-07-05 03:10:21.930952 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc
--rw-r--r--   0        0        0    25157 2023-07-16 00:24:41.799054 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0      943 2023-07-05 03:10:21.883207 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc
--rw-r--r--   0        0        0     2148 2023-07-16 00:33:11.740565 tkadw-0.3.3/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc
--rw-r--r--   0        0        0    18105 2023-07-15 12:30:12.087468 tkadw-0.3.3/tkadw/windows/canvas/button.py
--rw-r--r--   0        0        0     6156 2023-07-05 01:39:19.281978 tkadw-0.3.3/tkadw/windows/canvas/checkbox.py
--rw-r--r--   0        0        0    41631 2023-07-15 05:42:31.545384 tkadw-0.3.3/tkadw/windows/canvas/drawengine.py
--rw-r--r--   0        0        0    15971 2023-07-05 01:35:43.285417 tkadw-0.3.3/tkadw/windows/canvas/entry.py
--rw-r--r--   0        0        0     7018 2023-07-16 02:33:29.496750 tkadw-0.3.3/tkadw/windows/canvas/frame.py
--rw-r--r--   0        0        0     2442 2023-07-05 01:36:52.052770 tkadw-0.3.3/tkadw/windows/canvas/separator.py
--rw-r--r--   0        0        0    17828 2023-07-16 00:24:41.660268 tkadw-0.3.3/tkadw/windows/canvas/textbox.py
--rw-r--r--   0        0        0     4625 2023-07-16 02:11:24.455259 tkadw-0.3.3/tkadw/windows/canvas/titlebar.py
--rw-r--r--   0        0        0      782 2023-07-16 00:33:11.573705 tkadw-0.3.3/tkadw/windows/canvas/widget.py
--rw-r--r--   0        0        0      223 2023-07-05 01:38:08.509601 tkadw-0.3.3/tkadw/windows/fluent/__init__.py
--rw-r--r--   0        0        0      401 2023-07-05 03:10:21.986646 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      481 2023-07-05 01:38:08.644612 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2899 2023-07-05 03:10:22.025283 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc
--rw-r--r--   0        0        0     5148 2023-07-05 01:38:39.662205 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     2955 2023-07-05 03:10:22.017187 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc
--rw-r--r--   0        0        0     5190 2023-07-05 01:36:27.311777 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     1315 2023-07-05 03:10:22.047317 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc
--rw-r--r--   0        0        0     1968 2023-07-05 01:38:48.418651 tkadw-0.3.3/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0     4604 2023-07-05 01:38:39.519641 tkadw-0.3.3/tkadw/windows/fluent/button.py
--rw-r--r--   0        0        0     4545 2023-07-05 01:36:27.195727 tkadw-0.3.3/tkadw/windows/fluent/entry.py
--rw-r--r--   0        0        0      952 2023-07-05 01:38:48.118337 tkadw-0.3.3/tkadw/windows/fluent/frame.py
--rw-r--r--   0        0        0    66280 2022-07-26 17:24:46.000000 tkadw-0.3.3/tkadw/windows/fluent/GeneralSans-Regular.ttf
--rw-r--r--   0        0        0      639 2023-07-05 01:37:20.730737 tkadw-0.3.3/tkadw/windows/fluent/test.py
--rw-r--r--   0        0        0    25229 2023-07-16 02:32:48.172721 tkadw-0.3.3/tkadw/windows/theme.py
--rw-r--r--   0        0        0      151 2023-07-15 04:00:51.951970 tkadw-0.3.3/tkadw/windows/widgets/__init__.py
--rw-r--r--   0        0        0      271 2023-07-05 03:10:21.933019 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      395 2023-07-15 04:02:14.716290 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    19005 2023-07-05 03:10:21.948576 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc
--rw-r--r--   0        0        0    23348 2023-07-15 09:49:04.159720 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc
--rw-r--r--   0        0        0     2545 2023-07-05 03:10:21.971123 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc
--rw-r--r--   0        0        0     4377 2023-07-05 01:35:47.771212 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc
--rw-r--r--   0        0        0     3435 2023-07-15 04:48:08.638319 tkadw-0.3.3/tkadw/windows/widgets/__pycache__/mdi.cpython-311.pyc
--rw-r--r--   0        0        0    20035 2023-07-15 09:49:03.946070 tkadw-0.3.3/tkadw/windows/widgets/adw.py
--rw-r--r--   0        0        0     1992 2023-07-04 10:38:07.052633 tkadw-0.3.3/tkadw/windows/widgets/label.py
--rw-r--r--   0        0        0        0 2023-07-04 10:38:58.527667 tkadw-0.3.3/tkadw/windows/widgets/listbox.py
--rw-r--r--   0        0        0     1469 2023-07-15 04:48:08.519396 tkadw-0.3.3/tkadw/windows/widgets/mdi.py
--rw-r--r--   0        0        0        0 2023-07-15 06:50:07.630293 tkadw-0.3.3/tkadw/windows/widgets/toolbox.py
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 tkadw-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      421 2023-07-25 02:48:14.270638 tkadw-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3020 2023-07-25 05:02:48.562105 tkadw-0.3.5/README.md
+-rw-r--r--   0        0        0      636 2023-07-25 02:48:14.195797 tkadw-0.3.5/tkadw/__init__.py
+-rw-r--r--   0        0        0      629 2023-07-25 02:48:14.350383 tkadw-0.3.5/tkadw/__main__.py
+-rw-r--r--   0        0        0    14254 2023-07-16 00:41:12.056850 tkadw-0.3.5/tkadw/doc.py
+-rw-r--r--   0        0        0       82 2023-07-09 09:06:40.819424 tkadw-0.3.5/tkadw/game/__init__.py
+-rw-r--r--   0        0        0      274 2023-07-09 10:06:51.337745 tkadw-0.3.5/tkadw/game/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1081 2023-07-09 09:05:04.428075 tkadw-0.3.5/tkadw/game/__pycache__/surface.cpython-311.pyc
+-rw-r--r--   0        0        0     1623 2023-07-21 14:14:43.215025 tkadw-0.3.5/tkadw/game/__pycache__/window.cpython-311.pyc
+-rw-r--r--   0        0        0      146 2023-07-21 23:04:31.076115 tkadw-0.3.5/tkadw/game/sprite.py
+-rw-r--r--   0        0        0      302 2023-07-09 09:05:03.855776 tkadw-0.3.5/tkadw/game/surface.py
+-rw-r--r--   0        0        0      573 2023-07-21 14:14:42.889759 tkadw-0.3.5/tkadw/game/window.py
+-rw-r--r--   0        0        0      258 2023-07-25 04:35:13.985130 tkadw-0.3.5/tkadw/layout/__init__.py
+-rw-r--r--   0        0        0      684 2023-07-25 04:35:14.104912 tkadw-0.3.5/tkadw/layout/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2710 2023-07-25 04:56:28.925488 tkadw-0.3.5/tkadw/layout/__pycache__/column.cpython-311.pyc
+-rw-r--r--   0        0        0     4656 2023-07-25 05:00:02.984546 tkadw-0.3.5/tkadw/layout/__pycache__/put.cpython-311.pyc
+-rw-r--r--   0        0        0     2572 2023-07-25 04:58:14.523375 tkadw-0.3.5/tkadw/layout/__pycache__/row.cpython-311.pyc
+-rw-r--r--   0        0        0     1021 2023-07-25 04:56:28.814094 tkadw-0.3.5/tkadw/layout/column.py
+-rw-r--r--   0        0        0     2381 2023-07-25 05:00:02.849289 tkadw-0.3.5/tkadw/layout/put.py
+-rw-r--r--   0        0        0      946 2023-07-25 04:58:14.408996 tkadw-0.3.5/tkadw/layout/row.py
+-rw-r--r--   0        0        0        0 2023-07-05 02:47:22.168814 tkadw-0.3.5/tkadw/utility/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-05 03:10:22.091006 tkadw-0.3.5/tkadw/utility/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      143 2023-07-05 02:48:08.371100 tkadw-0.3.5/tkadw/utility/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      851 2023-07-05 03:10:22.094005 tkadw-0.3.5/tkadw/utility/__pycache__/appconfig.cpython-310.pyc
+-rw-r--r--   0        0        0     1779 2023-07-05 02:48:08.372100 tkadw-0.3.5/tkadw/utility/__pycache__/appconfig.cpython-311.pyc
+-rw-r--r--   0        0        0    10003 2023-07-15 00:06:35.798144 tkadw-0.3.5/tkadw/utility/__pycache__/dragtool.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.3.5/tkadw/utility/app.config
+-rw-r--r--   0        0        0      944 2023-07-05 02:48:08.189796 tkadw-0.3.5/tkadw/utility/appconfig.py
+-rw-r--r--   0        0        0     5435 2023-07-15 00:06:32.738325 tkadw-0.3.5/tkadw/utility/dragtool.py
+-rw-r--r--   0        0        0      107 2023-07-05 01:34:36.098785 tkadw-0.3.5/tkadw/windows/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-05 03:10:20.021585 tkadw-0.3.5/tkadw/windows/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      273 2023-07-05 01:35:29.380630 tkadw-0.3.5/tkadw/windows/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6883 2023-07-05 03:12:28.822756 tkadw-0.3.5/tkadw/windows/__pycache__/theme.cpython-310.pyc
+-rw-r--r--   0        0        0    20303 2023-07-25 04:27:03.987697 tkadw-0.3.5/tkadw/windows/__pycache__/theme.cpython-311.pyc
+-rw-r--r--   0        0        0     1138 2023-07-14 23:55:33.173781 tkadw-0.3.5/tkadw/windows/canvas/__init__.py
+-rw-r--r--   0        0        0     1263 2023-07-05 03:10:20.085734 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1945 2023-07-14 23:57:15.913264 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12827 2023-07-05 03:10:21.840626 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0        0        0    24715 2023-07-25 03:13:46.501249 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0    38279 2023-07-05 03:10:20.174751 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc
+-rw-r--r--   0        0        0    46492 2023-07-15 05:42:36.854511 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc
+-rw-r--r--   0        0        0    11053 2023-07-05 03:10:21.911520 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc
+-rw-r--r--   0        0        0    21085 2023-07-05 01:35:43.431699 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     6171 2023-07-05 03:10:22.086485 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc
+-rw-r--r--   0        0        0    11993 2023-07-25 00:33:28.501565 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2694 2023-07-05 03:12:28.867163 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc
+-rw-r--r--   0        0        0     4558 2023-07-05 01:36:52.241618 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc
+-rw-r--r--   0        0        0    13219 2023-07-05 03:10:21.930952 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc
+-rw-r--r--   0        0        0    25157 2023-07-16 00:24:41.799054 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0      943 2023-07-05 03:10:21.883207 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2214 2023-07-25 02:48:14.598610 tkadw-0.3.5/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc
+-rw-r--r--   0        0        0    19965 2023-07-25 03:13:46.132356 tkadw-0.3.5/tkadw/windows/canvas/button.py
+-rw-r--r--   0        0        0     6156 2023-07-05 01:39:19.281978 tkadw-0.3.5/tkadw/windows/canvas/checkbox.py
+-rw-r--r--   0        0        0    41631 2023-07-15 05:42:31.545384 tkadw-0.3.5/tkadw/windows/canvas/drawengine.py
+-rw-r--r--   0        0        0    15971 2023-07-05 01:35:43.285417 tkadw-0.3.5/tkadw/windows/canvas/entry.py
+-rw-r--r--   0        0        0     7018 2023-07-25 00:33:28.363491 tkadw-0.3.5/tkadw/windows/canvas/frame.py
+-rw-r--r--   0        0        0     1928 2023-07-17 04:17:02.611338 tkadw-0.3.5/tkadw/windows/canvas/scrollbar.py
+-rw-r--r--   0        0        0     2442 2023-07-05 01:36:52.052770 tkadw-0.3.5/tkadw/windows/canvas/separator.py
+-rw-r--r--   0        0        0    17828 2023-07-16 00:24:41.660268 tkadw-0.3.5/tkadw/windows/canvas/textbox.py
+-rw-r--r--   0        0        0     4625 2023-07-16 02:11:24.455259 tkadw-0.3.5/tkadw/windows/canvas/titlebar.py
+-rw-r--r--   0        0        0      829 2023-07-25 02:48:14.320275 tkadw-0.3.5/tkadw/windows/canvas/widget.py
+-rw-r--r--   0        0        0      223 2023-07-05 01:38:08.509601 tkadw-0.3.5/tkadw/windows/fluent/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-05 03:10:21.986646 tkadw-0.3.5/tkadw/windows/fluent/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      481 2023-07-05 01:38:08.644612 tkadw-0.3.5/tkadw/windows/fluent/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2899 2023-07-05 03:10:22.025283 tkadw-0.3.5/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0        0        0     5148 2023-07-05 01:38:39.662205 tkadw-0.3.5/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     2955 2023-07-05 03:10:22.017187 tkadw-0.3.5/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc
+-rw-r--r--   0        0        0     5190 2023-07-05 01:36:27.311777 tkadw-0.3.5/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     1315 2023-07-05 03:10:22.047317 tkadw-0.3.5/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc
+-rw-r--r--   0        0        0     1968 2023-07-05 01:38:48.418651 tkadw-0.3.5/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     4604 2023-07-05 01:38:39.519641 tkadw-0.3.5/tkadw/windows/fluent/button.py
+-rw-r--r--   0        0        0     4545 2023-07-05 01:36:27.195727 tkadw-0.3.5/tkadw/windows/fluent/entry.py
+-rw-r--r--   0        0        0      952 2023-07-05 01:38:48.118337 tkadw-0.3.5/tkadw/windows/fluent/frame.py
+-rw-r--r--   0        0        0    66280 2022-07-26 17:24:46.000000 tkadw-0.3.5/tkadw/windows/fluent/GeneralSans-Regular.ttf
+-rw-r--r--   0        0        0      639 2023-07-05 01:37:20.730737 tkadw-0.3.5/tkadw/windows/fluent/test.py
+-rw-r--r--   0        0        0    37403 2023-07-25 03:52:25.175668 tkadw-0.3.5/tkadw/windows/theme.py
+-rw-r--r--   0        0        0      151 2023-07-15 04:00:51.951970 tkadw-0.3.5/tkadw/windows/widgets/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-05 03:10:21.933019 tkadw-0.3.5/tkadw/windows/widgets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      395 2023-07-15 04:02:14.716290 tkadw-0.3.5/tkadw/windows/widgets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    19005 2023-07-05 03:10:21.948576 tkadw-0.3.5/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc
+-rw-r--r--   0        0        0    23374 2023-07-20 23:39:05.118210 tkadw-0.3.5/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc
+-rw-r--r--   0        0        0     2545 2023-07-05 03:10:21.971123 tkadw-0.3.5/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc
+-rw-r--r--   0        0        0     4443 2023-07-25 02:48:14.754551 tkadw-0.3.5/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc
+-rw-r--r--   0        0        0     3435 2023-07-15 04:48:08.638319 tkadw-0.3.5/tkadw/windows/widgets/__pycache__/mdi.cpython-311.pyc
+-rw-r--r--   0        0        0    20069 2023-07-20 23:39:04.914194 tkadw-0.3.5/tkadw/windows/widgets/adw.py
+-rw-r--r--   0        0        0     2039 2023-07-25 02:48:14.174162 tkadw-0.3.5/tkadw/windows/widgets/label.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:38:58.527667 tkadw-0.3.5/tkadw/windows/widgets/listbox.py
+-rw-r--r--   0        0        0     1469 2023-07-15 04:48:08.519396 tkadw-0.3.5/tkadw/windows/widgets/mdi.py
+-rw-r--r--   0        0        0     1517 2023-07-18 09:23:03.152145 tkadw-0.3.5/tkadw/windows/widgets/task.py
+-rw-r--r--   0        0        0        0 2023-07-15 06:50:07.630293 tkadw-0.3.5/tkadw/windows/widgets/toolbox.py
+-rw-r--r--   0        0        0     3599 1970-01-01 00:00:00.000000 tkadw-0.3.5/PKG-INFO
```

### Comparing `tkadw-0.3.3/README.md` & `tkadw-0.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -76,8 +76,16 @@
 >> `321` 新增`AdwMDI`组件
 > 
 >> `322` 添加`metro`主题
 
 > `0.3.3`
 >> `331` 修复`AdwDrawFrame`的边框宽度问题
 > 
->> `332` 增加主题属性`AdwDrawFrame` `padding`
+>> `332` 增加主题属性`AdwDrawFrame` `padding`
+
+> `0.3.4`
+>> `341` 为`AdwTButton`增添新样式`win11_accent_light` `win11_accent_dark`
+
+> `0.3.5`
+>> `351`补充`AdwTCircularButton`主题组件
+> 
+>> `352`增添新快速布局`row`、`coloumn`以及高级布局`put`，所有可视化组件已继承布局类。
```

### Comparing `tkadw-0.3.3/tkadw/__init__.py` & `tkadw-0.3.5/tkadw/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,12 +4,15 @@
 from tkadw.windows import *
 
 # 0.3.0加入
 from tkadw.windows.theme import *
 
 from tkadw.game import *
 
+# 0.3.5加入
+from tkadw.layout import *
+
 # from tkadw.tkite import * 已废弃移除
 # from tkadw.win11 import * 已废弃移除
 # from tkadw.advanced import * 已废弃移除，改为from tkadw.adw import Adw导入
 # from tkadw.bilibili import BiliBiliButton, BiliBiliDarkButton, BiliBiliFrame, BiliBiliDarkFrame, \
 #     BiliBiliEntry, BiliBiliDarkEntry, BiliBiliDarkTextBox, BiliBiliTextBox 已废弃移除
```

### Comparing `tkadw-0.3.3/tkadw/doc.py` & `tkadw-0.3.5/tkadw/doc.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/game/__pycache__/surface.cpython-311.pyc` & `tkadw-0.3.5/tkadw/game/__pycache__/surface.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/utility/__pycache__/appconfig.cpython-310.pyc` & `tkadw-0.3.5/tkadw/utility/__pycache__/appconfig.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/utility/__pycache__/appconfig.cpython-311.pyc` & `tkadw-0.3.5/tkadw/utility/__pycache__/appconfig.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/utility/__pycache__/dragtool.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.3.5/tkadw/utility/__pycache__/dragtool.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/utility/appconfig.py` & `tkadw-0.3.5/tkadw/utility/appconfig.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/utility/dragtool.py` & `tkadw-0.3.5/tkadw/utility/dragtool.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/__pycache__/theme.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/__pycache__/theme.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__init__.py` & `tkadw-0.3.5/tkadw/windows/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x5491b264 (Sat Jul 15 12:30:12 2023 UTC)
-files sz: 18105
+moddate:  0xea3dbf64 (Tue Jul 25 03:13:46 2023 UTC)
+files sz: 19965
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -211,197 +211,197 @@
                428 MAKE_FUNCTION            0
                430 LOAD_CONST              32 ('AdwDrawBasicCircularButton')
                432 LOAD_NAME                5 (AdwDrawBasicButton)
                434 PRECALL                  3
                438 CALL                     3
                448 STORE_NAME              19 (AdwDrawBasicCircularButton)
    
-   525         450 PUSH_NULL
+   559         450 PUSH_NULL
                452 LOAD_BUILD_CLASS
-               454 LOAD_CONST              33 (<code object AdwDrawCircularButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 525>)
+               454 LOAD_CONST              33 (<code object AdwDrawCircularButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 559>)
                456 MAKE_FUNCTION            0
                458 LOAD_CONST              34 ('AdwDrawCircularButton')
                460 LOAD_NAME               19 (AdwDrawBasicCircularButton)
                462 PRECALL                  3
                466 CALL                     3
                476 STORE_NAME              20 (AdwDrawCircularButton)
    
-   530         478 PUSH_NULL
+   564         478 PUSH_NULL
                480 LOAD_BUILD_CLASS
-               482 LOAD_CONST              35 (<code object AdwDrawCircularDarkButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 530>)
+               482 LOAD_CONST              35 (<code object AdwDrawCircularDarkButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 564>)
                484 MAKE_FUNCTION            0
                486 LOAD_CONST              36 ('AdwDrawCircularDarkButton')
                488 LOAD_NAME               19 (AdwDrawBasicCircularButton)
                490 PRECALL                  3
                494 CALL                     3
                504 STORE_NAME              21 (AdwDrawCircularDarkButton)
    
-   535         506 LOAD_NAME               22 (__name__)
+   569         506 LOAD_NAME               22 (__name__)
                508 LOAD_CONST              37 ('__main__')
                510 COMPARE_OP               2 (==)
                516 EXTENDED_ARG             1
                518 POP_JUMP_FORWARD_IF_FALSE   333 (to 1186)
    
-   536         520 LOAD_CONST               0 (0)
+   570         520 LOAD_CONST               0 (0)
                522 LOAD_CONST              38 (('Tk',))
                524 IMPORT_NAME             23 (tkinter)
                526 IMPORT_FROM             24 (Tk)
                528 STORE_NAME              24 (Tk)
                530 POP_TOP
    
-   538         532 PUSH_NULL
+   572         532 PUSH_NULL
                534 LOAD_NAME               24 (Tk)
                536 PRECALL                  0
                540 CALL                     0
                550 STORE_NAME              25 (root)
    
-   540         552 PUSH_NULL
+   574         552 PUSH_NULL
                554 LOAD_NAME                6 (AdwDrawButton)
                556 LOAD_CONST              39 ('Hello')
                558 KW_NAMES                40
                560 PRECALL                  1
                564 CALL                     1
                574 STORE_NAME              26 (button)
    
-   541         576 LOAD_NAME               26 (button)
+   575         576 LOAD_NAME               26 (button)
                578 LOAD_METHOD             27 (bind)
                600 LOAD_CONST              41 ('<<Click>>')
-               602 LOAD_CONST              42 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 541>)
+               602 LOAD_CONST              42 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 575>)
                604 MAKE_FUNCTION            0
                606 PRECALL                  2
                610 CALL                     2
                620 POP_TOP
    
-   542         622 LOAD_NAME               26 (button)
+   576         622 LOAD_NAME               26 (button)
                624 LOAD_METHOD             28 (pack)
                646 LOAD_CONST              43 ('x')
                648 LOAD_CONST              44 (5)
                650 LOAD_CONST              44 (5)
                652 KW_NAMES                45
                654 PRECALL                  3
                658 CALL                     3
                668 POP_TOP
    
-   544         670 PUSH_NULL
+   578         670 PUSH_NULL
                672 LOAD_NAME               10 (AdwDrawRoundButton)
                674 LOAD_CONST              39 ('Hello')
                676 KW_NAMES                40
                678 PRECALL                  1
                682 CALL                     1
                692 STORE_NAME              29 (button4)
    
-   545         694 LOAD_NAME               29 (button4)
+   579         694 LOAD_NAME               29 (button4)
                696 LOAD_METHOD             27 (bind)
                718 LOAD_CONST              41 ('<<Click>>')
-               720 LOAD_CONST              46 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 545>)
+               720 LOAD_CONST              46 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 579>)
                722 MAKE_FUNCTION            0
                724 PRECALL                  2
                728 CALL                     2
                738 POP_TOP
    
-   546         740 LOAD_NAME               29 (button4)
+   580         740 LOAD_NAME               29 (button4)
                742 LOAD_METHOD             28 (pack)
                764 LOAD_CONST              43 ('x')
                766 LOAD_CONST              44 (5)
                768 LOAD_CONST              44 (5)
                770 KW_NAMES                45
                772 PRECALL                  3
                776 CALL                     3
                786 POP_TOP
    
-   548         788 PUSH_NULL
+   582         788 PUSH_NULL
                790 LOAD_NAME               13 (AdwDrawRoundButton2)
                792 LOAD_CONST              39 ('Hello')
                794 KW_NAMES                40
                796 PRECALL                  1
                800 CALL                     1
                810 STORE_NAME              30 (button7)
    
-   549         812 LOAD_NAME               30 (button7)
+   583         812 LOAD_NAME               30 (button7)
                814 LOAD_METHOD             27 (bind)
                836 LOAD_CONST              41 ('<<Click>>')
-               838 LOAD_CONST              47 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 549>)
+               838 LOAD_CONST              47 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 583>)
                840 MAKE_FUNCTION            0
                842 PRECALL                  2
                846 CALL                     2
                856 POP_TOP
    
-   550         858 LOAD_NAME               30 (button7)
+   584         858 LOAD_NAME               30 (button7)
                860 LOAD_METHOD             28 (pack)
                882 LOAD_CONST              43 ('x')
                884 LOAD_CONST              44 (5)
                886 LOAD_CONST              44 (5)
                888 KW_NAMES                45
                890 PRECALL                  3
                894 CALL                     3
                904 POP_TOP
    
-   552         906 PUSH_NULL
+   586         906 PUSH_NULL
                908 LOAD_NAME               16 (AdwDrawRoundButton3)
                910 LOAD_CONST              39 ('Hello')
                912 KW_NAMES                40
                914 PRECALL                  1
                918 CALL                     1
                928 STORE_NAME              31 (button10)
    
-   553         930 LOAD_NAME               31 (button10)
+   587         930 LOAD_NAME               31 (button10)
                932 LOAD_METHOD             27 (bind)
                954 LOAD_CONST              41 ('<<Click>>')
-               956 LOAD_CONST              48 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 553>)
+               956 LOAD_CONST              48 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 587>)
                958 MAKE_FUNCTION            0
                960 PRECALL                  2
                964 CALL                     2
                974 POP_TOP
    
-   554         976 LOAD_NAME               31 (button10)
+   588         976 LOAD_NAME               31 (button10)
                978 LOAD_METHOD             28 (pack)
               1000 LOAD_CONST              43 ('x')
               1002 LOAD_CONST              44 (5)
               1004 LOAD_CONST              44 (5)
               1006 KW_NAMES                45
               1008 PRECALL                  3
               1012 CALL                     3
               1022 POP_TOP
    
-   556        1024 PUSH_NULL
+   590        1024 PUSH_NULL
               1026 LOAD_NAME               20 (AdwDrawCircularButton)
               1028 LOAD_CONST              39 ('Hello')
               1030 KW_NAMES                40
               1032 PRECALL                  1
               1036 CALL                     1
               1046 STORE_NAME              32 (button13)
    
-   557        1048 LOAD_NAME               32 (button13)
+   591        1048 LOAD_NAME               32 (button13)
               1050 LOAD_METHOD             27 (bind)
               1072 LOAD_CONST              41 ('<<Click>>')
-              1074 LOAD_CONST              49 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 557>)
+              1074 LOAD_CONST              49 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 591>)
               1076 MAKE_FUNCTION            0
               1078 PRECALL                  2
               1082 CALL                     2
               1092 POP_TOP
    
-   558        1094 LOAD_NAME               32 (button13)
+   592        1094 LOAD_NAME               32 (button13)
               1096 LOAD_METHOD             28 (pack)
               1118 LOAD_CONST              43 ('x')
               1120 LOAD_CONST              44 (5)
               1122 LOAD_CONST              44 (5)
               1124 KW_NAMES                45
               1126 PRECALL                  3
               1130 CALL                     3
               1140 POP_TOP
    
-   560        1142 LOAD_NAME               25 (root)
+   594        1142 LOAD_NAME               25 (root)
               1144 LOAD_METHOD             33 (mainloop)
               1166 PRECALL                  0
               1170 CALL                     0
               1180 POP_TOP
               1182 LOAD_CONST              50 (None)
               1184 RETURN_VALUE
    
-   535     >> 1186 LOAD_CONST              50 (None)
+   569     >> 1186 LOAD_CONST              50 (None)
               1188 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
       ('AdwWidget',)
       code
          argcount  : 0
@@ -3067,128 +3067,133 @@
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab01000000000000000001007c00a0010000000000000000000000
-                  0000000000000000007c006a0200000000000000007c006a020000000000
-                  0000007c00a0030000000000000000000000000000000000000000a60000
-                  00ab0000000000000000007c006a0200000000000000007a0a00007c00a0
-                  040000000000000000000000000000000000000000a6000000ab00000000
-                  00000000007c006a0200000000000000007a0a00007c006a050000000000
-                  0000007c006a0200000000000000007c006a0600000000000000007c006a
-                  070000000000000000ac02a6080000ab080000000000000000010064037c
-                  005f0800000000000000007c00a009000000000000000000000000000000
-                  00000000007c00a0030000000000000000000000000000000000000000a6
-                  000000ab00000000000000000064047a0b00007c00a00400000000000000
-                  00000000000000000000000000a6000000ab00000000000000000064047a
-                  0b00007c006a0a00000000000000007c006a0b00000000000000007c006a
-                  0c0000000000000000ac05a6050000ab0500000000000000007c005f0d00
-                  0000000000000064005300
+                  0000000000000000007c006a02000000000000000064027a0a00007c006a
+                  02000000000000000064027a0a00007c00a0030000000000000000000000
+                  000000000000000000a6000000ab0000000000000000007c006a02000000
+                  00000000007a0a00007c00a0040000000000000000000000000000000000
+                  000000a6000000ab0000000000000000007c006a0200000000000000007a
+                  0a00007c006a0500000000000000007c006a0200000000000000007c006a
+                  0600000000000000007c006a070000000000000000ac03a6080000ab0800
+                  00000000000000010064047c005f0800000000000000007c00a009000000
+                  00000000000000000000000000000000007c00a003000000000000000000
+                  0000000000000000000000a6000000ab00000000000000000064057a0b00
+                  007c00a0040000000000000000000000000000000000000000a6000000ab
+                  00000000000000000064057a0b00007c006a0a00000000000000007c006a
+                  0b00000000000000007c006a0c0000000000000000ac06a6050000ab0500
+                  000000000000007c005f0d000000000000000064005300
                442           0 RESUME                   0
                
                443           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
                446          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
                447          68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                2 (_button_border_width)
-                            80 LOAD_FAST                0 (self)
-                            82 LOAD_ATTR                2 (_button_border_width)
+                            80 LOAD_CONST               2 (1)
+                            82 BINARY_OP               10 (-)
+                            86 LOAD_FAST                0 (self)
+                            88 LOAD_ATTR                2 (_button_border_width)
+                            98 LOAD_CONST               2 (1)
+                           100 BINARY_OP               10 (-)
                
-               448          92 LOAD_FAST                0 (self)
-                            94 LOAD_METHOD              3 (winfo_width)
-                           116 PRECALL                  0
-                           120 CALL                     0
-                           130 LOAD_FAST                0 (self)
-                           132 LOAD_ATTR                2 (_button_border_width)
-                           142 BINARY_OP               10 (-)
-               
-               449         146 LOAD_FAST                0 (self)
-                           148 LOAD_METHOD              4 (winfo_height)
-                           170 PRECALL                  0
-                           174 CALL                     0
-                           184 LOAD_FAST                0 (self)
-                           186 LOAD_ATTR                2 (_button_border_width)
-                           196 BINARY_OP               10 (-)
+               448         104 LOAD_FAST                0 (self)
+                           106 LOAD_METHOD              3 (winfo_width)
+                           128 PRECALL                  0
+                           132 CALL                     0
+                           142 LOAD_FAST                0 (self)
+                           144 LOAD_ATTR                2 (_button_border_width)
+                           154 BINARY_OP               10 (-)
                
-               450         200 LOAD_FAST                0 (self)
-                           202 LOAD_ATTR                5 (button_radius)
+               449         158 LOAD_FAST                0 (self)
+                           160 LOAD_METHOD              4 (winfo_height)
+                           182 PRECALL                  0
+                           186 CALL                     0
+                           196 LOAD_FAST                0 (self)
+                           198 LOAD_ATTR                2 (_button_border_width)
+                           208 BINARY_OP               10 (-)
                
-               451         212 LOAD_FAST                0 (self)
-                           214 LOAD_ATTR                2 (_button_border_width)
+               450         212 LOAD_FAST                0 (self)
+                           214 LOAD_ATTR                5 (button_radius)
                
-               452         224 LOAD_FAST                0 (self)
-                           226 LOAD_ATTR                6 (_button_border)
-                           236 LOAD_FAST                0 (self)
-                           238 LOAD_ATTR                7 (_button_back)
+               451         224 LOAD_FAST                0 (self)
+                           226 LOAD_ATTR                2 (_button_border_width)
                
-               446         248 KW_NAMES                 2
-                           250 PRECALL                  8
-                           254 CALL                     8
-                           264 POP_TOP
-               
-               455         266 LOAD_CONST               3 ('button_frame')
-                           268 LOAD_FAST                0 (self)
-                           270 STORE_ATTR               8 (button_frame)
-               
-               458         280 LOAD_FAST                0 (self)
-                           282 LOAD_METHOD              9 (create_text)
-               
-               459         304 LOAD_FAST                0 (self)
-                           306 LOAD_METHOD              3 (winfo_width)
-                           328 PRECALL                  0
-                           332 CALL                     0
-                           342 LOAD_CONST               4 (2)
-                           344 BINARY_OP               11 (/)
-                           348 LOAD_FAST                0 (self)
-                           350 LOAD_METHOD              4 (winfo_height)
-                           372 PRECALL                  0
-                           376 CALL                     0
-                           386 LOAD_CONST               4 (2)
-                           388 BINARY_OP               11 (/)
-               
-               460         392 LOAD_FAST                0 (self)
-                           394 LOAD_ATTR               10 (text)
-                           404 LOAD_FAST                0 (self)
-                           406 LOAD_ATTR               11 (_button_text_back)
-               
-               461         416 LOAD_FAST                0 (self)
-                           418 LOAD_ATTR               12 (button_text_font)
-               
-               458         428 KW_NAMES                 5
-                           430 PRECALL                  5
-                           434 CALL                     5
-                           444 LOAD_FAST                0 (self)
-                           446 STORE_ATTR              13 (button_text)
-                           456 LOAD_CONST               0 (None)
-                           458 RETURN_VALUE
+               452         236 LOAD_FAST                0 (self)
+                           238 LOAD_ATTR                6 (_button_border)
+                           248 LOAD_FAST                0 (self)
+                           250 LOAD_ATTR                7 (_button_back)
+               
+               446         260 KW_NAMES                 3
+                           262 PRECALL                  8
+                           266 CALL                     8
+                           276 POP_TOP
+               
+               455         278 LOAD_CONST               4 ('button_frame')
+                           280 LOAD_FAST                0 (self)
+                           282 STORE_ATTR               8 (button_frame)
+               
+               458         292 LOAD_FAST                0 (self)
+                           294 LOAD_METHOD              9 (create_text)
+               
+               459         316 LOAD_FAST                0 (self)
+                           318 LOAD_METHOD              3 (winfo_width)
+                           340 PRECALL                  0
+                           344 CALL                     0
+                           354 LOAD_CONST               5 (2)
+                           356 BINARY_OP               11 (/)
+                           360 LOAD_FAST                0 (self)
+                           362 LOAD_METHOD              4 (winfo_height)
+                           384 PRECALL                  0
+                           388 CALL                     0
+                           398 LOAD_CONST               5 (2)
+                           400 BINARY_OP               11 (/)
+               
+               460         404 LOAD_FAST                0 (self)
+                           406 LOAD_ATTR               10 (text)
+                           416 LOAD_FAST                0 (self)
+                           418 LOAD_ATTR               11 (_button_text_back)
+               
+               461         428 LOAD_FAST                0 (self)
+                           430 LOAD_ATTR               12 (button_text_font)
+               
+               458         440 KW_NAMES                 6
+                           442 PRECALL                  5
+                           446 CALL                     5
+                           456 LOAD_FAST                0 (self)
+                           458 STORE_ATTR              13 (button_text)
+                           468 LOAD_CONST               0 (None)
+                           470 RETURN_VALUE
                consts
                   None
                   'all'
+                  1
                   ('width', 'outline', 'fill')
                   'button_frame'
                   2
                   ('text', 'fill', 'font')
                names      ('delete', 'create_round_rect4', '_button_border_width', 'winfo_width', 'winfo_height', 'button_radius', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_draw'
                firstlineno 442
                lnotab
-                  0x02012a0318011801360136010c010c0118fa12090e031801580118010c
+                  0x02012a0318012401360136010c010c0118fa12090e031801580118010c
                   fd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
@@ -3464,15 +3469,15 @@
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '__init__'
                firstlineno 504
                lnotab 0x0401
             code
                argcount  : 2
-               nlocals   : 2
+               nlocals   : 3
                stacksize : 9
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
                   010000ab01000000000000000001007c00a0010000000000000000000000
                   000000000000000000640264027c00a00200000000000000000000000000
                   00000000000000a6000000ab00000000000000000064037a0a00007c00a0
@@ -3481,15 +3486,15 @@
                   00000000007c006a060000000000000000ac04a6070000ab070000000000
                   0000007c005f0700000000000000007c00a0080000000000000000000000
                   0000000000000000007c00a0020000000000000000000000000000000000
                   000000a6000000ab00000000000000000064057a0b00007c00a003000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0064057a0b00007c006a0900000000000000007c006a0a00000000000000
                   007c006a0b0000000000000000ac06a6050000ab0500000000000000007c
-                  005f0c000000000000000064005300
+                  005f0c00000000000000006408640784017d0264005300
                507           0 RESUME                   0
                
                508           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
@@ -3552,32 +3557,286 @@
                            362 LOAD_ATTR               11 (button_text_font)
                
                518         372 KW_NAMES                 6
                            374 PRECALL                  5
                            378 CALL                     5
                            388 LOAD_FAST                0 (self)
                            390 STORE_ATTR              12 (button_text)
-                           400 LOAD_CONST               0 (None)
-                           402 RETURN_VALUE
+               
+               524         400 LOAD_CONST               8 ((None,))
+                           402 LOAD_CONST               7 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 524>)
+                           404 MAKE_FUNCTION            1 (defaults)
+                           406 STORE_FAST               2 (palette)
+                           408 LOAD_CONST               0 (None)
+                           410 RETURN_VALUE
                consts
                   None
                   'all'
                   1.5
                   3
                   ('width', 'outline', 'fill')
                   2
                   ('text', 'fill', 'font')
+                  code
+                     argcount  : 2
+                     nlocals   : 2
+                     stacksize : 4
+                     flags     : 19
+                     code
+                        0x97007c019001818d64017c017600900172287c01640119000000000000
+                        0000006402190000000000000000007c005f0000000000000000007c0164
+                        01190000000000000000006403190000000000000000007c005f01000000
+                        00000000007c016401190000000000000000006404190000000000000000
+                        007c005f0200000000000000007c01640119000000000000000000640519
+                        0000000000000000007c005f03000000000000000064067c016401190000
+                        00000000000000760072647c016401190000000000000000006406190000
+                        000000000000006402190000000000000000007c005f0400000000000000
+                        007c01640119000000000000000000640619000000000000000000640319
+                        0000000000000000007c005f0500000000000000007c0164011900000000
+                        00000000006406190000000000000000006404190000000000000000007c
+                        005f0600000000000000007c016401190000000000000000006406190000
+                        000000000000006405190000000000000000007c005f0700000000000000
+                        0064077c01640119000000000000000000760072647c0164011900000000
+                        00000000006407190000000000000000006402190000000000000000007c
+                        005f0800000000000000007c016401190000000000000000006407190000
+                        000000000000006403190000000000000000007c005f0900000000000000
+                        007c01640119000000000000000000640719000000000000000000640419
+                        0000000000000000007c005f0a00000000000000007c0164011900000000
+                        00000000006407190000000000000000006405190000000000000000007c
+                        005f0b00000000000000007c017c005f0c00000000000000007c006a0000
+                        000000000000007c005f0d00000000000000007c006a0100000000000000
+                        007c005f0e00000000000000007c006a0300000000000000007c005f0f00
+                        000000000000007c006a0200000000000000007c005f1000000000000000
+                        0009007c00a01100000000000000000000000000000000000000006400a6
+                        010000ab0100000000000000000100640053002300742400000000000000
+                        00000024007204010059006400530077007803590077017c006a0c000000
+                        00000000005300
+                     524           0 RESUME                   0
+                     
+                     525           2 LOAD_FAST                1 (dict)
+                                   4 EXTENDED_ARG             1
+                                   6 POP_JUMP_FORWARD_IF_NONE   397 (to 802)
+                     
+                     526           8 LOAD_CONST               1 ('circular_button')
+                                  10 LOAD_FAST                1 (dict)
+                                  12 CONTAINS_OP              0
+                                  14 EXTENDED_ARG             1
+                                  16 POP_JUMP_FORWARD_IF_FALSE   296 (to 610)
+                     
+                     527          18 LOAD_FAST                1 (dict)
+                                  20 LOAD_CONST               1 ('circular_button')
+                                  22 BINARY_SUBSCR
+                                  32 LOAD_CONST               2 ('back')
+                                  34 BINARY_SUBSCR
+                                  44 LOAD_FAST                0 (self)
+                                  46 STORE_ATTR               0 (button_back)
+                     
+                     528          56 LOAD_FAST                1 (dict)
+                                  58 LOAD_CONST               1 ('circular_button')
+                                  60 BINARY_SUBSCR
+                                  70 LOAD_CONST               3 ('border')
+                                  72 BINARY_SUBSCR
+                                  82 LOAD_FAST                0 (self)
+                                  84 STORE_ATTR               1 (button_border)
+                     
+                     529          94 LOAD_FAST                1 (dict)
+                                  96 LOAD_CONST               1 ('circular_button')
+                                  98 BINARY_SUBSCR
+                                 108 LOAD_CONST               4 ('text_back')
+                                 110 BINARY_SUBSCR
+                                 120 LOAD_FAST                0 (self)
+                                 122 STORE_ATTR               2 (button_text_back)
+                     
+                     530         132 LOAD_FAST                1 (dict)
+                                 134 LOAD_CONST               1 ('circular_button')
+                                 136 BINARY_SUBSCR
+                                 146 LOAD_CONST               5 ('border_width')
+                                 148 BINARY_SUBSCR
+                                 158 LOAD_FAST                0 (self)
+                                 160 STORE_ATTR               3 (button_border_width)
+                     
+                     532         170 LOAD_CONST               6 ('active')
+                                 172 LOAD_FAST                1 (dict)
+                                 174 LOAD_CONST               1 ('circular_button')
+                                 176 BINARY_SUBSCR
+                                 186 CONTAINS_OP              0
+                                 188 POP_JUMP_FORWARD_IF_FALSE   100 (to 390)
+                     
+                     533         190 LOAD_FAST                1 (dict)
+                                 192 LOAD_CONST               1 ('circular_button')
+                                 194 BINARY_SUBSCR
+                                 204 LOAD_CONST               6 ('active')
+                                 206 BINARY_SUBSCR
+                                 216 LOAD_CONST               2 ('back')
+                                 218 BINARY_SUBSCR
+                                 228 LOAD_FAST                0 (self)
+                                 230 STORE_ATTR               4 (button_active_back)
+                     
+                     534         240 LOAD_FAST                1 (dict)
+                                 242 LOAD_CONST               1 ('circular_button')
+                                 244 BINARY_SUBSCR
+                                 254 LOAD_CONST               6 ('active')
+                                 256 BINARY_SUBSCR
+                                 266 LOAD_CONST               3 ('border')
+                                 268 BINARY_SUBSCR
+                                 278 LOAD_FAST                0 (self)
+                                 280 STORE_ATTR               5 (button_active_border)
+                     
+                     535         290 LOAD_FAST                1 (dict)
+                                 292 LOAD_CONST               1 ('circular_button')
+                                 294 BINARY_SUBSCR
+                                 304 LOAD_CONST               6 ('active')
+                                 306 BINARY_SUBSCR
+                                 316 LOAD_CONST               4 ('text_back')
+                                 318 BINARY_SUBSCR
+                                 328 LOAD_FAST                0 (self)
+                                 330 STORE_ATTR               6 (button_active_text_back)
+                     
+                     536         340 LOAD_FAST                1 (dict)
+                                 342 LOAD_CONST               1 ('circular_button')
+                                 344 BINARY_SUBSCR
+                                 354 LOAD_CONST               6 ('active')
+                                 356 BINARY_SUBSCR
+                                 366 LOAD_CONST               5 ('border_width')
+                                 368 BINARY_SUBSCR
+                                 378 LOAD_FAST                0 (self)
+                                 380 STORE_ATTR               7 (button_active_border_width)
+                     
+                     538     >>  390 LOAD_CONST               7 ('pressed')
+                                 392 LOAD_FAST                1 (dict)
+                                 394 LOAD_CONST               1 ('circular_button')
+                                 396 BINARY_SUBSCR
+                                 406 CONTAINS_OP              0
+                                 408 POP_JUMP_FORWARD_IF_FALSE   100 (to 610)
+                     
+                     539         410 LOAD_FAST                1 (dict)
+                                 412 LOAD_CONST               1 ('circular_button')
+                                 414 BINARY_SUBSCR
+                                 424 LOAD_CONST               7 ('pressed')
+                                 426 BINARY_SUBSCR
+                                 436 LOAD_CONST               2 ('back')
+                                 438 BINARY_SUBSCR
+                                 448 LOAD_FAST                0 (self)
+                                 450 STORE_ATTR               8 (button_pressed_back)
+                     
+                     540         460 LOAD_FAST                1 (dict)
+                                 462 LOAD_CONST               1 ('circular_button')
+                                 464 BINARY_SUBSCR
+                                 474 LOAD_CONST               7 ('pressed')
+                                 476 BINARY_SUBSCR
+                                 486 LOAD_CONST               3 ('border')
+                                 488 BINARY_SUBSCR
+                                 498 LOAD_FAST                0 (self)
+                                 500 STORE_ATTR               9 (button_pressed_border)
+                     
+                     541         510 LOAD_FAST                1 (dict)
+                                 512 LOAD_CONST               1 ('circular_button')
+                                 514 BINARY_SUBSCR
+                                 524 LOAD_CONST               7 ('pressed')
+                                 526 BINARY_SUBSCR
+                                 536 LOAD_CONST               4 ('text_back')
+                                 538 BINARY_SUBSCR
+                                 548 LOAD_FAST                0 (self)
+                                 550 STORE_ATTR              10 (button_pressed_text_back)
+                     
+                     542         560 LOAD_FAST                1 (dict)
+                                 562 LOAD_CONST               1 ('circular_button')
+                                 564 BINARY_SUBSCR
+                                 574 LOAD_CONST               7 ('pressed')
+                                 576 BINARY_SUBSCR
+                                 586 LOAD_CONST               5 ('border_width')
+                                 588 BINARY_SUBSCR
+                                 598 LOAD_FAST                0 (self)
+                                 600 STORE_ATTR              11 (button_pressed_border_width)
+                     
+                     544     >>  610 LOAD_FAST                1 (dict)
+                                 612 LOAD_FAST                0 (self)
+                                 614 STORE_ATTR              12 (_palette)
+                     
+                     546         624 LOAD_FAST                0 (self)
+                                 626 LOAD_ATTR                0 (button_back)
+                                 636 LOAD_FAST                0 (self)
+                                 638 STORE_ATTR              13 (_button_back)
+                     
+                     547         648 LOAD_FAST                0 (self)
+                                 650 LOAD_ATTR                1 (button_border)
+                                 660 LOAD_FAST                0 (self)
+                                 662 STORE_ATTR              14 (_button_border)
+                     
+                     548         672 LOAD_FAST                0 (self)
+                                 674 LOAD_ATTR                3 (button_border_width)
+                                 684 LOAD_FAST                0 (self)
+                                 686 STORE_ATTR              15 (_button_border_width)
+                     
+                     549         696 LOAD_FAST                0 (self)
+                                 698 LOAD_ATTR                2 (button_text_back)
+                                 708 LOAD_FAST                0 (self)
+                                 710 STORE_ATTR              16 (_button_text_back)
+                     
+                     551         720 NOP
+                     
+                     552         722 LOAD_FAST                0 (self)
+                                 724 LOAD_METHOD             17 (_draw)
+                                 746 LOAD_CONST               0 (None)
+                                 748 PRECALL                  1
+                                 752 CALL                     1
+                                 762 POP_TOP
+                                 764 LOAD_CONST               0 (None)
+                                 766 RETURN_VALUE
+                             >>  768 PUSH_EXC_INFO
+                     
+                     553         770 LOAD_GLOBAL             36 (AttributeError)
+                                 782 CHECK_EXC_MATCH
+                                 784 POP_JUMP_FORWARD_IF_FALSE     4 (to 794)
+                                 786 POP_TOP
+                     
+                     554         788 POP_EXCEPT
+                                 790 LOAD_CONST               0 (None)
+                                 792 RETURN_VALUE
+                     
+                     553     >>  794 RERAISE                  0
+                             >>  796 COPY                     3
+                                 798 POP_EXCEPT
+                                 800 RERAISE                  1
+                     
+                     556     >>  802 LOAD_FAST                0 (self)
+                                 804 LOAD_ATTR               12 (_palette)
+                                 814 RETURN_VALUE
+                     ExceptionTable:
+                       722 to 762 -> 768 [0]
+                       768 to 786 -> 796 [1] lasti
+                       794 to 794 -> 796 [1] lasti
+                     consts
+                        None
+                        'circular_button'
+                        'back'
+                        'border'
+                        'text_back'
+                        'border_width'
+                        'active'
+                        'pressed'
+                     names      ('button_back', 'button_border', 'button_text_back', 'button_border_width', 'button_active_back', 'button_active_border', 'button_active_text_back', 'button_active_border_width', 'button_pressed_back', 'button_pressed_border', 'button_pressed_text_back', 'button_pressed_border_width', '_palette', '_button_back', '_button_border', '_button_border_width', '_button_text_back', '_draw', 'AttributeError')
+                     varnames   ('self', 'dict')
+                     freevars   ()
+                     cellvars   ()
+                     filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
+                     name       'palette'
+                     firstlineno 524
+                     lnotab
+                        0x020106010a012601260126012602140132013201320132021401320132
+                        01320132020e02180118011801180202013001120106ff0803
+                  (None,)
                names      ('delete', 'create_oval', 'winfo_width', 'winfo_height', 'button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
-               varnames   ('self', 'evt')
+               varnames   ('self', 'evt', 'palette')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_draw'
                firstlineno 507
-               lnotab 0x02012a0318015c010c0118fd1c071801580118010cfd
+               lnotab 0x02012a0318015c010c0118fd1c071801580118010cfd1c06
          names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawBasicCircularButton'
          firstlineno 503
@@ -3585,118 +3844,118 @@
       'AdwDrawBasicCircularButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         525           0 RESUME                   0
+         559           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawCircularButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         526          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 526>)
+         560          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 560>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawCircularButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               526           0 RESUME                   0
+               560           0 RESUME                   0
                
-               527           2 LOAD_FAST                0 (self)
+               561           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 526
+               firstlineno 560
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawCircularButton'
-         firstlineno 525
+         firstlineno 559
          lnotab 0x0a01
       'AdwDrawCircularButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         530           0 RESUME                   0
+         564           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawCircularDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         531          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 531>)
+         565          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 565>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawCircularDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               531           0 RESUME                   0
+               565           0 RESUME                   0
                
-               532           2 LOAD_FAST                0 (self)
+               566           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 531
+               firstlineno 565
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawCircularDarkButton'
-         firstlineno 530
+         firstlineno 564
          lnotab 0x0a01
       'AdwDrawCircularDarkButton'
       '__main__'
       ('Tk',)
       'Hello'
       ('text',)
       '<<Click>>'
@@ -3704,139 +3963,139 @@
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         541           0 RESUME                   0
+         575           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 541
+         firstlineno 575
          lnotab 0x
       'x'
       5
       ('fill', 'padx', 'pady')
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         545           0 RESUME                   0
+         579           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 545
+         firstlineno 579
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         549           0 RESUME                   0
+         583           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 549
+         firstlineno 583
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         553           0 RESUME                   0
+         587           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 553
+         firstlineno 587
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         557           0 RESUME                   0
+         591           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button6 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button6 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 557
+         firstlineno 591
          lnotab 0x
       None
    names      ('tkinter.font', 'Font', 'nametofont', 'tkadw.windows.canvas.widget', 'AdwWidget', 'AdwDrawBasicButton', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawBasicRoundButton', 'AdwDrawRoundButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawBasicCircularButton', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', '__name__', 'tkinter', 'Tk', 'root', 'button', 'bind', 'pack', 'button4', 'button7', 'button10', 'button13', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020110010c041c7f004d1c051c051c1d1c5a1c051c1d1c051c1d1c
-      1d1c051c1b1c1d1c061c161c051c050e010c02140218012e01300218012e
+      1d1c051c1b1c1d1c061c381c051c050e010c02140218012e01300218012e
       01300218012e01300218012e01300218012e0130022ce7
```

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xf956b364 (Sun Jul 16 02:33:29 2023 UTC)
+moddate:  0x5818bf64 (Tue Jul 25 00:33:28 2023 UTC)
 files sz: 7018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,80 +1,90 @@
 magic:    0xa70d0d0a
-moddate:  0xc73ab364 (Sun Jul 16 00:33:11 2023 UTC)
-files sz: 782
+moddate:  0xee37bf64 (Tue Jul 25 02:48:14 2023 UTC)
+files sz: 829
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 5
+   stacksize : 6
    flags     : 0
    code
-      0x9700640064016c006d015a010100020047006402840064036501a60300
-      00ab0300000000000000005a0264045300
+      0x9700640064016c006d015a010100640064026c026d035a030100020047
+      0064038400640465016503a6040000ab0400000000000000005a04640553
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('AdwDrawEngine',))
                  6 IMPORT_NAME              0 (tkadw.windows.canvas.drawengine)
                  8 IMPORT_FROM              1 (AdwDrawEngine)
                 10 STORE_NAME               1 (AdwDrawEngine)
                 12 POP_TOP
    
-     4          14 PUSH_NULL
-                16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               2 (<code object AdwWidget, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 4>)
-                20 MAKE_FUNCTION            0
-                22 LOAD_CONST               3 ('AdwWidget')
-                24 LOAD_NAME                1 (AdwDrawEngine)
-                26 PRECALL                  3
-                30 CALL                     3
-                40 STORE_NAME               2 (AdwWidget)
-                42 LOAD_CONST               4 (None)
-                44 RETURN_VALUE
+     2          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('AdwLayout',))
+                18 IMPORT_NAME              2 (tkadw.layout)
+                20 IMPORT_FROM              3 (AdwLayout)
+                22 STORE_NAME               3 (AdwLayout)
+                24 POP_TOP
+   
+     5          26 PUSH_NULL
+                28 LOAD_BUILD_CLASS
+                30 LOAD_CONST               3 (<code object AdwWidget, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 5>)
+                32 MAKE_FUNCTION            0
+                34 LOAD_CONST               4 ('AdwWidget')
+                36 LOAD_NAME                1 (AdwDrawEngine)
+                38 LOAD_NAME                3 (AdwLayout)
+                40 PRECALL                  4
+                44 CALL                     4
+                54 STORE_NAME               4 (AdwWidget)
+                56 LOAD_CONST               5 (None)
+                58 RETURN_VALUE
    consts
       0
       ('AdwDrawEngine',)
+      ('AdwLayout',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0388006601640284085a04640384
             005a056408880066016406840c5a066409640784015a07880078015a0853
             00
                        0 MAKE_CELL                0 (__class__)
          
-           4           2 RESUME                   0
+           5           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwWidget')
                       10 STORE_NAME               2 (__qualname__)
          
-           6          12 LOAD_CONST               1 ('\n    基础绘制组件类\n\n    特性：自动将背景颜色设为父组件背景颜色\n    ')
+           7          12 LOAD_CONST               1 ('\n    基础绘制组件类\n\n    特性：自动将背景颜色设为父组件背景颜色\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-          12          16 LOAD_CLOSURE             0 (__class__)
+          13          16 LOAD_CLOSURE             0 (__class__)
                       18 BUILD_TUPLE              1
-                      20 LOAD_CONST               2 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 12>)
+                      20 LOAD_CONST               2 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 13>)
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (__init__)
          
-          18          26 LOAD_CONST               3 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 18>)
+          19          26 LOAD_CONST               3 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 19>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               5 (_other)
          
-          24          32 LOAD_CONST               8 (('return', None))
+          25          32 LOAD_CONST               8 (('return', None))
                       34 LOAD_CLOSURE             0 (__class__)
                       36 BUILD_TUPLE              1
-                      38 LOAD_CONST               6 (<code object update, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 24>)
+                      38 LOAD_CONST               6 (<code object update, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 25>)
                       40 MAKE_FUNCTION           12 (annotations, closure)
                       42 STORE_NAME               6 (update)
          
-          28          44 LOAD_CONST               9 ((None,))
-                      46 LOAD_CONST               7 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 28>)
+          29          44 LOAD_CONST               9 ((None,))
+                      46 LOAD_CONST               7 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 29>)
                       48 MAKE_FUNCTION            1 (defaults)
                       50 STORE_NAME               7 (_draw)
                       52 LOAD_CLOSURE             0 (__class__)
                       54 COPY                     1
                       56 STORE_NAME               8 (__classcell__)
                       58 RETURN_VALUE
          consts
@@ -90,40 +100,40 @@
                   0000006a0100000000000000007c0169007c02a4018e0101007c00a00200
                   0000000000000000000000000000000000000064017c006a030000000000
                   0000006402ac03a6030000ab03000000000000000001007c00a004000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   00010064005300
                              0 COPY_FREE_VARS           1
                
-                12           2 RESUME                   0
+                13           2 RESUME                   0
                
-                13           4 PUSH_NULL
+                14           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
                             48 DICT_MERGE               1
                             50 CALL_FUNCTION_EX         1
                             52 POP_TOP
                
-                15          54 LOAD_FAST                0 (self)
+                16          54 LOAD_FAST                0 (self)
                             56 LOAD_METHOD              2 (bind)
                             78 LOAD_CONST               1 ('<Configure>')
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (_draw)
                             92 LOAD_CONST               2 ('+')
                             94 KW_NAMES                 3
                             96 PRECALL                  3
                            100 CALL                     3
                            110 POP_TOP
                
-                16         112 LOAD_FAST                0 (self)
+                17         112 LOAD_FAST                0 (self)
                            114 LOAD_METHOD              4 (_other)
                            136 PRECALL                  0
                            140 CALL                     0
                            150 POP_TOP
                            152 LOAD_CONST               0 (None)
                            154 RETURN_VALUE
                consts
@@ -133,15 +143,15 @@
                   ('add',)
                names      ('super', '__init__', 'bind', '_draw', '_other')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       '__init__'
-               firstlineno 12
+               firstlineno 13
                lnotab 0x040132023a01
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
@@ -149,42 +159,42 @@
                   0300000000000000006403a6020000ab02000000000000000072207c00a0
                   0400000000000000000000000000000000000000007c006a030000000000
                   0000006a050000000000000000ac04a6010000ab01000000000000000001
                   007c00a00400000000000000000000000000000000000000007c006a0300
                   00000000000000a006000000000000000000000000000000000000000064
                   05a6010000ab0100000000000000006401ac06a6020000ab020000000000
                   000000010064005300
-                18           0 RESUME                   0
+                19           0 RESUME                   0
                
-                19           2 LOAD_CONST               1 (0)
+                20           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('AdwDrawBasicFrame',))
                              6 IMPORT_NAME              0 (tkadw.windows.canvas.frame)
                              8 IMPORT_FROM              1 (AdwDrawBasicFrame)
                             10 STORE_FAST               1 (AdwDrawBasicFrame)
                             12 POP_TOP
                
-                20          14 LOAD_GLOBAL              5 (NULL + hasattr)
+                21          14 LOAD_GLOBAL              5 (NULL + hasattr)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                3 (master)
                             38 LOAD_CONST               3 ('frame_back')
                             40 PRECALL                  2
                             44 CALL                     2
                             54 POP_JUMP_FORWARD_IF_FALSE    32 (to 120)
                
-                21          56 LOAD_FAST                0 (self)
+                22          56 LOAD_FAST                0 (self)
                             58 LOAD_METHOD              4 (configure)
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (master)
                             92 LOAD_ATTR                5 (frame_back)
                            102 KW_NAMES                 4
                            104 PRECALL                  1
                            108 CALL                     1
                            118 POP_TOP
                
-                22     >>  120 LOAD_FAST                0 (self)
+                23     >>  120 LOAD_FAST                0 (self)
                            122 LOAD_METHOD              4 (configure)
                            144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                3 (master)
                            156 LOAD_METHOD              6 (cget)
                            178 LOAD_CONST               5 ('bg')
                            180 PRECALL                  1
                            184 CALL                     1
@@ -205,15 +215,15 @@
                   ('background', 'borderwidth')
                names      ('tkadw.windows.canvas.frame', 'AdwDrawBasicFrame', 'hasattr', 'master', 'configure', 'frame_back', 'cget')
                varnames   ('self', 'AdwDrawBasicFrame')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       '_other'
-               firstlineno 18
+               firstlineno 19
                lnotab 0x02010c012a014001
             'return'
             None
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -221,25 +231,25 @@
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a0010000000000000000000000000000000000000000a6000000ab0000
                   0000000000000001007c00a0020000000000000000000000000000000000
                   0000006400a6010000ab010000000000000000010064005300
                              0 COPY_FREE_VARS           1
                
-                24           2 RESUME                   0
+                25           2 RESUME                   0
                
-                25           4 LOAD_GLOBAL              1 (NULL + super)
+                26           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (update)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 POP_TOP
                
-                26          68 LOAD_FAST                0 (self)
+                27          68 LOAD_FAST                0 (self)
                             70 LOAD_METHOD              2 (_draw)
                             92 LOAD_CONST               0 (None)
                             94 PRECALL                  1
                             98 CALL                     1
                            108 POP_TOP
                            110 LOAD_CONST               0 (None)
                            112 RETURN_VALUE
@@ -247,49 +257,49 @@
                   None
                names      ('super', 'update', '_draw')
                varnames   ('self',)
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       'update'
-               firstlineno 24
+               firstlineno 25
                lnotab 0x04014001
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-                28           0 RESUME                   0
+                29           0 RESUME                   0
                
-                29           2 LOAD_CONST               0 (None)
+                30           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       '_draw'
-               firstlineno 28
+               firstlineno 29
                lnotab 0x0201
             ('return', None)
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '_other', 'update', '_draw', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
          name       'AdwWidget'
-         firstlineno 4
+         firstlineno 5
          lnotab 0x0c0204060a0606060c04
       'AdwWidget'
       None
-   names      ('tkadw.windows.canvas.drawengine', 'AdwDrawEngine', 'AdwWidget')
+   names      ('tkadw.windows.canvas.drawengine', 'AdwDrawEngine', 'tkadw.layout', 'AdwLayout', 'AdwWidget')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c03
+   lnotab 0x00ff02010c010c03
```

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/button.py` & `tkadw-0.3.5/tkadw/windows/canvas/button.py`

 * *Files 7% similar despite different names*

```diff
@@ -440,15 +440,15 @@
 
 class AdwDrawRoundButton3(AdwDrawBasicRoundButton):
     def _draw(self, evt):
         self.delete("all")
 
         # 绘制按钮边框
         self.create_round_rect4(
-            self._button_border_width, self._button_border_width,
+            self._button_border_width - 1, self._button_border_width - 1,
             self.winfo_width() - self._button_border_width,
             self.winfo_height() - self._button_border_width,
             self.button_radius,
             width=self._button_border_width,
             outline=self._button_border, fill=self._button_back,
         )
 
@@ -517,14 +517,48 @@
         # 绘制按钮文本
         self.button_text = self.create_text(
             self.winfo_width() / 2, self.winfo_height() / 2,
             text=self.text, fill=self._button_text_back,
             font=self.button_text_font
         )
 
+        def palette(self, dict=None):
+            if dict is not None:
+                if "circular_button" in dict:
+                    self.button_back = dict["circular_button"]["back"]
+                    self.button_border = dict["circular_button"]["border"]
+                    self.button_text_back = dict["circular_button"]["text_back"]
+                    self.button_border_width = dict["circular_button"]["border_width"]
+
+                    if "active" in dict["circular_button"]:
+                        self.button_active_back = dict["circular_button"]["active"]["back"]
+                        self.button_active_border = dict["circular_button"]["active"]["border"]
+                        self.button_active_text_back = dict["circular_button"]["active"]["text_back"]
+                        self.button_active_border_width = dict["circular_button"]["active"]["border_width"]
+
+                    if "pressed" in dict["circular_button"]:
+                        self.button_pressed_back = dict["circular_button"]["pressed"]["back"]
+                        self.button_pressed_border = dict["circular_button"]["pressed"]["border"]
+                        self.button_pressed_text_back = dict["circular_button"]["pressed"]["text_back"]
+                        self.button_pressed_border_width = dict["circular_button"]["pressed"]["border_width"]
+
+                self._palette = dict
+
+                self._button_back = self.button_back
+                self._button_border = self.button_border
+                self._button_border_width = self.button_border_width
+                self._button_text_back = self.button_text_back
+
+                try:
+                    self._draw(None)
+                except AttributeError:
+                    pass
+            else:
+                return self._palette
+
 
 class AdwDrawCircularButton(AdwDrawBasicCircularButton):
     def default_palette(self):
         self.palette_light()
 
 
 class AdwDrawCircularDarkButton(AdwDrawBasicCircularButton):
```

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/checkbox.py` & `tkadw-0.3.5/tkadw/windows/canvas/checkbox.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/drawengine.py` & `tkadw-0.3.5/tkadw/windows/canvas/drawengine.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/entry.py` & `tkadw-0.3.5/tkadw/windows/canvas/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/frame.py` & `tkadw-0.3.5/tkadw/windows/canvas/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/separator.py` & `tkadw-0.3.5/tkadw/windows/canvas/separator.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/textbox.py` & `tkadw-0.3.5/tkadw/windows/canvas/textbox.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/titlebar.py` & `tkadw-0.3.5/tkadw/windows/canvas/titlebar.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/canvas/widget.py` & `tkadw-0.3.5/tkadw/windows/canvas/widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from tkadw.windows.canvas.drawengine import AdwDrawEngine
+from tkadw.layout import AdwLayout
 
 
-class AdwWidget(AdwDrawEngine):
+class AdwWidget(AdwDrawEngine, AdwLayout):
 
     """
     基础绘制组件类
 
     特性：自动将背景颜色设为父组件背景颜色
     """
```

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/button.py` & `tkadw-0.3.5/tkadw/windows/fluent/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/entry.py` & `tkadw-0.3.5/tkadw/windows/fluent/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/frame.py` & `tkadw-0.3.5/tkadw/windows/fluent/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/GeneralSans-Regular.ttf` & `tkadw-0.3.5/tkadw/windows/fluent/GeneralSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/fluent/test.py` & `tkadw-0.3.5/tkadw/windows/fluent/test.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/theme.py` & `tkadw-0.3.5/tkadw/windows/theme.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,14 +26,35 @@
             "back": "#fafafa",
             "border": "#ebebeb",
             "text_back": "#202020",
             "border_width": 1,
         },
     },
 
+    "circular_button": {
+        "back": "#fdfdfd",
+        "border": "#ededed",
+        "text_back": "#202020",
+        "border_width": 1,
+
+        "active": {
+            "back": "#f9f9f9",
+            "border": "#d5d5d5",
+            "text_back": "#202020",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#fafafa",
+            "border": "#ebebeb",
+            "text_back": "#202020",
+            "border_width": 1,
+        },
+    },
+
     "frame": {
         "radius": 15,
         "back": "#fafafa",
         "border": "#e7e7e7",
         "border_width": 1,
         "padding": 0
     },
@@ -120,14 +141,35 @@
             "back": "#232323",
             "border": "#2c2c2c",
             "text_back": "#ebebeb",
             "border_width": 1,
         },
     },
 
+    "circular_button": {
+        "back": "#2a2a2a",
+        "border": "#313131",
+        "text_back": "#ebebeb",
+        "border_width": 1,
+
+        "active": {
+            "back": "#2f2f2f",
+            "border": "#313131",
+            "text_back": "#ebebeb",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#232323",
+            "border": "#2c2c2c",
+            "text_back": "#ebebeb",
+            "border_width": 1,
+        },
+    },
+
     "frame": {
         "radius": 15,
         "back": "#1c1c1c",
         "border": "#2f2f2f",
         "border_width": 1,
         "padding": 0
     },
@@ -214,14 +256,35 @@
             "back": "#dad6d2",
             "border": "#dad6d2",
             "text_back": "#2e3436",
             "border_width": 1.3,
         },
     },
 
+    "circular_button": {
+        "back": "#f6f5f4",
+        "border": "#ccc6c1",
+        "text_back": "#2e3436",
+        "border_width": 1.3,
+
+        "active": {
+            "back": "#f8f8f7",
+            "border": "#dad6d2",
+            "text_back": "#2e3436",
+            "border_width": 1.3,
+        },
+
+        "pressed": {
+            "back": "#dad6d2",
+            "border": "#dad6d2",
+            "text_back": "#2e3436",
+            "border_width": 1.3,
+        },
+    },
+
     "frame": {
         "radius": 0,
         "back": "#f6f5f4",
         "border": "#d5d0cc",
         "border_width": 1,
         "padding": 0
     },
@@ -308,14 +371,35 @@
             "back": "#1e1e1e",
             "border": "#282828",
             "text_back": "#eeeeec",
             "border_width": 1.3,
         },
     },
 
+    "circular_button": {
+        "back": "#353535",
+        "border": "#1b1b1b",
+        "text_back": "#eeeeec",
+        "border_width": 1.3,
+
+        "active": {
+            "back": "#373737",
+            "border": "#1b1b1b",
+            "text_back": "#eeeeec",
+            "border_width": 1.3,
+        },
+
+        "pressed": {
+            "back": "#1e1e1e",
+            "border": "#282828",
+            "text_back": "#eeeeec",
+            "border_width": 1.3,
+        },
+    },
+
     "frame": {
         "radius": 0,
         "back": "#313131",
         "border": "#1b1b1b",
         "border_width": 1,
         "padding": 0
     },
@@ -402,14 +486,35 @@
             "back": "#eceff0",
             "border": "#e3e5e7",
             "text_back": "#6d7479",
             "border_width": 1,
         },
     },
 
+    "circular_button": {
+        "back": "#ffffff",
+        "border": "#e3e5e7",
+        "text_back": "#18191c",
+        "border_width": 1,
+
+        "active": {
+            "back": "#e3e5e7",
+            "border": "#e3e5e7",
+            "text_back": "#18191c",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#eceff0",
+            "border": "#e3e5e7",
+            "text_back": "#6d7479",
+            "border_width": 1,
+        },
+    },
+
     "frame": {
         "radius": 18,
         "back": "#f6f7f8",
         "border": "#f1f2f3",
         "border_width": 1,
         "padding": 0
     },
@@ -496,14 +601,36 @@
             "back": "#26282a",
             "border": "#2f3134",
             "text_back": "#a9abad",
             "border_width": 1,
         },
     },
 
+    "circular_button": {
+        "radius": 16,
+        "back": "#242628",
+        "border": "#2f3134",
+        "text_back": "#dcdee0",
+        "border_width": 1,
+
+        "active": {
+            "back": "#2f3134",
+            "border": "#2f3134",
+            "text_back": "#dcdee0",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#26282a",
+            "border": "#2f3134",
+            "text_back": "#a9abad",
+            "border_width": 1,
+        },
+    },
+
     "frame": {
         "radius": 18,
         "back": "#1e2022",
         "border": "#232527",
         "border_width": 1,
         "padding": 0
     },
@@ -590,14 +717,35 @@
             "back": "#333333",
             "border": "#333333",
             "text_back": "#ffffff",
             "border_width": 1,
         },
     },
 
+    "circular_button": {
+        "back": "#eeeeee",
+        "border": "#cccccc",
+        "text_back": "#000000",
+        "border_width": 1,
+
+        "active": {
+            "back": "#666666",
+            "border": "#666666",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#333333",
+            "border": "#333333",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+    },
+
     "frame": {
         "radius": 0,
         "back": "#ffffff",
         "border": "#bfbfbf",
         "border_width": 1,
         "padding": 0
     },
@@ -659,15 +807,15 @@
 metro_dark_theme = {
     "window": {
         "back": "#111111"
     },
 
     "label": {
         "back": "transparent",
-        "text_back": "#000000",
+        "text_back": "#ffffff",
     },
 
     "button": {
         "radius": 0,
         "back": "#222222",
         "border": "#444444",
         "text_back": "#ffffff",
@@ -684,14 +832,35 @@
             "back": "#eeeeee",
             "border": "#eeeeee",
             "text_back": "#000000",
             "border_width": 1,
         },
     },
 
+    "circular_button": {
+        "back": "#222222",
+        "border": "#444444",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "active": {
+            "back": "#aaaaaa",
+            "border": "#aaaaaa",
+            "text_back": "#000000",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#eeeeee",
+            "border": "#eeeeee",
+            "text_back": "#000000",
+            "border_width": 1,
+        },
+    },
+
     "frame": {
         "radius": 0,
         "back": "#111111",
         "border": "#373737",
         "border_width": 1,
         "padding": 0
     },
@@ -778,14 +947,35 @@
             "back": "#dce9fc",
             "border": "#4e6d9c",
             "text_back": "#000000",
             "border_width": 2,
         },
     },
 
+    "circular_button": {
+        "back": "#ffffff",
+        "border": "#a0a0a0",
+        "text_back": "#000000",
+        "border_width": 1,
+
+        "active": {
+            "back": "#dce9fc",
+            "border": "#a0a0a0",
+            "text_back": "#000000",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#dce9fc",
+            "border": "#4e6d9c",
+            "text_back": "#000000",
+            "border_width": 2,
+        },
+    },
+
     "frame": {
         "radius": 0,
         "back": "#f0f0f0",
         "border": "#c8c8c8",
         "border_width": 1,
         "padding": 0
     },
@@ -851,15 +1041,35 @@
 
     "label": {
         "back": "transparent",
         "text_back": "#ffffff",
     },
 
     "button": {
-        "radius": 0,
+        "back": "#232323",
+        "border": "#4b4b4b",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "active": {
+            "back": "#373737",
+            "border": "#4b4b4b",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#373737",
+            "border": "#4e6d9c",
+            "text_back": "#ffffff",
+            "border_width": 2,
+        },
+    },
+
+    "circular_button": {
         "back": "#232323",
         "border": "#4b4b4b",
         "text_back": "#ffffff",
         "border_width": 1,
 
         "active": {
             "back": "#373737",
@@ -934,14 +1144,223 @@
         "back": "#464646",
         "border_width": 1,
 
         "rounded": False
     }
 }
 
+highlight_theme = {
+    "window": {
+        "back": "#000000"
+    },
+
+    "label": {
+        "back": "transparent",
+        "text_back": "#ffffff",
+    },
+
+    "button": {
+        "radius": 0,
+        "back": "#000000",
+        "border": "#ffffff",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "active": {
+            "back": "#000000",
+            "border": "#9A9A9A",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#000000",
+            "border": "#555555",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+    },
+
+    "circular_button": {
+        "back": "#000000",
+        "border": "#ffffff",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "active": {
+            "back": "#000000",
+            "border": "#9A9A9A",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#000000",
+            "border": "#555555",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+    },
+
+    "frame": {
+        "radius": 0,
+        "back": "#000000",
+        "border": "#ffffff",
+        "border_width": 1,
+        "padding": 0
+    },
+
+    "entry": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#000000",
+        "border": "#ffffff",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#000000",
+            "border": "#9A9A9A",
+            "text_back": "#ffffff",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "text": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#000000",
+        "border": "#ffffff",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#000000",
+            "border": "#9A9A9A",
+            "text_back": "#ffffff",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "separator": {
+        "back": "#ffffff",
+        "border_width": 1,
+
+        "rounded": False
+    }
+}
+
+uwp_dark_theme = {
+    "window": {
+        "back": "#212121"
+    },
+
+    "label": {
+        "back": "transparent",
+        "text_back": "#ffffff",
+    },
+
+    "button": {
+        "radius": 0,
+        "back": "#4c4c4c",
+        "border": "#ffffff",
+        "text_back": "#ffffff",
+        "border_width": 0,
+
+        "active": {
+            "back": "#000000",
+            "border": "#949494",
+            "text_back": "#ffffff",
+            "border_width": 2,
+        },
+
+        "pressed": {
+            "back": "#797979",
+            "border": "#555555",
+            "text_back": "#e2e2e2",
+            "border_width": 1,
+        },
+    },
+
+    "frame": {
+        "radius": 0,
+        "back": "#1f1f1f",
+        "border": "#ffffff",
+        "border_width": 1,
+        "padding": 0
+    },
+
+    "entry": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#000000",
+        "border": "#ffffff",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#000000",
+            "border": "#9A9A9A",
+            "text_back": "#ffffff",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "text": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#000000",
+        "border": "#ffffff",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#000000",
+            "border": "#9A9A9A",
+            "text_back": "#ffffff",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "separator": {
+        "back": "#ffffff",
+        "border_width": 1,
+
+        "rounded": False
+    }
+}
+
 
 def get_default_theme():
     from os import environ
     from json import loads
     try:
         return loads(environ["tkAdwite.DefaultTheme"])
     except KeyError:
@@ -1038,23 +1457,44 @@
 set_default_theme("win11")
 
 
 from tkadw.windows.widgets.adw import Adw
 
 
 class Adwite(Adw):
+    def __init__(self, default_theme="win11", *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.set_default_theme(default_theme)
+
     def set_default_theme(self, theme, _mode="auto"):
         set_default_theme(theme, _mode)
         for widget in self.winfo_children():
             if hasattr(widget, "palette"):
                 widget.palette(get_default_theme())
-                widget.configure(background=widget.master.cget("bg"))
                 widget.update()
         self.palette(get_default_theme())
 
+        from sys import platform
+        """
+        if platform == "win32":
+            from sys import platform
+            from ctypes import windll, byref, sizeof, c_int
+            from ctypes.wintypes import RGB
+            color = self.winfo_rgb(self.cget("bg"))
+            windll.dwmapi.DwmSetWindowAttribute(windll.user32.GetParent(self.winfo_id()), 35,
+                                                byref(c_int(RGB(color[0], color[1], color[2]))),
+                                                sizeof(c_int))
+        """
+
+    def use_win_mica(self, caption=None):
+        from win32mica import ApplyMica, MICAMODE
+        from ctypes import windll
+
+        ApplyMica(windll.user32.GetParent(root.winfo_id()), MICAMODE.DARK)
+
     def default_palette(self):
         self.palette(get_default_theme())
 
 
 from tkadw.windows.widgets import AdwLabel
 
 
@@ -1066,14 +1506,76 @@
 from tkadw.windows.canvas.button import AdwDrawRoundButton3
 
 
 class AdwTButton(AdwDrawRoundButton3):
     def default_palette(self):
         self.palette(get_default_theme())
 
+    def win11_accent_dark(self):
+        self.palette(
+            {
+                "button": {
+                    "radius": 13,
+                    "back": "#57c8ff",
+                    "border": "#64cdff",
+                    "text_back": "#1c1c1c",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#51b7eb",
+                        "border": "#5fbced",
+                        "text_back": "#1c1c1c",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#4ba6d5",
+                        "border": "#59aed9",
+                        "text_back": "#1c1c1c",
+                        "border_width": 1,
+                    },
+                }
+            }
+        )
+
+    def win11_accent_light(self):
+        self.palette(
+            {
+                "button": {
+                    "radius": 13,
+                    "back": "#0560b6",
+                    "border": "#1a6cba",
+                    "text_back": "#ebebeb",
+                    "border_width": 1,
+
+                    "active": {
+                        "back": "#1e6fbc",
+                        "border": "#307bc2",
+                        "text_back": "#ebebeb",
+                        "border_width": 1,
+                    },
+
+                    "pressed": {
+                        "back": "#327ec5",
+                        "border": "#4288ca",
+                        "text_back": "#ebebeb",
+                        "border_width": 1,
+                    },
+                }
+            }
+        )
+
+
+from tkadw.windows.canvas.button import AdwDrawCircularButton
+
+
+class AdwTCircularButton(AdwDrawCircularButton, AdwTButton):
+    def default_palette(self):
+        self.palette(get_default_theme())
+
 
 from tkadw.windows.canvas.entry import AdwDrawRoundEntry3
 
 
 class AdwTEntry(AdwDrawRoundEntry3):
     def default_palette(self):
         self.palette(get_default_theme())
@@ -1100,23 +1602,24 @@
 
 class AdwTSeparator(AdwDrawSeparator):
     def default_palette(self):
         self.palette(get_default_theme())
 
 
 if __name__ == '__main__':
-    from darkdetect import isDark
-
-    root = Adwite()
-    root.set_default_theme("win11", "dark")
+    root = Adwite(windark=True)
 
     button = AdwTButton(text="AdwTButton")
-    button.pack(fill="x", padx=5, pady=5)
+    button.win11_accent_dark()
+    button.row(padx=5, pady=5)
+    circular_button = AdwTCircularButton(text="AdwTCirculaButtorn")
+    circular_button.win11_accent_dark()
+    circular_button.row(padx=5, pady=5, fill="none")
     separator = AdwTSeparator()
-    separator.pack(fill="x", padx=5, pady=5)
+    separator.row(padx=5, pady=5)
     entry = AdwTEntry(text="AdwTEntry")
-    entry.pack(fill="x", padx=5, pady=5)
+    entry.row(padx=5, pady=5)
     text = AdwTText(text="AdwTText")
-    text.pack(fill="x", padx=5, pady=5)
+    text.row(padx=5, pady=5)
     frame = AdwTFrame()
-    frame.pack(fill="x", padx=5, pady=5)
+    frame.row(padx=5, pady=5)
     root.mainloop()
```

### Comparing `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x8f6bb264 (Sat Jul 15 09:49:03 2023 UTC)
-files sz: 20035
+moddate:  0x98c5b964 (Thu Jul 20 23:39:04 2023 UTC)
+files sz: 20069
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
@@ -62,28 +62,28 @@
                       32 BUILD_TUPLE              4
                       34 LOAD_CLOSURE             0 (__class__)
                       36 BUILD_TUPLE              1
                       38 LOAD_CONST               8 (<code object __init__, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 5>)
                       40 MAKE_FUNCTION           14 (kwdefaults, annotations, closure)
                       42 STORE_NAME               5 (__init__)
          
-          64          44 LOAD_CONST              14 (('#0a080a',))
-                      46 LOAD_CONST              10 (<code object custom, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 64>)
+          66          44 LOAD_CONST              14 (('#0a080a',))
+                      46 LOAD_CONST              10 (<code object custom, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 66>)
                       48 MAKE_FUNCTION            1 (defaults)
                       50 STORE_NAME               6 (custom)
          
-          82          52 LOAD_CONST              11 (<code object bind_move, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 82>)
+          84          52 LOAD_CONST              11 (<code object bind_move, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 84>)
                       54 MAKE_FUNCTION            0
                       56 STORE_NAME               7 (bind_move)
          
-          96          58 LOAD_CONST              12 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 96>)
+          98          58 LOAD_CONST              12 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 98>)
                       60 MAKE_FUNCTION            0
                       62 STORE_NAME               8 (default_palette)
          
-          99          64 LOAD_CONST              13 (<code object palette, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 99>)
+         101          64 LOAD_CONST              13 (<code object palette, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 101>)
                       66 MAKE_FUNCTION            0
                       68 STORE_NAME               9 (palette)
                       70 LOAD_CLOSURE             0 (__class__)
                       72 COPY                     1
                       74 STORE_NAME              10 (__classcell__)
                       76 RETURN_VALUE
          consts
@@ -123,36 +123,36 @@
                   0984087d10881a6601640a84087d117c02a00a0000000000000000000000
                   000000000000000000a6000000ab000000000000000000640b6b02000000
                   00720b02007c11a6000000ab0000000000000000007d026e227c02a00a00
                   00000000000000000000000000000000000000a6000000ab000000000000
                   000000640c6b0200000000720a02007c10a6000000ab0000000000000000
                   007d027c00a00b0000000000000000000000000000000000000000640d7c
                   02a6020000ab02000000000000000001007c00a00c000000000000000000
-                  0000000000000000000000a6000000ab0000000000000000000100640164
-                  0e6c0d6d0e7d1201007c12640f6b0200000000727d7c03727b0900640164
-                  106c0f6d107d136d117d146d127d156d137d166d147d17010002007c1664
-                  11a6010000ab0100000000000000007d187c136a150000000000000000a0
-                  1600000000000000000000000000000000000000007c136a170000000000
-                  000000a01800000000000000000000000000000000000000007c00a01900
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  000000a6010000ab010000000000000000641202007c157c18a6010000ab
-                  01000000000000000002007c177c18a6010000ab010000000000000000a6
-                  040000ab04000000000000000001006e072300010059006e037803590077
-                  017c12640f6b0200000000729b7c04819b6401640e6c0d6d0e7d12010064
-                  0164136c0f6d107d136d127d156d147d176d137d160100640164146c1a6d
-                  1b7d1901007c136a150000000000000000a0160000000000000000000000
-                  0000000000000000007c136a170000000000000000a01800000000000000
-                  000000000000000000000000007c00a01900000000000000000000000000
-                  00000000000000a6000000ab000000000000000000a6010000ab01000000
-                  0000000000641502007c1502007c1602007c197c04640119000000000000
-                  0000007c046411190000000000000000007c046416190000000000000000
-                  00a6030000ab030000000000000000a6010000ab010000000000000000a6
-                  010000ab01000000000000000002007c177c16a6010000ab010000000000
-                  000000a6040000ab04000000000000000001006400530064005300640053
-                  00
+                  0000000000000000000000a6000000ab00000000000000000001007c037c
+                  005f0d00000000000000006401640e6c0e6d0f7d1201007c12640f6b0200
+                  000000727d7c03727b0900640164106c106d117d136d127d146d137d156d
+                  147d166d157d17010002007c166411a6010000ab0100000000000000007d
+                  187c136a160000000000000000a017000000000000000000000000000000
+                  00000000007c136a180000000000000000a0190000000000000000000000
+                  0000000000000000007c00a01a0000000000000000000000000000000000
+                  000000a6000000ab000000000000000000a6010000ab0100000000000000
+                  00641202007c157c18a6010000ab01000000000000000002007c177c18a6
+                  010000ab010000000000000000a6040000ab04000000000000000001006e
+                  072300010059006e037803590077017c12640f6b0200000000729b7c0481
+                  9b6401640e6c0e6d0f7d120100640164136c106d117d136d137d156d157d
+                  176d147d160100640164146c1b6d1c7d1901007c136a1600000000000000
+                  00a01700000000000000000000000000000000000000007c136a18000000
+                  0000000000a01900000000000000000000000000000000000000007c00a0
+                  1a0000000000000000000000000000000000000000a6000000ab00000000
+                  0000000000a6010000ab010000000000000000641502007c1502007c1602
+                  007c197c046401190000000000000000007c046411190000000000000000
+                  007c04641619000000000000000000a6030000ab030000000000000000a6
+                  010000ab010000000000000000a6010000ab01000000000000000002007c
+                  177c16a6010000ab010000000000000000a6040000ab0400000000000000
+                  000100640053006400530064005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL               26 (adwite_dark_icon)
                              4 MAKE_CELL               27 (adwite_light_icon)
                
                  5           6 RESUME                   0
                
                  6           8 PUSH_NULL
@@ -360,188 +360,192 @@
                
                 42         766 LOAD_FAST                0 (self)
                            768 LOAD_METHOD             12 (default_palette)
                            790 PRECALL                  0
                            794 CALL                     0
                            804 POP_TOP
                
-                44         806 LOAD_CONST               1 (0)
-                           808 LOAD_CONST              14 (('platform',))
-                           810 IMPORT_NAME             13 (sys)
-                           812 IMPORT_FROM             14 (platform)
-                           814 STORE_FAST              18 (platform)
-                           816 POP_TOP
-               
-                45         818 LOAD_FAST               18 (platform)
-                           820 LOAD_CONST              15 ('win32')
-                           822 COMPARE_OP               2 (==)
-                           828 POP_JUMP_FORWARD_IF_FALSE   125 (to 1080)
-                           830 LOAD_FAST                3 (windark)
-                           832 POP_JUMP_FORWARD_IF_FALSE   123 (to 1080)
-               
-                46         834 NOP
-               
-                47         836 LOAD_CONST               1 (0)
-                           838 LOAD_CONST              16 (('windll', 'wintypes', 'byref', 'c_int', 'sizeof'))
-                           840 IMPORT_NAME             15 (ctypes)
-                           842 IMPORT_FROM             16 (windll)
-                           844 STORE_FAST              19 (windll)
-                           846 IMPORT_FROM             17 (wintypes)
-                           848 STORE_FAST              20 (wintypes)
-                           850 IMPORT_FROM             18 (byref)
-                           852 STORE_FAST              21 (byref)
-                           854 IMPORT_FROM             19 (c_int)
-                           856 STORE_FAST              22 (c_int)
-                           858 IMPORT_FROM             20 (sizeof)
-                           860 STORE_FAST              23 (sizeof)
-                           862 POP_TOP
-               
-                48         864 PUSH_NULL
-                           866 LOAD_FAST               22 (c_int)
-                           868 LOAD_CONST              17 (1)
-                           870 PRECALL                  1
-                           874 CALL                     1
-                           884 STORE_FAST              24 (value)
-               
-                49         886 LOAD_FAST               19 (windll)
-                           888 LOAD_ATTR               21 (dwmapi)
-                           898 LOAD_METHOD             22 (DwmSetWindowAttribute)
-               
-                50         920 LOAD_FAST               19 (windll)
-                           922 LOAD_ATTR               23 (user32)
-                           932 LOAD_METHOD             24 (GetParent)
-                           954 LOAD_FAST                0 (self)
-                           956 LOAD_METHOD             25 (winfo_id)
-                           978 PRECALL                  0
-                           982 CALL                     0
-                           992 PRECALL                  1
-                           996 CALL                     1
-               
-                51        1006 LOAD_CONST              18 (20)
-               
-                52        1008 PUSH_NULL
-                          1010 LOAD_FAST               21 (byref)
-                          1012 LOAD_FAST               24 (value)
-                          1014 PRECALL                  1
-                          1018 CALL                     1
-               
-                53        1028 PUSH_NULL
-                          1030 LOAD_FAST               23 (sizeof)
-                          1032 LOAD_FAST               24 (value)
-                          1034 PRECALL                  1
-                          1038 CALL                     1
-               
-                49        1048 PRECALL                  4
-                          1052 CALL                     4
-                          1062 POP_TOP
-                          1064 JUMP_FORWARD             7 (to 1080)
-                       >> 1066 PUSH_EXC_INFO
-               
-                55        1068 POP_TOP
-               
-                56        1070 POP_EXCEPT
-                          1072 JUMP_FORWARD             3 (to 1080)
-                       >> 1074 COPY                     3
-                          1076 POP_EXCEPT
-                          1078 RERAISE                  1
-               
-                57     >> 1080 LOAD_FAST               18 (platform)
-                          1082 LOAD_CONST              15 ('win32')
-                          1084 COMPARE_OP               2 (==)
-                          1090 POP_JUMP_FORWARD_IF_FALSE   155 (to 1402)
-                          1092 LOAD_FAST                4 (wincaption)
-                          1094 POP_JUMP_FORWARD_IF_NONE   155 (to 1406)
-               
-                58        1096 LOAD_CONST               1 (0)
-                          1098 LOAD_CONST              14 (('platform',))
-                          1100 IMPORT_NAME             13 (sys)
-                          1102 IMPORT_FROM             14 (platform)
-                          1104 STORE_FAST              18 (platform)
-                          1106 POP_TOP
-               
-                59        1108 LOAD_CONST               1 (0)
-                          1110 LOAD_CONST              19 (('windll', 'byref', 'sizeof', 'c_int'))
-                          1112 IMPORT_NAME             15 (ctypes)
-                          1114 IMPORT_FROM             16 (windll)
-                          1116 STORE_FAST              19 (windll)
-                          1118 IMPORT_FROM             18 (byref)
-                          1120 STORE_FAST              21 (byref)
-                          1122 IMPORT_FROM             20 (sizeof)
-                          1124 STORE_FAST              23 (sizeof)
-                          1126 IMPORT_FROM             19 (c_int)
-                          1128 STORE_FAST              22 (c_int)
-                          1130 POP_TOP
-               
-                60        1132 LOAD_CONST               1 (0)
-                          1134 LOAD_CONST              20 (('RGB',))
-                          1136 IMPORT_NAME             26 (ctypes.wintypes)
-                          1138 IMPORT_FROM             27 (RGB)
-                          1140 STORE_FAST              25 (RGB)
-                          1142 POP_TOP
-               
-                61        1144 LOAD_FAST               19 (windll)
-                          1146 LOAD_ATTR               21 (dwmapi)
-                          1156 LOAD_METHOD             22 (DwmSetWindowAttribute)
-                          1178 LOAD_FAST               19 (windll)
-                          1180 LOAD_ATTR               23 (user32)
-                          1190 LOAD_METHOD             24 (GetParent)
-                          1212 LOAD_FAST                0 (self)
-                          1214 LOAD_METHOD             25 (winfo_id)
-                          1236 PRECALL                  0
-                          1240 CALL                     0
-                          1250 PRECALL                  1
-                          1254 CALL                     1
-                          1264 LOAD_CONST              21 (35)
-                          1266 PUSH_NULL
-                          1268 LOAD_FAST               21 (byref)
-                          1270 PUSH_NULL
-                          1272 LOAD_FAST               22 (c_int)
-                          1274 PUSH_NULL
-                          1276 LOAD_FAST               25 (RGB)
-                          1278 LOAD_FAST                4 (wincaption)
-                          1280 LOAD_CONST               1 (0)
-                          1282 BINARY_SUBSCR
+                44         806 LOAD_FAST                3 (windark)
+                           808 LOAD_FAST                0 (self)
+                           810 STORE_ATTR              13 (windark)
+               
+                46         820 LOAD_CONST               1 (0)
+                           822 LOAD_CONST              14 (('platform',))
+                           824 IMPORT_NAME             14 (sys)
+                           826 IMPORT_FROM             15 (platform)
+                           828 STORE_FAST              18 (platform)
+                           830 POP_TOP
+               
+                47         832 LOAD_FAST               18 (platform)
+                           834 LOAD_CONST              15 ('win32')
+                           836 COMPARE_OP               2 (==)
+                           842 POP_JUMP_FORWARD_IF_FALSE   125 (to 1094)
+                           844 LOAD_FAST                3 (windark)
+                           846 POP_JUMP_FORWARD_IF_FALSE   123 (to 1094)
+               
+                48         848 NOP
+               
+                49         850 LOAD_CONST               1 (0)
+                           852 LOAD_CONST              16 (('windll', 'wintypes', 'byref', 'c_int', 'sizeof'))
+                           854 IMPORT_NAME             16 (ctypes)
+                           856 IMPORT_FROM             17 (windll)
+                           858 STORE_FAST              19 (windll)
+                           860 IMPORT_FROM             18 (wintypes)
+                           862 STORE_FAST              20 (wintypes)
+                           864 IMPORT_FROM             19 (byref)
+                           866 STORE_FAST              21 (byref)
+                           868 IMPORT_FROM             20 (c_int)
+                           870 STORE_FAST              22 (c_int)
+                           872 IMPORT_FROM             21 (sizeof)
+                           874 STORE_FAST              23 (sizeof)
+                           876 POP_TOP
+               
+                50         878 PUSH_NULL
+                           880 LOAD_FAST               22 (c_int)
+                           882 LOAD_CONST              17 (1)
+                           884 PRECALL                  1
+                           888 CALL                     1
+                           898 STORE_FAST              24 (value)
+               
+                51         900 LOAD_FAST               19 (windll)
+                           902 LOAD_ATTR               22 (dwmapi)
+                           912 LOAD_METHOD             23 (DwmSetWindowAttribute)
+               
+                52         934 LOAD_FAST               19 (windll)
+                           936 LOAD_ATTR               24 (user32)
+                           946 LOAD_METHOD             25 (GetParent)
+                           968 LOAD_FAST                0 (self)
+                           970 LOAD_METHOD             26 (winfo_id)
+                           992 PRECALL                  0
+                           996 CALL                     0
+                          1006 PRECALL                  1
+                          1010 CALL                     1
+               
+                53        1020 LOAD_CONST              18 (20)
+               
+                54        1022 PUSH_NULL
+                          1024 LOAD_FAST               21 (byref)
+                          1026 LOAD_FAST               24 (value)
+                          1028 PRECALL                  1
+                          1032 CALL                     1
+               
+                55        1042 PUSH_NULL
+                          1044 LOAD_FAST               23 (sizeof)
+                          1046 LOAD_FAST               24 (value)
+                          1048 PRECALL                  1
+                          1052 CALL                     1
+               
+                51        1062 PRECALL                  4
+                          1066 CALL                     4
+                          1076 POP_TOP
+                          1078 JUMP_FORWARD             7 (to 1094)
+                       >> 1080 PUSH_EXC_INFO
+               
+                57        1082 POP_TOP
+               
+                58        1084 POP_EXCEPT
+                          1086 JUMP_FORWARD             3 (to 1094)
+                       >> 1088 COPY                     3
+                          1090 POP_EXCEPT
+                          1092 RERAISE                  1
+               
+                59     >> 1094 LOAD_FAST               18 (platform)
+                          1096 LOAD_CONST              15 ('win32')
+                          1098 COMPARE_OP               2 (==)
+                          1104 POP_JUMP_FORWARD_IF_FALSE   155 (to 1416)
+                          1106 LOAD_FAST                4 (wincaption)
+                          1108 POP_JUMP_FORWARD_IF_NONE   155 (to 1420)
+               
+                60        1110 LOAD_CONST               1 (0)
+                          1112 LOAD_CONST              14 (('platform',))
+                          1114 IMPORT_NAME             14 (sys)
+                          1116 IMPORT_FROM             15 (platform)
+                          1118 STORE_FAST              18 (platform)
+                          1120 POP_TOP
+               
+                61        1122 LOAD_CONST               1 (0)
+                          1124 LOAD_CONST              19 (('windll', 'byref', 'sizeof', 'c_int'))
+                          1126 IMPORT_NAME             16 (ctypes)
+                          1128 IMPORT_FROM             17 (windll)
+                          1130 STORE_FAST              19 (windll)
+                          1132 IMPORT_FROM             19 (byref)
+                          1134 STORE_FAST              21 (byref)
+                          1136 IMPORT_FROM             21 (sizeof)
+                          1138 STORE_FAST              23 (sizeof)
+                          1140 IMPORT_FROM             20 (c_int)
+                          1142 STORE_FAST              22 (c_int)
+                          1144 POP_TOP
+               
+                62        1146 LOAD_CONST               1 (0)
+                          1148 LOAD_CONST              20 (('RGB',))
+                          1150 IMPORT_NAME             27 (ctypes.wintypes)
+                          1152 IMPORT_FROM             28 (RGB)
+                          1154 STORE_FAST              25 (RGB)
+                          1156 POP_TOP
+               
+                63        1158 LOAD_FAST               19 (windll)
+                          1160 LOAD_ATTR               22 (dwmapi)
+                          1170 LOAD_METHOD             23 (DwmSetWindowAttribute)
+                          1192 LOAD_FAST               19 (windll)
+                          1194 LOAD_ATTR               24 (user32)
+                          1204 LOAD_METHOD             25 (GetParent)
+                          1226 LOAD_FAST                0 (self)
+                          1228 LOAD_METHOD             26 (winfo_id)
+                          1250 PRECALL                  0
+                          1254 CALL                     0
+                          1264 PRECALL                  1
+                          1268 CALL                     1
+                          1278 LOAD_CONST              21 (35)
+                          1280 PUSH_NULL
+                          1282 LOAD_FAST               21 (byref)
+                          1284 PUSH_NULL
+                          1286 LOAD_FAST               22 (c_int)
+                          1288 PUSH_NULL
+                          1290 LOAD_FAST               25 (RGB)
                           1292 LOAD_FAST                4 (wincaption)
-                          1294 LOAD_CONST              17 (1)
+                          1294 LOAD_CONST               1 (0)
                           1296 BINARY_SUBSCR
                           1306 LOAD_FAST                4 (wincaption)
-                          1308 LOAD_CONST              22 (2)
+                          1308 LOAD_CONST              17 (1)
                           1310 BINARY_SUBSCR
-                          1320 PRECALL                  3
-                          1324 CALL                     3
-                          1334 PRECALL                  1
-                          1338 CALL                     1
+                          1320 LOAD_FAST                4 (wincaption)
+                          1322 LOAD_CONST              22 (2)
+                          1324 BINARY_SUBSCR
+                          1334 PRECALL                  3
+                          1338 CALL                     3
                           1348 PRECALL                  1
                           1352 CALL                     1
+                          1362 PRECALL                  1
+                          1366 CALL                     1
                
-                62        1362 PUSH_NULL
-                          1364 LOAD_FAST               23 (sizeof)
-                          1366 LOAD_FAST               22 (c_int)
-                          1368 PRECALL                  1
-                          1372 CALL                     1
-               
-                61        1382 PRECALL                  4
-                          1386 CALL                     4
-                          1396 POP_TOP
-                          1398 LOAD_CONST               0 (None)
-                          1400 RETURN_VALUE
-               
-                57     >> 1402 LOAD_CONST               0 (None)
-                          1404 RETURN_VALUE
-                       >> 1406 LOAD_CONST               0 (None)
-                          1408 RETURN_VALUE
+                64        1376 PUSH_NULL
+                          1378 LOAD_FAST               23 (sizeof)
+                          1380 LOAD_FAST               22 (c_int)
+                          1382 PRECALL                  1
+                          1386 CALL                     1
+               
+                63        1396 PRECALL                  4
+                          1400 CALL                     4
+                          1410 POP_TOP
+                          1412 LOAD_CONST               0 (None)
+                          1414 RETURN_VALUE
+               
+                59     >> 1416 LOAD_CONST               0 (None)
+                          1418 RETURN_VALUE
+                       >> 1420 LOAD_CONST               0 (None)
+                          1422 RETURN_VALUE
                ExceptionTable:
                  204 to 276 -> 302 [1] lasti
                  302 to 308 -> 310 [3] lasti
                  316 to 316 -> 310 [3] lasti
                  356 to 428 -> 454 [1] lasti
                  454 to 460 -> 462 [3] lasti
                  468 to 468 -> 462 [3] lasti
-                 836 to 1062 -> 1066 [0]
-                 1066 to 1068 -> 1074 [1] lasti
+                 850 to 1076 -> 1080 [0]
+                 1080 to 1082 -> 1088 [1] lasti
                consts
                   None
                   0
                   ('mkstemp',)
                   b'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'
                   b'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'
                   'wb'
@@ -634,26 +638,26 @@
                   ('windll', 'wintypes', 'byref', 'c_int', 'sizeof')
                   1
                   20
                   ('windll', 'byref', 'sizeof', 'c_int')
                   ('RGB',)
                   35
                   2
-               names      ('super', '__init__', 'title', 'tempfile', 'mkstemp', 'open', 'base64', 'b64decode', 'write', 'replace', 'lower', 'iconphoto', 'default_palette', 'sys', 'platform', 'ctypes', 'windll', 'wintypes', 'byref', 'c_int', 'sizeof', 'dwmapi', 'DwmSetWindowAttribute', 'user32', 'GetParent', 'winfo_id', 'ctypes.wintypes', 'RGB')
+               names      ('super', '__init__', 'title', 'tempfile', 'mkstemp', 'open', 'base64', 'b64decode', 'write', 'replace', 'lower', 'iconphoto', 'default_palette', 'windark', 'sys', 'platform', 'ctypes', 'windll', 'wintypes', 'byref', 'c_int', 'sizeof', 'dwmapi', 'DwmSetWindowAttribute', 'user32', 'GetParent', 'winfo_id', 'ctypes.wintypes', 'RGB')
                varnames   ('self', 'title', 'icon', 'windark', 'wincaption', 'args', 'kwargs', 'mkstemp', '_adwite_light', '_adwite_dark', '_', '_adwite_light_temp', '_adwite_dark_temp', '_adwite_light_file', 'b64decode', '_adwite_dark_file', 'adwite_light_photo', 'adwite_dark_photo', 'platform', 'windll', 'wintypes', 'byref', 'c_int', 'sizeof', 'value', 'RGB')
                freevars   ('__class__',)
                cellvars   ('adwite_dark_icon', 'adwite_light_icon')
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
                name       '__init__'
                firstlineno 5
                lnotab
                   0x080132012a020c02040104021a011a0222010c013cfe2e0422010c013c
-                  fe2e042c012c020a040a0430011601300114012c0228020c01100102011c
-                  011601220156010201140114fc140602010a0110010c0118010c01da0114
-                  ff14fc
+                  fe2e042c012c020a040a0430011601300114012c0228020e020c01100102
+                  011c011601220156010201140114fc140602010a0110010c0118010c01da
+                  0114ff14fc
             '#0a080a'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
@@ -666,90 +670,90 @@
                   0000000000000000007c01ac08a6010000ab01000000000000000001007c
                   0364096b020000000072177c00a008000000000000000000000000000000
                   0000000000640a7c01a6020000ab02000000000000000001006e2564017c
                   006a0500000000000000005f0900000000000000007c006a050000000000
                   000000a00a0000000000000000000000000000000000000000a6000000ab
                   00000000000000000001007c00a00b000000000000000000000000000000
                   0000000000640b6403a6020000ab020000000000000000010064005300
-                64           0 RESUME                   0
+                66           0 RESUME                   0
                
-                65           2 LOAD_CONST               1 (0)
+                67           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('AdwTFrame',))
                              6 IMPORT_NAME              0 (tkadw.windows.theme)
                              8 IMPORT_FROM              1 (AdwTFrame)
                             10 STORE_FAST               2 (AdwTFrame)
                             12 POP_TOP
                
-                66          14 LOAD_FAST                0 (self)
+                68          14 LOAD_FAST                0 (self)
                             16 LOAD_METHOD              2 (overrideredirect)
                             38 LOAD_CONST               3 (True)
                             40 PRECALL                  1
                             44 CALL                     1
                             54 POP_TOP
                
-                68          56 LOAD_CONST               1 (0)
+                70          56 LOAD_CONST               1 (0)
                             58 LOAD_CONST               4 (('platform',))
                             60 IMPORT_NAME              3 (sys)
                             62 IMPORT_FROM              4 (platform)
                             64 STORE_FAST               3 (platform)
                             66 POP_TOP
                
-                70          68 PUSH_NULL
+                72          68 PUSH_NULL
                             70 LOAD_FAST                2 (AdwTFrame)
                             72 PRECALL                  0
                             76 CALL                     0
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               5 (frame)
                
-                71          98 LOAD_FAST                0 (self)
+                73          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                5 (frame)
                            110 LOAD_METHOD              6 (pack)
                            132 LOAD_CONST               5 ('both')
                            134 LOAD_CONST               6 ('yes')
                            136 KW_NAMES                 7
                            138 PRECALL                  2
                            142 CALL                     2
                            152 POP_TOP
                
-                72         154 LOAD_FAST                0 (self)
+                74         154 LOAD_FAST                0 (self)
                            156 LOAD_ATTR                5 (frame)
                            166 LOAD_METHOD              7 (configure)
                            188 LOAD_FAST                1 (tcolor)
                            190 KW_NAMES                 8
                            192 PRECALL                  1
                            196 CALL                     1
                            206 POP_TOP
                
-                74         208 LOAD_FAST                3 (platform)
+                76         208 LOAD_FAST                3 (platform)
                            210 LOAD_CONST               9 ('win32')
                            212 COMPARE_OP               2 (==)
                            218 POP_JUMP_FORWARD_IF_FALSE    23 (to 266)
                
-                75         220 LOAD_FAST                0 (self)
+                77         220 LOAD_FAST                0 (self)
                            222 LOAD_METHOD              8 (attributes)
                            244 LOAD_CONST              10 ('-transparentcolor')
                            246 LOAD_FAST                1 (tcolor)
                            248 PRECALL                  2
                            252 CALL                     2
                            262 POP_TOP
                            264 JUMP_FORWARD            37 (to 340)
                
-                77     >>  266 LOAD_CONST               1 (0)
+                79     >>  266 LOAD_CONST               1 (0)
                            268 LOAD_FAST                0 (self)
                            270 LOAD_ATTR                5 (frame)
                            280 STORE_ATTR               9 (frame_radius)
                
-                78         290 LOAD_FAST                0 (self)
+                80         290 LOAD_FAST                0 (self)
                            292 LOAD_ATTR                5 (frame)
                            302 LOAD_METHOD             10 (update)
                            324 PRECALL                  0
                            328 CALL                     0
                            338 POP_TOP
                
-                80     >>  340 LOAD_FAST                0 (self)
+                82     >>  340 LOAD_FAST                0 (self)
                            342 LOAD_METHOD             11 (wm_attributes)
                            364 LOAD_CONST              11 ('-topmost')
                            366 LOAD_CONST               3 (True)
                            368 PRECALL                  2
                            372 CALL                     2
                            382 POP_TOP
                            384 LOAD_CONST               0 (None)
@@ -769,52 +773,52 @@
                   '-topmost'
                names      ('tkadw.windows.theme', 'AdwTFrame', 'overrideredirect', 'sys', 'platform', 'frame', 'pack', 'configure', 'attributes', 'frame_radius', 'update', 'wm_attributes')
                varnames   ('self', 'tcolor', 'AdwTFrame', 'platform')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
                name       'custom'
-               firstlineno 64
+               firstlineno 66
                lnotab 0x02010c012a020c021e01380136020c012e0218013202
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x87009700640184007d0288006601640284087d037c01a0000000000000
                   00000000000000000000000000000064037c026404ac05a6030000ab0300
                   0000000000000001007c01a0000000000000000000000000000000000000
                   00000064067c036404ac05a6030000ab0300000000000000000100640053
                   00
                              0 MAKE_CELL                0 (self)
                
-                82           2 RESUME                   0
+                84           2 RESUME                   0
                
-                83           4 LOAD_CONST               1 (<code object _click, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 83>)
+                85           4 LOAD_CONST               1 (<code object _click, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 85>)
                              6 MAKE_FUNCTION            0
                              8 STORE_FAST               2 (_click)
                
-                87          10 LOAD_CLOSURE             0 (self)
+                89          10 LOAD_CLOSURE             0 (self)
                             12 BUILD_TUPLE              1
-                            14 LOAD_CONST               2 (<code object _move, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 87>)
+                            14 LOAD_CONST               2 (<code object _move, file "D:\tkadw\tkadw\windows\widgets\adw.py", line 89>)
                             16 MAKE_FUNCTION            8 (closure)
                             18 STORE_FAST               3 (_move)
                
-                93          20 LOAD_FAST                1 (widget)
+                95          20 LOAD_FAST                1 (widget)
                             22 LOAD_METHOD              0 (bind)
                             44 LOAD_CONST               3 ('<Button-1>')
                             46 LOAD_FAST                2 (_click)
                             48 LOAD_CONST               4 ('+')
                             50 KW_NAMES                 5
                             52 PRECALL                  3
                             56 CALL                     3
                             66 POP_TOP
                
-                94          68 LOAD_FAST                1 (widget)
+                96          68 LOAD_FAST                1 (widget)
                             70 LOAD_METHOD              0 (bind)
                             92 LOAD_CONST               6 ('<B1-Motion>')
                             94 LOAD_FAST                3 (_move)
                             96 LOAD_CONST               4 ('+')
                             98 KW_NAMES                 5
                            100 PRECALL                  3
                            104 CALL                     3
@@ -827,17 +831,17 @@
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x97007c006a0000000000000000007c006a010000000000000000630261
                         00610164005300
-                      83           0 RESUME                   0
+                      85           0 RESUME                   0
                      
-                      85           2 LOAD_FAST                0 (event)
+                      87           2 LOAD_FAST                0 (event)
                                    4 LOAD_ATTR                0 (x)
                                   14 LOAD_FAST                0 (event)
                                   16 LOAD_ATTR                1 (y)
                                   26 SWAP                     2
                                   28 STORE_GLOBAL             0 (x)
                                   30 STORE_GLOBAL             1 (y)
                                   32 LOAD_CONST               0 (None)
@@ -846,15 +850,15 @@
                         None
                      names      ('x', 'y')
                      varnames   ('event',)
                      freevars   ()
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
                      name       '_click'
-                     firstlineno 83
+                     firstlineno 85
                      lnotab 0x0202
                   code
                      argcount  : 1
                      nlocals   : 4
                      stacksize : 4
                      flags     : 19
                      code
@@ -864,48 +868,48 @@
                         04000000000000000000007a0a00008904a0030000000000000000000000
                         000000000000000000a6000000ab0000000000000000007a0000007d0264
                         017c019b0064017c029b009d047d038904a0040000000000000000000000
                         0000000000000000007c03a6010000ab0100000000000000000100640053
                         00
                                    0 COPY_FREE_VARS           1
                      
-                      87           2 RESUME                   0
+                      89           2 RESUME                   0
                      
-                      88           4 LOAD_FAST                0 (event)
+                      90           4 LOAD_FAST                0 (event)
                                    6 LOAD_ATTR                0 (x)
                                   16 LOAD_GLOBAL              0 (x)
                                   28 BINARY_OP               10 (-)
                                   32 LOAD_DEREF               4 (self)
                                   34 LOAD_METHOD              1 (winfo_x)
                                   56 PRECALL                  0
                                   60 CALL                     0
                                   70 BINARY_OP                0 (+)
                                   74 STORE_FAST               1 (new_x)
                      
-                      89          76 LOAD_FAST                0 (event)
+                      91          76 LOAD_FAST                0 (event)
                                   78 LOAD_ATTR                2 (y)
                                   88 LOAD_GLOBAL              4 (y)
                                  100 BINARY_OP               10 (-)
                                  104 LOAD_DEREF               4 (self)
                                  106 LOAD_METHOD              3 (winfo_y)
                                  128 PRECALL                  0
                                  132 CALL                     0
                                  142 BINARY_OP                0 (+)
                                  146 STORE_FAST               2 (new_y)
                      
-                      90         148 LOAD_CONST               1 ('+')
+                      92         148 LOAD_CONST               1 ('+')
                                  150 LOAD_FAST                1 (new_x)
                                  152 FORMAT_VALUE             0
                                  154 LOAD_CONST               1 ('+')
                                  156 LOAD_FAST                2 (new_y)
                                  158 FORMAT_VALUE             0
                                  160 BUILD_STRING             4
                                  162 STORE_FAST               3 (s)
                      
-                      91         164 LOAD_DEREF               4 (self)
+                      93         164 LOAD_DEREF               4 (self)
                                  166 LOAD_METHOD              4 (geometry)
                                  188 LOAD_FAST                3 (s)
                                  190 PRECALL                  1
                                  194 CALL                     1
                                  204 POP_TOP
                                  206 LOAD_CONST               0 (None)
                                  208 RETURN_VALUE
@@ -914,109 +918,109 @@
                         '+'
                      names      ('x', 'winfo_x', 'y', 'winfo_y', 'geometry')
                      varnames   ('event', 'new_x', 'new_y', 's')
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
                      name       '_move'
-                     firstlineno 87
+                     firstlineno 89
                      lnotab 0x0401480148011001
                   '<Button-1>'
                   '+'
                   ('add',)
                   '<B1-Motion>'
                names      ('bind',)
                varnames   ('self', 'widget', '_click', '_move')
                freevars   ()
                cellvars   ('self',)
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
                name       'bind_move'
-               firstlineno 82
+               firstlineno 84
                lnotab 0x040106040a063001
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-                96           0 RESUME                   0
+                98           0 RESUME                   0
                
-                97           2 LOAD_CONST               0 (None)
+                99           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
                name       'default_palette'
-               firstlineno 96
+               firstlineno 98
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c01812864017c01760072267c00a0000000000000000000000000
                   0000000000000000007c0164011900000000000000000064021900000000
                   0000000000ac03a6010000ab010000000000000000010064005300640053
                   0064005300
-                99           0 RESUME                   0
+               101           0 RESUME                   0
                
-               100           2 LOAD_FAST                1 (dict)
+               102           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE    40 (to 86)
                
-               101           6 LOAD_CONST               1 ('window')
+               103           6 LOAD_CONST               1 ('window')
                              8 LOAD_FAST                1 (dict)
                             10 CONTAINS_OP              0
                             12 POP_JUMP_FORWARD_IF_FALSE    38 (to 90)
                
-               102          14 LOAD_FAST                0 (self)
+               104          14 LOAD_FAST                0 (self)
                             16 LOAD_METHOD              0 (configure)
                             38 LOAD_FAST                1 (dict)
                             40 LOAD_CONST               1 ('window')
                             42 BINARY_SUBSCR
                             52 LOAD_CONST               2 ('back')
                             54 BINARY_SUBSCR
                             64 KW_NAMES                 3
                             66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                
-               100     >>   86 LOAD_CONST               0 (None)
+               102     >>   86 LOAD_CONST               0 (None)
                             88 RETURN_VALUE
                
-               101     >>   90 LOAD_CONST               0 (None)
+               103     >>   90 LOAD_CONST               0 (None)
                             92 RETURN_VALUE
                consts
                   None
                   'window'
                   'back'
                   ('background',)
                names      ('configure',)
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
                name       'palette'
-               firstlineno 99
+               firstlineno 101
                lnotab 0x02010401080148fe0401
             ('#0a080a',)
          names      ('__name__', '__module__', '__qualname__', 'str', 'bool', '__init__', 'custom', 'bind_move', 'default_palette', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
          name       'Adw'
          firstlineno 4
-         lnotab 0x0c01203b0812060e0603
+         lnotab 0x0c01203d0812060e0603
       'Adw'
       None
    names      ('tkinter', 'Tk', 'Adw')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\widgets\\adw.py'
```

### Comparing `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc` & `tkadw-0.3.5/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,177 +1,187 @@
 magic:    0xa70d0d0a
-moddate:  0x8ff6a364 (Tue Jul  4 10:38:07 2023 UTC)
-files sz: 1992
+moddate:  0xee37bf64 (Tue Jul 25 02:48:14 2023 UTC)
+files sz: 2039
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 5
+   stacksize : 6
    flags     : 0
    code
-      0x9700640064016c006d015a010100020047006402840064036501a60300
-      00ab0300000000000000005a02020047006404840064056502a6030000ab
-      0300000000000000005a03020047006406840064076502a6030000ab0300
-      000000000000005a04650564086b02000000007266640064096c006d065a
-      06010002006506a6000000ab0000000000000000005a0702006503640aac
-      0ba6010000ab0100000000000000005a086508a009000000000000000000
-      0000000000000000000000a6000000ab0000000000000000000100020065
-      04640aac0ba6010000ab0100000000000000005a0a650aa0090000000000
-      000000000000000000000000000000a6000000ab00000000000000000001
-      006507a00b0000000000000000000000000000000000000000a6000000ab
-      0000000000000000000100640c5300640c5300
+      0x9700640064016c006d015a010100640064026c026d035a030100020047
+      0064038400640465016503a6040000ab0400000000000000005a04020047
+      006405840064066504a6030000ab0300000000000000005a050200470064
+      07840064086504a6030000ab0300000000000000005a06650764096b0200
+      00000072666400640a6c006d085a08010002006508a6000000ab00000000
+      00000000005a0902006505640bac0ca6010000ab0100000000000000005a
+      0a650aa00b0000000000000000000000000000000000000000a6000000ab
+      000000000000000000010002006506640bac0ca6010000ab010000000000
+      0000005a0c650ca00b0000000000000000000000000000000000000000a6
+      000000ab00000000000000000001006509a00d0000000000000000000000
+      000000000000000000a6000000ab0000000000000000000100640d530064
+      0d5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Label',))
                  6 IMPORT_NAME              0 (tkinter)
                  8 IMPORT_FROM              1 (Label)
                 10 STORE_NAME               1 (Label)
                 12 POP_TOP
    
-     4          14 PUSH_NULL
-                16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               2 (<code object AdwBasicLabel, file "D:\tkadw\tkadw\windows\widgets\label.py", line 4>)
-                20 MAKE_FUNCTION            0
-                22 LOAD_CONST               3 ('AdwBasicLabel')
-                24 LOAD_NAME                1 (Label)
-                26 PRECALL                  3
-                30 CALL                     3
-                40 STORE_NAME               2 (AdwBasicLabel)
-   
-    63          42 PUSH_NULL
-                44 LOAD_BUILD_CLASS
-                46 LOAD_CONST               4 (<code object AdwLabel, file "D:\tkadw\tkadw\windows\widgets\label.py", line 63>)
-                48 MAKE_FUNCTION            0
-                50 LOAD_CONST               5 ('AdwLabel')
-                52 LOAD_NAME                2 (AdwBasicLabel)
-                54 PRECALL                  3
-                58 CALL                     3
-                68 STORE_NAME               3 (AdwLabel)
-   
-    68          70 PUSH_NULL
-                72 LOAD_BUILD_CLASS
-                74 LOAD_CONST               6 (<code object AdwDarkLabel, file "D:\tkadw\tkadw\windows\widgets\label.py", line 68>)
-                76 MAKE_FUNCTION            0
-                78 LOAD_CONST               7 ('AdwDarkLabel')
-                80 LOAD_NAME                2 (AdwBasicLabel)
-                82 PRECALL                  3
-                86 CALL                     3
-                96 STORE_NAME               4 (AdwDarkLabel)
-   
-    73          98 LOAD_NAME                5 (__name__)
-               100 LOAD_CONST               8 ('__main__')
-               102 COMPARE_OP               2 (==)
-               108 POP_JUMP_FORWARD_IF_FALSE   102 (to 314)
-   
-    74         110 LOAD_CONST               0 (0)
-               112 LOAD_CONST               9 (('Tk',))
-               114 IMPORT_NAME              0 (tkinter)
-               116 IMPORT_FROM              6 (Tk)
-               118 STORE_NAME               6 (Tk)
-               120 POP_TOP
-   
-    75         122 PUSH_NULL
-               124 LOAD_NAME                6 (Tk)
-               126 PRECALL                  0
-               130 CALL                     0
-               140 STORE_NAME               7 (root)
-   
-    76         142 PUSH_NULL
-               144 LOAD_NAME                3 (AdwLabel)
-               146 LOAD_CONST              10 ('hello')
-               148 KW_NAMES                11
-               150 PRECALL                  1
-               154 CALL                     1
-               164 STORE_NAME               8 (label)
-   
-    77         166 LOAD_NAME                8 (label)
-               168 LOAD_METHOD              9 (pack)
-               190 PRECALL                  0
-               194 CALL                     0
-               204 POP_TOP
-   
-    78         206 PUSH_NULL
-               208 LOAD_NAME                4 (AdwDarkLabel)
-               210 LOAD_CONST              10 ('hello')
-               212 KW_NAMES                11
-               214 PRECALL                  1
-               218 CALL                     1
-               228 STORE_NAME              10 (label2)
-   
-    79         230 LOAD_NAME               10 (label2)
-               232 LOAD_METHOD              9 (pack)
-               254 PRECALL                  0
-               258 CALL                     0
-               268 POP_TOP
-   
-    80         270 LOAD_NAME                7 (root)
-               272 LOAD_METHOD             11 (mainloop)
-               294 PRECALL                  0
-               298 CALL                     0
-               308 POP_TOP
-               310 LOAD_CONST              12 (None)
-               312 RETURN_VALUE
+     2          14 LOAD_CONST               0 (0)
+                16 LOAD_CONST               2 (('AdwLayout',))
+                18 IMPORT_NAME              2 (tkadw.layout)
+                20 IMPORT_FROM              3 (AdwLayout)
+                22 STORE_NAME               3 (AdwLayout)
+                24 POP_TOP
+   
+     5          26 PUSH_NULL
+                28 LOAD_BUILD_CLASS
+                30 LOAD_CONST               3 (<code object AdwBasicLabel, file "D:\tkadw\tkadw\windows\widgets\label.py", line 5>)
+                32 MAKE_FUNCTION            0
+                34 LOAD_CONST               4 ('AdwBasicLabel')
+                36 LOAD_NAME                1 (Label)
+                38 LOAD_NAME                3 (AdwLayout)
+                40 PRECALL                  4
+                44 CALL                     4
+                54 STORE_NAME               4 (AdwBasicLabel)
+   
+    64          56 PUSH_NULL
+                58 LOAD_BUILD_CLASS
+                60 LOAD_CONST               5 (<code object AdwLabel, file "D:\tkadw\tkadw\windows\widgets\label.py", line 64>)
+                62 MAKE_FUNCTION            0
+                64 LOAD_CONST               6 ('AdwLabel')
+                66 LOAD_NAME                4 (AdwBasicLabel)
+                68 PRECALL                  3
+                72 CALL                     3
+                82 STORE_NAME               5 (AdwLabel)
+   
+    69          84 PUSH_NULL
+                86 LOAD_BUILD_CLASS
+                88 LOAD_CONST               7 (<code object AdwDarkLabel, file "D:\tkadw\tkadw\windows\widgets\label.py", line 69>)
+                90 MAKE_FUNCTION            0
+                92 LOAD_CONST               8 ('AdwDarkLabel')
+                94 LOAD_NAME                4 (AdwBasicLabel)
+                96 PRECALL                  3
+               100 CALL                     3
+               110 STORE_NAME               6 (AdwDarkLabel)
+   
+    74         112 LOAD_NAME                7 (__name__)
+               114 LOAD_CONST               9 ('__main__')
+               116 COMPARE_OP               2 (==)
+               122 POP_JUMP_FORWARD_IF_FALSE   102 (to 328)
+   
+    75         124 LOAD_CONST               0 (0)
+               126 LOAD_CONST              10 (('Tk',))
+               128 IMPORT_NAME              0 (tkinter)
+               130 IMPORT_FROM              8 (Tk)
+               132 STORE_NAME               8 (Tk)
+               134 POP_TOP
+   
+    76         136 PUSH_NULL
+               138 LOAD_NAME                8 (Tk)
+               140 PRECALL                  0
+               144 CALL                     0
+               154 STORE_NAME               9 (root)
+   
+    77         156 PUSH_NULL
+               158 LOAD_NAME                5 (AdwLabel)
+               160 LOAD_CONST              11 ('hello')
+               162 KW_NAMES                12
+               164 PRECALL                  1
+               168 CALL                     1
+               178 STORE_NAME              10 (label)
+   
+    78         180 LOAD_NAME               10 (label)
+               182 LOAD_METHOD             11 (pack)
+               204 PRECALL                  0
+               208 CALL                     0
+               218 POP_TOP
+   
+    79         220 PUSH_NULL
+               222 LOAD_NAME                6 (AdwDarkLabel)
+               224 LOAD_CONST              11 ('hello')
+               226 KW_NAMES                12
+               228 PRECALL                  1
+               232 CALL                     1
+               242 STORE_NAME              12 (label2)
+   
+    80         244 LOAD_NAME               12 (label2)
+               246 LOAD_METHOD             11 (pack)
+               268 PRECALL                  0
+               272 CALL                     0
+               282 POP_TOP
+   
+    81         284 LOAD_NAME                9 (root)
+               286 LOAD_METHOD             13 (mainloop)
+               308 PRECALL                  0
+               312 CALL                     0
+               322 POP_TOP
+               324 LOAD_CONST              13 (None)
+               326 RETURN_VALUE
    
-    73     >>  314 LOAD_CONST              12 (None)
-               316 RETURN_VALUE
+    74     >>  328 LOAD_CONST              13 (None)
+               330 RETURN_VALUE
    consts
       0
       ('Label',)
+      ('AdwLayout',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x8700970065005a0164005a02640164029c016403650366028800660164
             04840e5a04640c640684015a05640784005a06640884005a07640984005a
             08640a84005a09640c640b84015a0a880078015a0b5300
                        0 MAKE_CELL                0 (__class__)
          
-           4           2 RESUME                   0
+           5           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwBasicLabel')
                       10 STORE_NAME               2 (__qualname__)
          
-           5          12 LOAD_CONST               1 ('')
+           6          12 LOAD_CONST               1 ('')
                       14 LOAD_CONST               2 (('text',))
                       16 BUILD_CONST_KEY_MAP      1
                       18 LOAD_CONST               3 ('text')
                       20 LOAD_NAME                3 (str)
                       22 BUILD_TUPLE              2
                       24 LOAD_CLOSURE             0 (__class__)
                       26 BUILD_TUPLE              1
-                      28 LOAD_CONST               4 (<code object __init__, file "D:\tkadw\tkadw\windows\widgets\label.py", line 5>)
+                      28 LOAD_CONST               4 (<code object __init__, file "D:\tkadw\tkadw\windows\widgets\label.py", line 6>)
                       30 MAKE_FUNCTION           14 (kwdefaults, annotations, closure)
                       32 STORE_NAME               4 (__init__)
          
-          16          34 LOAD_CONST              12 ((None,))
-                      36 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\windows\widgets\label.py", line 16>)
+          17          34 LOAD_CONST              12 ((None,))
+                      36 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\windows\widgets\label.py", line 17>)
                       38 MAKE_FUNCTION            1 (defaults)
                       40 STORE_NAME               5 (_draw)
          
-          21          42 LOAD_CONST               7 (<code object _other, file "D:\tkadw\tkadw\windows\widgets\label.py", line 21>)
+          22          42 LOAD_CONST               7 (<code object _other, file "D:\tkadw\tkadw\windows\widgets\label.py", line 22>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               6 (_other)
          
-          24          48 LOAD_CONST               8 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\label.py", line 24>)
+          25          48 LOAD_CONST               8 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\label.py", line 25>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               7 (default_palette)
          
-          27          54 LOAD_CONST               9 (<code object palette_light, file "D:\tkadw\tkadw\windows\widgets\label.py", line 27>)
+          28          54 LOAD_CONST               9 (<code object palette_light, file "D:\tkadw\tkadw\windows\widgets\label.py", line 28>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               8 (palette_light)
          
-          37          60 LOAD_CONST              10 (<code object palette_dark, file "D:\tkadw\tkadw\windows\widgets\label.py", line 37>)
+          38          60 LOAD_CONST              10 (<code object palette_dark, file "D:\tkadw\tkadw\windows\widgets\label.py", line 38>)
                       62 MAKE_FUNCTION            0
                       64 STORE_NAME               9 (palette_dark)
          
-          47          66 LOAD_CONST              12 ((None,))
-                      68 LOAD_CONST              11 (<code object palette, file "D:\tkadw\tkadw\windows\widgets\label.py", line 47>)
+          48          66 LOAD_CONST              12 ((None,))
+                      68 LOAD_CONST              11 (<code object palette, file "D:\tkadw\tkadw\windows\widgets\label.py", line 48>)
                       70 MAKE_FUNCTION            1 (defaults)
                       72 STORE_NAME              10 (palette)
                       74 LOAD_CLOSURE             0 (__class__)
                       76 COPY                     1
                       78 STORE_NAME              11 (__classcell__)
                       80 RETURN_VALUE
          consts
@@ -196,67 +206,67 @@
                   00000000000000a6000000ab0000000000000000006403ac04a6030000ab
                   03000000000000000001007c00a004000000000000000000000000000000
                   000000000064067c00a00500000000000000000000000000000000000000
                   00a6000000ab0000000000000000006403ac04a6030000ab030000000000
                   000000010064005300
                              0 COPY_FREE_VARS           1
                
-                 5           2 RESUME                   0
+                 6           2 RESUME                   0
                
-                 6           4 PUSH_NULL
+                 7           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                2 (args)
                             44 LOAD_CONST               1 ('text')
                             46 LOAD_FAST                1 (text)
                             48 BUILD_MAP                1
                             50 LOAD_FAST                3 (kwargs)
                             52 DICT_MERGE               1
                             54 CALL_FUNCTION_EX         1
                             56 POP_TOP
                
-                 8          58 LOAD_FAST                0 (self)
+                 9          58 LOAD_FAST                0 (self)
                             60 LOAD_METHOD              2 (_other)
                             82 PRECALL                  0
                             86 CALL                     0
                             96 POP_TOP
                
-                10          98 LOAD_FAST                0 (self)
+                11          98 LOAD_FAST                0 (self)
                            100 LOAD_METHOD              3 (default_palette)
                            122 PRECALL                  0
                            126 CALL                     0
                            136 POP_TOP
                
-                12         138 LOAD_FAST                0 (self)
+                13         138 LOAD_FAST                0 (self)
                            140 LOAD_METHOD              4 (bind)
                            162 LOAD_CONST               2 ('<Configure>')
                            164 LOAD_FAST                0 (self)
                            166 LOAD_ATTR                5 (_draw)
                            176 LOAD_CONST               3 ('+')
                            178 KW_NAMES                 4
                            180 PRECALL                  3
                            184 CALL                     3
                            194 POP_TOP
                
-                13         196 LOAD_FAST                0 (self)
+                14         196 LOAD_FAST                0 (self)
                            198 LOAD_METHOD              4 (bind)
                            220 LOAD_CONST               5 ('<Enter>')
                            222 LOAD_FAST                0 (self)
                            224 LOAD_METHOD              5 (_draw)
                            246 PRECALL                  0
                            250 CALL                     0
                            260 LOAD_CONST               3 ('+')
                            262 KW_NAMES                 4
                            264 PRECALL                  3
                            268 CALL                     3
                            278 POP_TOP
                
-                14         280 LOAD_FAST                0 (self)
+                15         280 LOAD_FAST                0 (self)
                            282 LOAD_METHOD              4 (bind)
                            304 LOAD_CONST               6 ('<Leave>')
                            306 LOAD_FAST                0 (self)
                            308 LOAD_METHOD              5 (_draw)
                            330 PRECALL                  0
                            334 CALL                     0
                            344 LOAD_CONST               3 ('+')
@@ -276,51 +286,51 @@
                   '<Leave>'
                names      ('super', '__init__', '_other', 'default_palette', 'bind', '_draw')
                varnames   ('self', 'text', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
                name       '__init__'
-               firstlineno 5
+               firstlineno 6
                lnotab 0x04013602280228023a015401
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a00000000000000000064016b0200000000722e7c00a00100
                   000000000000000000000000000000000000007c006a0200000000000000
                   00a00300000000000000000000000000000000000000006402a6010000ab
                   010000000000000000ac03a6010000ab01000000000000000001007c00a0
                   0100000000000000000000000000000000000000007c006a040000000000
                   000000ac04a6010000ab010000000000000000010064005300
-                16           0 RESUME                   0
+                17           0 RESUME                   0
                
-                17           2 LOAD_FAST                0 (self)
+                18           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (label_back)
                             14 LOAD_CONST               1 ('transparent')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE    46 (to 116)
                
-                18          24 LOAD_FAST                0 (self)
+                19          24 LOAD_FAST                0 (self)
                             26 LOAD_METHOD              1 (configure)
                             48 LOAD_FAST                0 (self)
                             50 LOAD_ATTR                2 (master)
                             60 LOAD_METHOD              3 (cget)
                             82 LOAD_CONST               2 ('bg')
                             84 PRECALL                  1
                             88 CALL                     1
                             98 KW_NAMES                 3
                            100 PRECALL                  1
                            104 CALL                     1
                            114 POP_TOP
                
-                19     >>  116 LOAD_FAST                0 (self)
+                20     >>  116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              1 (configure)
                            140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                4 (label_text_back)
                            152 KW_NAMES                 4
                            154 PRECALL                  1
                            158 CALL                     1
                            168 POP_TOP
@@ -334,88 +344,88 @@
                   ('foreground',)
                names      ('label_back', 'configure', 'master', 'cget', 'label_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
                name       '_draw'
-               firstlineno 16
+               firstlineno 17
                lnotab 0x020116015c01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x970064005300
-                21           0 RESUME                   0
+                22           0 RESUME                   0
                
-                22           2 LOAD_CONST               0 (None)
+                23           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
                name       '_other'
-               firstlineno 21
+               firstlineno 22
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                24           0 RESUME                   0
+                25           0 RESUME                   0
                
-                25           2 LOAD_FAST                0 (self)
+                26           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
                name       'default_palette'
-               firstlineno 24
+               firstlineno 25
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364049c026901a6010000ab010000000000000000010064005300
-                27           0 RESUME                   0
+                28           0 RESUME                   0
                
-                28           2 LOAD_FAST                0 (self)
+                29           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                30          26 LOAD_CONST               1 ('label')
+                31          26 LOAD_CONST               1 ('label')
                
-                31          28 LOAD_CONST               2 ('transparent')
+                32          28 LOAD_CONST               2 ('transparent')
                
-                32          30 LOAD_CONST               3 ('#000000')
+                33          30 LOAD_CONST               3 ('#000000')
                
-                30          32 LOAD_CONST               4 (('back', 'text_back'))
+                31          32 LOAD_CONST               4 (('back', 'text_back'))
                             34 BUILD_CONST_KEY_MAP      2
                
-                29          36 BUILD_MAP                1
+                30          36 BUILD_MAP                1
                
-                28          38 PRECALL                  1
+                29          38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
                             56 RETURN_VALUE
                consts
                   None
                   'label'
@@ -424,41 +434,41 @@
                   ('back', 'text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
                name       'palette_light'
-               firstlineno 27
+               firstlineno 28
                lnotab 0x020118020201020102fe04ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 6
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364049c026901a6010000ab010000000000000000010064005300
-                37           0 RESUME                   0
+                38           0 RESUME                   0
                
-                38           2 LOAD_FAST                0 (self)
+                39           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-                40          26 LOAD_CONST               1 ('label')
+                41          26 LOAD_CONST               1 ('label')
                
-                41          28 LOAD_CONST               2 ('transparent')
+                42          28 LOAD_CONST               2 ('transparent')
                
-                42          30 LOAD_CONST               3 ('#ffffff')
+                43          30 LOAD_CONST               3 ('#ffffff')
                
-                40          32 LOAD_CONST               4 (('back', 'text_back'))
+                41          32 LOAD_CONST               4 (('back', 'text_back'))
                             34 BUILD_CONST_KEY_MAP      2
                
-                39          36 BUILD_MAP                1
+                40          36 BUILD_MAP                1
                
-                38          38 PRECALL                  1
+                39          38 PRECALL                  1
                             42 CALL                     1
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
                             56 RETURN_VALUE
                consts
                   None
                   'label'
@@ -467,86 +477,86 @@
                   ('back', 'text_back')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
                name       'palette_dark'
-               firstlineno 37
+               firstlineno 38
                lnotab 0x020118020201020102fe04ff02ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c01815a64017c01760072267c0164011900000000000000000064
                   02190000000000000000007c005f0000000000000000007c016401190000
                   000000000000006403190000000000000000007c005f0100000000000000
                   007c017c005f02000000000000000009007c00a003000000000000000000
                   00000000000000000000006400a6010000ab010000000000000000010064
                   005300230074080000000000000000000024007204010059006400530077
                   007803590077017c006a0200000000000000005300
-                47           0 RESUME                   0
+                48           0 RESUME                   0
                
-                48           2 LOAD_FAST                1 (dict)
+                49           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE    90 (to 186)
                
-                49           6 LOAD_CONST               1 ('label')
+                50           6 LOAD_CONST               1 ('label')
                              8 LOAD_FAST                1 (dict)
                             10 CONTAINS_OP              0
                             12 POP_JUMP_FORWARD_IF_FALSE    38 (to 90)
                
-                50          14 LOAD_FAST                1 (dict)
+                51          14 LOAD_FAST                1 (dict)
                             16 LOAD_CONST               1 ('label')
                             18 BINARY_SUBSCR
                             28 LOAD_CONST               2 ('back')
                             30 BINARY_SUBSCR
                             40 LOAD_FAST                0 (self)
                             42 STORE_ATTR               0 (label_back)
                
-                51          52 LOAD_FAST                1 (dict)
+                52          52 LOAD_FAST                1 (dict)
                             54 LOAD_CONST               1 ('label')
                             56 BINARY_SUBSCR
                             66 LOAD_CONST               3 ('text_back')
                             68 BINARY_SUBSCR
                             78 LOAD_FAST                0 (self)
                             80 STORE_ATTR               1 (label_text_back)
                
-                53     >>   90 LOAD_FAST                1 (dict)
+                54     >>   90 LOAD_FAST                1 (dict)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               2 (_palette)
                
-                55         104 NOP
+                56         104 NOP
                
-                56         106 LOAD_FAST                0 (self)
+                57         106 LOAD_FAST                0 (self)
                            108 LOAD_METHOD              3 (_draw)
                            130 LOAD_CONST               0 (None)
                            132 PRECALL                  1
                            136 CALL                     1
                            146 POP_TOP
                            148 LOAD_CONST               0 (None)
                            150 RETURN_VALUE
                        >>  152 PUSH_EXC_INFO
                
-                57         154 LOAD_GLOBAL              8 (AttributeError)
+                58         154 LOAD_GLOBAL              8 (AttributeError)
                            166 CHECK_EXC_MATCH
                            168 POP_JUMP_FORWARD_IF_FALSE     4 (to 178)
                            170 POP_TOP
                
-                58         172 POP_EXCEPT
+                59         172 POP_EXCEPT
                            174 LOAD_CONST               0 (None)
                            176 RETURN_VALUE
                
-                57     >>  178 RERAISE                  0
+                58     >>  178 RERAISE                  0
                        >>  180 COPY                     3
                            182 POP_EXCEPT
                            184 RERAISE                  1
                
-                60     >>  186 LOAD_FAST                0 (self)
+                61     >>  186 LOAD_FAST                0 (self)
                            188 LOAD_ATTR                2 (_palette)
                            198 RETURN_VALUE
                ExceptionTable:
                  106 to 146 -> 152 [0]
                  152 to 170 -> 180 [1] lasti
                  178 to 178 -> 180 [1] lasti
                consts
@@ -556,144 +566,146 @@
                   'text_back'
                names      ('label_back', 'label_text_back', '_palette', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
                name       'palette'
-               firstlineno 47
+               firstlineno 48
                lnotab 0x020104010801260126020e0202013001120106ff0803
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'str', '__init__', '_draw', '_other', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
          name       'AdwBasicLabel'
-         firstlineno 4
+         firstlineno 5
          lnotab 0x0c01160b080506030603060a060a
       'AdwBasicLabel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          63           0 RESUME                   0
+          64           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwLabel')
                        8 STORE_NAME               2 (__qualname__)
          
-          64          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\label.py", line 64>)
+          65          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\label.py", line 65>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwLabel'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                64           0 RESUME                   0
+                65           0 RESUME                   0
                
-                65           2 LOAD_FAST                0 (self)
+                66           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
                name       'default_palette'
-               firstlineno 64
+               firstlineno 65
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
          name       'AdwLabel'
-         firstlineno 63
+         firstlineno 64
          lnotab 0x0a01
       'AdwLabel'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-          68           0 RESUME                   0
+          69           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDarkLabel')
                        8 STORE_NAME               2 (__qualname__)
          
-          69          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\label.py", line 69>)
+          70          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\widgets\label.py", line 70>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDarkLabel'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-                69           0 RESUME                   0
+                70           0 RESUME                   0
                
-                70           2 LOAD_FAST                0 (self)
+                71           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
                name       'default_palette'
-               firstlineno 69
+               firstlineno 70
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
          name       'AdwDarkLabel'
-         firstlineno 68
+         firstlineno 69
          lnotab 0x0a01
       'AdwDarkLabel'
       '__main__'
       ('Tk',)
       'hello'
       ('text',)
       None
-   names      ('tkinter', 'Label', 'AdwBasicLabel', 'AdwLabel', 'AdwDarkLabel', '__name__', 'Tk', 'root', 'label', 'pack', 'label2', 'mainloop')
+   names      ('tkinter', 'Label', 'tkadw.layout', 'AdwLayout', 'AdwBasicLabel', 'AdwLabel', 'AdwDarkLabel', '__name__', 'Tk', 'root', 'label', 'pack', 'label2', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\widgets\\label.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c031c3b1c051c050c010c01140118012801180128012cf9
+   lnotab
+      0x00ff02010c010c031e3b1c051c050c010c01140118012801180128012c
+      f9
```

### Comparing `tkadw-0.3.3/tkadw/windows/widgets/__pycache__/mdi.cpython-311.pyc` & `tkadw-0.3.5/tkadw/windows/widgets/__pycache__/mdi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/tkadw/windows/widgets/adw.py` & `tkadw-0.3.5/tkadw/windows/widgets/adw.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
             icon = adwite_dark_photo()
         elif icon.lower() == "light":
             icon = adwite_light_photo()
         self.iconphoto(False, icon)
 
         self.default_palette()
 
+        self.windark = windark
+
         from sys import platform
         if platform == "win32" and windark:
             try:
                 from ctypes import windll, wintypes, byref, c_int, sizeof
                 value = c_int(1)
                 windll.dwmapi.DwmSetWindowAttribute(
                     windll.user32.GetParent(self.winfo_id()),  # 窗柄 输入值
```

### Comparing `tkadw-0.3.3/tkadw/windows/widgets/label.py` & `tkadw-0.3.5/tkadw/windows/widgets/label.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from tkinter import Label
+from tkadw.layout import AdwLayout
 
 
-class AdwBasicLabel(Label):
+class AdwBasicLabel(Label, AdwLayout):
     def __init__(self, *args, text: str = "", **kwargs):
         super().__init__(*args, text=text, **kwargs)
 
         self._other()
 
         self.default_palette()
```

### Comparing `tkadw-0.3.3/tkadw/windows/widgets/mdi.py` & `tkadw-0.3.5/tkadw/windows/widgets/mdi.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.3/PKG-INFO` & `tkadw-0.3.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkadw
-Version: 0.3.3
+Version: 0.3.5
 Summary: extra for tkinter
 License: MIT
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -96,7 +96,15 @@
 > 
 >> `322` 添加`metro`主题
 
 > `0.3.3`
 >> `331` 修复`AdwDrawFrame`的边框宽度问题
 > 
 >> `332` 增加主题属性`AdwDrawFrame` `padding`
+
+> `0.3.4`
+>> `341` 为`AdwTButton`增添新样式`win11_accent_light` `win11_accent_dark`
+
+> `0.3.5`
+>> `351`补充`AdwTCircularButton`主题组件
+> 
+>> `352`增添新快速布局`row`、`coloumn`以及高级布局`put`，所有可视化组件已继承布局类。
```

