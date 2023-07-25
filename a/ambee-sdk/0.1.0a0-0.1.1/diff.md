# Comparing `tmp/ambee_sdk-0.1.0a0.tar.gz` & `tmp/ambee_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambee_sdk-0.1.0a0.tar", last modified: Mon Mar 20 14:25:18 2023, max compression
+gzip compressed data, was "ambee_sdk-0.1.1.tar", last modified: Tue Jul 25 09:03:23 2023, max compression
```

## Comparing `ambee_sdk-0.1.0a0.tar` & `ambee_sdk-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     1062 2023-03-01 05:42:50.000000 ambee_sdk-0.1.0a0/LICENSE
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     1619 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/PKG-INFO
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     1145 2023-03-20 14:22:23.000000 ambee_sdk-0.1.0a0/README.md
-drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/ambee_sdk/
--rw-rw-r--   0 ambee     (1000) ambee     (1000)       25 2023-03-02 06:32:50.000000 ambee_sdk-0.1.0a0/ambee_sdk/__init__.py
--rw-rw-r--   0 ambee     (1000) ambee     (1000)    43276 2023-03-09 08:26:46.000000 ambee_sdk-0.1.0a0/ambee_sdk/ambee_sdk.py
-drwxrwxr-x   0 ambee     (1000) ambee     (1000)        0 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/
--rw-rw-r--   0 ambee     (1000) ambee     (1000)     1619 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ambee     (1000) ambee     (1000)      235 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ambee     (1000) ambee     (1000)        1 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ambee     (1000) ambee     (1000)       26 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/requires.txt
--rw-rw-r--   0 ambee     (1000) ambee     (1000)       10 2023-03-20 14:25:18.000000 ambee_sdk-0.1.0a0/ambee_sdk.egg-info/top_level.txt
--rw-rw-r--   0 ambee     (1000) ambee     (1000)       38 2023-03-20 14:25:18.461502 ambee_sdk-0.1.0a0/setup.cfg
--rw-rw-r--   0 ambee     (1000) ambee     (1000)      939 2023-03-09 04:15:39.000000 ambee_sdk-0.1.0a0/setup.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-25 09:03:23.780321 ambee_sdk-0.1.1/
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1062 2023-03-01 05:42:50.000000 ambee_sdk-0.1.1/LICENSE
+-rw-r--r--   0 ambee      (501) staff       (20)     1560 2023-07-25 09:03:23.780204 ambee_sdk-0.1.1/PKG-INFO
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1107 2023-07-25 07:53:23.000000 ambee_sdk-0.1.1/README.md
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-25 09:03:23.779254 ambee_sdk-0.1.1/ambee_sdk/
+-rwxr-xr-x   0 ambee      (501) staff       (20)       25 2023-03-02 06:32:50.000000 ambee_sdk-0.1.1/ambee_sdk/__init__.py
+-rwxr-xr-x   0 ambee      (501) staff       (20)    48872 2023-07-25 08:58:37.000000 ambee_sdk-0.1.1/ambee_sdk/ambee_sdk.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-25 09:03:23.779943 ambee_sdk-0.1.1/ambee_sdk.egg-info/
+-rwxr-xr-x   0 ambee      (501) staff       (20)     1560 2023-07-25 09:03:23.000000 ambee_sdk-0.1.1/ambee_sdk.egg-info/PKG-INFO
+-rwxr-xr-x   0 ambee      (501) staff       (20)      259 2023-07-25 09:03:23.000000 ambee_sdk-0.1.1/ambee_sdk.egg-info/SOURCES.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)        1 2023-07-25 09:03:23.000000 ambee_sdk-0.1.1/ambee_sdk.egg-info/dependency_links.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)       26 2023-07-25 09:03:23.000000 ambee_sdk-0.1.1/ambee_sdk.egg-info/requires.txt
+-rwxr-xr-x   0 ambee      (501) staff       (20)       10 2023-07-25 09:03:23.000000 ambee_sdk-0.1.1/ambee_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ambee      (501) staff       (20)       38 2023-07-25 09:03:23.780366 ambee_sdk-0.1.1/setup.cfg
+-rwxr-xr-x   0 ambee      (501) staff       (20)      938 2023-07-25 06:00:24.000000 ambee_sdk-0.1.1/setup.py
+drwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-07-25 09:03:23.780077 ambee_sdk-0.1.1/tests/
+-rwxr-xr-x   0 ambee      (501) staff       (20)        0 2023-01-21 20:20:29.000000 ambee_sdk-0.1.1/tests/test_functions.py
```

### Comparing `ambee_sdk-0.1.0a0/LICENSE` & `ambee_sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ambee_sdk-0.1.0a0/PKG-INFO` & `ambee_sdk-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ambee_sdk
-Version: 0.1.0a0
+Version: 0.1.1
 Summary: Python SDK for Ambee's APIs
 Home-page: 
 Author: Ambee
 License: MIT
 Keywords: ambee climate environment pollen air-quality weather api sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -21,15 +20,15 @@
 [![Downloads](https://static.pepy.tech/badge/ambee-sdk)](https://pepy.tech/project/ambee-sdk)
 [![Documentation Status](https://readthedocs.org/projects/ambee-sdk/badge/?version=latest)](https://ambee-sdk.readthedocs.io/en/latest/?badge=latest)
 
 Ambee SDK for python provides classes and methods to make use of ambee's APIs inside your python code. You can make calls to our apis, get output in dataframe format, make calls to multiple locations and more.
 
 Read our API documentation: [Ambee: Developers tool](https://docs.ambeedata.com/DeveloperTools/)
 
-Readthedocs - [Welcome to ambee-sdk’s documentation! &mdash; ambee-sdk 0.1.0a documentation](https://ambee-sdk.readthedocs.io/en/latest/index.html)
+Readthedocs - [Welcome to ambee-sdk’s documentation! ](https://ambee-sdk.readthedocs.io/en/latest/index.html)
 
 ## Getting Started
 
 ```py
 import ambee_sdk as ambee
 import datetime
 ```
@@ -38,8 +37,7 @@
 x_api_key = "Your Key Here"
 ```
 
 ```python
 aq = ambee.air_quality(x_api_key=x_api_key)
 aq.get_latest(by='latlng', lat=12, lng=77)
 ```
-
```

### Comparing `ambee_sdk-0.1.0a0/README.md` & `ambee_sdk-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Downloads](https://static.pepy.tech/badge/ambee-sdk)](https://pepy.tech/project/ambee-sdk)
 [![Documentation Status](https://readthedocs.org/projects/ambee-sdk/badge/?version=latest)](https://ambee-sdk.readthedocs.io/en/latest/?badge=latest)
 
 Ambee SDK for python provides classes and methods to make use of ambee's APIs inside your python code. You can make calls to our apis, get output in dataframe format, make calls to multiple locations and more.
 
 Read our API documentation: [Ambee: Developers tool](https://docs.ambeedata.com/DeveloperTools/)
 
-Readthedocs - [Welcome to ambee-sdk’s documentation! &mdash; ambee-sdk 0.1.0a documentation](https://ambee-sdk.readthedocs.io/en/latest/index.html)
+Readthedocs - [Welcome to ambee-sdk’s documentation! ](https://ambee-sdk.readthedocs.io/en/latest/index.html)
 
 ## Getting Started
 
 ```py
 import ambee_sdk as ambee
 import datetime
 ```
```

### Comparing `ambee_sdk-0.1.0a0/ambee_sdk/ambee_sdk.py` & `ambee_sdk-0.1.1/ambee_sdk/ambee_sdk.py`

 * *Files 9% similar despite different names*

```diff
@@ -150,29 +150,26 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/latest/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/latest/by-lat-lng?lat={}&lng={}".format(
-                            lat, lng
-                        ),
-                        headers=headers,
-                    )
+                    url = base_url + "by-lat-lng?lat={}&lng={}".format(lat, lng)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["stations"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
@@ -186,20 +183,21 @@
                 )
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/latest/by-postal-code?postalCode={}&countryCode={}".format(
+                    url = (
+                        base_url
+                        + "by-postal-code?postalCode={}&countryCode={}".format(
                             postalCode, countryCode
-                        ),
-                        headers=headers,
+                        )
                     )
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["stations"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
@@ -211,28 +209,18 @@
                 raise InvalidInputError("The call is missing city value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    if limit == None:
-                        response = requests.get(
-                            "https://api.ambeedata.com/latest/by-city?city={}".format(
-                                city
-                            ),
-                            headers=headers,
-                        )
-                    else:
-                        response = requests.get(
-                            "https://api.ambeedata.com/latest/by-city?city={}&limit={}".format(
-                                city, limit
-                            ),
-                            headers=headers,
-                        )
+                    url = base_url + "by-city?city={}".format(city)
+                    if limit is not None:
+                        url = url + "&limit={}".format(limit)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["stations"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
@@ -244,28 +232,20 @@
                 raise InvalidInputError("The call is missing countryCode value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    if limit == None:
-                        response = requests.get(
-                            "https://api.ambeedata.com/latest/by-country-code?countryCode={}".format(
-                                countryCode
-                            ),
-                            headers=headers,
-                        )
-                    else:
-                        response = requests.get(
-                            "https://api.ambeedata.com/latest/by-country-code?countryCode={}&limit={}".format(
-                                countryCode, limit
-                            ),
-                            headers=headers,
-                        )
+                    url = base_url + "by-country-code?countryCode={}".format(
+                        countryCode
+                    )
+                    if limit is not None:
+                        url = url + "&limit={}".format(limit)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["stations"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
@@ -298,29 +278,28 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/history/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/history/by-lat-lng?lat={}&lng={}&from={}&to={}".format(
-                            lat, lng, from_val, to_val
-                        ),
-                        headers=headers,
+                    url = base_url + "by-lat-lng?lat={}&lng={}&from={}&to={}".format(
+                        lat, lng, from_val, to_val
                     )
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["data"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
@@ -333,20 +312,21 @@
                 )
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/history/by-postal-code?postalCode={}&countryCode={}&from={}&to={}".format(
+                    url = (
+                        base_url
+                        + "by-postal-code?postalCode={}&countryCode={}&from={}&to={}".format(
                             postalCode, countryCode, from_val, to_val
-                        ),
-                        headers=headers,
+                        )
                     )
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["data"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
@@ -364,73 +344,74 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/latest/"
         if by == "order":
             if order == None:
                 raise InvalidInputError("The call is missing order value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/latest/by-order/{}".format(order),
-                        headers=headers,
-                    )
+                    url = base_url + "by-order/{}".format(order)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["stations"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
                     print(response.status_code)
                     raise e
 
 
 class pollen(ambee):
     """Contains methods to fetch data from Pollen API"""
 
-    def get_latest(self, by, lat=None, lng=None, place=None, return_df=False):
+    def get_latest(
+        self, by, lat=None, lng=None, place=None, speciesRisk=False, return_df=False
+    ):
         """Retrives latest pollen data for a given location
 
         Args:
             by (str): signifies the type of input supported by Ambee API. Refer to API Documentation.
             lat (float/int/str, optional): Latitude. Defaults to None.
             lng (float/int/str, optional): Longitude. Defaults to None.
             place (str, optional): Placename. Defaults to None.
+            speciesRisk (bool, optional): Gives risk for species if True
             return_df (bool, optional): Converts results to pandas dataframe if True. Defaults to False.
 
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/latest/pollen/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/latest/pollen/by-lat-lng?lat={}&lng={}".format(
-                            lat, lng
-                        ),
-                        headers=headers,
+                    url = base_url + "by-lat-lng?lat={}&lng={}&speciesRisk={}".format(
+                        lat, lng, speciesRisk
                     )
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
                             meta=["lat", "lng"],
                             errors="ignore",
                         )
@@ -444,35 +425,41 @@
                 raise InvalidInputError("The call is missing place value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/latest/pollen/by-place?place={}".format(
-                            place
-                        ),
-                        headers=headers,
+                    url = base_url + "by-place?place={}&speciesRisk={}".format(
+                        place, speciesRisk
                     )
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
                             meta=["lat", "lng"],
                             errors="ignore",
                         )
                     else:
                         return response.json()
                 except Exception as e:
                     print(response.status_code)
                     raise e
 
     def get_historical(
-        self, by, from_val, to_val, lat=None, lng=None, place=None, return_df=False
+        self,
+        by,
+        from_val,
+        to_val,
+        lat=None,
+        lng=None,
+        place=None,
+        speciesRisk=False,
+        return_df=False,
     ):
         """Retrives historical pollen data for a given location
 
         Args:
             by (str): signifies the type of input supported by Ambee API. Refer to API Documentation.
             from_val (str): Start timestamp for historical query
             to_val (_type_): End timestamp for historical query
@@ -484,29 +471,31 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/history/pollen/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/history/pollen/by-lat-lng?lat={}&lng={}&from={}&to={}".format(
-                            lat, lng, from_val, to_val
-                        ),
-                        headers=headers,
+                    url = (
+                        base_url
+                        + "by-lat-lng?lat={}&lng={}&from={}&to={}&speciesRisk={}".format(
+                            lat, lng, from_val, to_val, speciesRisk
+                        )
                     )
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
                             meta=["lat", "lng"],
                             errors="ignore",
                         )
@@ -520,34 +509,37 @@
                 raise InvalidInputError("The call is missing place value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/history/pollen/by-place?place={}&from={}&to={}".format(
-                            place, from_val, to_val
-                        ),
-                        headers=headers,
+                    url = (
+                        base_url
+                        + "by-place?place={}&from={}&to={}&speciesRisk={}".format(
+                            place, from_val, to_val, speciesRisk
+                        )
                     )
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
                             meta=["lat", "lng"],
                             errors="ignore",
                         )
                     else:
                         return response.json()
                 except Exception as e:
                     print(response.status_code)
                     raise e
 
-    def get_forecast(self, by, lat=None, lng=None, place=None, return_df=False):
+    def get_forecast(
+        self, by, lat=None, lng=None, place=None, speciesRisk=False, return_df=False
+    ):
         """Retrives forecasted pollen data for a given location
 
         Args:
             by (str): signifies the type of input supported by Ambee API. Refer to API Documentation.
             lat (float/int/str, optional): Latitude. Defaults to None.
             lng (float/int/str, optional): Longitude. Defaults to None.
             place (str, optional): Placename. Defaults to None.
@@ -556,29 +548,28 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/forecast/pollen/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/forecast/pollen/by-lat-lng?lat={}&lng={}".format(
-                            lat, lng
-                        ),
-                        headers=headers,
+                    url = base_url + "by-lat-lng?lat={}&lng={}&speciesRisk={}".format(
+                        lat, lng, speciesRisk
                     )
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
                             meta=["lat", "lng"],
                             errors="ignore",
                         )
@@ -592,20 +583,18 @@
                 raise InvalidInputError("The call is missing place value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/forecast/pollen/by-place?place={}".format(
-                            place
-                        ),
-                        headers=headers,
+                    url = base_url + "by-place?place={}&speciesRisk={}".format(
+                        place, speciesRisk
                     )
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(),
                             record_path=["data"],
                             meta=["lat", "lng"],
                             errors="ignore",
                         )
@@ -632,37 +621,28 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/weather/latest/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    if units != None:
-                        response = requests.get(
-                            "https://api.ambeedata.com/weather/latest/by-lat-lng?lat={}&lng={}&units={}".format(
-                                lat, lng, units
-                            ),
-                            headers=headers,
-                        )
-                    else:
-                        response = requests.get(
-                            "https://api.ambeedata.com/weather/latest/by-lat-lng?lat={}&lng={}".format(
-                                lat, lng
-                            ),
-                            headers=headers,
-                        )
+                    url = base_url + "by-lat-lng?lat={}&lng={}".format(lat, lng)
+                    if units is not None:
+                        url = url + "&units={}".format(units)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json()["data"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
@@ -695,53 +675,32 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/weather/history/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
                     if daily == True:
-                        if units != None:
-                            response = requests.get(
-                                "https://api.ambeedata.com/weather/history/daily/by-lat-lng?lat={}&lng={}&from={}&to={}&units={}".format(
-                                    lat, lng, from_val, to_val, units
-                                ),
-                                headers=headers,
-                            )
-                        else:
-                            response = requests.get(
-                                "https://api.ambeedata.com/weather/history/daily/by-lat-lng?lat={}&lng={}&from={}&to={}".format(
-                                    lat, lng, from_val, to_val
-                                ),
-                                headers=headers,
-                            )
-                    else:
-                        if units != None:
-                            response = requests.get(
-                                "https://api.ambeedata.com/weather/history/by-lat-lng?lat={}&lng={}&from={}&to={}&units={}".format(
-                                    lat, lng, from_val, to_val, units
-                                ),
-                                headers=headers,
-                            )
-                        else:
-                            response = requests.get(
-                                "https://api.ambeedata.com/weather/history/by-lat-lng?lat={}&lng={}&from={}&to={}".format(
-                                    lat, lng, from_val, to_val
-                                ),
-                                headers=headers,
-                            )
+                        base_url = base_url + "daily/"
+                    url = base_url + "by-lat-lng?lat={}&lng={}&from={}&to={}".format(
+                        lat, lng, from_val, to_val
+                    )
+                    if units is not None:
+                        url = url + "&units={}".format(units)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json()["data"],
                             record_path=["history"],
                             meta=["lat", "lng"],
                             errors="ignore",
                         )
@@ -767,53 +726,30 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/weather/forecast/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
                     if daily == True:
-                        if units != None:
-                            response = requests.get(
-                                "https://api.ambeedata.com/weather/forecast/daily/by-lat-lng?lat={}&lng={}&units={}".format(
-                                    lat, lng, units
-                                ),
-                                headers=headers,
-                            )
-                        else:
-                            response = requests.get(
-                                "https://api.ambeedata.com/weather/forecast/daily/by-lat-lng?lat={}&lng={}".format(
-                                    lat, lng
-                                ),
-                                headers=headers,
-                            )
-                    else:
-                        if units != None:
-                            response = requests.get(
-                                "https://api.ambeedata.com/weather/forecast/by-lat-lng?lat={}&lng={}&units={}".format(
-                                    lat, lng, units
-                                ),
-                                headers=headers,
-                            )
-                        else:
-                            response = requests.get(
-                                "https://api.ambeedata.com/weather/forecast/by-lat-lng?lat={}&lng={}".format(
-                                    lat, lng
-                                ),
-                                headers=headers,
-                            )
+                        base_url = base_url + "daily/"
+                    url = base_url + "by-lat-lng?lat={}&lng={}".format(lat, lng)
+                    if units is not None:
+                        url = url + "&units={}".format(units)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json()["data"],
                             record_path=["forecast"],
                             meta=["lat", "lng"],
                             errors="ignore",
                         )
@@ -839,37 +775,28 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/weather/alerts/latest/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    if units != None:
-                        response = requests.get(
-                            "https://api.ambeedata.com/weather/alerts/latest/by-lat-lng?lat={}&lng={}&units={}".format(
-                                lat, lng, units
-                            ),
-                            headers=headers,
-                        )
-                    else:
-                        response = requests.get(
-                            "https://api.ambeedata.com/weather/alerts/latest/by-lat-lng?lat={}&lng={}".format(
-                                lat, lng
-                            ),
-                            headers=headers,
-                        )
+                    url = base_url + "by-lat-lng?lat={}&lng={}".format(lat, lng)
+                    if units is not None:
+                        url = url + "&units={}".format(units)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["data"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
@@ -881,78 +808,114 @@
                 raise InvalidInputError("The call is missing place value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    if units != None:
-                        response = requests.get(
-                            "https://api.ambeedata.com/weather/alerts/latest/by-place?place={}&units={}".format(
-                                place, units
-                            ),
-                            headers=headers,
-                        )
-                    else:
-                        response = requests.get(
-                            "https://api.ambeedata.com/weather/alerts/latest/by-place?place={}".format(
-                                place
-                            ),
-                            headers=headers,
-                        )
+                    url = base_url + "by-place?place={}".format(place)
+                    if units is not None:
+                        url = url + "&units={}".format(units)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["data"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
                     print(response.status_code)
                     raise e
 
 
 class fire(ambee):
     """Contains methods to fetch data from Fire API"""
 
-    def get_latest(self, by, lat=None, lng=None, place=None, return_df=False):
+    def get_latest(
+        self,
+        by,
+        lat=None,
+        lng=None,
+        place=None,
+        coordinates=None,
+        burnedAreaLoc=False,
+        type=None,
+        return_df=False,
+    ):
         """Retrives latest fire data for a given location
 
         Args:
             by (str): signifies the type of input supported by Ambee API. Refer to API Documentation.
             lat (float/int/str, optional): Latitude. Defaults to None.
             lng (float/int/str, optional): Longitude. Defaults to None.
-            place (str, optional): Placename. Defaults to None.
+            place (str, optional): _description_. Defaults to None.
+            coordinates (list, optional): _description_. Defaults to None.
+            burnedAreaLoc (bool, optional): Returns burned area polygon locations if True. Defaults to False.
+            type (str,optional): The type of fire (Reported Fire/ Detected Fire)
             return_df (bool, optional): Converts results to pandas dataframe if True. Defaults to False.
 
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/fire/v2/latest/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/latest/fire?lat={}&lng={}".format(
-                            lat, lng
-                        ),
+                    url = base_url + "by-lat-lng?lat={}&lng={}&burnedAreaLoc={}".format(
+                        lat, lng, burnedAreaLoc
+                    )
+                    if type is not None:
+                        url = url + "type={}".format(type)
+                    response = requests.get(url, headers=headers)
+                    if return_df == True:
+                        try:
+                            return pd.json_normalize(
+                                response.json(), record_path=["result"], errors="ignore"
+                            )
+                        except:
+                            print("Cannot convert to df")
+                            return response.json()
+                    else:
+                        return response.json()
+                except Exception as e:
+                    print(response.status_code)
+                    raise e
+
+        if by == "polygon":
+            if coordinates == None:
+                raise InvalidInputError("The call is missing coordinates")
+            else:
+                try:
+                    headers = {
+                        "x-api-key": self.x_api_key,
+                        "Content-type": "application/json",
+                    }
+                    body = {"coordinates": coordinates}
+                    url = base_url + "by-polygon?burnedAreaLoc={}".format(burnedAreaLoc)
+                    if type is not None:
+                        url = url + "type={}".format(type)
+                    response = requests.post(
+                        url,
                         headers=headers,
+                        json=body,
                     )
                     if return_df == True:
                         try:
                             return pd.json_normalize(
-                                response.json(), record_path=["data"], errors="ignore"
+                                response.json(), record_path=["result"], errors="ignore"
                             )
                         except:
                             print("Cannot convert to df")
                             return response.json()
                     else:
                         return response.json()
                 except Exception as e:
@@ -964,24 +927,72 @@
                 raise InvalidInputError("The call is missing place value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/latest/fire/by-place?place={}".format(
-                            place
-                        ),
-                        headers=headers,
+                    url = base_url + "by-place?place={}&burnedAreaLoc={}".format(
+                        place, burnedAreaLoc
                     )
+                    if type is not None:
+                        url = url + "type={}".format(type)
+                    response = requests.get(url, headers=headers)
+                    if return_df == True:
+                        try:
+                            return pd.json_normalize(
+                                response.json(), record_path=["result"], errors="ignore"
+                            )
+                        except:
+                            print("Cannot convert to df")
+                            return response.json()
+                    else:
+                        return response.json()
+                except Exception as e:
+                    print(response.status_code)
+                    raise e
+
+    def get_forcast(
+        self,
+        by,
+        lat=None,
+        lng=None,
+        return_df=False,
+    ):
+        """Retrives fire danger forecasr for a given location
+
+        Args:
+            by (_type_): _description_
+            lat (_type_, optional): _description_. Defaults to None.
+            lng (_type_, optional): _description_. Defaults to None.
+            return_df (bool, optional): _description_. Defaults to False.
+
+        Raises:
+            InvalidInputError: Raised when the input to query is invalid
+            e: Any exception that occurs during api call and data parsing
+
+        Returns:
+            dict: API response in dictionary format
+        """
+        base_url = "https://api.ambeedata.com/fire/v2/forecast/"
+        if by == "latlng":
+            if lat == None or lng == None:
+                raise InvalidInputError("The call is missing either lat or lng value")
+            else:
+                try:
+                    headers = {
+                        "x-api-key": self.x_api_key,
+                        "Content-type": "application/json",
+                    }
+                    url = base_url + "by-lat-lng?lat={}&lng={}".format(lat, lng)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         try:
                             return pd.json_normalize(
-                                response.json(), record_path=["data"], errors="ignore"
+                                response.json(), record_path=["result"], errors="ignore"
                             )
                         except:
                             print("Cannot convert to df")
                             return response.json()
                     else:
                         return response.json()
                 except Exception as e:
@@ -1004,31 +1015,160 @@
         Raises:
             InvalidInputError: Raised when the input to query is invalid
             e: Any exception that occurs during api call and data parsing
 
         Returns:
             dict: API response in dictionary format
         """
+        base_url = "https://api.ambeedata.com/ndvi/latest/"
         if by == "latlng":
             if lat == None or lng == None:
                 raise InvalidInputError("The call is missing either lat or lng value")
             else:
                 try:
                     headers = {
                         "x-api-key": self.x_api_key,
                         "Content-type": "application/json",
                     }
-                    response = requests.get(
-                        "https://api.ambeedata.com/ndvi/latest/by-lat-lng?lat={}&lng={}".format(
-                            lat, lng
-                        ),
-                        headers=headers,
-                    )
+                    url = base_url + "by-lat-lng?lat={}&lng={}".format(lat, lng)
+                    response = requests.get(url, headers=headers)
                     if return_df == True:
                         return pd.json_normalize(
                             response.json(), record_path=["data"], errors="ignore"
                         )
                     else:
                         return response.json()
                 except Exception as e:
                     print(response.status_code)
                     raise e
+
+
+class natural_disaster(ambee):
+    """Contains methods to fetch data from disasters API"""
+
+    def get_latest(
+        self,
+        by,
+        lat=None,
+        lng=None,
+        alertLevel=None,
+        continent=None,
+        eventType=None,
+        return_df=False,
+    ):
+        """Retrives latest disasters data for a given location
+
+        Args:
+            by (str): signifies the type of input supported by Ambee API. Refer to API Documentation.
+            lat (float/int/str, optional): Latitude. Defaults to None.
+            lng (float/int/str, optional): Longitude. Defaults to None.
+            alertLevel (str, optional): Alert level value should be red, orange or green. Defaults to None.
+            continent (str, optional): Continent value should be afr, ant, asia, aus, eur, nar, sar or ocean. Defaults to None.
+            eventType (str, optional): Event Type value should be tropicalcyclone, flood, volcano, forestfire, drought or earthquake. Defaults to None.
+            return_df (bool, optional): Converts results to pandas dataframe if True. Defaults to False.
+
+        Raises:
+            InvalidInputError: Raised when the input to query is invalid
+            e: Any exception that occurs during api call and data parsing
+
+        Returns:
+            dict: API response in dictionary format
+        """
+        base_url = "https://api.ambeedata.com/disasters/latest/"
+        if by == "latlng":
+            if lat == None or lng == None:
+                raise InvalidInputError("The call is missing either lat or lng value")
+            else:
+                try:
+                    headers = {
+                        "x-api-key": self.x_api_key,
+                        "Content-type": "application/json",
+                    }
+                    url = base_url + "by-lat-lng?lat={}&lng={}".format(lat, lng)
+                    if alertLevel is not None:
+                        url = url + "&alertLevel={}".format(alertLevel)
+                    if continent is not None:
+                        url = url + "&continent={}".format(continent)
+                    if eventType is not None:
+                        url = url + "&eventType={}".format(eventType)
+                    response = requests.get(url, headers=headers)
+                    if return_df == True:
+                        try:
+                            return pd.json_normalize(
+                                response.json(), record_path=["result"], errors="ignore"
+                            )
+                        except:
+                            print("Cannot convert to df")
+                            return response.json()
+                    else:
+                        return response.json()
+                except Exception as e:
+                    print(response.status_code)
+                    raise e
+
+    def get_historical(
+        self,
+        by,
+        from_val,
+        to_val,
+        lat=None,
+        lng=None,
+        alertLevel=None,
+        continent=None,
+        eventType=None,
+        return_df=False,
+    ):
+        """Retrives historical disasters data for a given location
+
+        Args:
+            by (str): signifies the type of input supported by Ambee API. Refer to API Documentation.
+            from_val (str): Start timestamp for historical query
+            to_val (_type_): End timestamp for historical query
+            lat (float/int/str, optional): Latitude. Defaults to None.
+            lng (float/int/str, optional): Longitude. Defaults to None.
+            alertLevel (str, optional): Alert level value should be red, orange or green. Defaults to None.
+            continent (str, optional): Continent value should be afr, ant, asia, aus, eur, nar, sar or ocean. Defaults to None.
+            eventType (str, optional): Event Type value should be tropicalcyclone, flood, volcano, forestfire, drought or earthquake. Defaults to None.
+            return_df (bool, optional): Converts results to pandas dataframe if True. Defaults to False.s
+
+        Raises:
+            InvalidInputError: Raised when the input to query is invalid
+            e: Any exception that occurs during api call and data parsing
+        Returns:
+            dict: API response in dictionary format
+        """
+        base_url = "https://api.ambeedata.com/disasters/history/"
+        if by == "latlng":
+            if lat == None or lng == None:
+                raise InvalidInputError("The call is missing either lat or lng value")
+            else:
+                try:
+                    headers = {
+                        "x-api-key": self.x_api_key,
+                        "Content-type": "application/json",
+                    }
+                    url = base_url + "by-lat-lng?lat={}&lng={}&from={}&to={}".format(
+                        lat,
+                        lng,
+                        from_val,
+                        to_val,
+                    )
+                    if alertLevel is not None:
+                        url = url + "&alertLevel={}".format(alertLevel)
+                    if continent is not None:
+                        url = url + "&continent={}".format(continent)
+                    if eventType is not None:
+                        url = url + "&eventType={}".format(eventType)
+                    response = requests.get(url, headers=headers)
+                    if return_df == True:
+                        try:
+                            return pd.json_normalize(
+                                response.json(), record_path=["result"], errors="ignore"
+                            )
+                        except:
+                            print("Cannot convert to df")
+                            return response.json()
+                    else:
+                        return response.json()
+                except Exception as e:
+                    print(response.status_code)
+                    raise e
```

### Comparing `ambee_sdk-0.1.0a0/ambee_sdk.egg-info/PKG-INFO` & `ambee_sdk-0.1.1/ambee_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ambee-sdk
-Version: 0.1.0a0
+Version: 0.1.1
 Summary: Python SDK for Ambee's APIs
 Home-page: 
 Author: Ambee
 License: MIT
 Keywords: ambee climate environment pollen air-quality weather api sdk
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -21,15 +20,15 @@
 [![Downloads](https://static.pepy.tech/badge/ambee-sdk)](https://pepy.tech/project/ambee-sdk)
 [![Documentation Status](https://readthedocs.org/projects/ambee-sdk/badge/?version=latest)](https://ambee-sdk.readthedocs.io/en/latest/?badge=latest)
 
 Ambee SDK for python provides classes and methods to make use of ambee's APIs inside your python code. You can make calls to our apis, get output in dataframe format, make calls to multiple locations and more.
 
 Read our API documentation: [Ambee: Developers tool](https://docs.ambeedata.com/DeveloperTools/)
 
-Readthedocs - [Welcome to ambee-sdk’s documentation! &mdash; ambee-sdk 0.1.0a documentation](https://ambee-sdk.readthedocs.io/en/latest/index.html)
+Readthedocs - [Welcome to ambee-sdk’s documentation! ](https://ambee-sdk.readthedocs.io/en/latest/index.html)
 
 ## Getting Started
 
 ```py
 import ambee_sdk as ambee
 import datetime
 ```
@@ -38,8 +37,7 @@
 x_api_key = "Your Key Here"
 ```
 
 ```python
 aq = ambee.air_quality(x_api_key=x_api_key)
 aq.get_latest(by='latlng', lat=12, lng=77)
 ```
-
```

### Comparing `ambee_sdk-0.1.0a0/setup.py` & `ambee_sdk-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 long_description = open(os.path.join(here, 'README.md')).read()
 
 setup(
     name="ambee_sdk",
     packages=find_packages(include=["ambee_sdk"]),
-    version="0.1.0a",
+    version="0.1.1",
     author="Ambee",
     license="MIT",
     url='',
     description="Python SDK for Ambee's APIs",
     long_description_content_type="text/markdown",
     long_description=long_description,
     install_requires=[ "requests", "pandas", "geopandas"
```

