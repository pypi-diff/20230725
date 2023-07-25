# Comparing `tmp/NewsArticlesScraper-0.2.5.tar.gz` & `tmp/NewsArticlesScraper-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewsArticlesScraper-0.2.5.tar", last modified: Mon May 22 21:45:56 2023, max compression
+gzip compressed data, was "dist\NewsArticlesScraper-0.2.7.tar", last modified: Tue Jul 25 14:49:53 2023, max compression
```

## Comparing `NewsArticlesScraper-0.2.5.tar` & `NewsArticlesScraper-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 21:45:56.001160 NewsArticlesScraper-0.2.5/
-drwxrwxrwx   0        0        0        0 2023-05-22 21:45:55.980159 NewsArticlesScraper-0.2.5/NewsArticlesScraper/
--rw-rw-rw-   0        0        0    14673 2023-05-22 21:42:30.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper/Scrapers.py
--rw-rw-rw-   0        0        0       64 2023-02-14 20:15:57.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper/__init__.py
--rw-rw-rw-   0        0        0     1074 2023-04-23 16:12:20.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper/test.py
-drwxrwxrwx   0        0        0        0 2023-05-22 21:45:55.999160 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/
--rw-rw-rw-   0        0        0      648 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-22 21:45:55.000000 NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2023-05-22 21:45:56.000659 NewsArticlesScraper-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-02-14 20:04:13.000000 NewsArticlesScraper-0.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 21:45:56.001160 NewsArticlesScraper-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      996 2023-05-22 21:45:42.000000 NewsArticlesScraper-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:49:53.332652 NewsArticlesScraper-0.2.7/
+drwxrwxrwx   0        0        0        0 2023-07-25 14:49:53.274650 NewsArticlesScraper-0.2.7/NewsArticlesScraper/
+-rw-rw-rw-   0        0        0    11043 2023-07-25 08:07:58.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper/ArticleUrlSrapers.py
+-rw-rw-rw-   0        0        0    14676 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper/Scrapers.py
+-rw-rw-rw-   0        0        0       64 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 14:49:53.328652 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/
+-rw-rw-rw-   0        0        0      648 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-25 14:49:53.000000 NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2023-07-25 14:49:53.331653 NewsArticlesScraper-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-07 10:09:57.000000 NewsArticlesScraper-0.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 14:49:53.333653 NewsArticlesScraper-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-07-25 14:39:52.000000 NewsArticlesScraper-0.2.7/setup.py
```

### Comparing `NewsArticlesScraper-0.2.5/NewsArticlesScraper/Scrapers.py` & `NewsArticlesScraper-0.2.7/NewsArticlesScraper/Scrapers.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             if api_point == "historic" and self.subsections_to_include is not None:
                 subsection = article.get("subsection_name", None)
                 if subsection is None:
                     continue
                 if subsection not in self.subsections_to_include:
                     continue
             if api_point == "recent" and self.subsections_to_include is not None:
-                if article["section"] not in self.subsections_to_include:
+                if article["subsection"] not in self.subsections_to_include:
                     continue
             if api_point == "historic":
                 pub_date = article["pub_date"]
             else:
                 pub_date = article["published_date"]
             pub_date = ciso8601.parse_datetime(pub_date)
             if pub_date < self.from_time:
```

### Comparing `NewsArticlesScraper-0.2.5/NewsArticlesScraper.egg-info/PKG-INFO` & `NewsArticlesScraper-0.2.7/NewsArticlesScraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.5
+Version: 0.2.7
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.5/PKG-INFO` & `NewsArticlesScraper-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewsArticlesScraper
-Version: 0.2.5
+Version: 0.2.7
 Summary: Scraping news articles
 Author: PySlayer (Paul Antweiler)
 Author-email: antweiler.paul@gmail.com
 Keywords: python,news,scraping,news scraping,news articles
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NewsArticlesScraper-0.2.5/setup.py` & `NewsArticlesScraper-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.5'
+VERSION = '0.2.7'
 DESCRIPTION = 'Scraping news articles'
 LONG_DESCRIPTION = 'A package that allows you to scrape news articles from various news sites via scrapy.'
 
 # Setting up
 setup(
     name="NewsArticlesScraper",
     version=VERSION,
```

