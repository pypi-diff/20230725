# Comparing `tmp/odoo_addon_extendable_fastapi-16.0.1.0.1-py3-none-any.whl.zip` & `tmp/odoo_addon_extendable_fastapi-16.0.2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,17 @@
-Zip file size: 21609 bytes, number of entries: 16
--rw-r--r--  2.0 unx     3207 b- defN 23-Jun-28 11:20 odoo/addons/extendable_fastapi/README.rst
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-28 11:19 odoo/addons/extendable_fastapi/__init__.py
--rw-r--r--  2.0 unx      627 b- defN 23-Jun-28 11:20 odoo/addons/extendable_fastapi/__manifest__.py
--rw-r--r--  2.0 unx      496 b- defN 23-Jun-28 11:19 odoo/addons/extendable_fastapi/i18n/extendable_fastapi.pot
--rw-r--r--  2.0 unx       31 b- defN 23-Jun-28 11:19 odoo/addons/extendable_fastapi/models/__init__.py
--rw-r--r--  2.0 unx     1136 b- defN 23-Jun-28 11:19 odoo/addons/extendable_fastapi/models/fastapi_endpoint.py
--rw-r--r--  2.0 unx       64 b- defN 23-Jun-28 11:19 odoo/addons/extendable_fastapi/readme/CONTRIBUTORS.rst
--rw-r--r--  2.0 unx      346 b- defN 23-Jun-28 11:19 odoo/addons/extendable_fastapi/readme/DESCRIPTION.rst
--rw-r--r--  2.0 unx     9455 b- defN 23-Jun-28 11:19 odoo/addons/extendable_fastapi/static/description/icon.png
--rw-r--r--  2.0 unx    12482 b- defN 23-Jun-28 11:20 odoo/addons/extendable_fastapi/static/description/index.html
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-28 11:19 odoo/addons/extendable_fastapi/tests/__init__.py
--rw-r--r--  2.0 unx      653 b- defN 23-Jun-28 11:19 odoo/addons/extendable_fastapi/tests/common.py
--rw-r--r--  2.0 unx     3939 b- defN 23-Jun-28 11:20 odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-28 11:20 odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-28 11:20 odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1689 b- defN 23-Jun-28 11:20 odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/RECORD
-16 files, 34243 bytes uncompressed, 18675 bytes compressed:  45.5%
+Zip file size: 21212 bytes, number of entries: 15
+-rw-r--r--  2.0 unx     3207 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/README.rst
+-rw-r--r--  2.0 unx       33 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/__init__.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/__manifest__.py
+-rw-r--r--  2.0 unx      927 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/fastapi_dispatcher.py
+-rw-r--r--  2.0 unx      341 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/i18n/extendable_fastapi.pot
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/readme/CONTRIBUTORS.rst
+-rw-r--r--  2.0 unx      346 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/readme/DESCRIPTION.rst
+-rw-r--r--  2.0 unx     9455 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/static/description/icon.png
+-rw-r--r--  2.0 unx    12482 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/static/description/index.html
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/tests/__init__.py
+-rw-r--r--  2.0 unx      653 b- defN 23-Jul-25 16:11 odoo/addons/extendable_fastapi/tests/common.py
+-rw-r--r--  2.0 unx     3939 b- defN 23-Jul-25 16:11 odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-25 16:11 odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-25 16:11 odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1579 b- defN 23-Jul-25 16:11 odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/RECORD
+15 files, 33750 bytes uncompressed, 18462 bytes compressed:  45.3%
```

## zipnote {}

```diff
@@ -3,21 +3,18 @@
 
 Filename: odoo/addons/extendable_fastapi/__init__.py
 Comment: 
 
 Filename: odoo/addons/extendable_fastapi/__manifest__.py
 Comment: 
 
-Filename: odoo/addons/extendable_fastapi/i18n/extendable_fastapi.pot
-Comment: 
-
-Filename: odoo/addons/extendable_fastapi/models/__init__.py
+Filename: odoo/addons/extendable_fastapi/fastapi_dispatcher.py
 Comment: 
 
