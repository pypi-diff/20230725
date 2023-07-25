# Comparing `tmp/cubicweb-timesheet-0.9.1.tar.gz` & `tmp/cubicweb-timesheet-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-timesheet-0.9.1.tar", last modified: Tue Jan  7 17:39:52 2014, max compression, from Unix
+gzip compressed data, was "cubicweb-timesheet-1.0.0.tar", last modified: Tue Jul 25 09:16:45 2023, max compression
```

## Comparing `cubicweb-timesheet-0.9.1.tar` & `cubicweb-timesheet-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,60 @@
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2014-01-07 17:39:52.000000 cubicweb-timesheet-0.9.1/
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2014-01-07 17:39:52.000000 cubicweb-timesheet-0.9.1/test/
--rw-r--r--   0 narval     (105) narval     (109)      970 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/test/test_timesheet.py
--rw-r--r--   0 narval     (105) narval     (109)      137 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/README
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2014-01-07 17:39:52.000000 cubicweb-timesheet-0.9.1/data/
--rw-r--r--   0 narval     (105) narval     (109)      186 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/data/cubes.timesheet.css
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2014-01-07 17:39:52.000000 cubicweb-timesheet-0.9.1/views/
--rw-r--r--   0 narval     (105) narval     (109)     2447 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/views/boxes.py
--rw-r--r--   0 narval     (105) narval     (109)     3865 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/views/forms.py
--rw-r--r--   0 narval     (105) narval     (109)    10776 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/views/activity.py
--rw-r--r--   0 narval     (105) narval     (109)     4078 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/views/startup.py
--rw-r--r--   0 narval     (105) narval     (109)     3281 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/views/__init__.py
--rw-r--r--   0 narval     (105) narval     (109)      893 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/views/facets.py
--rw-r--r--   0 narval     (105) narval     (109)    14031 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/views/euser.py
--rw-r--r--   0 narval     (105) narval     (109)    12306 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/views/primaries.py
--rw-rw-r--   0 narval     (105) narval     (109)      437 2014-01-07 17:39:52.000000 cubicweb-timesheet-0.9.1/PKG-INFO
--rw-r--r--   0 narval     (105) narval     (109)     2165 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/schema.py
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2014-01-07 17:39:52.000000 cubicweb-timesheet-0.9.1/migration/
--rw-r--r--   0 narval     (105) narval     (109)      340 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/migration/postcreate.py
--rw-r--r--   0 narval     (105) narval     (109)      200 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/migration/0.5.1_Any.py
--rw-r--r--   0 narval     (105) narval     (109)       70 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/migration/0.9.0_Any.py
--rw-r--r--   0 narval     (105) narval     (109)       70 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/migration/0.9.1_Any.py
--rw-r--r--   0 narval     (105) narval     (109)     1081 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/hooks.py
--rw-r--r--   0 narval     (105) narval     (109)       25 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/__init__.py
--rw-r--r--   0 narval     (105) narval     (109)     7513 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/entities.py
--rw-r--r--   0 narval     (105) narval     (109)     1656 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/__pkginfo__.py
-drwxrwxr-x   0 narval     (105) narval     (109)        0 2014-01-07 17:39:52.000000 cubicweb-timesheet-0.9.1/i18n/
--rw-r--r--   0 narval     (105) narval     (109)     6016 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/i18n/en.po
--rw-r--r--   0 narval     (105) narval     (109)     5344 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/i18n/es.po
--rw-r--r--   0 narval     (105) narval     (109)     7105 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/i18n/fr.po
--rw-r--r--   0 narval     (105) narval     (109)     5478 2014-01-07 17:33:25.000000 cubicweb-timesheet-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.676563 cubicweb-timesheet-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      557 2023-07-25 09:16:45.672563 cubicweb-timesheet-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.196557 cubicweb-timesheet-1.0.0/cubicweb_timesheet/
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      919 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.220557 cubicweb-timesheet-1.0.0/cubicweb_timesheet/data/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/data/cubes.timesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)      406 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/data/cubes.timesheet.js
+-rw-rw-rw-   0 root         (0) root         (0)     7538 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.240557 cubicweb-timesheet-1.0.0/cubicweb_timesheet/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     5977 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     5310 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)     7050 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.344559 cubicweb-timesheet-1.0.0/cubicweb_timesheet/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/migration/0.12.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/migration/0.13.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/migration/0.17.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/migration/0.18.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/migration/0.5.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/migration/0.9.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/migration/0.9.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.408559 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/
+-rw-rw-rw-   0 root         (0) root         (0)     3290 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12765 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11294 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/euser.py
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/facets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3988 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/jsonp.py
+-rw-rw-rw-   0 root         (0) root         (0)    10959 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/primaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4089 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.220557 cubicweb-timesheet-1.0.0/cubicweb_timesheet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-07-25 09:16:44.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1505 2023-07-25 09:16:45.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:16:44.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-25 09:16:44.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:16:44.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-25 09:16:44.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-25 09:16:44.000000 cubicweb-timesheet-1.0.0/cubicweb_timesheet.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.664563 cubicweb-timesheet-1.0.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)     5109 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/debian/copyright
+-rwxrwxrwx   0 root         (0) root         (0)       45 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/debian/rules
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/debian/watch
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:16:45.676563 cubicweb-timesheet-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.672563 cubicweb-timesheet-1.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:16:45.672563 cubicweb-timesheet-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/test/test_timesheet.py
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/test/unittest_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2023-07-25 09:15:45.000000 cubicweb-timesheet-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-timesheet-0.9.1/views/boxes.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/boxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """gingouz specific boxes
 
 :organization: Logilab
-:copyright: 2003-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+:copyright: 2003-2014 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 from datetime import date
 
 from logilab.common.date import first_day
 from logilab.common.registry import objectify_predicate
 from logilab.mtconverter import xml_escape
 
+from cubicweb import _
 from cubicweb import tags
-from cubicweb.web import component
+from cubicweb_web import component
+
 
 @objectify_predicate
 def has_resource(cls, req, **kwargs):
     return bool(req.user.cw_adapt_to('timesheet.IResource'))
 
 
 class ActivitiesBox(component.CtxComponent):
     """display a box with an activity calendar"""
     __regid__ = 'timesheet.activities_box'
     __select__ = component.CtxComponent.__select__ & has_resource()
-    visible = True # enabled by default
+    visible = True  # enabled by default
     title = _('My activities')
     order = 10
 
     def render_title(self, w):
         title = self._cw._(self.title)
         url = self._cw.build_url(rql="Any C WHERE R use_calendar CU, CU use_calendar C, "
                                  "R euser U, U eid %s" % self._cw.user.eid)
@@ -44,15 +46,15 @@
 
 
 class MyActionsBox(component.CtxComponent):
     """display a box with util links"""
     __regid__ = 'timesheet.my_actions_box'
     __select__ = component.CtxComponent.__select__ & has_resource()
 
-    visible = True # enabled by default
+    visible = True  # enabled by default
     title = _('My actions')
     order = 3
 
     def render_body(self, w):
         req = self._cw
         resource = req.user.cw_adapt_to('timesheet.IResource').resource
         self.append(tags.a(req._('my_space'), href=resource.absolute_url()))
```

### Comparing `cubicweb-timesheet-0.9.1/views/forms.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,94 @@
-from cubicweb.predicates import is_instance
-from cubicweb.web.views import autoform
-from cubicweb.web import INTERNAL_FIELD_VALUE, uicfg, formfields as ff, formwidgets as fw
-from cubicweb.web.formwidgets import HiddenInput
+import six
+from cubicweb_web import INTERNAL_FIELD_VALUE, formwidgets as fw
+from cubicweb_web.views import uicfg
 
 _afs = uicfg.autoform_section
 _affk = uicfg.autoform_field_kwargs
 
 _afs.tag_subject_of(('Resource', 'use_calendar', '*'), 'main', 'inlined')
 _afs.tag_subject_of(('WorkOrder', 'uses_technology', '*'), 'main', 'attributes')
 _afs.tag_subject_of(('WorkOrder', 'uses_technology', '*'), 'muledit', 'attributes')
 # XXX should not be always hidden
 _affk.tag_subject_of(('Activity', 'done_by', '*'), {'widget': fw.HiddenInput})
 
 
-
 def tp_periods_choices(form, field, limit=None):
-    #voc = self.object_relation_vocabulary(rtype, limit)
     if form._cw.form.get('vid') == 'holidays_form':
         rset = form._cw.execute("Any C WHERE R use_calendar CU, CU use_calendar C, "
-                                "R euser U, U eid %(u)s", {'u':form._cw.user.eid})
-        return sorted((v.view('combobox'), unicode(v.eid))
+                                "R euser U, U eid %(u)s", {'u': form._cw.user.eid})
+        return sorted((v.view('combobox'), six.text_type(v.eid))
                       for v in rset.entities())
     return field.__class__.choices(field, form, limit=limit)
+
+
 _affk.tag_object_of(('*', 'periods', 'Timeperiod'),
                     {'choices': tp_periods_choices})
 
 
-
 def activity_done_by_choices(form, field, limit=None):
     user = form._cw.user
     entity = form.edited_entity
     # managers can edit the done_by relation as they wish
     if user.is_in_group('managers'):
         rql = 'Any R,T '
         if limit is not None:
             rql += 'LIMIT %s ' % limit
         rql += 'WHERE R is Resource, R title T'
-        return sorted((entity.view('combobox'), unicode(entity.eid))
+        return sorted((entity.view('combobox'), six.text_type(entity.eid))
                       for entity in form._cw.execute(rql).entities())
     # users can't edit an existing done_by relation
     if entity.has_eid():
         return []
     rql = 'Any R,T WHERE R euser U, R title T, U eid %(u)s'
     res = form._cw.execute(rql, {'u': user.eid}).get_entity(0, 0)
-    return [(res.view('combobox'), unicode(res.eid))]
+    return [(res.view('combobox'), six.text_type(res.eid))]
+
+
 _affk.tag_subject_of(('Activity', 'done_by', '*'),
                      {'choices': activity_done_by_choices})
 
+
 def activity_done_for_choices(form, field, limit=None):
     req = form._cw
     user = req.user
-    entity = form.edited_entity
     options = []
     open_state = req.vreg['etypes'].etype_class('WorkOrder').open_state
     # managers can edit the done_for relation as they wish
     if user.is_in_group('managers'):
         if limit is None:
             limit = ''
         else:
             limit = ' LIMIT %s' % limit
         rql = ('Any WO,T %s WHERE WO is WorkOrder, WO title T, '
                'WO in_state S, S name "%s"' % (limit, open_state))
         rset = form._cw.execute(rql)
         if rset:
             options += [(req._('workorders in state %s') % req._(open_state), None)]
-            options += sorted((entity.view('combobox'), unicode(entity.eid))
+            options += sorted((entity.view('combobox'), six.text_type(entity.eid))
                               for entity in rset.entities())
         else:
             options += [(req._('no workorders in state %s') % req._(open_state),
                          INTERNAL_FIELD_VALUE)]
     else:
         # for new entities, users will only see their matching resource
-        rql = ('DISTINCT Any WO,T WHERE WO is WorkOrder, WO title T, '
-               'WO in_state S, S name %(s)s, '
-               'WO todo_by R, R euser U')
-        rset = req.execute(rql+', U eid %(u)s', {'u': req.user.eid,
-                                                 's': open_state})
+        rset = req.execute('DISTINCT Any WO,T WHERE WO is WorkOrder, WO title T, '
+                           'WO in_state S, S name %(s)s, '
+                           'WO todo_by R, R euser U, U eid %(u)s',
+                           {'u': req.user.eid, 's': open_state})
         if rset:
-            options += sorted((entity.view('combobox'), unicode(entity.eid))
+            options += sorted((entity.view('combobox'), six.text_type(entity.eid))
                               for entity in rset.entities())
         else:
             options += [(req._('no workorders'),
                          INTERNAL_FIELD_VALUE)]
+    # ensure current value is in the list
+    if form.edited_entity.has_eid():
+        budget = form.edited_entity.done_for[0]
+        cval = six.text_type(budget.eid)
+        if not any(val == cval for _, val in options):
+            options.insert(0, (budget.view('combobox'), six.text_type(budget.eid)))
     return options
+
+
 _affk.tag_subject_of(('Activity', 'done_for', '*'),
                      {'choices': activity_done_for_choices})
```

### Comparing `cubicweb-timesheet-0.9.1/views/activity.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/activity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # -*- coding: utf-8 -*-
 """activity related views.
 
 :organization: Logilab
