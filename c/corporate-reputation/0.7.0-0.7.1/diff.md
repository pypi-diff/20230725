# Comparing `tmp/corporate_reputation-0.7.0.tar.gz` & `tmp/corporate_reputation-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corporate_reputation-0.7.0.tar", max compression
+gzip compressed data, was "corporate_reputation-0.7.1.tar", max compression
```

## Comparing `corporate_reputation-0.7.0.tar` & `corporate_reputation-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-07-24 19:56:19.218549 corporate_reputation-0.7.0/LICENSE
--rw-r--r--   0        0        0     3898 2023-07-24 19:56:19.222549 corporate_reputation-0.7.0/README.md
--rw-r--r--   0        0        0     3045 2023-07-24 19:56:53.906680 corporate_reputation-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      182 2023-07-24 19:56:19.222549 corporate_reputation-0.7.0/src/corprep/__cli__.py
--rw-r--r--   0        0        0      502 2023-07-24 19:56:19.222549 corporate_reputation-0.7.0/src/corprep/__init__.py
--rw-r--r--   0        0        0       22 2023-07-24 19:56:53.862680 corporate_reputation-0.7.0/src/corprep/_version.py
--rw-r--r--   0        0        0        0 2023-07-24 19:56:19.222549 corporate_reputation-0.7.0/src/corprep/absa/__init__.py
--rw-r--r--   0        0        0     1757 2023-07-24 19:56:19.222549 corporate_reputation-0.7.0/src/corprep/absa/agent.py
--rw-r--r--   0        0        0     4793 2023-07-24 19:56:19.222549 corporate_reputation-0.7.0/src/corprep/absa/config.py
--rw-r--r--   0        0        0        0 2023-07-24 19:56:19.222549 corporate_reputation-0.7.0/src/corprep/conf/__init__.py
--rw-r--r--   0        0        0      286 2023-07-24 19:56:19.222549 corporate_reputation-0.7.0/src/corprep/conf/about/corprep.yaml
--rw-r--r--   0        0        0      259 2023-07-24 19:56:19.222549 corporate_reputation-0.7.0/src/corprep/conf/absa/default.yaml
--rw-r--r--   0        0        0     2930 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/conf/absa/prompts/default.yaml
--rw-r--r--   0        0        0      294 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/conf/pipe/absa_agent_predict.yaml
--rw-r--r--   0        0        0      274 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/conf/pipe/dataset_filter.yaml
--rw-r--r--   0        0        0      163 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/conf/pipe/dataset_load_raw.yaml
--rw-r--r--   0        0        0      276 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/conf/pipe/dataset_tokenize.yaml
--rw-r--r--   0        0        0      204 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/datasets/__init__.py
--rw-r--r--   0        0        0     1665 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/datasets/io.py
--rw-r--r--   0        0        0      617 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/datasets/sample.py
--rw-r--r--   0        0        0     1790 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/datasets/similarity.py
--rw-r--r--   0        0        0     1039 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/datasets/tokenize.py
--rw-r--r--   0        0        0        0 2023-07-24 19:56:19.226549 corporate_reputation-0.7.0/src/corprep/py.typed
--rw-r--r--   0        0        0  2355775 2023-07-24 19:56:19.238549 corporate_reputation-0.7.0/src/corprep/resources/dictionaries/mecab/ekon_v1.dic
--rw-r--r--   0        0        0     4811 1970-01-01 00:00:00.000000 corporate_reputation-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-25 00:30:01.415885 corporate_reputation-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3898 2023-07-25 00:30:01.415885 corporate_reputation-0.7.1/README.md
+-rw-r--r--   0        0        0     3045 2023-07-25 00:30:44.408557 corporate_reputation-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/__cli__.py
+-rw-r--r--   0        0        0      484 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-25 00:30:44.352556 corporate_reputation-0.7.1/src/corprep/_version.py
+-rw-r--r--   0        0        0        0 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/absa/__init__.py
+-rw-r--r--   0        0        0     1757 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/absa/agent.py
+-rw-r--r--   0        0        0     4793 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/absa/config.py
+-rw-r--r--   0        0        0        0 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/__init__.py
+-rw-r--r--   0        0        0      286 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/about/corprep.yaml
+-rw-r--r--   0        0        0      259 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/absa/default.yaml
+-rw-r--r--   0        0        0     2930 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/absa/prompts/default.yaml
+-rw-r--r--   0        0        0      294 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/pipe/absa_agent_predict.yaml
+-rw-r--r--   0        0        0      274 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/pipe/dataset_filter.yaml
+-rw-r--r--   0        0        0      163 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/pipe/dataset_load_raw.yaml
+-rw-r--r--   0        0        0      276 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/conf/pipe/dataset_tokenize.yaml
+-rw-r--r--   0        0        0      204 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/__init__.py
+-rw-r--r--   0        0        0     1665 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/io.py
+-rw-r--r--   0        0        0      617 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/sample.py
+-rw-r--r--   0        0        0     1790 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/similarity.py
+-rw-r--r--   0        0        0     1039 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/datasets/tokenize.py
+-rw-r--r--   0        0        0        0 2023-07-25 00:30:01.419885 corporate_reputation-0.7.1/src/corprep/py.typed
+-rw-r--r--   0        0        0  2355775 2023-07-25 00:30:01.435886 corporate_reputation-0.7.1/src/corprep/resources/dictionaries/mecab/ekon_v1.dic
+-rw-r--r--   0        0        0     4811 1970-01-01 00:00:00.000000 corporate_reputation-0.7.1/PKG-INFO
```

### Comparing `corporate_reputation-0.7.0/LICENSE` & `corporate_reputation-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/README.md` & `corporate_reputation-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/pyproject.toml` & `corporate_reputation-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "corporate-reputation"
-version = "0.7.0"
+version = "0.7.1"
 description = "Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/corporate-reputation"
 repository = "https://github.com/entelecheia/corporate-reputation"
 readme = "README.md"
 packages = [{ include = "corprep", from = "src" }]
 
 [tool.poetry.scripts]
 corprep = 'corprep.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.9.2"
