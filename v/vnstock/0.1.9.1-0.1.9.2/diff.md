# Comparing `tmp/vnstock-0.1.9.1.tar.gz` & `tmp/vnstock-0.1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnstock-0.1.9.1.tar", last modified: Tue Jul 25 12:12:11 2023, max compression
+gzip compressed data, was "vnstock-0.1.9.2.tar", last modified: Tue Jul 25 14:03:49 2023, max compression
```

## Comparing `vnstock-0.1.9.1.tar` & `vnstock-0.1.9.2.tar`

### file list

```diff
@@ -1,15 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 12:12:11.712042 vnstock-0.1.9.1/
--rw-rw-rw-   0        0        0     1071 2022-02-26 11:38:24.000000 vnstock-0.1.9.1/LICENSE
--rw-rw-rw-   0        0        0    72835 2023-07-25 12:12:11.720021 vnstock-0.1.9.1/PKG-INFO
--rw-rw-rw-   0        0        0    72406 2023-07-25 12:04:09.000000 vnstock-0.1.9.1/README.md
--rw-rw-rw-   0        0        0      146 2023-06-22 12:09:26.000000 vnstock-0.1.9.1/pyproject.toml
--rw-rw-rw-   0        0        0      514 2023-07-25 12:12:11.730992 vnstock-0.1.9.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 12:12:11.654198 vnstock-0.1.9.1/vnstock/
--rw-rw-rw-   0        0        0      178 2023-07-13 14:02:40.000000 vnstock-0.1.9.1/vnstock/__init__.py
--rw-rw-rw-   0        0        0    45357 2023-07-25 12:03:57.000000 vnstock-0.1.9.1/vnstock/stock.py
--rw-rw-rw-   0        0        0     2929 2023-07-13 14:01:17.000000 vnstock-0.1.9.1/vnstock/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 12:12:11.707056 vnstock-0.1.9.1/vnstock.egg-info/
--rw-rw-rw-   0        0        0    72835 2023-07-25 12:12:11.000000 vnstock-0.1.9.1/vnstock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-07-25 12:12:11.000000 vnstock-0.1.9.1/vnstock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 12:12:11.000000 vnstock-0.1.9.1/vnstock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 12:12:11.000000 vnstock-0.1.9.1/vnstock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 14:03:49.369386 vnstock-0.1.9.2/
+-rw-rw-rw-   0        0        0     1071 2022-02-26 11:38:24.000000 vnstock-0.1.9.2/LICENSE
+-rw-rw-rw-   0        0        0    73061 2023-07-25 14:03:49.373380 vnstock-0.1.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0    72632 2023-07-25 13:50:06.000000 vnstock-0.1.9.2/README.md
+-rw-rw-rw-   0        0        0      146 2023-06-22 12:09:26.000000 vnstock-0.1.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0      514 2023-07-25 14:03:49.384375 vnstock-0.1.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 14:03:49.368389 vnstock-0.1.9.2/vnstock.egg-info/
+-rw-rw-rw-   0        0        0    73061 2023-07-25 14:03:49.000000 vnstock-0.1.9.2/vnstock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-07-25 14:03:49.000000 vnstock-0.1.9.2/vnstock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:03:49.000000 vnstock-0.1.9.2/vnstock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 14:03:49.000000 vnstock-0.1.9.2/vnstock.egg-info/top_level.txt
```

### Comparing `vnstock-0.1.9.1/LICENSE` & `vnstock-0.1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vnstock-0.1.9.1/PKG-INFO` & `vnstock-0.1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: vnstock
-Version: 0.1.9.1
+Version: 0.1.9.2
 Summary: Vietnam Stock Market Data
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: mrthinh@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div id="badges" align="center">
+<img src="https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/vnstock-logo-white.jpg" alt= "logo"/>
+</div>
+
+<div id="badges" align="center">
 <img src="https://img.shields.io/pypi/pyversions/vnstock?logoColor=brown&style=plastic" alt= "Version"/>
 <img src="https://img.shields.io/pypi/dm/vnstock" alt="Download Badge"/>
 <img src="https://img.shields.io/github/last-commit/thinh-vu/vnstock" alt="Commit Badge"/>
 <img src="https://img.shields.io/github/license/thinh-vu/vnstock?color=red" alt="License Badge"/>
 </div>
 
 ---