-:copyright: 2007-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+:copyright: 2007-2014 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
-import datetime
-
-from logilab.common.date import todate
 
 from logilab.mtconverter import xml_escape
 
+from cubicweb import _
 from cubicweb.utils import UStringIO
 from cubicweb.schema import display_name
-from cubicweb.predicates import (is_instance, empty_rset, multi_columns_rset,
-                                match_user_groups, score_entity)
-from cubicweb.view import AnyRsetView, EntityView, EntityAdapter
-from cubicweb.web import INTERNAL_FIELD_VALUE, stdmsgs, action
-from cubicweb.web.views import tableview, calendar, navigation, editcontroller
+from cubicweb.predicates import (is_instance, multi_columns_rset,
+                                 match_user_groups, score_entity, rql_condition)
+from cubicweb_web.view import AnyRsetView, EntityView, EntityAdapter
+from cubicweb_web import action
+from cubicweb_web.component import Link
+from cubicweb_web.views import tableview, calendar, navigation, editcontroller
+
+from cubicweb_calendar.views import get_date_range_from_reqform
 
-from cubes.calendar.views import get_date_range_from_reqform
 
 class ActivitySummaryView(AnyRsetView):
     __regid__ = 'actsummary'
     __select__ = is_instance('Activity') & multi_columns_rset(7)
 
     # XXX we should make a very strict selector here
     def call(self):
         total_duration = sum(e.duration for e in self.cw_rset.entities())
         self.w(u'<h3>%s: %s</h3>' % (_('total'), total_duration))
-        self.wview('table', self.cw_rset, 'null', displaycols=range(1,6))
+        self.wview('table', self.cw_rset, 'null', displaycols=range(1, 6))
 
         resdict = {}
         for __, __, res, __, duration, __, login in self.cw_rset:
             resdur = resdict.get(login, 0)
             resdur += duration
             resdict[login] = resdur
         self.w(u'<h2>%s</h2>' % _('statistics'))
@@ -44,14 +44,15 @@
         for even_odd, (login, resdur) in enumerate(sorted(resdict.iteritems())):
             self.w(u'<tr class="%s">' % (even_odd % 2 and "odd" or "even"))
             self.w(u'<td>%s</td>' % login)
             self.w(u'<td>%s</td>' % resdur)
             self.w(u'</tr>')
         self.w(u'</table>')
 
+
 class ActivitySubmitView(EntityView):
     __regid__ = 'activities-list'
     __select__ = is_instance('Resource')
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
         firstday, lastday = get_date_range_from_reqform(self._cw.form)
@@ -76,167 +77,223 @@
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
         self.w(u'<a href="%s"><img alt="%s" src="data/accessories-text-editor.png" /></a>' %
                (xml_escape(entity.absolute_url(vid='edition')),
                 self._cw._('actions_edit')))
 
 
-class ActivityTable(EntityView):
+class ActivityTableView(EntityView):
     __regid__ = 'activitytable'
     __select__ = is_instance('Activity')
     title = _('activitytable')
 
     def call(self, showresource=True):
-        _ = self._cw._
-        headers  = [_("diem"), _("duration"), _("workpackage"), _("description"), _("state"), u""]
         eids = ','.join(str(row[0]) for row in self.cw_rset)
         rql = ('Any R, D, DUR, WO, DESCR, S, A, SN, RT, WT ORDERBY D DESC '
                'WHERE '
                '   A is Activity, A done_by R, R title RT, '
                '   A diem D, A duration DUR, '
                '   A done_for WO, WO title WT, '
                '   A description DESCR, A in_state S, S name SN, A eid IN (%s)' % eids)
-        if showresource:
-            displaycols = range(7)
-            headers.insert(0, display_name(self._cw, 'Resource'))
-        else: # skip resource column if asked to
-            displaycols = range(1, 7)
         rset = self._cw.execute(rql)
-        self.wview('editable-table', rset, 'null', #subvid='tablecontext',
-                   displayfilter=True, displayactions=False,
-                   headers=headers, displaycols=displaycols,
-                   cellvids={3: 'editable-final'})
+        self.wview('activity-table', rset, 'null',
+                   showresource=showresource)
 
 
-class GenericActivityTable(tableview.EditableTableView):
+class GenericActivityTable(tableview.RsetTableView):
     __regid__ = 'generic-activitytable'
     __select__ = multi_columns_rset()
     title = _('activitytable')
+    cellvids = {4: 'editable-final'}
+    finalvid = 'editable-final'
+    layout_args = {
+        'display_filter': 'top',
+        'add_view_actions': False,
+    }
 
     def call(self, title=None):
-        labels = self.columns_labels()
-        labels[0] = u'edit'
         strio = UStringIO()
         self.paginate(self, w=strio.write, page_size=20)
-        super(GenericActivityTable, self).call(
-            #subvid='tablecontext', headers=headers,
-            displayfilter=True, displayactions=False, actions=(),
-            cellvids={4: 'editable-final'})
+        super(GenericActivityTable, self).call()
         self.w(strio.getvalue())
 
 
+class ActivityTable(tableview.RsetTableView):
+    __regid__ = 'activity-table'
+
+    def call(self, title=None, showresource=True):
+        _ = self._cw._
+        self.headers = [_("diem"), _("duration"), _("workpackage"),
+                        _("description"), _("state"), ""]
+        if showresource:
+            self.displaycols = range(7)
+            self.headers.insert(0, display_name(self._cw, 'Resource'))
+            self.cellvids = {1: 'editable-final',
+                             2: 'editable-final',
+                             3: 'editable-final',
+                             4: 'editable-final'}
+        else:  # skip resource column if asked to
+            self.displaycols = range(1, 7)
+            self.cellvids = {
+                             0: 'editable-final',
+                             1: 'editable-final',
+                             2: 'editable-final',
+                             3: 'editable-final'}
+        super(ActivityTable, self).call()
+
+
 class ActivityCalendarItemView(calendar.CalendarItemView):
     __select__ = is_instance('Activity')
 
     def cell_call(self, row, col):
         activity = self.cw_rset.get_entity(row, col)
         self.w(u'<a href="%s">%s %s</a>' % (xml_escape(activity.absolute_url()),
                                             xml_escape(activity.workorder.dc_long_title()),
                                             activity.duration))
 
 
 class ValidateActivitiesAction(action.Action):
     __regid__ = 'validate-activities'
     __select__ = (action.Action.__select__
-                  & match_user_groups('managers')
                   & is_instance('Activity')
+                  & (match_user_groups('managers')
+                     | rql_condition('X done_for W, W owned_by U'))
                   & score_entity(lambda x: x.cw_adapt_to('IWorkflowable').state == 'pending'))
 
     category = 'mainactions'
     title = _('validate activities')
