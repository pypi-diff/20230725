# Comparing `tmp/lamin_utils-0.9.2.tar.gz` & `tmp/lamin_utils-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_utils-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_utils-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_utils-0.9.2.tar` & `lamin_utils-0.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      977 2023-07-23 09:54:55.938805 lamin_utils-0.9.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-07-23 09:54:55.938918 lamin_utils-0.9.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-07-23 09:54:55.939014 lamin_utils-0.9.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-07-23 09:54:55.939121 lamin_utils-0.9.2/.gitignore
--rw-r--r--   0        0        0     1798 2023-07-23 09:54:55.939232 lamin_utils-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2023-07-23 09:54:55.939391 lamin_utils-0.9.2/LICENSE
--rw-r--r--   0        0        0      176 2023-07-23 09:54:55.939490 lamin_utils-0.9.2/README.md
--rw-r--r--   0        0        0     6518 2023-07-25 14:10:30.979172 lamin_utils-0.9.2/docs/changelog.md
--rw-r--r--   0        0        0     1359 2023-07-23 14:46:35.798941 lamin_utils-0.9.2/docs/quickstart.ipynb
--rw-r--r--   0        0        0      149 2023-07-23 09:54:55.939845 lamin_utils-0.9.2/lamin-project.yaml
--rw-r--r--   0        0        0      161 2023-07-25 14:10:22.384361 lamin_utils-0.9.2/lamin_utils/__init__.py
--rw-r--r--   0        0        0     1632 2023-07-25 14:09:10.077910 lamin_utils-0.9.2/lamin_utils/_core.py
--rw-r--r--   0        0        0     3825 2023-07-23 09:54:55.940185 lamin_utils-0.9.2/lamin_utils/_inspect.py
--rw-r--r--   0        0        0     7393 2023-07-23 09:54:55.940290 lamin_utils-0.9.2/lamin_utils/_logger.py
--rw-r--r--   0        0        0     4282 2023-07-23 14:49:00.466496 lamin_utils-0.9.2/lamin_utils/_lookup.py
--rw-r--r--   0        0        0     7410 2023-07-23 09:54:55.940498 lamin_utils-0.9.2/lamin_utils/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-07-23 09:54:55.940588 lamin_utils-0.9.2/lamin_utils/_python_version.py
--rw-r--r--   0        0        0     3609 2023-07-23 09:54:55.940683 lamin_utils-0.9.2/lamin_utils/_search.py
--rw-r--r--   0        0        0      285 2023-07-23 09:54:55.940763 lamin_utils-0.9.2/noxfile.py
--rw-r--r--   0        0        0      896 2023-07-23 09:54:55.940837 lamin_utils-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      114 2023-07-23 09:54:55.940955 lamin_utils-0.9.2/tests/test_base.py
--rw-r--r--   0        0        0     4153 2023-07-23 09:54:55.941046 lamin_utils-0.9.2/tests/test_inspect.py
--rw-r--r--   0        0        0     1607 2023-07-23 09:54:55.941146 lamin_utils-0.9.2/tests/test_lookup.py
--rw-r--r--   0        0        0     6152 2023-07-23 09:54:55.941242 lamin_utils-0.9.2/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-07-23 09:54:55.941327 lamin_utils-0.9.2/tests/test_notebooks.py
--rw-r--r--   0        0        0     2449 2023-07-23 09:54:55.941414 lamin_utils-0.9.2/tests/test_search.py
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 lamin_utils-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      977 2023-07-23 09:54:55.938805 lamin_utils-0.9.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-07-23 09:54:55.938918 lamin_utils-0.9.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-07-23 09:54:55.939014 lamin_utils-0.9.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-07-23 09:54:55.939121 lamin_utils-0.9.3/.gitignore
+-rw-r--r--   0        0        0     1798 2023-07-23 09:54:55.939232 lamin_utils-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2023-07-23 09:54:55.939391 lamin_utils-0.9.3/LICENSE
+-rw-r--r--   0        0        0      176 2023-07-23 09:54:55.939490 lamin_utils-0.9.3/README.md
+-rw-r--r--   0        0        0     6671 2023-07-25 19:58:24.969203 lamin_utils-0.9.3/docs/changelog.md
+-rw-r--r--   0        0        0     1359 2023-07-23 14:46:35.798941 lamin_utils-0.9.3/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      149 2023-07-23 09:54:55.939845 lamin_utils-0.9.3/lamin-project.yaml
+-rw-r--r--   0        0        0      161 2023-07-25 19:58:18.819710 lamin_utils-0.9.3/lamin_utils/__init__.py
+-rw-r--r--   0        0        0     1632 2023-07-25 14:09:10.077910 lamin_utils-0.9.3/lamin_utils/_core.py
+-rw-r--r--   0        0        0     3825 2023-07-23 09:54:55.940185 lamin_utils-0.9.3/lamin_utils/_inspect.py
+-rw-r--r--   0        0        0     7393 2023-07-23 09:54:55.940290 lamin_utils-0.9.3/lamin_utils/_logger.py
+-rw-r--r--   0        0        0     4282 2023-07-23 14:49:00.466496 lamin_utils-0.9.3/lamin_utils/_lookup.py
+-rw-r--r--   0        0        0     7526 2023-07-25 19:58:03.772477 lamin_utils-0.9.3/lamin_utils/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-07-23 09:54:55.940588 lamin_utils-0.9.3/lamin_utils/_python_version.py
+-rw-r--r--   0        0        0     3609 2023-07-23 09:54:55.940683 lamin_utils-0.9.3/lamin_utils/_search.py
+-rw-r--r--   0        0        0      285 2023-07-23 09:54:55.940763 lamin_utils-0.9.3/noxfile.py
+-rw-r--r--   0        0        0      896 2023-07-23 09:54:55.940837 lamin_utils-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-07-23 09:54:55.940955 lamin_utils-0.9.3/tests/test_base.py
+-rw-r--r--   0        0        0     4153 2023-07-23 09:54:55.941046 lamin_utils-0.9.3/tests/test_inspect.py
+-rw-r--r--   0        0        0     1607 2023-07-23 09:54:55.941146 lamin_utils-0.9.3/tests/test_lookup.py
+-rw-r--r--   0        0        0     6152 2023-07-23 09:54:55.941242 lamin_utils-0.9.3/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-07-23 09:54:55.941327 lamin_utils-0.9.3/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2449 2023-07-23 09:54:55.941414 lamin_utils-0.9.3/tests/test_search.py
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 lamin_utils-0.9.3/PKG-INFO
```

### Comparing `lamin_utils-0.9.2/.github/workflows/build.yml` & `lamin_utils-0.9.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/.github/workflows/latest-changes.yml` & `lamin_utils-0.9.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/.gitignore` & `lamin_utils-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/.pre-commit-config.yaml` & `lamin_utils-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/LICENSE` & `lamin_utils-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/docs/changelog.md` & `lamin_utils-0.9.3/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Fix for categorical index | [45](https://github.com/laminlabs/lamin-utils/pull/45) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-25 | 0.9.3
 ✨ Added italic and underline | [44](https://github.com/laminlabs/lamin-utils/pull/44) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-25 | 0.9.2
 🐛 Fix _append_records_to_list in lookup | [43](https://github.com/laminlabs/lamin-utils/pull/43) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-23 |
 ✨ Allow indenting logging messages | [42](https://github.com/laminlabs/lamin-utils/pull/42) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 | 0.9.0
 💚 Fix | [41](https://github.com/laminlabs/lamin-utils/pull/41) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 |
 🚚 Rename `lamin_logger` to `lamin_utils` | [40](https://github.com/laminlabs/lamin-utils/pull/40) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 |
 🎨 Fix for duplicated values in search | [39](https://github.com/laminlabs/lamin-logger/pull/39) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-19 |
 🎨 Return None if searching against Nones | [38](https://github.com/laminlabs/lamin-logger/pull/38) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-18 |
```

### Comparing `lamin_utils-0.9.2/docs/quickstart.ipynb` & `lamin_utils-0.9.3/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/lamin_utils/_core.py` & `lamin_utils-0.9.3/lamin_utils/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/lamin_utils/_inspect.py` & `lamin_utils-0.9.3/lamin_utils/_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/lamin_utils/_logger.py` & `lamin_utils-0.9.3/lamin_utils/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/lamin_utils/_lookup.py` & `lamin_utils-0.9.3/lamin_utils/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/lamin_utils/_map_synonyms.py` & `lamin_utils-0.9.3/lamin_utils/_map_synonyms.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,16 +114,20 @@
         else:
             return mapped_list
 
 
 def to_str(identifiers: Any, case_sensitive: bool = False):
     """Convert a pandas series values to strings with case sensitive option."""
     if identifiers.dtype.name == "category":
-        if "" not in identifiers.cat.categories:
-            values = identifiers.cat.add_categories("")
+        try:
+            categorical = identifiers.cat
+        except AttributeError:
+            categorical = identifiers
+        if "" not in categorical.categories:
+            values = categorical.add_categories("")
         else:
             values = identifiers
         values = values.fillna("").astype(str)
     else:
         values = identifiers.fillna("")
     if case_sensitive is False:
         values = values.str.lower()
```

### Comparing `lamin_utils-0.9.2/lamin_utils/_python_version.py` & `lamin_utils-0.9.3/lamin_utils/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/lamin_utils/_search.py` & `lamin_utils-0.9.3/lamin_utils/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/pyproject.toml` & `lamin_utils-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/tests/test_inspect.py` & `lamin_utils-0.9.3/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/tests/test_lookup.py` & `lamin_utils-0.9.3/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/tests/test_map_synonyms.py` & `lamin_utils-0.9.3/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/tests/test_search.py` & `lamin_utils-0.9.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_utils-0.9.2/PKG-INFO` & `lamin_utils-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_utils
-Version: 0.9.2
+Version: 0.9.3
 Summary: Lamin Utils.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

