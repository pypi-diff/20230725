# Comparing `tmp/cubicweb-comment-2.0.0.tar.gz` & `tmp/cubicweb-comment-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-comment-2.0.0.tar", last modified: Fri Nov 25 13:48:10 2022, max compression
+gzip compressed data, was "cubicweb-comment-3.0.0.tar", last modified: Tue Jul 25 09:34:13 2023, max compression
```

## Comparing `cubicweb-comment-2.0.0.tar` & `cubicweb-comment-3.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 13:48:10.531032 cubicweb-comment-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      466 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2200 2022-11-25 13:48:10.531032 cubicweb-comment-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1758 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 13:48:10.527032 cubicweb-comment-2.0.0/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)       23 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 13:48:10.531032 cubicweb-comment-2.0.0/cubicweb_comment/data/
--rw-rw-rw-   0 root         (0) root         (0)      931 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/data/cubes.comment.css
--rw-rw-rw-   0 root         (0) root         (0)     3252 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/data/cubes.comment.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 13:48:10.531032 cubicweb-comment-2.0.0/cubicweb_comment/doc/
--rw-rw-rw-   0 root         (0) root         (0)     1781 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/doc/basic_usage.rst
--rw-rw-rw-   0 root         (0) root         (0)    47298 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/doc/screenshot_comment_section.png
--rw-rw-rw-   0 root         (0) root         (0)     4236 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 13:48:10.531032 cubicweb-comment-2.0.0/cubicweb_comment/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     2558 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)     3164 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 13:48:10.531032 cubicweb-comment-2.0.0/cubicweb_comment/migration/
--rw-rw-rw-   0 root         (0) root         (0)       36 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/migration/1.2.1_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    16527 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/cubicweb_comment/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 13:48:10.527032 cubicweb-comment-2.0.0/cubicweb_comment.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2200 2022-11-25 13:48:09.000000 cubicweb-comment-2.0.0/cubicweb_comment.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      901 2022-11-25 13:48:10.000000 cubicweb-comment-2.0.0/cubicweb_comment.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 13:48:09.000000 cubicweb-comment-2.0.0/cubicweb_comment.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-11-25 13:48:10.000000 cubicweb-comment-2.0.0/cubicweb_comment.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-25 13:48:09.000000 cubicweb-comment-2.0.0/cubicweb_comment.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2022-11-25 13:48:10.000000 cubicweb-comment-2.0.0/cubicweb_comment.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2022-11-25 13:48:10.000000 cubicweb-comment-2.0.0/cubicweb_comment.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-25 13:48:10.531032 cubicweb-comment-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2626 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 13:48:10.531032 cubicweb-comment-2.0.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-25 13:48:10.531032 cubicweb-comment-2.0.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       13 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)      192 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/test/test_comment.py
--rw-rw-rw-   0 root         (0) root         (0)     9521 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/test/unittest_comment.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2022-11-25 13:47:52.000000 cubicweb-comment-2.0.0/test/unittest_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:34:13.202438 cubicweb-comment-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-25 09:34:13.202438 cubicweb-comment-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1758 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:34:13.186438 cubicweb-comment-3.0.0/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:34:13.194438 cubicweb-comment-3.0.0/cubicweb_comment/data/
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/data/cubes.comment.css
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/data/cubes.comment.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:34:13.194438 cubicweb-comment-3.0.0/cubicweb_comment/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/doc/basic_usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)    47298 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/doc/screenshot_comment_section.png
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:34:13.194438 cubicweb-comment-3.0.0/cubicweb_comment/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:34:13.198439 cubicweb-comment-3.0.0/cubicweb_comment/migration/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/migration/1.2.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    16565 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/cubicweb_comment/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:34:13.190438 cubicweb-comment-3.0.0/cubicweb_comment.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-25 09:34:13.000000 cubicweb-comment-3.0.0/cubicweb_comment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      901 2023-07-25 09:34:13.000000 cubicweb-comment-3.0.0/cubicweb_comment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:34:13.000000 cubicweb-comment-3.0.0/cubicweb_comment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-25 09:34:13.000000 cubicweb-comment-3.0.0/cubicweb_comment.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:34:13.000000 cubicweb-comment-3.0.0/cubicweb_comment.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-25 09:34:13.000000 cubicweb-comment-3.0.0/cubicweb_comment.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-25 09:34:13.000000 cubicweb-comment-3.0.0/cubicweb_comment.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:34:13.202438 cubicweb-comment-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:34:13.202438 cubicweb-comment-3.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:34:13.202438 cubicweb-comment-3.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      193 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/test/test_comment.py
+-rw-rw-rw-   0 root         (0) root         (0)    10070 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/test/unittest_comment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-25 09:33:45.000000 cubicweb-comment-3.0.0/test/unittest_hooks.py
```

### Comparing `cubicweb-comment-2.0.0/PKG-INFO` & `cubicweb-comment-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-comment
-Version: 2.0.0
+Version: 3.0.0
 Summary: commenting system for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-comment
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -69,9 +68,7 @@
 comments automatically on blog entry's primary view.
 
 Documentation
 -------------
 
 Look in the ``doc/`` subdirectory or read
 http://www.cubicweb.org/doc/en/
