# Comparing `tmp/meringue-1.1.0.dev3.tar.gz` & `tmp/meringue-1.1.0.dev5.tar.gz`

## Comparing `meringue-1.1.0.dev3.tar` & `meringue-1.1.0.dev5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/__init__.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/apps.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/handlers.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/routers.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/api/utils.py
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/conf/__init__.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/conf/default_settings.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/__init__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/apps.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/options.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/query.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/translation.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/upload_handlers.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/views.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/templatetags/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/templatetags/meringue_base.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/utils/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/utils/crypt.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/utils/datetime.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/meringue/core/utils/frontend.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/.gitignore
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/AUTHORS
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/LICENSE
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/README.md
--rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     8764 2020-02-02 00:00:00.000000 meringue-1.1.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/apps.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/handlers.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/routers.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/api/utils.py
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/conf/__init__.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/conf/default_settings.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/__init__.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/apps.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/options.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/query.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/translation.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/upload_handlers.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/views.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/templatetags/__init__.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/templatetags/meringue_base.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/utils/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/utils/crypt.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/utils/datetime.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/meringue/core/utils/frontend.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/.gitignore
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/AUTHORS
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/LICENSE
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/README.md
+-rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0     8924 2020-02-02 00:00:00.000000 meringue-1.1.0.dev5/PKG-INFO
```

### Comparing `meringue-1.1.0.dev3/meringue/api/handlers.py` & `meringue-1.1.0.dev5/meringue/api/handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/api/routers.py` & `meringue-1.1.0.dev5/meringue/api/routers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/api/utils.py` & `meringue-1.1.0.dev5/meringue/api/utils.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/conf/__init__.py` & `meringue-1.1.0.dev5/meringue/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/conf/default_settings.py` & `meringue-1.1.0.dev5/meringue/conf/default_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,9 +36,9 @@
 """
 
 
 # API #############################################################################################
 
 API_ENABLE_ROOT_VIEW: Final[str] = settings.DEBUG
 """