@@ -169,15 +173,15 @@
 
 Để nạp các hàm của vnstock vào dự án Python của bạn, cần `import` chúng thông qua câu lệnh như dưới đây. Như vậy mọi thứ đã sẵn sàng để truy cập dữ liệu do vnstock cung cấp thông qua các hàm được liệt kê trong tài liệu hướng dẫn.
 
 ```python
 from vnstock import *
 ```
 
-## 3.1. Danh sách cổ phiếu niêm yết (Listing)
+## 3.1. ☑ Danh sách cổ phiếu niêm yết (Listing)
 
 ### 3.1.1. 📰 Danh sách các công ty niêm yết
 ```python
 listing_companies()
 ```
 Hàm này đọc dữ liệu từ tệp csv đính kèm trên Github theo mặc định (trong thư mục /data của repo này). Bởi danh sách các công ty niêm yết thường không thay đổi liên tục nên việc này không gây trở ngại nhiều.
 
@@ -190,17 +194,17 @@
 0    VVS   UpcomIndex  Công ty Cổ phần Đầu tư Phát triển Máy Việt Nam  Đầu tư Phát triển Máy Việt Nam            DN          CT  ...  False  False  False  False  False  False
 1    XDC   UpcomIndex   Công ty TNHH MTV Xây dựng Công trình Tân Cảng    Xây dựng Công trình Tân Cảng            DN          CT  ...  False  False  False  False  False  False
 2    HSV   UpcomIndex           Công ty Cổ phần Tập đoàn HSV Việt Nam                Gang Thép Hà Nội            DN          CT  ...  False  False  False  False  False  False
 ```
 
 </details>
 
-## 3.2. Phân tích cơ bản (Fundamental Analysis)
+## 3.2. 🏳 Phân tích cơ bản (Fundamental Analysis)
 
-### 3.2.1. Thông tin tổng quan công ty
+### 3.2.1. 🏚 Thông tin tổng quan công ty
 
 ```python
 company_overview('TCB')
 ```
 
 <details>
   <summary>Output</summary>
@@ -621,27 +625,26 @@
 
   ![stock_scanner](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/stock_scanner_tcbs.png)
 
 </details>
 
 Tham số
 - params (dict): một từ điển chứa các tham số và giá trị của chúng cho việc lọc cổ phiếu. Các `key` là tên của các bộ lọc, và các `value` là một giá trị đơn hoặc một tupple gồm hai giá trị (min và max) cho bộ lọc đó. Đây là ví dụ cho tham số params được thiết lập đúng:
+- drop_lang: Loại bỏ các cột dữ liệu sử dụng tên tiếng Việt (`vi`) hoặc Anh (`en`)
 
 ```python
 params = {
-            "exchangeName": "HOSE",
+            "exchangeName": "HOSE,HNX,UPCOM",
             "marketCap": (100, 1000),
-            "pe": (10, 20),
-            "dividendYield": (5, 10),
-            "tcbsRecommend": "BUY",
-            "size": 50
+            "dividendYield": (5, 10)
         }
 
 # Áp dụng bộ lọc với hàm để lấy kết quả
-stock_screening_insights (params)
+
+df = stock_screening_insights (params, size=1700, drop_lang='vi')
 ```
 
 <details>
 
 <summary>Các bộ lọc gợi ý và tiêu chí hỗ trợ bao gồm</summary>
 
   a. BỘ LỌC GỢI Ý (PRESET)
```

### Comparing `vnstock-0.1.9.1/README.md` & `vnstock-0.1.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 <div id="badges" align="center">
+<img src="https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/vnstock-logo-white.jpg" alt= "logo"/>
+</div>
+
+<div id="badges" align="center">
 <img src="https://img.shields.io/pypi/pyversions/vnstock?logoColor=brown&style=plastic" alt= "Version"/>
 <img src="https://img.shields.io/pypi/dm/vnstock" alt="Download Badge"/>
 <img src="https://img.shields.io/github/last-commit/thinh-vu/vnstock" alt="Commit Badge"/>
 <img src="https://img.shields.io/github/license/thinh-vu/vnstock?color=red" alt="License Badge"/>
 </div>
 
 ---