-
-
```

### Comparing `cubicweb-comment-2.0.0/README.rst` & `cubicweb-comment-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment/data/cubes.comment.css` & `cubicweb-comment-3.0.0/cubicweb_comment/data/cubes.comment.css`

 * *Files identical despite different names*

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment/data/cubes.comment.js` & `cubicweb-comment-3.0.0/cubicweb_comment/data/cubes.comment.js`

 * *Files identical despite different names*

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment/doc/basic_usage.rst` & `cubicweb-comment-3.0.0/cubicweb_comment/doc/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment/doc/screenshot_comment_section.png` & `cubicweb-comment-3.0.0/cubicweb_comment/doc/screenshot_comment_section.png`

 * *Files identical despite different names*

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment/hooks.py` & `cubicweb-comment-3.0.0/cubicweb_comment/hooks.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 from cubicweb import RegistryException
 from cubicweb.predicates import is_instance
 from cubicweb.sobjects import notification
 
 
 class CommentAddedView(notification.NotificationView):
     """get notified from new comments"""
-    __regid__ = 'notif_after_add_relation_comments'
-    __select__ = is_instance('Comment',)
+
+    __regid__ = "notif_after_add_relation_comments"
+    __select__ = is_instance(
+        "Comment",
+    )
     msgid_timestamp = False
 
     def subject(self):
-        root = self.cw_rset.get_entity(self.cw_row, self.cw_col).cw_adapt_to('ITree').root()
-        return '%s %s %s' % (self._cw._('new comment for'),
-                             root.dc_type(),
-                             root.dc_title())
+        root = (
+            self.cw_rset.get_entity(self.cw_row, self.cw_col)
+            .cw_adapt_to("ITree")
+            .root()
+        )
+        return f"{self._cw._('new comment for')} {root.dc_type()} {root.dc_title()}"
 
     def render(self, **kwargs):
         try:
-            view = self._cw.vreg['views'].select('fullthreadtext', self._cw,
-                                                 rset=self.cw_rset)
+            view = self._cw.vreg["views"].select(
+                "fullthreadtext", self._cw, rset=self.cw_rset
+            )
         except RegistryException:
             return
         return view.render()
```

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment/i18n/en.po` & `cubicweb-comment-3.0.0/cubicweb_comment/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment/i18n/fr.po` & `cubicweb-comment-3.0.0/cubicweb_comment/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment/views.py` & `cubicweb-comment-3.0.0/cubicweb_comment/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,400 +1,475 @@
 """Specific views and actions for application using the Comment entity type
 
 :organization: Logilab
 :copyright: 2003-2011 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
-from __future__ import with_statement
 
 __docformat__ = "restructuredtext en"
 
 
 from cubicweb import _
 
 from logilab.mtconverter import xml_escape
 
-from cubicweb.predicates import (is_instance, has_permission, authenticated_user,
-                                 score_entity, relation_possible, one_line_rset,
-                                 match_kwargs, match_form_params,
-                                 partial_relation_possible)
+from cubicweb.predicates import (
+    is_instance,
+    has_permission,
+    authenticated_user,
+    score_entity,
+    relation_possible,
+    one_line_rset,
+    match_kwargs,
+    match_form_params,
+    partial_relation_possible,
+)
 from cubicweb_web.view import EntityView
 from cubicweb.uilib import cut, js
 from cubicweb_web import component, form, formwidgets as fw
 from cubicweb_web.action import LinkToEntityAction, Action
 from cubicweb_web.views import primary, baseviews, xmlrss, treeview, ajaxedit, uicfg
 
 _afs = uicfg.autoform_section
-_afs.tag_object_of(('*', 'comments', '*'), formtype='main', section='hidden')
+_afs.tag_object_of(("*", "comments", "*"), formtype="main", section="hidden")
 
 _affk = uicfg.autoform_field_kwargs
-_affk.tag_subject_of(('*', 'comments', '*'), {'widget': fw.HiddenInput})
+_affk.tag_subject_of(("*", "comments", "*"), {"widget": fw.HiddenInput})
 
 _abaa = uicfg.actionbox_appearsin_addmenu
-_abaa.tag_subject_of(('*', 'comments', '*'),  False)
-_abaa.tag_object_of(('*', 'comments', '*'), False)
+_abaa.tag_subject_of(("*", "comments", "*"), False)
+_abaa.tag_object_of(("*", "comments", "*"), False)
 
 _pvs = uicfg.primaryview_section
-_pvs.tag_subject_of(('*', 'comments', '*'),  'hidden')
-_pvs.tag_object_of(('*', 'comments', '*'), 'hidden')
+_pvs.tag_subject_of(("*", "comments", "*"), "hidden")
+_pvs.tag_object_of(("*", "comments", "*"), "hidden")
 
 
 # comment views ###############################################################
 
+
 class CommentPrimaryView(primary.PrimaryView):
-    __select__ = is_instance('Comment')
+    __select__ = is_instance("Comment")
 
     def cell_call(self, row, col):
-        self._cw.add_css('cubes.comment.css')
+        self._cw.add_css("cubes.comment.css")
         entity = self.cw_rset.complete_entity(row, col)
         # display text, author and creation date
-        self.w(u'<div class="comment">')
-        self.w(u'<div class="commentInfo">')
+        self.w('<div class="comment">')
+        self.w('<div class="commentInfo">')
         # do not try to display creator when you're not allowed to see CWUsers
         if entity.creator:
-            authorlink = entity.creator.view('oneline')
-            self.w(u'%s %s\n' % (self._cw._('written by'), authorlink))
+            authorlink = entity.creator.view("oneline")
+            self.w(f"{self._cw._('written by')} {authorlink}\n")
         self.w(self._cw.format_date(entity.creation_date))
         # commented object
         if entity.comments:
-            self.w(u",  %s " % self._cw._('comments'))
-            entity.comments[0].view('oneline', w=self.w)
-            self.w(u"\n")
+            self.w(f",  {self._cw._('comments')} ")
+            entity.comments[0].view("oneline", w=self.w)
+            self.w("\n")
         # don't include responses in this view, since the comment section
         # component will display them
-        self.w(u'</div>\n')
-        self.w(u'<div class="commentBody">%s</div>\n'
-               % entity.printable_value('content'))
+        self.w("</div>\n")
+        self.w(
+            f"<div class=\"commentBody\">{entity.printable_value('content')}</div>\n"
+        )
         # XXX attribute generated_by added by email component
-        if hasattr(entity, 'generated_by') and entity.generated_by:
+        if hasattr(entity, "generated_by") and entity.generated_by:
             gen = entity.generated_by[0]
-            link = '<a href="%s">%s</a>' % (gen.absolute_url(),
-                                            gen.dc_type().lower())
-            txt = self._cw._('this comment has been generated from this %s') % link
-            self.w(u'<div class="commentBottom">%s</div>\n' % txt)
-        self.w(u'</div>\n')
+            link = f'<a href="{gen.absolute_url()}">{gen.dc_type().lower()}</a>'
+            txt = self._cw._("this comment has been generated from this %s") % link
+            self.w(f'<div class="commentBottom">{txt}</div>\n')
+        self.w("</div>\n")
 
 
 class CommentRootView(EntityView):
-    __regid__ = 'commentroot'
-    __select__ = is_instance('Comment')
+    __regid__ = "commentroot"
+    __select__ = is_instance("Comment")
 
     def cell_call(self, row, col, **kwargs):
         entity = self.cw_rset.get_entity(row, col)
-        root = entity.cw_adapt_to('ITree').root()
-        self.w(u'<a href="%s">%s %s</a> ' % (
-            xml_escape(root.absolute_url()),
-            xml_escape(root.dc_type()),
-            xml_escape(cut(root.dc_title(), 40))))
+        root = entity.cw_adapt_to("ITree").root()
+        self.w(
+            '<a href="%s">%s %s</a> '
+            % (
+                xml_escape(root.absolute_url()),
+                xml_escape(root.dc_type()),
+                xml_escape(cut(root.dc_title(), 40)),
+            )
+        )
 
 
 class CommentSummary(EntityView):
-    __regid__ = 'commentsummary'
-    __select__ = is_instance('Comment')
+    __regid__ = "commentsummary"
+    __select__ = is_instance("Comment")
 
     def cell_call(self, row, col, **kwargs):
         entity = self.cw_rset.get_entity(row, col)
-        maxsize = self._cw.property_value('navigation.short-line-size')
-        content = entity.printable_value('content', format='text/plain')
+        maxsize = self._cw.property_value("navigation.short-line-size")
+        content = entity.printable_value("content", format="text/plain")
         self.w(xml_escape(cut(content, maxsize)))
 
 
 class CommentOneLineView(baseviews.OneLineView):
-    __select__ = is_instance('Comment')
+    __select__ = is_instance("Comment")
 
     def cell_call(self, row, col, **kwargs):
         entity = self.cw_rset.get_entity(row, col)
-        self.w(u'[%s] ' % entity.view('commentroot'))
-        self.w(u'<a href="%s"><i>%s</i></a>\n' % (
-            xml_escape(entity.absolute_url()),
-            entity.view('commentsummary')))
+        self.w(f"[{entity.view('commentroot')}] ")
+        self.w(
+            '<a href="%s"><i>%s</i></a>\n'
+            % (xml_escape(entity.absolute_url()), entity.view("commentsummary"))
+        )
 
 
 class CommentTreeItemView(baseviews.ListItemView):
-    __regid__ = 'treeitem'
-    __select__ = is_instance('Comment')
+    __regid__ = "treeitem"
+    __select__ = is_instance("Comment")
 
     def cell_call(self, row, col, **kwargs):
-        self._cw.add_js('cubicweb.ajax.js')
-        self._cw.add_css('cubes.comment.css')
-        self._cw.add_css('cubicweb.pictograms.css')
+        self._cw.add_js("cubicweb.ajax.js")
+        self._cw.add_css("cubes.comment.css")
+        self._cw.add_css("cubicweb.pictograms.css")
         entity = self.cw_rset.get_entity(row, col)
-        actions = self._cw.vreg['actions']
+        actions = self._cw.vreg["actions"]
         # DOM id of the whole comment's content
-        cdivid = 'comment%sDiv' % entity.eid
-        self.w(u'<div class="cwjs-comment" data-eid="%i" id="%s">' % (entity.eid, cdivid))
-        self.w(u'<div class="commentInfo">')
-        self.w(u'<span class="commentDate">')
+        cdivid = f"comment{entity.eid}Div"
+        self.w(
+            '<div class="cwjs-comment" data-eid="%i" id="%s">' % (entity.eid, cdivid)
+        )
+        self.w('<div class="commentInfo">')
+        self.w('<span class="commentDate">')
         self.w(self._cw.format_date(entity.creation_date))
-        self.w(u' %s' % self._cw.format_time(entity.creation_date))
-        self.w(u'</span>')
+        self.w(f" {self._cw.format_time(entity.creation_date)}")
+        self.w("</span>")
         if entity.creator:
-            authorlink = entity.creator.view('oneline')
-            self.w(u', %s <span class="author">%s</span> \n'
-                   % (self._cw._('written by'), authorlink,))
-        replyaction = actions.select_or_none('reply_comment', self._cw,
-                                             rset=self.cw_rset, row=row)
+            authorlink = entity.creator.view("oneline")
+            self.w(
+                ', %s <span class="author">%s</span> \n'
+                % (
+                    self._cw._("written by"),
+                    authorlink,
+                )
+            )
+        replyaction = actions.select_or_none(
+            "reply_comment", self._cw, rset=self.cw_rset, row=row
+        )
         if replyaction is not None:
-            self.w(u' <span class="replyto">'
-                   u'<a class="cwjs-comment-reply icon-reply" href="#">%s</a></span>'
-                   % self._cw._(replyaction.title))
-        editaction = actions.select_or_none('edit_comment', self._cw,
-                                            rset=self.cw_rset, row=row)
-        self.w(u'<span class="commentaction">')
+            self.w(
+                ' <span class="replyto">'
+                '<a class="cwjs-comment-reply icon-reply" href="#">%s</a></span>'
+                % self._cw._(replyaction.title)
+            )
+        editaction = actions.select_or_none(
+            "edit_comment", self._cw, rset=self.cw_rset, row=row
+        )
+        self.w('<span class="commentaction">')
         if editaction is not None:
-            self.w(u'<span class="replyto">'
-                   u'<a class="cwjs-comment-edit icon-pencil" href="#">%s</a></span>'
-                   % self._cw._(editaction.title))
-
-        deleteaction = actions.select_or_none('delete_comment', self._cw,
-                                              rset=self.cw_rset, row=row)
+            self.w(
+                '<span class="replyto">'
+                '<a class="cwjs-comment-edit icon-pencil" href="#">%s</a></span>'
+                % self._cw._(editaction.title)
+            )
+
+        deleteaction = actions.select_or_none(
+            "delete_comment", self._cw, rset=self.cw_rset, row=row
+        )
         if deleteaction is not None:
-            root = entity.cw_adapt_to('ITree').root()
-            self.w(u'<span class="replyto">'
-                   u'<a class="cwjs-comment-delete icon-trash" '
-                   u'   data-redirect="%s" href="#">%s</a></span>'
-                   % (xml_escape(root.rest_path()), self._cw._(deleteaction.title)))
-        self.w(u'</span>')
-        self.w(u'</div>\n')  # close comment's info div
-        self.w(u'<div class="commentBody">%s</div>\n'
-               % entity.printable_value('content'))
+            root = entity.cw_adapt_to("ITree").root()
+            self.w(
+                '<span class="replyto">'
+                '<a class="cwjs-comment-delete icon-trash" '
+                '   data-redirect="%s" href="#">%s</a></span>'
+                % (xml_escape(root.rest_path()), self._cw._(deleteaction.title))
+            )
+        self.w("</span>")
+        self.w("</div>\n")  # close comment's info div
+        self.w(
+            f"<div class=\"commentBody\">{entity.printable_value('content')}</div>\n"
+        )
         # holder for reply form
-        self.w(u'<div id="comment%sHolder" class="cwjs-comment-holder replyComment"></div>'
-               % entity.eid)
-        self.w(u'</div>\n')  # close comment's content div
+        self.w(
+            '<div id="comment%sHolder" class="cwjs-comment-holder replyComment"></div>'
+            % entity.eid
+        )
+        self.w("</div>\n")  # close comment's content div
 
 
 class CommentThreadView(treeview.BaseTreeView):
     """a recursive tree view"""
-    __select__ = is_instance('Comment')
-    title = _('thread view')
+
+    __select__ = is_instance("Comment")
+    title = _("thread view")
 
     def open_item(self, entity):
-        self.w(u'<li id="comment%s" class="comment">\n' % entity.eid)
+        self.w(f'<li id="comment{entity.eid}" class="comment">\n')
 
 
 class RssItemCommentView(xmlrss.RSSItemView):
-    __select__ = is_instance('Comment')
+    __select__ = is_instance("Comment")
 
     def cell_call(self, row, col, seen=None):
         entity = self.cw_rset.complete_entity(row, col)
         seen = seen or set()
         if entity.eid in seen:
             # avoid infinite recursion in case of loop on "comments" relation
             # since we're calling 'rssitem' view recursively.
             return
         seen.add(entity.eid)
-        self.w(u'<item>\n')
-        self.w(u'<guid isPermaLink="true">%s</guid>\n'
-               % xml_escape(entity.absolute_url()))
+        self.w("<item>\n")
+        self.w(f'<guid isPermaLink="true">{xml_escape(entity.absolute_url())}</guid>\n')
         self.render_title_link(entity)
-        root = entity.cw_adapt_to('ITree').root()
-        description = (entity.dc_description(format='text/html') +
-                       self._cw._(u'about') +
-                       u' <a href=%s>%s</a>' % (root.absolute_url(),
-                                                root.dc_title()))
-        self._marker('description', description)
-        self._marker('dc:date', entity.dc_date(self.date_format))
+        root = entity.cw_adapt_to("ITree").root()
+        description = (
+            entity.dc_description(format="text/html")
+            + self._cw._("about")
+            + f" <a href={root.absolute_url()}>{root.dc_title()}</a>"
+        )
+        self._marker("description", description)
+        self._marker("dc:date", entity.dc_date(self.date_format))
         self.render_entity_creator(entity)
-        self.w(u'</item>\n')
-        self.wview('rssitem', entity.related('comments', 'object'), 'null', seen=seen)
+        self.w("</item>\n")
+        self.wview("rssitem", entity.related("comments", "object"), "null", seen=seen)
 
 
 # comment forms ################################################################
 
+
 class InlineEditCommentFormView(form.FormViewMixIn, EntityView):
-    __regid__ = 'editcommentform'
-    __select__ = is_instance('Comment')
+    __regid__ = "editcommentform"
+    __select__ = is_instance("Comment")
 
     def entity_call(self, entity):
         self.comment_form(entity)
 
     def propose_to_login(self):
-        self.w(u'<div class="warning">%s ' % self._cw._(
-            'You are not authenticated. Your comment will be anonymous if you '
-            'do not <a onclick="showLoginBox()">login</a>.'))
-        if 'registration' in self._cw.vreg.config.cubes():
-            self.w(self._cw._(' If you have no account, you may want to '
-                              '<a href="%s">create one</a>.')
-                   % self._cw.build_url('register'))
-        self.w(u'</div>')
+        self.w(
+            '<div class="warning">%s '
+            % self._cw._(
+                "You are not authenticated. Your comment will be anonymous if you "
+                'do not <a onclick="showLoginBox()">login</a>.'
+            )
+        )
+        if "registration" in self._cw.vreg.config.cubes():
+            self.w(
+                self._cw._(
+                    " If you have no account, you may want to "
+                    '<a href="%s">create one</a>.'
+                )
+                % self._cw.build_url("register")
+            )
+        self.w("</div>")
 
     def comment_form(self, commented, newcomment=None):
-        self._cw.add_js(('cubicweb.edition.js', 'cubes.comment.js'))
+        self._cw.add_js(("cubicweb.edition.js", "cubes.comment.js"))
         if self._cw.cnx.session.anonymous_session:
             self.propose_to_login()
         entity = newcomment or commented
-        okjs = js.processComment(commented.eid, not entity.has_eid(),
-                                 not (newcomment is None or commented.has_eid()),
-                                 self.cw_extra_kwargs.get('context'))
+        okjs = js.processComment(
+            commented.eid,
+            not entity.has_eid(),
+            not (newcomment is None or commented.has_eid()),
+            self.cw_extra_kwargs.get("context"),
+        )
         canceljs = js.cancelCommentEdition(commented.eid, not entity.has_eid())
         form, formvalues = ajaxedit.ajax_composite_form(
-            commented, newcomment, 'comments', okjs, canceljs)
-        self.w(u'<div id="comment%sSlot">' % commented.eid)
-        form.render(w=self.w, formvalues=formvalues,
-                    main_form_title=u'', display_label=False)
-        self.w(u'</div>')
+            commented, newcomment, "comments", okjs, canceljs
+        )
+        self.w(f'<div id="comment{commented.eid}Slot">')
+        form.render(
+            w=self.w, formvalues=formvalues, main_form_title="", display_label=False
+        )
+        self.w("</div>")
 
 
 class InlineAddCommentFormView(InlineEditCommentFormView):
-    __regid__ = 'addcommentform'
-    __select__ = (relation_possible('comments', 'object', 'Comment', 'add')
-                  | match_form_params('etype'))
+    __regid__ = "addcommentform"
+    __select__ = relation_possible(
+        "comments", "object", "Comment", "add"
+    ) | match_form_params("etype")
 
     def call(self, **kwargs):
         if self.cw_rset is None:
-            entity = self._cw.vreg['etypes'].etype_class(self._cw.form['etype'])(self._cw)
-            entity.eid = self._cw.form['tempEid']
+            entity = self._cw.vreg["etypes"].etype_class(self._cw.form["etype"])(
+                self._cw
+            )
+            entity.eid = self._cw.form["tempEid"]
             self.entity_call(entity)
         else:
-            super(InlineAddCommentFormView, self).call(**kwargs)
+            super().call(**kwargs)
 
     def entity_call(self, commented):
-        newcomment = self._cw.vreg['etypes'].etype_class('Comment')(self._cw)
+        newcomment = self._cw.vreg["etypes"].etype_class("Comment")(self._cw)
         newcomment.eid = self._cw.varmaker.next()
         self.comment_form(commented, newcomment)
 
 
 # contextual components ########################################################
 
+
 class CommentSectionVComponent(component.EntityCtxComponent):
     """a component to display a <div> html section including comments
     related to an object
     """
-    __regid__ = 'commentsection'
-    __select__ = (component.EntityCtxComponent.__select__
-                  & relation_possible('comments', 'object', 'Comment'))
 
-    context = 'navcontentbottom'
+    __regid__ = "commentsection"
+    __select__ = component.EntityCtxComponent.__select__ & relation_possible(
+        "comments", "object", "Comment"
+    )
+
+    context = "navcontentbottom"
 
     def render_body(self, w):
         req = self._cw
-        req.add_js(('cubicweb.ajax.js', 'cubes.comment.js'))
-        req.add_css('cubicweb.pictograms.css')
+        req.add_js(("cubicweb.ajax.js", "cubes.comment.js"))
+        req.add_css("cubicweb.pictograms.css")
         entity = self.entity
-        addcomment = self._cw.vreg['actions'].select_or_none(
-            'reply_comment', req, entity=entity,
-            rset=entity.cw_rset, row=entity.cw_row, col=entity.cw_col)
+        addcomment = self._cw.vreg["actions"].select_or_none(
+            "reply_comment",
+            req,
+            entity=entity,
+            rset=entity.cw_rset,
+            row=entity.cw_row,
+            col=entity.cw_col,
+        )
         if entity.has_eid():
-            rql = u'Any C,CD,CC,CCF,U,UL,US,UF ORDERBY CD WHERE C is Comment, '\
-                  'C comments X, C creation_date CD, C content CC, C content_format CCF, ' \
-                  'C created_by U?, U login UL, U firstname UF, U surname US, X eid %(x)s'
-            rset = req.execute(rql, {'x': entity.eid})
+            rql = (
+                "Any C,CD,CC,CCF,U,UL,US,UF ORDERBY CD WHERE C is Comment, "
+                "C comments X, C creation_date CD, C content CC, C content_format CCF, "
+                "C created_by U?, U login UL, U firstname UF, U surname US, X eid %(x)s"
+            )
+            rset = req.execute(rql, {"x": entity.eid})
             if rset.rowcount:
-                w(u'<h4>%s</h4>' % (req._('Comment_plural')))
-                w(u'<ul class="comment list-unstyled">')
+                w(f"<h4>{req._('Comment_plural')}</h4>")
+                w('<ul class="comment list-unstyled">')
                 for i in range(rset.rowcount):
-                    self._cw.view('tree', rset, row=i, w=w,
-                                  klass='list-unstyled')
-                w(u'</ul>')
+                    self._cw.view("tree", rset, row=i, w=w, klass="list-unstyled")
+                w("</ul>")
         if addcomment is not None:
-            url = self.lazy_view_holder(w, entity, 'addcommentform')
-            w(u' <span class="addcomment"><a class="icon-comment" href="%s">%s</a></span>'
-              % (xml_escape(url), req._(addcomment.title)))
+            url = self.lazy_view_holder(w, entity, "addcommentform")
+            w(
+                ' <span class="addcomment"><a class="icon-comment" href="%s">%s</a></span>'
+                % (xml_escape(url), req._(addcomment.title))
+            )
 
 
 class UserLatestCommentsSection(component.EntityCtxComponent):
     """a section to display latest comments by a user"""
-    __select__ = component.EntityCtxComponent.__select__ & is_instance('CWUser')
-    __regid__ = 'latestcomments'
-    context = 'navcontentbottom'
+
+    __select__ = component.EntityCtxComponent.__select__ & is_instance("CWUser")
+    __regid__ = "latestcomments"
+    context = "navcontentbottom"
 
     def render_body(self, w):
-        maxrelated = self._cw.property_value('navigation.related-limit') + 1
+        maxrelated = self._cw.property_value("navigation.related-limit") + 1
         rset = self._cw.execute(
-            'Any C,CD,C,CCF ORDERBY CD DESC LIMIT %s WHERE C is Comment, '
-            'C creation_date CD, C content CC, C content_format CCF, '
-            'C created_by U, U eid %%(u)s' % maxrelated,
-            {'u': self.entity.eid})
+            "Any C,CD,C,CCF ORDERBY CD DESC LIMIT %s WHERE C is Comment, "
+            "C creation_date CD, C content CC, C content_format CCF, "
+            "C created_by U, U eid %%(u)s" % maxrelated,
+            {"u": self.entity.eid},
+        )
         if rset:
-            w(u'<div class="section">')
-            w(u'<h4>%s</h4>\n' % self._cw._('Latest comments').capitalize())
-            self._cw.view('table', rset, w=w,
-                          headers=[_('about'), _('on date'),
-                                   _('comment content')],
-                          cellvids={0: 'commentroot',
-                                    2: 'commentsummary'})
-            w(u'</div>')
+            w('<div class="section">')
+            w(f"<h4>{self._cw._('Latest comments').capitalize()}</h4>\n")
+            self._cw.view(
+                "table",
+                rset,
+                w=w,
+                headers=[_("about"), _("on date"), _("comment content")],
+                cellvids={0: "commentroot", 2: "commentsummary"},
+            )
+            w("</div>")
+
 
 # adapters #####################################################################
 
 # XXX implements ibreadcrumbs instead
 
 
 from cubicweb_web.views.editcontroller import IEditControlAdapter  # noqa: E402
 
 
 class CommentIEditControlAdapter(IEditControlAdapter):
-    __select__ = is_instance('Comment')
+    __select__ = is_instance("Comment")
 
     def after_deletion_path(self):
         """return (path, parameters) which should be used as redirect
         information when this entity is being deleted
         """
-        return self.entity.cw_adapt_to('ITree').root().rest_path(), {}
+        return self.entity.cw_adapt_to("ITree").root().rest_path(), {}
+
 
 # actions ######################################################################
 
 
 class ReplyCommentAction(LinkToEntityAction):
-    __regid__ = 'reply_comment'
-    __select__ = LinkToEntityAction.__select__ & is_instance('Comment')
+    __regid__ = "reply_comment"
+    __select__ = LinkToEntityAction.__select__ & is_instance("Comment")
 
-    rtype = 'comments'
-    role = 'object'
-    target_etype = 'Comment'
+    rtype = "comments"
+    role = "object"
+    target_etype = "Comment"
 
-    title = _('reply')
-    category = 'hidden'
+    title = _("reply")
+    category = "hidden"
     order = 111
 
     def url(self):
         comment = self.cw_rset.get_entity(self.cw_row or 0, self.cw_col or 0)
-        linkto = '%s:%s:subject' % (self.rtype, comment.eid)
-        root = comment.cw_adapt_to('ITree').root()
-        return self._cw.build_url(vid='creation', etype=self.target_etype,
-                                  __linkto=linkto,
-                                  __redirectpath=root.rest_path(),
-                                  __redirectvid=self._cw.form.get('vid', ''))
+        linkto = f"{self.rtype}:{comment.eid}:subject"
+        root = comment.cw_adapt_to("ITree").root()
+        return self._cw.build_url(
+            vid="creation",
+            etype=self.target_etype,
+            __linkto=linkto,
+            __redirectpath=root.rest_path(),
+            __redirectvid=self._cw.form.get("vid", ""),
+        )
 
 
 class AddCommentAction(LinkToEntityAction):
     """add comment is like reply for everything but Comment"""
-    __regid__ = 'reply_comment'
-    __select__ = ((LinkToEntityAction.__select__
-                   | (match_kwargs('entity') &
-                      partial_relation_possible(action='add', strict=True)))
-                  & ~is_instance('Comment'))
-
-    rtype = 'comments'
-    role = 'object'
-    target_etype = 'Comment'
 
-    title = _('add comment')
-    category = 'hidden'
+    __regid__ = "reply_comment"
+    __select__ = (
+        LinkToEntityAction.__select__
+        | (
+            match_kwargs("entity")
+            & partial_relation_possible(action="add", strict=True)
+        )
+    ) & ~is_instance("Comment")
+
+    rtype = "comments"
+    role = "object"
+    target_etype = "Comment"
+
+    title = _("add comment")
+    category = "hidden"
     order = 111
 
 
 class EditCommentAction(Action):
-    __regid__ = 'edit_comment'
-    __select__ = one_line_rset() & is_instance('Comment') & has_permission('update')
+    __regid__ = "edit_comment"
+    __select__ = one_line_rset() & is_instance("Comment") & has_permission("update")
 
-    title = 'modify'  # not internationalized on purpose (wanna use cw translation)
-    category = 'hidden'
+    title = "modify"  # not internationalized on purpose (wanna use cw translation)
+    category = "hidden"
     order = 110
 
     def url(self):
-        return self._cw.build_url(rql=self.cw_rset.printable_rql(), vid='edition')
+        return self._cw.build_url(rql=self.cw_rset.printable_rql(), vid="edition")
 
 
 class DeleteCommentAction(Action):
-    __regid__ = 'delete_comment'
-    __select__ = (is_instance('Comment')
-                  & authenticated_user()
-                  & score_entity(lambda x: not x.reverse_comments and x.cw_has_perm('delete')))
+    __regid__ = "delete_comment"
+    __select__ = (
+        is_instance("Comment")
+        & authenticated_user()
+        & score_entity(lambda x: not x.reverse_comments and x.cw_has_perm("delete"))
+    )
 
-    title = 'delete'  # not internationalized on purpose (wanna use cw translation)
-    category = 'hidden'
+    title = "delete"  # not internationalized on purpose (wanna use cw translation)
+    category = "hidden"
     order = 110
 
     def url(self):
-        return self._cw.build_url(rql=self.cw_rset.printable_rql(), vid='deleteconf')
+        return self._cw.build_url(rql=self.cw_rset.printable_rql(), vid="deleteconf")
```

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment.egg-info/PKG-INFO` & `cubicweb-comment-3.0.0/cubicweb_comment.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-comment
-Version: 2.0.0
+Version: 3.0.0
 Summary: commenting system for the CubicWeb framework
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-comment
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -69,9 +68,7 @@
 comments automatically on blog entry's primary view.
 
 Documentation
 -------------
 
 Look in the ``doc/`` subdirectory or read
 http://www.cubicweb.org/doc/en/
-
-
```

### Comparing `cubicweb-comment-2.0.0/cubicweb_comment.egg-info/SOURCES.txt` & `cubicweb-comment-3.0.0/cubicweb_comment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-comment-2.0.0/setup.py` & `cubicweb-comment-3.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of a CubicWeb cube.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -26,58 +26,56 @@
 from setuptools import find_packages, setup
 
 
 here = dirname(__file__)
 
 # load metadata from the __pkginfo__.py file so there is no risk of conflict
 # see https://packaging.python.org/en/latest/single_source_version.html
-pkginfo = join(here, 'cubicweb_comment', '__pkginfo__.py')
+pkginfo = join(here, "cubicweb_comment", "__pkginfo__.py")
 __pkginfo__ = {}
 with open(pkginfo) as f:
     exec(f.read(), __pkginfo__)
 
 # get required metadatas
-distname = __pkginfo__['distname']
-version = __pkginfo__['version']
-license = __pkginfo__['license']
-description = __pkginfo__['description']
-web = __pkginfo__['web']
-author = __pkginfo__['author']
-author_email = __pkginfo__['author_email']
-classifiers = __pkginfo__['classifiers']
+distname = __pkginfo__["distname"]
+version = __pkginfo__["version"]
+license = __pkginfo__["license"]
+description = __pkginfo__["description"]
+web = __pkginfo__["web"]
+author = __pkginfo__["author"]
+author_email = __pkginfo__["author_email"]
+classifiers = __pkginfo__["classifiers"]
 
-with open(join(here, 'README.rst')) as f:
+with open(join(here, "README.rst")) as f:
     long_description = f.read()
 
 # get optional metadatas
-data_files = __pkginfo__.get('data_files', None)
-dependency_links = __pkginfo__.get('dependency_links', ())
+data_files = __pkginfo__.get("data_files", None)
+dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
 
-install_requires = ["{0} {1}".format(d, v and v or "").strip()
-                    for d, v in requires.items()]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
     long_description=long_description,
     author=author,
     author_email=author_email,
     url=web,
     classifiers=classifiers,
-    packages=find_packages(exclude=['test']),
+    packages=find_packages(exclude=["test"]),
     install_requires=install_requires,
     include_package_data=True,
     entry_points={
-        'cubicweb.cubes': [
-            'comment=cubicweb_comment',
+        "cubicweb.cubes": [
+            "comment=cubicweb_comment",
         ],
     },
-
     zip_safe=False,
 )
```

### Comparing `cubicweb-comment-2.0.0/test/unittest_comment.py` & `cubicweb-comment-3.0.0/test/unittest_comment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,206 +1,250 @@
 import re
 from lxml import etree
 
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC
+from cubicweb_web.devtools.testlib import WebCWTC
 
 from cubicweb_comment import views
 
 
-class CommentTC(CubicWebTC):
+class CommentTC(WebCWTC):
     """Comment"""
 
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
-            self.b = cnx.create_entity('BlogEntry', title=u"yo", content=u"qu\'il est beau").eid
+            self.b = cnx.create_entity(
+                "BlogEntry", title="yo", content="qu'il est beau"
+            ).eid
             cnx.commit()
 
     def test_schema(self):
-        self.assertEqual(self.schema['comments'].rdef('Comment', 'BlogEntry').composite,
-                         'object')
+        self.assertEqual(
+            self.schema["comments"]
+            .relation_definition("Comment", "BlogEntry")
+            .composite,
+            "object",
+        )
 
     def test_possible_views(self):
         # comment primary view priority
         with self.admin_access.web_request() as req:
-            rset = req.create_entity('Comment', content=u"bouh!", comments=self.b).as_rset()
-            self.assertIsInstance(self.vreg['views'].select('primary', req, rset=rset),
-                                  views.CommentPrimaryView)
-            self.assertIsInstance(self.vreg['views'].select('tree', req, rset=rset),
-                                  views.CommentThreadView)
+            rset = req.create_entity(
+                "Comment", content="bouh!", comments=self.b
+            ).as_rset()
+            self.assertIsInstance(
+                self.vreg["views"].select("primary", req, rset=rset),
+                views.CommentPrimaryView,
+            )
+            self.assertIsInstance(
+                self.vreg["views"].select("tree", req, rset=rset),
+                views.CommentThreadView,
+            )
 
     def test_possible_actions(self):
         with self.admin_access.web_request() as req:
-            req.create_entity('Comment', content=u"bouh!", comments=self.b)
-            self.create_user(req, 'user')  # will commit
-            rset = req.execute('Any X WHERE X is BlogEntry')
+            req.create_entity("Comment", content="bouh!", comments=self.b)
+            self.create_user(req, "user")  # will commit
+            rset = req.execute("Any X WHERE X is BlogEntry")
             actions = self.pactions(req, rset)
-            self.assertIn(('reply_comment', views.AddCommentAction), actions)
-            self.assertNotIn(('edit_comment', views.EditCommentAction), actions)
-            rset = req.execute('Any X WHERE X is Comment')
+            self.assertIn(("reply_comment", views.AddCommentAction), actions)
+            self.assertNotIn(("edit_comment", views.EditCommentAction), actions)
+            rset = req.execute("Any X WHERE X is Comment")
             actions = self.pactions(req, rset)
-            self.assertIn(('reply_comment', views.ReplyCommentAction), actions)
-            self.assertIn(('edit_comment', views.EditCommentAction), actions)
+            self.assertIn(("reply_comment", views.ReplyCommentAction), actions)
+            self.assertIn(("edit_comment", views.EditCommentAction), actions)
             req.cnx.commit()
 
-        with self.new_access('user').web_request() as req:
-            rset = req.execute('Any X WHERE X is Comment')
+        with self.new_access("user").web_request() as req:
+            rset = req.execute("Any X WHERE X is Comment")
             actions = self.pactions(req, rset)
-            self.assertIn(('reply_comment', views.ReplyCommentAction), actions)
-            self.assertNotIn(('edit_comment', views.EditCommentAction), actions)
-            rset = req.execute('INSERT Comment X: X content "ho bah non!", X comments B WHERE B is Comment')
+            self.assertIn(("reply_comment", views.ReplyCommentAction), actions)
+            self.assertNotIn(("edit_comment", views.EditCommentAction), actions)
+            rset = req.execute(
+                'INSERT Comment X: X content "ho bah non!", X comments B WHERE B is Comment'
+            )
             req.cnx.commit()
             actions = self.pactions(req, rset)
-            self.assertIn(('reply_comment', views.ReplyCommentAction), actions)
-            self.assertIn(('edit_comment', views.EditCommentAction), actions)
+            self.assertIn(("reply_comment", views.ReplyCommentAction), actions)
+            self.assertIn(("edit_comment", views.EditCommentAction), actions)
 
-        with self.new_access('anon').web_request() as req:
-            rset = req.execute('Any X WHERE X is Comment')
+        with self.new_access("anon").web_request() as req:
+            rset = req.execute("Any X WHERE X is Comment")
             self.assertEqual(self.pactions(req, rset), [])
 
     def test_nonregr_possible_actions(self):
         with self.admin_access.web_request() as req:
-            req.create_entity('Comment', content=u"bouh!", comments=self.b)
-            req.create_entity('Comment', content=u"Yooo!", comments=self.b)
+            req.create_entity("Comment", content="bouh!", comments=self.b)
+            req.create_entity("Comment", content="Yooo!", comments=self.b)
             # now two comments are commenting the blog
             b = req.entity_from_eid(self.b)
-            rset = b.related('comments', 'object')
+            rset = b.related("comments", "object")
             self.assertEqual(len(rset), 2)
-            self.assertTrue(self.vreg['actions'].select('reply_comment', req, rset=rset, row=0))
-            self.assertTrue(self.vreg['actions'].select('reply_comment', req, rset=rset, row=1))
+            self.assertTrue(
+                self.vreg["actions"].select("reply_comment", req, rset=rset, row=0)
+            )
+            self.assertTrue(
+                self.vreg["actions"].select("reply_comment", req, rset=rset, row=1)
+            )
 
     def test_add_related_actions(self):
         with self.admin_access.web_request() as req:
-            req.create_entity('Comment', content=u"bouh!", comments=self.b)
-            self.create_user(req, 'user')  # will comit
-            rset = req.execute('Any X WHERE X is Comment')
+            req.create_entity("Comment", content="bouh!", comments=self.b)
+            self.create_user(req, "user")  # will comit
+            rset = req.execute("Any X WHERE X is Comment")
             self.assertEqual(self.pactions_by_cats(req, rset), [])
             req.cnx.commit()
 
-        with self.new_access('user').web_request() as req:
-            rset = req.execute('Any X WHERE X is Comment')
+        with self.new_access("user").web_request() as req:
+            rset = req.execute("Any X WHERE X is Comment")
             self.assertEqual(self.pactions_by_cats(req, rset), [])
 
-        with self.new_access('anon').web_request() as req:
-            rset = req.execute('Any X WHERE X is Comment')
+        with self.new_access("anon").web_request() as req:
+            rset = req.execute("Any X WHERE X is Comment")
             self.assertEqual(self.pactions_by_cats(req, rset), [])
 
     def test_path(self):
         with self.admin_access.repo_cnx() as cnx:
-            c1 = cnx.create_entity('Comment', content=u"oijzr", comments=self.b)
-            itreec1 = c1.cw_adapt_to('ITree')
-            c11 = cnx.create_entity('Comment', content=u"duh?", comments=c1)
-            itreec11 = c11.cw_adapt_to('ITree')
+            c1 = cnx.create_entity("Comment", content="oijzr", comments=self.b)
+            itreec1 = c1.cw_adapt_to("ITree")
+            c11 = cnx.create_entity("Comment", content="duh?", comments=c1)
+            itreec11 = c11.cw_adapt_to("ITree")
             self.assertEqual(itreec1.path(), [self.b, c1.eid])
             self.assertEqual(itreec1.root().eid, self.b)
             self.assertEqual(itreec11.path(), [self.b, c1.eid, c11.eid])
             self.assertEqual(itreec11.root().eid, self.b)
 
     def test_comments_ascending_order(self):
         with self.admin_access.repo_cnx() as cnx:
             b = cnx.entity_from_eid(self.b)
-            c1 = cnx.create_entity('Comment', content=u"one", comments=self.b)
-            c11 = cnx.create_entity('Comment', content=u"one-one", comments=c1)
-            c12 = cnx.create_entity('Comment', content=u"one-two", comments=c1)
-            c2 = cnx.create_entity('Comment', content=u"two", comments=self.b)
-            self.assertEqual([c.eid for c in b.reverse_comments],
-                             [c1.eid, c2.eid])
-            self.assertEqual([c.eid for c in c1.cw_adapt_to('ITree').children()],
-                             [c11.eid, c12.eid])
+            c1 = cnx.create_entity("Comment", content="one", comments=self.b)
+            c11 = cnx.create_entity("Comment", content="one-one", comments=c1)
+            c12 = cnx.create_entity("Comment", content="one-two", comments=c1)
+            c2 = cnx.create_entity("Comment", content="two", comments=self.b)
+            self.assertEqual([c.eid for c in b.reverse_comments], [c1.eid, c2.eid])
+            self.assertEqual(
+                [c.eid for c in c1.cw_adapt_to("ITree").children()], [c11.eid, c12.eid]
+            )
 
     def test_subcomments_count(self):
         with self.admin_access.repo_cnx() as cnx:
-            c1 = cnx.create_entity('Comment', content=u"one", comments=self.b)
-            cnx.create_entity('Comment', content=u"one-one", comments=c1)
-            c12 = cnx.create_entity('Comment', content=u"one-two", comments=c1)
-            cnx.create_entity('Comment', content=u"two-one", comments=c12)
+            c1 = cnx.create_entity("Comment", content="one", comments=self.b)
+            cnx.create_entity("Comment", content="one-one", comments=c1)
+            c12 = cnx.create_entity("Comment", content="one-two", comments=c1)
+            cnx.create_entity("Comment", content="two-one", comments=c12)
             self.assertEqual(c1.subcomments_count(), 3)
 
     def test_fullthreadtext_views(self):
         with self.admin_access.web_request() as req:
-            c = req.create_entity('Comment', content=u"bouh!", comments=self.b)
-            c2 = req.create_entity('Comment', content=u"""
+            c = req.create_entity("Comment", content="bouh!", comments=self.b)
+            c2 = req.create_entity(
+                "Comment",
+                content="""
 some long <b>HTML</b> text which <em>should not</em> fit on 80 characters, so i'll add some extra xxxxxxx.
-Yeah !""", content_format=u"text/html", comments=c)
+Yeah !""",
+                content_format="text/html",
+                comments=c,
+            )
             req.cnx.commit()  # needed to set author
-            content = c2.view('fullthreadtext')
+            content = c2.view("fullthreadtext")
             # remove date
-            content = re.sub('..../../.. ..:..', '', content)
-            self.assertMultiLineEqual(content,
-                                      f"""\
+            content = re.sub("..../../.. ..:..", "", content)
+            self.assertMultiLineEqual(
+                content,
+                f"""\
 > On  - admin wrote :
 > bouh!
 
 some long **HTML** text which _should not_ fit on 80 characters, so i'll add
 some extra xxxxxxx. Yeah !
 
 
 i18n_by_author_field: admin
-url: {BASE_URL}blogentry/%s""" % self.b)
+url: {BASE_URL}blogentry/%s"""
+                % self.b,
+            )
             # fullthreadtext_descending view
-            self.assertMultiLineEqual('''On  - admin wrote :
+            self.assertMultiLineEqual(
+                """On  - admin wrote :
 bouh!
 > On  - admin wrote :
 > some long **HTML** text which _should not_ fit on 80 characters, so i\'ll add
 > some extra xxxxxxx. Yeah !
 > 
 
