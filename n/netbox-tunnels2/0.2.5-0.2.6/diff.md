# Comparing `tmp/netbox-tunnels2-0.2.5.tar.gz` & `tmp/netbox-tunnels2-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-tunnels2-0.2.5.tar", last modified: Fri Jun 23 18:41:30 2023, max compression
+gzip compressed data, was "netbox-tunnels2-0.2.6.tar", last modified: Tue Jul 25 16:47:57 2023, max compression
```

## Comparing `netbox-tunnels2-0.2.5.tar` & `netbox-tunnels2-0.2.6.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.506685 netbox-tunnels2-0.2.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.506685 netbox-tunnels2-0.2.5/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/docs/img/tunnel-info.png
--rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/docs/img/tunnel-list.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.506685 netbox-tunnels2-0.2.5/netbox_tunnels2/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.506685 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.687743 netbox-tunnels2-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-07-25 16:47:57.687743 netbox-tunnels2-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.675743 netbox-tunnels2-0.2.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.679743 netbox-tunnels2-0.2.6/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/docs/img/tunnel-info.png
+-rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/docs/img/tunnel-list.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.679743 netbox-tunnels2-0.2.6/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.683743 netbox-tunnels2-0.2.6/netbox_tunnels2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.683743 netbox-tunnels2-0.2.6/netbox_tunnels2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/migrations/0003_tunnel_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.675743 netbox-tunnels2-0.2.6/netbox_tunnels2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.683743 netbox-tunnels2-0.2.6/netbox_tunnels2/templates/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.683743 netbox-tunnels2-0.2.6/netbox_tunnels2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/tests/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/netbox_tunnels2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:47:57.683743 netbox-tunnels2-0.2.6/netbox_tunnels2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-07-25 16:47:57.000000 netbox-tunnels2-0.2.6/netbox_tunnels2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-25 16:47:57.000000 netbox-tunnels2-0.2.6/netbox_tunnels2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:47:57.000000 netbox-tunnels2-0.2.6/netbox_tunnels2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 16:47:57.000000 netbox-tunnels2-0.2.6/netbox_tunnels2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 16:47:57.000000 netbox-tunnels2-0.2.6/netbox_tunnels2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-25 16:47:57.687743 netbox-tunnels2-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-25 16:47:43.000000 netbox-tunnels2-0.2.6/setup.py
```

### Comparing `netbox-tunnels2-0.2.5/CONTRIBUTING.md` & `netbox-tunnels2-0.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/LICENSE` & `netbox-tunnels2-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/PKG-INFO` & `netbox-tunnels2-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `netbox-tunnels2-0.2.5/README.md` & `netbox-tunnels2-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/docs/img/tunnel-info.png` & `netbox-tunnels2-0.2.6/docs/img/tunnel-info.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/docs/img/tunnel-list.png` & `netbox-tunnels2-0.2.6/docs/img/tunnel-list.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/__init__.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/api/serializers.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
     side_b_assigned_object = serializers.SerializerMethodField(read_only=True)
     class Meta:
         model = Tunnel
         fields = (
             'id', 
             'url', 
             'display', 
-            'name', 
+            'name',
+            'tenant',
             'a_pub_address', 
             'b_pub_address', 
             'side_a_assigned_object_type',
             'side_a_assigned_object_id',
             'side_a_assigned_object',
             'side_b_assigned_object_type',
             'side_b_assigned_object_id',
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/api/views.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/filtersets.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/filtersets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import django_filters
 from netbox.filtersets import NetBoxModelFilterSet
 from dcim.models import Interface
+from tenancy.models import Tenant
 from .models import Tunnel, TunnelType
 
 
 class TunnelFilterSet(NetBoxModelFilterSet):
     side_a_interface = django_filters.ModelMultipleChoiceFilter(
         field_name="interface__name",
         queryset=Interface.objects.all(),
@@ -23,30 +24,39 @@
         label="Side B Interface (name)",
     )
     side_b_interface_id = django_filters.ModelMultipleChoiceFilter(
         field_name="interface",
         queryset=Interface.objects.all(),
         label="Side B Interface (ID)",
     )
+    tenant_id = django_filters.ModelChoiceFilter(
+        field_name="tenant_id",
+        queryset=Tenant.objects.all(),
+        to_field_name="id",
+        label="Tenant (ID)",
+    )
+
     class Meta:
         model = Tunnel
         fields = (
             "name",
             "status",
             "tunnel_type",
             "a_pub_address",
             "b_pub_address",
             "side_a_interface",
             "side_a_interface_id",
             "side_b_interface",
             "side_b_interface_id",
         )
+
     def search(self, queryset, name, value):
         return queryset.filter(description__icontains=value)
-    
+
+
 class TunnelTypeFilterSet(NetBoxModelFilterSet):
     class Meta:
         model = TunnelType
         fields = (
             "name",
             "slug"
         )
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/forms.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from dcim.models import Interface, Device
 from ipam.models import IPAddress, VRF
 from ipam.formfields import IPNetworkFormField
 from django.core.exceptions import MultipleObjectsReturned, ObjectDoesNotExist, ValidationError
 from django.contrib.contenttypes.models import ContentType
 
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm
+from tenancy.models import Tenant
 
 from .models import Tunnel, TunnelStatusChoices, TunnelType
 
 class TunnelEditForm(NetBoxModelForm):
     """Form for creating a new tunnel."""
 
     name = CharField(required=True, label="Name", help_text="Name of tunnel")
@@ -33,52 +34,70 @@
             required=False
         )
 
     tunnel_type = ModelChoiceField(
             queryset=TunnelType.objects.all(),
             required=True
     )
-    a_pub_VRF = DynamicModelChoiceField(label='Side A Address VRF', queryset=VRF.objects.all(),required=False)
+    a_pub_VRF = DynamicModelChoiceField(
+        label='Side A Address VRF',
+        queryset=VRF.objects.all(),
+        required=False,
+        selector=True,
+        query_params={
+            "tenant_id": "$tenant",
+        },
+    )
     a_pub_address = DynamicModelChoiceField(
         label='Side A Public IP Address',
         queryset=IPAddress.objects.all(),
         query_params={
             'vrf_id': '$a_pub_VRF',
-            'device_id':'$side_a_device'
+            'device_id': '$side_a_device'
         }
     )
-    b_pub_VRF = DynamicModelChoiceField(label='Side B Address VRF', queryset=VRF.objects.all(),required=False)
+    b_pub_VRF = DynamicModelChoiceField(
+        label='Side B Address VRF',
+        queryset=VRF.objects.all(),
+        selector=True,
+        required=False
+    )
     b_pub_address = DynamicModelChoiceField(
         label='Side B Public IP Address',
         queryset=IPAddress.objects.all(),
         query_params={
             'vrf_id': '$side_b_device',
-            'device_id':'$side_b_device'
+            'device_id': '$side_b_device'
         },
         required=False
     )
     psk = CharField(required=False, label="Pre-shared Key", help_text="Pre-shared key")
 
     side_a_device = DynamicModelChoiceField(
         queryset=Device.objects.all(),
         label="Site A Device",
-        required=False
+        required=False,
+        selector=True,
+        query_params={
+            "tenant_id": "$tenant",
+        },
     )
     side_a_interface = DynamicModelChoiceField(
         queryset=Interface.objects.all(),
         label="Site A Interface",
         required=False,
         query_params={
             "device_id": "$side_a_device",
         },
     )
     side_b_device = DynamicModelChoiceField(
         queryset=Device.objects.all(),
         label="Site B Device",
-        required=False
+        required=False,
+        selector=True,
     )
     side_b_interface = DynamicModelChoiceField(
         queryset=Interface.objects.all(),
         label="Site B Interface",
         required=False,
         query_params={
             "device_id": "$side_b_device",
@@ -109,14 +128,15 @@
             "status",
             "tunnel_type",
             "a_pub_address",
             "b_pub_address",
             "psk",
             'comments',
             'tags',
+            'tenant',
         )
     def clean(self):
         cleaned_data = super().clean()
         error_message = {}
         name = cleaned_data.get("name")
         status = cleaned_data.get("status")
         tunnel_type = cleaned_data.get("tunnel_type")
@@ -168,23 +188,25 @@
             "a_pub_VRF",
             "a_pub_address",
             "b_pub_VRF",
             "b_pub_address",
             "psk",
             "comments",
             "tags",
+            "tenant",
         )
     field_order = ["name",
             "status",
             "tunnel_type",
             "a_pub_VRF",
             "a_pub_address",
             "b_pub_VRF",
             "b_pub_address",
             "psk",
+            "tenant",
             "comments",
             "tags"]
     
     def clean_b_pub_address(self):
         
         if self.data['remote_VRF']!='':
             vrf=VRF.objects.get(id=self.data['remote_VRF'])
@@ -208,36 +230,40 @@
         self.cleaned_data['b_pub_address'] = ip
         return self.cleaned_data['b_pub_address']
     
 class TunnelFilterForm(NetBoxModelFilterSetForm):
     """Form for filtering Tunnel instances."""
     model = Tunnel
     status = MultipleChoiceField(choices=TunnelStatusChoices, required=False)
-    tunnel_type = tunnel_type = ModelChoiceField(
+    tunnel_type = ModelChoiceField(
             queryset=TunnelType.objects.all(),
             required=False
     )
     a_pub_address = DynamicModelMultipleChoiceField(
         queryset=IPAddress.objects.all(),
         required=False,
         label="Local Address",
     )
     b_pub_address = DynamicModelMultipleChoiceField(
         queryset=IPAddress.objects.all(),
         required=False,
         label="Remote Address",
     )
+    tenant_id = DynamicModelMultipleChoiceField(
+        required=False, queryset=Tenant.objects.all(), label="Tenant"
+    )
     class Meta:
         """Class to define what is used for filtering tunnels with the search box."""
         model = Tunnel
         fields = (
             "a_pub_address",
             "b_pub_address",
             "psk",
             "tunnel_type",
+            "tenant_id",
         )
 
 #
 # Tunnel Type
 #
 
 class TunnelTypeEditForm(NetBoxModelForm):
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/graphql.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/0001_initial.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,8 @@
                 ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
                 ('tunnel_type', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, related_name='tunnels', to='netbox_tunnels2.tunneltype')),
             ],
             options={
                 'verbose_name_plural': 'Tunnels',
             },
         ),
-    ]
+    ]
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/models.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from django.db import models
 from django.urls import reverse
 from django.contrib.contenttypes.models import ContentType
 from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 
 from netbox.models import NetBoxModel, OrganizationalModel
 from utilities.querysets import RestrictedQuerySet
+from tenancy.models import Tenant
 from .constants import TUNNEL_INTERFACE_ASSIGNMENT_MODELS
 
 from dcim.models import Device, Interface
 
 
 
 
@@ -112,14 +113,20 @@
         null=True,
         blank=True
     )
     description = models.CharField(
         max_length=200,
         blank=True
     )
+    tenant = models.ForeignKey(
+        to=Tenant,
+        on_delete=models.RESTRICT,
+        null=True,
+        blank=True
+    )
     psk = models.CharField(verbose_name="Pre-shared Key", max_length=100, blank=True)
     comments = models.TextField(blank=True)
 
     class Meta:
         """Class to define what will be used to set order based on. Will be using the unique tunnel ID for this purpose."""
         verbose_name_plural='Tunnels'
     def __str__(self):
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/navigation.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/tables.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,19 @@
  """
 
 class TunnelTable(NetBoxTable):
     """Table for displaying configured Tunnel instances."""
     name = tables.Column(
         linkify=True
     )
-    tunnel_type=tables.Column(linkify=True)
+    tunnel_type = tables.Column(linkify=True)
     a_pub_address = tables.Column(linkify=True)
     b_pub_address = tables.Column(linkify=True)
     status = ChoiceFieldColumn()
+    tenant = tables.Column(linkify=True)
 
     side_a_host = tables.TemplateColumn(
         template_code=COL_SIDE_A_HOST_ASSIGNMENT,
         verbose_name="Side A Host",
     )
     side_a_assigned_object = tables.Column(
         linkify=True,
@@ -53,24 +54,25 @@
     side_b_host = tables.TemplateColumn(
         template_code=COL_SIDE_B_HOST_ASSIGNMENT,
         verbose_name="Side B Host",
     )
     side_b_assigned_object = tables.Column(
         linkify=True,
         orderable=False,
-        verbose_name="Side ABInterface",
+        verbose_name="Side B Interface",
     )
     class Meta(NetBoxTable.Meta):
         """Class to define what is used for tunnel_lists.html template to show configured tunnels."""
 
         model = Tunnel
         fields = (
             'pk',
             'id',
             "name",
+            "tenant",
             "tunnel_type",
             "side_a_host",
             "side_a_assigned_object",
             "side_b_host",
             "side_b_assigned_object",
             "status",
             "a_pub_address",
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html` & `netbox-tunnels2-0.2.6/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,31 @@
             </tr>
             <tr>
               <th scope="row">Status</th>
               <td>{% badge object.get_status_display bg_color=object.get_status_color %}</td>
             </tr>
             <tr>
               <th scope="row">Tunnel Type</th>
-              <td><a href="{{ object.tunnel_type.get_absolute_url }}">{{ object.tunnel_type }}</a></td>
+              <td>{{ object.tunnel_type|linkify|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Local Address</th>
-              <td><a href="{{ object.a_pub_address.get_absolute_url }}">{{ object.a_pub_address }}</a></td>
+              <td>{{ object.a_pub_address|linkify|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Remote Address</th>
-              <td><a href="{{ object.b_pub_address.get_absolute_url }}">{{ object.b_pub_address }}</a></td>
+              <td>{{ object.b_pub_address|linkify|placeholder }}</td>
             </tr>
             <tr>
               <th scope="row">Pre Shared Key</th>
-              <td>{{ object.psk }}</td>
+              <td>{{ object.psk|placeholder }}</td>
+            </tr>
+            <tr>
+              <th scope="row">Tenant</th>
+              <td>{{ object.tenant|linkify|placeholder }}</td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
       {% plugin_left_page object %}
     </div>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
 {% extends 'generic/object.html' %} {% load plugins %} {% block content %}
 ** Tunnel **
 Name           {{ object.name }}
 Status         {% badge object.get_status_display
                bg_color=object.get_status_color %}
-Tunnel Type    {{_object.tunnel_type_}}
-Local Address  {{_object.a_pub_address_}}
-Remote Address {{_object.b_pub_address_}}
-Pre Shared Key {{ object.psk }}
+Tunnel Type    {{ object.tunnel_type|linkify|placeholder }}
+Local Address  {{ object.a_pub_address|linkify|placeholder }}
+Remote Address {{ object.b_pub_address|linkify|placeholder }}
+Pre Shared Key {{ object.psk|placeholder }}
+Tenant         {{ object.tenant|linkify|placeholder }}
 {% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% plugin_right_page object %}
 ** Endpoints **
 Side A Device                                    Side A Inside Interface                   Side B Device                                    Side B Inside Interface
 {                                                {                                         {                                                {
 {                                                {                                         {                                                {
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html` & `netbox-tunnels2-0.2.6/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 {% extends 'generic/object_edit.html' %}
 {% load static %}
 {% load form_helpers %}
 
-{% block title %}{% if obj.pk %}Editing {{ obj }}{% else %}Add a tunnel{% endif %}{% endblock %}
-
 {% block form %}
 {% render_errors form %}
 <div class="field-group">
   <h4>Tunnel Details</h4>
   {% render_field form.name %}
   {% render_field form.status %}
   {% render_field form.tunnel_type %}
   {% render_field form.a_pub_VRF %}
   {% render_field form.a_pub_address %}
   {% render_field form.b_pub_VRF %}
   {% render_field form.b_pub_address %}
   {% render_field form.psk %}
+  {% render_field form.tenant %}
 </div>
 <div class="field-group">
     <h4>Side A Interface Assignment</h4>
     <div class="tab-content">
         <div class="tab-pane{% if not form.initial.side_a_virtual_chassis and not form.initial.side_a_virtual_machine %} active{% endif %}" id="deviceA">
             {% render_field form.side_a_device %}
             {% render_field form.side_a_interface %}
@@ -33,21 +32,19 @@
         <div class="tab-pane{% if not form.initial.side_b_virtual_chassis and not form.initial.side_b_virtual_machine %} active{% endif %}" id="deviceB">
             {% render_field form.side_b_device %}
             {% render_field form.side_b_interface %}
         </div>
     </div>
 </div>
 
+{% if form.custom_fields %}
+    <div class="field-group">
+        <h4>Custom Fields</h4>
+            {% render_custom_fields form %}
+    </div>
+{% endif %}
 
 <div class="field-group">
     <h4>Comments</h4>
     {% render_field form.comments %}
 </div>
-{% if form.custom_fields %}
-    <div class="card">
-        <h5 class="card-header">Custom Fields</h5>
-        <div class="card-body">
-            {% render_custom_fields form %}
-        </div>
-    </div>
-{% endif %}
 {% endblock %}
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html` & `netbox-tunnels2-0.2.6/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/tests/custom.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/tests/test_models.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/tests/test_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from django.core.exceptions import ValidationError
 from django.db import IntegrityError, transaction
 from django.test import TestCase
 
 from netbox_tunnels2.models import Tunnel, TunnelType
 from ipam.models import IPAddress
+from tenancy.models.tenants import Tenant
 
 class TunnelTestCase(TestCase):
     def setUp(self):
         self.tunnelType1 = TunnelType.objects.create(name='GRE', slug='gre')
         self.tunnelType2 = TunnelType.objects.create(name='IPSec Tunnel', slug='ipsec')
         self.ipAddressA = IPAddress.objects.create(address='1.0.0.1/32')
         self.ipAddressB = IPAddress.objects.create(address='1.0.0.2/32')
+        self.tenant = Tenant.objects.create(name='TestTenant')
     def test_tunnel_creation(self):
-        tunnel1=Tunnel.objects.create(name='Test Tunnel1', tunnel_type=self.tunnelType1, a_pub_address=self.ipAddressA)
+        tunnel1 = Tunnel.objects.create(name='Test Tunnel1',
+                                      tunnel_type=self.tunnelType1,
+                                      a_pub_address=self.ipAddressA,
+                                      tenant=self.tenant)
         tunnel1.full_clean()
         self.assertEqual(tunnel1.a_pub_address, self.ipAddressA)
+        self.assertEqual(tunnel1.tenant, self.tenant)
 
 
         # Tests an (invalid) Null for a_pub_address
         with self.assertRaises(IntegrityError):
             with transaction.atomic():
                 Tunnel.objects.create(name='Test Tunnel2', tunnel_type=self.tunnelType1, b_pub_address=self.ipAddressA)
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/urls.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2/views.py` & `netbox-tunnels2-0.2.6/netbox_tunnels2/views.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/PKG-INFO` & `netbox-tunnels2-0.2.6/netbox_tunnels2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/SOURCES.txt` & `netbox-tunnels2-0.2.6/netbox_tunnels2.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 netbox_tunnels2.egg-info/top_level.txt
 netbox_tunnels2/api/__init__.py
 netbox_tunnels2/api/serializers.py
 netbox_tunnels2/api/urls.py
 netbox_tunnels2/api/views.py
 netbox_tunnels2/migrations/0001_initial.py
 netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py
+netbox_tunnels2/migrations/0003_tunnel_tenant.py
 netbox_tunnels2/migrations/__init__.py
 netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
 netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
 netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
 netbox_tunnels2/tests/__init__.py
 netbox_tunnels2/tests/custom.py
 netbox_tunnels2/tests/test_api.py
```

### Comparing `netbox-tunnels2-0.2.5/pyproject.toml` & `netbox-tunnels2-0.2.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-tunnels2"
-version = "0.2.5"
+version = "0.2.6"
 description = "Provides the ability track IP Tunnels."
 readme = "README.md"
 authors = [{ name = "Robert Lynch", email = "robertlynch3@users.noreply.github.com" }]
 license = { file = "LICENSE" }
 
 [project.urls]
 Homepage = "https://github.com/robertlynch3/netbox-tunnels2"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
-current_version = "0.2.5"
+current_version = "0.2.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
-commit = true
-tag = true
-push = true
+commit = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"$',
     'version = "{version}"$',
 ]
 "netbox_tunnels2/version.py" = [
```

### Comparing `netbox-tunnels2-0.2.5/setup.cfg` & `netbox-tunnels2-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.5/setup.py` & `netbox-tunnels2-0.2.6/setup.py`

 * *Files identical despite different names*

