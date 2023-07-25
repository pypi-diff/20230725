# Comparing `tmp/microlearn_gen_course-0.0.3.tar.gz` & `tmp/microlearn_gen_course-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microlearn_gen_course-0.0.3.tar", last modified: Mon Jul 24 07:09:04 2023, max compression
+gzip compressed data, was "microlearn_gen_course-0.0.4.tar", last modified: Tue Jul 25 07:14:29 2023, max compression
```

## Comparing `microlearn_gen_course-0.0.3.tar` & `microlearn_gen_course-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:04.207457 microlearn_gen_course-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:04.199457 microlearn_gen_course-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:04.203457 microlearn_gen_course-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 07:09:04.207457 microlearn_gen_course-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-24 07:09:04.207457 microlearn_gen_course-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:04.199457 microlearn_gen_course-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:04.203457 microlearn_gen_course-0.0.3/src/gen_course/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/gen_course/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/gen_course/gen_answer_to_article_ques.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/gen_course/gen_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/gen_course/gen_course_article_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/gen_course/gen_course_articles_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/gen_course/gen_course_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:04.203457 microlearn_gen_course-0.0.3/src/microlearn_gen_course.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 07:09:04.000000 microlearn_gen_course-0.0.3/src/microlearn_gen_course.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-24 07:09:04.000000 microlearn_gen_course-0.0.3/src/microlearn_gen_course.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:09:04.000000 microlearn_gen_course-0.0.3/src/microlearn_gen_course.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-24 07:09:04.000000 microlearn_gen_course-0.0.3/src/microlearn_gen_course.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 07:09:04.000000 microlearn_gen_course-0.0.3/src/microlearn_gen_course.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:09:04.207457 microlearn_gen_course-0.0.3/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/tests/test_answer_to_article_ques.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/tests/test_gen_course_article_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/tests/test_gen_course_articles_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-24 07:08:52.000000 microlearn_gen_course-0.0.3/src/tests/test_gen_course_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/src/gen_course/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_answer_to_article_ques.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_course_article_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_course_articles_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_course_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/tests/test_answer_to_article_ques.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/tests/test_gen_course_article_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/tests/test_gen_course_articles_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/tests/test_gen_course_metadata.py
```

### Comparing `microlearn_gen_course-0.0.3/.github/workflows/publish.yml` & `microlearn_gen_course-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/PKG-INFO` & `microlearn_gen_course-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn_gen_course
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for generating microlearn course content
 Home-page: https://github.com/AIprojectflow/gen_course
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/gen_course/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/gen_course/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `microlearn_gen_course-0.0.3/setup.cfg` & `microlearn_gen_course-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/src/gen_course/gen_answer_to_article_ques.py` & `microlearn_gen_course-0.0.4/src/gen_course/gen_answer_to_article_ques.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/src/gen_course/gen_base.py` & `microlearn_gen_course-0.0.4/src/gen_course/gen_base.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/src/gen_course/gen_course_article_content.py` & `microlearn_gen_course-0.0.4/src/gen_course/gen_course_article_content.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/src/gen_course/gen_course_articles_titles.py` & `microlearn_gen_course-0.0.4/src/gen_course/gen_course_articles_titles.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/src/gen_course/gen_course_metadata.py` & `microlearn_gen_course-0.0.4/src/gen_course/gen_course_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class GenCourseMetadata(GenBase):
     """
     Generator class for course metadata(title, description, etc.) using the description as text.
     """
     SYSTEM_PROMPT = """Act like a copywriter expert in course editing"""
-    HUMAN_PROMPT = """Write a title of only 3 words and an introduction article to a course of maximum 40 words based on the following:
+    HUMAN_PROMPT = """Write a title of only 3 words and an introduction article to a course of aproximately 40 words based on the following:
 ---
 Description: {course_description}
 ---
 """
 
     def __init__(self, llm, verbose: bool = False):
         super().__init__(llm, verbose)
```

### Comparing `microlearn_gen_course-0.0.3/src/microlearn_gen_course.egg-info/PKG-INFO` & `microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn-gen-course
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for generating microlearn course content
 Home-page: https://github.com/AIprojectflow/gen_course
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/gen_course/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/gen_course/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `microlearn_gen_course-0.0.3/src/microlearn_gen_course.egg-info/SOURCES.txt` & `microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/src/tests/test_answer_to_article_ques.py` & `microlearn_gen_course-0.0.4/src/tests/test_answer_to_article_ques.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/src/tests/test_gen_course_article_content.py` & `microlearn_gen_course-0.0.4/src/tests/test_gen_course_article_content.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/src/tests/test_gen_course_articles_titles.py` & `microlearn_gen_course-0.0.4/src/tests/test_gen_course_articles_titles.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.3/src/tests/test_gen_course_metadata.py` & `microlearn_gen_course-0.0.4/src/tests/test_gen_course_metadata.py`

 * *Files identical despite different names*

