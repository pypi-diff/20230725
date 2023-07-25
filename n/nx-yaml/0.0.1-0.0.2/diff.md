# Comparing `tmp/nx_yaml-0.0.1.tar.gz` & `tmp/nx_yaml-0.0.2.tar.gz`

## Comparing `nx_yaml-0.0.1.tar` & `nx_yaml-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nx_yaml-0.0.1/Pipfile
--rw-r--r--   0        0        0    47199 2020-02-02 00:00:00.000000 nx_yaml-0.0.1/Pipfile.lock
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 nx_yaml-0.0.1/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 nx_yaml-0.0.1/nx_yaml.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 nx_yaml-0.0.1/test_nx_yaml.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 nx_yaml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nx_yaml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/Pipfile
+-rw-r--r--   0        0        0    47199 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/Pipfile.lock
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/README.md
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/nx_yaml.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/test_nx_yaml.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/tests/resources/networkx/loop.gml
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/tests/resources/networkx/null.gml
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/tests/resources/networkx/single_node.gml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/tests/resources/yaml/empty.yaml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/tests/resources/yaml/loop.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/tests/resources/yaml/single_node.yaml
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/.gitignore
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nx_yaml-0.0.2/PKG-INFO
```

### Comparing `nx_yaml-0.0.1/Pipfile.lock` & `nx_yaml-0.0.2/Pipfile.lock`

 * *Files identical despite different names*

