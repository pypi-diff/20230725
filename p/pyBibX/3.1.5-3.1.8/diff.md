# Comparing `tmp/pyBibX-3.1.5.tar.gz` & `tmp/pyBibX-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-3.1.5.tar", last modified: Sat Jun 17 23:52:27 2023, max compression
+gzip compressed data, was "dist\pyBibX-3.1.8.tar", last modified: Tue Jul 25 12:42:52 2023, max compression
```

## Comparing `pyBibX-3.1.5.tar` & `pyBibX-3.1.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 23:52:27.000000 pyBibX-3.1.5/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.1.5/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     9608 2023-06-17 23:52:27.000000 pyBibX-3.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 23:52:26.000000 pyBibX-3.1.5/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.5/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 23:52:26.000000 pyBibX-3.1.5/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.1.5/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   265168 2023-06-17 23:51:26.000000 pyBibX-3.1.5/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-06-17 23:52:27.000000 pyBibX-3.1.5/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Chinese.txt
--rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Greek.txt
--rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Hebrew.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Japanese.txt
--rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Korean.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Slovak.txt
--rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Thai.txt
--rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Ukrainian.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.5/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 23:52:26.000000 pyBibX-3.1.5/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9608 2023-06-17 23:52:25.000000 pyBibX-3.1.5/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-06-17 23:52:26.000000 pyBibX-3.1.5/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 23:52:25.000000 pyBibX-3.1.5/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      218 2023-06-17 23:52:25.000000 pyBibX-3.1.5/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 23:52:25.000000 pyBibX-3.1.5/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-17 23:52:25.000000 pyBibX-3.1.5/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-06-17 23:52:27.000000 pyBibX-3.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-06-17 23:51:53.000000 pyBibX-3.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:52.000000 pyBibX-3.1.8/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-3.1.8/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-3.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     9608 2023-07-25 12:42:52.000000 pyBibX-3.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9165 2023-05-06 14:18:32.000000 pyBibX-3.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:51.000000 pyBibX-3.1.8/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.8/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:51.000000 pyBibX-3.1.8/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-3.1.8/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   265828 2023-07-25 12:41:38.000000 pyBibX-3.1.8/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:52.000000 pyBibX-3.1.8/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     6482 2023-05-31 13:32:50.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     3295 2023-05-28 21:46:34.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Chinese.txt
+-rw-rw-rw-   0        0        0     1934 2023-05-31 13:36:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4284 2023-05-31 13:37:00.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3484 2023-05-31 13:37:46.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-31 13:39:46.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     7901 2023-05-28 21:47:27.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Greek.txt
+-rw-rw-rw-   0        0        0     1656 2023-05-28 21:47:36.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hebrew.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     4074 2023-05-31 13:48:26.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     2202 2023-05-28 21:48:04.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Japanese.txt
+-rw-rw-rw-   0        0        0     7417 2023-05-28 21:48:29.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Korean.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0      883 2023-05-28 21:48:40.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Slovak.txt
+-rw-rw-rw-   0        0        0     3128 2023-05-31 13:53:58.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0     1521 2023-05-28 21:58:26.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Thai.txt
+-rw-rw-rw-   0        0        0      627 2023-05-28 21:49:00.000000 pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Ukrainian.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-3.1.8/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 12:42:51.000000 pyBibX-3.1.8/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      218 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 12:42:50.000000 pyBibX-3.1.8/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-07-25 12:42:52.000000 pyBibX-3.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-07-25 12:41:51.000000 pyBibX-3.1.8/setup.py
```

### Comparing `pyBibX-3.1.5/LICENSE` & `pyBibX-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/PKG-INFO` & `pyBibX-3.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.1.5
+Version: 3.1.8
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.1.5/README.md` & `pyBibX-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/pbx.py` & `pyBibX-3.1.8/pyBibX/base/pbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,25 +745,31 @@
         self.__make_bib(verbose = False)
         return
     
     # Function: Merge Institution
     def merge_institution(self, get = [], replace_for = 'name'):
         for name in get:
             for i in range(0, self.data.shape[0]):
-                target = self.data.loc[i, 'affiliation'].lower()
+                if (self.data.loc[i, 'source'].lower() == 'scopus' or self.data.loc[i, 'source'].lower() == 'pubmed'):
+                    target = self.data.loc[i, 'affiliation'].lower()
+                elif (self.data.loc[i, 'source'].lower() == 'wos'):
+                    target = self.data.loc[i, 'affiliation_'].lower()
                 if (name.lower() in target):
                     self.data.loc[i, 'affiliation'] = target.replace(name, replace_for)
         self.__make_bib(verbose = False)
         return
-    
+                
     # Function: Merge Country
     def merge_country(self, get = [], replace_for = 'name'):
         for name in get:
             for i in range(0, self.data.shape[0]):