-Filename: odoo/addons/extendable_fastapi/models/fastapi_endpoint.py
+Filename: odoo/addons/extendable_fastapi/i18n/extendable_fastapi.pot
 Comment: 
 
 Filename: odoo/addons/extendable_fastapi/readme/CONTRIBUTORS.rst
 Comment: 
 
 Filename: odoo/addons/extendable_fastapi/readme/DESCRIPTION.rst
 Comment: 
@@ -30,20 +27,20 @@
 
 Filename: odoo/addons/extendable_fastapi/tests/__init__.py
 Comment: 
 
 Filename: odoo/addons/extendable_fastapi/tests/common.py
 Comment: 
 
-Filename: odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/METADATA
+Filename: odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/WHEEL
+Filename: odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/top_level.txt
+Filename: odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/RECORD
+Filename: odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/extendable_fastapi/__init__.py

```diff
@@ -1 +1 @@
-from . import models
+from . import fastapi_dispatcher
```

## odoo/addons/extendable_fastapi/__manifest__.py

```diff
@@ -1,22 +1,22 @@
 # Copyright 2023 ACSONE SA/NV
 # License LGPL-3.0 or later (https://www.gnu.org/licenses/lgpl).
 
 {
     "name": "Extendable Fastapi",
     "summary": """
         Allows the use of extendable into fastapi apps""",
-    "version": "16.0.1.0.1",
+    "version": "16.0.2.0.0",
     "license": "LGPL-3",
     "author": "ACSONE SA/NV,Odoo Community Association (OCA)",
     "maintainers": ["lmignon"],
     "website": "https://github.com/OCA/rest-framework",
     "depends": ["fastapi", "extendable"],
     "data": [],
     "demo": [],
     "external_dependencies": {
         "python": [
-            "extendable-pydantic>=0.0.4",
+            "extendable-pydantic>=1.0.0",
         ],
     },
     "installable": True,
 }
```

## odoo/addons/extendable_fastapi/i18n/extendable_fastapi.pot

```diff
@@ -1,19 +1,13 @@
 # Translation of Odoo Server.
 # This file contains the translation of the following modules:
-# 	* extendable_fastapi
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Odoo Server 16.0\n"
 "Report-Msgid-Bugs-To: \n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: \n"
 "Plural-Forms: \n"
-
-#. module: extendable_fastapi
-#: model:ir.model,name:extendable_fastapi.model_fastapi_endpoint
-msgid "FastAPI Endpoint"
-msgstr ""
```

## Comparing `odoo/addons/extendable_fastapi/models/fastapi_endpoint.py` & `odoo/addons/extendable_fastapi/fastapi_dispatcher.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 # Copyright 2023 ACSONE SA/NV
-# License LGPL-3.0 or later (https://www.gnu.org/licenses/lgpl).
+# License LGPL-3.0 or later (http://www.gnu.org/licenses/LGPL).
 
-from typing import List
-
-from starlette.middleware import Middleware
-
-from odoo import models
+from contextlib import contextmanager
 
 from odoo.addons.extendable.registry import _extendable_registries_database
+from odoo.addons.fastapi.fastapi_dispatcher import (
+    FastApiDispatcher as BaseFastApiDispatcher,
+)
 
 from extendable import context
 
 
-class ExtendableContextManagerMiddleware(object):
-    def __init__(self, app, dbname):
-        self.app = app
-        self.dbname = dbname
+class FastApiDispatcher(BaseFastApiDispatcher):
+    routing_type = "fastapi"
 
-    async def __call__(self, scope, receive, send):
-        registry = _extendable_registries_database.get(self.dbname, {})
+    def dispatch(self, endpoint, args):
+        with self._manage_extendable_context():
+            return super().dispatch(endpoint, args)
+
+    @contextmanager
+    def _manage_extendable_context(self):
+        env = self.request.env
+        registry = _extendable_registries_database.get(env.cr.dbname, {})
         token = context.extendable_registry.set(registry)
         try:
-            response = await self.app(scope, receive, send)
+            response = yield
         finally:
             context.extendable_registry.reset(token)
         return response
