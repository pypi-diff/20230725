# Comparing `tmp/pyreason-1.8.4.tar.gz` & `tmp/pyreason-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.8.4.tar", last modified: Tue Jul 18 13:35:14 2023, max compression
+gzip compressed data, was "pyreason-1.8.5.tar", last modified: Tue Jul 18 13:36:45 2023, max compression
```

## Comparing `pyreason-1.8.4.tar` & `pyreason-1.8.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-18 13:35:03.000000 pyreason-1.8.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 13:35:03.000000 pyreason-1.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-18 13:35:14.621158 pyreason-1.8.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-07-18 13:35:03.000000 pyreason-1.8.4/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    31359 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/facts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/facts/fact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    77308 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5238 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2404 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4552 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/rule_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-07-18 13:35:03.000000 pyreason-1.8.4/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.617158 pyreason-1.8.4/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 13:35:14.000000 pyreason-1.8.4/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:35:14.621158 pyreason-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-18 13:35:03.000000 pyreason-1.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:35:14.621158 pyreason-1.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-18 13:35:03.000000 pyreason-1.8.4/tests/test_hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.414481 pyreason-1.8.5/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-07-18 13:36:29.000000 pyreason-1.8.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 13:36:29.000000 pyreason-1.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-18 13:36:45.414481 pyreason-1.8.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-07-18 13:36:29.000000 pyreason-1.8.5/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.402481 pyreason-1.8.5/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.402481 pyreason-1.8.5/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.406481 pyreason-1.8.5/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31359 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.406481 pyreason-1.8.5/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.406481 pyreason-1.8.5/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.406481 pyreason-1.8.5/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4655 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.406481 pyreason-1.8.5/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/facts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/facts/fact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1011 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.406481 pyreason-1.8.5/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    77010 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.410481 pyreason-1.8.5/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.410481 pyreason-1.8.5/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.410481 pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6241 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6015 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10414 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.410481 pyreason-1.8.5/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2404 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.410481 pyreason-1.8.5/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1188 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.414481 pyreason-1.8.5/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4801 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4551 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/utils/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/utils/rule_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8756 2023-07-18 13:36:29.000000 pyreason-1.8.5/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.402481 pyreason-1.8.5/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-18 13:36:45.000000 pyreason-1.8.5/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-18 13:36:45.000000 pyreason-1.8.5/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:36:45.000000 pyreason-1.8.5/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 13:36:45.000000 pyreason-1.8.5/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 13:36:45.000000 pyreason-1.8.5/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:36:45.414481 pyreason-1.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-18 13:36:29.000000 pyreason-1.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:36:45.414481 pyreason-1.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-18 13:36:29.000000 pyreason-1.8.5/tests/test_hello_world.py
```

### Comparing `pyreason-1.8.4/LICENSE.md` & `pyreason-1.8.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/PKG-INFO` & `pyreason-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.4
+Version: 1.8.5
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.4/README.md` & `pyreason-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/__init__.py` & `pyreason-1.8.5/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.8.5/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.8.5/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.8.5/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/pyreason.py` & `pyreason-1.8.5/pyreason/pyreason.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.8.5/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/args.py` & `pyreason-1.8.5/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/components/world.py` & `pyreason-1.8.5/pyreason/scripts/components/world.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/diffuse.py` & `pyreason-1.8.5/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/facts/fact.py` & `pyreason-1.8.5/pyreason/scripts/facts/fact.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.8.5/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/facts/fact_node.py` & `pyreason-1.8.5/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.8.5/pyreason/scripts/interpretation/interpretation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pyreason.scripts.numba_wrapper.numba_types.world_type as world
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
-import pyreason.scripts.annotation_functions.annotation_functions as ann_fns
 
 import numba
 from numba import objmode, prange
 
 
 # Parallel computing settings
 PARALLEL_COMPUTING = False
@@ -1162,23 +1161,19 @@
 		# Add label to world if it is not there
 		if l not in world.world:
 			world.world[l] = interval.closed(0, 1)
 
 		# Check if update is necessary with previous bnd
 		prev_bnd = world.world[l].copy()
 
-		if l.value == 'normal' or l.value == 'abnormal':
-			world.update_average(l, bnd)
+		# override will not check for inconsistencies
+		if override:
+			world.world[l].set_lower_upper(bnd.lower, bnd.upper)
 		else:
-			# override will not check for inconsistencies
-			if override:
-				world.world[l].set_lower_upper(bnd.lower, bnd.upper)
-			else:
-				world.update_intersection(l, bnd)
-
+			world.update(l, bnd)
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
 			if (save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact') and store_interpretation_changes:
@@ -1255,23 +1250,19 @@
 		# Add label to world if it is not there
 		if l not in world.world:
 			world.world[l] = interval.closed(0, 1)
 
 		# Check if update is necessary with previous bnd
 		prev_bnd = world.world[l].copy()
 
-		if l.value == 'normal' or l.value == 'abnormal':
-			world.update_average(l, bnd)
+		# override will not check for inconsistencies
+		if override:
+			world.world[l].set_lower_upper(bnd.lower, bnd.upper)
 		else:
-			# override will not check for inconsistencies
-			if override:
-				world.world[l].set_lower_upper(bnd.lower, bnd.upper)
-			else:
-				world.update_intersection(l, bnd)
-
+			world.update(l, bnd)
 		world.world[l].set_static(static)
 		if world.world[l]!=prev_bnd:
 			updated = True
 			updated_bnds.append(world.world[l])
 
 			# Add to rule trace if update happened and add to atom trace if necessary
 			if (save_graph_attributes_to_rule_trace or not mode=='graph-attribute-fact') and store_interpretation_changes:
@@ -1528,15 +1519,14 @@
 	for source in sources:
 		for target in targets:
 			edge, new_edge = _add_edge(source, target, neighbors, reverse_neighbors, nodes, edges, l, interpretations_node, interpretations_edge)
 			edges_added.append(edge)
 			changes = changes+1 if new_edge else changes
 	return (edges_added, changes)
 
-
 @numba.njit(cache=CACHEING)
 def _delete_edge(edge, neighbors, reverse_neighbors, edges, interpretations_edge):
 	source, target = edge
 	edges.remove(edge)
 	del interpretations_edge[edge]
 	neighbors[source].remove(target)
 	reverse_neighbors[target].remove(source)
```

### Comparing `pyreason-1.8.4/pyreason/scripts/interval/interval.py` & `pyreason-1.8.5/pyreason/scripts/interval/interval.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.8.5/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,30 +96,19 @@
         result = False
         bnd = world.world[label]
         result = bnd in interval
 
         return result
     return impl
 
-@overload_method(WorldType, 'update_intersection')
-def update_intersection(w, label, bnd):
-    def impl(w, label, bnd):       
+@overload_method(WorldType, 'update')
+def update(w, label, interval):
+    def impl(w, label, interval):       
         current_bnd = w.world[label]
-        new_bnd = current_bnd.intersection(bnd)
-        w.world[label] = new_bnd
-    return impl
-
-@overload_method(WorldType, 'update_average')
-def update_average(w, label, bnd):
-    def impl(w, label, bnd):       
-        current_bnd = w.world[label]
-        if current_bnd.lower == 0 and current_bnd.upper == 1:
-            new_bnd = interval.closed(bnd.lower, bnd.upper)
-        else:
-            new_bnd = interval.closed((bnd.lower + current_bnd.lower)/2, (bnd.upper + current_bnd.upper)/2)
+        new_bnd = current_bnd.intersection(interval)
         w.world[label] = new_bnd
     return impl
 
 @overload_method(WorldType, 'get_bound')
 def get_bound(world, label):
     def impl(world, label):
         result = None
```

### Comparing `pyreason-1.8.4/pyreason/scripts/program/program.py` & `pyreason-1.8.5/pyreason/scripts/program/program.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/rules/rule.py` & `pyreason-1.8.5/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/utils/filter.py` & `pyreason-1.8.5/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.8.5/pyreason/scripts/utils/graphml_parser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 
                 if label.Label(l) not in specific_edge_labels.keys():
                     specific_edge_labels[label.Label(l)] = numba.typed.List.empty_list(numba.types.Tuple((numba.types.string, numba.types.string)))
                 specific_edge_labels[label.Label(l)].append((e[0], e[1]))
                 f = fact_edge.Fact('graph-attribute-fact', (e[0], e[1]), label.Label(l), interval.closed(l_bnd, u_bnd), 0, 0, static=static_facts)
                 facts_edge.append(f)
 
-        return facts_node, facts_edge, specific_node_labels, specific_edge_labels
+        return facts_node, facts_edge, specific_node_labels, specific_edge_labels
```

### Comparing `pyreason-1.8.4/pyreason/scripts/utils/output.py` & `pyreason-1.8.5/pyreason/scripts/utils/output.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/utils/plotter.py` & `pyreason-1.8.5/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/utils/rule_parser.py` & `pyreason-1.8.5/pyreason/scripts/utils/rule_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/utils/visuals.py` & `pyreason-1.8.5/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.8.5/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/pyreason.egg-info/PKG-INFO` & `pyreason-1.8.5/pyreason.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.8.4
+Version: 1.8.5
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
```

### Comparing `pyreason-1.8.4/pyreason.egg-info/SOURCES.txt` & `pyreason-1.8.5/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.8.4/setup.py` & `pyreason-1.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyreason',
-    version='1.8.4',
+    version='1.8.5',
     author='Dyuman Aditya',
     author_email='dyuman.aditya@gmail.com',
     description='An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/lab-v2/pyreason',
     license='BSD 3-clause',
```

### Comparing `pyreason-1.8.4/tests/test_hello_world.py` & `pyreason-1.8.5/tests/test_hello_world.py`

 * *Files identical despite different names*