+    trname = 'validate'
 
-    def url(self):
+    def fill_menu(self, box, menu):
         if self.cw_row is None:
             eids = [row[0] for row in self.cw_rset]
         else:
             eids = (self.cw_rset[self.cw_row][self.cw_col or 0],)
-        def validate_cb(req, eids):
-            for eid in eids:
-                entity = req.entity_from_eid(eid, 'Activity')
-                entity.fire_transition('validate')
-        msg = self._cw._('activities validated')
-        return self._cw.user_callback(validate_cb, (eids,), msg)
+        menu.append(self.build_link(self.title, eids))
+
+    def build_link(self, title, eids, item=None):
+        rql = ('INSERT TrInfo X: '
+               'X by_transition BT, X wf_info_for Y '
+               'WHERE Y eid in ({0}), Y in_state S, S state_of W, '
+               'BT transition_of W, BT name \'{1}\'')
+        rql = rql.format(','.join(str(eid) for eid in eids), self.trname)
+        self._cw.add_js('cubes.timesheet.js')
+        href = self._cw.build_url('rqlio/1.0')
+        attrs = {'class': 'rqlio',
+                 'data-rql': rql}
+        return Link(href, self._cw._(title), **attrs)
+
+
+class ArchiveActivitiesAction(ValidateActivitiesAction):
+    __regid__ = 'archive-activities'
+    __select__ = (action.Action.__select__
+                  & match_user_groups('managers')
+                  & is_instance('Activity')
+                  & score_entity(lambda x: x.cw_adapt_to('IWorkflowable').state == 'validated'))
+
+    title = _('archive activities')
+    trname = 'archive'
+
+
+WORKORDER_CLOSED_STATES = ['validated', 'canceled']
 
-WORKORDER_CLOSED_STATES = ('validated', 'canceled')
 
 class MoveActivitiesAction(action.Action):
     __regid__ = 'move-activities'
     __select__ = (action.Action.__select__
-                  & match_user_groups('managers')
+                  & ~match_user_groups('managers')
                   & is_instance('Activity')
+                  & rql_condition('X done_for W, W owned_by U')
                   & score_entity(lambda x: x.cw_adapt_to('IWorkflowable').state == 'pending'))
 
     category = 'mainactions'
     submenu = _('move activities')
 
-    def actual_actions(self):
-        states = ','.join('"%s"' % state for state in WORKORDER_CLOSED_STATES)
-        for item in self._cw.execute('Any W,WT,O,OT ORDERBY OT,WT WHERE W is WorkOrder, '
-                                     'W in_state S, NOT S name IN (%s), '
-                                     'O split_into W, O title OT, W title WT'
-                                     % states).entities():
-            yield self.build_action(item.dc_long_title(), self.url(item))
-
-    def url(self, workorder):
+    def fill_menu(self, box, menu):
+        self._cw.add_js('cubes.timesheet.js')
         if self.cw_row is None:
             eids = [str(row[self.cw_col or 0]) for row in self.cw_rset]
         else:
             eids = [str(self.cw_rset[self.cw_row][self.cw_col or 0])]
-        rql = 'SET X done_for Y WHERE X eid IN(%s), Y eid %%(y)s' % ','.join(eids)
-        msg = self._cw._('activities moved to workorder %s') % workorder.dc_long_title()
-        return self._cw.user_rql_callback((rql, {'y': workorder.eid}), msg)
+        for item in self.actual_actions():
+            menu.append(self.build_link(item.dc_long_title(), item, eids))
 
+    def actual_actions(self):
+        states = ','.join('"%s"' % state for state in WORKORDER_CLOSED_STATES)
+        return self._cw.execute('Any W,WT,O,OT ORDERBY OT,WT WHERE W is WorkOrder, '
+                                'W in_state S, NOT S name IN (%s), '
+                                'O split_into W, O title OT, W title WT'
+                                % states).entities()
+
+    def build_link(self, title, workorder, eids):
+        rql = 'SET X done_for Y WHERE X eid IN({0}), Y eid {1}'
+        rql = rql.format(','.join(eids), workorder.eid)
+        href = self._cw.build_url('rqlio/1.0')
+        attrs = {'class': 'rqlio',
+                 'data-rql': rql, }
+        return Link(href, title, **attrs)
+
+
+class ManagerMoveActivitiesAction(MoveActivitiesAction):
+    __select__ = (action.Action.__select__
+                  & match_user_groups('managers')
+                  & is_instance('Activity')
+                  & score_entity(lambda x: x.cw_adapt_to('IWorkflowable').state != 'archived'))
+
+    def actual_actions(self):
+        return self._cw.execute('Any W,WT,O,OT ORDERBY OT,WT WHERE W is WorkOrder, '
+                                'O split_into W, O title OT, W title WT'
+                                ).entities()
 
 
 class ActivityIPrevNextAdapter(navigation.IPrevNextAdapter):
     __select__ = is_instance('Activity')
 
     def previous_entity(self):
         entity = self.entity
         execute = self._cw.execute
         # if the smallest duration
         rset = execute("Activity A ORDERBY DUR DESC LIMIT 1 WHERE "
                        "A done_by R, R euser U, U eid %(u)s, A diem %(d)s, "
                        "A duration DUR, A duration < %(t)s",
                        {'u': entity.user.eid, 'd': entity.diem,
-                        't':entity.duration})
+                        't': entity.duration})
         if rset:
             return rset.get_entity(0, 0)
         # the smallest id
         rset = execute("Activity A ORDERBY A DESC LIMIT 1 WHERE "
                        "A done_by R, R euser U, U eid %(u)s, A diem %(d)s, "
                        "A duration < %(t)s, A eid < %(eid)s",
                        {'u': entity.user.eid, 'd': entity.diem,
-                        't': entity.duration, 'eid':entity.eid})
+                        't': entity.duration, 'eid': entity.eid})
         if rset:
             return rset.get_entity(0, 0)
         # next days
         rset = execute("Activity A ORDERBY D DESC LIMIT 1 WHERE "
                        "A done_by R, R euser U, U eid %(u)s, "
                        "A diem D, A diem < %(d)s ",
                        {'u': entity.user.eid, 'd': entity.diem})
         if rset:
             return rset.get_entity(0, 0)
 
-
     def next_entity(self):
         entity = self.entity
         execute = self._cw.execute
         rset = execute("Activity A ORDERBY DUR LIMIT 1 WHERE "
                        "A done_by R, R euser U, U eid %(u)s, A diem %(d)s, "
                        "A duration DUR, A duration > %(t)s",
                        {'u': entity.user.eid, 'd': entity.diem,
                         't': entity.duration})
         if rset:
             return rset.get_entity(0, 0)
         rset = execute("Activity A ORDERBY A LIMIT 1 WHERE "
                        "A done_by R, R euser U, U eid %(u)s, A diem %(d)s, "
                        "A eid > %(eid)s, A duration > %(t)s",
                        {'u': entity.user.eid, 'd': entity.diem,
-                        't':entity.duration, 'eid':entity.eid})
+                        't': entity.duration, 'eid': entity.eid})
         if rset:
             return rset.get_entity(0, 0)
         rset = execute("Activity A ORDERBY D LIMIT 1 WHERE "
                        "A done_by R, R euser U, U eid %(u)s, "
                        "A diem D, A diem > %(d)s ",
                        {'u': entity.user.eid, 'd': entity.diem})
         if rset:
```

### Comparing `cubicweb-timesheet-0.9.1/views/startup.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/startup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """activity related startup views.
 
 :organization: Logilab
-:copyright: 2007-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+:copyright: 2007-2014 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 from logilab.common.date import strptime
 
+from cubicweb import _
 from cubicweb.predicates import match_form_params
-from cubicweb.view import StartupView
-from cubicweb.web import httpcache
-from cubicweb.web.views import startup
+from cubicweb_web.view import StartupView
+from cubicweb_web import httpcache
+from cubicweb_web.views import startup
+
 
 class WorkcaseActivityStatsView(StartupView):
     __regid__ = 'actstats'
     __select__ = StartupView.__select__ & match_form_params('workcase')
     ref_attr = u'workcase'
 
     def call(self):
         _ = self._cw._
         ref = self._cw.form[self.ref_attr]
         start, stop, restrict = self.build_startstop_restriction()
         rset = self.get_activities(ref, start, stop, restrict)
         self.wtitle(ref, start, stop)
         self.wview('actsummary', rset, 'null')
 
-
     def wtitle(self, ref, start, stop):
         tail = ''
         if start:
             tail = '%s %s' % (_('from'), self.format_date(start))
         if stop:
             tail += ' %s %s' % (_('until'), self.format_date(stop))
         self.w(u'<h1>%s - %s</h1>' % (ref, tail))
 
-
     def build_startstop_restriction(self):
         restrict = []
         start = self._cw.form.get('start')
         stop = self._cw.form.get('stop')
         # XXX (syt) should use self._cw.parse_datetime(), no? (maybe not if we
         # rely on generated url)
         if start:
@@ -48,47 +48,46 @@
         if stop:
             stop = strptime(stop, '%Y-%m-%d')
             restrict.append('A diem < %(stop)s')
         if restrict:
             return start, stop, ',' + ','.join(restrict)
         return start, stop, ''
 
-
     def get_activities(self, ref, start=None, stop=None, restrict=u''):
         rql = ('Any A, DI, R, DESCR, D, WO, L ORDERBY DI WHERE A is Activity, '
                'A done_for WO, O split_into WO, W title %%(title)s, '
                'A duration D, A diem DI, A description DESCR, '
                'A done_by R, R euser U, U login L %s' % restrict)
-        return self._cw.execute(rql, {'ref' : ref, 'start' : start,
-                                         'stop' : stop, })
-
+        return self._cw.execute(rql, {'ref': ref, 'start': start,
+                                      'stop': stop, })
 
 
 class ProjectActivityStatsView(WorkcaseActivityStatsView):
     __regid__ = 'prj-actstats'
     __select__ = StartupView.__select__ & match_form_params('project')
     ref_attr = u'project'
 
     def get_activities(self, ref, start=None, stop=None, restrict=u''):
         rql = ('Any A, DI, R, DESCR, D, V, L ORDERBY DI WHERE A is Activity, '
                'A done_for W, version_of P, P name %%(ref)s, A duration D, '
                'A diem DI, A description DESCR, A done_by R, R euser U, '
                'U login L %s' % restrict)
-        return self._cw.execute(rql, {'ref' : ref, 'start' : start,
-                                         'stop' : stop, })
+        return self._cw.execute(rql, {'ref': ref, 'start': start,
+                                      'stop': stop, })
+
 
 class MyActivities(startup.IndexView):
     http_cache_manager = httpcache.NoHTTPCacheManager
 
     title = _('my activities')
 
     def call(self):
         req = self._cw
         _ = req._
-        req.add_js( ('cubicweb.ajax.js', 'cubicweb.edition.js') )
+        req.add_js(('cubicweb.ajax.js', 'cubicweb.edition.js'))
         req.add_css('cubicweb.form.css')
         iresource = self._cw.user.cw_adapt_to('timesheet.IResource')
         if iresource:
             resource = iresource.resource
             self.w(u'Go to your <a href="%s">resource page (%s)</a>'
                    % (resource.absolute_url(), resource.title))
         # orders
```

### Comparing `cubicweb-timesheet-0.9.1/views/__init__.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 """template-specific forms/views/actions/components"""
-from cubicweb.web import uicfg
-from cubicweb.web.views.urlrewrite import SimpleReqRewriter, rgx
+from cubicweb_web.views import uicfg
+from cubicweb_web.views.urlrewrite import SimpleReqRewriter, rgx
 
 uicfg.primaryview_section.tag_object_of(('*', 'use_calendar', 'Calendar'), 'hidden')
 
 uicfg.actionbox_appearsin_addmenu.tag_subject_of(('Resource', 'has_vacation', '*'), True)
 uicfg.actionbox_appearsin_addmenu.tag_object_of(('Resource', 'euser', 'CWUser'), True)
 
-uicfg.reledit_ctrl.tag_subject_of(('Activity', 'done_for', 'WorkOrder'),
+uicfg.reledit_ctrl.tag_subject_of(('Activity', 'done_for', '*'),
                                   {'rvid': 'outofcontext'})
 
 
 rql_all_users_resources = (r'Any R,L ORDERBY L WHERE R is Resource, R euser U,'
                            r' U login L,U in_state S, S name "activated"')
 
 rql_user_or_group_resources = (r'Any R WHERE R is Resource, R euser U,'
                                r' EXISTS (U login "\1")'
                                r' OR EXISTS(U in_group G, G name "\1")')
 
 
 class TimesheetReqRewriter(SimpleReqRewriter):
     rules = [
 
-        (rgx('/activities/(.*?)/(\d{4})$'),
+        (rgx(r'/activities/(.*?)/(\d{4})$'),
          dict(year=r'\2', month=r'01', day=r'01',
               vid='activities-submit',
               rql=(r'Any A ORDERBY D WHERE A is Activity, A diem D,'
                    r' A diem >= "\2-01-01", A diem <= "\2-12-31", A done_by R,'
                    r' R euser U, U login "\1"'))),
 
-        (rgx('/activities/(.*?)/(\d{4})-(\d\d)'),
+        (rgx(r'/activities/(.*?)/(\d{4})-(\d\d)'),
          dict(year=r'\2', month=r'\3', day=r'01', vid='activities-submit',
               rql=(r'Any A WHERE A is Activity, A diem "\2-\3-01",'
                    r' A done_by R, R euser U, U login "\1"'))),
 
-        (rgx('/activities/(.*?)/(\d{8})-(\d{8})'),
+        (rgx(r'/activities/(.*?)/(\d{8})-(\d{8})'),
          dict(vid='activities-list', firstday=r'\2', lastday=r'\3',
               rql=r'Any R WHERE R is Resource, R title "\1"')),
 
-        (rgx('/activities/(.*?)/(\d{8})$'),
+        (rgx(r'/activities/(.*?)/(\d{8})$'),
          dict(vid='activities-list', firstday=r'\2',
               rql=r'Any R WHERE R is Resource, R title "\1"')),
 
         # this rule is for backward compatibility
-        (rgx('/activities/(.*?)/(\d{4})-(\d\d)-(\d\d)'),
+        (rgx(r'/activities/(.*?)/(\d{4})-(\d\d)-(\d\d)'),
          dict(year=r'\2', month=r'\3', day=r'\4', vid='activities-submit',
               rql=(r'Any A WHERE A is Activity, A diem "\2-\3-\4", A done_by R,'
                    r' R euser U, U login "\1"'))),
 
-        (rgx('/missing-activities/all/(\d{8})'),
+        (rgx(r'/missing-activities/all/(\d{8})'),
          dict(vid='missing-activities', firstday=r'\1',
               rql=rql_all_users_resources)),
 
-        (rgx('/missing-activities/all/(\d{8})-(\d{8})'),
+        (rgx(r'/missing-activities/all/(\d{8})-(\d{8})'),
          dict(vid='missing-activities', firstday=r'\1', lastday=r'\2',
               rql=rql_all_users_resources)),
 
-        (rgx('/missing-activities/all/(\d{8})-[tT][oO][dD][aA][yY]'),
+        (rgx(r'/missing-activities/all/(\d{8})-[tT][oO][dD][aA][yY]'),
          dict(vid='missing-activities', firstday=r'\1', lastday='TODAY',
               rql=rql_all_users_resources)),
 
-        (rgx('/missing-activities/(.*?)/(\d{8})'),
+        (rgx(r'/missing-activities/(.*?)/(\d{8})'),
          dict(vid='missing-activities', firstday=r'\2',
               rql=rql_user_or_group_resources)),
 
-        (rgx('/missing-activities/(.*?)/(\d{8})-(\d{8})'),
+        (rgx(r'/missing-activities/(.*?)/(\d{8})-(\d{8})'),
          dict(vid='missing-activities', firstday=r'\2', lastday=r'\3',
               rql=rql_user_or_group_resources)),
 
-        (rgx('/missing-activities/(.*?)/(\d{8})-[tT][oO][dD][aA][yY]'),
+        (rgx(r'/missing-activities/(.*?)/(\d{8})-[tT][oO][dD][aA][yY]'),
          dict(vid='missing-activities', firstday=r'\2', lastday='TODAY',
               rql=rql_user_or_group_resources)),
         ]
```

### Comparing `cubicweb-timesheet-0.9.1/views/facets.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/facets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from cubicweb.predicates import is_instance
-from cubicweb.web.facet import RelationFacet, AttributeFacet, RangeFacet, DateRangeFacet
+from cubicweb_web.facet import RelationFacet, RangeFacet, DateRangeFacet
+
 
 class ActivityDurationFacet(RangeFacet):
     __regid__ = 'duration-facet'
     __select__ = RangeFacet.__select__ & is_instance('Activity')
     rtype = 'duration'
 
+
 class ActivityDiemFacet(DateRangeFacet):
     __regid__ = 'diem-facet'
     __select__ = DateRangeFacet.__select__ & is_instance('Activity')
     rtype = 'diem'
 
+
 class ActivityWorkorderFacet(RelationFacet):
     __regid__ = 'activity-workorder-facet'
     __select__ = RelationFacet.__select__ & is_instance('Activity')
     rtype = 'done_for'
     target_attr = 'title'
+    label_vid = 'textoutofcontext'
+
 
 class ActivityResourceFacet(RelationFacet):
     __regid__ = 'activity-resource-facet'
     __select__ = RelationFacet.__select__ & is_instance('Activity')
     accepts = ('Activity',)
     rtype = 'done_by'
     target_attr = 'title'
-
```

### Comparing `cubicweb-timesheet-0.9.1/views/euser.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/euser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,22 @@
 import datetime
-from urlparse import urlparse
+from collections import defaultdict
 
 from logilab.mtconverter import xml_escape
 from logilab.common.date import (date_range, previous_month, next_month,
-                                 first_day, last_day, todate)
+                                 first_day, last_day)
 
-from rql.utils import rqlvar_maker
+from cubicweb import _
+from cubicweb_web.view import EntityView
+from cubicweb.predicates import is_instance, one_line_rset
+from cubicweb_web import form
+from cubicweb_web.views import json
 
-from cubicweb.view import AnyRsetView, EntityView
-from cubicweb.predicates import match_form_params, is_instance, one_line_rset, adaptable
-from cubicweb.uilib import toggle_action, printable_value
-from cubicweb.web import INTERNAL_FIELD_VALUE, stdmsgs, form
-
-from cubes.calendar.entities import BadCalendar
-from cubes.calendar.views import get_date_range_from_reqform
-
-
-class CWUserActivitySummaryView(EntityView):
-    __regid__ = 'euser-stats'
-    __select__ = match_form_params('start', 'stop') & is_instance('CWUser')
-
-    def cell_call(self, row, col):
-        _ = self._cw._
-        entity = self.cw_rset.get_entity(row, col)
-        start = strptime(self._cw.form['start'], '%Y-%m-%d')
-        stop = strptime(self._cw.form['stop'], '%Y-%m-%d')
-        self.w(u'<h1>%s %s</h1>' % (_('statisitics for user'), self._cw.user.login))
-        self.w(u'<div class="actsum"><table class="listing"><tr>')
-        self.w(u'<th>%s</th><th>%s</th><th>%%</th>' %
-               (_('project'), _('days worked')))
-        self.w(u'</tr><tr>')
-        total_days = 0
-        # select workcases' activities
-        rql = ("Any W, SUM(DUR) WHERE A is Activity, A done_by R, "
-               "R euser U, U eid %(x)s, A diem >= %(start)s, "
-               "A diem < %(stop)s, A duration DUR, A workorder WP, W split_into WP GROUPBY W")
-        wactivities = self._cw.execute(rql, {'x' : entity.eid,
-                                             'start' : start, 'stop' : stop})
-        if wactivities:
-            total_days += sum(dur for __, dur in wactivities)
-        # select projects' activities
-        rql = ("Any P, SUM(DUR) WHERE A is Activity, A done_by R, "
-               "R euser U, U eid %(x)s,A diem >= %(start)s, "
-               "A diem < %(stop)s, A duration DUR, A workorder WP, WP version_of P GROUPBY P")
-        pactivities = self._cw.execute(rql, {'x' : entity.eid,
-                                             'start' : start, 'stop' : stop})
-        if pactivities:
-            total_days += sum(dur for __, dur in pactivities)
-        for acts in (wactivities, pactivities):
-            for row, (__, dur) in enumerate(acts):
-                self.w(u'<tr>')
-                self.w(u'<td>%s</td><td>%s</td><td>%s</td>' % (
-                    self.view('incontext', acts, row=row, col=0), dur,
-                    (100. * dur / total_days)))
-                self.w(u'</tr>')
-        self.w(u'</table></div>')
-
-
-class CWUserActivitySubmitFormView(form.FormViewMixIn, EntityView):
-    __regid__ = 'euser-activities-submitform'
-    __select__ = one_line_rset() & is_instance('CWUser') & adaptable('timesheet.IResource')
-
-    def entity_call(self, entity, **formvalues):
-        self.warning('[cw-timesheet 0.4.0] euser-activities-submitform view is deprecated, use '
-                     'activities-submitform view on corresponding resource instead')
-        resource = entity.cw_adapt_to('timesheet.IResource').resource
-        resource.view('activities-submitform', w=self.w, **formvalues)
+from cubicweb_calendar.entities import BadCalendar
+from cubicweb_calendar.views import get_date_range_from_reqform
 
 
 class ResourceActivitySubmitFormView(form.FormViewMixIn, EntityView):
     __regid__ = 'activities-submitform'
     __select__ = one_line_rset() & is_instance('Resource')
     domid = 'activityForm'
 
@@ -93,38 +40,26 @@
                           ('done_by', 'subject')]
         vreg = self._cw.vreg
         activity = vreg['etypes'].etype_class('Activity')(self._cw)
         activity.eid = self._cw.varmaker.next()
         form = vreg['forms'].select('edition', self._cw, entity=activity,
                                     display_fields=display_fields,
                                     redirect_path=self._cw.relative_path(False))
-        form.form_buttons = form.form_buttons[:1] # only keep ok button
+        form.form_buttons = form.form_buttons[:1]  # only keep ok button
         renderer = vreg['formrenderers'].select_or_none('htable', self._cw)
         formvalues.setdefault('done_by', resource.eid)
         form.render(formvalues=formvalues, renderer=renderer, w=self.w)
 
 
-class CWUserMonitorCalendar(EntityView):
-    __regid__ = 'user_activity_calendar'
-    __select__ = is_instance('CWUser') & adaptable('timesheet.IResource')
-
-    def cell_call(self, row, col, year=None, month=None, calid=None):
-        self.warning('[cw-timesheet 0.4.0] user_activity_calendar view is deprecated, use '
-                     'activity_calendar view on corresponding resource instead')
-        user = self.cw_rset.get_entity(row, col)
-        resource = user.cw_adapt_to('timesheet.IResource').resource
-        resource.view('activity_calendar', w=self.w,
-                      year=year, month=month, day=day, calid=calid)
-
 class ResourceMonitorCalendar(EntityView):
     __regid__ = 'activity_calendar'
     __select__ = is_instance('Resource')
 
     def call(self):
-        for row in xrange(len(self.cw_rset)):
+        for row in range(len(self.cw_rset)):
             # only display resource title if there's more than one in the resultset
             if len(self.cw_rset) > 1:
                 entity = self.cw_rset.get_entity(row, 0)
                 self.w(u'<h2>%s</h2>' % xml_escape(entity.dc_title()))
             self.cell_call(row, 0)
 
     def cell_call(self, row, col, firstday=None, calid=None):
@@ -142,29 +77,29 @@
         prevurl, nexturl = self._prevnext_links(firstday, resource, calid)
         prevlink = '<a href="%s">&lt;&lt;</a>' % xml_escape(prevurl)
         nextlink = '<a href="%s">&gt;&gt;</a>' % xml_escape(nexturl)
 
         # build cells
         try:
             celldatas = self._build_activities(resource, firstday, lastday)
-        except BadCalendar, exc: # in case of missing week day information
+        except BadCalendar as exc:  # in case of missing week day information
             self.w(u'<div class="error">%s</div>' % exc)
             return
         # build table/header
         self.w(u'<table id="%s" class="activitiesCal">'
                u'<tr><th class="prev">%s</th>'
                u'<th class="calTitle" colspan="5"><span>%s</span></th>'
                u'<th class="next">%s</th></tr>'
                u'<tr><th>L</th><th>M</th><th>M</th><th>J</th><th>V</th><th>S</th><th>D</th></tr>'
                % (calid, prevlink, caption, nextlink))
         start = firstday - datetime.timedelta(firstday.weekday())
         # date range exclude last day so we should add one day, hence the 7
         stop = lastday + datetime.timedelta(7 - lastday.weekday())
         for curdate in date_range(start, stop):
-            if curdate == start or curdate.weekday() == 0: # sunday
+            if curdate == start or curdate.weekday() == 0:  # sunday
                 self.w(u'<tr>')
             self._build_calendar_cell(curdate, celldatas, firstday)
             if curdate.weekday() == 6:
                 self.w(u'</tr>')
         self.w(u'</table>')
 
     def _build_calendar_cell(self, curdate, celldatas, firstday):
@@ -182,22 +117,20 @@
     def _prevnext_links(self, curdate, resource, calid):
         prevdate = previous_month(curdate)
         nextdate = next_month(curdate)
         rql = 'Any X WHERE X eid %s' % resource.eid
         prevlink = self._cw.ajax_replace_url(calid, rql=rql, vid='activity_calendar',
                                              replacemode='swap',
                                              firstday=prevdate.strftime('%Y%m01'))
-        nextlink = self._cw.ajax_replace_url(calid, rql=rql,vid= 'activity_calendar',
+        nextlink = self._cw.ajax_replace_url(calid, rql=rql, vid='activity_calendar',
                                              replacemode='swap',
                                              firstday=nextdate.strftime('%Y%m01'))
         return prevlink, nextlink
 
     def _build_activities(self, resource, firstday, lastday):
-        # get activities
-        activities = resource.activities_summary(firstday, lastday)
         # build result
         celldatas = {}
         _today = datetime.date.today()
         dtypes = resource.get_day_types(firstday, lastday)
         for date_, dtstate, expected, day_report in resource.iter_activities(firstday, lastday):
             declared = sum([a.duration for a in day_report])
             cssclass = []
@@ -232,53 +165,73 @@
             celldatas[date_] = (cssclass, total_duration, url, summary)
         if _today in celldatas:
             # celldatas maps days to tuples (cssclass, duration, url, descr)
             celldatas[_today][0].append(u'today')
         return celldatas
 
 
-class ResourceMissingActivitiesBoard(EntityView):
+class ResourceMissingActivitiesMixIn(object):
+
+    def missing_activities(self, entity):
+        firstday, lastday = get_date_range_from_reqform(self._cw.form,
+                                                        autoset_lastday=True)
+        for first_day_of_month in date_range(firstday, lastday, incmonth=1):
+            last_day_of_month = min(lastday, last_day(first_day_of_month))
+            for date_, __, expected, day_report in entity.iter_activities(
+                    first_day_of_month, last_day_of_month):
+                declared = sum([a.duration for a in day_report])
+                if abs(declared - expected) > 1e-3:
+                    summary = ','.join(a.workorder.dc_long_title() for a in day_report)
+                    yield date_, expected, declared, summary
+
+
+class JsonResourceMissingActivitiesBoard(json.JsonMixIn, ResourceMissingActivitiesMixIn, EntityView):
+    __regid__ = 'missing-activities.json'
+    __select__ = is_instance('Resource')
+
+    def call(self):
+        result = []
+        for entity in self.cw_rset.entities():
+            result += self.entity_data(entity)
+        self.wdata(result)
+
+    def entity_call(self, entity):
+        self.wdata(list(self.entity_data(entity)))
+
+    def entity_data(self, entity):
+        for date, expected, declared, summary in self.missing_activities(entity):
+            yield {'user': entity.euser[0].login, 'date': date,
+                   'expected': expected, 'declared': declared, 'summary': summary}
+
+
+class ResourceMissingActivitiesBoard(ResourceMissingActivitiesMixIn, EntityView):
     __regid__ = 'missing-activities'
     __select__ = is_instance('Resource')
 
     def _make_report_table(self, first_day_of_month, lines):
-        table = []
-        w = table.append
+        w = self.w
         w(u'<table class="listing actboard">')
         w(u'<tr><th colspan="4">%s</th></tr>' %
-               first_day_of_month.strftime('%B %Y'))
+          first_day_of_month.strftime('%B %Y'))
         w(u'<tr><th>%s</th><th>%s</th><th>%s</th><th>%s</th></tr>' % (
                 _('date'), _('expected activity report'),
                 _('declared activity report'), _('same day activity summary')))
         for day, act_url, expected, declared, summary in lines:
             cssclass = u'missing' if declared < expected else u'toomuch'
             w(u'<tr><td><a href="%s">%s</a></td><td>%s</td><td class="%s">%s</td><td>%s</td></tr>' %
-                   (xml_escape(act_url),
-                    printable_value(self._cw, 'Date', day), expected,
-                    cssclass, declared, xml_escape(summary)))
+              (xml_escape(act_url),
+               self._cw.printable_value('Date', day), expected,
+               cssclass, declared, xml_escape(summary)))
         w(u'</table>')
-        return u'\n'.join(table)
 
-    def entity_call(self, entity, firstday=None, lastday=None):
-        _ = self._cw._
+    def entity_call(self, entity):
         self._cw.add_css('cubes.timesheet.css')
-        firstday, lastday = get_date_range_from_reqform(self._cw.form,
-                                                        autoset_lastday=True)
-        tables = []
-        for first_day_of_month in date_range(firstday, lastday, incmonth=1):
-            last_day_of_month = min(lastday, last_day(first_day_of_month))
-            lines = []
-            for date_, __, expected, day_report in entity.iter_activities(first_day_of_month, last_day_of_month):
-                declared = sum([a.duration for a in day_report])
-                act_url = self._cw.build_url('activities/%s/%s' %
-                                             (entity.title, date_.strftime('%Y%m%d')))
-                if abs(declared - expected) > 1e-3:
-                    summary = ','.join(a.workorder.dc_long_title() for a in day_report)
-                    lines.append( (date_, act_url, expected, declared, summary) )
-            if lines:
-                tables.append(self._make_report_table(first_day_of_month, lines))
-        if tables:
-            # only display resource title if there's more than one in the resultset
-            if len(self.cw_rset) > 1:
-                self.w(u'<h2>%s</h2>' % entity.dc_title())
-            for table in tables:
-                self.w(table)
+        lines_per_month = defaultdict(list)
+        for date_, expected, declared, summary in self.missing_activities(entity):
+            act_url = self._cw.build_url('activities/%s/%s' %
+                                         (entity.title, date_.strftime('%Y%m%d')))
+            month = date_.replace(day=1)
+            lines_per_month[month].append((date_, act_url, expected, declared, summary))
+        if lines_per_month:
+            self.w(u'<h2>%s</h2>' % entity.dc_title())
+            for month, lines in lines_per_month.items():
+                self._make_report_table(month, lines)
```

### Comparing `cubicweb-timesheet-0.9.1/views/primaries.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/views/primaries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 """gingouz specific primary views
 """
 
 from logilab.mtconverter import xml_escape
 
+from cubicweb import _
 from cubicweb.schema import display_name
-from cubicweb.view import EntityView
-from cubicweb.uilib import toggle_link
+from cubicweb_web.view import EntityView
 from cubicweb.predicates import is_instance, one_line_rset
-from cubicweb.web.views import baseviews, primary, tabs
+from cubicweb_web.views import primary, tabs
+
+from cubicweb_calendar.views import primaries as cal_primaries
 
-from cubes.calendar.views import primaries as cal_primaries
 
 def print_resource_ratio(self, rset):
     """prints the ratio time spent per resource / time spent by everyone
     """
     if rset:
-        duration = sum(duration for r,s,duration,i,di,mi,ma in rset if duration)
+        duration = sum(duration for r, s, duration, i, di, mi, ma in rset if duration)
         tot_by_res = dict.fromkeys((row[0] for row in rset), 0)
-        for r,s,d,i,di,mi,ma in rset:
+        for r, s, d, i, di, mi, ma in rset:
             tot_by_res[r] += d
         done = set()
         self.w(u'<p>%s</p>' % self._cw._('percentage of time spent per resource'))
         self.w(u'<table class="listing">')
         self.w(u'<tr><th>%s</th><th>%s</th></tr>' % (display_name(self._cw, 'Resource'),
                                                      self._cw._('time spent ratio')))
-        for row in xrange(len(rset)):
+        for row in range(len(rset)):
             if rset[row][0] not in done:
                 self.w(u'<tr>')
                 entity = rset.get_entity(row, 0)
                 eid = entity.eid
                 done.add(eid)
                 ratio = tot_by_res[eid] * 100 / duration
                 self.w(u'<td>%s</td><td>%.2f %%</td>' % (entity.view('oneline'), ratio))
                 self.w(u'</tr>')
         self.w(u'</table>')
 
-# order #####################################################################
 
+# order #####################################################################
 class OrderPrimaryView(tabs.TabsMixin, primary.PrimaryView):
     __select__ = is_instance('Order') & one_line_rset()
-    tabs = [_('activity-overview'), _('activity-details'), _('activity-graph')]
+    tabs = [_('activity-overview'), _('activity-details')]
     default_tab = 'activity-overview'
 
     def render_entity_title(self, entity):
         self.w(u'<h1>%s</h1>' % xml_escape(entity.dc_long_title()))
         if entity.date:
             self.w(u'%s: %s<br />' % (display_name(self._cw, 'date'),
                                       self._cw.format_date(entity.date)))
@@ -51,14 +52,15 @@
     def render_entity(self, entity):
         self.render_entity_title(entity)
         rql = 'Any WO ORDERBY T WHERE W eid %(eid)s, W split_into WO, WO title T'
         rset = self._cw.execute(rql, {'eid': entity.eid})
         self.wview('ic_progress_table_view', rset, 'null')
         self.render_tabs(self.tabs, self.default_tab, entity)
 
+
 class OrderOverviewView(EntityView):
     __regid__ = 'activity-overview'
     __select__ = is_instance('Order')
     title = _('activity-overview')
 
     def cell_call(self, row, col):
         _ = self._cw._
@@ -66,41 +68,32 @@
         rset = self._cw.execute(entity.rql_activities_groupby_resource, {'eid': entity.eid})
         headers = (_('Resource'), _('status'), _('time spent'), _('begin date'), _('end date'))
         self.wview('table', rset, 'null', headers=headers)
         self.w('<div style="margin-top: 1em"><a href="%s">%s</a></div>' %
                (self._cw.build_url(rql='Any A WHERE A done_for Y, X split_into Y, X eid %s' % entity.eid),
                 self._cw._('View all activities')))
 
+
 class OrderDetailView(EntityView):
     __regid__ = 'activity-details'
     title = _('activity-details')
     __select__ = is_instance('Order') & one_line_rset()
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
         rset = self._cw.execute(entity.rql_activities, {'eid': entity.eid})
         self.wview('generic-activitytable', rset, 'null')
 
-class OrderGraphView(EntityView):
-    __regid__ = 'activity-graph'
-    title = _('activity-graph')
-    __select__ = is_instance('Order')
-
-    def cell_call(self, row, col):
-        entity = self.cw_rset.get_entity(row, col)
-        rql = 'Any D,U WHERE O eid %(eid)s, O split_into W, A done_for W, A diem D, A duration U'
-        rset = self._cw.execute(rql, {'eid': entity.eid})
-        self.wview('plot', rset, 'null')
-
 # workorder ####################################################################
 
+
 class WorkorderPrimaryView(tabs.TabsMixin, primary.PrimaryView):
     """display workpackage's activity summary"""
     __select__ = is_instance('WorkOrder') & one_line_rset()
