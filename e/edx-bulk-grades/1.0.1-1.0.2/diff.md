# Comparing `tmp/edx-bulk-grades-1.0.1.tar.gz` & `tmp/edx-bulk-grades-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-bulk-grades-1.0.1.tar", last modified: Wed Dec 21 16:32:51 2022, max compression
+gzip compressed data, was "edx-bulk-grades-1.0.2.tar", last modified: Tue Jul 25 14:16:02 2023, max compression
```

## Comparing `edx-bulk-grades-1.0.1.tar` & `edx-bulk-grades-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:51.650430 edx-bulk-grades-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     4761 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35119 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      169 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10657 2022-12-21 16:32:51.650430 edx-bulk-grades-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5179 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:51.650430 edx-bulk-grades-1.0.1/bulk_grades/
--rw-r--r--   0 runner    (1001) docker     (122)      159 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28888 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      674 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1750 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:51.650430 edx-bulk-grades-1.0.1/bulk_grades/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      506 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/migrations/0002_auto_20190703_1526.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      782 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:51.650430 edx-bulk-grades-1.0.1/bulk_grades/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      267 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      500 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/settings/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:51.646430 edx-bulk-grades-1.0.1/bulk_grades/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:51.650430 edx-bulk-grades-1.0.1/bulk_grades/templates/bulk_grades/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/templates/bulk_grades/base.html
--rw-r--r--   0 runner    (1001) docker     (122)      639 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     7685 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/bulk_grades/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:51.650430 edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10657 2022-12-21 16:32:51.000000 edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      807 2022-12-21 16:32:51.000000 edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-21 16:32:51.000000 edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2022-12-21 16:32:51.000000 edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-21 16:32:51.000000 edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       69 2022-12-21 16:32:51.000000 edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-12-21 16:32:51.000000 edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-21 16:32:51.650430 edx-bulk-grades-1.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      516 2022-12-21 16:32:51.650430 edx-bulk-grades-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2945 2022-12-21 16:32:43.000000 edx-bulk-grades-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 14:16:02.098850 edx-bulk-grades-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     4932 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35119 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    10774 2023-07-25 14:16:02.098850 edx-bulk-grades-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5047 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 14:16:02.094850 edx-bulk-grades-1.0.2/bulk_grades/
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28851 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 14:16:02.098850 edx-bulk-grades-1.0.2/bulk_grades/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/migrations/0002_auto_20190703_1526.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      782 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 14:16:02.098850 edx-bulk-grades-1.0.2/bulk_grades/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      500 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/settings/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 14:16:02.094850 edx-bulk-grades-1.0.2/bulk_grades/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 14:16:02.098850 edx-bulk-grades-1.0.2/bulk_grades/templates/bulk_grades/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/templates/bulk_grades/base.html
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7685 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/bulk_grades/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 14:16:02.098850 edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10774 2023-07-25 14:16:01.000000 edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-07-25 14:16:02.000000 edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 14:16:01.000000 edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-25 14:16:01.000000 edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 14:16:01.000000 edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-07-25 14:16:01.000000 edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-25 14:16:01.000000 edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 14:16:02.098850 edx-bulk-grades-1.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-25 14:16:02.098850 edx-bulk-grades-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3021 2023-07-25 14:15:53.000000 edx-bulk-grades-1.0.2/setup.py
```

### Comparing `edx-bulk-grades-1.0.1/CHANGELOG.rst` & `edx-bulk-grades-1.0.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,23 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 
+
+
+[1.0.2] - 2023-06-14
+~~~~~~~~~~~~~~~~~~~~
+* Support added for Django 4.2.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+
 [1.0.1] - 2022-12-21
 * Fix a bug in building error response messaging.
 
 [1.0.0] - 2022-02-16
 * Dropped Support for Django22, 30 and 31
 * Added Support for Django40
 ~~~~~~~~~~
```

### Comparing `edx-bulk-grades-1.0.1/LICENSE.txt` & `edx-bulk-grades-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/PKG-INFO` & `edx-bulk-grades-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: edx-bulk-grades
-Version: 1.0.1
+Version: 1.0.2
 Summary: Support for bulk scoring and grading
 Home-page: https://github.com/openedx/edx-bulk-grades
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
 
@@ -103,18 +105,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
 can find it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-bulk-grades/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-bulk-grades/blob/master/.github/ISSUE_TEMPLATE.md>`_.
 
@@ -168,14 +167,23 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 
+
+
+[1.0.2] - 2023-06-14
+~~~~~~~~~~~~~~~~~~~~
+* Support added for Django 4.2.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+
 [1.0.1] - 2022-12-21
 * Fix a bug in building error response messaging.
 
 [1.0.0] - 2022-02-16
 * Dropped Support for Django22, 30 and 31
 * Added Support for Django40
 ~~~~~~~~~~
```

### Comparing `edx-bulk-grades-1.0.1/README.rst` & `edx-bulk-grades-1.0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -82,18 +82,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
 can find it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-bulk-grades/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-bulk-grades/blob/master/.github/ISSUE_TEMPLATE.md>`_.
```

