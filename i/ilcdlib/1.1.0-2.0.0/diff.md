# Comparing `tmp/ilcdlib-1.1.0.tar.gz` & `tmp/ilcdlib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-1.1.0.tar", max compression
+gzip compressed data, was "ilcdlib-2.0.0.tar", max compression
```

## Comparing `ilcdlib-1.1.0.tar` & `ilcdlib-2.0.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-07-25 14:34:41.570335 ilcdlib-1.1.0/LICENSE
--rw-r--r--   0        0        0     5311 2023-07-25 14:34:41.570335 ilcdlib-1.1.0/README.md
--rw-r--r--   0        0        0     3489 2023-07-25 14:34:41.570335 ilcdlib-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      837 2023-07-25 14:34:41.570335 ilcdlib-1.1.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2023-07-25 14:34:41.570335 ilcdlib-1.1.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2023-07-25 14:34:41.570335 ilcdlib-1.1.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2023-07-25 14:34:41.570335 ilcdlib-1.1.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17587 2023-07-25 14:34:41.570335 ilcdlib-1.1.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0     1796 2023-07-25 14:34:41.570335 ilcdlib-1.1.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0   172140 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     4431 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     6946 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     3361 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     4160 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     3024 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3797 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     6864 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     1329 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2051 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3328 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    32071 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2050 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7667 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0     1928 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     1892 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     2588 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2023-07-25 14:34:41.574335 ilcdlib-1.1.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1705 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0    10655 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     2513 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/soda4lca/api_client_4x.py
--rw-r--r--   0        0        0     1206 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     3329 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2023-07-25 14:34:41.578335 ilcdlib-1.1.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6421 1970-01-01 00:00:00.000000 ilcdlib-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-22 15:44:46.266401 ilcdlib-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5311 2023-07-22 15:44:46.266401 ilcdlib-2.0.0/README.md
+-rw-r--r--   0        0        0     3488 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17587 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0     1796 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0   172140 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     4727 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     6375 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     3361 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     3638 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     2745 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3774 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10086 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     3399 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     1329 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2051 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3328 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    32071 2023-07-22 15:44:46.270401 ilcdlib-2.0.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2050 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7667 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0     1900 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     1892 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     1737 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1705 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    10655 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     2513 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/soda4lca/api_client_4x.py
+-rw-r--r--   0        0        0     1206 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     3329 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2023-07-22 15:44:46.274401 ilcdlib-2.0.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6420 1970-01-01 00:00:00.000000 ilcdlib-2.0.0/PKG-INFO
```

### Comparing `ilcdlib-1.1.0/LICENSE` & `ilcdlib-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/README.md` & `ilcdlib-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/pyproject.toml` & `ilcdlib-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "1.1.0"
+version = "2.0.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
@@ -22,15 +22,15 @@
 [tool.poetry.scripts]
 ilcdtool = { callable = "ilcdlib:cli.entrypoint", extras = ["cli"] }
 
 [tool.poetry.dependencies]
 python = "^3.11"
 urllib3 = { version = ">=1.26.16,<2.0.0" }
 requests = { version = ">=2.1.0,<3.0.0" }
-openepd = { version = ">=0.11.1,<2.0.0" }
+openepd = { version = ">=2.0.0,<3.0.0" }
 
 # Optional dependencies
 lxml = { version = "~=4.9.2", optional = true }
 cli-rack = { version = ">=1.0.6", optional = true }
 
 [tool.poetry.dev-dependencies]
 wheel = { version ="~=0.40.0" }
@@ -60,15 +60,15 @@
 types-urllib3 = ">=1.26.2"
 
 [tool.poetry.extras]
 lxml = ["lxml"]
 cli = ["cli-rack"]
 
 [tool.commitizen]
-version = "1.1.0"
+version = "2.0.0"
 bump_version = "bump: version $current_version → $new_version"
 update_changelog_on_bump = true
 pre_bump_hooks = []
 version_files = [
     "pyproject.toml",
     "src/ilcdlib/__version__.py",
 ]
```

### Comparing `ilcdlib-1.1.0/src/ilcdlib/__init__.py` & `ilcdlib-2.0.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/__main__.py` & `ilcdlib-2.0.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/__version__.py` & `ilcdlib-2.0.0/src/ilcdlib/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "1.1.0"
+VERSION = "2.0.0"
```

### Comparing `ilcdlib-1.1.0/src/ilcdlib/cli.py` & `ilcdlib-2.0.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/common.py` & `ilcdlib-2.0.0/src/ilcdlib/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/const.py` & `ilcdlib-2.0.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-2.0.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/dto.py` & `ilcdlib-2.0.0/src/ilcdlib/dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -100,21 +100,39 @@
 
     pass
 
 
 class IlcdContactInfo(BaseOpenEpdSchema):
     """Contact information extracted from ILCD contact."""
 