-    tabs = [_('activity-overview'), _('activity-details'), _('activity-graph')]
+    tabs = [_('activity-overview'), _('activity-details')]
     default_tab = 'activity-overview'
 
     def render_entity_title(self, entity):
         self.w(u'<h1>%s</h1>' % xml_escape(entity.dc_long_title()))
 
     def render_entity(self, entity):
         self.render_entity_title(entity)
@@ -111,14 +104,15 @@
             try:
                 columns.remove(col)
             except ValueError:
                 self.warning('could not remove %s from columns' % col)
         view.render(w=self.w, columns=columns)
         self.render_tabs(self.tabs, self.default_tab, entity)
 
+
 class WorkOrderOverviewView(EntityView):
     __regid__ = 'activity-overview'
     __select__ = is_instance('WorkOrder')
     title = _('activity-overview')
 
     def cell_call(self, row, col):
         _ = self._cw._
@@ -137,43 +131,33 @@
     title = _('activity-details')
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
         rset = self._cw.execute(entity.rql_activities, {'eid': entity.eid})
         self.wview('generic-activitytable', rset, 'null')
 
-class WorkOrderGraphView(EntityView):
-    __regid__ = 'activity-graph'
-    title = _('activity-graph')
-    __select__ = is_instance('WorkOrder')
-
-    def cell_call(self, row, col):
-        entity = self.cw_rset.get_entity(row, col)
-        rql = 'Any D,U WHERE W eid %(eid)s, A done_for W, A diem D, A duration U'
-        rset = self._cw.execute(rql, {'eid': entity.eid})
-        self.wview('plot', rset, 'null')
-
 # resource #####################################################################
 
