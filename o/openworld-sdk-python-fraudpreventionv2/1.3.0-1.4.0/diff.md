# Comparing `tmp/openworld-sdk-python-fraudpreventionv2-1.3.0.tar.gz` & `tmp/openworld-sdk-python-fraudpreventionv2-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.3.0.tar", last modified: Tue Jul 18 15:00:35 2023, max compression
+gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.4.0.tar", last modified: Tue Jul 25 11:07:56 2023, max compression
```

## Comparing `openworld-sdk-python-fraudpreventionv2-1.3.0.tar` & `openworld-sdk-python-fraudpreventionv2-1.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-18 15:00:28.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-18 15:00:28.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   118595 2023-07-18 15:00:28.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:00:35.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:00:35.514364 openworld-sdk-python-fraudpreventionv2-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-18 15:00:21.000000 openworld-sdk-python-fraudpreventionv2-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:56.476272 openworld-sdk-python-fraudpreventionv2-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-25 11:07:56.476272 openworld-sdk-python-fraudpreventionv2-1.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:56.472272 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:56.472272 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld/sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:56.472272 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld/sdk/fraudpreventionv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-25 11:07:49.000000 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld/sdk/fraudpreventionv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-25 11:07:49.000000 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld/sdk/fraudpreventionv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118595 2023-07-25 11:07:49.000000 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld/sdk/fraudpreventionv2/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:56.476272 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld_sdk_python_fraudpreventionv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-25 11:07:56.000000 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-25 11:07:56.000000 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:07:56.000000 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 11:07:56.000000 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 11:07:56.000000 openworld-sdk-python-fraudpreventionv2-1.4.0/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:07:56.476272 openworld-sdk-python-fraudpreventionv2-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-25 11:07:40.000000 openworld-sdk-python-fraudpreventionv2-1.4.0/setup.py
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.3.0/PKG-INFO` & `openworld-sdk-python-fraudpreventionv2-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudpreventionv2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Open World F r a u d P r e v e n t i o n V 2 SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/__init__.py` & `openworld-sdk-python-fraudpreventionv2-1.4.0/openworld/sdk/fraudpreventionv2/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/client.py` & `openworld-sdk-python-fraudpreventionv2-1.4.0/openworld/sdk/fraudpreventionv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         r"""F r a u d P r e v e n t i o n V 2 API Client.
 
         Args:
             client_config(ClientConfig): SDK Client Configurations Holder.
         """
         python_version = platform.python_version()
         os_name, os_version, *_ = platform.platform().split('-')
