# Comparing `tmp/django_feedback_govuk-0.1.3.tar.gz` & `tmp/django_feedback_govuk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_feedback_govuk-0.1.3.tar", max compression
+gzip compressed data, was "django_feedback_govuk-0.1.4.tar", max compression
```

## Comparing `django_feedback_govuk-0.1.3.tar` & `django_feedback_govuk-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1091 2023-03-14 11:04:30.618076 django_feedback_govuk-0.1.3/LICENSE
--rw-r--r--   0        0        0     2786 2023-04-11 10:12:43.934435 django_feedback_govuk-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/__init__.py
--rw-r--r--   0        0        0       95 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/admin.py
--rw-r--r--   0        0        0     1652 2023-04-11 10:35:22.354859 django_feedback_govuk-0.1.3/django_feedback_govuk/forms.py
--rw-r--r--   0        0        0     1840 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/migrations/__init__.py
--rw-r--r--   0        0        0      920 2023-03-14 14:16:33.472164 django_feedback_govuk-0.1.3/django_feedback_govuk/models.py
--rw-r--r--   0        0        0      789 2023-04-11 10:31:05.018794 django_feedback_govuk-0.1.3/django_feedback_govuk/notify.py
--rw-r--r--   0        0        0     2061 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.3/django_feedback_govuk/settings.py
--rw-r--r--   0        0        0     3357 2023-03-14 16:49:16.438614 django_feedback_govuk-0.1.3/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
--rw-r--r--   0        0        0     2339 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
--rw-r--r--   0        0        0      180 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
--rw-r--r--   0        0        0     1399 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
--rw-r--r--   0        0        0      351 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
--rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
--rw-r--r--   0        0        0       49 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
--rw-r--r--   0        0        0       48 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
--rw-r--r--   0        0        0     1898 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
--rw-r--r--   0        0        0     1737 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
--rw-r--r--   0        0        0        0 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/templatetags/__init__.py
--rw-r--r--   0        0        0     1605 2023-04-11 10:12:43.944435 django_feedback_govuk-0.1.3/django_feedback_govuk/templatetags/feedback_tags.py
--rw-r--r--   0        0        0        0 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/__init__.py
--rw-r--r--   0        0        0      406 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/factories.py
--rw-r--r--   0        0        0     1870 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/settings.py
--rw-r--r--   0        0        0      558 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/test_views.py
--rw-r--r--   0        0        0      153 2023-04-19 11:46:43.885872 django_feedback_govuk-0.1.3/django_feedback_govuk/tests/urls.py
--rw-r--r--   0        0        0      471 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/urls.py
--rw-r--r--   0        0        0     1826 2023-03-15 17:24:02.507405 django_feedback_govuk-0.1.3/django_feedback_govuk/views.py
--rw-r--r--   0        0        0     1877 2023-04-19 11:46:43.895872 django_feedback_govuk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.3/setup.py
--rw-r--r--   0        0        0     4034 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-03-14 14:16:27.435397 django_feedback_govuk-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3779 2023-07-25 15:16:30.134524 django_feedback_govuk-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:27.435813 django_feedback_govuk-0.1.4/django_feedback_govuk/__init__.py
+-rw-r--r--   0        0        0       95 2023-03-14 14:16:27.435920 django_feedback_govuk-0.1.4/django_feedback_govuk/admin.py
+-rw-r--r--   0        0        0     1701 2023-05-12 10:41:14.673909 django_feedback_govuk-0.1.4/django_feedback_govuk/forms.py
+-rw-r--r--   0        0        0     1840 2023-03-14 15:01:24.022779 django_feedback_govuk-0.1.4/django_feedback_govuk/migrations/0001_initial.py
+-rw-r--r--   0        0        0      599 2023-05-12 10:17:33.056308 django_feedback_govuk-0.1.4/django_feedback_govuk/migrations/0002_alter_feedback_submitter.py
+-rw-r--r--   0        0        0        0 2023-03-14 14:16:27.436236 django_feedback_govuk-0.1.4/django_feedback_govuk/migrations/__init__.py
+-rw-r--r--   0        0        0      931 2023-05-12 10:17:33.056402 django_feedback_govuk-0.1.4/django_feedback_govuk/models.py
+-rw-r--r--   0        0        0      789 2023-04-19 09:27:29.084478 django_feedback_govuk-0.1.4/django_feedback_govuk/notify.py
+-rw-r--r--   0        0        0     2061 2023-03-30 14:40:03.820144 django_feedback_govuk-0.1.4/django_feedback_govuk/settings.py
+-rw-r--r--   0        0        0     3357 2023-03-14 16:21:30.430574 django_feedback_govuk-0.1.4/django_feedback_govuk/static/django_feedback_govuk/star-rating.css
+-rw-r--r--   0        0        0     2339 2023-03-27 15:26:37.000943 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html
+-rw-r--r--   0        0        0      180 2023-03-30 14:37:22.279652 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/partials/confirm.html
+-rw-r--r--   0        0        0     1399 2023-03-27 15:26:37.002076 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html
+-rw-r--r--   0        0        0      351 2023-05-12 10:41:38.860286 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/partials/submit.html
+-rw-r--r--   0        0        0       49 2023-03-14 16:54:07.004331 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/templates/confirm.html
+-rw-r--r--   0        0        0       49 2023-03-14 16:54:07.001438 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/templates/listing.html
+-rw-r--r--   0        0        0       48 2023-03-14 16:54:07.003157 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/templates/submit.html
+-rw-r--r--   0        0        0     1898 2023-03-14 16:54:07.005607 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html
+-rw-r--r--   0        0        0     1737 2023-03-27 15:26:37.001191 django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html
+-rw-r--r--   0        0        0        0 2023-03-14 16:54:07.001284 django_feedback_govuk-0.1.4/django_feedback_govuk/templatetags/__init__.py
+-rw-r--r--   0        0        0     1605 2023-03-30 14:38:34.189260 django_feedback_govuk-0.1.4/django_feedback_govuk/templatetags/feedback_tags.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:40:19.911848 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/__init__.py
+-rw-r--r--   0        0        0      406 2023-04-19 11:01:06.172436 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/factories.py
+-rw-r--r--   0        0        0     1870 2023-04-19 11:05:11.695891 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/settings.py
+-rw-r--r--   0        0        0      558 2023-04-19 11:08:49.348404 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/test_views.py
+-rw-r--r--   0        0        0      153 2023-04-19 10:48:59.640805 django_feedback_govuk-0.1.4/django_feedback_govuk/tests/urls.py
+-rw-r--r--   0        0        0      471 2023-03-27 15:26:37.002513 django_feedback_govuk-0.1.4/django_feedback_govuk/urls.py
+-rw-r--r--   0        0        0     1839 2023-07-25 15:06:50.646118 django_feedback_govuk-0.1.4/django_feedback_govuk/views.py
+-rw-r--r--   0        0        0     1877 2023-07-25 15:16:30.134442 django_feedback_govuk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4976 1970-01-01 00:00:00.000000 django_feedback_govuk-0.1.4/PKG-INFO
```

### Comparing `django_feedback_govuk-0.1.3/LICENSE` & `django_feedback_govuk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/forms.py` & `django_feedback_govuk-0.1.4/django_feedback_govuk/forms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from crispy_forms_gds.helper import FormHelper
-from crispy_forms_gds.layout import HTML, Field, Fieldset, Layout, Size, Submit
-from django.conf import settings
+from crispy_forms_gds.layout import HTML, Field, Fieldset, Hidden, Layout, Size, Submit
 from django.forms import HiddenInput, ModelForm, RadioSelect
 
 from .models import Feedback, SatisfactionOptions
 from .settings import dfg_settings
 
 
 class FeedbackForm(ModelForm):
     class Meta:
         model = Feedback
         fields = ["satisfaction", "comment", "submitter"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.fields["submitter"].widget = HiddenInput()
+        submitter = self.initial["submitter"]
+        submitter_id = str(submitter.id) if submitter.id else ""
+
+        self.fields["submitter"].required = False
         self.fields["satisfaction"].label = ""
         self.fields["satisfaction"].required = True
         self.fields["satisfaction"].widget = RadioSelect()
         self.fields["satisfaction"].choices = SatisfactionOptions.choices
         self.fields["comment"].label = ""
-        self.fields["comment"].required = True
 
         self.helper = FormHelper()
-
         self.helper.layout = Layout(
-            Field("submitter"),
+            Hidden("submitter", submitter_id),
             Fieldset(
                 Field.radios(
                     "satisfaction",
                     template="django_feedback_govuk/widgets/star_rating/star_rating.html",
                 ),
                 legend=dfg_settings.COPY_FIELD_SATISFACTION_LEGEND,
                 legend_size=Size.MEDIUM,
@@ -39,7 +39,8 @@
                 HTML(f"<p class='govuk-hint'>{dfg_settings.COPY_FIELD_COMMENT_HINT}</p>"),
                 Field("comment"),
                 legend=dfg_settings.COPY_FIELD_COMMENT_LEGEND,
                 legend_size=Size.MEDIUM,
             ),
             Submit("submit", "Send feedback"),
         )
+
```

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/migrations/0001_initial.py` & `django_feedback_govuk-0.1.4/django_feedback_govuk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/models.py` & `django_feedback_govuk-0.1.4/django_feedback_govuk/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,13 +14,13 @@
     SATISFIED = "satisfied", "Satisfied"
     VERY_SATISFIED = "very_satisfied", "Very satisfied"
 
 
 class Feedback(models.Model):
     satisfaction = models.CharField(max_length=30, choices=SatisfactionOptions.choices)
     comment = models.TextField(blank=True)
-    submitter = models.ForeignKey(get_user_model(), on_delete=models.CASCADE)
+    submitter = models.ForeignKey(get_user_model(), on_delete=models.CASCADE, null=True)
     submitted_at = models.DateTimeField(null=True, auto_now_add=True)
 
     class Meta:
         verbose_name = "Feedback Submission"
         verbose_name_plural = "Feedback Submissions"
```

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/notify.py` & `django_feedback_govuk-0.1.4/django_feedback_govuk/notify.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/settings.py` & `django_feedback_govuk-0.1.4/django_feedback_govuk/settings.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/static/django_feedback_govuk/star-rating.css` & `django_feedback_govuk-0.1.4/django_feedback_govuk/static/django_feedback_govuk/star-rating.css`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html` & `django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html` & `django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/partials/listing.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html` & `django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/radios.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html` & `django_feedback_govuk-0.1.4/django_feedback_govuk/templates/django_feedback_govuk/widgets/star_rating/star_rating.html`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/templatetags/feedback_tags.py` & `django_feedback_govuk-0.1.4/django_feedback_govuk/templatetags/feedback_tags.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/tests/settings.py` & `django_feedback_govuk-0.1.4/django_feedback_govuk/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/tests/test_views.py` & `django_feedback_govuk-0.1.4/django_feedback_govuk/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_feedback_govuk-0.1.3/django_feedback_govuk/views.py` & `django_feedback_govuk-0.1.4/django_feedback_govuk/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def feedback_confirm(request):
     return render(request, "django_feedback_govuk/templates/confirm.html")
 
 
 class UserCanViewFeedback(UserPassesTestMixin):
     def test_func(self):
-        return self.request.user.has_perm("feedback.view_feedback")
+        return self.request.user.has_perm("django_feedback_govuk.view_feedback")
 
 
 class FeedbackListingView(UserCanViewFeedback, ListView):
     template_name = "django_feedback_govuk/templates/listing.html"
     model = Feedback
     paginate_by = 5
```

### Comparing `django_feedback_govuk-0.1.3/pyproject.toml` & `django_feedback_govuk-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-feedback-govuk"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Django app to gather and send internal Government staff feedback"
 authors = ["jafacakes2011 <cameron.lamb@digitial.trade.gov.uk>", "marcelkornblum <marcel.kornblum@digitial.trade.gov.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_feedback_govuk"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `django_feedback_govuk-0.1.3/PKG-INFO` & `django_feedback_govuk-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: django-feedback-govuk
-Version: 0.1.3
-Summary: A Django app to gather and send internal Government staff feedback
-License: MIT
-Author: jafacakes2011
-Author-email: cameron.lamb@digitial.trade.gov.uk
-Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Django (>=3.2,<4.3)
-Requires-Dist: crispy-forms-gds (>=0.2.4,<0.3.0)
-Requires-Dist: django-crispy-forms (>=1.9,<2.0)
-Requires-Dist: notifications-python-client (>=8.0.0,<9.0.0)
-Description-Content-Type: text/markdown
-
 # django-feedback
 
 A Django app to gather and send internal Government staff feedback, e.g. for open beta periods
 
 ## Installation
 
 ```
@@ -40,14 +12,15 @@
 
 ```py
 INSTALLED_APPS = [
     ...
     'crispy_forms',
     'crispy_forms_gds',
     'django_feedback_govuk',
+    ...
 ]
 ```
 
 2. Create a new email template in the GovUk Notify service, making sure to create a ((feedback_url)) field.
 
 > Note that ((feedback_url)) will be a link to the listing view, not an individual piece of feedback.
 
@@ -68,14 +41,15 @@
     "SERVICE_NAME": "<your-service>",
     "FEEDBACK_NOTIFICATION_EMAIL_TEMPLATE_ID": "xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
     "FEEDBACK_NOTIFICATION_EMAIL_RECIPIENTS": ["email@example.com"],
     "COPY": {
         #...add any copy tags to override here
     }
 }
+```
 
 The copy dict contains string IDs for all user-facing copy, defaulting to the following (override
 just the fields you want to, using the `{{ service_name }}` variable if necessary for _title and _body strings):
 
 ```py
 {
     "SUBMIT_TITLE": "Give feedback on {{ service_name }}",
@@ -120,7 +94,43 @@
     path("feedback/", include(feedback_urls)),
     ...
 ]
 ```
 
 5. Set up user permissions
 
+## Pushing to PyPI
+
+- [PyPI Package](https://pypi.org/project/django-feedback-govuk/)
+- [Test PyPI Package](https://test.pypi.org/project/django-feedback-govuk/)
+
+Running `make build-package` will build the package into the `dist/` directory.
+
+Running `make push-pypi-test` will push the built package to Test PyPI.
+
+Running `make push-pypi` will push the built package to PyPI.
+
+### Setting up poetry for pushing to PyPI
+
+First you will need to add the test pypy repository to your poetry config:
+
+```
+poetry config repositories.test-pypi https://test.pypi.org/legacy/
+```
+
+Then go to https://test.pypi.org/manage/account/token/ and generate a token.
+
+Then add it to your poetry config:
+
+```
+poetry config pypi-token.test-pypi XXXXXXXX
+```
+
+Then you also need to go to https://pypi.org/manage/account/token/ to generate a token for the real PyPI.
+
+Then add it to your poetry config:
+
+```
+poetry config pypi-token.pypi XXXXXXXX
+```
+
+Now the make commands should work as expected.
```