+
 class ResourcePrimaryView(tabs.TabsMixin, primary.PrimaryView):
     """display workpackage's activity summary"""
     __select__ = is_instance('Resource') & one_line_rset()
     tabs = [_('activity-current'), _('activity-overview'), _('activity-details'),
-            _('activity-graph'), _('resource-calendar'),]
+            _('resource-calendar'), ]
     default_tab = 'activity-current'
 
     def render_entity_title(self, entity):
         self.w(u'<h1>%s</h1>' % xml_escape(entity.dc_long_title()))
 
     def render_entity(self, entity):
         self.render_entity_title(entity)
-        if entity.euser:
-            entity.euser[0].view('euser-activities-submitform', w=self.w)
+        entity.view('activities-submitform', w=self.w)
         self.render_tabs(self.tabs, self.default_tab, entity)
 
+
 class ResourceRecentView(EntityView):
     __regid__ = 'activity-current'
     title = _('recent activities')
     __select__ = is_instance('Resource')
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
@@ -184,49 +168,39 @@
         self.wview('activitytable', rset, 'null', showresource=False)
         self.w(u'<h2>%s</h2>' % _('Open workorders'))
         rset = self._cw.execute('Any W WHERE W is WorkOrder, W todo_by R, '
                                 'R eid %(r)s, W in_state S, S name "in progress"',
                                 {'r': entity.eid})
         self.wview('ic_progress_table_view', rset, 'null')
 
