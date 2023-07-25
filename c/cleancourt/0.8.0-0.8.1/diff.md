# Comparing `tmp/cleancourt-0.8.0.tar.gz` & `tmp/cleancourt-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cleancourt-0.8.0.tar", last modified: Tue Jul 25 17:46:35 2023, max compression
+gzip compressed data, was "dist/cleancourt-0.8.1.tar", last modified: Tue Jul 25 20:22:05 2023, max compression
```

## Comparing `cleancourt-0.8.0.tar` & `cleancourt-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:46:35.000000 cleancourt-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-07-25 17:46:20.000000 cleancourt-0.8.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    15858 2023-07-25 17:46:35.000000 cleancourt-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13776 2023-07-25 17:46:20.000000 cleancourt-0.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-25 17:46:35.000000 cleancourt-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-07-25 17:46:20.000000 cleancourt-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/check_spaces.py
--rw-rw-rw-   0 root         (0) root         (0)     4004 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/clean_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4234 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/compare_companies.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/compute_ngrams.py
--rw-rw-rw-   0 root         (0) root         (0)     9428 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/cosine_similarity.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/filter_types.py
--rw-rw-rw-   0 root         (0) root         (0)     6232 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/full_clean_names.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/integrate_output.py
--rw-rw-rw-   0 root         (0) root         (0)     3745 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/parse_names.py
--rw-rw-rw-   0 root         (0) root         (0)     2601 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/separate_parent_company.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15858 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 20:22:05.000000 cleancourt-0.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-07-25 20:21:49.000000 cleancourt-0.8.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    15858 2023-07-25 20:22:05.000000 cleancourt-0.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13776 2023-07-25 20:21:49.000000 cleancourt-0.8.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-25 20:22:05.000000 cleancourt-0.8.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-07-25 20:21:49.000000 cleancourt-0.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 20:22:05.000000 cleancourt-0.8.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 20:22:05.000000 cleancourt-0.8.1/src/cleancourt/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/check_spaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4004 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/clean_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4234 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/compare_companies.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/compute_ngrams.py
+-rw-rw-rw-   0 root         (0) root         (0)     9428 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/cosine_similarity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/filter_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/full_clean_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/integrate_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/parse_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     2601 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/separate_parent_company.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-07-25 20:21:49.000000 cleancourt-0.8.1/src/cleancourt/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 20:22:05.000000 cleancourt-0.8.1/src/cleancourt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15858 2023-07-25 20:22:05.000000 cleancourt-0.8.1/src/cleancourt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-25 20:22:05.000000 cleancourt-0.8.1/src/cleancourt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 20:22:05.000000 cleancourt-0.8.1/src/cleancourt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-25 20:22:05.000000 cleancourt-0.8.1/src/cleancourt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 20:22:05.000000 cleancourt-0.8.1/src/cleancourt.egg-info/top_level.txt
```

### Comparing `cleancourt-0.8.0/LICENSE.txt` & `cleancourt-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/PKG-INFO` & `cleancourt-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.8.0
+Version: 0.8.1
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
```

### Comparing `cleancourt-0.8.0/README.md` & `cleancourt-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/setup.py` & `cleancourt-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="cleancourt",
-    version="0.8.0",
+    version="0.8.1",
     description="a library for cleaning court docket entries",
     author="Logan Pratico",
     author_email="praticol@lsc.gov",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.9",
```

### Comparing `cleancourt-0.8.0/src/cleancourt/__init__.py` & `cleancourt-0.8.1/src/cleancourt/__init__.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt/check_spaces.py` & `cleancourt-0.8.1/src/cleancourt/check_spaces.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt/clean_data.py` & `cleancourt-0.8.1/src/cleancourt/clean_data.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt/compare_companies.py` & `cleancourt-0.8.1/src/cleancourt/compare_companies.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt/cosine_similarity.py` & `cleancourt-0.8.1/src/cleancourt/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt/filter_types.py` & `cleancourt-0.8.1/src/cleancourt/filter_types.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt/full_clean_names.py` & `cleancourt-0.8.1/src/cleancourt/full_clean_names.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt/integrate_output.py` & `cleancourt-0.8.1/src/cleancourt/integrate_output.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt/parse_names.py` & `cleancourt-0.8.1/src/cleancourt/parse_names.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,87 +42,96 @@
 
         else:
             # If no label is specified, use built in filter
             is_person = filter_people(name)
 
         # If is a person, grab name components from parsed names and place in a common format
         if is_person:
-            val = pp.tag(name)
-            try:
-                firstI = val[0]["FirstInitial"]
-            except KeyError:
-                firstI = ""
-
-            try:
-                prefOther = val[0]["PrefixOther"]
-            except KeyError:
-                prefOther = ""
-
+            
+            # 7/25/2023 - added try catch to account for parsing errors in probable people. In these cases just skip parsing.
+            success=False
+            try:
+                val = pp.tag(name)
+                success = True
+            except:
+                names_dict[name] = name
+            
+            if success:
+                try:
+                    firstI = val[0]["FirstInitial"]
+                except KeyError:
+                    firstI = ""
+
+                try:
+                    prefOther = val[0]["PrefixOther"]
+                except KeyError:
+                    prefOther = ""
+
+
+                try: # Update 0.7.8 first names are sometimes parsed as SuffixOther in probablepeople. this attempts to correct for that error
+                    sufOther = val[0]["SuffixOther"]
+                    if sufOther == 'dds' or sufOther == 'md' or sufOther == 'dmd' or sufOther == 'dpn':
+                        sufOtherEnd = sufOther
+                        sufOther = ""
+                    else:
+                        sufOtherEnd = ""
 
-            try: # Update 0.7.8 first names are sometimes parsed as SuffixOther in probablepeople. this attempts to correct for that error
-                sufOther = val[0]["SuffixOther"]
-                if sufOther == 'dds' or sufOther == 'md' or sufOther == 'dmd' or sufOther == 'dpn':
-                    sufOtherEnd = sufOther
+                except KeyError:
                     sufOther = ""
-                else:
                     sufOtherEnd = ""
 
-            except KeyError:
-                sufOther = ""
-                sufOtherEnd = ""
-
-
-            try:
-                first = val[0]["GivenName"]
-            except KeyError:
-                first = ""
-
-            try:
-                middle = val[0]["MiddleName"]
-            except KeyError:
-                middle = ""
-
-            try:
-                middleI = val[0]["MiddleInitial"]
-            except KeyError:
-                middleI = ""
-
-            try:
-                last = val[0]["Surname"]
-            except KeyError:
-                last = ""
-
-            try:
-                lastI = val[0]["LastInitial"]
-            except KeyError:
-                lastI = ""
 
-            try:
-                suffix = val[0]["SuffixGenerational"]
-            except KeyError:
-                suffix = ""
-
-            full_name = ( # Add all of the parsed names together in a standard format
-                firstI
-                + " "
-                + prefOther
-                + " "
-                + first
-                + " "
-                + sufOther
-                + " "
-                + middle
-                + " "
-                + middleI
-                + " "
-                + last
-                + " " 
-                + lastI
-                + " "
-                + suffix
-                + " " 
-                + sufOtherEnd
-            )
+                try:
+                    first = val[0]["GivenName"]
+                except KeyError:
+                    first = ""
+
+                try:
+                    middle = val[0]["MiddleName"]
+                except KeyError:
+                    middle = ""
+
+                try:
+                    middleI = val[0]["MiddleInitial"]
+                except KeyError:
+                    middleI = ""
+
+                try:
+                    last = val[0]["Surname"]
+                except KeyError:
+                    last = ""
+
+                try:
+                    lastI = val[0]["LastInitial"]
+                except KeyError:
+                    lastI = ""
+
+                try:
+                    suffix = val[0]["SuffixGenerational"]
+                except KeyError:
+                    suffix = ""
+
+                full_name = ( # Add all of the parsed names together in a standard format
+                    firstI
+                    + " "
+                    + prefOther
+                    + " "
+                    + first
+                    + " "
+                    + sufOther
+                    + " "
+                    + middle
+                    + " "
+                    + middleI
+                    + " "
+                    + last
+                    + " " 
+                    + lastI
+                    + " "
+                    + suffix
+                    + " " 
+                    + sufOtherEnd
+                )
 
-            names_dict[name] = re.sub(" +", " ", full_name.strip()) # Strip any extra white spaces
+                names_dict[name] = re.sub(" +", " ", full_name.strip()) # Strip any extra white spaces
 
     return names_dict
```

### Comparing `cleancourt-0.8.0/src/cleancourt/separate_parent_company.py` & `cleancourt-0.8.1/src/cleancourt/separate_parent_company.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt/test_utils.py` & `cleancourt-0.8.1/src/cleancourt/test_utils.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.8.0/src/cleancourt.egg-info/PKG-INFO` & `cleancourt-0.8.1/src/cleancourt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.8.0
+Version: 0.8.1
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
```

### Comparing `cleancourt-0.8.0/src/cleancourt.egg-info/SOURCES.txt` & `cleancourt-0.8.1/src/cleancourt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