@@ -155,15 +159,15 @@
 
 Để nạp các hàm của vnstock vào dự án Python của bạn, cần `import` chúng thông qua câu lệnh như dưới đây. Như vậy mọi thứ đã sẵn sàng để truy cập dữ liệu do vnstock cung cấp thông qua các hàm được liệt kê trong tài liệu hướng dẫn.
 
 ```python
 from vnstock import *
 ```
 
-## 3.1. Danh sách cổ phiếu niêm yết (Listing)
+## 3.1. ☑ Danh sách cổ phiếu niêm yết (Listing)
 
 ### 3.1.1. 📰 Danh sách các công ty niêm yết
 ```python
 listing_companies()
 ```
 Hàm này đọc dữ liệu từ tệp csv đính kèm trên Github theo mặc định (trong thư mục /data của repo này). Bởi danh sách các công ty niêm yết thường không thay đổi liên tục nên việc này không gây trở ngại nhiều.
 
@@ -176,17 +180,17 @@
 0    VVS   UpcomIndex  Công ty Cổ phần Đầu tư Phát triển Máy Việt Nam  Đầu tư Phát triển Máy Việt Nam            DN          CT  ...  False  False  False  False  False  False
 1    XDC   UpcomIndex   Công ty TNHH MTV Xây dựng Công trình Tân Cảng    Xây dựng Công trình Tân Cảng            DN          CT  ...  False  False  False  False  False  False
 2    HSV   UpcomIndex           Công ty Cổ phần Tập đoàn HSV Việt Nam                Gang Thép Hà Nội            DN          CT  ...  False  False  False  False  False  False
 ```
 
 </details>
 
-## 3.2. Phân tích cơ bản (Fundamental Analysis)
+## 3.2. 🏳 Phân tích cơ bản (Fundamental Analysis)
 
-### 3.2.1. Thông tin tổng quan công ty
+### 3.2.1. 🏚 Thông tin tổng quan công ty
 
 ```python
 company_overview('TCB')
 ```
 
 <details>
   <summary>Output</summary>
@@ -607,27 +611,26 @@
 
   ![stock_scanner](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/stock_scanner_tcbs.png)
 
 </details>
 
 Tham số
 - params (dict): một từ điển chứa các tham số và giá trị của chúng cho việc lọc cổ phiếu. Các `key` là tên của các bộ lọc, và các `value` là một giá trị đơn hoặc một tupple gồm hai giá trị (min và max) cho bộ lọc đó. Đây là ví dụ cho tham số params được thiết lập đúng:
+- drop_lang: Loại bỏ các cột dữ liệu sử dụng tên tiếng Việt (`vi`) hoặc Anh (`en`)
 
 ```python
 params = {
-            "exchangeName": "HOSE",
+            "exchangeName": "HOSE,HNX,UPCOM",
             "marketCap": (100, 1000),
-            "pe": (10, 20),
-            "dividendYield": (5, 10),
-            "tcbsRecommend": "BUY",
-            "size": 50
+            "dividendYield": (5, 10)
         }
 
 # Áp dụng bộ lọc với hàm để lấy kết quả
-stock_screening_insights (params)
+
+df = stock_screening_insights (params, size=1700, drop_lang='vi')
 ```
 
 <details>
 
 <summary>Các bộ lọc gợi ý và tiêu chí hỗ trợ bao gồm</summary>
 
   a. BỘ LỌC GỢI Ý (PRESET)
```

### Comparing `vnstock-0.1.9.1/setup.cfg` & `vnstock-0.1.9.2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e73 746f 636b 0d0a 7665 7273   = vnstock..vers
-00000020: 696f 6e20 3d20 302e 312e 392e 310d 0a61  ion = 0.1.9.1..a
+00000020: 696f 6e20 3d20 302e 312e 392e 320d 0a61  ion = 0.1.9.2..a
 00000030: 7574 686f 7220 3d20 5468 696e 6820 5675  uthor = Thinh Vu
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 206d 7274 6869 6e68 406c 6976 652e 636f   mrthinh@live.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2056 6965 746e 616d 2053 746f 636b 204d   Vietnam Stock M
 00000080: 6172 6b65 7420 4461 7461 0d0a 6c6f 6e67  arket Data..long
 00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
