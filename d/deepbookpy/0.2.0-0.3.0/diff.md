# Comparing `tmp/deepbookpy-0.2.0.tar.gz` & `tmp/deepbookpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepbookpy-0.2.0.tar", max compression
+gzip compressed data, was "deepbookpy-0.3.0.tar", max compression
```

## Comparing `deepbookpy-0.2.0.tar` & `deepbookpy-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    11356 2023-06-26 18:27:36.623393 deepbookpy-0.2.0/LICENSE
--rw-r--r--   0        0        0       42 2023-07-22 19:38:53.006898 deepbookpy-0.2.0/deepbookpy/__init__.py
--rw-r--r--   0        0        0     6967 2023-07-05 23:16:47.015849 deepbookpy-0.2.0/deepbookpy/deepbook_query.py
--rw-r--r--   0        0        0    19172 2023-07-05 23:16:47.047849 deepbookpy-0.2.0/deepbookpy/deepbook_sdk.py
--rw-r--r--   0        0        0       70 2023-06-26 18:27:36.623393 deepbookpy-0.2.0/deepbookpy/utils/constant.py
--rw-r--r--   0        0        0     1195 2023-06-26 18:27:36.623393 deepbookpy-0.2.0/deepbookpy/utils/normalizer.py
--rw-r--r--   0        0        0       47 2023-07-22 19:38:53.006898 deepbookpy-0.2.0/deepbookpy/version.py
--rw-r--r--   0        0        0      411 2023-07-22 19:38:53.018898 deepbookpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      634 2023-07-22 19:38:59.115018 deepbookpy-0.2.0/setup.py
--rw-r--r--   0        0        0      310 2023-07-22 19:38:59.115230 deepbookpy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-26 18:27:36.623393 deepbookpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1371 2023-07-24 20:30:43.377606 deepbookpy-0.3.0/README.md
+-rw-r--r--   0        0        0       42 2023-07-24 13:51:37.948879 deepbookpy-0.3.0/deepbookpy/__init__.py
+-rw-r--r--   0        0        0     6985 2023-07-24 23:39:11.925948 deepbookpy-0.3.0/deepbookpy/deepbook_query.py
+-rw-r--r--   0        0        0    19172 2023-07-24 17:20:44.892315 deepbookpy-0.3.0/deepbookpy/deepbook_sdk.py
+-rw-r--r--   0        0        0       70 2023-06-26 18:27:36.623393 deepbookpy-0.3.0/deepbookpy/utils/constant.py
+-rw-r--r--   0        0        0     1195 2023-06-26 18:27:36.623393 deepbookpy-0.3.0/deepbookpy/utils/normalizer.py
+-rw-r--r--   0        0        0       47 2023-07-24 23:39:11.925948 deepbookpy-0.3.0/deepbookpy/version.py
+-rw-r--r--   0        0        0      448 2023-07-24 23:39:11.925948 deepbookpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2042 2023-07-24 23:39:17.001875 deepbookpy-0.3.0/setup.py
+-rw-r--r--   0        0        0     1723 2023-07-24 23:39:17.002214 deepbookpy-0.3.0/PKG-INFO
```

### Comparing `deepbookpy-0.2.0/LICENSE` & `deepbookpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepbookpy-0.2.0/deepbookpy/deepbook_query.py` & `deepbookpy-0.3.0/deepbookpy/deepbook_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         
         """
 
         txer = SuiTransaction(self.client)
 
         txer.move_call(
 
-            target=f"{self.package_id}::clob::get_order_status",
+            target=f"{self.package_id}::clob_v2::get_order_status",
 
             arguments= [
                 ObjectID(pool_id),
                 SuiU64(str(order_id)),
                 ObjectID(account_cap)
                 ],
 
@@ -82,15 +82,15 @@
         :param pool_id: 
             object id of the pool, created after invoking create_pool(), eg: 0xcaee8e1c046b58e55196105f1436a2337dcaa0c340a7a8c8baf65e4afb8823a4
         """
         txer = SuiTransaction(self.client)
        
         txer.move_call(
 
-            target=f"{self.package_id}::clob::get_market_price",
+            target=f"{self.package_id}::clob_v2::get_market_price",
 
             arguments= [
                 ObjectID(pool_id),
                 ],
 
             type_arguments = [token_1, token_2]
     )
@@ -117,15 +117,15 @@
 
         """
 
         txer = SuiTransaction(self.client)
 
         txer.move_call(
 
-            target=f"{self.package_id}::clob::account_balance",
+            target=f"{self.package_id}::clob_v2::account_balance",
 
             arguments= [
                 ObjectID(pool_id),
                 ObjectID(account_cap)
                 ],
 
             type_arguments = [token_1, token_2]
@@ -152,15 +152,15 @@
             object id of the accountCap, created by invoking create_account, eg: 0x6f699fef193723277559c8f499ca3706121a65ac96d273151b8e52deb29135d3
         """
         
         txer = SuiTransaction(self.client)
 
         txer.move_call(
 
-            target=f"{self.package_id}::clob::list_open_orders",
+            target=f"{self.package_id}::clob_v2::list_open_orders",
 
             arguments= [
                 ObjectID(pool_id),
                 ObjectID(account_cap)
                 ],
 
             type_arguments = [token_1, token_2]
@@ -194,15 +194,15 @@
         
         """
 
         txer = SuiTransaction(self.client)
 
         txer.move_call(
     
-            target=f"{self.package_id}::clob::get_level2_book_status_bid_side" if is_bid_side else f"{self.package_id}::clob::get_level2_book_status_ask_side",
+            target=f"{self.package_id}::clob_v2::get_level2_book_status_bid_side" if is_bid_side else f"{self.package_id}::clob_v2::get_level2_book_status_ask_side",
             
             arguments= [
                 ObjectID(pool_id),
                 SuiU64(str(lower_price)),
                 SuiU64(str(higher_price)),
                 ObjectID(normalize_sui_object_id('0x6'))
                 ],
```

### Comparing `deepbookpy-0.2.0/deepbookpy/deepbook_sdk.py` & `deepbookpy-0.3.0/deepbookpy/deepbook_sdk.py`

 * *Files identical despite different names*

### Comparing `deepbookpy-0.2.0/deepbookpy/utils/normalizer.py` & `deepbookpy-0.3.0/deepbookpy/utils/normalizer.py`

 * *Files identical despite different names*

