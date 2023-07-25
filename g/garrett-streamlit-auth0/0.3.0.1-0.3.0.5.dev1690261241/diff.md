# Comparing `tmp/garrett-streamlit-auth0-0.3.0.1.tar.gz` & `tmp/garrett-streamlit-auth0-0.3.0.5.dev1690261241.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garrett-streamlit-auth0-0.3.0.1.tar", last modified: Tue Jul 25 05:02:40 2023, max compression
+gzip compressed data, was "garrett-streamlit-auth0-0.3.0.5.dev1690261241.tar", last modified: Tue Jul 25 05:00:42 2023, max compression
```

## Comparing `garrett-streamlit-auth0-0.3.0.1.tar` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:02:40.212592 garrett-streamlit-auth0-0.3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 05:02:24.000000 garrett-streamlit-auth0-0.3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 05:02:24.000000 garrett-streamlit-auth0-0.3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-25 05:02:40.212592 garrett-streamlit-auth0-0.3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-25 05:02:24.000000 garrett-streamlit-auth0-0.3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:02:40.204591 garrett-streamlit-auth0-0.3.0.1/auth0_component/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-25 05:02:24.000000 garrett-streamlit-auth0-0.3.0.1/auth0_component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:02:40.200591 garrett-streamlit-auth0-0.3.0.1/auth0_component/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:02:40.204591 garrett-streamlit-auth0-0.3.0.1/auth0_component/frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:02:40.208591 garrett-streamlit-auth0-0.3.0.1/auth0_component/frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 05:02:39.000000 garrett-streamlit-auth0-0.3.0.1/auth0_component/frontend/dist/assets/index.1dbfa948.css
--rw-r--r--   0 runner    (1001) docker     (123)   337632 2023-07-25 05:02:39.000000 garrett-streamlit-auth0-0.3.0.1/auth0_component/frontend/dist/assets/index.84bf3e3f.js
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-25 05:02:39.000000 garrett-streamlit-auth0-0.3.0.1/auth0_component/frontend/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:02:40.212592 garrett-streamlit-auth0-0.3.0.1/garrett_streamlit_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-25 05:02:40.000000 garrett-streamlit-auth0-0.3.0.1/garrett_streamlit_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-25 05:02:40.000000 garrett-streamlit-auth0-0.3.0.1/garrett_streamlit_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:02:40.000000 garrett-streamlit-auth0-0.3.0.1/garrett_streamlit_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 05:02:40.000000 garrett-streamlit-auth0-0.3.0.1/garrett_streamlit_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 05:02:40.000000 garrett-streamlit-auth0-0.3.0.1/garrett_streamlit_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 05:02:24.000000 garrett-streamlit-auth0-0.3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:02:40.212592 garrett-streamlit-auth0-0.3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-25 05:02:24.000000 garrett-streamlit-auth0-0.3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.024566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.016566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 05:00:41.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/index.1dbfa948.css
+-rw-r--r--   0 runner    (1001) docker     (123)   337632 2023-07-25 05:00:41.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/index.84bf3e3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-25 05:00:41.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:00:42.028566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 05:00:42.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/garrett_streamlit_auth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:00:42.032566 garrett-streamlit-auth0-0.3.0.5.dev1690261241/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-25 05:00:29.000000 garrett-streamlit-auth0-0.3.0.5.dev1690261241/setup.py
```

### Comparing `garrett-streamlit-auth0-0.3.0.1/LICENSE` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/LICENSE`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.0.1/README.md` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/README.md`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.0.1/auth0_component/__init__.py` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/__init__.py`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.0.1/auth0_component/frontend/dist/assets/index.1dbfa948.css` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/index.1dbfa948.css`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.0.1/auth0_component/frontend/dist/assets/index.84bf3e3f.js` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/auth0_component/frontend/dist/assets/index.84bf3e3f.js`

 * *Files identical despite different names*

### Comparing `garrett-streamlit-auth0-0.3.0.1/setup.py` & `garrett-streamlit-auth0-0.3.0.5.dev1690261241/setup.py`

 * *Files identical despite different names*

