# Comparing `tmp/drf_misc-0.2.0.tar.gz` & `tmp/drf_misc-0.2.1.tar.gz`

## Comparing `drf_misc-0.2.0.tar` & `drf_misc-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.isort.cfg
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.pylintrc
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-0.2.0/ignore-spelling-words.txt
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-0.2.0/mypy.ini
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-0.2.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.2.0/setup.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/__init__.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/admin.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/apps.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/settings.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/api_exceptions.py
--rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/api_views.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/audit_service.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/cache.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/fields.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/filter_backend.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/middlewares.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/models.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/paginations.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/parsers.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/permissions.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/serializers.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/services.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/core/throttling.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/decorators.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/epoch_util.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/misc.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 drf_misc-0.2.0/drf_misc/utility/validator.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 drf_misc-0.2.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-0.2.0/LICENSE
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 drf_misc-0.2.0/README.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 drf_misc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 drf_misc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 drf_misc-0.2.1/.isort.cfg
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 drf_misc-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20793 2020-02-02 00:00:00.000000 drf_misc-0.2.1/.pylintrc
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 drf_misc-0.2.1/ignore-spelling-words.txt
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 drf_misc-0.2.1/mypy.ini
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 drf_misc-0.2.1/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.2.1/setup.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 drf_misc-0.2.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 drf_misc-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/admin.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/apps.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/settings.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/__init__.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/api_exceptions.py
+-rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/api_views.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/audit_service.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/cache.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/fields.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/filter_backend.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/middlewares.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/models.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/paginations.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/parsers.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/permissions.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/serializers.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/services.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/core/throttling.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/utility/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/utility/decorators.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/utility/epoch_util.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/utility/misc.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 drf_misc-0.2.1/drf_misc/utility/validator.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 drf_misc-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 drf_misc-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 drf_misc-0.2.1/README.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 drf_misc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 drf_misc-0.2.1/PKG-INFO
```

### Comparing `drf_misc-0.2.0/.pre-commit-config.yaml` & `drf_misc-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/.pylintrc` & `drf_misc-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/.github/workflows/publish.yaml` & `drf_misc-0.2.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/admin.py` & `drf_misc-0.2.1/drf_misc/admin.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/settings.py` & `drf_misc-0.2.1/drf_misc/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 from django.conf import settings
 
 # pylint: disable=invalid-name
 
+temp_app_settings = getattr(settings, "DRF_MISC_SETTINGS", {})
+assert temp_app_settings.get("service_name") != None
 
-class AppSettings:
-    def __init__(self):
-        self.app_settings = getattr(settings, "DRF_MISC_SETTINGS", {})
 
+class AppSettings:
     @property
     def service_name(self):
         """Control how many times a task will be attempted."""
-        return self.app_settings.get("service_name", "django_extra")
+        return temp_app_settings.get("service_name", "django_extra")
 
     @property
     def audit_queue_url(self):
         """Control how many times a task will be attempted."""
-        return self.app_settings.get("audit_queue_url", {})
+        return temp_app_settings.get("audit_queue_url", {})
 
     @property
     def use_service_cache(self):
-        return self.app_settings.get("use_service_cache", False)
+        return temp_app_settings.get("use_service_cache", False)
 
     @property
     def auth_check_disabled_paths(self):
-        return self.app_settings.get("auth_check_disabled_paths", [])
+        return temp_app_settings.get("auth_check_disabled_paths", [])
 
 
 app_settings = AppSettings()
 
 TIME_ZONE = "Asia/Kolkata"
```

### Comparing `drf_misc-0.2.0/drf_misc/core/api_exceptions.py` & `drf_misc-0.2.1/drf_misc/core/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/core/api_views.py` & `drf_misc-0.2.1/drf_misc/core/api_views.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/core/audit_service.py` & `drf_misc-0.2.1/drf_misc/core/audit_service.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/core/fields.py` & `drf_misc-0.2.1/drf_misc/core/fields.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/core/filter_backend.py` & `drf_misc-0.2.1/drf_misc/core/filter_backend.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/core/middlewares.py` & `drf_misc-0.2.1/drf_misc/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/core/models.py` & `drf_misc-0.2.1/drf_misc/core/models.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/core/paginations.py` & `drf_misc-0.2.1/drf_misc/core/paginations.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/core/serializers.py` & `drf_misc-0.2.1/drf_misc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/core/services.py` & `drf_misc-0.2.1/drf_misc/core/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     def __init__(self, instance_id=None, instance=None):
         if instance_id:
             self.instance = get_object_or_404(self.model, id=instance_id)
         elif instance:
             self.instance = instance
 
     def get_cache_key(self):
-        return f"{app_settings.service_name}:\
-                {self.instance.__class__.__name__.lower()}:{self.instance.id}"
+        return f"{app_settings.service_name}:{self.instance.__class__.__name__.lower()}:{self.instance.id}"
 
     def create(self, data, request, audit_data=None):
         ser = self.serializer(data=data)
         ser.is_valid(raise_exception=True)
         ser.save()
         self.instance = ser.instance
         if app_settings.use_service_cache and self.cache_serializer:
```

### Comparing `drf_misc-0.2.0/drf_misc/core/throttling.py` & `drf_misc-0.2.1/drf_misc/core/throttling.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/utility/decorators.py` & `drf_misc-0.2.1/drf_misc/utility/decorators.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/utility/epoch_util.py` & `drf_misc-0.2.1/drf_misc/utility/epoch_util.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/utility/misc.py` & `drf_misc-0.2.1/drf_misc/utility/misc.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/drf_misc/utility/validator.py` & `drf_misc-0.2.1/drf_misc/utility/validator.py`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/.gitignore` & `drf_misc-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/LICENSE` & `drf_misc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/README.md` & `drf_misc-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_misc-0.2.0/pyproject.toml` & `drf_misc-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "drf-misc"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Abhishek Sharma", email="abhishm20@gmail.com" },
 ]
 description = "A small Django DRF extension library which includes some useful utilities, APIs, Serializers and Services."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `drf_misc-0.2.0/PKG-INFO` & `drf_misc-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-misc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A small Django DRF extension library which includes some useful utilities, APIs, Serializers and Services.
 Project-URL: Homepage, https://github.com/abhishm20/drf-misc
 Project-URL: Bug Tracker, https://github.com/abhishm20/drf-misc/issues
 Author-email: Abhishek Sharma <abhishm20@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