+
 class ResourceOverviewView(EntityView):
     __regid__ = 'activity-overview'
     __select__ = is_instance('Resource')
     title = _('activity overview')
 
     def cell_call(self, row, col):
         _ = self._cw._
         entity = self.cw_rset.get_entity(row, col)
         rset = self._cw.execute(entity.rql_activities_groupby_workorder, {'eid': entity.eid})
         headers = (_('workorder'), _('status'), _('time spent'), _('begin date'), _('end date'))
-        self.wview('table', rset, 'null', headers=headers, cellvids={0: 'outofcontext'})#, subvid='tablecontext')
+        self.wview('table', rset, 'null', headers=headers, cellvids={0: 'outofcontext'})  # , subvid='tablecontext')
 
 
 class ResourceDetailView(EntityView):
     __regid__ = 'activity-details'
     __select__ = is_instance('Resource') & one_line_rset()
     title = _('activity details')
 
     def cell_call(self, row, col):
         entity = self.cw_rset.get_entity(row, col)
         rset = self._cw.execute(entity.rql_activities,  {'eid': entity.eid})
         self.wview('generic-activitytable', rset, 'null')
 
 
-class ResourceGraphView(EntityView):
-    __regid__ = 'activity-graph'
-    __select__ = is_instance('Resource')
-    title = _('activity-graph')
-
-    def cell_call(self, row, col):
-        entity = self.cw_rset.get_entity(row, col)
-        rql = 'Any D,U WHERE R eid %(eid)s, A done_by R, A diem D, A duration U'
-        rset = self._cw.execute(rql, {'eid': entity.eid})
-        self.wview('plot', rset, 'null')
-
 class ResourceCalendarView(EntityView):
     __regid__ = 'resource-calendar'
     __select__ = is_instance('Resource')
     title = _('resource-calendar')
 
     def cell_call(self, row, col):
         _ = self._cw._
@@ -249,35 +223,37 @@
         _ = self._cw._
         activity = self.cw_rset.get_entity(row, col)
         self.w(u'<h2>%s: %s</h2>' % (
             display_name(self._cw, 'State'),
             xml_escape(activity.cw_adapt_to('IWorkflowable').printable_state)))
         rql = ("Any D,U,DU,WO,DE,A WHERE A is Activity, A done_by R, R euser U, "
                "A diem D, A done_for WO, A eid %(x)s, A duration DU, A description DE")
-        headers  = (_("diem"), _("euser"), _("duration"), _("workpackage"), _("description"), u"")
-        rset = self._cw.execute(rql, {'x' : activity.eid})
+        headers = (_("diem"), _("euser"), _("duration"), _("workpackage"), _("description"), u"")
+        rset = self._cw.execute(rql, {'x': activity.eid})
         if rset:
-            self.wview('table', rset, headers=headers, displaycols=range(0,6))#, subvid='tablecontext')
+            self.wview('table', rset, headers=headers, displaycols=range(0, 6))  # , subvid='tablecontext')
         else:
             # missing information or remote sources unavailable
             super(ActivityPrimaryView, self).cell_call(row, col)
 
 # calendar  ####################################################################
 
+
 class PrimaryCalendar(cal_primaries.PrimaryCalendar):
 
     def render_entity_attributes(self, entity):
         super(PrimaryCalendar, self).render_entity_attributes(entity)
         rset = self._cw.execute('Any A,B,U ORDERBY A WHERE C eid %(eid)s, '
                                 'U use_calendar CU, CU use_calendar C, '
                                 'CU start A, CU stop B', {'eid': entity.eid})
         if rset:
             self.w(u'<h2>%s</h2>' % _('Resources using this calendar'))
             headers = (_('begin date'), _('end date'), _('resource'))
             self.wview('table', rset, 'null', headers=headers)
 
 # registration #################################################################
 
+
 def registration_callback(vreg):
     vreg.register_all(globals().values(), __name__,
                       butclasses=(PrimaryCalendar,))
     vreg.register_and_replace(PrimaryCalendar, cal_primaries.PrimaryCalendar)
```

### Comparing `cubicweb-timesheet-0.9.1/schema.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from yams.buildobjs import (EntityType, RelationDefinition,
                             SubjectRelation, String, Float, Date)
 
-from cubicweb.schema import WorkflowableEntityType, ERQLExpression, RRQLExpression
-from cubes.workorder.schema import WorkOrder
-
-_ = unicode
+from cubicweb.schema import (
+    WorkflowableEntityType, ERQLExpression, RRQLExpression, RQLVocabularyConstraint)
 
 
 class Activity(WorkflowableEntityType):
     """time someone spent working on something
     """