-''', re.sub('..../../.. ..:..', '', c.view('fullthreadtext_descending')))  # noqa: W291
+""",
+                re.sub("..../../.. ..:..", "", c.view("fullthreadtext_descending")),
+            )  # noqa: W291
 
     def test_fulltext_view_markdown(self):
         with self.admin_access.web_request() as req:
-            content = u'\n'.join([
-                (u'some long *Markdown* text which **should not** fit on 80 '
-                 u'characters, so i\'ll add some extra xxxxxxx. Yeah !'),
-                u'',
-                u'* and a',
-                u'* list',
-            ])
-
-            comment = req.create_entity('Comment', content=content,
-                                        content_format=u'text/markdown',
-                                        comments=self.b)
+            content = "\n".join(
+                [
+                    (
+                        "some long *Markdown* text which **should not** fit on 80 "
+                        "characters, so i'll add some extra xxxxxxx. Yeah !"
+                    ),
+                    "",
+                    "* and a",
+                    "* list",
+                ]
+            )
+
+            comment = req.create_entity(
+                "Comment",
+                content=content,
+                content_format="text/markdown",
+                comments=self.b,
+            )
             req.cnx.commit()
-            content = comment.view('fulltext')
-            content = re.sub('..../../.. ..:..', '', content)
-            expected = '\n'.join([
-                'On  - admin wrote :',
-                'some long *Markdown* text which **should not** fit on 80 characters, so i\'ll add',
-                'some extra xxxxxxx. Yeah !',
-                '',
-                '* and a',
-                '* list',
-                '',
-            ])
+            content = comment.view("fulltext")
+            content = re.sub("..../../.. ..:..", "", content)
+            expected = "\n".join(
+                [
+                    "On  - admin wrote :",
+                    "some long *Markdown* text which **should not** fit on 80 characters, so i'll add",
+                    "some extra xxxxxxx. Yeah !",
+                    "",
+                    "* and a",
+                    "* list",
+                    "",
+                ]
+            )
             self.assertMultiLineEqual(content, expected)
 
     def test_edit_comment_form(self):
-
         def render_comment_form(req):
-            rset = req.create_entity('Comment', content=u'test').as_rset()
-            view = self.vreg['views'].select('editcommentform', req, rset=rset)
+            rset = req.create_entity("Comment", content="test").as_rset()
+            view = self.vreg["views"].select("editcommentform", req, rset=rset)
             return view.render()
 
-        with self.new_access('anon').web_request() as req:
+        with self.new_access("anon").web_request() as req:
             body = render_comment_form(req)
-            self.assertIn('You are not authenticated. Your comment will be anonymous', body)
+            self.assertIn(
+                "You are not authenticated. Your comment will be anonymous", body
+            )
         with self.admin_access.web_request() as req:
             body = render_comment_form(req)
-            self.assertNotIn('You are not authenticated. Your comment will be anonymous', body)
+            self.assertNotIn(
+                "You are not authenticated. Your comment will be anonymous", body
+            )
 
     def test_rssitem_view(self):
         with self.admin_access.web_request() as req:
-            c1 = req.create_entity('Comment', content=u'foo', comments=self.b)
-            c2 = req.create_entity('Comment', content=u'foo', comments=c1)
+            c1 = req.create_entity("Comment", content="foo", comments=self.b)
+            c2 = req.create_entity("Comment", content="foo", comments=c1)
             c1.cw_set(comments=c2)
-            xmldata = '<items>' + c1.view('rssitem') + '</items>'
+            xmldata = "<items>" + c1.view("rssitem") + "</items>"
             doc = etree.fromstring(xmldata, etree.XMLParser(recover=True))
             self.assertEqual(
-                [node.text for node in doc.xpath('//guid')], [
-                    '{}comment/{}'.format(BASE_URL, c1.eid),
-                    '{}comment/{}'.format(BASE_URL, c2.eid),
-                ])
+                [node.text for node in doc.xpath("//guid")],
+                [
+                    f"{BASE_URL}comment/{c1.eid}",
+                    f"{BASE_URL}comment/{c2.eid}",
+                ],
+            )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import unittest
+
     unittest.main()
```

### Comparing `cubicweb-comment-2.0.0/test/unittest_hooks.py` & `cubicweb-comment-3.0.0/test/unittest_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from cubicweb.devtools import BASE_URL
-from cubicweb.devtools.testlib import CubicWebTC, MAILBOX
+from cubicweb.devtools.testlib import MAILBOX
+from cubicweb_web.devtools.testlib import WebCWTC
 
 
-class CommentViewsTC(CubicWebTC):
+class CommentViewsTC(WebCWTC):
     def setup_database(self):
         with self.admin_access.repo_cnx() as cnx:
             self.set_option("default-dest-addrs", "john.doe@example.com")
             self.blogentry = cnx.create_entity(
                 "BlogEntry", title="une news !", content="cubicweb c'est beau"
             )
             cnx.commit()
```