-
-
-class FastapiEndpoint(models.Model):
-
-    _inherit = "fastapi.endpoint"
-
-    def _get_fastapi_app_middlewares(self) -> List[Middleware]:
-        middlewares = super()._get_fastapi_app_middlewares()
-        middlewares.append(
-            (ExtendableContextManagerMiddleware, {"dbname": self.env.cr.dbname})
-        )
-        return middlewares
```

## Comparing `odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/METADATA` & `odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: odoo-addon-extendable-fastapi
-Version: 16.0.1.0.1
+Version: 16.0.2.0.0
 Summary: Allows the use of extendable into fastapi apps
 Home-page: https://github.com/OCA/rest-framework
 Author: ACSONE SA/NV,Odoo Community Association (OCA)
 Author-email: support@odoo-community.org
 License: LGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.10
-Requires-Dist: extendable-pydantic (>=0.0.4)
+Requires-Dist: extendable-pydantic (>=1.0.0)
 Requires-Dist: odoo-addon-extendable (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-fastapi (<16.1dev,>=16.0dev)
 Requires-Dist: odoo (<16.1dev,>=16.0a)
 
 ==================
 Extendable Fastapi
 ==================
```

## Comparing `odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/RECORD` & `odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 odoo/addons/extendable_fastapi/README.rst,sha256=6CYiFtFpypAt-RcVvZRSb1-a53JVNbA3U8ivhRdAzec,3207
-odoo/addons/extendable_fastapi/__init__.py,sha256=X9EJGOE2GtZbS0G82PtSXmWSZ_R8jEM0rlJTDliQjp4,21
-odoo/addons/extendable_fastapi/__manifest__.py,sha256=le8wSnnQYPjEeVx3yDQL3jUdMbWp_tQTlcxof7UR0rc,627
-odoo/addons/extendable_fastapi/i18n/extendable_fastapi.pot,sha256=YS2iOEx-hogBI4iLHbJppu7t2UlgfI0Lc_SGefvMDRA,496
-odoo/addons/extendable_fastapi/models/__init__.py,sha256=NF75IvaT9G60mgm2FqAkfw91SzMZ9m7CL41HiOD3rj4,31
-odoo/addons/extendable_fastapi/models/fastapi_endpoint.py,sha256=OOASq1MgCX-pHrM372azxLRARmpN8ObD7BnVYM_yQnQ,1136
+odoo/addons/extendable_fastapi/__init__.py,sha256=QQD_pxV1KCC13JIIYAOUhm0MbmOszCIeRU9c3moKwGU,33
+odoo/addons/extendable_fastapi/__manifest__.py,sha256=HKplJncxfIb4gXab_etgaXZ5K7p5MJk4fHyy1YpHN8E,627
+odoo/addons/extendable_fastapi/fastapi_dispatcher.py,sha256=bNU0qaPM4X4U3FtQ-75z2ZSZ_096nGQfoi3-2_z99XI,927
+odoo/addons/extendable_fastapi/i18n/extendable_fastapi.pot,sha256=leB6MlaWiU1sPOdcOTxNVY5KVORnHv0MfD14HgQJIIs,341
 odoo/addons/extendable_fastapi/readme/CONTRIBUTORS.rst,sha256=WW1D_j8BmB4IAjFMy5KNdQqpwZKOTTFWOXomGl5cl2M,64
 odoo/addons/extendable_fastapi/readme/DESCRIPTION.rst,sha256=grk1QShjGk-LgDXbqxACMB4Wbeo8iMAaAEzDCYPYq-k,346
 odoo/addons/extendable_fastapi/static/description/icon.png,sha256=6xBPJauaFOF0KDHfHgQopSc28kKvxMaeoQFQWZtfZDo,9455
 odoo/addons/extendable_fastapi/static/description/index.html,sha256=NWcA_Z4ELf5cIzBCATujLPMCr2lUKFI10MOKtZ1GFeI,12482
 odoo/addons/extendable_fastapi/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 odoo/addons/extendable_fastapi/tests/common.py,sha256=WE5B-n4PwHWMR7gS5idD5iXnDD6-0-otzMqaBHLql_o,653
-odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/METADATA,sha256=2bv8IxSN99MCoY1ek4ZDkso0xPmYCkDlQ3RZTRwYD78,3939
-odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo_addon_extendable_fastapi-16.0.1.0.1.dist-info/RECORD,,
+odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/METADATA,sha256=bvmcyKCGFIWZvj3IY62F067xCwP049WjjaJHUfCqp_E,3939
+odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo_addon_extendable_fastapi-16.0.2.0.0.dist-info/RECORD,,
```