-                target = self.data.loc[i, 'affiliation'].lower()
+                if (self.data.loc[i, 'source'].lower() == 'scopus' or self.data.loc[i, 'source'].lower() == 'pubmed'):
+                    target = self.data.loc[i, 'affiliation'].lower()
+                elif (self.data.loc[i, 'source'].lower() == 'wos'):
+                    target = self.data.loc[i, 'affiliation_'].lower()
                 if (name.lower() in target):
                     self.data.loc[i, 'affiliation'] = target.replace(name, replace_for)
         self.__make_bib(verbose = False)
         return
     
     # Function: Merge Language
     def merge_language(self, get = [], replace_for = 'name'):
@@ -1246,15 +1252,15 @@
     # Function: Get Countries
     def __get_countries(self):
         df = pd.Series(np.zeros(self.data.shape[0]))
         for i in range(0, self.data.shape[0]):
             if (self.data.loc[i, 'source'].lower() == 'scopus' or self.data.loc[i, 'source'].lower() == 'pubmed'):
                 df[i] = self.data.loc[i, 'affiliation']
             elif (self.data.loc[i, 'source'].lower() == 'wos'):
-                df[i] = self.data.loc[i, 'affiliation_']
+                df[i] = self.data.loc[i, 'affiliation_'].replace('(Corresponding Author)', '')
         df = df.str.replace(' USA',            ' United States of America',   case = False, regex = True)
         df = df.str.replace('ENGLAND',         'United Kingdom',              case = False, regex = True)
         df = df.str.replace('Antigua & Barbu', 'Antigua and Barbuda',         case = False, regex = True)
         df = df.str.replace('Bosnia & Herceg', 'Bosnia and Herzegovina',      case = False, regex = True)
         df = df.str.replace('Cent Afr Republ', 'Central African Republic',    case = False, regex = True)
         df = df.str.replace('Dominican Rep',   'Dominican Republic',          case = False, regex = True)
         df = df.str.replace('Equat Guinea',    'Equatorial Guinea',           case = False, regex = True)
@@ -1269,15 +1275,16 @@
         df = df.str.replace('Sao Tome E Prin', 'Sao Tome and Principe',       case = False, regex = True)
         df = df.str.replace('St Kitts & Nevi', 'Saint Kitts and Nevis',       case = False, regex = True)
         df = df.str.replace('Trinid & Tobago', 'Trinidad and Tobago',         case = False, regex = True)
         df = df.str.replace('U Arab Emirates', 'United Arab Emirates',        case = False, regex = True)
         df = df.str.lower()
         for i in range(0, len(self.aut)):
             for j in range(0, len(self.aut[i])):
-                df = df.str.replace(self.aut[i][j], self.aut[i][j].replace('.', ''), regex = True)
+                for k in range(0, df.shape[0]):
+                    df[k] = df[k].replace(self.aut[i][j], self.aut[i][j].replace('.', ''))
         ctrs = [[] for i in range(0, df.shape[0])]
         for i in range(0, self.data.shape[0]):
             if (self.data.loc[i, 'source'].lower() == 'scopus'):
                 affiliations = str(df[i]).strip().split(';')
                 for affiliation in affiliations:
                     for country in self.country_names:
                         if (country.lower() in affiliation.lower()):
@@ -1318,15 +1325,16 @@
             if (self.data.loc[i, 'source'].lower() == 'scopus' or self.data.loc[i, 'source'].lower() == 'pubmed'):
                 df[i] = self.data.loc[i, 'affiliation']
             elif (self.data.loc[i, 'source'].lower() == 'wos'):
                 df[i] = self.data.loc[i, 'affiliation_']
         df = df.str.lower()
         for i in range(0, len(self.aut)):
             for j in range(0, len(self.aut[i])):
-                df = df.str.replace(self.aut[i][j], self.aut[i][j].replace('.', ''), regex = True)
+                for k in range(0, df.shape[0]):
+                    df[k] = df[k].replace(self.aut[i][j], self.aut[i][j].replace('.', ''))
         inst  = [[] for i in range(0, df.shape[0])]
         inst_ = [[] for i in range(0, df.shape[0])]
         for i in range(0, df.shape[0]):
             if  (self.data.loc[i, 'source'].lower() == 'scopus'):
                 affiliations = str(df[i]).split(';')
                 for affiliation in affiliations:
                     for institution in self.institution_names:
```

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Chinese.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Chinese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Greek.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Greek.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Hebrew.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hebrew.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Japanese.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Japanese.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Korean.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Korean.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Slovak.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Slovak.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Thai.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Thai.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX/base/stws/Stopwords-Ukrainian.txt` & `pyBibX-3.1.8/pyBibX/base/stws/Stopwords-Ukrainian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/pyBibX.egg-info/PKG-INFO` & `pyBibX-3.1.8/pyBibX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 3.1.5
+Version: 3.1.8
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyBibX-3.1.5/pyBibX.egg-info/SOURCES.txt` & `pyBibX-3.1.8/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-3.1.5/setup.py` & `pyBibX-3.1.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='3.1.5',
+    version='3.1.8',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

