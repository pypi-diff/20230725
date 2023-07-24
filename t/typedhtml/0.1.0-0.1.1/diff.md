# Comparing `tmp/typedhtml-0.1.0.tar.gz` & `tmp/typedhtml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedhtml-0.1.0.tar", max compression
+gzip compressed data, was "typedhtml-0.1.1.tar", max compression
```

## Comparing `typedhtml-0.1.0.tar` & `typedhtml-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0        0 2023-07-21 23:03:24.783891 typedhtml-0.1.0/README.md
--rw-r--r--   0        0        0      345 2023-07-24 22:25:09.775370 typedhtml-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      154 2023-07-23 17:35:32.083325 typedhtml-0.1.0/typedhtml/__init__.py
--rw-r--r--   0        0        0    16611 2023-07-23 19:34:38.466445 typedhtml-0.1.0/typedhtml/attributes.py
--rw-r--r--   0        0        0      661 2023-07-23 19:48:40.440999 typedhtml-0.1.0/typedhtml/document.py
--rw-r--r--   0        0        0     2969 2023-07-22 18:24:49.759970 typedhtml-0.1.0/typedhtml/events.py
--rw-r--r--   0        0        0     7348 2023-07-23 19:50:40.425730 typedhtml-0.1.0/typedhtml/globals.py
--rw-r--r--   0        0        0     1211 2023-07-23 06:34:06.643229 typedhtml-0.1.0/typedhtml/svg.py
--rw-r--r--   0        0        0    32122 2023-07-23 20:49:38.749637 typedhtml-0.1.0/typedhtml/tags.py
--rw-r--r--   0        0        0     5949 2023-07-24 21:15:57.863382 typedhtml-0.1.0/typedhtml/ui5/__init__.py
--rw-r--r--   0        0        0     3264 2023-07-24 03:41:38.489987 typedhtml-0.1.0/typedhtml/ui5/avatar.py
--rw-r--r--   0        0        0      863 2023-07-24 03:38:24.465498 typedhtml-0.1.0/typedhtml/ui5/badge.py
--rw-r--r--   0        0        0      740 2023-07-24 21:10:42.887836 typedhtml-0.1.0/typedhtml/ui5/base.py
--rw-r--r--   0        0        0     1354 2023-07-24 03:41:10.194619 typedhtml-0.1.0/typedhtml/ui5/breadcrumbs.py
--rw-r--r--   0        0        0      797 2023-07-24 03:42:17.102817 typedhtml-0.1.0/typedhtml/ui5/busy_indicator.py
--rw-r--r--   0        0        0     1091 2023-07-24 03:42:46.370478 typedhtml-0.1.0/typedhtml/ui5/button.py
--rw-r--r--   0        0        0     1214 2023-07-24 21:22:07.958588 typedhtml-0.1.0/typedhtml/ui5/calendar.py
--rw-r--r--   0        0        0     1424 2023-07-24 03:44:35.261001 typedhtml-0.1.0/typedhtml/ui5/card.py
--rw-r--r--   0        0        0     1356 2023-07-24 03:44:57.515274 typedhtml-0.1.0/typedhtml/ui5/carousel.py
--rw-r--r--   0        0        0     1405 2023-07-24 03:45:38.605099 typedhtml-0.1.0/typedhtml/ui5/checkbox.py
--rw-r--r--   0        0        0     1551 2023-07-24 03:48:24.851505 typedhtml-0.1.0/typedhtml/ui5/color_palette.py
--rw-r--r--   0        0        0      619 2023-07-24 03:48:50.205563 typedhtml-0.1.0/typedhtml/ui5/color_picker.py
--rw-r--r--   0        0        0     1018 2023-07-24 03:49:37.145966 typedhtml-0.1.0/typedhtml/ui5/combobox.py
--rw-r--r--   0        0        0     1062 2023-07-24 03:50:02.077503 typedhtml-0.1.0/typedhtml/ui5/datepicker.py
--rw-r--r--   0        0        0      797 2023-07-24 21:22:33.226998 typedhtml-0.1.0/typedhtml/ui5/daterange_picker.py
--rw-r--r--   0        0        0      634 2023-07-24 03:51:37.839555 typedhtml-0.1.0/typedhtml/ui5/datetime_picker.py
--rw-r--r--   0        0        0      724 2023-07-24 03:51:59.287201 typedhtml-0.1.0/typedhtml/ui5/dialog.py
--rw-r--r--   0        0        0     1018 2023-07-24 03:52:52.259960 typedhtml-0.1.0/typedhtml/ui5/file_uploader.py
--rw-r--r--   0        0        0      989 2023-07-24 03:53:09.125464 typedhtml-0.1.0/typedhtml/ui5/icon.py
--rw-r--r--   0        0        0     1104 2023-07-24 18:46:05.721707 typedhtml-0.1.0/typedhtml/ui5/input.py
--rw-r--r--   0        0        0      677 2023-07-24 03:35:27.924512 typedhtml-0.1.0/typedhtml/ui5/label.py
--rw-r--r--   0        0        0      848 2023-07-24 04:19:28.264763 typedhtml-0.1.0/typedhtml/ui5/link.py
--rw-r--r--   0        0        0     2336 2023-07-24 04:55:43.979158 typedhtml-0.1.0/typedhtml/ui5/list.py
--rw-r--r--   0        0        0     1292 2023-07-24 05:07:02.147480 typedhtml-0.1.0/typedhtml/ui5/menu.py
--rw-r--r--   0        0        0      934 2023-07-24 05:11:38.448763 typedhtml-0.1.0/typedhtml/ui5/message_strip.py
--rw-r--r--   0        0        0     2111 2023-07-24 05:32:56.437095 typedhtml-0.1.0/typedhtml/ui5/multi_combobox.py
--rw-r--r--   0        0        0     1217 2023-07-24 05:47:28.390516 typedhtml-0.1.0/typedhtml/ui5/multi_input.py
--rw-r--r--   0        0        0      786 2023-07-24 05:56:13.272720 typedhtml-0.1.0/typedhtml/ui5/panel.py
--rw-r--r--   0        0        0     1049 2023-07-24 16:47:51.776836 typedhtml-0.1.0/typedhtml/ui5/popover.py
--rw-r--r--   0        0        0      813 2023-07-24 16:53:02.111474 typedhtml-0.1.0/typedhtml/ui5/progress.py
--rw-r--r--   0        0        0     1147 2023-07-24 17:23:34.365913 typedhtml-0.1.0/typedhtml/ui5/radio.py
--rw-r--r--   0        0        0      739 2023-07-24 17:26:16.577498 typedhtml-0.1.0/typedhtml/ui5/range_slider.py
--rw-r--r--   0        0        0      846 2023-07-24 17:30:46.775794 typedhtml-0.1.0/typedhtml/ui5/rating_indicator.py
--rw-r--r--   0        0        0      460 2023-07-24 19:03:12.882005 typedhtml-0.1.0/typedhtml/ui5/responsive_popover.py
--rw-r--r--   0        0        0     1240 2023-07-24 17:45:46.706947 typedhtml-0.1.0/typedhtml/ui5/segmented_button.py
--rw-r--r--   0        0        0     1330 2023-07-24 17:52:58.144971 typedhtml-0.1.0/typedhtml/ui5/select.py
--rw-r--r--   0        0        0      686 2023-07-24 18:07:42.261132 typedhtml-0.1.0/typedhtml/ui5/slider.py
--rw-r--r--   0        0        0      992 2023-07-24 18:15:29.579762 typedhtml-0.1.0/typedhtml/ui5/split_button.py
--rw-r--r--   0        0        0      925 2023-07-24 18:19:41.715572 typedhtml-0.1.0/typedhtml/ui5/step_input.py
--rw-r--r--   0        0        0      915 2023-07-24 18:23:43.502304 typedhtml-0.1.0/typedhtml/ui5/switch.py
--rw-r--r--   0        0        0     1051 2023-07-24 18:37:11.846161 typedhtml-0.1.0/typedhtml/ui5/tab_container.py
--rw-r--r--   0        0        0     2066 2023-07-24 19:41:17.961063 typedhtml-0.1.0/typedhtml/ui5/table.py
--rw-r--r--   0        0        0      904 2023-07-24 20:54:41.376476 typedhtml-0.1.0/typedhtml/ui5/textarea.py
--rw-r--r--   0        0        0      665 2023-07-24 20:57:46.970970 typedhtml-0.1.0/typedhtml/ui5/time_picker.py
--rw-r--r--   0        0        0      566 2023-07-24 21:01:29.280885 typedhtml-0.1.0/typedhtml/ui5/title.py
--rw-r--r--   0        0        0      708 2023-07-24 21:04:14.974066 typedhtml-0.1.0/typedhtml/ui5/toast.py
--rw-r--r--   0        0        0      496 2023-07-24 22:06:21.633647 typedhtml-0.1.0/typedhtml/ui5/toggle_button.py
--rw-r--r--   0        0        0     1135 2023-07-24 22:10:33.706725 typedhtml-0.1.0/typedhtml/ui5/tree.py
--rw-r--r--   0        0        0      626 2023-07-23 23:21:00.787615 typedhtml-0.1.0/typedhtml/util.py
--rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 typedhtml-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 23:03:24.783891 typedhtml-0.1.1/README.md
+-rw-r--r--   0        0        0      346 2023-07-24 23:26:57.538721 typedhtml-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-07-23 17:35:32.083325 typedhtml-0.1.1/typedhtml/__init__.py
+-rw-r--r--   0        0        0    17304 2023-07-24 23:24:43.336075 typedhtml-0.1.1/typedhtml/attributes.py
+-rw-r--r--   0        0        0      661 2023-07-23 19:48:40.440999 typedhtml-0.1.1/typedhtml/document.py
+-rw-r--r--   0        0        0     2969 2023-07-22 18:24:49.759970 typedhtml-0.1.1/typedhtml/events.py
+-rw-r--r--   0        0        0     7348 2023-07-23 19:50:40.425730 typedhtml-0.1.1/typedhtml/globals.py
+-rw-r--r--   0        0        0     1211 2023-07-23 06:34:06.643229 typedhtml-0.1.1/typedhtml/svg.py
+-rw-r--r--   0        0        0    31856 2023-07-24 23:25:41.816888 typedhtml-0.1.1/typedhtml/tags.py
+-rw-r--r--   0        0        0     5949 2023-07-24 21:15:57.863382 typedhtml-0.1.1/typedhtml/ui5/__init__.py
+-rw-r--r--   0        0        0     3264 2023-07-24 03:41:38.489987 typedhtml-0.1.1/typedhtml/ui5/avatar.py
+-rw-r--r--   0        0        0      863 2023-07-24 03:38:24.465498 typedhtml-0.1.1/typedhtml/ui5/badge.py
+-rw-r--r--   0        0        0      740 2023-07-24 21:10:42.887836 typedhtml-0.1.1/typedhtml/ui5/base.py
+-rw-r--r--   0        0        0     1354 2023-07-24 03:41:10.194619 typedhtml-0.1.1/typedhtml/ui5/breadcrumbs.py
+-rw-r--r--   0        0        0      797 2023-07-24 03:42:17.102817 typedhtml-0.1.1/typedhtml/ui5/busy_indicator.py
+-rw-r--r--   0        0        0     1091 2023-07-24 03:42:46.370478 typedhtml-0.1.1/typedhtml/ui5/button.py
+-rw-r--r--   0        0        0     1214 2023-07-24 21:22:07.958588 typedhtml-0.1.1/typedhtml/ui5/calendar.py
+-rw-r--r--   0        0        0     1424 2023-07-24 03:44:35.261001 typedhtml-0.1.1/typedhtml/ui5/card.py
+-rw-r--r--   0        0        0     1356 2023-07-24 03:44:57.515274 typedhtml-0.1.1/typedhtml/ui5/carousel.py
+-rw-r--r--   0        0        0     1405 2023-07-24 03:45:38.605099 typedhtml-0.1.1/typedhtml/ui5/checkbox.py
+-rw-r--r--   0        0        0     1551 2023-07-24 03:48:24.851505 typedhtml-0.1.1/typedhtml/ui5/color_palette.py
+-rw-r--r--   0        0        0      619 2023-07-24 03:48:50.205563 typedhtml-0.1.1/typedhtml/ui5/color_picker.py
+-rw-r--r--   0        0        0     1018 2023-07-24 03:49:37.145966 typedhtml-0.1.1/typedhtml/ui5/combobox.py
+-rw-r--r--   0        0        0     1062 2023-07-24 03:50:02.077503 typedhtml-0.1.1/typedhtml/ui5/datepicker.py
+-rw-r--r--   0        0        0      797 2023-07-24 21:22:33.226998 typedhtml-0.1.1/typedhtml/ui5/daterange_picker.py
+-rw-r--r--   0        0        0      634 2023-07-24 03:51:37.839555 typedhtml-0.1.1/typedhtml/ui5/datetime_picker.py
+-rw-r--r--   0        0        0      724 2023-07-24 03:51:59.287201 typedhtml-0.1.1/typedhtml/ui5/dialog.py
+-rw-r--r--   0        0        0     1018 2023-07-24 03:52:52.259960 typedhtml-0.1.1/typedhtml/ui5/file_uploader.py
+-rw-r--r--   0        0        0      989 2023-07-24 03:53:09.125464 typedhtml-0.1.1/typedhtml/ui5/icon.py
+-rw-r--r--   0        0        0     1104 2023-07-24 18:46:05.721707 typedhtml-0.1.1/typedhtml/ui5/input.py
+-rw-r--r--   0        0        0      677 2023-07-24 03:35:27.924512 typedhtml-0.1.1/typedhtml/ui5/label.py
+-rw-r--r--   0        0        0      848 2023-07-24 04:19:28.264763 typedhtml-0.1.1/typedhtml/ui5/link.py
+-rw-r--r--   0        0        0     2336 2023-07-24 04:55:43.979158 typedhtml-0.1.1/typedhtml/ui5/list.py
+-rw-r--r--   0        0        0     1292 2023-07-24 05:07:02.147480 typedhtml-0.1.1/typedhtml/ui5/menu.py
+-rw-r--r--   0        0        0      934 2023-07-24 05:11:38.448763 typedhtml-0.1.1/typedhtml/ui5/message_strip.py
+-rw-r--r--   0        0        0     2111 2023-07-24 05:32:56.437095 typedhtml-0.1.1/typedhtml/ui5/multi_combobox.py
+-rw-r--r--   0        0        0     1217 2023-07-24 05:47:28.390516 typedhtml-0.1.1/typedhtml/ui5/multi_input.py
+-rw-r--r--   0        0        0      786 2023-07-24 05:56:13.272720 typedhtml-0.1.1/typedhtml/ui5/panel.py
+-rw-r--r--   0        0        0     1049 2023-07-24 16:47:51.776836 typedhtml-0.1.1/typedhtml/ui5/popover.py
+-rw-r--r--   0        0        0      813 2023-07-24 16:53:02.111474 typedhtml-0.1.1/typedhtml/ui5/progress.py
+-rw-r--r--   0        0        0     1147 2023-07-24 17:23:34.365913 typedhtml-0.1.1/typedhtml/ui5/radio.py
+-rw-r--r--   0        0        0      739 2023-07-24 17:26:16.577498 typedhtml-0.1.1/typedhtml/ui5/range_slider.py
+-rw-r--r--   0        0        0      846 2023-07-24 17:30:46.775794 typedhtml-0.1.1/typedhtml/ui5/rating_indicator.py
+-rw-r--r--   0        0        0      460 2023-07-24 19:03:12.882005 typedhtml-0.1.1/typedhtml/ui5/responsive_popover.py
+-rw-r--r--   0        0        0     1240 2023-07-24 17:45:46.706947 typedhtml-0.1.1/typedhtml/ui5/segmented_button.py
+-rw-r--r--   0        0        0     1330 2023-07-24 17:52:58.144971 typedhtml-0.1.1/typedhtml/ui5/select.py
+-rw-r--r--   0        0        0      686 2023-07-24 18:07:42.261132 typedhtml-0.1.1/typedhtml/ui5/slider.py
+-rw-r--r--   0        0        0      992 2023-07-24 18:15:29.579762 typedhtml-0.1.1/typedhtml/ui5/split_button.py
+-rw-r--r--   0        0        0      925 2023-07-24 18:19:41.715572 typedhtml-0.1.1/typedhtml/ui5/step_input.py
+-rw-r--r--   0        0        0      915 2023-07-24 18:23:43.502304 typedhtml-0.1.1/typedhtml/ui5/switch.py
+-rw-r--r--   0        0        0     1051 2023-07-24 18:37:11.846161 typedhtml-0.1.1/typedhtml/ui5/tab_container.py
+-rw-r--r--   0        0        0     2066 2023-07-24 19:41:17.961063 typedhtml-0.1.1/typedhtml/ui5/table.py
+-rw-r--r--   0        0        0      904 2023-07-24 20:54:41.376476 typedhtml-0.1.1/typedhtml/ui5/textarea.py
+-rw-r--r--   0        0        0      665 2023-07-24 20:57:46.970970 typedhtml-0.1.1/typedhtml/ui5/time_picker.py
+-rw-r--r--   0        0        0      566 2023-07-24 21:01:29.280885 typedhtml-0.1.1/typedhtml/ui5/title.py
+-rw-r--r--   0        0        0      708 2023-07-24 21:04:14.974066 typedhtml-0.1.1/typedhtml/ui5/toast.py
+-rw-r--r--   0        0        0      496 2023-07-24 22:06:21.633647 typedhtml-0.1.1/typedhtml/ui5/toggle_button.py
+-rw-r--r--   0        0        0     1135 2023-07-24 22:10:33.706725 typedhtml-0.1.1/typedhtml/ui5/tree.py
+-rw-r--r--   0        0        0      626 2023-07-23 23:21:00.787615 typedhtml-0.1.1/typedhtml/util.py
+-rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 typedhtml-0.1.1/PKG-INFO
```

### Comparing `typedhtml-0.1.0/typedhtml/attributes.py` & `typedhtml-0.1.1/typedhtml/attributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 from typing import Literal
 
 from typedhtml.globals import GLOBAL_ATTR
 
 __all__ = [
+    "script_attr",
     "slot_attr",
     "meter_attr",
     "output_attr",
     "option_attr",
     "optgroup_attr",
     "base_attr",
     "html_attr",
@@ -663,7 +664,36 @@
 
 class data_attr(GLOBAL_ATTR, total=False):
     value: str
 
 
 class slot_attr(GLOBAL_ATTR, total=False):
     name: str
+
+
+class script_attr(GLOBAL_ATTR, total=False):
+    async_: bool
+    crossorigin: CrossOrigin
+    defer: bool
+    integrity: str
+    nomodule: bool
+    nonce: str
+    fetchpriority: Literal["auto", "high", "low"]
+    referrerpolicy: Literal[
+        "no-referrer",
+        "no-referrer-when-downgrade",
+        "origin",
+        "origin-when-cross-origin",
+        "unsafe-url",
+        "same-origin",
+        "strict-origin",
+        "strict-origin-when-cross-origin",
+    ]
+    src: str
+    type: Literal[
+        "module",
+        "text/javascript",
+        "text/ecmascript",
+        "application/javascript",
+        "application/ecmascript",
+        "importmap",
+    ]
```

### Comparing `typedhtml-0.1.0/typedhtml/document.py` & `typedhtml-0.1.1/typedhtml/document.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/events.py` & `typedhtml-0.1.1/typedhtml/events.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/globals.py` & `typedhtml-0.1.1/typedhtml/globals.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/svg.py` & `typedhtml-0.1.1/typedhtml/svg.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/tags.py` & `typedhtml-0.1.1/typedhtml/tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 
 from dominate.tags import comment as comment_tag
 from dominate.tags import html_tag
 from dominate.tags import time_ as time_tag
 from dominate.tags import title as title_tag
 
 from .attributes import *
-from .attributes import (
-    details_attr,
-    meter_attr,  # noqa: F403
-    textarea_attr,
-)
+from .attributes import meter_attr  # noqa: F403
+from .attributes import details_attr, textarea_attr
 from .globals import GLOBAL_ATTR, extrakeys
 
 
 def _get_attr(data: Any):
     if isinstance(data, dict):
         return list(cast(Mapping[str, str], data).keys())[0]
     return str(data)
@@ -73,15 +70,15 @@
 
 class a(typed_tag):
     """
     The a element represents a hyperlink.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[a_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[a_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class abbr(typed_tag):
     """the abbr element represents an abbreviation or acronym, optionally with its
     expansion. The title attribute may be used to provide an expansion of the
@@ -104,15 +101,15 @@
 
 class html(typed_tag):
     """
     Creates a new html tag instance.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[html_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[html_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class head(typed_tag):
     """
     The head element represents a collection of metadata for the document.
@@ -138,53 +135,53 @@
     The base element allows authors to specify the document base URL for the
     purposes of resolving relative URLs, and the name of the default browsing
     context for the purposes of following hyperlinks. The element does not
     represent any content beyond this information.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[base_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[base_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
     is_single = True
 
 
 class link(typed_tag):
     """
     The link element allows authors to link their document to other resources.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[link_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[link_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
     is_single = True
 
 
 class meta(typed_tag):
     """
     The meta element represents various kinds of metadata that cannot be
     expressed using the title, base, link, style, and script elements.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[meta_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[meta_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
     is_single = True
 
 
 class style(typed_tag):
     """The script element allows authors to include dynamic script and data"""
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[style_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[style_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
     is_pretty = False
 
 
 class noscript(typed_tag):
@@ -200,15 +197,15 @@
 
 class body(typed_tag):
     """
     The body element represents the content of the document.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[body_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[body_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class main(typed_tag):
     """
     The main element represents the main content of the body of a document or
@@ -362,26 +359,26 @@
 
 class blockquote(typed_tag):
     """
     The blockquote element represents a section that is quoted from another source.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[blockquote_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[blockquote_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class ol(typed_tag):
     """the ol element represents a list of items, where the items have been
     intentionally ordered,
     such that changing the order would change the meaning of the document."""
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[ol_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[ol_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class ul(typed_tag):
     """The ul element represents a list of items, where the order of the items is
     not important - that is, where changing the order would not materially change
@@ -395,15 +392,15 @@
     The li element represents a list item. If its parent element is an ol, or ul
     element, then the element is an item of the parent element's list, as defined
     for those elements. Otherwise, the list item has no defined list-related
     relationship to any other li element.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[li_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[li_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class dl(typed_tag):
     """
     The dl element represents an association list consisting of zero or more
@@ -490,36 +487,36 @@
     The s element represents contents that are no longer accurate or no longer
     relevant.
     """
 
     pass
 
 
-class cite(html_tag):
+class cite(typed_tag):
     """
     The cite element represents the title of a work (e.g. a book, a paper, an
     essay, a poem, a score, a song, a script, a film, a TV show, a game, a
     sculpture, a painting, a theatre production, a play, an opera, a musical, an
     exhibition, a legal case report, etc). This can be a work that is being
     quoted or referenced in detail (i.e. a citation), or it can just be a work
     that is mentioned in passing.
     """
 
     pass
 
 
-class q(html_tag):
+class q(typed_tag):
     """
     The q element represents some phrasing content quoted from another source.
     """
 
     pass
 
 
-class dfn(html_tag):
+class dfn(typed_tag):
     """
     The dfn element represents the defining instance of a term. The paragraph,
     description list group, or section that is the nearest ancestor of the dfn
     element must also contain the definition(s) for the term given by the dfn
     element.
     """
 
@@ -530,15 +527,15 @@
     """
     The time element represents either a time on a 24 hour clock, or a precise
     date in the proleptic Gregorian calendar, optionally with a time and a
     time-zone offset.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[time_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[time_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class code(typed_tag):
     """
     The code element represents a fragment of computer code. This could be an
@@ -732,156 +729,144 @@
 
 
 class del_(typed_tag):
     """
     The del element represents a removal from the document.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[del_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[del_attr]) -> None:
+        super().__init__(*args, **kwargs)
+
+
+class script(typed_tag):
+    """
+    The script element allows authors to include dynamic script and data blocks
+    in their documents. The element does not represent content for the user.
+    """
+
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[script_attr]) -> None:
         super().__init__(*args, **kwargs)
 
+    is_pretty = False
+
 
 class img(typed_tag):
     """
     An img element represents an image.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[img_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[img_attr]) -> None:
         super().__init__(*args, **kwargs)
 
     is_single = True
 
 
 class iframe(typed_tag):
     """
     The iframe element represents a nested browsing context.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[iframe_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[iframe_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class embed(typed_tag):
     """
     The embed element represents an integration point for an external (typically
     non-HTML) application or interactive content.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[embed_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[embed_attr]) -> None:
         super().__init__(*args, **kwargs)
 
     is_single = True
 
 
 class object_(typed_tag):
     """
     The object element can represent an external resource, which, depending on
     the type of the resource, will either be treated as an image, as a nested
     browsing context, or as an external resource to be processed by a plugin.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[object_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[object_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class video(typed_tag):
     """
     A video element is used for playing videos or movies, and audio files with
     captions.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[video_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[video_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class audio(typed_tag):
     """
     An audio element represents a sound or audio stream.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[audio_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[audio_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class source(typed_tag):
     """
     The source element allows authors to specify multiple alternative media
     resources for media elements. It does not represent anything on its own.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[source_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[source_attr]) -> None:
         super().__init__(*args, **kwargs)
 
     is_single = True
 
 
 class track(typed_tag):
     """
     The track element allows authors to specify explicit external timed text
     tracks for media elements. It does not represent anything on its own.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[track_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[track_attr]) -> None:
         super().__init__(*args, **kwargs)
 
     is_single = True
 
 
 class canvas(typed_tag):
     """
     The canvas element provides scripts with a resolution-dependent bitmap
     canvas, which can be used for rendering graphs, game graphics, or other
     visual images on the fly.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[canvas_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[canvas_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class map_(typed_tag):
     """
     The map element, in conjunction with any area element descendants, defines an
     image map. The element represents its children.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[map_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[map_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class area(typed_tag):
     """
     The area element represents either a hyperlink with some text and a
     corresponding area on an image map, or a dead area on an image map.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[area_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[area_attr]) -> None:
         super().__init__(*args, **kwargs)
 
     is_single = True
 
 
 class table(typed_tag):
     """
@@ -904,28 +889,28 @@
 class colgroup(typed_tag):
     """
     The colgroup element represents a group of one or more columns in the table
     that is its parent, if it has a parent and that is a table element.
     """
 
     def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[colgroup_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[colgroup_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class col(typed_tag):
     """
     If a col element has a parent and that is a colgroup element that itself has
       a parent that is a table element, then the col element represents one or more
       columns in the column group represented by that colgroup.
     """
 
     def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[colgroup_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[colgroup_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class tbody(typed_tag):
     """
     The tbody element represents a block of rows that consist of a body of data
@@ -965,53 +950,47 @@
 
 
 class td(typed_tag):
     """
     The td element represents a data cell in a table.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[td_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[td_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class th(typed_tag):
     """
     The th element represents a header cell in a table.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[th_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[th_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 # Forms
 class form(typed_tag):
     """
     The form element represents a collection of form-associated elements, some of
     which can represent editable values that can be submitted to a server for
     processing.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[form_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[form_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class fieldset(typed_tag):
     """
     The fieldset element represents a set of form controls optionally grouped
     under a common name.
     """
 
     def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[fieldset_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[fieldset_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class legend(typed_tag):
     """
     The legend element represents a caption for the rest of the contents of the
@@ -1025,55 +1004,49 @@
     """
     The label represents a caption in a user interface. The caption can be
     associated with a specific form control, known as the label element's labeled
     control, either using for attribute, or by putting the form control inside
     the label element itself.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[label_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[label_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class input_(typed_tag):
     """
     The input element represents a typed data field, usually with a form control
     to allow the user to edit the data.
     """
 
     def __init__(  # type: ignore
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[input_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[input_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
     is_single = True
 
 
 class button(typed_tag):
     """
     The button element represents a button. If the element is not disabled, then
     the user agent should allow the user to activate the button.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[button_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[button_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class select(typed_tag):
     """
     The select element represents a control for selecting amongst a set of
     options.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[select_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[select_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class datalist(typed_tag):
     """
     The datalist element represents a set of option elements that represent
     predefined options for other controls. The contents of the element represents
@@ -1088,94 +1061,86 @@
 class optgroup(typed_tag):
     """
     The optgroup element represents a group of option elements with a common
     label.
     """
 
     def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[optgroup_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[optgroup_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class option(typed_tag):
     """
     The option element represents an option in a select element or as part of a
     list of suggestions in a datalist element.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[option_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[option_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class textarea(typed_tag):
     """
     The textarea element represents a multiline plain text edit control for the
     element's raw value. The contents of the control represent the control's
     default value.
     """
 
     def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[textarea_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[textarea_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class output(typed_tag):
     """
     The output element represents the result of a calculation.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[output_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[output_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
-class progress(html_tag):
+class progress(typed_tag):
     """
     The progress element represents the completion progress of a task. The
     progress is either indeterminate, indicating that progress is being made but
     that it is not clear how much more work remains to be done before the task is
     complete (e.g. because the task is waiting for a remote host to respond), or
     the progress is a number in the range zero to a maximum, giving the fraction
     of work that has so far been completed.
     """
 
     def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[progress_attr]
+        self: typing.Self, *args: Any, **kwargs: Unpack[progress_attr]
     ) -> None:
         super().__init__(*args, **kwargs)
 
 
 class meter(typed_tag):
     """
     The meter element represents a scalar measurement within a known range, or a
     fractional value; for example disk usage, the relevance of a query result, or
     the fraction of a voting population to have selected a particular candidate.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[meter_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[meter_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 # Interactive elements
 class details(typed_tag):
     """
     The details element represents a disclosure widget from which the user can
     obtain additional information or controls.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[details_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[details_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class summary(typed_tag):
     """
     The summary element represents a summary, caption, or legend for the rest of
     the contents of the summary element's parent details element, if any.
@@ -1194,17 +1159,15 @@
 
 class data(typed_tag):
     """
     The data element represents its contents, along with a machine-readable form
     of those contents in the value attribute.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[data_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[data_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class picture(typed_tag):
     """
     The <picture> HTML element contains zero or more <source> elements and one <img>
     element
@@ -1217,17 +1180,15 @@
 class slot(typed_tag):
     """
     The slot HTML element—part of the Web Components technology suite—is a placeholder
     inside a web component that you can fill with your own markup, which lets you
     create separate DOM trees and present them together.
     """
 
-    def __init__(
-        self: typing.Self, *args: tuple[Any], **kwargs: Unpack[slot_attr]
-    ) -> None:
+    def __init__(self: typing.Self, *args: Any, **kwargs: Unpack[slot_attr]) -> None:
         super().__init__(*args, **kwargs)
 
 
 class template(typed_tag):
     """The <template> HTML element is a mechanism for holding HTML that is not to be
     rendered immediately when a page is loaded but may be instantiated subsequently
     during runtime using JavaScript.
```

### Comparing `typedhtml-0.1.0/typedhtml/ui5/__init__.py` & `typedhtml-0.1.1/typedhtml/ui5/__init__.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/avatar.py` & `typedhtml-0.1.1/typedhtml/ui5/avatar.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/badge.py` & `typedhtml-0.1.1/typedhtml/ui5/badge.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/base.py` & `typedhtml-0.1.1/typedhtml/ui5/base.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/breadcrumbs.py` & `typedhtml-0.1.1/typedhtml/ui5/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/busy_indicator.py` & `typedhtml-0.1.1/typedhtml/ui5/busy_indicator.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/button.py` & `typedhtml-0.1.1/typedhtml/ui5/button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/calendar.py` & `typedhtml-0.1.1/typedhtml/ui5/calendar.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/card.py` & `typedhtml-0.1.1/typedhtml/ui5/card.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/carousel.py` & `typedhtml-0.1.1/typedhtml/ui5/carousel.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/checkbox.py` & `typedhtml-0.1.1/typedhtml/ui5/checkbox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/color_palette.py` & `typedhtml-0.1.1/typedhtml/ui5/color_palette.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/color_picker.py` & `typedhtml-0.1.1/typedhtml/ui5/color_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/combobox.py` & `typedhtml-0.1.1/typedhtml/ui5/combobox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/datepicker.py` & `typedhtml-0.1.1/typedhtml/ui5/datepicker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/daterange_picker.py` & `typedhtml-0.1.1/typedhtml/ui5/daterange_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/datetime_picker.py` & `typedhtml-0.1.1/typedhtml/ui5/datetime_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/dialog.py` & `typedhtml-0.1.1/typedhtml/ui5/dialog.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/file_uploader.py` & `typedhtml-0.1.1/typedhtml/ui5/file_uploader.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/icon.py` & `typedhtml-0.1.1/typedhtml/ui5/icon.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/input.py` & `typedhtml-0.1.1/typedhtml/ui5/input.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/label.py` & `typedhtml-0.1.1/typedhtml/ui5/label.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/link.py` & `typedhtml-0.1.1/typedhtml/ui5/link.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/list.py` & `typedhtml-0.1.1/typedhtml/ui5/list.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/menu.py` & `typedhtml-0.1.1/typedhtml/ui5/menu.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/message_strip.py` & `typedhtml-0.1.1/typedhtml/ui5/message_strip.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/multi_combobox.py` & `typedhtml-0.1.1/typedhtml/ui5/multi_combobox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/multi_input.py` & `typedhtml-0.1.1/typedhtml/ui5/multi_input.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/panel.py` & `typedhtml-0.1.1/typedhtml/ui5/panel.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/popover.py` & `typedhtml-0.1.1/typedhtml/ui5/popover.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/progress.py` & `typedhtml-0.1.1/typedhtml/ui5/progress.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/radio.py` & `typedhtml-0.1.1/typedhtml/ui5/radio.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/range_slider.py` & `typedhtml-0.1.1/typedhtml/ui5/range_slider.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/rating_indicator.py` & `typedhtml-0.1.1/typedhtml/ui5/rating_indicator.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/segmented_button.py` & `typedhtml-0.1.1/typedhtml/ui5/segmented_button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/select.py` & `typedhtml-0.1.1/typedhtml/ui5/select.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/slider.py` & `typedhtml-0.1.1/typedhtml/ui5/slider.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/split_button.py` & `typedhtml-0.1.1/typedhtml/ui5/split_button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/step_input.py` & `typedhtml-0.1.1/typedhtml/ui5/step_input.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/switch.py` & `typedhtml-0.1.1/typedhtml/ui5/switch.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/tab_container.py` & `typedhtml-0.1.1/typedhtml/ui5/tab_container.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/table.py` & `typedhtml-0.1.1/typedhtml/ui5/table.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/textarea.py` & `typedhtml-0.1.1/typedhtml/ui5/textarea.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/time_picker.py` & `typedhtml-0.1.1/typedhtml/ui5/time_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/title.py` & `typedhtml-0.1.1/typedhtml/ui5/title.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/toast.py` & `typedhtml-0.1.1/typedhtml/ui5/toast.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/ui5/tree.py` & `typedhtml-0.1.1/typedhtml/ui5/tree.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.1.0/typedhtml/util.py` & `typedhtml-0.1.1/typedhtml/util.py`

 * *Files identical despite different names*

