# Comparing `tmp/cleancourt-0.7.9.tar.gz` & `tmp/cleancourt-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cleancourt-0.7.9.tar", last modified: Wed Apr 19 17:19:05 2023, max compression
+gzip compressed data, was "dist/cleancourt-0.8.0.tar", last modified: Tue Jul 25 17:46:35 2023, max compression
```

## Comparing `cleancourt-0.7.9.tar` & `cleancourt-0.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:19:05.000000 cleancourt-0.7.9/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-19 17:18:50.000000 cleancourt-0.7.9/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    15468 2023-04-19 17:19:05.000000 cleancourt-0.7.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13414 2023-04-19 17:18:50.000000 cleancourt-0.7.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-19 17:19:05.000000 cleancourt-0.7.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1195 2023-04-19 17:18:50.000000 cleancourt-0.7.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt/
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/check_spaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3351 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/clean_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4124 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/compare_companies.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/compute_ngrams.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/cosine_similarity.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/filter_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5985 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/full_clean_names.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/integrate_output.py
--rw-rw-rw-   0 root         (0) root         (0)     3226 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/parse_names.py
--rw-rw-rw-   0 root         (0) root         (0)     2047 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/separate_parent_company.py
--rw-rw-rw-   0 root         (0) root         (0)      832 2023-04-19 17:18:50.000000 cleancourt-0.7.9/src/cleancourt/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15468 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      623 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-19 17:19:05.000000 cleancourt-0.7.9/src/cleancourt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:46:35.000000 cleancourt-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-07-25 17:46:20.000000 cleancourt-0.8.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    15858 2023-07-25 17:46:35.000000 cleancourt-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13776 2023-07-25 17:46:20.000000 cleancourt-0.8.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-25 17:46:35.000000 cleancourt-0.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1195 2023-07-25 17:46:20.000000 cleancourt-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt/
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/check_spaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     4004 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/clean_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4234 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/compare_companies.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/compute_ngrams.py
+-rw-rw-rw-   0 root         (0) root         (0)     9428 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/cosine_similarity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/filter_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6232 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/full_clean_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/integrate_output.py
+-rw-rw-rw-   0 root         (0) root         (0)     3745 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/parse_names.py
+-rw-rw-rw-   0 root         (0) root         (0)     2601 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/separate_parent_company.py
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-07-25 17:46:20.000000 cleancourt-0.8.0/src/cleancourt/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15858 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-25 17:46:35.000000 cleancourt-0.8.0/src/cleancourt.egg-info/top_level.txt
```

### Comparing `cleancourt-0.7.9/LICENSE.txt` & `cleancourt-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.9/PKG-INFO` & `cleancourt-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.7.9
+Version: 0.8.0
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
@@ -30,23 +30,27 @@
         
         #### full_clean_names
         
         ```python
         cleancourt.full_clean_names(
           messy_name_list,
           separate_management=False,
-          min_similarity_score=.80
+          min_similarity_score=.80,
+          party_type = 'None Specified'
+        
         )
         ```
         The full_clean_names function takes in a list of messy names in the dataset and applies all name cleaning functions to said dataset. The function first cleans the data using pattern matching, then separates the data based on whether a party name refers to an individual or a company. From there, the two datasets are cleaned in isolation using the format_people_names or the link_company_names discussed below. The datasets are then rejoined and linked one more time by removing spaces using the check_spaces function.
         
         The full_clean_names function also takes in an optional boolean parameter to determine whether or not a party name should be separated into two separate lists when a management company is present. When set to True, the party name 'A doing business as B', for example, would be separated into two lists, where B is put in the original column, and A is added to a _managing companies_ column. When set to True, the function will return two lists.
         
         Another optional parameter taken by full_clean_names is the min_similarity_score parameter, which is passed directly to the link_company_names function and used to compute the threshold for similarity among company names.
         
+        As of CC 0.8.0, full_clean_names now takes an optional party_type parameter. You can use this parameter should you wish to skip the labeling of entities as either people or companies. In order to skip this ordering, you must supply a value of either 'person' or 'company' depending on the list type that you are supplying.
+        
         #### compare_companies
         
         ```python
         cleancourt.compare_companies(
         	org_name_messy,
         	org_name_clean,
         	threshold=.25,
```