-    contact_person: str | None = pyd.Field(description="Name of the contact person", example="John Doe", default=None)
-    email: pyd.EmailStr | None = pyd.Field(description="Email", example="contact@c-change-labs.com", default=None)
-    phone: str | None = pyd.Field(description="Phone number", example="+15263327352", default=None)
+    contact_person: str | None = pyd.Field(
+        default=None,
+        description="Name of the contact person",
+        json_schema_extra=dict(example="John Doe"),
+    )
+    email: pyd.EmailStr | None = pyd.Field(
+        default=None,
+        description="Email",
+        json_schema_extra=dict(example="contact@c-change-labs.com"),
+    )
+    phone: str | None = pyd.Field(
+        default=None,
+        description="Phone number",
+        json_schema_extra=dict(example="+15263327352"),
+    )
     website: pyd.AnyUrl | None = pyd.Field(
-        description="Url of the website", example="http://buildingtransparency.org", default=None
+        default=None,
+        description="Url of the website",
+        json_schema_extra=dict(example="http://buildingtransparency.org"),
+    )
+    address: str | None = pyd.Field(
+        default=None,
+        description="Address",
+        json_schema_extra=dict(example="123 Main St, San Francisco, CA 94105"),
     )
-    address: str | None = pyd.Field(description="Address", example="123 Main St, San Francisco, CA 94105", default=None)
 
 
 class OpenEpdIlcdOrg(Org):
     """Org object with ILCD specific extension."""
 
     def get_contact(self) -> IlcdContactInfo | None:
         """Return ILCD contact information from extension field if any."""
@@ -124,18 +142,18 @@
         return ext.contact if ext else None
 
 
 class ComplianceDto(pydantic.BaseModel):
     """Basic information about a Compliance."""
 
     uuid: str
-    short_name: str | None
-    name: str | None
-    link: str | None
-    issuer: OpenEpdIlcdOrg | None
+    short_name: str | None = None
+    name: str | None = None
+    link: str | None = None
+    issuer: OpenEpdIlcdOrg | None = None
 
 
 class ValidationDto(pydantic.BaseModel):
     """Basic information about a Compliance."""
 
-    validation_type: IlcdTypeOfReview | None
+    validation_type: IlcdTypeOfReview | None = None
     org: OpenEpdIlcdOrg
```

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,45 +45,40 @@
 
     def _get_scope_set_for_el(
         self,
         el: T_ET.Element,
         reference_data_set: XmlPath,
         mapper: SimpleDataMapper[str],
         scenario_names: dict[str, str],
-        scope_to_units_mapper: SimpleDataMapper[str],
     ) -> tuple[ScopeSet, str] | None:
         """Extract all scope set information from element."""
         # Impact name
         type_el = self._get_el(el, reference_data_set)
         if type_el is None:
             return None
         type_uuid = type_el.attrib.get("refObjectId") if type_el is not None else None
         if type_uuid is None:
             return None
         impact_name: str | None = mapper.map(type_uuid, type_uuid)
         if impact_name == type_uuid:
             impact_name = self._get_localized_text(type_el, ("common:shortDescription",), ("en", None))
         if impact_name is None:
             return None
+        # UoM
         unit_el = self._get_external_tree(
             el,
             (
                 "common:other",
                 "epd2013:referenceToUnitGroupDataSet",
             ),
         )
-        unit_name: str | None
         if unit_el is None:
-            # This step is assumption for cases, when program operator omit unit group reference in related ILCD file.
-            # In future, we should add context to the curator notes field for such cases.
-            if unit_name := scope_to_units_mapper.map(impact_name, None):
-                scopes = self.__extract_scopes(el, unit_name, scenario_names)
-                return ScopeSet(**scopes), impact_name  # type: ignore
             return None
         unit = self.unit_group_reader_cls(unit_el, self.data_provider).get_reference_unit(allow_mapping=True)
+        unit_name: str | None
         if unit is not None:
             unit_name = unit.name
         else:
             unit_name = self._get_text(
                 el, ("common:other", "epd2013:referenceToUnitGroupDataSet", "common:shortDescription")
             )
         if unit_name is None:
@@ -153,20 +148,17 @@
         el: T_ET.Element,
         reference_path: XmlPath,
         scope_set_type: Type[BaseOpenEpdSchema],
         scope_set_dict: dict[str, ScopeSet | dict],
         ext: dict[str, ScopeSet],
         mapper: SimpleDataMapper[str],
         scenario_names: dict[str, str],
-        scope_to_units_mapper: SimpleDataMapper[str],
     ) -> None:
         """Extract scope set from element and set to its dictionary."""
-        scope_set_and_impact_name = self._get_scope_set_for_el(
-            el, reference_path, mapper, scenario_names, scope_to_units_mapper
-        )
+        scope_set_and_impact_name = self._get_scope_set_for_el(el, reference_path, mapper, scenario_names)
         if scope_set_and_impact_name is None:
             return None
         scope_set, impact_name = scope_set_and_impact_name
         if scope_set_type.is_allowed_field_name(impact_name):
             scope_set_dict[impact_name] = scope_set
         else:
             ext[impact_name] = scope_set
```

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/category.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/contact.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/flow.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/lcia.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,30 +19,27 @@
 #
 from openepd.model.lcia import Impacts, ImpactSet, ScopeSet
 
 from ilcdlib.common import OpenEpdImpactSetSupportReader
 from ilcdlib.entity.base_scope_set_reader import BaseIlcdScopeSetsReader
 from ilcdlib.mapping.common import SimpleDataMapper
 from ilcdlib.mapping.impacts import default_impacts_uuid_mapper