### Comparing `edx-bulk-grades-1.0.1/bulk_grades/api.py` & `edx-bulk-grades-1.0.2/bulk_grades/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,18 +50,18 @@
     if cohort:
         enrollments = enrollments.filter(
             user__cohortmembership__course_id=course_id,
             user__cohortmembership__course_user_group__name=cohort)
     if active_only:
         enrollments = enrollments.filter(is_active=True)
     if excluded_course_roles:
-        course_access_role_filters = dict(
-            user=OuterRef('user'),
-            course_id=course_id
-        )
+        course_access_role_filters = {
+            "user": OuterRef('user'),
+            "course_id": course_id
+        }
         if 'all' not in excluded_course_roles:
             course_access_role_filters['role__in'] = excluded_course_roles
         enrollments = enrollments.annotate(has_excluded_course_role=Exists(
             apps.get_model('student', 'CourseAccessRole').objects.filter(**course_access_role_filters)
         ))
         enrollments = enrollments.exclude(has_excluded_course_role=True)
 
@@ -379,18 +379,18 @@
                     short_id = key.split('-', 1)[1]
                     subsection = self._subsections[short_id][0]
                     block_id = str(subsection.location)
                     try:
                         new_grade = float(value)
                     except ValueError as error:
                         raise ValidationError(_('Grade must be a number')) from error
-                    else:
-                        if new_grade < 0:
-                            raise ValidationError(_('Grade must not be negative'))
-                        operation['new_override_grades'].append((block_id, new_grade))
+
+                    if new_grade < 0:
+                        raise ValidationError(_('Grade must not be negative'))
+                    operation['new_override_grades'].append((block_id, new_grade))
 
         return operation
 
     def process_row(self, row):
         """
         Save a row to the persistent subsection override table.
         """
@@ -582,15 +582,15 @@
                         or
                         (self.subsection_grade_max and (effective_grade > self.subsection_grade_max))
                 ):
                     continue
             # pylint: disable=E1111
             course_grade = grades_api.CourseGradeFactory().read(enrollment['user'], course_key=self._course_key)
             if self.course_grade_min or self.course_grade_max:
-                course_grade_normalized = (course_grade.percent * 100)
+                course_grade_normalized = course_grade.percent * 100
 
                 if (
                         (self.course_grade_min and (course_grade_normalized < self.course_grade_min))
                         or
                         (self.course_grade_max and (course_grade_normalized > self.course_grade_max))
                 ):
                     continue
```

### Comparing `edx-bulk-grades-1.0.1/bulk_grades/apps.py` & `edx-bulk-grades-1.0.2/bulk_grades/apps.py`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/bulk_grades/clients.py` & `edx-bulk-grades-1.0.2/bulk_grades/clients.py`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/bulk_grades/migrations/0001_initial.py` & `edx-bulk-grades-1.0.2/bulk_grades/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/bulk_grades/models.py` & `edx-bulk-grades-1.0.2/bulk_grades/models.py`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/bulk_grades/templates/bulk_grades/base.html` & `edx-bulk-grades-1.0.2/bulk_grades/templates/bulk_grades/base.html`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/bulk_grades/urls.py` & `edx-bulk-grades-1.0.2/bulk_grades/urls.py`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/bulk_grades/views.py` & `edx-bulk-grades-1.0.2/bulk_grades/views.py`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/PKG-INFO` & `edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: edx-bulk-grades
-Version: 1.0.1
+Version: 1.0.2
 Summary: Support for bulk scoring and grading
 Home-page: https://github.com/openedx/edx-bulk-grades
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
 
@@ -103,18 +105,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 The pull request description template should be automatically applied if you are creating a pull request from GitHub. Otherwise you
 can find it at `PULL_REQUEST_TEMPLATE.md <https://github.com/openedx/edx-bulk-grades/blob/master/.github/PULL_REQUEST_TEMPLATE.md>`_.
 
 The issue report template should be automatically applied if you are creating an issue on GitHub as well. Otherwise you
 can find it at `ISSUE_TEMPLATE.md <https://github.com/openedx/edx-bulk-grades/blob/master/.github/ISSUE_TEMPLATE.md>`_.
 
@@ -168,14 +167,23 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 
+
+
+[1.0.2] - 2023-06-14
+~~~~~~~~~~~~~~~~~~~~
+* Support added for Django 4.2.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
+
+
 [1.0.1] - 2022-12-21
 * Fix a bug in building error response messaging.
 
 [1.0.0] - 2022-02-16
 * Dropped Support for Django22, 30 and 31
 * Added Support for Django40
 ~~~~~~~~~~
```

### Comparing `edx-bulk-grades-1.0.1/edx_bulk_grades.egg-info/SOURCES.txt` & `edx-bulk-grades-1.0.2/edx_bulk_grades.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/setup.cfg` & `edx-bulk-grades-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `edx-bulk-grades-1.0.1/setup.py` & `edx-bulk-grades-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,16 @@
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
     entry_points={
```