### Comparing `cleancourt-0.7.9/README.md` & `cleancourt-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,27 @@
 
 #### full_clean_names
 
 ```python
 cleancourt.full_clean_names(
   messy_name_list,
   separate_management=False,
-  min_similarity_score=.80
+  min_similarity_score=.80,
+  party_type = 'None Specified'
+
 )
 ```
 The full_clean_names function takes in a list of messy names in the dataset and applies all name cleaning functions to said dataset. The function first cleans the data using pattern matching, then separates the data based on whether a party name refers to an individual or a company. From there, the two datasets are cleaned in isolation using the format_people_names or the link_company_names discussed below. The datasets are then rejoined and linked one more time by removing spaces using the check_spaces function.
 
 The full_clean_names function also takes in an optional boolean parameter to determine whether or not a party name should be separated into two separate lists when a management company is present. When set to True, the party name 'A doing business as B', for example, would be separated into two lists, where B is put in the original column, and A is added to a _managing companies_ column. When set to True, the function will return two lists.
 
 Another optional parameter taken by full_clean_names is the min_similarity_score parameter, which is passed directly to the link_company_names function and used to compute the threshold for similarity among company names.
 
+As of CC 0.8.0, full_clean_names now takes an optional party_type parameter. You can use this parameter should you wish to skip the labeling of entities as either people or companies. In order to skip this ordering, you must supply a value of either 'person' or 'company' depending on the list type that you are supplying.
+
 #### compare_companies
 
 ```python
 cleancourt.compare_companies(
 	org_name_messy,
 	org_name_clean,
 	threshold=.25,
```

### Comparing `cleancourt-0.7.9/setup.py` & `cleancourt-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="cleancourt",
-    version="0.7.9",
+    version="0.8.0",
     description="a library for cleaning court docket entries",
     author="Logan Pratico",
     author_email="praticol@lsc.gov",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.9",
```

### Comparing `cleancourt-0.7.9/src/cleancourt/__init__.py` & `cleancourt-0.8.0/src/cleancourt/__init__.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.9/src/cleancourt/check_spaces.py` & `cleancourt-0.8.0/src/cleancourt/check_spaces.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.9/src/cleancourt/clean_data.py` & `cleancourt-0.8.0/src/cleancourt/clean_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,16 +27,18 @@
         "#",
         ";",
     ]  # remove these characters
     rx = "[" + re.escape("".join(chars_to_remove)) + "]"
     string = re.sub(rx, "", string)
 
     # Replace special characters and symbols