-from ilcdlib.mapping.units import default_scope_to_units_mapper
 
 
 class IlcdLciaResultsReader(OpenEpdImpactSetSupportReader, BaseIlcdScopeSetsReader):
     """Read an ILCD PCR XML file."""
 
     def __init__(
         self,
         *args,
         impact_mapper: SimpleDataMapper[str] = default_impacts_uuid_mapper,
-        scope_to_units_mapper: SimpleDataMapper[str] = default_scope_to_units_mapper,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.impact_mapper = impact_mapper
-        self.scope_to_units_mapper = scope_to_units_mapper
 
     def get_impact_set(self, scenario_names: dict[str, str]) -> ImpactSet:
         """Get the impacts from the ILCD EPD file."""
         ext: dict[str, ScopeSet] = {}
         lcia_results = self._get_all_els(self._entity, ("process:LCIAResult",))
         impacts: dict[str, ScopeSet | dict] = {"ext": ext}
 
@@ -51,25 +48,24 @@
                 el=lr,
                 reference_path=("process:referenceToLCIAMethodDataSet",),
                 scope_set_type=ImpactSet,
                 scope_set_dict=impacts,
                 ext=ext,
                 mapper=self.impact_mapper,
                 scenario_names=scenario_names,
-                scope_to_units_mapper=self.scope_to_units_mapper,
             )
         if len(ext) == 0:
             del impacts["ext"]
         return ImpactSet(**impacts)  # type: ignore
 
     def to_openepd_impacts(
         self,
         scenario_names: dict[str, str],
         lcia_method: str | None = None,
         base_url: str | None = None,
         provider_domain: str | None = None,
     ) -> Impacts:
         """Read as openEPD ImpactSet object."""
         impact_set = self.get_impact_set(scenario_names)
-        impacts = Impacts(__root__={})
+        impacts = Impacts(root={})
         impacts.set_impact_set(lcia_method, impact_set)
         return impacts
```

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/material.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/source.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/unit.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,16 +86,16 @@
                 f"ug:unit[@dataSetInternalID='{reference_unit_id}']",
             ),
         )
         if element is None:
             return None
         unit_name = none_throws(self._get_text(element, "ug:name"))
         unit_uuid = self.get_uuid()
-        if allow_mapping and unit_uuid is not None and (u_name := self.unit_mapper.map(unit_uuid, unit_name)):
-            unit_name = u_name
+        if allow_mapping and unit_uuid is not None:
+            unit_name = self.unit_mapper.map(unit_uuid, unit_name)
         return (
             UnitDto(
                 name=unit_name,
                 mean_value=none_throws(self._get_float(element, "ug:meanValue")),
             )
             if element is not None
             else None
```

### Comparing `ilcdlib-1.1.0/src/ilcdlib/entity/validation.py` & `ilcdlib-2.0.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-2.0.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/epd/cli.py` & `ilcdlib-2.0.0/src/ilcdlib/epd/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,27 +196,27 @@
             )
         lang_list = [lang, None]
         if prioritize_english:
             lang_list.insert(0, "en")
         CLI.print_info("Language priority: " + ",".join([x if x is not None else "any other" for x in lang_list]))
         base_url = self.__extract_base_url(doc_ref)
         open_epd = epd_reader.to_openepd_epd(lang_list, base_url=base_url, provider_domain=provider_domain)
-        CLI.print_data(open_epd.json(indent=2, exclude_none=True, exclude_unset=True))
+        CLI.print_data(open_epd.model_dump_json(indent=2, exclude_none=True, exclude_unset=True))
         if save:
             self.save_results(epd_reader, open_epd, extract_pdf=extract_pdf, base_dir=target_dir)
 
     def save_results(
         self, epd_reader: IlcdEpdReader, result: Epd, *, extract_pdf: bool = False, base_dir: Path | None = None
     ):
         if base_dir is None:
             base_dir = Path.cwd()
         output_dir = base_dir / Path(epd_reader.get_uuid())
         ensure_dir(output_dir)
         with open(output_dir / "openEPD.json", "w") as f:
-            f.write(result.json(indent=2, exclude_none=True, exclude_unset=True))
+            f.write(result.model_dump_json(indent=2, exclude_none=True, exclude_unset=True))
         if isinstance(epd_reader.data_provider, ZipIlcdReader):
             epd_reader.data_provider.save_to(output_dir / "ilcd_epd.zip")
         if extract_pdf:
             # EPD Pdf
             pdf_stream = epd_reader.get_epd_document_stream()
             if pdf_stream is None and isinstance(epd_reader.data_provider, Soda4LcaZipReader):
                 try:
```

### Comparing `ilcdlib-1.1.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-2.0.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-2.0.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-2.0.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/epd/factory.py` & `ilcdlib-2.0.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/epd/reader.py` & `ilcdlib-2.0.0/src/ilcdlib/epd/reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/extension.py` & `ilcdlib-2.0.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/http_common.py` & `ilcdlib-2.0.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-2.0.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/mapping/common.py` & `ilcdlib-2.0.0/src/ilcdlib/mapping/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 K = TypeVar("K")
 
 
 class BaseDataMapper(Generic[T, K], abc.ABC):
     """Base class for all data mappers."""
 
     @abc.abstractmethod
-    def map(self, input_value: T, default_value: K | None) -> K | None:
+    def map(self, input_value: T, default_value: K) -> K:
         """
         Map the input value to the output value.
 
         :param input_value: The input value to map.
         :param default_value: The default value to return if there is no mapping for input value.
         """
         pass
 
 
 class SimpleDataMapper(BaseDataMapper[T, T], Generic[T]):
     """A data mapper that does not change the type of the input value."""
 
     DATABASE: dict[T, T] = {}
 
-    def map(self, input_value: T, default_value: T | None) -> T | None:
+    def map(self, input_value: T, default_value: T) -> T:
         """
         Map the input value to the output value.
 
         :param input_value: The input value to map.
         :param default_value: The default value to return if there is no mapping for input value.
         """
         return self.DATABASE.get(input_value, default_value)
```

### Comparing `ilcdlib-1.1.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-2.0.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-2.0.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-2.0.0/src/ilcdlib/mapping/impacts.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-2.0.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-2.0.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-2.0.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/medium/archive.py` & `ilcdlib-2.0.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-2.0.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/reference_data.py` & `ilcdlib-2.0.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-2.0.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-2.0.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-2.0.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/sanitizing/text.py` & `ilcdlib-2.0.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-2.0.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-2.0.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/soda4lca/api_client_4x.py` & `ilcdlib-2.0.0/src/ilcdlib/soda4lca/api_client_4x.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/type.py` & `ilcdlib-2.0.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/utils.py` & `ilcdlib-2.0.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/src/ilcdlib/xml_parser.py` & `ilcdlib-2.0.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-1.1.0/PKG-INFO` & `ilcdlib-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 1.1.0
+Version: 2.0.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: cli
 Provides-Extra: lxml
 Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml"
-Requires-Dist: openepd (>=0.11.1,<2.0.0)
+Requires-Dist: openepd (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.1.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/cchangelabs/ilcdlib
 Description-Content-Type: text/markdown
 
 # ILCD Lib
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 1.1.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 2.0.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Provides-Extra: cli
 Provides-Extra: lxml Requires-Dist: cli-rack (>=1.0.6) ; extra == "cli"
 Requires-Dist: lxml (>=4.9.2,<4.10.0) ; extra == "lxml" Requires-Dist: openepd
-(>=0.11.1,<2.0.0) Requires-Dist: requests (>=2.1.0,<3.0.0) Requires-Dist:
+(>=2.0.0,<3.0.0) Requires-Dist: requests (>=2.1.0,<3.0.0) Requires-Dist:
 urllib3 (>=1.26.16,<2.0.0) Project-URL: Repository, https://github.com/
 cchangelabs/ilcdlib Description-Content-Type: text/markdown # ILCD Lib
      [https://img.shields.io/pypi/l/ilcdlib?style=for-the-badge] [https://
      img.shields.io/pypi/pyversions/ilcdlib?style=for-the-badge] [https://
  img.shields.io/badge/Code%20Style-black-black?style=for-the-badge] [https://
   img.shields.io/pypi/v/ilcdlib?style=for-the-badge] [https://img.shields.io/
                      pypi/dm/ilcdlib?style=for-the-badge]
```

