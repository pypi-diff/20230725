# Comparing `tmp/payload-api-0.4.6.tar.gz` & `tmp/payload-api-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payload-api-0.4.6.tar", last modified: Tue Jul 18 16:01:41 2023, max compression
+gzip compressed data, was "payload-api-0.4.7.tar", last modified: Tue Jul 25 19:58:42 2023, max compression
```

## Comparing `payload-api-0.4.6.tar` & `payload-api-0.4.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1089 2023-05-21 11:19:23.567686 payload-api-0.4.6/LICENSE
--rw-r--r--   0        0        0      673 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/__init__.py
--rw-r--r--   0        0        0      122 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/arm/__init__.py
--rw-r--r--   0        0        0     2104 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/arm/attr.py
--rw-r--r--   0        0        0     3930 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/arm/object.py
--rw-r--r--   0        0        0     7131 2023-07-17 21:59:24.811514 payload-api-0.4.6/payload/arm/request.py
--rw-r--r--   0        0        0      989 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/arm/session.py
--rw-r--r--   0        0        0     1282 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/exceptions.py
--rw-r--r--   0        0        0     2094 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/objects.py
--rw-r--r--   0        0        0     3418 2023-05-21 11:19:23.567686 payload-api-0.4.6/payload/utils.py
--rw-r--r--   0        0        0      495 2023-07-18 16:01:06.820588 payload-api-0.4.6/payload/version.py
--rw-r--r--   0        0        0      615 2023-07-18 16:01:21.664373 payload-api-0.4.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-21 11:19:23.567686 payload-api-0.4.6/tests/__init__.py
--rw-r--r--   0        0        0     4678 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/fixtures.py
--rw-r--r--   0        0        0     3250 2023-05-21 11:19:23.567686 payload-api-0.4.6/tests/test_account.py
--rw-r--r--   0        0        0     1419 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_billing.py
--rw-r--r--   0        0        0     1568 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_invoice.py
--rw-r--r--   0        0        0     1416 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_payment_link.py
--rw-r--r--   0        0        0     3446 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_payment_method.py
--rw-r--r--   0        0        0    27158 2023-07-17 21:59:24.811514 payload-api-0.4.6/tests/test_request.py
--rw-r--r--   0        0        0     3704 2023-05-21 11:19:23.567686 payload-api-0.4.6/tests/test_session.py
--rw-r--r--   0        0        0     1473 2023-05-21 11:19:23.567686 payload-api-0.4.6/tests/test_transaction.py
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 payload-api-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-21 11:19:23.567686 payload-api-0.4.7/LICENSE
+-rw-r--r--   0        0        0      673 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/arm/__init__.py
+-rw-r--r--   0        0        0     2104 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/arm/attr.py
+-rw-r--r--   0        0        0     3930 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/arm/object.py
+-rw-r--r--   0        0        0     7131 2023-07-17 21:59:24.811514 payload-api-0.4.7/payload/arm/request.py
+-rw-r--r--   0        0        0      989 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/arm/session.py
+-rw-r--r--   0        0        0     1282 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/exceptions.py
+-rw-r--r--   0        0        0     2255 2023-07-25 19:27:28.628182 payload-api-0.4.7/payload/objects.py
+-rw-r--r--   0        0        0     3418 2023-05-21 11:19:23.567686 payload-api-0.4.7/payload/utils.py
+-rw-r--r--   0        0        0      495 2023-07-18 16:01:06.820588 payload-api-0.4.7/payload/version.py
+-rw-r--r--   0        0        0      766 2023-07-25 19:47:22.165762 payload-api-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-21 11:19:23.567686 payload-api-0.4.7/tests/__init__.py
+-rw-r--r--   0        0        0     4760 2023-07-25 19:52:34.456622 payload-api-0.4.7/tests/fixtures.py
+-rw-r--r--   0        0        0      430 2023-07-25 19:53:17.275924 payload-api-0.4.7/tests/test_access_token.py
+-rw-r--r--   0        0        0     3252 2023-07-25 19:51:47.197393 payload-api-0.4.7/tests/test_account.py
+-rw-r--r--   0        0        0     1419 2023-07-17 21:59:24.811514 payload-api-0.4.7/tests/test_billing.py
+-rw-r--r--   0        0        0     1660 2023-07-25 19:53:03.976140 payload-api-0.4.7/tests/test_invoice.py
+-rw-r--r--   0        0        0     1416 2023-07-17 21:59:24.811514 payload-api-0.4.7/tests/test_payment_link.py
+-rw-r--r--   0        0        0     3552 2023-07-25 19:53:31.039700 payload-api-0.4.7/tests/test_payment_method.py
+-rw-r--r--   0        0        0    27158 2023-07-17 21:59:24.811514 payload-api-0.4.7/tests/test_request.py
+-rw-r--r--   0        0        0     3515 2023-07-25 19:51:47.201393 payload-api-0.4.7/tests/test_session.py
+-rw-r--r--   0        0        0     1473 2023-05-21 11:19:23.567686 payload-api-0.4.7/tests/test_transaction.py
+-rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 payload-api-0.4.7/PKG-INFO
```

### Comparing `payload-api-0.4.6/LICENSE` & `payload-api-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/payload/__init__.py` & `payload-api-0.4.7/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/payload/arm/attr.py` & `payload-api-0.4.7/payload/arm/attr.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/payload/arm/object.py` & `payload-api-0.4.7/payload/arm/object.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/payload/arm/request.py` & `payload-api-0.4.7/payload/arm/request.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/payload/arm/session.py` & `payload-api-0.4.7/payload/arm/session.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/payload/exceptions.py` & `payload-api-0.4.7/payload/exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/payload/objects.py` & `payload-api-0.4.7/payload/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 from .arm.object import ARMObject
 
