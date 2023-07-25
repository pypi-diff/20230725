# Comparing `tmp/otree_vcee_payment-0.9.0.tar.gz` & `tmp/otree-vcee-payment-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "otree-vcee-payment-0.9.1.tar", last modified: Tue Jul 25 15:04:12 2023, max compression
```

## Comparing `otree_vcee_payment-0.9.0.tar` & `otree-vcee-payment-0.9.1.tar`

### file list

```diff
@@ -1,38 +1,26 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/.flake8
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/.isort.cfg
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/Procfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/__init__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/manage.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/requirements.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/runtime.txt
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/_static/global/empty.css
--rw-r--r--   0        0        0   166949 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/_static/vceepayment/vcee_logo.jpg
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/_templates/global/Page.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/__init__.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/encryption.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/models.py
--rw-r--r--   0        0        0     3791 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/pages.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/tests.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/_builtin/__init__.py
--rw-r--r--   0        0        0   166949 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/static/vceepayment/vcee_logo.jpg
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/ConfirmationPage.html
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/PaymentInfos.html
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/admin_report.html
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/pyvenv.cfg
--rw-r--r--   0        0        0     8834 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/Activate.ps1
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/activate
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/activate.csh
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/activate.fish
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/django-admin
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/django-admin.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/otree
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/pip
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/pip3
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/pip3.8
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/venvmac/bin/sqlformat
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/.gitignore
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/README.rst
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 otree_vcee_payment-0.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 15:04:12.717427 otree-vcee-payment-0.9.1/
+-rw-rw-rw-   0        0        0      120 2023-07-25 13:50:51.000000 otree-vcee-payment-0.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2773 2023-07-25 15:04:12.718425 otree-vcee-payment-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2139 2023-07-25 15:03:40.000000 otree-vcee-payment-0.9.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-25 15:04:12.630480 otree-vcee-payment-0.9.1/otree_vcee_payment.egg-info/
+-rw-rw-rw-   0        0        0     2773 2023-07-25 15:04:12.000000 otree-vcee-payment-0.9.1/otree_vcee_payment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-07-25 15:04:12.000000 otree-vcee-payment-0.9.1/otree_vcee_payment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 15:04:12.000000 otree-vcee-payment-0.9.1/otree_vcee_payment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-25 15:04:12.000000 otree-vcee-payment-0.9.1/otree_vcee_payment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-25 15:04:12.000000 otree-vcee-payment-0.9.1/otree_vcee_payment.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      774 2023-07-25 15:04:12.721423 otree-vcee-payment-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-07-25 13:50:51.000000 otree-vcee-payment-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:04:12.682448 otree-vcee-payment-0.9.1/vceepayment/
+-rw-rw-rw-   0        0        0        0 2021-01-27 15:35:43.000000 otree-vcee-payment-0.9.1/vceepayment/__init__.py
+-rw-rw-rw-   0        0        0     2114 2021-01-27 15:35:43.000000 otree-vcee-payment-0.9.1/vceepayment/encryption.py
+-rw-rw-rw-   0        0        0     1283 2023-07-25 13:46:01.000000 otree-vcee-payment-0.9.1/vceepayment/models.py
+-rw-rw-rw-   0        0        0     3791 2023-07-24 13:28:35.000000 otree-vcee-payment-0.9.1/vceepayment/pages.py
+drwxrwxrwx   0        0        0        0 2023-07-25 15:04:12.551528 otree-vcee-payment-0.9.1/vceepayment/static/
+drwxrwxrwx   0        0        0        0 2023-07-25 15:04:12.692442 otree-vcee-payment-0.9.1/vceepayment/static/vceepayment/
+-rw-rw-rw-   0        0        0   166949 2023-07-24 13:28:35.000000 otree-vcee-payment-0.9.1/vceepayment/static/vceepayment/vcee_logo.jpg
+drwxrwxrwx   0        0        0        0 2023-07-25 15:04:12.557525 otree-vcee-payment-0.9.1/vceepayment/templates/
+drwxrwxrwx   0        0        0        0 2023-07-25 15:04:12.714429 otree-vcee-payment-0.9.1/vceepayment/templates/vceepayment/
+-rw-rw-rw-   0        0        0     1125 2023-07-24 13:44:33.000000 otree-vcee-payment-0.9.1/vceepayment/templates/vceepayment/ConfirmationPage.html
+-rw-rw-rw-   0        0        0     4455 2023-07-24 13:39:44.000000 otree-vcee-payment-0.9.1/vceepayment/templates/vceepayment/PaymentInfos.html
+-rw-rw-rw-   0        0        0      524 2023-07-25 13:46:01.000000 otree-vcee-payment-0.9.1/vceepayment/templates/vceepayment/admin_report.html
+-rw-rw-rw-   0        0        0     2489 2021-01-27 15:35:43.000000 otree-vcee-payment-0.9.1/vceepayment/tests.py
```

### Comparing `otree_vcee_payment-0.9.0/_static/vceepayment/vcee_logo.jpg` & `otree-vcee-payment-0.9.1/vceepayment/static/vceepayment/vcee_logo.jpg`

 * *Files identical despite different names*

### Comparing `otree_vcee_payment-0.9.0/vceepayment/encryption.py` & `otree-vcee-payment-0.9.1/vceepayment/encryption.py`

 * *Files identical despite different names*

### Comparing `otree_vcee_payment-0.9.0/vceepayment/models.py` & `otree-vcee-payment-0.9.1/vceepayment/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 output_col_names = ["full_name", "iban", "bic"]
 
 
 class Constants(BaseConstants):
     name_in_url = "vceepayment"
     players_per_group = None
     num_rounds = 1
-    default_waiting_for_others = True
+    default_waiting_for_others = False
 
 
 class Subsession(BaseSubsession):
     def vars_for_admin_report(self):
         with open("payment_info.csv", "r") as f:
             return {"file_path": f.read()}
```

### Comparing `otree_vcee_payment-0.9.0/vceepayment/pages.py` & `otree-vcee-payment-0.9.1/vceepayment/pages.py`

 * *Files identical despite different names*

### Comparing `otree_vcee_payment-0.9.0/vceepayment/tests.py` & `otree-vcee-payment-0.9.1/vceepayment/tests.py`

 * *Files identical despite different names*

### Comparing `otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/ConfirmationPage.html` & `otree-vcee-payment-0.9.1/vceepayment/templates/vceepayment/ConfirmationPage.html`

 * *Files identical despite different names*

### Comparing `otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/PaymentInfos.html` & `otree-vcee-payment-0.9.1/vceepayment/templates/vceepayment/PaymentInfos.html`

 * *Files identical despite different names*

### Comparing `otree_vcee_payment-0.9.0/vceepayment/templates/vceepayment/admin_report.html` & `otree-vcee-payment-0.9.1/vceepayment/templates/vceepayment/admin_report.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% load otree %}
-<div>You can download the payoff file here: </div>
+<div>You can download the payment file here: </div>
 <button class="btn btn-primary" onClick="download_csv()">Download CSV</button>
 
 <script>
     function download_csv() {
         var csv = "{{ file_path|escapejs }}";
         var hiddenElement = document.createElement('a');
         hiddenElement.href = 'data:text/csv;charset=utf-8,' + encodeURI(csv);
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 {% load otree %}
-You can download the payoff file here:
+You can download the payment file here:
 Download CSV
```