-    string = string.replace("&", "and")
-    string = string.replace("@", "at")
+    string = string.replace("&", " and ")
+    string = string.replace("@", " at ")
+    #string = re.sub(' {2}', ' ', string)
+
     string = string.replace(
         "h/w", ""
     )  # Sometimes appears next to party names that are husband (h) and wife (w)
     string = string.replace("-", " ")
     string = string.replace("_", " ")
 
     string = re.sub(
@@ -55,36 +57,48 @@
     string = re.sub(" maa?nage?ment", " mgmt", string)  # etc
     string = re.sub(" incorporated", " inc", string)
     string = re.sub(" apartment", " apt", string)
     string = re.sub(" square(\s|$|,)", " sq\\1", string)
     string = re.sub("department", "dept", string)
 
     string = re.sub("fed[^\s]{0,4} cred[^\s]{0,2} un[^\s]{0,4}", "fcu", string)
+    string = re.sub("credit union", "fcu", string)
 
     string = re.sub("home ?owners association", "hoa", string)
-    string = re.sub("home ?owners assoc[^\s]{0,3}", "hoa", string)
+    string = re.sub("home ?owners assoc[^\s]{0,5}", "hoa", string)
     string = re.sub("hoa,? inc", "hoa", string)
 
     string = re.sub("national association", "na", string)
 
     string = re.sub("housing authy", "housing authority", string) # this replacement is being placed before any of the other housing authority replacements because "authy" appears in both PHA and RHA names
     string = re.sub("housing authority, inc", "housing authority", string)
 
     string = re.sub("redevelopment and housing authority", "rha", string)
     string = re.sub("redevelopment and housing auth[^\s]?", "rha", string)
     string = re.sub("redevelopment and housing", "rha", string)
     string = re.sub("redevelopment housing authority", "rha", string)
 
     string = re.sub("public housing authority", "pha", string)
+    string = re.sub("metropolitan housing authority", "pha", string)
     string = re.sub("housing authority", "pha", string)
     string = re.sub("housing and redevelopment authority", "pha", string)
 
     
 
     string = re.sub(" et\.?\s?al\.?$", "", string)
     string = re.sub(
         "p\.?c\.?$", "", string
     )  # Remove P.C. (Personal Corporation) abbreviation on the end of a name
 
     string = re.sub("\.", "", string)  # Remove any periods
 
+    # 6/26/2023 - remove strings that end a sentence and commonly contain filler language
+    string = re.sub(' usa na$', '', string)
+    string = re.sub(' successor in interest to$', '', string)
+    string = re.sub(' as successor to$', '', string)
+    string = re.sub(' as assignee of$', '', string)
+    string = re.sub(' as managing agent for$', '', string)
+    string = re.sub(' as managing agent$', '', string)
+    string = re.sub(' doing business as$', '', string)
+
+
     return string
```

### Comparing `cleancourt-0.7.9/src/cleancourt/compare_companies.py` & `cleancourt-0.8.0/src/cleancourt/compare_companies.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,28 +25,30 @@
 
 def compare_companies(
     org_name_messy,
     org_name_clean,
     threshold=SIMILARITY_DISTANCE,
     print_all_matches=False,
     clean_org_names=[False, False],
+    all_companies = False
 ):
     """This method implements a K-Nearest Neighbors (KNN) algorithm to
     compare a standard list of *clean* party names to a *messy* list of
     party names.
 
     With KNN algorithms, individual (new) data points are added to an existing
     dataset, and the "distance" to all other points in the dataset is computed.
 
     "Distance" is measured using TFIDF and cosine similarities similarly to the link_company_names_function.
 
     """
 
-    # Remove people from the list of names
-    org_name_messy = [name for name in org_name_messy if filter_companies(name)]
+    # Remove people from the list of names, unless you are already passing a list of companies
+    if not all_companies:
+        org_name_messy = [name for name in org_name_messy if filter_companies(name)]
 
     # Clean data in both lists if optional parameters are set to true
     if clean_org_names[0]:
         logger.info("Cleaning Messy Org Dataset")
         org_name_messy = [clean_data(name) for name in org_name_messy]
     if clean_org_names[1]:
         logger.info("Cleaning Clean Org Dataset")
```

### Comparing `cleancourt-0.7.9/src/cleancourt/cosine_similarity.py` & `cleancourt-0.8.0/src/cleancourt/cosine_similarity.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,32 +99,40 @@
         data,
     )
 
     return csr_matrix((data, indices, indptr), shape=(M, N))
 
 
 ## MAIN CODE
-def link_company_names(df, min_similarity_score=0.80):
+def link_company_names(df, min_similarity_score=0.80, party_type = 'None Specified'):
 
     """Take in a df of 1 column or a list and a minimum similarity score cutoff and return a dictionary with each of the doc"""
 
+    if party_type not in ['company', 'person', 'None Specified']:
+        logger.error('Company type must equal person, company or None')
+
     # Group data by exact matches and count the number of values
     logger.info("GROUPING DATA")
     grouped_df = (
         df.value_counts().rename_axis("first_plaintiff").reset_index(name="counts")
     )
 
     # Grab the names of each plaintiff and place into a list
     # Note: Order of this list does matter.
     # Names are prioritized based on the number of exact matches in the document
 
     names = grouped_df.first_plaintiff
 
     # create list of only company names