+class AccessToken(ARMObject):
+    __spec__ = {'object': 'access_token'}
+
+class ClientToken(AccessToken):
+    __spec__ = { 'polymorphic': { 'type': 'client' } }
+
 class Account(ARMObject):
     __spec__ = { 'object': 'account' }
 
 class Customer(ARMObject):
     __spec__ = { 'object': 'customer' }
 
 class ProcessingAccount(ARMObject):
```

### Comparing `payload-api-0.4.6/payload/utils.py` & `payload-api-0.4.7/payload/utils.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/pyproject.toml` & `payload-api-0.4.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "payload-api"
-version = "0.4.6"
+version = "0.4.7"
 description = "Payload Python Library"
 authors = [
     { name = "Ian Halpern", email = "ian@payload.co" },
 ]
 dependencies = [
     "requests",
     "six",
@@ -30,8 +30,19 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "black",
     "pathlib",
     "pytest",
     "python-dateutil",
     "mock",
+    "pylint",
 ]
+
+[tool.pdm.scripts._]
+env_file = ".env"
+
+[tool.black]
+line-length = 96
+target-version = [
+    "py38",
+]
+skip-string-normalization = true
```

### Comparing `payload-api-0.4.6/tests/test_account.py` & `payload-api-0.4.7/tests/test_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,31 +49,31 @@
             [
                 pl.Customer(email="account1@example.com", name="Randy Robson"),
                 pl.Customer(email="account2@example.com", name="Brandy Bobson"),
                 pl.Customer(email="account3@example.com", name="Mandy Johnson"),
             ]
         )
 
-        customers = pl.Customer.filter_by(
-            order_by="created_at", limit=3, offset=1
-        ).all()
+        customers = pl.Customer.filter_by(order_by="created_at", limit=3, offset=1).all()
 
         assert len(customers) == 3