+hyfi = "^1.9.3"
 openai = "^0.27.8"
 backoff = "^2.2.1"
 scikit-learn = "^1.3.0"
-lexikanon = "^0.2.2"
+lexikanon = "^0.2.3"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `corporate_reputation-0.7.0/src/corprep/absa/agent.py` & `corporate_reputation-0.7.1/src/corprep/absa/agent.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/src/corprep/absa/config.py` & `corporate_reputation-0.7.1/src/corprep/absa/config.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/src/corprep/conf/absa/prompts/default.yaml` & `corporate_reputation-0.7.1/src/corprep/conf/absa/prompts/default.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/src/corprep/datasets/io.py` & `corporate_reputation-0.7.1/src/corprep/datasets/io.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/src/corprep/datasets/sample.py` & `corporate_reputation-0.7.1/src/corprep/datasets/sample.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/src/corprep/datasets/similarity.py` & `corporate_reputation-0.7.1/src/corprep/datasets/similarity.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/src/corprep/datasets/tokenize.py` & `corporate_reputation-0.7.1/src/corprep/datasets/tokenize.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/src/corprep/resources/dictionaries/mecab/ekon_v1.dic` & `corporate_reputation-0.7.1/src/corprep/resources/dictionaries/mecab/ekon_v1.dic`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.7.0/PKG-INFO` & `corporate_reputation-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: corporate-reputation
-Version: 0.7.0
+Version: 0.7.1
 Summary: Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling
 Home-page: https://entelecheia.github.io/corporate-reputation
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: hyfi (>=1.9.2,<2.0.0)
-Requires-Dist: lexikanon (>=0.2.2,<0.3.0)
+Requires-Dist: hyfi (>=1.9.3,<2.0.0)
+Requires-Dist: lexikanon (>=0.2.3,<0.3.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/corporate-reputation
 Description-Content-Type: text/markdown
 
 # Reputation Analysis of Companies and CEOs
```