-    __permissions__ = {'read' : ('managers', 'users'),
-                       'update' : ('managers', ERQLExpression('X in_state ST, ST name "pending", X owned_by U')),
-                       'delete' : ('managers', ERQLExpression('X in_state ST, ST name "pending", X owned_by U')),
-                       'add' : ('managers', 'users'),
+    __permissions__ = {'read': ('managers', 'users'),
+                       'update': ('managers', ERQLExpression('X in_state ST, ST name "pending", X owned_by U')),
+                       'delete': ('managers', ERQLExpression('X in_state ST, ST name "pending", X owned_by U')),
+                       'add': ('managers', 'users'),
                        }
     duration = Float(required=True, default=1.0)
     diem = Date(default='TODAY', required=True)
     description = String(fulltextindexed=True, maxsize=256)
 
 
 class Resourcetype(EntityType):
@@ -32,27 +30,32 @@
     rtype = SubjectRelation('Resourcetype', cardinality='1*')
     use_calendar = SubjectRelation('Calendaruse', cardinality='+?', composite='subject')
     euser = SubjectRelation('CWUser', cardinality='??')
 
 
 class done_by(RelationDefinition):
     """activity performed by a Resource"""
-    __permissions__ = {'read' : ('managers', 'users'),
-                       'delete' : ('managers', RRQLExpression('S in_state ST, ST name "pending", O euser U')),
-                       'add' : ('managers', RRQLExpression('O euser U'),),
+    __permissions__ = {'read': ('managers', 'users'),
+                       'delete': ('managers', RRQLExpression('S in_state ST, ST name "pending", O euser U')),
+                       'add': ('managers', RRQLExpression('O euser U'),),
                        }
     subject = 'Activity'
     object = 'Resource'
     cardinality = '1*'
     constraints = [RQLVocabularyConstraint('O euser OU?, OU in_state ST, NOT ST name "deactivated"')]
 
+
 class done_for(RelationDefinition):
     subject = 'Activity'
     object = 'WorkOrder'
     cardinality = '1*'
 
 
 class todo_by(RelationDefinition):
+    __permissions__ = {'read': ('managers', 'users'),
+                       'delete': ('managers', RRQLExpression('S owned_by U')),
+                       'add': ('managers', RRQLExpression('S owned_by U')),
+                       }
     subject = 'WorkOrder'
     object = 'Resource'
     cardinality = '+*'
     constraints = [RQLVocabularyConstraint('O euser OU?, OU in_state ST, NOT ST name "deactivated"')]
```

### Comparing `cubicweb-timesheet-0.9.1/hooks.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 """
 
 __docformat__ = "restructuredtext en"
 
 from cubicweb.predicates import is_instance
 from cubicweb.server import hook
 
-from cubes.workorder.hooks import UpdateProgressOp
+from cubicweb_workorder.hooks import UpdateProgressOp
 
 
 class UpdateProgressOnActivityModification(hook.Hook):
     __regid__ = 'timesheet.progress.activity'
     __select__ = hook.Hook.__select__ & is_instance('Activity')
     events = ('after_update_entity', )
 
     def __call__(self):
         if 'duration' in self.entity.cw_edited:
             for workorder in self.entity.done_for:
                 UpdateProgressOp.get_instance(self._cw).add_data(
-                    (workorder.eid, True) )
+                    (workorder.eid, True))
 
 
 class UpdateProgressOnDoneForChange(hook.Hook):
     __regid__ = 'timesheet_update_done_for'
     __select__ = (hook.Hook.__select__
                   & hook.match_rtype('done_for', toetypes=('WorkOrder',)))
     events = ('after_add_relation', 'after_delete_relation',)
```

### Comparing `cubicweb-timesheet-0.9.1/entities.py` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from datetime import timedelta
 
 from logilab.common.date import date_range, todate
 
 from cubicweb.entities import AnyEntity, fetch_config
-from cubicweb.view import EntityAdapter
+from cubicweb_web.view import EntityAdapter
 from cubicweb.predicates import is_instance, score_entity
 
-from cubes.workorder import entities as workorder
-from cubes.calendar.entities import intersect
+from cubicweb_workorder import entities as workorder
+from cubicweb_calendar.entities import intersect
 
 
 class Activity(AnyEntity):
     __regid__ = 'Activity'
     fetch_attrs, cw_fetch_order = fetch_config(['diem', 'done_for', 'duration'])
 
     @property
@@ -25,15 +25,15 @@
         else:
             login = u''
         try:
             return u'%s %s %s %s [%s]' % (
                 self._cw.format_date(self.diem), login, duration,
                 self.workorder.dc_title(),
                 self.cw_adapt_to('IWorkflowable').printable_state)
-        except:
+        except Exception:
             # remote sources unavailable or no related wp
             return u'%s %s %s [%s]' % (
                 self._cw.format_date(self.diem), login, duration,
                 self.cw_adapt_to('IWorkflowable').printable_state)
 
     def dc_long_title(self):
         return u'%s %s' % (self.dc_title(), self.description)
@@ -41,27 +41,28 @@
     @property
     def workorder(self):
         return self.done_for[0]
 
 
 class IResource(EntityAdapter):
     __regid__ = 'timesheet.IResource'
-    __select__ = is_instance('CWUser') and score_entity(lambda x:x.reverse_euser)
+    __select__ = is_instance('CWUser') and score_entity(lambda x: x.reverse_euser)
 
     @property
     def resource(self):
         return self.entity.reverse_euser[0]
 
 
 AWHERE = ('WHERE A is Activity, A diem DI, A duration DU, A description DE, '
           'A done_by R, A in_state S, A done_for WO, O split_into WO, ')
 ADETAILS = 'Any A, DI, R, DU, WO, DE, S ORDERBY DI,R ' + AWHERE
 A_BY_R = 'Any R, S, SUM(DU), MIN(DI), MAX(DI) GROUPBY R,S ORDERBY S ' + AWHERE
 A_BY_W = 'Any WO, S, SUM(DU), MIN(DI), MAX(DI) GROUPBY WO, S ORDERBY S ' + AWHERE
 
+
 class Resource(AnyEntity):
     __regid__ = 'Resource'
     rest_attr = 'title'
     fetch_attrs, cw_fetch_order = fetch_config(('title',))
 
     rql_activities = ADETAILS+'R eid %(eid)s'
     rql_activities_groupby_workorder = A_BY_W + 'R eid %(eid)s'
@@ -96,26 +97,25 @@
         cuses = []
         for cuse in self.use_calendar:
             cstart = cuse.start or start
             cstart = todate(cstart)
             cstop = cuse.stop or stop
             cstop = todate(cstop)
             if intersect((start, stop), (cstart, cstop)):
-                cuses.append( (cstart, cstop, cuse) )
+                cuses.append((cstart, cstop, cuse))
         for date in date_range(start, stop + timedelta(days=1)):
             for cstart, cstop, cuse in cuses:
                 if cstart <= date <= cstop:
                     _, dtype, dstate = cuse.calendar.get_days_type(date, date)[0]
                     day_types[date] = (dtype, dstate)
                     break
         return day_types
 
     def activities_summary(self, firstday, lastday):
         activities = {}
-        workcases = {}
         rset = self._cw.execute("Any A,DI,DU,ST,S,W,WO,WR WHERE A is Activity, "
                                 "  A in_state ST, ST name S, "
                                 "  A diem <= %(l)s, A diem >= %(f)s, "
                                 "  A diem DI, A duration DU, "
                                 "  A done_by R, R eid %(r)s, "
                                 "  A done_for WO, W split_into WO, W title WR",
                                 {'r': self.eid, 'f': firstday, 'l': lastday})
@@ -145,15 +145,15 @@
                 expected = 0.
             else:
                 expected = working_dtype[dtype_eid].expected_worktime
             yield date_, dtstate, expected, day_report
 
     def missing_for(self, day):
         """return missing activity declaration for `day`"""
-        _, _, expected, day_report = self.iter_activities(day, day).next()
+        _, _, expected, day_report = next(self.iter_activities(day, day))
         declared = sum(a.duration for a in day_report)
         missing = expected - declared
         if abs(missing) > 1e-3:
             return missing
         return 0.
 
 
@@ -174,33 +174,36 @@
     # XXX deprecate this in favor of IMileStoneAdapter.contractors()
     def contractors(self):
         return self.todo_by
 
     def update_progress(self, compute=True):
         if compute:
             done = sum(activity.duration for activity in self.reverse_done_for)
-            self.set_attributes(progress_done=done,
-                                progress_todo=max(0, self.budget - done))
+            self.cw_set(progress_done=done,
+                        progress_todo=max(0, self.budget - done))
         super(WorkOrder, self).update_progress(compute)
 
     # number of columns to display
     activities_rql_nb_displayed_cols = 10
+
     def activities_rql(self, limit=None):
         return ADETAILS+'WO eid %(eid)s'
 
+
 class TimesheetWorkOrderIMileStoneAdapter(workorder.WorkOrderIMileStoneAdapter):
 
     def contractors(self):
         return self.entity.todo_by
 
 
 class TimesheetOrderIMileStoneAdapter(workorder.OrderIMileStoneAdapter):
 
     def contractors(self):
         return list(set(x for worder in self.entity.split_into for x in worder.todo_by))
 
 
 def registration_callback(vreg):
-    vreg.register_all(globals().values(), __name__, [TimesheetOrderIMileStoneAdapter, TimesheetWorkOrderIMileStoneAdapter])
+    vreg.register_all(globals().values(),
+                      __name__,
+                      [TimesheetOrderIMileStoneAdapter, TimesheetWorkOrderIMileStoneAdapter])
     vreg.register_and_replace(TimesheetWorkOrderIMileStoneAdapter, workorder.WorkOrderIMileStoneAdapter)
     vreg.register_and_replace(TimesheetOrderIMileStoneAdapter, workorder.OrderIMileStoneAdapter)
-
```

### Comparing `cubicweb-timesheet-0.9.1/i18n/en.po` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/i18n/en.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # erudi-activity-report i18n catalog
-# Copyright 2003-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# Copyright 2003-2014 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # Logilab <contact@logilab.fr>
 msgid ""
 msgstr ""
 "Project-Id-Version: erudi-activity-report 0.1.0\n"
 "PO-Revision-Date: 2008-02-15 11:33+0100\n"
 "Last-Translator: Logilab Team <contact@logilab.fr>\n"
 "Language-Team: en <contact@logilab.fr>\n"
@@ -84,17 +84,14 @@
 
 msgid "activity-current"
 msgstr "current"
 
 msgid "activity-details"
 msgstr "details"
 
-msgid "activity-graph"
-msgstr "graph"
-
 msgid "activity-overview"
 msgstr "overview"
 
 msgid "activitytable"
 msgstr "activity table"
 
 msgid "add Resource euser CWUser object"
```

### Comparing `cubicweb-timesheet-0.9.1/i18n/es.po` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/i18n/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -86,17 +86,14 @@
 
 msgid "activity-current"
 msgstr ""
 
 msgid "activity-details"
 msgstr ""
 
-msgid "activity-graph"
-msgstr ""
-
 msgid "activity-overview"
 msgstr ""
 
 msgid "activitytable"
 msgstr ""
 
 msgid "add Resource euser CWUser object"
```

### Comparing `cubicweb-timesheet-0.9.1/i18n/fr.po` & `cubicweb-timesheet-1.0.0/cubicweb_timesheet/i18n/fr.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # erudi-activity-report i18n catalog
-# Copyright 2003-2013 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# Copyright 2003-2014 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # Logilab <contact@logilab.fr>
 msgid ""
 msgstr ""
 "Project-Id-Version: erudi-intranet 0.1.0\n"
 "PO-Revision-Date: 2008-07-21 09:07+0200\n"
 "Last-Translator: Logilab Team <contact@logilab.fr>\n"
 "Language-Team: fr <contact@logilab.fr>\n"
@@ -87,17 +87,14 @@
 
 msgid "activity-current"
 msgstr "activités récentes"
 
 msgid "activity-details"
 msgstr "détail des activités"
 
-msgid "activity-graph"
-msgstr "graphe des activités"
-
 msgid "activity-overview"
 msgstr "résumé des activités"
 
 msgid "activitytable"
 msgstr "table d'activités"
 
 msgid "add Resource euser CWUser object"
```