```

### Comparing `vnstock-0.1.9.1/vnstock.egg-info/PKG-INFO` & `vnstock-0.1.9.2/vnstock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: vnstock
-Version: 0.1.9.1
+Version: 0.1.9.2
 Summary: Vietnam Stock Market Data
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: mrthinh@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div id="badges" align="center">
+<img src="https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/vnstock-logo-white.jpg" alt= "logo"/>
+</div>
+
+<div id="badges" align="center">
 <img src="https://img.shields.io/pypi/pyversions/vnstock?logoColor=brown&style=plastic" alt= "Version"/>
 <img src="https://img.shields.io/pypi/dm/vnstock" alt="Download Badge"/>
 <img src="https://img.shields.io/github/last-commit/thinh-vu/vnstock" alt="Commit Badge"/>
 <img src="https://img.shields.io/github/license/thinh-vu/vnstock?color=red" alt="License Badge"/>
 </div>
 
 ---
@@ -169,15 +173,15 @@
 
 Để nạp các hàm của vnstock vào dự án Python của bạn, cần `import` chúng thông qua câu lệnh như dưới đây. Như vậy mọi thứ đã sẵn sàng để truy cập dữ liệu do vnstock cung cấp thông qua các hàm được liệt kê trong tài liệu hướng dẫn.
 
 ```python
 from vnstock import *
 ```
 
-## 3.1. Danh sách cổ phiếu niêm yết (Listing)
+## 3.1. ☑ Danh sách cổ phiếu niêm yết (Listing)
 
 ### 3.1.1. 📰 Danh sách các công ty niêm yết
 ```python
 listing_companies()
 ```
 Hàm này đọc dữ liệu từ tệp csv đính kèm trên Github theo mặc định (trong thư mục /data của repo này). Bởi danh sách các công ty niêm yết thường không thay đổi liên tục nên việc này không gây trở ngại nhiều.
 
@@ -190,17 +194,17 @@
 0    VVS   UpcomIndex  Công ty Cổ phần Đầu tư Phát triển Máy Việt Nam  Đầu tư Phát triển Máy Việt Nam            DN          CT  ...  False  False  False  False  False  False
 1    XDC   UpcomIndex   Công ty TNHH MTV Xây dựng Công trình Tân Cảng    Xây dựng Công trình Tân Cảng            DN          CT  ...  False  False  False  False  False  False
 2    HSV   UpcomIndex           Công ty Cổ phần Tập đoàn HSV Việt Nam                Gang Thép Hà Nội            DN          CT  ...  False  False  False  False  False  False
 ```
 
 </details>
 
-## 3.2. Phân tích cơ bản (Fundamental Analysis)
+## 3.2. 🏳 Phân tích cơ bản (Fundamental Analysis)
 
-### 3.2.1. Thông tin tổng quan công ty
+### 3.2.1. 🏚 Thông tin tổng quan công ty
 
 ```python
 company_overview('TCB')
 ```
 
 <details>
   <summary>Output</summary>
@@ -621,27 +625,26 @@
 
   ![stock_scanner](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/stock_scanner_tcbs.png)
 
 </details>
 
 Tham số
 - params (dict): một từ điển chứa các tham số và giá trị của chúng cho việc lọc cổ phiếu. Các `key` là tên của các bộ lọc, và các `value` là một giá trị đơn hoặc một tupple gồm hai giá trị (min và max) cho bộ lọc đó. Đây là ví dụ cho tham số params được thiết lập đúng:
+- drop_lang: Loại bỏ các cột dữ liệu sử dụng tên tiếng Việt (`vi`) hoặc Anh (`en`)
 
 ```python
 params = {
-            "exchangeName": "HOSE",
+            "exchangeName": "HOSE,HNX,UPCOM",
             "marketCap": (100, 1000),
-            "pe": (10, 20),
-            "dividendYield": (5, 10),
-            "tcbsRecommend": "BUY",
-            "size": 50
+            "dividendYield": (5, 10)
         }
 
 # Áp dụng bộ lọc với hàm để lấy kết quả
-stock_screening_insights (params)
+
+df = stock_screening_insights (params, size=1700, drop_lang='vi')
 ```
 
 <details>
 
 <summary>Các bộ lọc gợi ý và tiêu chí hỗ trợ bao gồm</summary>
 
   a. BỘ LỌC GỢI Ý (PRESET)
```