-Option to enable or disable the root view of the [Router][meringue.api.routers.DefaultRouter]
+Option to enable or disable the root view of the [Router][meringue.api.routers.MeringueRouter]
 """
```

### Comparing `meringue-1.1.0.dev3/meringue/core/models.py` & `meringue-1.1.0.dev5/meringue/core/models.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/core/query.py` & `meringue-1.1.0.dev5/meringue/core/query.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/core/translation.py` & `meringue-1.1.0.dev5/meringue/core/translation.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/core/upload_handlers.py` & `meringue-1.1.0.dev5/meringue/core/upload_handlers.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/core/locale/en/LC_MESSAGES/django.po` & `meringue-1.1.0.dev5/meringue/core/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/core/locale/ru/LC_MESSAGES/django.po` & `meringue-1.1.0.dev5/meringue/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/core/templatetags/meringue_base.py` & `meringue-1.1.0.dev5/meringue/core/templatetags/meringue_base.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/core/utils/crypt.py` & `meringue-1.1.0.dev5/meringue/core/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/core/utils/datetime.py` & `meringue-1.1.0.dev5/meringue/core/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/meringue/core/utils/frontend.py` & `meringue-1.1.0.dev5/meringue/core/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/LICENSE` & `meringue-1.1.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `meringue-1.1.0.dev3/README.md` & `meringue-1.1.0.dev5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,29 +63,29 @@
 However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
 
 ## Roadmap
 
 Adding new functionality. Can change.
 
-* [x] Universal manager worked with all abstract models
-* [x] Tests of all functionality
+* [x] Universal manager worked with all abstract models.
+* [x] Tests of all functionality.
 * [x] Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
 * [x] Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
-* [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
- generating form based on response from api).
+* [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed generating form based on response from api).
 * [x] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
 * [ ] Authorization backend for authorization by a pair of email and password.
-* [ ] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
+* [x] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
+* [x] drf-spectacular view with patching documentation.
 * [ ] Functionality for working with images.
 	* [ ] Image editor like easy_thumbnails.
 	* [ ] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
 * [ ] Functionality similar to that described in the previous paragraph only for video.
 * [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
-* [x] Exception handler for drf that returns an error code in addition to the error text
+* [x] Exception handler for drf that returns an error code in addition to the error text.
 
 
 ## Contributing
 
 - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to resolve the versioning
 - [x] Linter with a [Ruff](https://github.com/charliermarsh/ruff)
 - [x] Formatter with a [Black](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -12,42 +12,43 @@
 works. However, if someone decides to use this functionality in their project,
 and even more so to add functionality or change the implementation to a more
 correct, beautiful or understandable one, I will only be happy, do not worry
 and feel free to write to me by [mail](mailto:dd@manin.space), create an
 [issue](https://github.com/dd/Meringue/issues) or [pull request](https://
 github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue). ##
 Roadmap Adding new functionality. Can change. * [x] Universal manager worked
-with all abstract models * [x] Tests of all functionality * [x] Methods for
+with all abstract models. * [x] Tests of all functionality. * [x] Methods for
 encrypting and decrypting text content (To create various secrets, such as a
 link to change your password or activate your profile). * [x] Functionality for
 obtaining absolute links to resources presented on the front, located on
 another domain (When working through api) (utils methods, template tags and
 filters). * [ ] [drf](https://www.django-rest-framework.org/) serializer
 serializer for automatic form generation on the front when working through rest
 api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
 generating form based on response from api). * [x] Extended [drf router](https:
 //www.django-rest-framework.org/api-guide/routers/) that allows you to add
 resources like `/profile` returning the profile data of an authorized user
 without his id. * [ ] Authorization backend for authorization by a pair of
-email and password. * [ ] Helpers to extend documentation generated by [drf-
+email and password. * [x] Helpers to extend documentation generated by [drf-
 spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to
 easily add links to different deployed environments (production, test, local,
 etc.) or let's say for more digestible tags instead of initially generated ones
-* [ ] Functionality for working with images. * [ ] Image editor like
-easy_thumbnails. * [ ] A field for the drf serializer that returns a set of
-images (for example, a standard image and a double-sized image for a retina
-screen), as well as in different formats (for example, in the original format
-and in webp). * [ ] Functionality similar to that described in the previous
-paragraph only for video. * [ ] Functionality for loading private files
-available through [nginx internal](http://nginx.org/en/docs/http/
-ngx_http_core_module.html#internal). * [x] Exception handler for drf that
-returns an error code in addition to the error text ## Contributing - [x] Use
-Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https:
-//www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to
-resolve the versioning - [x] Linter with a [Ruff](https://github.com/
-charliermarsh/ruff) - [x] Formatter with a [Black](https://github.com/psf/
-black) - [x] Lint commit with [Gitlint](https://jorisroovers.com/gitlint/) and
-[Conventional Commits](https://www.conventionalcommits.org/) - [x]
-Documentation with [mkdocs](https://www.mkdocs.org/) and [mkdocs-material]
-(https://squidfunk.github.io/mkdocs-material/) - [x] Testing local with [hatch]
-(https://hatch.pypa.io/1.7/meta/faq/#environments) - [x] Testing in CI/CD on
-push - [ ] Add [mypy](https://mypy-lang.org/) ???
+* [x] drf-spectacular view with patching documentation. * [ ] Functionality for
+working with images. * [ ] Image editor like easy_thumbnails. * [ ] A field for
+the drf serializer that returns a set of images (for example, a standard image
+and a double-sized image for a retina screen), as well as in different formats
+(for example, in the original format and in webp). * [ ] Functionality similar
+to that described in the previous paragraph only for video. * [ ] Functionality
+for loading private files available through [nginx internal](http://nginx.org/
+en/docs/http/ngx_http_core_module.html#internal). * [x] Exception handler for
+drf that returns an error code in addition to the error text. ## Contributing -
+[x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and
+[here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-
+workflow)) to resolve the versioning - [x] Linter with a [Ruff](https://
+github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
+github.com/psf/black) - [x] Lint commit with [Gitlint](https://
+jorisroovers.com/gitlint/) and [Conventional Commits](https://
+www.conventionalcommits.org/) - [x] Documentation with [mkdocs](https://
+www.mkdocs.org/) and [mkdocs-material](https://squidfunk.github.io/mkdocs-
+material/) - [x] Testing local with [hatch](https://hatch.pypa.io/1.7/meta/faq/
+#environments) - [x] Testing in CI/CD on push - [ ] Add [mypy](https://mypy-
+lang.org/) ???
```

### Comparing `meringue-1.1.0.dev3/pyproject.toml` & `meringue-1.1.0.dev5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 	"Django>=1.11.17",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 modeltranslation = ["django-modeltranslation>=0.17,<0.19"]
 drf = ["djangorestframework>=3.13,<4"]
+drf-spectacular = ["drf-spectacular>=0.26.3,<1"]
 
 [project.urls]
 "Homepage" = "https://github.com/dd/Meringue"
 "Documentation" = "https://dd.github.io/Meringue/"
 "Repository" = "https://github.com/dd/Meringue"
 "Changelog" = "https://github.com/dd/Meringue/blob/master/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/dd/Meringue/issues"
@@ -85,14 +86,15 @@
 description = "Dev environment"
 python = "3.11"
 dependencies = [
 	"pre-commit==3.3.3",
 	"ipython==8.14.0",
 	"pycryptodome==3.18.0",
 	"djangorestframework==3.14.0",
+	"drf-spectacular==0.26.4",
 ]
 [tool.hatch.envs.default.scripts]
 precommit_install = "pre-commit install {args}"
 precommit_uninstall = "pre-commit uninstall {args}"
 init = [
 	"git config --local gitflow.branch.master \"master\"",
 	"git config --local gitflow.branch.develop \"dev\"",
@@ -114,15 +116,15 @@
 compilemessages = "cd meringue && django-admin compilemessages -l en -l ru {args}"
 
 [tool.hatch.envs.lint]
 description = "Lint environment"
 detached = true
 python = "3.11"
 dependencies = [
-	"ruff==0.0.278",
+	"ruff==0.0.280",
 	"black==23.7.0",
 ]
 [tool.hatch.envs.lint.scripts]
 check = [
 	"ruff {args:.}",
 	"black --check --diff --exclude=\".*migrations\\/.*$\" {args:.}",
 ]
@@ -135,20 +137,21 @@
 description = "Tests environment"
 detached = true
 python = "3.11"
 dependencies = [
 	"pytest==7.4.0",
 	"pytest-django==4.5.2",
 	"pytest-cov==4.1.0",
-	"Faker==19.1.0",
+	"Faker==19.2.0",
 	"django==4.2",
 	"pytz==2023.3",
 	"django-modeltranslation==0.18.11",
 	"pycryptodome==3.18.0",
 	"djangorestframework==3.14.0",
+	"drf-spectacular==0.26.4",
 ]
 [tool.hatch.envs.test.env-vars]
 DJANGO_SETTINGS_MODULE = 'test_project.settings'
 PYTHONPATH  = '.'
 [tool.hatch.envs.test.scripts]
 check = "pytest {args:--cov=meringue --cov-report term-missing}"
 makemigrations = "django-admin makemigrations {args}"
@@ -156,17 +159,18 @@
 [tool.hatch.envs.mtest]
 description = "Test matrix environment"
 detached = true
 dependencies = [
 	"pytest==7.4.0",
 	"pytest-django==4.5.2",
 	"pytest-cov==4.1.0",  # for ci tests with cover
-	"Faker==19.1.0",
+	"Faker==19.2.0",
 	"pytz==2023.3",
 	"pycryptodome==3.18.0",
+	"drf-spectacular==0.26.4",
 ]
 [tool.hatch.envs.mtest.overrides]
 matrix.django.dependencies = [
 	{ value = "django~={matrix:django}" },
 	{ value = "django-modeltranslation=={matrix:modeltranslation}" },
 	{ value = "djangorestframework=={matrix:djangorestframework}" },
 ]
@@ -189,19 +193,19 @@
 [tool.hatch.envs.docs]
 description = "Docs environment"
 detached = true
 python = "3.11"
 dependencies = [
 	"mkdocs[i18n]==1.4.3",
 	"mkdocs-literate-nav==0.6.0",
-	"mkdocs-material==9.1.17",
+	"mkdocs-material==9.1.19",
 	"mkdocs-git-revision-date-localized-plugin==1.2.0",
 	"mkdocs-git-authors-plugin==0.7.2",
 	"mkdocstrings[python]==0.22.0",
-	"black==23.3.0",
+	"black==23.7.0",
 	"mkdocs-minify-plugin==0.6.4",
 	"mkdocs-gen-files==0.5.0",
 	"Pygments==2.15.1",
 	"mike==1.1.2",
 	"linkchecker==10.2.1",
 ]
 [tool.hatch.envs.docs.env-vars]
@@ -214,20 +218,20 @@
 validate = "linkchecker --config .linkcheckerrc docs/dist"
 build-check = [
 	"build --no-directory-urls",
 	"validate",
 ]
 
 [tool.black]
-line-length = 99
+line-length = 100
 target-version = ["py311"]
 
 [tool.ruff]
 target-version = "py311"
-line-length = 99
+line-length = 100
 show-fixes = true
 # update-check = true
 select = [
 	"A",
 	"B",
 	"C",
 	"DTZ",
@@ -270,15 +274,15 @@
 ]
 # unfixable = [
 # 	# Don't touch unused imports
 # 	"F401",
 # ]
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401", "F403"]
-"test_*.py" = ["S101", "PLR2004", "DTZ001"]
+"test_*.py" = ["S101", "PLR2004", "DTZ001", "RUF012"]
 "*/migrations/*" = ["I", "E", "Q", "RUF"]
 "test_project/*models.py" = ["RUF012"]
 "test_project/*views.py" = ["RUF012"]
 [tool.ruff.flake8-import-conventions]
 [tool.ruff.flake8-import-conventions.extend-aliases]
 "datetime" = "dt"
 # [tool.ruff.flake8-quotes]
```

### Comparing `meringue-1.1.0.dev3/PKG-INFO` & `meringue-1.1.0.dev5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meringue
-Version: 1.1.0.dev3
+Version: 1.1.0.dev5
 Summary: A set of various functionality for a Django based web application.
 Project-URL: Homepage, https://github.com/dd/Meringue
 Project-URL: Documentation, https://dd.github.io/Meringue/
 Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues
 Author-email: Dmitry Dobrynin <dd@manin.space>
@@ -45,14 +45,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Requires-Dist: django>=1.11.17
 Provides-Extra: drf
 Requires-Dist: djangorestframework<4,>=3.13; extra == 'drf'
+Provides-Extra: drf-spectacular
+Requires-Dist: drf-spectacular<1,>=0.26.3; extra == 'drf-spectacular'
 Provides-Extra: modeltranslation
 Requires-Dist: django-modeltranslation<0.19,>=0.17; extra == 'modeltranslation'
 Description-Content-Type: text/markdown
 
 <h1 align="center" >Meringue</h1>
 
 <p align="center">
@@ -118,29 +120,29 @@
 However, if someone decides to use this functionality in their project, and even more so to add functionality or change the implementation to a more correct, beautiful or understandable one, I will only be happy, do not worry and feel free to write to me by [mail](mailto:dd@manin.space), create an [issue](https://github.com/dd/Meringue/issues) or [pull request](https://github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue).
 
 
 ## Roadmap
 
 Adding new functionality. Can change.
 
-* [x] Universal manager worked with all abstract models
-* [x] Tests of all functionality
+* [x] Universal manager worked with all abstract models.
+* [x] Tests of all functionality.
 * [x] Methods for encrypting and decrypting text content (To create various secrets, such as a link to change your password or activate your profile).
 * [x] Functionality for obtaining absolute links to resources presented on the front, located on another domain (When working through api) (utils methods, template tags and filters).
-* [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
- generating form based on response from api).
+* [ ] [drf](https://www.django-rest-framework.org/) serializer serializer for automatic form generation on the front when working through rest api. (An npm package on [vuejs](https://vuejs.org/) will also be developed generating form based on response from api).
 * [x] Extended [drf router](https://www.django-rest-framework.org/api-guide/routers/) that allows you to add resources like `/profile` returning the profile data of an authorized user without his id.
 * [ ] Authorization backend for authorization by a pair of email and password.
-* [ ] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
+* [x] Helpers to extend documentation generated by [drf-spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to easily add links to different deployed environments (production, test, local, etc.) or let's say for more digestible tags instead of initially generated ones
+* [x] drf-spectacular view with patching documentation.
 * [ ] Functionality for working with images.
 	* [ ] Image editor like easy_thumbnails.
 	* [ ] A field for the drf serializer that returns a set of images (for example, a standard image and a double-sized image for a retina screen), as well as in different formats (for example, in the original format and in webp).
 * [ ] Functionality similar to that described in the previous paragraph only for video.
 * [ ] Functionality for loading private files available through [nginx internal](http://nginx.org/en/docs/http/ngx_http_core_module.html#internal).
-* [x] Exception handler for drf that returns an error code in addition to the error text
+* [x] Exception handler for drf that returns an error code in addition to the error text.
 
 
 ## Contributing
 
 - [x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to resolve the versioning
 - [x] Linter with a [Ruff](https://github.com/charliermarsh/ruff)
 - [x] Formatter with a [Black](https://github.com/psf/black)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: meringue Version: 1.1.0.dev3 Summary: A set of
+Metadata-Version: 2.1 Name: meringue Version: 1.1.0.dev5 Summary: A set of
 various functionality for a Django based web application. Project-URL:
 Homepage, https://github.com/dd/Meringue Project-URL: Documentation, https://
 dd.github.io/Meringue/ Project-URL: Repository, https://github.com/dd/Meringue
 Project-URL: Changelog, https://github.com/dd/Meringue/blob/master/CHANGELOG.md
 Project-URL: Bug Tracker, https://github.com/dd/Meringue/issues Author-email:
 Dmitry Dobrynin
 manin.space> License-Expression: LGPL-3.0 License-File: AUTHORS License-File:
@@ -24,17 +24,18 @@
 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet ::
 WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Classifier: Topic :: Software
 Development :: Libraries Requires-Python: >=3.10 Requires-Dist: django>=1.11.17
 Provides-Extra: drf Requires-Dist: djangorestframework<4,>=3.13; extra == 'drf'
-Provides-Extra: modeltranslation Requires-Dist: django-
-modeltranslation<0.19,>=0.17; extra == 'modeltranslation' Description-Content-
-Type: text/markdown
+Provides-Extra: drf-spectacular Requires-Dist: drf-spectacular<1,>=0.26.3;
+extra == 'drf-spectacular' Provides-Extra: modeltranslation Requires-Dist:
+django-modeltranslation<0.19,>=0.17; extra == 'modeltranslation' Description-
+Content-Type: text/markdown
                             ****** Meringue ******
  [PyPI_-_Status] [PyPI_-_Version] [PyPI_-_Downloads]  [PyPI_-_Python_Version]
         [Documentation_-_Release] [Tests_-_Running] [Tests_-_Coverage]
  [Hatch_project] [Material_for_MkDocs] [linting_-_Ruff] [code_style_-_black]
               [License_-_GNU_Lesser_General_Public_License_v3.0]
 Full documentation for the project is available at [dd.github.io/Meringue]
 (https://dd.github.io/Meringue/). Package with various functional (such as
@@ -45,42 +46,43 @@
 works. However, if someone decides to use this functionality in their project,
 and even more so to add functionality or change the implementation to a more
 correct, beautiful or understandable one, I will only be happy, do not worry
 and feel free to write to me by [mail](mailto:dd@manin.space), create an
 [issue](https://github.com/dd/Meringue/issues) or [pull request](https://
 github.com/dd/Meringue/pulls) on [github](https://github.com/dd/Meringue). ##
 Roadmap Adding new functionality. Can change. * [x] Universal manager worked
-with all abstract models * [x] Tests of all functionality * [x] Methods for
+with all abstract models. * [x] Tests of all functionality. * [x] Methods for
 encrypting and decrypting text content (To create various secrets, such as a
 link to change your password or activate your profile). * [x] Functionality for
 obtaining absolute links to resources presented on the front, located on
 another domain (When working through api) (utils methods, template tags and
 filters). * [ ] [drf](https://www.django-rest-framework.org/) serializer
 serializer for automatic form generation on the front when working through rest
 api. (An npm package on [vuejs](https://vuejs.org/) will also be developed
 generating form based on response from api). * [x] Extended [drf router](https:
 //www.django-rest-framework.org/api-guide/routers/) that allows you to add
 resources like `/profile` returning the profile data of an authorized user
 without his id. * [ ] Authorization backend for authorization by a pair of
-email and password. * [ ] Helpers to extend documentation generated by [drf-
+email and password. * [x] Helpers to extend documentation generated by [drf-
 spectacular](https://drf-spectacular.readthedocs.io/) - just a small helper to
 easily add links to different deployed environments (production, test, local,
 etc.) or let's say for more digestible tags instead of initially generated ones
-* [ ] Functionality for working with images. * [ ] Image editor like
-easy_thumbnails. * [ ] A field for the drf serializer that returns a set of
-images (for example, a standard image and a double-sized image for a retina
-screen), as well as in different formats (for example, in the original format
-and in webp). * [ ] Functionality similar to that described in the previous
-paragraph only for video. * [ ] Functionality for loading private files
-available through [nginx internal](http://nginx.org/en/docs/http/
-ngx_http_core_module.html#internal). * [x] Exception handler for drf that
-returns an error code in addition to the error text ## Contributing - [x] Use
-Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and [here](https:
-//www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)) to
-resolve the versioning - [x] Linter with a [Ruff](https://github.com/
-charliermarsh/ruff) - [x] Formatter with a [Black](https://github.com/psf/
-black) - [x] Lint commit with [Gitlint](https://jorisroovers.com/gitlint/) and
-[Conventional Commits](https://www.conventionalcommits.org/) - [x]
-Documentation with [mkdocs](https://www.mkdocs.org/) and [mkdocs-material]
-(https://squidfunk.github.io/mkdocs-material/) - [x] Testing local with [hatch]
-(https://hatch.pypa.io/1.7/meta/faq/#environments) - [x] Testing in CI/CD on
-push - [ ] Add [mypy](https://mypy-lang.org/) ???
+* [x] drf-spectacular view with patching documentation. * [ ] Functionality for
+working with images. * [ ] Image editor like easy_thumbnails. * [ ] A field for
+the drf serializer that returns a set of images (for example, a standard image
+and a double-sized image for a retina screen), as well as in different formats
+(for example, in the original format and in webp). * [ ] Functionality similar
+to that described in the previous paragraph only for video. * [ ] Functionality
+for loading private files available through [nginx internal](http://nginx.org/
+en/docs/http/ngx_http_core_module.html#internal). * [x] Exception handler for
+drf that returns an error code in addition to the error text. ## Contributing -
+[x] Use Git Flow (read [here](https://jeffkreeftmeijer.com/git-flow/) and
+[here](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-
+workflow)) to resolve the versioning - [x] Linter with a [Ruff](https://
+github.com/charliermarsh/ruff) - [x] Formatter with a [Black](https://
+github.com/psf/black) - [x] Lint commit with [Gitlint](https://
+jorisroovers.com/gitlint/) and [Conventional Commits](https://
+www.conventionalcommits.org/) - [x] Documentation with [mkdocs](https://
+www.mkdocs.org/) and [mkdocs-material](https://squidfunk.github.io/mkdocs-
+material/) - [x] Testing local with [hatch](https://hatch.pypa.io/1.7/meta/faq/
+#environments) - [x] Testing in CI/CD on push - [ ] Add [mypy](https://mypy-
+lang.org/) ???
```