-        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.3.0'
+        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.4.0'
 
         self.__api_client = ApiClient(client_config, _OpenWorldAuthClient)
 
         self.__user_agent = f'{sdk_metadata} (Python {python_version}; {os_name} {os_version})'
 
     def screen(
         self, transaction_id: UUID = uuid4(), body: OrderPurchaseScreenRequest = None
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.3.0/openworld/sdk/fraudpreventionv2/model.py` & `openworld-sdk-python-fraudpreventionv2-1.4.0/openworld/sdk/fraudpreventionv2/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -914,15 +914,15 @@
     * `SOFORT`
     * `YANDEX`
     * `WEB_MONEY`
     * `QIWI`
     * `BITCOIN`
 
     'brand' with 'DirectDebit' payment_type is an enum value with following:
-    * `EVL`
+    * `ELV`
     * `INTER_COMPANY`
 
     Attributes:
         AMERICAN_EXPRESS(Any): --
         DINERS_CLUB_INTERNATIONAL(Any): --
         BC_CARD(Any): --
         DISCOVER(Any): --
@@ -963,15 +963,15 @@
         IBP(Any): --
         LOCAL_DEBIT_CARD(Any): --
         SOFORT(Any): --
         YANDEX(Any): --
         WEB_MONEY(Any): --
         QIWI(Any): --
         BITCOIN(Any): --
-        EVL(Any): --
+        ELV(Any): --
         INTER_COMPANY(Any): --
 
     """
     AMERICAN_EXPRESS: Any = 'AMERICAN_EXPRESS'
     DINERS_CLUB_INTERNATIONAL: Any = 'DINERS_CLUB_INTERNATIONAL'
     BC_CARD: Any = 'BC_CARD'
     DISCOVER: Any = 'DISCOVER'
@@ -1012,15 +1012,15 @@
     IBP: Any = 'IBP'
     LOCAL_DEBIT_CARD: Any = 'LOCAL_DEBIT_CARD'
     SOFORT: Any = 'SOFORT'
     YANDEX: Any = 'YANDEX'
     WEB_MONEY: Any = 'WEB_MONEY'
     QIWI: Any = 'QIWI'
     BITCOIN: Any = 'BITCOIN'
-    EVL: Any = 'EVL'
+    ELV: Any = 'ELV'
     INTER_COMPANY: Any = 'INTER_COMPANY'
 
 
 class PaymentThreeDSCriteria(
     BaseModel,
     smart_union=True,
     extra=Extra.forbid,
@@ -2203,15 +2203,15 @@
     * `PAYPAL`: `PayPal`
     * `POINTS`: `Points`
     * `GIFT_CARD`: `GiftCard`
     * `INTERNET_BANK_PAYMENT`: `InternetBankPayment`
     * `DIRECT_DEBIT`: `DirectDebit`
 
     Attributes:
-        brand(Brand): The `brand` field value is the payment brand used for payment on this transaction. For credit card payment method ensure attributes mentioned in dictionary below are set to corresponding values only. Ensure to comply with the naming standards provided in below dictionary. For example, some Payment processors use “Japan Credit Bureau” but “JCB” should be used when calling Fraud API. Incorrect `brand` - `card_type` combination will result in data quality issues and result in degraded risk recommendation. 'brand' is an enum value with the following mapping with CreditCard 'card_type' attribute: *       brand                 :      card_type * ------------------------------------------------------- * `AMERICAN_EXPRESS`          : `AMERICAN_EXPRESS` * `DINERS_CLUB_INTERNATIONAL` : `DINERS_CLUB` * `BC_CARD`                   : `DINERS_CLUB` * `DISCOVER`                  : `DISCOVER` * `BC_CARD`                   : `DISCOVER` * `DINERS_CLUB_INTERNATIONAL` : `DISCOVER` * `JCB`                       : `DISCOVER` * `JCB`                       : `JCB` * `MASTER_CARD`               : `MASTER_CARD` * `MAESTRO`                   : `MASTER_CARD` * `POSTEPAY_MASTERCARD`       : `MASTER_CARD` * `SOLO`                      : `SOLO` * `SWITCH`                    : `SWITCH` * `MAESTRO`                   : `MAESTRO` * `CHINA_UNION_PAY`           : `CHINA_UNION_PAY` * `VISA`                      : `VISA` * `VISA_DELTA`                : `VISA` * `VISA_ELECTRON`             : `VISA` * `CARTA_SI`                  : `VISA` * `CARTE_BLEUE`               : `VISA` * `VISA_DANKORT`              : `VISA` * `POSTEPAY_VISA_ELECTRON`    : `VISA` * `PAYPAL`                    :  'brand' with 'Points' payment_type is an enum value with following: * `EXPEDIA_REWARDS` * `AMEX_POINTS` * `BANK_OF_AMERICA_REWARDS` * `DISCOVER_POINTS` * `MASTER_CARD_POINTS` * `CITI_THANK_YOU_POINTS` * `MERRILL_LYNCH_REWARDS` * `WELLS_FARGO_POINTS` * `DELTA_SKY_MILES` * `UNITED_POINTS` * `DISCOVER_MILES` * `ALASKA_MILES` * `RBC_REWARDS` * `BILT_REWARDS` * `ORBUCKS` * `CHEAP_CASH` * `BONUS_PLUS` * `ULTIMATE_REWARDS`  'brand' with 'GiftCard' payment_type is an enum value with following: * `GIFT_CARD`  'brand' with 'InternetBankPayment' payment_type is an enum value with following: * `IBP` * `LOCAL_DEBIT_CARD` * `SOFORT` * `YANDEX` * `WEB_MONEY` * `QIWI` * `BITCOIN`  'brand' with 'DirectDebit' payment_type is an enum value with following: * `EVL` * `INTER_COMPANY`
+        brand(Brand): The `brand` field value is the payment brand used for payment on this transaction. For credit card payment method ensure attributes mentioned in dictionary below are set to corresponding values only. Ensure to comply with the naming standards provided in below dictionary. For example, some Payment processors use “Japan Credit Bureau” but “JCB” should be used when calling Fraud API. Incorrect `brand` - `card_type` combination will result in data quality issues and result in degraded risk recommendation. 'brand' is an enum value with the following mapping with CreditCard 'card_type' attribute: *       brand                 :      card_type * ------------------------------------------------------- * `AMERICAN_EXPRESS`          : `AMERICAN_EXPRESS` * `DINERS_CLUB_INTERNATIONAL` : `DINERS_CLUB` * `BC_CARD`                   : `DINERS_CLUB` * `DISCOVER`                  : `DISCOVER` * `BC_CARD`                   : `DISCOVER` * `DINERS_CLUB_INTERNATIONAL` : `DISCOVER` * `JCB`                       : `DISCOVER` * `JCB`                       : `JCB` * `MASTER_CARD`               : `MASTER_CARD` * `MAESTRO`                   : `MASTER_CARD` * `POSTEPAY_MASTERCARD`       : `MASTER_CARD` * `SOLO`                      : `SOLO` * `SWITCH`                    : `SWITCH` * `MAESTRO`                   : `MAESTRO` * `CHINA_UNION_PAY`           : `CHINA_UNION_PAY` * `VISA`                      : `VISA` * `VISA_DELTA`                : `VISA` * `VISA_ELECTRON`             : `VISA` * `CARTA_SI`                  : `VISA` * `CARTE_BLEUE`               : `VISA` * `VISA_DANKORT`              : `VISA` * `POSTEPAY_VISA_ELECTRON`    : `VISA` * `PAYPAL`                    :  'brand' with 'Points' payment_type is an enum value with following: * `EXPEDIA_REWARDS` * `AMEX_POINTS` * `BANK_OF_AMERICA_REWARDS` * `DISCOVER_POINTS` * `MASTER_CARD_POINTS` * `CITI_THANK_YOU_POINTS` * `MERRILL_LYNCH_REWARDS` * `WELLS_FARGO_POINTS` * `DELTA_SKY_MILES` * `UNITED_POINTS` * `DISCOVER_MILES` * `ALASKA_MILES` * `RBC_REWARDS` * `BILT_REWARDS` * `ORBUCKS` * `CHEAP_CASH` * `BONUS_PLUS` * `ULTIMATE_REWARDS`  'brand' with 'GiftCard' payment_type is an enum value with following: * `GIFT_CARD`  'brand' with 'InternetBankPayment' payment_type is an enum value with following: * `IBP` * `LOCAL_DEBIT_CARD` * `SOFORT` * `YANDEX` * `WEB_MONEY` * `QIWI` * `BITCOIN`  'brand' with 'DirectDebit' payment_type is an enum value with following: * `ELV` * `INTER_COMPANY`
         method(PaymentMethod): --
         reason(Optional[PaymentReason], optional): --
         billing_name(Name): --
         billing_address(Address): --
         billing_email_address(EmailStr): Email address associated with the payment.
         authorized_amount(Optional[Amount], optional): --
         verified_amount(Optional[Amount], optional): --
@@ -2281,15 +2281,15 @@
     * `SOFORT`
     * `YANDEX`
     * `WEB_MONEY`
     * `QIWI`
     * `BITCOIN`
 
     'brand' with 'DirectDebit' payment_type is an enum value with following:
-    * `EVL`
+    * `ELV`
     * `INTER_COMPANY`
 
     """
     method: PaymentMethod = None
     reason: Optional[PaymentReason] = None
     billing_name: Name = None
     billing_address: Address = None
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.3.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO` & `openworld-sdk-python-fraudpreventionv2-1.4.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudpreventionv2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Open World F r a u d P r e v e n t i o n V 2 SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.3.0/setup.py` & `openworld-sdk-python-fraudpreventionv2-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from setuptools import setup
 
 setup(
     name='openworld-sdk-python-fraudpreventionv2',
-    version='1.3.0',
+    version='1.4.0',
     packages=['openworld.sdk.fraudpreventionv2'],
     package_dir={'openworld-sdk-python-fraudpreventionv2': '.'},
     license='Apache License, Version 2.0',
     author='Expedia Group',
     author_email='oss@expediagroup.com',
     url='https://github.com/ExpediaGroup/openworld-sdk-python',
     classifiers=[
```