-        assert dateutil.parser.parse(customers[0].created_at) < dateutil.parser.parse(customers[1].created_at)
-        assert dateutil.parser.parse(customers[1].created_at) < dateutil.parser.parse(customers[2].created_at)
+        assert dateutil.parser.parse(customers[0].created_at) <= dateutil.parser.parse(
+            customers[1].created_at
+        )
+        assert dateutil.parser.parse(customers[1].created_at) <= dateutil.parser.parse(
+            customers[2].created_at
+        )
 
     def test_update_cust(self, api_key, customer_account):
         customer_account.update(email="test2@example.com")
 
         assert customer_account.email == "test2@example.com"
 
     def test_update_mult_acc(self, api_key):
-        customer_account_1 = pl.Customer.create(
-            name="Brandy", email="test1@example.com"
-        )
+        customer_account_1 = pl.Customer.create(name="Brandy", email="test1@example.com")
         customer_account_2 = pl.Customer.create(name="Sandy", email="test2@example.com")
 
         pl.update(
             [
                 [customer_account_1, {"email": "brandy@example.com"}],
                 [customer_account_2, {"email": "sandy@example.com"}],
             ]
```

### Comparing `payload-api-0.4.6/tests/test_billing.py` & `payload-api-0.4.7/tests/test_billing.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/tests/test_invoice.py` & `payload-api-0.4.7/tests/test_invoice.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,49 +4,52 @@
 
 import payload as pl
 
 from .fixtures import Fixtures
 from payload.exceptions import NotFound
 
 
-
 @pytest.fixture
 def invoice(processing_account, customer_account):
     invoice = pl.Invoice.create(
-        type="bill",
+        type='bill',
         processing_id=processing_account.id,
         due_date=datetime.datetime.today().strftime('%Y-%m-%d'),
         customer_id=customer_account.id,
         items=[pl.ChargeItem(amount=29.99)],
     )
 
     return invoice
 
 
 class TestInvoice(Fixtures):
     def test_create_invoice(self, invoice):
         assert invoice.due_date == datetime.datetime.today().strftime('%Y-%m-%d')
-        assert invoice.status == "unpaid"
+        assert invoice.status == 'unpaid'
 
     def test_pay_invoice(self, invoice, customer_account):
         assert invoice.due_date == datetime.datetime.today().strftime('%Y-%m-%d')
-        assert invoice.status == "unpaid"
+        assert invoice.status == 'unpaid'
 
         card_payment = pl.Card.create(
-            account_id=customer_account.id, card_number="4242 4242 4242 4242", expiry='12/35', card_code='123'
+            account_id=customer_account.id,
+            card_number='4242 4242 4242 4242',
+            expiry='12/35',
+            card_code='123',
+            billing_address=dict(postal_code='11111'),
         )
 
-        if invoice.status != "paid":
+        if invoice.status != 'paid':
             pl.Payment.create(
                 amount=invoice.amount_due,
                 customer_id=customer_account.id,
                 payment_method_id=card_payment.id,
                 allocations=[pl.PaymentItem(invoice_id=invoice.id)],
             )
 
         get_invoice = pl.Invoice.get(invoice.id)
-        assert get_invoice.status == "paid"
+        assert get_invoice.status == 'paid'
 
     def test_delete_invoice(self, invoice):
         with pytest.raises(NotFound):
             invoice.delete()
-            invoice_get = pl.Invoice.get(invoice.id)
+            invoice_get = pl.Invoice.get(invoice.id)
```

### Comparing `payload-api-0.4.6/tests/test_payment_link.py` & `payload-api-0.4.7/tests/test_payment_link.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/tests/test_payment_method.py` & `payload-api-0.4.7/tests/test_payment_method.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,97 +7,99 @@
 from payload.exceptions import BadRequest
 
 from .fixtures import Fixtures
 
 
 class TestPaymentMethod(Fixtures):
     def test_create_payment_card(self, api_key, card_payment):
-        assert card_payment.status == "processed"
+        assert card_payment.status == 'processed'
 
     def test_create_payment_bank(self, api_key, bank_payment):
-        assert bank_payment.status == "processed"
+        assert bank_payment.status == 'processed'
 
     def test_payment_filters(self, api_key, processing_account):
         letters = string.ascii_lowercase
-        rand_description = "".join(random.choice(letters) for i in range(10))
+        rand_description = ''.join(random.choice(letters) for i in range(10))
 
         card_payment = pl.Payment.create(
             amount=100.0,
             description=rand_description,
             processing_id=processing_account.id,
             payment_method=pl.Card(
-                card_number="4242 4242 4242 4242", expiry="05/35", card_code="123"
+                card_number='4242 4242 4242 4242', expiry='05/35', card_code='123'
             ),
         )
 
         payments = pl.Payment.filter_by(
             pl.attr.amount > 99,
             pl.attr.amount < (200),
             pl.attr.description.contains(rand_description),
-            pl.attr.created_at > ("2019-12-31"),
+            pl.attr.created_at > ('2019-12-31'),
         ).all()
 
         assert len(payments) == 1
         assert payments[0].id == card_payment.id
 
     def test_void_card_payment(self, api_key, card_payment):
-        card_payment.update(status="voided")
+        card_payment.update(status='voided')
 
-        assert card_payment.status == "voided"
+        assert card_payment.status == 'voided'
 
     def test_void_bank_payment(self, api_key, bank_payment):
-        bank_payment.update(status="voided")
+        bank_payment.update(status='voided')
 
-        assert bank_payment.status == "voided"
+        assert bank_payment.status == 'voided'
 
     def test_refund_card_payment(self, api_key, card_payment):
-
         refund = pl.Refund.create(
-            amount=100, ledger=[pl.Ledger(assoc_transaction_id=card_payment.id)]
+            amount=card_payment.amount, ledger=[pl.Ledger(assoc_transaction_id=card_payment.id)]
         )
 
-        assert refund.type == "refund"
-        assert refund.amount == 100
-        assert refund.status_code == "approved"
+        assert refund.type == 'refund'
+        assert refund.amount == card_payment.amount
+        assert refund.status_code == 'approved'
 
     def test_partial_refund_card_payment(self, api_key, card_payment):
-
         refund = pl.Refund.create(
             amount=10, ledger=[pl.Ledger(assoc_transaction_id=card_payment.id)]
         )
 
-        assert refund.type == "refund"
+        assert refund.type == 'refund'
         assert refund.amount == 10
-        assert refund.status_code == "approved"
+        assert refund.status_code == 'approved'
 
     def test_blind_refund_card_payment(self, api_key, processing_account):
         refund = pl.Refund.create(
             amount=10,
             processing_id=processing_account.id,
-            payment_method=pl.Card(card_number="4242 4242 4242 4242", expiry="12/25", card_code='123'),
+            payment_method=pl.Card(
+                card_number='4242 4242 4242 4242', expiry='12/25', card_code='123'
+            ),
         )
 
-        assert refund.type == "refund"
+        assert refund.type == 'refund'
         assert refund.amount == 10
-        assert refund.status_code == "approved"
+        assert refund.status_code == 'approved'
 
     def test_refund_bank_payment(self, api_key, bank_payment):
         refund = pl.Refund.create(
-            amount=100, ledger=[pl.Ledger(assoc_transaction_id=bank_payment.id)]
+            amount=bank_payment.amount, ledger=[pl.Ledger(assoc_transaction_id=bank_payment.id)]
         )
 
-        assert refund.type == "refund"
+        assert refund.type == 'refund'
         assert refund.amount == bank_payment.amount
-        assert refund.status_code == "approved"
+        assert refund.status_code == 'approved'
 
     def test_partial_refund_bank_payment(self, api_key, bank_payment):
         refund = pl.Refund.create(
             amount=10, ledger=[pl.Ledger(assoc_transaction_id=bank_payment.id)]
         )
 
-        assert refund.type == "refund"
+        assert refund.type == 'refund'
         assert refund.amount == 10
-        assert refund.status_code == "approved"
+        assert refund.status_code == 'approved'
 
     def test_invalid_payment_method_type_invalid_attributes(self, api_key):
         with pytest.raises(BadRequest):
-            pl.Transaction.create(type="invalid", card_number="4242 4242 4242 4242", expiry="12/25")
+            pl.Transaction.create(
+                type='invalid', card_number='4242 4242 4242 4242', expiry='12/25'
+            )
```

### Comparing `payload-api-0.4.6/tests/test_request.py` & `payload-api-0.4.7/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.6/tests/test_session.py` & `payload-api-0.4.7/tests/test_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 import payload
 from payload.exceptions import BadRequest, NotFound
 
 from .fixtures import Fixtures
 
 import dateutil.parser
 
+
 @pytest.fixture
 def pl():
     payload.api_key = None
     pl = payload.Session(os.environ["TEST_SECRET_KEY"])
     if "TEST_API_URL" in os.environ:
         pl.api_url = os.environ["TEST_API_URL"]
 
     return pl
 
+
 class TestSession(Fixtures):
     def test_create_customer_account(self, pl):
         customer_account = pl.Customer.create(name="Test", email="test@example.com")
         assert customer_account.id
 
     def test_delete(self, pl):
         customer_account = pl.Customer.create(name="Test", email="test@example.com")
@@ -44,45 +46,41 @@
 
         get_account_1 = pl.Customer.filter_by(email=rand_email1).all()[0]
         get_account_2 = pl.Customer.filter_by(email=rand_email2).all()[0]
 
         assert get_account_1
         assert get_account_2
 
-    #def test_get_processing_account(self, api_key, processing_account):
-    #    assert pl.ProcessingAccount.get(processing_account.id)
-    #    assert processing_account.status == "pending"
-
     def test_paging_and_ordering_results(self, pl):
         accounts = pl.create(
             [
                 pl.Customer(email="account1@example.com", name="Randy Robson"),
                 pl.Customer(email="account2@example.com", name="Brandy Bobson"),
                 pl.Customer(email="account3@example.com", name="Mandy Johnson"),
             ]
         )
 
-        customers = pl.Customer.filter_by(
-            order_by="created_at", limit=3, offset=1
-        ).all()
+        customers = pl.Customer.filter_by(order_by="created_at", limit=3, offset=1).all()
 
         assert len(customers) == 3
-        assert dateutil.parser.parse(customers[0].created_at) < dateutil.parser.parse(customers[1].created_at)
-        assert dateutil.parser.parse(customers[1].created_at) < dateutil.parser.parse(customers[2].created_at)
+        assert dateutil.parser.parse(customers[0].created_at) <= dateutil.parser.parse(
+            customers[1].created_at
+        )
+        assert dateutil.parser.parse(customers[1].created_at) <= dateutil.parser.parse(
+            customers[2].created_at
+        )
 
     def test_update_cust(self, pl):
         customer_account = pl.Customer.create(name="Test", email="test@example.com")
         customer_account.update(email="test2@example.com")
 
         assert customer_account.email == "test2@example.com"
 
     def test_update_mult_acc(self, pl):
-        customer_account_1 = pl.Customer.create(
-            name="Brandy", email="test1@example.com"
-        )
+        customer_account_1 = pl.Customer.create(name="Brandy", email="test1@example.com")
         customer_account_2 = pl.Customer.create(name="Sandy", email="test2@example.com")
 
         pl.update(
             [
                 [customer_account_1, {"email": "brandy@example.com"}],
                 [customer_account_2, {"email": "sandy@example.com"}],
             ]
```

### Comparing `payload-api-0.4.6/tests/test_transaction.py` & `payload-api-0.4.7/tests/test_transaction.py`

 * *Files identical despite different names*

