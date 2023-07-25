# Comparing `tmp/pyrosimple-2.9.0.tar.gz` & `tmp/pyrosimple-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosimple-2.9.0.tar", max compression
+gzip compressed data, was "pyrosimple-2.9.1.tar", max compression
```

## Comparing `pyrosimple-2.9.0.tar` & `pyrosimple-2.9.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     2131 2023-04-13 23:28:24.964236 pyrosimple-2.9.0/README.md
--rw-r--r--   0        0        0     3349 2023-07-02 14:02:08.845891 pyrosimple-2.9.0/pyproject.toml
--rw-r--r--   0        0        0      538 2023-04-13 23:28:24.974236 pyrosimple-2.9.0/src/pyrosimple/__init__.py
--rw-r--r--   0        0        0     8778 2023-05-20 14:13:17.963479 pyrosimple-2.9.0/src/pyrosimple/config.py
--rw-r--r--   0        0        0       67 2023-04-13 23:29:22.257480 pyrosimple-2.9.0/src/pyrosimple/data/__init__.py
--rw-r--r--   0        0        0    10194 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/data/full-example.rc
--rw-r--r--   0        0        0     1273 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/error.py
--rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/io/__init__.py
--rw-r--r--   0        0        0     8666 2023-06-13 22:46:07.960229 pyrosimple-2.9.0/src/pyrosimple/io/scgi.py
--rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/__init__.py
--rw-r--r--   0        0        0     2963 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/action.py
--rw-r--r--   0        0        0     2977 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/base.py
--rw-r--r--   0        0        0     9444 2023-04-13 23:29:22.257480 pyrosimple-2.9.0/src/pyrosimple/job/metrics.py
--rw-r--r--   0        0        0     1691 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/move_path.py
--rw-r--r--   0        0        0     1743 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/move_torrent.py
--rw-r--r--   0        0        0     4192 2023-04-29 17:58:28.391573 pyrosimple-2.9.0/src/pyrosimple/job/queue.py
--rw-r--r--   0        0        0     9954 2023-04-13 23:29:54.100762 pyrosimple-2.9.0/src/pyrosimple/job/watch.py
--rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/py.typed
--rw-r--r--   0        0        0      112 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/scripts/__init__.py
--rw-r--r--   0        0        0     8094 2023-04-29 17:15:41.825951 pyrosimple-2.9.0/src/pyrosimple/scripts/base.py
--rw-r--r--   0        0        0    17593 2023-04-13 23:38:22.673176 pyrosimple-2.9.0/src/pyrosimple/scripts/chtor.py
--rw-r--r--   0        0        0     6590 2023-04-13 23:29:22.260813 pyrosimple-2.9.0/src/pyrosimple/scripts/lstor.py
--rw-r--r--   0        0        0     9779 2023-06-11 16:08:49.615631 pyrosimple-2.9.0/src/pyrosimple/scripts/mktor.py
--rw-r--r--   0        0        0    13632 2023-04-29 15:30:45.910385 pyrosimple-2.9.0/src/pyrosimple/scripts/pyroadmin.py
--rw-r--r--   0        0        0     9555 2023-04-13 23:29:22.260813 pyrosimple-2.9.0/src/pyrosimple/scripts/pyrotorque.py
--rw-r--r--   0        0        0    36574 2023-05-31 14:56:02.708905 pyrosimple-2.9.0/src/pyrosimple/scripts/rtcontrol.py
--rw-r--r--   0        0        0     8199 2023-05-30 20:05:50.210723 pyrosimple-2.9.0/src/pyrosimple/scripts/rtmv_legacy.py
--rw-r--r--   0        0        0    10373 2023-05-20 14:17:01.248156 pyrosimple-2.9.0/src/pyrosimple/scripts/rtxmlrpc.py
--rw-r--r--   0        0        0      117 2023-04-13 23:28:24.980902 pyrosimple-2.9.0/src/pyrosimple/torrent/__init__.py
--rw-r--r--   0        0        0    30483 2023-06-08 19:31:12.538264 pyrosimple-2.9.0/src/pyrosimple/torrent/engine.py
--rw-r--r--   0        0        0    37020 2023-05-20 14:01:14.338449 pyrosimple-2.9.0/src/pyrosimple/torrent/rtorrent.py
--rw-r--r--   0        0        0      118 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/ui/__init__.py
--rw-r--r--   0        0        0     2903 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/ui/categories.py
--rw-r--r--   0        0        0      122 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/util/__init__.py
--rw-r--r--   0        0        0     2164 2023-04-19 02:04:04.304690 pyrosimple-2.9.0/src/pyrosimple/util/cache.py
--rw-r--r--   0        0        0     7891 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/util/fmt.py
--rw-r--r--   0        0        0      459 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/util/logutil.py
--rw-r--r--   0        0        0    32171 2023-06-24 12:58:29.919468 pyrosimple-2.9.0/src/pyrosimple/util/matching.py
--rw-r--r--   0        0        0    26411 2023-04-13 23:29:22.267480 pyrosimple-2.9.0/src/pyrosimple/util/metafile.py
--rw-r--r--   0        0        0     2124 2023-05-30 20:07:35.753819 pyrosimple-2.9.0/src/pyrosimple/util/pymagic.py
--rwxr-xr-x   0        0        0     9602 2023-05-20 14:22:27.819352 pyrosimple-2.9.0/src/pyrosimple/util/rpc.py
--rw-r--r--   0        0        0     8584 2023-04-19 02:15:38.352321 pyrosimple-2.9.0/src/pyrosimple/util/traits.py
--rw-r--r--   0        0        0     2187 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/util/ui.py
--rw-r--r--   0        0        0     4287 1970-01-01 00:00:00.000000 pyrosimple-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2131 2023-04-13 23:28:24.964236 pyrosimple-2.9.1/README.md
+-rw-r--r--   0        0        0     3349 2023-07-09 22:05:24.653095 pyrosimple-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0      538 2023-04-13 23:28:24.974236 pyrosimple-2.9.1/src/pyrosimple/__init__.py
+-rw-r--r--   0        0        0     8778 2023-05-20 14:13:17.963479 pyrosimple-2.9.1/src/pyrosimple/config.py
+-rw-r--r--   0        0        0       67 2023-04-13 23:29:22.257480 pyrosimple-2.9.1/src/pyrosimple/data/__init__.py
+-rw-r--r--   0        0        0    10194 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/data/full-example.rc
+-rw-r--r--   0        0        0     1273 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/error.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/io/__init__.py
+-rw-r--r--   0        0        0     8666 2023-06-13 22:46:07.960229 pyrosimple-2.9.1/src/pyrosimple/io/scgi.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/job/__init__.py
+-rw-r--r--   0        0        0     2963 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/job/action.py
+-rw-r--r--   0        0        0     2977 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/job/base.py
+-rw-r--r--   0        0        0     9444 2023-04-13 23:29:22.257480 pyrosimple-2.9.1/src/pyrosimple/job/metrics.py
+-rw-r--r--   0        0        0     1691 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/job/move_path.py
+-rw-r--r--   0        0        0     1743 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/job/move_torrent.py
+-rw-r--r--   0        0        0     4192 2023-04-29 17:58:28.391573 pyrosimple-2.9.1/src/pyrosimple/job/queue.py
+-rw-r--r--   0        0        0     9954 2023-04-13 23:29:54.100762 pyrosimple-2.9.1/src/pyrosimple/job/watch.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/py.typed
+-rw-r--r--   0        0        0      112 2023-04-13 23:28:24.977569 pyrosimple-2.9.1/src/pyrosimple/scripts/__init__.py
+-rw-r--r--   0        0        0     8094 2023-04-29 17:15:41.825951 pyrosimple-2.9.1/src/pyrosimple/scripts/base.py
+-rw-r--r--   0        0        0    17593 2023-04-13 23:38:22.673176 pyrosimple-2.9.1/src/pyrosimple/scripts/chtor.py
+-rw-r--r--   0        0        0     6590 2023-04-13 23:29:22.260813 pyrosimple-2.9.1/src/pyrosimple/scripts/lstor.py
+-rw-r--r--   0        0        0     9779 2023-06-11 16:08:49.615631 pyrosimple-2.9.1/src/pyrosimple/scripts/mktor.py
+-rw-r--r--   0        0        0    13632 2023-04-29 15:30:45.910385 pyrosimple-2.9.1/src/pyrosimple/scripts/pyroadmin.py
+-rw-r--r--   0        0        0     9555 2023-04-13 23:29:22.260813 pyrosimple-2.9.1/src/pyrosimple/scripts/pyrotorque.py
+-rw-r--r--   0        0        0    36661 2023-07-09 22:01:36.930222 pyrosimple-2.9.1/src/pyrosimple/scripts/rtcontrol.py
+-rw-r--r--   0        0        0     8199 2023-05-30 20:05:50.210723 pyrosimple-2.9.1/src/pyrosimple/scripts/rtmv_legacy.py
+-rw-r--r--   0        0        0    10373 2023-05-20 14:17:01.248156 pyrosimple-2.9.1/src/pyrosimple/scripts/rtxmlrpc.py
+-rw-r--r--   0        0        0      117 2023-04-13 23:28:24.980902 pyrosimple-2.9.1/src/pyrosimple/torrent/__init__.py
+-rw-r--r--   0        0        0    30483 2023-06-08 19:31:12.538264 pyrosimple-2.9.1/src/pyrosimple/torrent/engine.py
+-rw-r--r--   0        0        0    37102 2023-07-04 13:42:16.215209 pyrosimple-2.9.1/src/pyrosimple/torrent/rtorrent.py
+-rw-r--r--   0        0        0      118 2023-04-13 23:28:24.984236 pyrosimple-2.9.1/src/pyrosimple/ui/__init__.py
+-rw-r--r--   0        0        0     2903 2023-04-13 23:28:24.984236 pyrosimple-2.9.1/src/pyrosimple/ui/categories.py
+-rw-r--r--   0        0        0      122 2023-04-13 23:28:24.984236 pyrosimple-2.9.1/src/pyrosimple/util/__init__.py
+-rw-r--r--   0        0        0     2164 2023-04-19 02:04:04.304690 pyrosimple-2.9.1/src/pyrosimple/util/cache.py
+-rw-r--r--   0        0        0     7891 2023-07-09 22:00:01.523745 pyrosimple-2.9.1/src/pyrosimple/util/fmt.py
+-rw-r--r--   0        0        0      459 2023-04-13 23:28:24.984236 pyrosimple-2.9.1/src/pyrosimple/util/logutil.py
+-rw-r--r--   0        0        0    32171 2023-06-24 12:58:29.919468 pyrosimple-2.9.1/src/pyrosimple/util/matching.py
+-rw-r--r--   0        0        0    26411 2023-04-13 23:29:22.267480 pyrosimple-2.9.1/src/pyrosimple/util/metafile.py
+-rw-r--r--   0        0        0     2124 2023-05-30 20:07:35.753819 pyrosimple-2.9.1/src/pyrosimple/util/pymagic.py
+-rwxr-xr-x   0        0        0     9602 2023-05-20 14:22:27.819352 pyrosimple-2.9.1/src/pyrosimple/util/rpc.py
+-rw-r--r--   0        0        0     8584 2023-04-19 02:15:38.352321 pyrosimple-2.9.1/src/pyrosimple/util/traits.py
+-rw-r--r--   0        0        0     2187 2023-04-13 23:28:24.984236 pyrosimple-2.9.1/src/pyrosimple/util/ui.py
+-rw-r--r--   0        0        0     4287 1970-01-01 00:00:00.000000 pyrosimple-2.9.1/PKG-INFO
```

### Comparing `pyrosimple-2.9.0/README.md` & `pyrosimple-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/pyproject.toml` & `pyrosimple-2.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrosimple"
-version = "2.9.0"
+version = "2.9.1"
 description = "A stripped-down version of the pyrocore tools for working with rTorrent"
 authors = ["kannibalox <kannibalox@gmail.com>"]
 repository = "https://github.com/kannibalox/pyrosimple"
 documentation = "https://kannibalox.github.io/pyrosimple/"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 classifiers = [
```

### Comparing `pyrosimple-2.9.0/src/pyrosimple/__init__.py` & `pyrosimple-2.9.1/src/pyrosimple/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/config.py` & `pyrosimple-2.9.1/src/pyrosimple/config.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/data/full-example.rc` & `pyrosimple-2.9.1/src/pyrosimple/data/full-example.rc`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/error.py` & `pyrosimple-2.9.1/src/pyrosimple/error.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/io/scgi.py` & `pyrosimple-2.9.1/src/pyrosimple/io/scgi.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/job/action.py` & `pyrosimple-2.9.1/src/pyrosimple/job/action.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/job/base.py` & `pyrosimple-2.9.1/src/pyrosimple/job/base.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/job/metrics.py` & `pyrosimple-2.9.1/src/pyrosimple/job/metrics.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/job/move_path.py` & `pyrosimple-2.9.1/src/pyrosimple/job/move_path.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/job/move_torrent.py` & `pyrosimple-2.9.1/src/pyrosimple/job/move_torrent.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/job/queue.py` & `pyrosimple-2.9.1/src/pyrosimple/job/queue.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/job/watch.py` & `pyrosimple-2.9.1/src/pyrosimple/job/watch.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/scripts/base.py` & `pyrosimple-2.9.1/src/pyrosimple/scripts/base.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/scripts/chtor.py` & `pyrosimple-2.9.1/src/pyrosimple/scripts/chtor.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/scripts/lstor.py` & `pyrosimple-2.9.1/src/pyrosimple/scripts/lstor.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/scripts/mktor.py` & `pyrosimple-2.9.1/src/pyrosimple/scripts/mktor.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/scripts/pyroadmin.py` & `pyrosimple-2.9.1/src/pyrosimple/scripts/pyroadmin.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/scripts/pyrotorque.py` & `pyrosimple-2.9.1/src/pyrosimple/scripts/pyrotorque.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/scripts/rtcontrol.py` & `pyrosimple-2.9.1/src/pyrosimple/scripts/rtcontrol.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,27 +33,27 @@
         return ("custom_KEY", custom_manifold)
 
     def kind_manifold():
         "file types that contribute at least N% to the item's total size, e.g. 'kind_50'"
         return ("kind_N", kind_manifold)
 
     def d_manifold():
-        "call an arbiratry item method, e.g. 'd_session_file'"
+        "call an arbitrary item method, e.g. 'd_session_file'"
         return ("d_METHOD", d_manifold)
 
     def p_manifold():
-        "call an arbiratry p.multicall method, e.g. 'p_is_incoming'"
+        "call an arbitrary p.multicall method, e.g. 'p_is_incoming'"
         return ("p_METHOD", p_manifold)
 
     def f_manifold():
-        "call an arbiratry f.multicall method, e.g. 'f_path'"
+        "call an arbitrary f.multicall method, e.g. 'f_path'"
         return ("f_METHOD", f_manifold)
 
     def t_manifold():
-        "call an arbiratry t.multicall method, e.g. 't_url'"
+        "call an arbitrary t.multicall method, e.g. 't_url'"
         return ("t_METHOD", t_manifold)
 
     print("")
     print("Fields are:")
     print(
         "\n".join(
             [
@@ -673,27 +673,28 @@
     def show_in_view(self, sourceview, matches, targetname=None):
         """Show search result in ncurses view."""
         append = self.options.alter_view == "append"
         remove = self.options.alter_view == "remove"
         action_name = (
             ", appending to" if append else ", removing from" if remove else " into"
         )
-        targetname = self.engine.show(
-            matches,
-            targetname or self.options.to_view or "rtcontrol",
-            append=append,
-            disjoin=remove,
-        )
-        msg = "Filtered %d out of %d torrents using [ %s ]" % (
-            len(matches),
-            sourceview.size(),
-            sourceview.matcher,
-        )
-        self.log.info("%s%s rTorrent view %r.", msg, action_name, targetname)
-        self.engine.log(msg)
+        for engine in self.engines.values():
+            targetname = engine.show(
+                matches,
+                targetname or self.options.to_view or "rtcontrol",
+                append=append,
+                disjoin=remove,
+            )
+            msg = "Filtered %d out of %d torrents using [ %s ]" % (
+                len(matches),
+                sourceview.size(),
+                sourceview.matcher,
+            )
+            self.log.info("%s%s rTorrent view %r.", msg, action_name, targetname)
+            engine.log(msg)
 
     def mainloop(self):
         """The main loop."""
         if self.options.help_fields:
             print_help_fields()
             print_help_filters()
             sys.exit(0)
```

### Comparing `pyrosimple-2.9.0/src/pyrosimple/scripts/rtmv_legacy.py` & `pyrosimple-2.9.1/src/pyrosimple/scripts/rtmv_legacy.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/scripts/rtxmlrpc.py` & `pyrosimple-2.9.1/src/pyrosimple/scripts/rtxmlrpc.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/torrent/engine.py` & `pyrosimple-2.9.1/src/pyrosimple/torrent/engine.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/torrent/rtorrent.py` & `pyrosimple-2.9.1/src/pyrosimple/torrent/rtorrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,14 +558,15 @@
             if fullpath.is_file() or fullpath.is_symlink():
                 self._engine.logger.debug("Deleting '%s'", fullpath)
                 dirs_to_clean_up.add(fullpath.parent)
                 if not dry_run:
                     fullpath.unlink()
         for directory in dirs_to_clean_up:
             try:
+                self._engine.logger.debug("Cleaning up directory '%s'", fullpath)
                 if not dry_run:
                     directory.rmdir()
             except OSError as e:
                 if e.errno != errno.ENOTEMPTY:
                     raise
 
         # Delete item from engine
```

### Comparing `pyrosimple-2.9.0/src/pyrosimple/ui/categories.py` & `pyrosimple-2.9.1/src/pyrosimple/ui/categories.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/util/cache.py` & `pyrosimple-2.9.1/src/pyrosimple/util/cache.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/util/fmt.py` & `pyrosimple-2.9.1/src/pyrosimple/util/fmt.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/util/matching.py` & `pyrosimple-2.9.1/src/pyrosimple/util/matching.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/util/metafile.py` & `pyrosimple-2.9.1/src/pyrosimple/util/metafile.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/util/pymagic.py` & `pyrosimple-2.9.1/src/pyrosimple/util/pymagic.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/util/rpc.py` & `pyrosimple-2.9.1/src/pyrosimple/util/rpc.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/util/traits.py` & `pyrosimple-2.9.1/src/pyrosimple/util/traits.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/src/pyrosimple/util/ui.py` & `pyrosimple-2.9.1/src/pyrosimple/util/ui.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.9.0/PKG-INFO` & `pyrosimple-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosimple
-Version: 2.9.0
+Version: 2.9.1
 Summary: A stripped-down version of the pyrocore tools for working with rTorrent
 Home-page: https://github.com/kannibalox/pyrosimple
 License: GPL-3.0-or-later
 Author: kannibalox
 Author-email: kannibalox@gmail.com
 Requires-Python: >=3.7.2,<4
 Classifier: Development Status :: 4 - Beta
```

