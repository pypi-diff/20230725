# Comparing `tmp/cubicweb-skillmat-0.9.1.tar.gz` & `tmp/cubicweb-skillmat-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubicweb-skillmat-0.9.1.tar", last modified: Mon Dec 19 12:44:32 2016, max compression
+gzip compressed data, was "cubicweb-skillmat-1.0.0.tar", last modified: Tue Jul 25 10:09:06 2023, max compression
```

## Comparing `cubicweb-skillmat-0.9.1.tar` & `cubicweb-skillmat-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,52 @@
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/
--rw-r--r--   0 narval     (111) narval     (116)     1902 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/schema.py
--rw-r--r--   0 narval     (111) narval     (116)      540 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/sobjects.py
--rw-r--r--   0 narval     (111) narval     (116)      381 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/MANIFEST.in
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/cubicweb_skillmat.egg-info/
--rw-rw-r--   0 narval     (111) narval     (116)        1 2016-12-19 12:44:29.000000 cubicweb-skillmat-0.9.1/cubicweb_skillmat.egg-info/top_level.txt
--rw-rw-r--   0 narval     (111) narval     (116)      552 2016-12-19 12:44:30.000000 cubicweb-skillmat-0.9.1/cubicweb_skillmat.egg-info/SOURCES.txt
--rw-rw-r--   0 narval     (111) narval     (116)        1 2016-12-19 12:44:29.000000 cubicweb-skillmat-0.9.1/cubicweb_skillmat.egg-info/dependency_links.txt
--rw-rw-r--   0 narval     (111) narval     (116)      376 2016-12-19 12:44:29.000000 cubicweb-skillmat-0.9.1/cubicweb_skillmat.egg-info/PKG-INFO
--rw-rw-r--   0 narval     (111) narval     (116)       52 2016-12-19 12:44:29.000000 cubicweb-skillmat-0.9.1/cubicweb_skillmat.egg-info/requires.txt
--rw-rw-r--   0 narval     (111) narval     (116)       59 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/setup.cfg
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/wdoc/
--rw-r--r--   0 narval     (111) narval     (116)      443 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/wdoc/ChangeLog_en
--rw-r--r--   0 narval     (111) narval     (116)      544 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/wdoc/ChangeLog_fr
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/views/
--rw-r--r--   0 narval     (111) narval     (116)     4726 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/views/matrix.py
--rw-r--r--   0 narval     (111) narval     (116)     2213 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/views/boxes.py
--rw-r--r--   0 narval     (111) narval     (116)      892 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/views/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)     1700 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/views/sections.py
--rw-r--r--   0 narval     (111) narval     (116)     3436 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/views/primaries.py
--rw-r--r--   0 narval     (111) narval     (116)       84 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/README
--rw-r--r--   0 narval     (111) narval     (116)     1658 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/__pkginfo__.py
--rw-rw-r--   0 narval     (111) narval     (116)      376 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/PKG-INFO
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/test/
--rw-r--r--   0 narval     (111) narval     (116)      359 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/test/test_skillmat.py
--rw-r--r--   0 narval     (111) narval     (116)       24 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/__init__.py
--rw-r--r--   0 narval     (111) narval     (116)     5478 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/setup.py
--rw-r--r--   0 narval     (111) narval     (116)     1722 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/entities.py
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/i18n/
--rw-r--r--   0 narval     (111) narval     (116)     6777 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/i18n/fr.po
--rw-r--r--   0 narval     (111) narval     (116)     5140 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/i18n/en.po
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/data/
--rw-r--r--   0 narval     (111) narval     (116)      850 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/data/cubes.skillmat.css
-drwxrwxr-x   0 narval     (111) narval     (116)        0 2016-12-19 12:44:32.000000 cubicweb-skillmat-0.9.1/migration/
--rw-r--r--   0 narval     (111) narval     (116)       65 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/migration/postcreate.py
--rw-r--r--   0 narval     (111) narval     (116)      108 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/migration/0.2.0_Any.py
--rw-r--r--   0 narval     (111) narval     (116)      282 2016-12-19 12:39:21.000000 cubicweb-skillmat-0.9.1/migration/0.3.0_Any.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.603870 cubicweb-skillmat-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      496 2023-07-25 10:09:06.599870 cubicweb-skillmat-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.591870 cubicweb-skillmat-1.0.0/cubicweb_skillmat/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.591870 cubicweb-skillmat-1.0.0/cubicweb_skillmat/data/
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/data/cubes.skillmat.css
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.595870 cubicweb-skillmat-1.0.0/cubicweb_skillmat/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)     6284 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.595870 cubicweb-skillmat-1.0.0/cubicweb_skillmat/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/migration/0.2.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      282 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/migration/0.3.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1853 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/sobjects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.595870 cubicweb-skillmat-1.0.0/cubicweb_skillmat/views/
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2202 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     5909 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/views/matrix.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/views/primaries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.595870 cubicweb-skillmat-1.0.0/cubicweb_skillmat/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      443 2023-07-25 10:08:46.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/wdoc/ChangeLog_en
+-rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat/wdoc/ChangeLog_fr
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.591870 cubicweb-skillmat-1.0.0/cubicweb_skillmat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      496 2023-07-25 10:09:06.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-07-25 10:09:06.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:09:06.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-25 10:09:06.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:09:06.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-25 10:09:06.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 10:09:06.000000 cubicweb-skillmat-1.0.0/cubicweb_skillmat.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.599870 cubicweb-skillmat-1.0.0/debian/
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/debian/changelog
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/debian/compat
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/debian/control
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/debian/copyright
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/debian/cubicweb-skillmat.prerm
+-rwxrwxrwx   0 root         (0) root         (0)       46 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/debian/rules
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/dev-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 10:09:06.603870 cubicweb-skillmat-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2633 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.599870 cubicweb-skillmat-1.0.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:09:06.599870 cubicweb-skillmat-1.0.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/test/test_skillmat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/test/unittest_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     1785 2023-07-25 10:08:47.000000 cubicweb-skillmat-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cubicweb-skillmat-0.9.1/schema.py` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from yams.buildobjs import (EntityType, SubjectRelation, RelationDefinition,
                             String, Datetime, Int)
 from yams.constraints import IntervalBoundConstraint
 
-from cubicweb.schemas.base import CWUser
 from cubicweb.schema import ERQLExpression
 
-from cubes.folder.schema import Folder
+from cubicweb_folder.schema import Folder
 
-_ = unicode
+from cubicweb import _
 
 
-class Masters(EntityType): # XXX find a suitable name
+class Masters(EntityType):  # XXX find a suitable name
     """relation promoted to EntityType to store the `rate` attribute
     """
     __permissions__ = {'read': ('managers', 'users'),
                        'add': ('managers', ERQLExpression('X foruser U')),
                        'update': ('managers', 'owners'),
                        'delete': ('managers',),
                        }
@@ -26,30 +25,33 @@
 class Technology(Folder):
     pass
 
 
 class Talk(EntityType):
     """relation promoted to EntityType to store the `subject' attribute
     """
-    subject        = String(required=True, fulltextindexed=True, indexed=True, maxsize=32)
-    description    = String(fulltextindexed=True,
-                            description=_('more detailed subject description'))
-    talktime       = Datetime(description=_('estimated presentation date'))
-    presented_by   = SubjectRelation('CWUser', cardinality='?*')
-    attended_by    = SubjectRelation('CWUser', cardinality='**')
-    talks_about    = SubjectRelation(('Technology','Folder'), cardinality='+*')
+    subject = String(required=True, fulltextindexed=True, indexed=True, maxsize=32)
+    description = String(fulltextindexed=True,
+                         description=_('more detailed subject description'))
+    talktime = Datetime(description=_('estimated presentation date'))
+    presented_by = SubjectRelation('CWUser', cardinality='?*')
+    attended_by = SubjectRelation('CWUser', cardinality='**')
+    talks_about = SubjectRelation(('Technology', 'Folder'), cardinality='+*')
 
 
 class comments(RelationDefinition):
     subject = 'Comment'
     object = 'Talk'
     cardinality = '1*'
     composite = 'object'
 
 # extend CWUser
+
+
 class wishes_to_learn(RelationDefinition):
     subject = 'CWUser'
     object = ('Technology', 'Folder')
 
+
 class interested_in(RelationDefinition):
     subject = 'CWUser'
     object = 'Talk'
```

### Comparing `cubicweb-skillmat-0.9.1/sobjects.py` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/sobjects.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,7 @@
     __regid__ = 'skillmat_set_owner_when_set_foruser'
     __select__ = Hook.__select__ & match_rtype('foruser')
     events = ('after_add_relation',)
 
     def __call__(self):
         self._cw.execute('SET M owned_by U WHERE M eid %(m)s, U eid %(u)s, NOT M owned_by U',
                          {'m': self.eidfrom, 'u': self.eidto})
-
```

### Comparing `cubicweb-skillmat-0.9.1/wdoc/ChangeLog_fr` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/wdoc/ChangeLog_fr`

 * *Files identical despite different names*

### Comparing `cubicweb-skillmat-0.9.1/views/boxes.py` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/views/boxes.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 :organization: Logilab
 :copyright: 2003-2010 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
-from cubicweb.selectors import is_instance, match_user_groups
-from cubicweb.web import component
+from cubicweb.predicates import is_instance, match_user_groups
+from cubicweb_web import component
 
 
 class EditWishesBox(component.EditRelationCtxComponent):
     __regid__ = 'edit-wishes'
     __select__ = (component.EditRelationCtxComponent.__select__
                   & is_instance('CWUser') & match_user_groups('owners'))
 
@@ -35,24 +35,22 @@
 class EditAttendedByBox(component.EditRelationCtxComponent):
     __regid__ = 'edit-attended-by'
     __select__ = component.EditRelationCtxComponent.__select__ & is_instance('Talk')
 
     rtype = 'attended_by'
     target = 'object'
 
-    ## Todo : replace + et - in this box by a comprehensive label
+    # Todo : replace + et - in this box by a comprehensive label
 
-  #   def w_related(self, box, entity):
-#         """appends existing relations to the `box`"""
-#         rql = 'DELETE S %s O WHERE S eid %%(s)s, O eid %%(o)s' % self.rtype
-#         related = self.related_entities(entity)
-#         for etarget in related:
-#             box.append(self.box_item(entity, etarget, rql, u'assiste'))
-#         return len(related)
-    
-#     def w_unrelated(self, box, entity):
-#         """appends unrelated entities to the `box`"""
-#         rql = 'SET S %s O WHERE S eid %%(s)s, O eid %%(o)s' % self.rtype
-#         for etarget in self.unrelated_entities(entity):
-#             box.append(self.box_item(entity, etarget, rql, u'n\'assite pas'))
-  
-   
+    # def w_related(self, box, entity):
+    #     """appends existing relations to the `box`"""
+    #     rql = 'DELETE S %s O WHERE S eid %%(s)s, O eid %%(o)s' % self.rtype
+    #     related = self.related_entities(entity)
+    #     for etarget in related:
+    #         box.append(self.box_item(entity, etarget, rql, u'assiste'))
+    #     return len(related)
+
+    # def w_unrelated(self, box, entity):
+    #     """appends unrelated entities to the `box`"""
+    #     rql = 'SET S %s O WHERE S eid %%(s)s, O eid %%(o)s' % self.rtype
+    #     for etarget in self.unrelated_entities(entity):
+    #         box.append(self.box_item(entity, etarget, rql, u'n\'assite pas'))
```

### Comparing `cubicweb-skillmat-0.9.1/views/__init__.py` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/views/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """template-specific forms/views/actions/components"""
-from cubicweb.view import EntityAdapter
-from cubicweb.selectors import is_instance
-from cubicweb.web import uicfg
-from cubicweb.web.formfields import IntField
+import six
+from cubicweb_web.view import EntityAdapter
+from cubicweb.predicates import is_instance
+from cubicweb_web.views import uicfg
 
-from cubes.skillmat.entities import SKILLS
+from cubicweb_skillmat.entities import SKILLS
 
-RATEVOCAB = [(l, unicode(v)) for v, l in sorted(SKILLS.items())]
+RATEVOCAB = [(l, six.text_type(v)) for v, l in sorted(SKILLS.items())]
 uicfg.autoform_field_kwargs.tag_attribute(
     ('Masters', 'rate'),
     {'choices': RATEVOCAB,
      'internationalizable': True})
 
 uicfg.autoform_section.tag_subject_of(('Talk', 'attended_by', '*'), 'main', 'attributes')
 uicfg.autoform_section.tag_subject_of(('Talk', 'attended_by', '*'), 'muledit', 'attributes')
```

### Comparing `cubicweb-skillmat-0.9.1/views/primaries.py` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/views/primaries.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,41 +4,40 @@
 :copyright: 2003-2010 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
 from logilab.mtconverter import xml_escape
 
-from cubicweb.selectors import is_instance
-from cubicweb.view import EntityView
-from cubicweb.web import uicfg
-from cubicweb.web.views import primary
+from cubicweb.predicates import is_instance
+from cubicweb_web.views import primary
+
+from cubicweb_folder.views import FolderPrimaryView
 
-from cubes.folder.views import FolderPrimaryView
 
 class SkillPrimaryView(FolderPrimaryView):
 
     def cell_call(self, row, col):
         super(SkillPrimaryView, self).cell_call(row, col)
         skill = self.cw_rset.get_entity(row, col)
         rql = ('Any U,L,R ORDERBY L WITH U,L,R BEING ( '
                # get username and skill for those who specified it
                '   (Any U,L,R WHERE U login L, M foruser U, M rate R, '
                '    M skill S, S eid %(s)s) '
-               ' UNION ' # union users for who the skill is unknown
+               ' UNION '  # union users for who the skill is unknown
                '   (Any U,L,-1 WHERE U login L, U is CWUser, '
                '    NOT EXISTS(M skill S, S eid %(s)s, M foruser U))  )')
         rset = self._cw.execute(rql, {'s': skill.eid})
         if not rset:
             self.warning('no skill information found for %s', skill.dc_title())
             return
         self._cw.add_css('cubes.skillmat.css')
         self.w(u'<table class="matrix">')
         self.w(u'<tr>')
-        for row in xrange(len(rset)):
+        for row in range(len(rset)):
             self.w(u'<th>%s</th>' % self._cw.view('oneline', rset, row=row, col=0))
         self.w(u'</tr>\n<tr>')
         width = 100 / len(rset)
         for ueid, _, rate in rset:
             if rate == -1:
                 linkto = ('foruser:%s:subject' % ueid,
                           'skill:%s:subject' % skill.eid)
@@ -58,18 +57,14 @@
 
 
 class TalkPrimaryView(primary.PrimaryView):
     __select__ = is_instance('Talk',)
 
     def render_entity_title(self, entity):
         self.w(u'<h1>%s</h1>' % xml_escape(entity.dc_title()))
-        nc = self._cw.vreg['components'].select_or_none('interesting', self._cw,
-                                                        rset=self.cw_rset)
-        if nc:
-            nc.render(w=self.w)
 
     def render_entity_relations(self, entity):
         if entity.related('interested_in', 'object'):
             self.w(self._cw._('interested people :'))
             self.wview('list', entity.related('interested_in', 'object'), 'null')
         if entity.related('presented_by'):
             self.w(self._cw._('presented by :'))
```

### Comparing `cubicweb-skillmat-0.9.1/entities.py` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/entities.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,57 +2,61 @@
 
 :organization: Logilab
 :copyright: 2003-2010 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 :contact: http://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 __docformat__ = "restructuredtext en"
 
-from cubicweb.selectors import is_instance
+from cubicweb import _
+from cubicweb.predicates import is_instance
 from cubicweb.entities import AnyEntity, adapters
 
-from cubes.folder.entities import Folder
+from cubicweb_folder.entities import Folder
+
 
 class Masters(AnyEntity):
     __regid__ = 'Masters'
     fetch_attrs = ('rate', 'foruser', 'skill')
 
     def dc_title(self):
         return u'%s: %s' % (self.skill[0].name, self.rate)
 
     def dc_long_title(self):
         return u'%s / %s' % (self.foruser[0].dc_title(), self.dc_title())
 
+
 class Technology(AnyEntity):
     __regid__ = 'Technology'
     fetch_attrs = ('name',)
 
     def skill_categories(self):
         # XXX what if we have a skill tree with depth > 1
         return self.filed_under
 
 
-class Skill(Folder): # XXX
+class Skill(Folder):  # XXX
 
     def skill_categories(self):
         return [self]
 
 
 class Talk(AnyEntity):
     __regid__ = 'Talk'
     fetch_attrs = ('subject', 'description', 'talktime')
 
     def dc_title(self):
         return u'%s' % (self.subject)
 
-SKILLS = {0 : _("I don't want to learn this technology"),
-          1 : _('I know nothing about this technology'),
-          2 : _('Just beginning whith this technology'),
-          3 : _('I start on this technology, and I can help'),
-          4 : _('I am doing well, selfworking'),
-          5 : _('I can conduct a training course')}
+
+SKILLS = {0: _("I don't want to learn this technology"),
+          1: _('I know nothing about this technology'),
+          2: _('Just beginning whith this technology'),
+          3: _('I start on this technology, and I can help'),
+          4: _('I am doing well, selfworking'),
+          5: _('I can conduct a training course')}
 
 
 class TechnologyITreeAdapter(adapters.ITreeAdapter):
     __select__ = is_instance('Technology')
     tree_relation = 'filed_under'
 
     def children(self, entities=True, sametype=False):
```

### Comparing `cubicweb-skillmat-0.9.1/i18n/fr.po` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/i18n/fr.po`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 msgid "???"
 msgstr "???"
 
+msgid "export SkillMatrix"
+msgstr "exporter la matrice de compétences"
+
 msgid "I am doing well, selfworking"
 msgstr "Je me débrouille bien, je suis autonome"
 
 msgid "I can conduct a training course"
 msgstr "Je suis capable de faire une formation à ce sujet"
 
 msgid "I don't want to learn this technology"
@@ -90,20 +93,14 @@
 msgid "attended_by_object"
 msgstr "a assisté à"
 
 msgctxt "CWUser"
 msgid "attended_by_object"
 msgstr "a assisté à"
 
-msgid "click here if you are interested by this talk"
-msgstr "Cliquer ici si vous êtes intéressé par cet exposé"
-
-msgid "click here if you are not any more interested by this talk"
-msgstr "Cliquer ici si vous n'êtes plus intéressé par cet exposé"
-
 msgctxt "Talk"
 msgid "comments_object"
 msgstr "commentée par"
 
 msgid "components_interesting"
 msgstr "composant d'enregistrement pour une présentation"
 
@@ -133,17 +130,14 @@
 msgid "description"
 msgstr "description"
 
 msgctxt "Technology"
 msgid "description_format"
 msgstr "format"
 
-msgid "display the box or not"
-msgstr "Afficher la boîte ou non"
-
 msgid "estimated presentation date"
 msgstr "La date estimée"
 
 msgctxt "Technology"
 msgid "filed_under"
 msgstr ""
 
@@ -270,17 +264,14 @@
 msgid "talktime"
 msgstr "date"
 
 msgctxt "Talk"
 msgid "talktime"
 msgstr "date"
 
-msgid "visible"
-msgstr "visible"
-
 msgid "wishes_to_learn"
 msgstr "souhaite apprendre"
 
 msgctxt "CWUser"
 msgid "wishes_to_learn"
 msgstr "souhaite apprendre"
 
@@ -291,18 +282,12 @@
 msgid "wishes_to_learn_object"
 msgstr "souhaite être appris par"
 
 msgctxt "Technology"
 msgid "wishes_to_learn_object"
 msgstr "souhaite être appris par"
 
-msgid "you are not anymore registered for this project"
-msgstr "Vous n'êtes plus enregistré pour cet exposé"
-
-msgid "you are now registered for this talk"
-msgstr "vous êtes enregistré pour cet exposé "
-
 msgid ""
 "you can update your skill information by clicking on the corresponding cell"
 msgstr ""
 "vous pouvez mettre à jour vos niveaux de compétences en cliquant sur la "
 "cellule correspondante"
```

### Comparing `cubicweb-skillmat-0.9.1/i18n/en.po` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/i18n/en.po`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid "???"
 msgstr ""
 
+msgid "export SkillMatrix"
+msgstr ""
+
 msgid "I am doing well, selfworking"
 msgstr ""
 
 msgid "I can conduct a training course"
 msgstr ""
 
 msgid "I don't want to learn this technology"
@@ -88,20 +91,14 @@
 msgid "attended_by_object"
 msgstr "attends"
 
 msgctxt "CWUser"
 msgid "attended_by_object"
 msgstr ""
 
-msgid "click here if you are interested by this talk"
-msgstr ""
-
-msgid "click here if you are not any more interested by this talk"
-msgstr ""
-
 msgctxt "Talk"
 msgid "comments_object"
 msgstr ""
 
 msgid "components_interesting"
 msgstr ""
 
@@ -131,17 +128,14 @@
 msgid "description"
 msgstr ""
 
 msgctxt "Technology"
 msgid "description_format"
 msgstr ""
 
-msgid "display the box or not"
-msgstr ""
-
 msgid "estimated presentation date"
 msgstr ""
 
 msgctxt "Technology"
 msgid "filed_under"
 msgstr ""
 
@@ -267,17 +261,14 @@
 msgid "talktime"
 msgstr ""
 
 msgctxt "Talk"
 msgid "talktime"
 msgstr ""
 
-msgid "visible"
-msgstr ""
-
 msgid "wishes_to_learn"
 msgstr "wishes to learn"
 
 msgctxt "CWUser"
 msgid "wishes_to_learn"
 msgstr ""
 
@@ -288,16 +279,10 @@
 msgid "wishes_to_learn_object"
 msgstr ""
 
 msgctxt "Technology"
 msgid "wishes_to_learn_object"
 msgstr ""
 
-msgid "you are not anymore registered for this project"
-msgstr ""
-
-msgid "you are now registered for this talk"
-msgstr ""
-
 msgid ""
 "you can update your skill information by clicking on the corresponding cell"
 msgstr ""
```

### Comparing `cubicweb-skillmat-0.9.1/data/cubes.skillmat.css` & `cubicweb-skillmat-1.0.0/cubicweb_skillmat/data/cubes.skillmat.css`

 * *Files identical despite different names*

