# Comparing `tmp/metaphor-python-0.1.4.tar.gz` & `tmp/metaphor-python-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaphor-python-0.1.4.tar", last modified: Thu Jul 13 04:45:51 2023, max compression
+gzip compressed data, was "metaphor-python-0.1.5.tar", last modified: Tue Jul 25 03:48:01 2023, max compression
```

## Comparing `metaphor-python-0.1.4.tar` & `metaphor-python-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-13 04:45:51.136738 metaphor-python-0.1.4/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-13 04:45:51.136549 metaphor-python-0.1.4/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)       81 2023-07-04 22:56:54.000000 metaphor-python-0.1.4/README.md
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-13 04:45:51.135682 metaphor-python-0.1.4/metaphor_python/
--rw-r--r--   0 jwang      (501) staff       (20)      180 2023-07-04 23:03:27.000000 metaphor-python-0.1.4/metaphor_python/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)     3456 2023-07-13 04:44:55.000000 metaphor-python-0.1.4/metaphor_python/api.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-13 04:45:51.136340 metaphor-python-0.1.4/metaphor_python.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-13 04:45:51.000000 metaphor-python-0.1.4/metaphor_python.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-13 04:45:51.000000 metaphor-python-0.1.4/metaphor_python.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-13 04:45:51.000000 metaphor-python-0.1.4/metaphor_python.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-13 04:45:51.000000 metaphor-python-0.1.4/metaphor_python.egg-info/requires.txt
--rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-13 04:45:51.000000 metaphor-python-0.1.4/metaphor_python.egg-info/top_level.txt
--rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-13 04:45:51.136790 metaphor-python-0.1.4/setup.cfg
--rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-13 04:44:20.000000 metaphor-python-0.1.4/setup.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 03:48:01.471606 metaphor-python-0.1.5/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 03:48:01.471379 metaphor-python-0.1.5/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)     1505 2023-07-25 03:43:18.000000 metaphor-python-0.1.5/README.md
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 03:48:01.469863 metaphor-python-0.1.5/metaphor_python/
+-rw-r--r--   0 jwang      (501) staff       (20)      180 2023-07-04 23:03:27.000000 metaphor-python-0.1.5/metaphor_python/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)     4279 2023-07-25 03:42:32.000000 metaphor-python-0.1.5/metaphor_python/api.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-25 03:48:01.470870 metaphor-python-0.1.5/metaphor_python.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)      610 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      263 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        9 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/requires.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       16 2023-07-25 03:48:01.000000 metaphor-python-0.1.5/metaphor_python.egg-info/top_level.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-25 03:48:01.471655 metaphor-python-0.1.5/setup.cfg
+-rw-r--r--   0 jwang      (501) staff       (20)      773 2023-07-25 03:43:59.000000 metaphor-python-0.1.5/setup.py
```

### Comparing `metaphor-python-0.1.4/PKG-INFO` & `metaphor-python-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.4/metaphor_python/api.py` & `metaphor-python-0.1.5/metaphor_python/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import requests
 from typing import List, Optional
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 def snake_to_camel(snake_str: str) -> str:
     components = snake_str.split("_")
     return components[0] + "".join(x.title() for x in components[1:])
 
 def to_camel_case(data: dict) -> dict:
     return {snake_to_camel(k): v for k, v in data.items() if v is not None}
@@ -24,35 +24,34 @@
     include_domains: Optional[List[str]] = None
     exclude_domains: Optional[List[str]] = None
     start_crawl_date: Optional[str] = None
     end_crawl_date: Optional[str] = None
     start_published_date: Optional[str] = None
     end_published_date: Optional[str] = None
     use_autoprompt: Optional[bool] = None
+    type: Optional[str] = None
 
 @dataclass
 class Result:
     title: str
     url: str
     score: float
     id: str
     published_date: Optional[str] = None
     author: Optional[str] = None
+    extract: Optional[str] = None # beta field. returned when findSimilar_and_get_contents is called
 
     def __init__(self, title, url, score, id, published_date=None, author=None, **kwargs):
         self.title = title
         self.url = url
         self.score = score
         self.id = id
         self.published_date = published_date
         self.author = author
 
-@dataclass
-class SearchResponse:
-    results: List[Result]
 
 @dataclass
 class FindSimilarRequest:
     url: str
     num_results: Optional[int] = None
     include_domains: Optional[List[str]] = None
     exclude_domains: Optional[List[str]] = None
@@ -78,26 +77,44 @@
         self.title = title
         self.extract = extract
 
 @dataclass
 class GetContentsResponse:
     contents: List[DocumentContent]
 
+@dataclass
+class SearchResponse:
+    results: List[Result]
+    api: Optional['Metaphor'] = field(default=None, init=False)
+
+    def get_contents(self):
+        if self.api is None:
+            raise Exception("API client is not set. This method should be called on a SearchResponse returned by the 'search' method of 'Metaphor'.")
+        ids = [result.id for result in self.results]
+        get_contents_request = GetContentsRequest(ids=ids)
+        return self.api.get_contents(get_contents_request)
+
 class Metaphor:
     def __init__(self, api_key: str):
         self.base_url = "https://api.metaphor.systems"
         self.headers = {"x-api-key": api_key}
 
     def search(self, request: SearchRequest) -> SearchResponse:
         response = requests.post(f"{self.base_url}/search", json=to_camel_case(request.__dict__), headers=self.headers)
         response.raise_for_status()
-        return SearchResponse([Result(**to_snake_case(result)) for result in response.json()["results"]])
+        results = [Result(**to_snake_case(result)) for result in response.json()["results"]]
+        search_response = SearchResponse(results=results)
+        search_response.api = self
+        return search_response
 
     def find_similar(self, request: FindSimilarRequest) -> SearchResponse:
         response = requests.post(f"{self.base_url}/findSimilar", json=to_camel_case(request.__dict__), headers=self.headers)
         response.raise_for_status()
-        return SearchResponse([Result(**to_snake_case(result)) for result in response.json()["results"]])
+        results = [Result(**to_snake_case(result)) for result in response.json()["results"]]
+        find_similar_response = SearchResponse(results=results)
+        find_similar_response.api = self
+        return find_similar_response
 
     def get_contents(self, request: GetContentsRequest) -> GetContentsResponse:
         response = requests.get(f"{self.base_url}/contents", params=to_camel_case(request.__dict__), headers=self.headers)
         response.raise_for_status()
         return GetContentsResponse([DocumentContent(**to_snake_case(document)) for document in response.json()["contents"]])
```

### Comparing `metaphor-python-0.1.4/metaphor_python.egg-info/PKG-INFO` & `metaphor-python-0.1.5/metaphor_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for the Metaphor API.
 Home-page: https://github.com/metaphorsystems/metaphor-python
 Author: Metaphor
 Author-email: hello@metaphor.systems
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metaphor-python-0.1.4/setup.py` & `metaphor-python-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='metaphor-python',
-    version='0.1.4',
+    version='0.1.5',
     description='A Python package for the Metaphor API.',
     author='Metaphor',
     author_email='hello@metaphor.systems',
     url='https://github.com/metaphorsystems/metaphor-python',
     packages=find_packages(),
     install_requires=[
         'requests',
```