-    names = [name for name in names if filter_companies(name)]
+
+    # if party label is person, just return an empty dict
+    if party_type == 'person':
+        return {}
+    elif party_type != 'company':
+        names = [name for name in names if filter_companies(name)]
 
     # If there are fewer than 500 unique names in the list, compute similarity between strings using levenshtein distance
     if len(names) < MAX_NAME_LEVENSHTEIN:
         # To allow users to submit a similarity threshold that will return similar cutoffs for both methods, we multiply 1.16 as
         # a slightly higher threshold is required for levenshtein.
         min_similarity_score = min_similarity_score * SIMILARITY_SCORE_WEIGHT
```

### Comparing `cleancourt-0.7.9/src/cleancourt/filter_types.py` & `cleancourt-0.8.0/src/cleancourt/filter_types.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.9/src/cleancourt/full_clean_names.py` & `cleancourt-0.8.0/src/cleancourt/full_clean_names.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,38 +6,42 @@
 from cleancourt.clean_data import *
 from cleancourt.cosine_similarity import *
 from cleancourt.integrate_output import *
 from cleancourt.parse_names import *
 from cleancourt.separate_parent_company import separate_company_names
 
 
-def full_clean_names(messy_names, separate_management=False, min_similarity_score=0.80):
+def full_clean_names(messy_names, separate_management=False, min_similarity_score=0.80, party_type = "None Specified"):
     
     '''This is an abstracted function that calls the clean names function in CC in the order that they are intended to be called.'''
 
+    if party_type not in ['company', 'person', 'None Specified']:
+        logger.error('Company type must equal person, company or None')
+
+
 
     if not separate_management:
         df = pd.DataFrame()
 
         df["clean_names_1"] = [clean_data(x) for x in tqdm(messy_names)]
 
         # Parse the people names and format
         logger.info("PARSING PEOPLE NAMES")
-        duplicates_dict_people = format_people_names(df["clean_names_1"])
+        duplicates_dict_people = format_people_names(df["clean_names_1"], party_type)
 
         # Merge names into df
         logger.info("MERGING PEOPLE NAMES")
         df["formatted_people_names"] = df.apply(
             lambda x: map_values(x.clean_names_1, duplicates_dict_people), axis=1
         )
 
         # Parse company names
         logger.info("PARSING COMPANY NAMES")
         duplicates_dict_company = link_company_names(
-            df["clean_names_1"], min_similarity_score
+            df["clean_names_1"], min_similarity_score, party_type
         )
 
         # Merge company names into df
         logger.info("MERGING COMPANY NAMES")
         df["formatted_company_names"] = df.apply(
             lambda x: map_values(x.clean_names_1, duplicates_dict_company), axis=1
         )
@@ -73,30 +77,30 @@
         df["clean_names_1"] = [clean_data(x) for x in tqdm(messy_names)]
 
         logger.info("SEPARATING MANAGING NAMES")
         df["nameA"], df["nameB"] = separate_company_names(df["clean_names_1"])
 
         # Parse the people names and format
         logger.info("PARSING PEOPLE NAMES")
-        duplicates_dict_peopleA = format_people_names(df["nameA"])
-        duplicates_dict_peopleB = format_people_names(df["nameB"])
+        duplicates_dict_peopleA = format_people_names(df["nameA"], party_type)
+        duplicates_dict_peopleB = format_people_names(df["nameB"], party_type)
 
         # Merge names into df
         logger.info("MERGING PEOPLE NAMES")
         df["formatted_people_namesA"] = df.apply(
             lambda x: map_values(x.nameA, duplicates_dict_peopleA), axis=1
         )
         df["formatted_people_namesB"] = df.apply(
             lambda x: map_values(x.nameB, duplicates_dict_peopleB), axis=1
         )
 
         # Parse company names
         logger.info("PARSING COMPANY NAMES")
-        duplicates_dict_companyA = link_company_names(df["nameA"], min_similarity_score)
-        duplicates_dict_companyB = link_company_names(df["nameB"], min_similarity_score)
+        duplicates_dict_companyA = link_company_names(df["nameA"], min_similarity_score, party_type)
+        duplicates_dict_companyB = link_company_names(df["nameB"], min_similarity_score, party_type)
 
         # Merge company names into df
         logger.info("MERGING COMPANY NAMES")
         df["formatted_company_namesA"] = df.apply(
             lambda x: map_values(x.nameA, duplicates_dict_companyA), axis=1
         )
         df["formatted_company_namesB"] = df.apply(
```

### Comparing `cleancourt-0.7.9/src/cleancourt/integrate_output.py` & `cleancourt-0.8.0/src/cleancourt/integrate_output.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.9/src/cleancourt/parse_names.py` & `cleancourt-0.8.0/src/cleancourt/parse_names.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,38 +2,51 @@
 import probablepeople as pp
 from tqdm import tqdm
 import re
 
 from cleancourt.filter_types import filter_people
 
 
-def format_people_names(df):
+def format_people_names(df, party_type = "None Specified"):
 
     """Take in a list or df of one column and return a dictionary with each name in First Last format"""
 
+    if party_type not in ['company', 'person', 'None Specified']:
+        logger.error('Company type must equal person, company or None')
+
+
     # Group data by exact matches and count the number of values
     logger.info("GROUPING DATA")
     grouped_df = (
         df.value_counts().rename_axis("first_plaintiff").reset_index(name="counts")
     )
 
     # Grab the names of each plaintiff and place into a list
     # Note: Order of this list does matter.
     # Names are prioritized based on the number of exact matches in the document
 
     names = grouped_df.first_plaintiff
 
     names_dict = {}
 
+    # if party_type is company, no need to iterate 
+    if party_type == 'company':
+        return names_dict
+    
     # Iterate over names
-
     for name in tqdm(names):
 
         # Check if name is a person
-        is_person = filter_people(name)
+
+        if party_type == 'person':
+            is_person = True
+
+        else:
+            # If no label is specified, use built in filter
+            is_person = filter_people(name)
 
         # If is a person, grab name components from parsed names and place in a common format
         if is_person:
             val = pp.tag(name)
             try:
                 firstI = val[0]["FirstInitial"]
             except KeyError:
@@ -43,16 +56,17 @@
                 prefOther = val[0]["PrefixOther"]
             except KeyError:
                 prefOther = ""
 
 
             try: # Update 0.7.8 first names are sometimes parsed as SuffixOther in probablepeople. this attempts to correct for that error
                 sufOther = val[0]["SuffixOther"]
-                if sufOther == 'dds' or sufOther == 'md':
+                if sufOther == 'dds' or sufOther == 'md' or sufOther == 'dmd' or sufOther == 'dpn':
                     sufOtherEnd = sufOther
+                    sufOther = ""
                 else:
                     sufOtherEnd = ""
 
             except KeyError:
                 sufOther = ""
                 sufOtherEnd = ""
```

### Comparing `cleancourt-0.7.9/src/cleancourt/separate_parent_company.py` & `cleancourt-0.8.0/src/cleancourt/separate_parent_company.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 import re
 from tqdm import tqdm
 
 
 def remove_company_connector(string):
+    original_string = string
+
     string = re.sub(
-        "(.+) as a? ?management agent for (.{4,})", "\\2 /-/ \\1", string
+        "(.+) as a? ?management agent for (.{5,})", "\\2 /-/ \\1", string
     )  # Remove any appareance of as management agent for
-    string = re.sub("(.+) successor in interest to (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) [as ]?assignee of (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) [as ]?managing agent for (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) [as ]?m/a for (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.{4,}) by (.+) as managing agent$", "\\1 /-/ \\2", string)
+    string = re.sub("(.+) successor in interest to (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) as successor to (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) [as ]?assignee of (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) [as ]?managing agent for (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) [as ]?m/a for (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.{5,}) by (.+) as managing agent$", "\\1 /-/ \\2", string)
     string = re.sub(
-        "(.+) a[^A-z]?s[^A-z]?o[^A-z]? (.{4,})", "\\2 /-/ \\1", string
+        "(.+) a[^A-z]?s[^A-z]?o[^A-z]? (.{5,})", "\\2 /-/ \\1", string
     )  # Remove any appearance of a.s.o. and what follows
     string = re.sub(
-        "(.+) d[^A-z]?b[^A-z]?a[^A-z]? (.{4,})", "\\2 /-/ \\1", string
+        "(.+) d[^A-z]?b[^A-z]?a[^A-z]? (.{5,})", "\\2 /-/ \\1", string
     )  # Remove any appearance of d.b.a and what follows
-    string = re.sub("(.+) as agent for (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) agent for (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) as mg agent for (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) mg agt (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) as managing for (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) asset\.? management for (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) doing business as (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.+) owner of (.{4,})", "\\2 /-/ \\1", string)
-    string = re.sub("(.{4,}) trustee of (.+)", "\\1 /-/ \\2", string)
 
+    string = re.sub(
+        "(.+) a[^A-z]?s[^A-z]?o[^A-z]? (.{5,})", "\\2 /-/ \\1", string
+    )  # Remove any appearance of aso and what follows
+
+    string = re.sub("(.+) as agent for (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) as agent (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) agent for (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) by its agent (.{5,})", "\\1 /-/ \\2", string)
+    string = re.sub("(.+) by agent (.{5,})", "\\1 /-/ \\2", string)
+    string = re.sub("(.+) as mg agent for (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) mg agt (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) as managing for (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) asset\.? management for (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) doing business as (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.+) owner of (.{5,})", "\\2 /-/ \\1", string)
+    string = re.sub("(.{5,}) trustee of (.+)", "\\1 /-/ \\2", string)
+
+    if (re.search("^owner /-/", string)):
+        return original_string
+    
     return string
 
 
 def separate_company_names(names):
     plaintiffs = []
     plaintiff_parents = []
```

### Comparing `cleancourt-0.7.9/src/cleancourt/test_utils.py` & `cleancourt-0.8.0/src/cleancourt/test_utils.py`

 * *Files identical despite different names*

### Comparing `cleancourt-0.7.9/src/cleancourt.egg-info/PKG-INFO` & `cleancourt-0.8.0/src/cleancourt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleancourt
-Version: 0.7.9
+Version: 0.8.0
 Summary: a library for cleaning court docket entries
 Home-page: UNKNOWN
 Author: Logan Pratico
 Author-email: praticol@lsc.gov
 License: UNKNOWN
 Description: 
         # cleancourt
@@ -30,23 +30,27 @@
         
         #### full_clean_names
         
         ```python
         cleancourt.full_clean_names(
           messy_name_list,
           separate_management=False,
-          min_similarity_score=.80
+          min_similarity_score=.80,
+          party_type = 'None Specified'
+        
         )
         ```
         The full_clean_names function takes in a list of messy names in the dataset and applies all name cleaning functions to said dataset. The function first cleans the data using pattern matching, then separates the data based on whether a party name refers to an individual or a company. From there, the two datasets are cleaned in isolation using the format_people_names or the link_company_names discussed below. The datasets are then rejoined and linked one more time by removing spaces using the check_spaces function.
         
         The full_clean_names function also takes in an optional boolean parameter to determine whether or not a party name should be separated into two separate lists when a management company is present. When set to True, the party name 'A doing business as B', for example, would be separated into two lists, where B is put in the original column, and A is added to a _managing companies_ column. When set to True, the function will return two lists.
         
         Another optional parameter taken by full_clean_names is the min_similarity_score parameter, which is passed directly to the link_company_names function and used to compute the threshold for similarity among company names.
         
+        As of CC 0.8.0, full_clean_names now takes an optional party_type parameter. You can use this parameter should you wish to skip the labeling of entities as either people or companies. In order to skip this ordering, you must supply a value of either 'person' or 'company' depending on the list type that you are supplying.
+        
         #### compare_companies
         
         ```python
         cleancourt.compare_companies(
         	org_name_messy,
         	org_name_clean,
         	threshold=.25,
```

### Comparing `cleancourt-0.7.9/src/cleancourt.egg-info/SOURCES.txt` & `cleancourt-0.8.0/src/cleancourt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

