# Comparing `tmp/vnstock-0.1.8.tar.gz` & `tmp/vnstock-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnstock-0.1.8.tar", last modified: Sat Jul 15 00:37:08 2023, max compression
+gzip compressed data, was "vnstock-0.1.9.tar", last modified: Tue Jul 25 08:17:32 2023, max compression
```

## Comparing `vnstock-0.1.8.tar` & `vnstock-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 00:37:08.523763 vnstock-0.1.8/
--rw-rw-rw-   0        0        0     1071 2022-02-26 11:38:24.000000 vnstock-0.1.8/LICENSE
--rw-rw-rw-   0        0        0    52813 2023-07-15 00:37:08.525758 vnstock-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    52384 2023-07-15 00:21:27.000000 vnstock-0.1.8/README.md
--rw-rw-rw-   0        0        0      146 2023-06-22 12:09:26.000000 vnstock-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      512 2023-07-15 00:37:08.536729 vnstock-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-15 00:37:08.483869 vnstock-0.1.8/vnstock/
--rw-rw-rw-   0        0        0      178 2023-07-13 14:02:40.000000 vnstock-0.1.8/vnstock/__init__.py
--rw-rw-rw-   0        0        0    34354 2023-07-15 00:18:25.000000 vnstock-0.1.8/vnstock/stock.py
--rw-rw-rw-   0        0        0     2929 2023-07-13 14:01:17.000000 vnstock-0.1.8/vnstock/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:37:08.519773 vnstock-0.1.8/vnstock.egg-info/
--rw-rw-rw-   0        0        0    52813 2023-07-15 00:37:08.000000 vnstock-0.1.8/vnstock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-07-15 00:37:08.000000 vnstock-0.1.8/vnstock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 00:37:08.000000 vnstock-0.1.8/vnstock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-15 00:37:08.000000 vnstock-0.1.8/vnstock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 08:17:32.770106 vnstock-0.1.9/
+-rw-rw-rw-   0        0        0     1071 2022-02-26 11:38:24.000000 vnstock-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    72842 2023-07-25 08:17:32.772101 vnstock-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    72413 2023-07-25 08:13:35.000000 vnstock-0.1.9/README.md
+-rw-rw-rw-   0        0        0      146 2023-06-22 12:09:26.000000 vnstock-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      512 2023-07-25 08:17:32.784069 vnstock-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 08:17:32.419045 vnstock-0.1.9/vnstock/
+-rw-rw-rw-   0        0        0      178 2023-07-13 14:02:40.000000 vnstock-0.1.9/vnstock/__init__.py
+-rw-rw-rw-   0        0        0    47109 2023-07-25 07:53:59.000000 vnstock-0.1.9/vnstock/stock.py
+-rw-rw-rw-   0        0        0     2929 2023-07-13 14:01:17.000000 vnstock-0.1.9/vnstock/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-25 08:17:32.767114 vnstock-0.1.9/vnstock.egg-info/
+-rw-rw-rw-   0        0        0    72842 2023-07-25 08:17:32.000000 vnstock-0.1.9/vnstock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-07-25 08:17:32.000000 vnstock-0.1.9/vnstock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 08:17:32.000000 vnstock-0.1.9/vnstock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 08:17:32.000000 vnstock-0.1.9/vnstock.egg-info/top_level.txt
```

### Comparing `vnstock-0.1.8/LICENSE` & `vnstock-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vnstock-0.1.8/PKG-INFO` & `vnstock-0.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock
-Version: 0.1.8
+Version: 0.1.9
 Summary: Vietnam Stock Market Data
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: mrthinh@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,22 +20,25 @@
 </div>
 
 ---
 
 🌐 View in **[English](https://github.com/thinh-vu/vnstock/blob/main/README-en.md)**
 
 MỤC LỤC
+
 - [I. 🎤 Giới thiệu](#i--giới-thiệu)
-- [II. 📚 Hướng dẫn sử dụng cho người mới](#ii-hướng-dẫn-sử-dụng-cho-người-mới)
+- [II. 📚 Hướng dẫn sử dụng cho người mới](#ii--hướng-dẫn-sử-dụng-cho-người-mới)
 - [III. 💻 Cách sử dụng các hàm trong vnstock](#iii--cách-sử-dụng-các-hàm-trong-vnstock)
-- [IV. 🙋‍♂️ Contact Information](#iv-️-contact-information)
-- [V. 💪 Hỗ trợ phát triển dự án vnstock](#v--hỗ-trợ-phát-triển-dự-án-vnstock)
-- [VI. ⚖ Tuyên bố miễn trừ trách nhiệm](#vi--tuyên-bố-miễn-trừ-trách-nhiệm)
+- [IV. Xuất, Lưu trữ, Chia sẻ dữ liệu](#iv-xuất-lưu-trữ-chia-sẻ-dữ-liệu)
+- [V. 🙋‍♂️ Thông tin liên hệ](#v-️-thông-tin-liên-hệ)
+- [VI. 💪 Hỗ trợ phát triển dự án vnstock](#vi--hỗ-trợ-phát-triển-dự-án-vnstock)
+- [VII. ⚖ Tuyên bố miễn trừ trách nhiệm](#vii--tuyên-bố-miễn-trừ-trách-nhiệm)
 - [VII. Bản quyền và giấy phép](#vii-bản-quyền-và-giấy-phép)
 
+
 # I. 🎤 Giới thiệu
 ## 1.1. Giới thiệu chung
 vnstock là thư viện Python được thiết kế để tải dữ liệu chứng khoán Việt Nam một cách dễ dàng và miễn phí. vnstock sử dụng các nguồn cấp dữ liệu đáng tin cậy, bao gồm nhưng không giới hạn từ công ty chứng khoán và công ty phân tích thị trường tại Việt Nam. Gói thư viện được thiết kế dựa trên nguyên tắc về sự đơn giản và mã nguồn mở, hầu hết các hàm được viết dựa trên thư viện request và pandas có sẵn trên môi trường Google Colab do đó người dùng không cần cài đặt thêm các gói thư viện kèm theo.
 
 ## 1.2. Tính năng chính
 vnstock cung cấp nhiều tính năng đa dạng như tải dữ liệu lịch sử giá, thông tin công ty niêm yết, thông tin thị trường cho tất cả các mã chứng khoán niêm yết.
 
@@ -44,20 +47,41 @@
 
 ## 1.4. Tips
 - Theo dõi những cập nhật về thay đổi của vnstock bằng tính năng `Watch`. Hiện tại vnstock được cập nhật thường xuyên hàng tuần qua nhánh `beta`, vì vậy theo dõi repo này giúp bạn luôn nắm bắt được kịp thời những thay đổi mới nhất.
 - Đánh dấu yêu thích repo `vnstock` bằng tính năng `Star`. Đây cũng là cách giúp vnstock có thể tiếp cận tới nhiều người quan tâm hơn.
 
 <details>
   <summary> Minh họa tính năng Watch và Star </summary>
+  
 ![watch-star](https://github.com/thinh-vu/vnstock/blob/beta/src/vnstock-watch-and-star.png?raw=true)
 
 </details>
 
 ## 1.5. Đóng góp xây dựng mã nguồn vnstock
-- Bạn có thể đóng góp xây dựng vnstock thông qua nhiều hình thức khác nhau, trong đó có việc xây dựng và cải tiến mã nguồn hoặc dịch tài liệu của dự án. Để bắt đầu, bạn có thể `folk` repo này về tài khoản của mình, sửa đổi mã nguồn và tạo `pull request` để yêu cầu cập nhật mã nguồn. Sau khi kiểm tra các thay đổi và phê duyệt, mã nguồn do bạn đóng góp sẽ được gộp vào vnstock.
+- Bạn có thể đóng góp xây dựng vnstock thông qua nhiều hình thức khác nhau, trong đó có việc xây dựng và cải tiến mã nguồn hoặc dịch tài liệu của dự án. 
+- Để bắt đầu, bạn có thể `folk` nhánh `beta` của repo này về tài khoản của mình, sửa đổi mã nguồn và tạo `pull request` để yêu cầu cập nhật mã nguồn. Sau khi kiểm tra các thay đổi và phê duyệt, mã nguồn do bạn đóng góp sẽ được gộp vào vnstock.
+- Lưu ý: Những thay đổi do bạn đóng góp sẽ được phát hành trong phiên bản tiếp theo của `vnstock` trên Pypi.org đồng thời với những cập nhật của tác giả trên nhánh `beta`.
+
+## 1.6. Hoàn thành khảo sát về vnstock
+> vnstock là một dự án tôi tâm huyết, đầu tư nhiều thời gian để phát triển giúp bản thân và cộng đồng tiếp cận nguồn dữ liệu chứng khoán miễn phí và đáng tin cậy.
+
+Hoàn thành bản khảo sát: [Tại đây](https://forms.gle/zaJnbgUCjjL1GoTF6)
+Để đảm bảo rằng vnstock phát triển theo hướng đáp ứng nhu cầu của bạn, tôi rất mong nhận được phản hồi từ bạn. Bạn là người dùng quan trọng của vnstock và ý kiến của bạn sẽ giúp chúng tôi xây dựng một kế hoạch phát triển vnstock một cách toàn diện.
+
+## 1.7. Dịch vụ "code dạo", gây quỹ phát triển dự án
+
+Ngoài ra, để gây quỹ phát triển dự án, tôi cũng cung cấp dịch vụ "code dạo" theo đặt hàng bao gồm nhưng không giới hạn với các hoạt động dưới đây:
+- Tải dữ liệu thị trường
+- Viết workflow quét dữ liệu, cập nhật cơ sở dữ liệu, vv
+- Thiết lập dự án phân tích chứng khoán toàn diện
+- Tạo bộ lọc cổ phiếu độc quyền
+- Tạo robot giao dịch qua API
+- Cung cấp API dữ liệu độc quyền
+
+Nếu bạn nào quan tâm và có nhu cầu, vui lòng [inbox](https://www.messenger.com/t/mr.thinh.ueh) để trao đổi thêm. Hoạt động này cũng giúp tôi hiểu thêm về những ứng dụng thực tế và phát triển vnstock trong tương lai.
 
 # II. 📚 Hướng dẫn sử dụng cho người mới
 ## 2.1. Tài nguyên quan trọng
 
 ### 2.1.2 Blog
 
 👉 Để biết thêm thông tin và minh hoạ về cách sử dụng, bạn vui lòng truy cập bài viết trên blog của tôi, có sẵn bằng tiếng Việt/Anh [tại đây](https://thinhvu.com/2022/09/22/vnstock-api-tai-du-lieu-chung-khoan-python?utm_source=github&utm_medium=vnstock).
@@ -86,14 +110,17 @@
 
 </details>
 
 ### 2.1.4. Xây dựng cộng đồng vnstock
 
 🖐 Nếu bạn thấy thư viện này có giá trị và muốn hỗ trợ tác giả duy trì vnstock dưới dạng mã nguồn mở, miễn phí thì có thể tham gia ủng hộ gây quỹ phát triển dự án này. Để biết thêm chi tiết, vui lòng tham khảo bài viết trên blog sau: [Cùng nhau xây dựng cộng đồng VNStock vững mạnh](https://thinhvu.com/2023/04/15/xay-dung-cong-dong-vnstock-vung-manh/).
 
+- Tham gia nhóm vnstock trên Facebook: [Tại đây](https://www.facebook.com/groups/vnstock)
+- Tham gia Discord channel: [Tại đây](https://discord.gg/qJvxJcChJ3)
+
 <details>
   <summary>Ủng hộ quỹ phát triển vnstock</summary>
   Nếu vnstock giúp ích cho bạn, hãy đóng góp quỹ phát triển ứng dụng này theo một trong hai hình thức sau gồm chuyển khoản ngân hàng hoặc Momo. Mọi khoản đóng góp đều đáng trân quý và là động lực giúp tác giả duy trì vnstock luôn hữu ích, miễn phí, và dễ tiếp cận cho cộng đồng.
 
   - ![vcb-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/vcb-qr-thinhvu.jpg)
   - ![momo-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/momo-qr-thinhvu.jpeg)
 
@@ -143,15 +170,17 @@
 
 Để nạp các hàm của vnstock vào dự án Python của bạn, cần `import` chúng thông qua câu lệnh như dưới đây. Như vậy mọi thứ đã sẵn sàng để truy cập dữ liệu do vnstock cung cấp thông qua các hàm được liệt kê trong tài liệu hướng dẫn.
 
 ```python
 from vnstock import *
 ```
 
-## 3.1 📰 Danh sách các công ty niêm yết
+## 3.1. ☑ Danh sách cổ phiếu niêm yết (Listing)
+
+### 3.1.1. 📰 Danh sách các công ty niêm yết
 ```python
 listing_companies()
 ```
 Hàm này đọc dữ liệu từ tệp csv đính kèm trên Github theo mặc định (trong thư mục /data của repo này). Bởi danh sách các công ty niêm yết thường không thay đổi liên tục nên việc này không gây trở ngại nhiều.
 
 <details>
   <summary>Output</summary>
@@ -162,15 +191,18 @@
 0    VVS   UpcomIndex  Công ty Cổ phần Đầu tư Phát triển Máy Việt Nam  Đầu tư Phát triển Máy Việt Nam            DN          CT  ...  False  False  False  False  False  False
 1    XDC   UpcomIndex   Công ty TNHH MTV Xây dựng Công trình Tân Cảng    Xây dựng Công trình Tân Cảng            DN          CT  ...  False  False  False  False  False  False
 2    HSV   UpcomIndex           Công ty Cổ phần Tập đoàn HSV Việt Nam                Gang Thép Hà Nội            DN          CT  ...  False  False  False  False  False  False
 ```
 
 </details>
 
-## 3.2. Tổng quan về công ty
+## 3.2. 🏳 Phân tích cơ bản (Fundamental Analysis)
+
+### 3.2.1. 🏚 Thông tin tổng quan công ty
+
 ```python
 company_overview('TCB')
 ```
 
 <details>
   <summary>Output</summary>
 
@@ -178,29 +210,168 @@
   >>> company_overview('TCB')
     exchange    shortName  industryID industryIDv2   industry  ... deltaInMonth deltaInYear  outstandingShare  issueShare  ticker
   0     HOSE  Techcombank         289         8355  Ngân hàng  ...       -0.027      -0.038            3510.9      3510.9     TCB
   ```
 
 </details>
 
-## 3.3. 📈 Truy xuất dữ liệu giá lịch sử
+### 3.2.2. 🧧 Lịch sử chi trả cổ tức
+
+```python
+dividend_history("VNM")
+```
+
+<details>
+  <summary>Output</summary>
+
+```
+   exerciseDate  cashYear  cashDividendPercentage issueMethod
+0      10/01/22      2021                    0.14        cash
+1      07/09/21      2021                    0.15        cash
+2      07/06/21      2020                    0.11        cash
+3      05/01/21      2020                    0.10        cash
+```
+</details>
+
+## 3.3. 💰 Phân tích tài chính (Financial Analysis)
+
+### 3.3.1. Bộ chỉ số tài chính
+```python
+financial_ratio(symbol="TCB", report_range='yearly', is_all=False)
+```
+Trong đó:
+- `report_range` nhận 1 trong 2 giá trị: `yearly` cho phép trả về chỉ số theo năm, `quarterly` trả về dữ liệu theo quý
+- `is_all` có giá trị mặc định là `True` cho phép lấy chỉ số qua tất cả các kỳ (năm hoặc quý), `False` cho phép lấy các kỳ gần nhất (5 năm hoặc 10 quý gần đây).
+
+<details>
+  <summary>Output</summary>
+
+  ```
+>>> financial_ratio('TCB', 'yearly')
+year                      2022   2021   2020   2019   2018
+ticker                     TCB    TCB    TCB    TCB    TCB
+priceToEarning             4.5    9.7    9.0    8.2   10.7
+priceToBook                0.8    1.9    1.5    1.3    1.8
+roe                      0.197  0.217  0.181  0.178  0.215
+roa                      0.032  0.036   0.03  0.029  0.029
+earningPerShare           5729   5132   3504   2869   2410
+bookValuePerShare        32248  26452  21214  17679  14749
+interestMargin           0.053  0.057  0.049  0.043  0.041
+nonInterestOnToi         0.259   0.28  0.307  0.323  0.379
+badDebtPercentage        0.007  0.007  0.005  0.013  0.018
+provisionOnBadDebt       1.573  1.629   1.71  0.948  0.851
+costOfFinancing          0.028  0.022  0.031  0.038  0.041
+equityOnTotalAsset       0.162  0.164   0.17  0.162  0.161
+equityOnLoan              0.27  0.268  0.269  0.269  0.324
+costToIncome             0.328  0.301  0.319  0.347  0.318
+equityOnLiability          0.2    0.2    0.2    0.2    0.2
+epsChange                0.116  0.465  0.221  0.191  0.313
+assetOnEquity              6.2    6.1    5.9    6.2    6.2
+preProvisionOnToi        0.537  0.554  0.542   0.52  0.542
+postTaxOnToi               0.5  0.497  0.465  0.485  0.462
+loanOnEarnAsset          0.684  0.665  0.681  0.649  0.537
+loanOnAsset              0.602  0.611  0.631  0.602  0.498
+loanOnDeposit            1.173  1.104    1.0  0.998  0.794
+depositOnEarnAsset       0.583  0.603   0.68  0.651  0.676
+badDebtOnAsset           0.004  0.004  0.003  0.008  0.009
+liquidityOnLiability     0.347  0.382  0.372  0.411  0.531
+payableOnEquity            5.2    5.1    4.9    5.2    5.2
+cancelDebt               0.002  0.004  0.013  0.002  0.008
+bookValuePerShareChange  0.219  0.247    0.2  0.199  0.923
+creditGrowth             0.211  0.252  0.202  0.443 -0.006
+  ```
+</details>
+
+
+### 3.3.2. 💵 Báo cáo kết quả kinh doanh, cân đối kế toán và lưu chuyển tiền tệ
+
+#### 3.3.2.1. 📄 Báo cáo kinh doanh
+
+![income_statement](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_income_statement.png)
+```python
+financial_flow(symbol="TCB", report_type='incomestatement', report_range='quarterly')
+```
+
+
+<details>
+  <summary>Output</summary>
+
+```
+        ticker  revenue  yearRevenueGrowth  quarterRevenueGrowth costOfGoodSold grossProfit  ...  investProfit  serviceProfit  otherProfit  provisionExpense operationIncome  ebitda
+index                                                                                        ...
+2021-Q4    TCB     7245              0.328                 0.074           None        None  ...           279           2103          532              -627            6767    None
+2021-Q3    TCB     6742              0.310                 0.023           None        None  ...           384           1497          156              -589            6151    None
+2021-Q2    TCB     6588              0.674                 0.076           None        None  ...           717           1457          444              -598            6615    None
+2021-Q1    TCB     6124              0.454                 0.122           None        None  ...           812           1325          671              -851            6369    None
+```
+</details>
+
+#### 3.3.2.2. 🧾 Bảng cân đối kế toán
+
+![balance_sheet](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_balancesheet.png)
+```python
+financial_flow(symbol="TCB", report_type='balancesheet', report_range='quarterly')
+```
+
+<details>
+  <summary>Output</summary>
+
+```
+        ticker shortAsset  cash shortInvest shortReceivable inventory longAsset  fixedAsset  ...  payableInterest  receivableInterest deposit otherDebt  fund  unDistributedIncome  minorShareHolderProfit  payable
+index                                                                                        ...
+
+2021-Q4    TCB       None  3579        None            None      None      None        7224  ...             3098                5808  314753     33680  9156                47469                     845   475756
+2021-Q3    TCB       None  3303        None            None      None      None        7106  ...             3074                6224  316376     34003  6784                45261                     753   453251
+2021-Q2    TCB       None  3554        None            None      None      None        6739  ...             2643                5736  289335     27678  6790                40924                     659   420403
+2021-Q1    TCB       None  4273        None            None      None      None        4726  ...             2897                5664  287446     26035  6790                36213                     563   3837
+```
+</details>
+
+#### 3.3.2.3. 💶 Báo cáo lưu chuyển tiền tệ
 
-> Phiên bản API hiện tại cho phép truy cập giá lịch sử tối đa đến ngày 2012-03-20 đối với tất cả mã cổ phiếu. Nếu bạn có nhu cầu lấy lịch sử giá từ thời điểm thị trường chứng khoán bắt đầu hoạt động (REE là mã cổ phiếu có giao dịch sớm nhất thị trường vào 2000-07-31), hãy là một thành viên của [ vnstock membership](https://www.facebook.com/groups/vnstock) để được hỗ trợ.
+```python
+financial_flow(symbol="TCB", report_type='cashflow', report_range='quarterly')
+```
 
-vnstock cho phép người dùng **tải xuống dữ liệu lịch sử giao dịch cổ phiếu** với theo 5 mức độ chi tiết theo khoảng thời gian bao gồm: 1 phút, 15 phút, 30 phút, 1 giờ, 1 ngày. Trong ví dụ dưới đây, dữ liệu giá được truy xuất theo cấp độ ngày. Đơn vị giá mặc định là VND.
+<details>
+  <summary>Output</summary>
+
+```
+        ticker  investCost  fromInvest  fromFinancial  fromSale  freeCashFlow
+index
+2021-Q4    TCB        -280        -276              0     -9328             0
+2021-Q3    TCB        -180        -179             60     17974             0
+2021-Q2    TCB        -337        -282              0     11205             0
+2021-Q1    TCB        -143        -143              0     -6954             0
+```
+</details>
+
+## 3.4. Phân tích kỹ thuật (Technical Analysis)
+
+### 3.4.1 📈 Truy xuất dữ liệu giá lịch sử
+
+> Phiên bản API hiện tại cho phép truy cập giá lịch sử tối đa đến ngày 2012-03-20 đối với tất cả mã cổ phiếu. Nếu bạn có nhu cầu lấy lịch sử giá từ thời điểm thị trường chứng khoán bắt đầu hoạt động (REE là mã cổ phiếu có giao dịch sớm nhất thị trường vào 2000-07-31), hãy là một thành viên của [vnstock membership](https://www.facebook.com/groups/vnstock) để được hỗ trợ.
+
+vnstock cho phép người dùng tải xuống dữ liệu lịch sử giao dịch của `mã cổ phiếu, chỉ số, hợp đồng phái sinh`.
+- Dữ liệu `cổ phiếu` và `chỉ số` hỗ trợ 5 mức độ chi tiết theo khoảng thời gian bao gồm: 1 phút, 15 phút, 30 phút, 1 giờ, 1 ngày. 
+- Dữ liệu `phái sinh` hỗ trợ 8 mức độ chi tiết theo khoảng thời gian bao gồm: 1 phút, 3 phút, 5 phút, 15 phút, 30 phút, 45 phút, 1 giờ, 1 ngày
+- Trường dữ liệu `time` sẽ là giá trị ngày tháng `YYYY-mm-dd` nếu `resolution` nhập vào là `1D`, trong khi `resolution` là cấp độ phút và giờ sẽ cho thêm thông tin thời gian giờ/phút.
+- Đơn vị giá OHLC được làm tròn, chỉ lấy phần nguyên. Đơn vị tính là VND.
+
+Trong ví dụ dưới đây, dữ liệu giá được truy xuất theo cấp độ ngày.
 
 ```python
 df =  stock_historical_data(symbol='GMD', 
                             start_date="2021-01-01", 
                             end_date='2022-02-25', resolution='1D', type='stock')
 print(df)
 ```
 - Mới: 
-  - Giá trị mà tham số `resolution` có thể nhận là `1D` (mặc định, 1 ngày), '1' (1 phút), 15 (15 phút), 30 (30 phút), '1H' (hàng giờ).
-  - `type = 'stock'` cho phép lấy dữ liệu giá của mã cổ cổ phiếu, `type = 'index'` cho phép lấy dữ liệu giá của mã chỉ số. Các mã chỉ số hỗ trợ bao gồm: VNINDEX, VN30, HNX, HNX30, UPCOM, VNXALLSHARE, VN30F1M, VN30F2M, VN30F1Q, VN30F2Q
+  - Giá trị mà tham số `resolution` có thể nhận là `1D` (mặc định, 1 ngày), '1' (1 phút), 3 (3 phút), 5 (5 phút), 15 (15 phút), 30 (30 phút), 45 (45 phút), '1H' (hàng giờ).
+  - `type = 'stock'` cho phép lấy dữ liệu giá của mã cổ cổ phiếu, `type = 'index'` cho phép lấy dữ liệu giá của mã chỉ số, và `type='derivative` cho phép lấy dữ liệu phái sinh. Các mã được hỗ trợ bao gồm (nhưng không giới hạn): VNINDEX, VN30, HNX, HNX30, UPCOM, VNXALLSHARE, VN30F1M, VN30F2M, VN30F1Q, VN30F2Q
 
 Bạn cũng có thể viết hàm theo dạng rút gọn như dưới đây, điều này đúng với tất cả các hàm, miễn là thông số được nhập vào đúng thứ tự:
 
   - Lấy dữ liệu lịch sử cổ phiếu
   ```python
   df = stock_historical_data("GMD", "2021-01-01", "2022-02-25", "1D", 'stock')
   print(df)
@@ -221,26 +392,38 @@
 
 - Lấy dữ liệu lịch sử của mã chỉ số
 ```python
 df = stock_historical_data("VNINDEX", "2021-01-01", "2022-02-25", "1D", 'index')
 print(df)
 ```
 
-## 3.4. 📊 Bảng giá
+- Lấy dữ liệu lịch sử của hợp đồng phái sinh
+```python
+df = stock_historical_data("VN30F1M", "2023-07-01", "2023-07-24", "1D", 'derivative')
+print(df)
+```
+
+## 3.5. Lựa chọn cổ phiếu (Stock Screening)
+
+### 3.5.1. So sánh các cổ phiếu tiềm năng
+
+#### 3.5.1.1. 📊 Bảng giá (Price board)
 
 Bạn có thể tải xuống bảng giá của một danh sách các cổ phiếu được chọn để phân tích, thiết lập thuật toán dễ dàng hơn (khi xuất ra Google Sheets/Excel) so với việc xem trực tiếp trên bảng giá của các công ty chứng khoán.
 
 <details>
-  <summary>Bảng giá</summary>
+  <summary>Minh họa Bảng giá TCBS</summary>
 
   ![price_board](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_trading_board_sector.png)
 
 </details>
 
-### 3.4.1. Thông tin bước giá, khối lượng và khớp lệnh
+
+##### a. Thông tin bước giá, khối lượng và khớp lệnh
+
 ```python
 price_depth('TCB,SSI,VND')
 ```
 Sử dụng hàm này cho phép thống kê các bước giá và khối lượng trên bảng giá của một hoặc một danh sách các mã cổ phiếu. Bạn có thể sử dụng kết hợp hàm này với hàm `price_board` để kết hợp các thông tin đa dạng về giá, khối lượng, chỉ số, thông tin giao dịch để chọn lọc và theo dõi cổ phiếu theo mục đích sử dụng của mình.
 
 <details>
   <summary>Output</summary>
@@ -251,15 +434,16 @@
 1   SSI           28400     30350    26450      28450      100      28400     9850      28350  ...    30640      28550     22730      28600    48410          1610280   142759     17353  803963854     
 2   VND           17950     19200    16700      18450    11620      18400    38790      18350  ...    73180      18550     87830      18600   223700          4360710   152966      8355  932083910     
 
 [3 rows x 22 columns]
 
 </details>
 
-### 3.4.2. Thông tin giao dịch bổ sung và các chỉ số
+
+##### b. Thông tin giao dịch bổ sung và các chỉ số
 
 ```
 price_board('TCB,SSI,VND')
 ```
 Hàm này cho phép tải về thông tin giá, khối lượng và các chỉ số quan trọng cho một hoặc một danh sách mã cổ phiếu. Sử dụng kết hợp với hàm `price_depth` cho hiệu quả tốt nhất.
 
 <details>
@@ -270,114 +454,17 @@
   Mã CP  Giá Khớp Lệnh  KLBD/TB5D  T.độ GD  KLGD ròng(CM)  ...  vnid1m  vnid3m  vnid1y  vnipe    vnipb
 0   TCB        48600.0        0.6     0.49         -23200  ...    -3.7    -2.0    22.4  17.99  2.46159
 1   SSI        43300.0        0.5     0.50        -112200  ...    -3.7    -2.0    22.4  17.99  2.46159
 2   VND        32600.0        0.7     0.68          37300  ...    -3.7    -2.0    22.4  17.99  2.46159
 ```
 </details>
 
-## 3.5. 🔥 Dữ liệu khớp lệnh trong ngày giao dịch
-
-<details>
-  <summary>Minh hoạ giao diện TCBS</summary>
-
-  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen1.png)
-  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen2.png)
-
-</details>
-vnstock cho phép người dùng tải xuống dữ liệu khớp lệnh trong ngày giao dịch theo thời gian thực. Nếu mốc thời gian bạn truy cứu rơi vào Thứ Bảy, Chủ Nhật thì dữ liệu nhận được thể hiện cho ngày giao dịch của Thứ 6 của tuần đó.
-
-```python
-df =  stock_intraday_data(symbol='TCB', 
-                            page_size=500)
-print(df)
-```
-
-<details>
-  <summary>Terminal output</summary>
-
-  ```{r, engine='python', count_lines}
->>> stock_intraday_data('TCB', 500)
-
-  ticker      time  orderType investorType  volume  averagePrice  orderCount
-0    TCB  14:29:55  Sell Down        SHEEP    1000       32700.0           1
-1    TCB  14:29:47     Buy Up        SHEEP     200       32750.0           1
-2    TCB  14:29:44  Sell Down         WOLF    8000       32700.0          14
-3    TCB  14:29:41  Sell Down        SHEEP    1000       32700.0           5
-4    TCB  14:29:36  Sell Down         WOLF   23800       32700.0          10
-  ```
-
-</details>
-
-<details>
-  <summary>Giải thích ý nghĩa chỉ số</summary>
-  • Khi 1 lệnh lớn (từ Cá mập, tay to, tổ chức....) mua chủ động (hoặc bán chủ động) được đưa vào Sàn, thường thì nó sẽ được khớp với nhiều lệnh nhỏ đang chờ bán (hoặc chờ mua). Nếu chỉ nhìn realtime theo từng lệnh khớp riêng lẻ, thì sẽ không thể phát hiện được các lệnh to (của Cá mập, tay to...) vừa được đẩy vào Sàn. Vì vậy, chúng tôi "cộng dồn" các lệnh khớp này lại (phát sinh bởi 1 lệnh lớn chủ động vào sàn trong 1 khoảng thời gian rất nhanh) để giúp NĐT phát hiện các lệnh lớn (của Cá mập, tay to....) chính xác hơn. Lệnh Cá mập sẽ được tô xanh (cho Mua chủ động) và đỏ (cho Bán chủ động). 
 
-  • Cá mập: (CM - SHARK) nhà đầu tư tay to, tổ chức, đầu tư lớn, dẫn dắt thị trường. Giá trị 1 lệnh đặt > 1 tỷ đồng/lệnh đặt. Đồ thị 1N dùng số liệu 1 phút cho 60’ gần nhất; 1W là tổng mỗi 15’ cho 1 tuần; 1M là tổng hàng ngày cho 1 tháng
-
-  • Sói già: (SG - WOLF) nhà đầu tư kinh nghiệm, giá trị lệnh đặt cao. Giá trị 1 lệnh đặt từ 200 tr đến 1 tỷ đồng/lệnh đặt.
-
-  • Cừu non: (CN - SHEEP) nhà đầu tư nhỏ lẻ, giá trị giao dịch và mua bán chủ động thấp. Giá trị 1 lệnh đặt Mua hoặc Bán chủ động < 200 triệu đồng/lệnh đặt vào.
-
-  • Mua chủ động (hay Buy Up) là khi NĐT thực hiện chủ động mua lên qua việc đặt lệnh mua với giá bằng giá dư bán gần nhất để có thể khớp luôn. Như thế, giá khớp cho lệnh này thường sẽ đẩy giá khớp lên cao hơn thị giá trước đó.
-
-  • Bán chủ động (hay Sell Down) là khi NĐT thực hiện chủ động Bán dưới giá hiện tại (hay thị giá) của cổ phiếu bằng việc đặt lệnh bán với giá bán bằng giá dư mua gần nhất để khớp ngay. Và như thế, thị giá sẽ bị kéo xuống thấp hơn so với thị giá trước đó. Thống kê khối lượng giao dich theo Mua CĐ và Bán CĐ dùng để đánh giá tương quan giữa cung (Bán CĐ) và cầu (Mua CĐ) trên giao dịch khớp lệnh thực tế, nhằm nhận định tương đối về sự vận động của xu hướng dòng tiền. Khi tỷ lệ % Mua CĐ trên (Tổng Mua và Bán CĐ) lớn hơn 50%, đồng nghĩa với việc thị trường đang có xu hướng mua vào nhiều hơn bán ra và ngược lại, qua đó xác định được dòng tiền vào/ra với mỗi cổ phiếu. Khi tỷ lệ này cao đột biến (>70% hay <30%) so với điểm cân bằng (50%) , đó là tín hiệu của việc mua hoặc bán bất chấp của thị trường.
-
-</details>
-
-## 3.6. 💰 Các chỉ số tài chính
-
-### 3.6.1. Bộ chỉ số tài chính của một mã cổ phiếu
-```python
-financial_ratio(symbol="TCB", report_range='yearly', is_all=False)
-```
-Trong đó:
-- `report_range` nhận 1 trong 2 giá trị: `yearly` cho phép trả về chỉ số theo năm, `quarterly` trả về dữ liệu theo quý
-- `is_all` có giá trị mặc định là `True` cho phép lấy chỉ số qua tất cả các kỳ (năm hoặc quý), `False` cho phép lấy các kỳ gần nhất (5 năm hoặc 10 quý gần đây).
-
-<details>
-  <summary>Output</summary>
-
-  ```
->>> financial_ratio('TCB', 'yearly')
-year                      2022   2021   2020   2019   2018
-ticker                     TCB    TCB    TCB    TCB    TCB
-priceToEarning             4.5    9.7    9.0    8.2   10.7
-priceToBook                0.8    1.9    1.5    1.3    1.8
-roe                      0.197  0.217  0.181  0.178  0.215
-roa                      0.032  0.036   0.03  0.029  0.029
-earningPerShare           5729   5132   3504   2869   2410
-bookValuePerShare        32248  26452  21214  17679  14749
-interestMargin           0.053  0.057  0.049  0.043  0.041
-nonInterestOnToi         0.259   0.28  0.307  0.323  0.379
-badDebtPercentage        0.007  0.007  0.005  0.013  0.018
-provisionOnBadDebt       1.573  1.629   1.71  0.948  0.851
-costOfFinancing          0.028  0.022  0.031  0.038  0.041
-equityOnTotalAsset       0.162  0.164   0.17  0.162  0.161
-equityOnLoan              0.27  0.268  0.269  0.269  0.324
-costToIncome             0.328  0.301  0.319  0.347  0.318
-equityOnLiability          0.2    0.2    0.2    0.2    0.2
-epsChange                0.116  0.465  0.221  0.191  0.313
-assetOnEquity              6.2    6.1    5.9    6.2    6.2
-preProvisionOnToi        0.537  0.554  0.542   0.52  0.542
-postTaxOnToi               0.5  0.497  0.465  0.485  0.462
-loanOnEarnAsset          0.684  0.665  0.681  0.649  0.537
-loanOnAsset              0.602  0.611  0.631  0.602  0.498
-loanOnDeposit            1.173  1.104    1.0  0.998  0.794
-depositOnEarnAsset       0.583  0.603   0.68  0.651  0.676
-badDebtOnAsset           0.004  0.004  0.003  0.008  0.009
-liquidityOnLiability     0.347  0.382  0.372  0.411  0.531
-payableOnEquity            5.2    5.1    4.9    5.2    5.2
-cancelDebt               0.002  0.004  0.013  0.002  0.008
-bookValuePerShareChange  0.219  0.247    0.2  0.199  0.923
-creditGrowth             0.211  0.252  0.202  0.443 -0.006
-  ```
-</details>
+#### 3.5.1.2. 🏭 Phân tích chỉ số các cổ phiếu cùng ngành (Industry Analysis)
 
-## 3.7. So sánh cổ phiếu
-### 3.7.1. 🏭 Phân tích chỉ số các cổ phiếu cùng ngành
 ```python
 industry_analysis("VNM", lang='vi)
 ```
 - Trả về thông tin các mã cổ phiếu cùng ngành với mã cổ phiếu nằm trong cùng nhóm ngành với mã `VNM`.
 - Tham số `lang='vi` mặc định trả về tên các chỉ số bằng tiếng Việt, đổi thành `en` để giữ nguyên chỉ số với tên tiếng Anh.
 
 - Trong đó các chỉ số sau được thể hiện dưới dạng thập phân sử dụng để thể hiện chỉ số dưới dạng %: 
@@ -413,15 +500,16 @@
 Doanh thu quý gần nhất         NaN  -0.094 -0.252  0.093 -0.302  -0.057 -0.181  0.031 -0.352 -0.067  -0.31 -0.675 -0.197 -0.134 -0.123  0.102  -0.122 -0.142  0.009
 LNST năm tới                   NaN   0.285   0.26  0.173 -0.202   0.074  0.047 -0.719 -0.041   0.04 -0.939  0.116  6.025 -0.034   0.09 -0.155   0.813  0.022    NaN
 Doanh thu năm tới              NaN     0.2    0.3  0.162  0.283     0.1    0.1   -0.7   0.05   0.05   0.03   0.15   -0.5    0.1    0.3  -0.08   -0.06   0.02    NaN
 RSI                            NaN    50.7   43.1   71.8   24.0    28.5   59.2   33.7   68.2   53.5   46.6   44.1   51.1   32.3   55.5   55.3    33.3   54.8   61.1
 ```
 </details>
 
-### 3.7.2. 🔬 So sánh các chỉ số của danh sách các cổ phiếu tùy chọn
+
+#### 3.5.1.3. 🔬 So sánh các chỉ số của danh sách các cổ phiếu tùy chọn
 ```python
 stock_ls_analysis("TCB, BID, CEO, GMD", lang='vi')
 ```
 
 <details>
   <summary>Output</summary>
 
@@ -433,188 +521,327 @@
 1    CEO   17062  66300             1           183.2 -0.8          5.7               81.8       0.0  ...           7.8       -0.099     -0.086            NaN         3.002      -1.469      -0.2  51.9  82.0
 2    BID  225357  44550            -3            21.3  0.4          2.6                NaN       0.0  ...           NaN        0.115      0.154          0.083         0.000         NaN       NaN  49.1  34.0
 3    TCB  178003  50700             1             9.9  0.2          1.9                NaN       0.0  ...           NaN        0.418      0.255          0.059         0.157         NaN       NaN  45.2  28.0
 ```
 
 </details>
 
-### 3.7.4. 💵 Báo cáo kết quả kinh doanh, cân đối kế toán và lưu chuyển tiền tệ
 
-#### 3.7.4.1. 📄 Báo cáo kinh doanh
+#### 3.5.1.4. ⭐ Đánh giá xếp hạng 
+##### a. Đánh giá chung
+![general_rating](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/general_rating.png)
 
-![income_statement](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_income_statement.png)
 ```python
-financial_flow(symbol="TCB", report_type='incomestatement', report_range='quarterly')
+general_rating("VNM")
 ```
 
-
 <details>
   <summary>Output</summary>
 
 ```
-        ticker  revenue  yearRevenueGrowth  quarterRevenueGrowth costOfGoodSold grossProfit  ...  investProfit  serviceProfit  otherProfit  provisionExpense operationIncome  ebitda
-index                                                                                        ...
-2021-Q4    TCB     7245              0.328                 0.074           None        None  ...           279           2103          532              -627            6767    None
-2021-Q3    TCB     6742              0.310                 0.023           None        None  ...           384           1497          156              -589            6151    None
-2021-Q2    TCB     6588              0.674                 0.076           None        None  ...           717           1457          444              -598            6615    None
-2021-Q1    TCB     6124              0.454                 0.122           None        None  ...           812           1325          671              -851            6369    None
+   stockRating  valuation  financialHealth  businessModel  businessOperation  rsRating  taScore  ... ticker highestPrice  lowestPrice  priceChange3m  priceChange1y  beta   alpha
+0          2.4        1.5              4.8            3.0                3.2       1.0      1.0  ...    VNM     102722.2      78600.0         -0.092         -0.232  0.49 -0.0014
 ```
 </details>
 
-#### 3.7.4.2. 🧾 Bảng cân đối kế toán
-
-![balance_sheet](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_balancesheet.png)
+##### b. 🌱 Đánh giá mô hình kinh doanh
 ```python
-financial_flow(symbol="TCB", report_type='balancesheet', report_range='quarterly')
+biz_model_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-        ticker shortAsset  cash shortInvest shortReceivable inventory longAsset  fixedAsset  ...  payableInterest  receivableInterest deposit otherDebt  fund  unDistributedIncome  minorShareHolderProfit  payable
-index                                                                                        ...
-
-2021-Q4    TCB       None  3579        None            None      None      None        7224  ...             3098                5808  314753     33680  9156                47469                     845   475756
-2021-Q3    TCB       None  3303        None            None      None      None        7106  ...             3074                6224  316376     34003  6784                45261                     753   453251
-2021-Q2    TCB       None  3554        None            None      None      None        6739  ...             2643                5736  289335     27678  6790                40924                     659   420403
-2021-Q1    TCB       None  4273        None            None      None      None        4726  ...             2897                5664  287446     26035  6790                36213                     563   3837
+  ticker  businessModel  businessEfficiency  assetQuality  cashFlowQuality  bom  businessAdministration  productService  businessAdvantage  companyPosition  industry  operationRisk
+0    VNM            3.0                   3             3                3    3                       3               3                  3                3         3              3
 ```
 </details>
 
-#### 3.7.4.3. 💶 Báo cáo lưu chuyển tiền tệ
-
+##### c. 🎮 Đánh giá hiệu quả hoạt động
 ```python
-financial_flow(symbol="TCB", report_type='cashflow', report_range='quarterly')
+biz_operation_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-        ticker  investCost  fromInvest  fromFinancial  fromSale  freeCashFlow
-index
-2021-Q4    TCB        -280        -276              0     -9328             0
-2021-Q3    TCB        -180        -179             60     17974             0
-2021-Q2    TCB        -337        -282              0     11205             0
-2021-Q1    TCB        -143        -143              0     -6954             0
+      industryEn loanGrowth depositGrowth netInterestIncomeGrowth netInterestMargin  ... last5yearsFCFFGrowth lastYearGrossProfitMargin lastYearOperatingProfitMargin  lastYearNetProfitMargin  TOIGrowth
+0  Food Products       None          None                    None              None  ...                    2                         5                             3                        4       None
 ```
 </details>
 
-## 3.8. 🧧 Lịch sử chi trả cổ tức
-
+##### d. 📑 Đánh giá sức khỏe tài chính
 ```python
-dividend_history("VNM")
+financial_health_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-   exerciseDate  cashYear  cashDividendPercentage issueMethod
-0      10/01/22      2021                    0.14        cash
-1      07/09/21      2021                    0.15        cash
-2      07/06/21      2020                    0.11        cash
-3      05/01/21      2020                    0.10        cash
+      industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
+0  Food Products        None             None         None             None    VNM              4.8              4             5           5                 5              5
 ```
 </details>
 
-## 3.9. ⭐ Đánh giá xếp hạng 
-### 3.9.1. Đánh giá chung
-![general_rating](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/general_rating.png)
-
+##### e. 💲 Đánh giá về Định giá
 ```python
-general_rating("VNM")
+valuation_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-   stockRating  valuation  financialHealth  businessModel  businessOperation  rsRating  taScore  ... ticker highestPrice  lowestPrice  priceChange3m  priceChange1y  beta   alpha
-0          2.4        1.5              4.8            3.0                3.2       1.0      1.0  ...    VNM     102722.2      78600.0         -0.092         -0.232  0.49 -0.0014
+      industryEn ticker  valuation  pe  pb  ps  evebitda  dividendRate
+0  Food Products    VNM        1.5   2   1   1         1             3
 ```
 </details>
 
-### 3.9.2. 🌱 Đánh giá mô hình kinh doanh
+##### f. 💳 Sức khỏe tài chính theo ngành
 ```python
-biz_model_rating("VNM")
+industry_financial_health("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-  ticker  businessModel  businessEfficiency  assetQuality  cashFlowQuality  bom  businessAdministration  productService  businessAdvantage  companyPosition  industry  operationRisk
-0    VNM            3.0                   3             3                3    3                       3               3                  3                3         3              3
+  industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
+0       None        None             None         None             None    VNM              3.4              4             4           3                 3              3
 ```
 </details>
 
-### 3.9.3. 🎮 Đánh giá hiệu quả hoạt động
-```python
-biz_operation_rating("VNM")
-```
+### 3.5.2. 🔎 Bộ lọc cổ phiếu
+
+Bộ lọc cổ phiếu là một hàm cho phép bạn truy vấn và lọc các cổ phiếu theo nhiều tiêu chí đa dạng dựa trên dữ liệu phân tích của TCBS. Hàm này sẽ trả về một DataFrame chứa các thông tin toàn diện về các cổ phiếu thỏa mãn điều kiện lọc của bạn. Bạn có thể dùng DataFrame này để tiếp tục phân tích, biểu diễn hoặc xuất ra dữ liệu dạng bảng tính. Đây là cập nhật ưu việt giúp bạn tiết kiệm thời gian và công sức đáng kể khi làm việc với dữ liệu cổ phiếu, đồng thời cho phép lập trình để lọc là cập nhật danh sách cổ phiếu hiệu quả không cần sử dụng giao diện web từ công ty chứng khoán.
 
 <details>
-  <summary>Output</summary>
+  <summary> Bộ lọc cổ phiếu TCBS </summary>
+
+  ![stock_scanner](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/stock_scanner_tcbs.png)
 
-```
-      industryEn loanGrowth depositGrowth netInterestIncomeGrowth netInterestMargin  ... last5yearsFCFFGrowth lastYearGrossProfitMargin lastYearOperatingProfitMargin  lastYearNetProfitMargin  TOIGrowth
-0  Food Products       None          None                    None              None  ...                    2                         5                             3                        4       None
-```
 </details>
 
-### 3.9.4. 📑 Đánh giá sức khỏe tài chính
-```python
-financial_health_rating("VNM")
-```
+Tham số
+- params (dict): một từ điển chứa các tham số và giá trị của chúng cho việc lọc cổ phiếu. Các `key` là tên của các bộ lọc, và các `value` là một giá trị đơn hoặc một tupple gồm hai giá trị (min và max) cho bộ lọc đó. Đây là ví dụ cho tham số params được thiết lập đúng:
+
+```python
+params = {
+            "exchangeName": "HOSE",
+            "marketCap": (100, 1000),
+            "pe": (10, 20),
+            "dividendYield": (5, 10),
+            "tcbsRecommend": "BUY",
+            "size": 50
+        }
+
+# Áp dụng bộ lọc với hàm để lấy kết quả
+get_stock_screening_insights(params)
+```
+
+<details>
+
+<summary>Các bộ lọc gợi ý và tiêu chí hỗ trợ bao gồm</summary>
+
+  a. BỘ LỌC GỢI Ý (PRESET)
+
+    > Sử dụng các tiêu chí lọc như sau để thiết lập tham số params.
+
+    - CANSLIM: epsGrowth1Year, lastQuarterProfitGrowth, roe, avgTradingValue20Day, relativeStrength1Month
+    - Giá trị: roe, pe, avgTradingValue20Day
+    - Cổ tức cao: dividendYield, avgTradingValue20Day
+    - Phá nền mua: avgTradingValue20Day, forecastVolumeRatio, breakout: 'BULLISH'
+    - Giá tăng + Đột biến khối lượng: avgTradingValue20Day, forecastVolumeRatio
+    - Vượt đỉnh 52 tuần: avgTradingValue20Day, priceBreakOut52Week: 'BREAK_OUT'
+    - Phá đáy 52 tuần: avgTradingValue20Day, priceWashOut52Week: 'WASH_OUT'
+    - Uptrend ngắn hạn: avgTradingValue20Day, uptrend: 'buy-signal'
+    - Vượt trội ngắn hạn: relativeStrength3Day, 
+    - Tăng trưởng: epsGrowth1Year, roe, avgTradingValue20Day
+
+  b. THÔNG TIN CHUNG
+
+    - exchangeName: sàn giao dịch của cổ phiếu, ví dụ "HOSE", "HNX", hoặc "UPCOM". Bạn có thể dùng dấu phẩy để phân tách nhiều sàn, ví dụ "HOSE,HNX,UPCOM".
+    - hasFinancialReport: Có báo cáo tài chính gần nhất. `1` nghĩa là có, `0` nghĩa là không.
+    - industryName: Lọc các cổ phiếu theo ngành cụ thể. Giá trị dạng `Retail` cho ngành Bán lẻ. Các giá trị khác có thể là:
+      - `Insurance`: Bảo hiểm
+      - `Real Estate`: Bất động sản
+      - `Technology`: Công nghệ thông tin
+      - `Oil & Gas`: Dầu khí
+      - `Financial Services`: Dịch vụ tài chính
+      - `Utilities`: Điện, nước, xăng dầu và khí đốt
+      - `Travel & Leisure`: Du lịch và giải trí
+      - `Industrial Goods & Services`: Hàng và dịch vụ công nghiệp
+      - `Personal & Household Goods`: Hàng cá nhân và gia dụng
+      - `Chemicals`: Hóa chất
+      - `Banks`: Ngân hàng
+      - `Automobiles & Parts`: Ô tô và phụ tùng
+      - `Basic Resources`: Tài nguyên cơ bản
+      - `Food & Beverage`: Thực phẩm và đồ uống
+      - `Media`: Truyền thông
+      - `Telecommunications`: Viễn thông
+      - `Construction & Materials`: Xây dựng và vật liệu
+      - `Health Care`: Y tế
+      - marketCap: vốn hóa thị trường của cổ phiếu tính bằng tỷ VND.
+      - priceNearRealtime: giá hiện tại của cổ phiếu tính bằng VND.
+      - foreignVolumePercent: tỷ lệ phần trăm khối lượng nước ngoài trong tổng khối lượng.
+      - alpha: lợi nhuận vượt trội của cổ phiếu so với lợi nhuận thị trường.
+      - beta: độ biến động của cổ phiếu so với thị trường.
+      - freeTransferRate: tỷ lệ phần trăm cổ phiếu có thể chuyển nhượng tự do.
+  
+  c. TĂNG TRƯỞNG
 
-<details>
-  <summary>Output</summary>
+    - revenueGrowth1Year: tốc độ tăng trưởng doanh thu trong năm qua.
+    - revenueGrowth5Year: tốc độ tăng trưởng doanh thu trung bình trong 5 năm qua.
+    - epsGrowth1Year: tốc độ tăng trưởng lợi nhuận trên mỗi cổ phiếu trong năm qua.
+    - epsGrowth5Year: tốc độ tăng trưởng lợi nhuận trên mỗi cổ phiếu trung bình trong 5 năm qua.
+    - lastQuarterRevenueGrowth: tốc độ tăng trưởng doanh thu trong quý gần nhất.
+    - secondQuarterRevenueGrowth: tốc độ tăng trưởng doanh thu trong quý thứ hai.
+    - lastQuarterProfitGrowth: tốc độ tăng trưởng lợi nhuận trong quý gần nhất.
+    - secondQuarterProfitGrowth: tốc độ tăng trưởng lợi nhuận trong quý thứ hai.
+  
+  d. CHỈ SỐ TÀI CHÍNH
+  
+    - grossMargin: tỷ suất lợi nhuận gộp của cổ phiếu.
+    - netMargin: tỷ suất lợi nhuận ròng của cổ phiếu.
+    - roe: tỷ suất sinh lời về vốn chủ sở hữu của cổ phiếu.
+    - doe: tỷ suất cổ tức về vốn chủ sở hữu của cổ phiếu.
+    - dividendYield: tỷ suất cổ tức của cổ phiếu.
+    - eps: lợi nhuận trên mỗi cổ phiếu của cổ phiếu tính bằng VND.
+    - pe: tỷ số giá/lợi nhuận của cổ phiếu.
+    - pb: tỷ số giá/giá trị sổ sách của cổ phiếu.
+    - evEbitda: tỷ số giá trị doanh nghiệp/lợi nhuận trước thuế, lãi vay, khấu hao và amortization của cổ phiếu.
+    - netCashPerMarketCap: tỷ số tiền mặt ròng/vốn hóa thị trường của cổ phiếu.
+    - netCashPerTotalAssets: tỷ số tiền mặt ròng/tổng tài sản của cổ phiếu.
+    - profitForTheLast4Quarters: tổng lợi nhuận trong 4 quý gần nhất của cổ phiếu tính bằng tỷ VND.
+  
+  e. BIẾN ĐỘNG GIÁ & KHỐI LƯỢNG
+
+    - suddenlyHighVolumeMatching: tín hiệu chỉ ra nếu có sự tăng đột biến khối lượng khớp lệnh cho cổ phiếu này. 0 nghĩa là không, 1 nghĩa là có.
+    - totalTradingValue: tổng giá trị giao dịch của cổ phiếu này tính bằng tỷ VND hôm nay.
+    - avgTradingValue5Day: giá trị giao dịch trung bình của cổ phiếu này tính bằng tỷ VND trong 5 ngày.
+    - avgTradingValue10Day: giá trị giao dịch trung bình của cổ phiếu này tính bằng tỷ VND trong 10 ngày.
+    - avgTradingValue20Day: giá trị giao dịch trung bình của cổ phiếu này tính bằng tỷ VND trong 20 ngày.
+    - priceGrowth1Week: tốc độ tăng trưởng giá của cổ phiếu trong tuần qua.
+    - priceGrowth1Month: tốc độ tăng trưởng giá của cổ phiếu trong tháng qua.
+    - percent1YearFromPeak: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá cao nhất trong 1 năm.
+    - percentAwayFromHistoricalPeak: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá cao nhất lịch sử.
+    - percent1YearFromBottom: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá thấp nhất trong 1 năm.
+    - percentOffHistoricalBottom: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá thấp nhất lịch sử.
+    - priceVsSMA5: mối quan hệ giữa giá hiện tại và SMA 5 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSma10: mối quan hệ giữa giá hiện tại và SMA 10 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSMA20: mối quan hệ giữa giá hiện tại và SMA 20 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSma50: mối quan hệ giữa giá hiện tại và SMA 50 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSMA100: mối quan hệ giữa giá hiện tại và SMA 100 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - forecastVolumeRatio: tỷ số giữa khối lượng dự báo và khối lượng thực tế của cổ phiếu hôm nay.
+    - volumeVsVSma5: tỷ số giữa khối lượng hiện tại và SMA khối lượng 5 ngày của cổ phiếu.
+    - volumeVsVSma10: tỷ số giữa khối lượng hiện tại và SMA khối lượng 10 ngày của cổ phiếu.
+    - volumeVsVSma20: tỷ số giữa khối lượng hiện tại và SMA khối lượng 20 ngày của cổ phiếu.
+    - volumeVsVSma50: tỷ số giữa khối lượng hiện tại và SMA khối lượng 50 ngày của cổ phiếu.
+  
+  f. HÀNH VI THỊ TRƯỜNG
+
+    - strongBuyPercentage: tỷ lệ phần trăm tín hiệu mua mạnh cho cổ phiếu này dựa trên phân tích kỹ thuật.
+    - activeBuyPercentage: tỷ lệ phần trăm tín hiệu mua tích cực cho cổ phiếu này dựa trên phân tích kỹ thuật.
+    - foreignTransaction: loại giao dịch nước ngoài cho cổ phiếu này hôm nay. Các giá trị có thể là "buyMoreThanSell", "sellMoreThanBuy", hoặc "noTransaction".
+    - foreignBuySell20Session: giá trị mua bán ròng nước ngoài cho cổ phiếu này tính bằng tỷ VND trong 20 phiên.
+    - numIncreaseContinuousDay: số ngày liên tiếp cổ phiếu này tăng giá.
+    - numDecreaseContinuousDay: số ngày liên tiếp cổ phiếu này giảm giá.
+  
+  g. TÍN HIỆU KỸ THUẬT
+
+    - rsi14: chỉ số sức mạnh tương đối (RSI) của cổ phiếu với chu kỳ 14 ngày.
+    - rsi14Status: trạng thái của RSI cho cổ phiếu này. Các giá trị có thể là "intoOverBought", "intoOverSold", "outOfOverBought", hoặc "outOfOverSold".
+    - tcbsBuySellSignal: tín hiệu mua bán cho cổ phiếu này dựa trên phân tích của TCBS. Các giá trị có thể là "BUY" hoặc "SELL".
+    - priceBreakOut52Week: tín hiệu chỉ ra nếu có sự đột phá giá cho cổ phiếu này trong 52 tuần. Các giá trị có thể là "BREAK_OUT" hoặc "NO_BREAK_OUT".
+    - priceWashOut52Week: tín hiệu chỉ ra nếu có sự rửa giá cho cổ phiếu này trong 52 tuần. Các giá trị có thể là "WASH_OUT" hoặc "NO_WASH_OUT".
+    - macdHistogram: tín hiệu chỉ ra nếu có tín hiệu MACD histogram cho cổ phiếu này. Các giá trị có thể là "macdHistGT0Increase", "macdHistGT0Decrease", "macdHistLT0Increase", hoặc "macdHistLT0Decrease".
+    - relativeStrength3Day: sức mạnh tương đối của cổ phiếu so với thị trường trong 3 ngày.
+    - relativeStrength1Month: sức mạnh tương đối của cổ phiếu so với thị trường trong 1 tháng.
+    - relativeStrength3Month: sức mạnh tương đối của cổ phiếu so với thị trường trong 3 tháng.
+    - relativeStrength1Year: sức mạnh tương đối của cổ phiếu so với thị trường trong 1 năm.
+    - tcRS: sức mạnh tương đối của TCBS của cổ phiếu so với thị trường.
+    - sarVsMacdHist: tín hiệu chỉ ra nếu có tín hiệu SAR vs MACD histogram cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+  
+  h. TÍN HIỆU MUA/BÁN
+
+    - bollingBandSignal: tín hiệu chỉ ra nếu có tín hiệu Bollinger Band cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+    - dmiSignal: tín hiệu chỉ ra nếu có tín hiệu chỉ số chuyển động hướng (DMI) cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+    - uptrend: tín hiệu chỉ ra nếu có tín hiệu xu hướng tăng cho cổ phiếu này. Các giá trị có thể là "buy-signal" hoặc "sell-signal".
+    - breakout: tín hiệu chỉ ra nếu có tín hiệu đột phá cho cổ phiếu này. Các giá trị có thể là "BULLISH" hoặc "BEARISH".
+  
+  i. TCBS ĐÁNH GIÁ
+
+    - tcbsRecommend: tín hiệu chỉ ra nếu có khuyến nghị của TCBS cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+    - stockRating: điểm đánh giá cổ phiếu cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
+    - businessModel: điểm đánh giá mô hình kinh doanh cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
+    - businessOperation: điểm đánh giá hoạt động kinh doanh cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
+    - financialHealth: điểm đánh giá sức khỏe tài chính cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
 
-```
-      industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
-0  Food Products        None             None         None             None    VNM              4.8              4             5           5                 5              5
-```
 </details>
 
-### 3.9.5. 💲 Đánh giá về Định giá
-```python
-valuation_rating("VNM")
-```
+
+## 3.6. 🔥 Dữ liệu khớp lệnh trong ngày giao dịch
 
 <details>
-  <summary>Output</summary>
+  <summary>Minh hoạ giao diện TCBS</summary>
+
+  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen1.png)
+  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen2.png)
 
-```
-      industryEn ticker  valuation  pe  pb  ps  evebitda  dividendRate
-0  Food Products    VNM        1.5   2   1   1         1             3
-```
 </details>
+vnstock cho phép người dùng tải xuống dữ liệu khớp lệnh trong ngày giao dịch theo thời gian thực. Nếu mốc thời gian bạn truy cứu rơi vào Thứ Bảy, Chủ Nhật thì dữ liệu nhận được thể hiện cho ngày giao dịch của Thứ 6 của tuần đó.
 
-## 3.10.  💳 Sức khỏe tài chính theo ngành
 ```python
-industry_financial_health("VNM")
+df =  stock_intraday_data(symbol='TCB', 
+                            page_size=500)
+print(df)
 ```
 
 <details>
-  <summary>Output</summary>
+  <summary>Terminal output</summary>
+
+  ```{r, engine='python', count_lines}
+>>> stock_intraday_data('TCB', 500)
+
+  ticker      time  orderType investorType  volume  averagePrice  orderCount
+0    TCB  14:29:55  Sell Down        SHEEP    1000       32700.0           1
+1    TCB  14:29:47     Buy Up        SHEEP     200       32750.0           1
+2    TCB  14:29:44  Sell Down         WOLF    8000       32700.0          14
+3    TCB  14:29:41  Sell Down        SHEEP    1000       32700.0           5
+4    TCB  14:29:36  Sell Down         WOLF   23800       32700.0          10
+  ```
+
+</details>
+
+<details>
+  <summary>Giải thích ý nghĩa chỉ số</summary>
+  • Khi 1 lệnh lớn (từ Cá mập, tay to, tổ chức....) mua chủ động (hoặc bán chủ động) được đưa vào Sàn, thường thì nó sẽ được khớp với nhiều lệnh nhỏ đang chờ bán (hoặc chờ mua). Nếu chỉ nhìn realtime theo từng lệnh khớp riêng lẻ, thì sẽ không thể phát hiện được các lệnh to (của Cá mập, tay to...) vừa được đẩy vào Sàn. Vì vậy, chúng tôi "cộng dồn" các lệnh khớp này lại (phát sinh bởi 1 lệnh lớn chủ động vào sàn trong 1 khoảng thời gian rất nhanh) để giúp NĐT phát hiện các lệnh lớn (của Cá mập, tay to....) chính xác hơn. Lệnh Cá mập sẽ được tô xanh (cho Mua chủ động) và đỏ (cho Bán chủ động). 
+
+  • Cá mập: (CM - SHARK) nhà đầu tư tay to, tổ chức, đầu tư lớn, dẫn dắt thị trường. Giá trị 1 lệnh đặt > 1 tỷ đồng/lệnh đặt. Đồ thị 1N dùng số liệu 1 phút cho 60’ gần nhất; 1W là tổng mỗi 15’ cho 1 tuần; 1M là tổng hàng ngày cho 1 tháng
+
+  • Sói già: (SG - WOLF) nhà đầu tư kinh nghiệm, giá trị lệnh đặt cao. Giá trị 1 lệnh đặt từ 200 tr đến 1 tỷ đồng/lệnh đặt.
+
+  • Cừu non: (CN - SHEEP) nhà đầu tư nhỏ lẻ, giá trị giao dịch và mua bán chủ động thấp. Giá trị 1 lệnh đặt Mua hoặc Bán chủ động < 200 triệu đồng/lệnh đặt vào.
+
+  • Mua chủ động (hay Buy Up) là khi NĐT thực hiện chủ động mua lên qua việc đặt lệnh mua với giá bằng giá dư bán gần nhất để có thể khớp luôn. Như thế, giá khớp cho lệnh này thường sẽ đẩy giá khớp lên cao hơn thị giá trước đó.
+
+  • Bán chủ động (hay Sell Down) là khi NĐT thực hiện chủ động Bán dưới giá hiện tại (hay thị giá) của cổ phiếu bằng việc đặt lệnh bán với giá bán bằng giá dư mua gần nhất để khớp ngay. Và như thế, thị giá sẽ bị kéo xuống thấp hơn so với thị giá trước đó. Thống kê khối lượng giao dich theo Mua CĐ và Bán CĐ dùng để đánh giá tương quan giữa cung (Bán CĐ) và cầu (Mua CĐ) trên giao dịch khớp lệnh thực tế, nhằm nhận định tương đối về sự vận động của xu hướng dòng tiền. Khi tỷ lệ % Mua CĐ trên (Tổng Mua và Bán CĐ) lớn hơn 50%, đồng nghĩa với việc thị trường đang có xu hướng mua vào nhiều hơn bán ra và ngược lại, qua đó xác định được dòng tiền vào/ra với mỗi cổ phiếu. Khi tỷ lệ này cao đột biến (>70% hay <30%) so với điểm cân bằng (50%) , đó là tín hiệu của việc mua hoặc bán bất chấp của thị trường.
 
-```
-  industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
-0       None        None             None         None             None    VNM              3.4              4             4           3                 3              3
-```
 </details>
 
-## 3.11. 🌏 Thông tin thị trường
+
+## 3.7. 🌏 Thông tin thị trường
 
 <details>
-  <summary>Tạm ngưng hoạt động do SSI từ chối truy cập</summary>
+  <summary>Tạm ngưng hoạt động, chờ nâng cấp APIs</summary>
 
-### 3.11.1. Các mã cổ phiếu đứng đầu theo tiêu chí xếp loại 
+### 3.7.1. Các mã cổ phiếu đứng đầu theo tiêu chí xếp loại 
 
 <details>
   <summary>SSI Top Stocks</summary>
 
 Top Breakout (Đột phá) > Top Gainers (Tăng giá) > Top Losers (Giảm giá) > Top Value (Giá trị) > Top Volume (Khối lượng)
 ![top_mover](./src/ssi_top_breakout_gainer_loser.png)
 
@@ -636,15 +863,15 @@
 1          3270200.0     1.088892e+11  ...  {'organCode': 'STB', 'rtd7': 18173.6958318461,...  {'organCode': 'STB', 'sma20Past4': 34332.5, 's...
 2          1456800.0     4.199166e+10  ...  {'organCode': 'FUEVFVND', 'rtd7': None, 'rtd11...  {'organCode': 'FUEVFVND', 'sma20Past4': 27993....
 3          1033300.0     1.281170e+10  ...  {'organCode': 'FLC', 'rtd7': 12898.0038031343,...  {'organCode': 'FLC', 'sma20Past4': 12062.5, 's...
 4           998600.0     5.324337e+10  ...  {'organCode': 'NLG', 'rtd7': 23318.1252311207,...  {'organCode': 'NLG', 'sma20Past4': 52385.0, 's...
 ```
 </details>
 
-### 3.11.2. Thông tin giao dịch nhà đầu tư nước ngoài (NDTNN)
+### 3.7.2. Thông tin giao dịch nhà đầu tư nước ngoài (NDTNN)
 Trong ví dụ dưới đây, thể hiện giao dịch mua vào của NDTNN.
 
 ```python
 fr_trade_heatmap ('All', 'FrBuyVol')
 ```
 <details>
   <summary>Output</summary>
@@ -663,15 +890,15 @@
   2        ELC   ELC     4100.0            0.049197  ...       10650.0      9270.0  Công nghệ Thông tin  0.034816
   3        ITD   ITD     2000.0            0.068548  ...       13250.0     11550.0  Công nghệ Thông tin  0.034816
 
   [92 rows x 10 columns]
   ```
 </details>
 
-### 3.11.3. Biến động của các nhóm chỉ số
+### 3.7.3. Biến động của các nhóm chỉ số
 ![latest_indices](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/get_latest_indices.png)
 
 Thông tin các nhóm chỉ số phổ biến của thị trường chứng khoán Việt Nam.
 
 ```python
 get_latest_indices()
 ```
@@ -706,16 +933,16 @@
 21        0         VNSI     1715.37  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
 22        0        VNSML     1140.40  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
 23        0        VNUTI      874.84  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
 24        0        VNX50     1805.33  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
   ```
 </details>
 
-### 3.11.4. Dữ liệu chuyên sâu theo nhóm chỉ số cụ thể
-![index_series_data](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/get_index_series_data.png)
+### 3.7.4. Dữ liệu chuyên sâu theo nhóm chỉ số cụ thể
+![index_series_data](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/get_index_series_data.png)
 
 ```python
 get_index_series(index_code='VNINDEX', time_range='OneYear')
 ```
 - Nhà cung cấp dữ liệu: SSI iBoard sử dụng dữ liệu từ FiinTrade.
 - Sử dụng một trong các mã chỉ số sau để tra cứu:
   
@@ -751,15 +978,65 @@
 
   [246 rows x 14 columns]
   ```
 </details>
 
 </details>
 
-# IV. 🙋‍♂️ Contact Information
+## 3.8. 🛡 Thị trường Phái Sinh
+
+### 3.8.1. Dữ liệu giá lịch sử
+
+> Xem chi tiết mục [3.4.1 📈 Truy xuất dữ liệu giá lịch sử](#341--truy-xuất-dữ-liệu-giá-lịch-sử) cùng với thông tin giá chứng khoán cơ sở.
+
+### 3.8.2. Dữ liệu khớp lệnh lịch sử
+
+<details>
+
+<summary>Minh họa bảng dữ liệu khớp lệnh Phái sinh - CK Rồng Việt </summary>
+
+![livedragon_derivative_match](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/livedragon_derivative_history_match.png)
+
+</details>
+
+Để truy vấn dữ liệu từ hàm này, bạn cần có cookie người dùng (không cần đăng nhập) của chứng khoán Rồng Việt. Các bước thực hiện như sau:
+  1. Truy cập `https://livedragon.vdsc.com.vn/all/all.rv`
+  2. Mở `Developer Tools` trên trình duyệt, sử dụng F12 hoặc `Ctrl` + `Shift` + `I` trên Windows hoặc `Cmd` + `Option` + `I` trên macOS
+  3. Chuyển đến tab `Network` và chọn mục `Fetch/XHR`
+  4. Mở bất kỳ mục request nào trong tab này, tìm mục `Header` của request
+  5. Tìm và copy giá trị của `Cookie` trong request này để điền vào bước tiếp theo dưới đây trước khi gọi hàm
+
+```python
+cookie = 'GIÁ TRỊ COOKIE CẦN PASTE VÀO ĐÂY'
+derivatives_historical_match (symbol='VN30F2308', date='2023-07-24', cookie=cookie)
+```
+
+# IV. 🚚 Xuất, Lưu trữ, Chia sẻ dữ liệu
+
+> Để xuất, lưu trữ và chia sẻ dữ liệu với vnstock, bạn có rất nhiều sự lựa chọn kể cả sử dụng cơ sở dữ liệu, bảng tính (Excel, Google Sheets) và nhiều hình thức khác. Dữ liệu tiêu chuẩn tạo ra bởi vnstock là các pandas DataFrame do đó bạn có thể biến đổi và lưu trữ/chia sẻ dữ liệu dễ dàng với cách thức tiêu chuẩn của python. Dưới đây là hướng dẫn cơ bản với cách thức xuất dữ liệu ra csv và Google Sheets.
+
+## 4.1. Xuất dữ liệu ra csv
+
+Dành cho những bạn mới làm quen Python và Pandas có thể sử dụng dữ liệu từ vnstock dễ dàng với công cụ bảng tính quen thuộc. Bạn có thể xuất dữ liệu từ hàm bất kỳ ra csv và mở bằng Excel hoặc upload lên Google Drive và mở bằng Google Sheets.
+
+```python
+start_date = '2023-06-01'
+end_date = '2023-07-24'
+# Truy xuất dữ liệu
+df = stock_historical_data('TCB', start_date, end_date)
+# Xuất dữ liệu ra csv, chèn ngày tháng và mã CP
+df.to_csv(f'THƯ-MỤC-CỦA-BẠN/TCB_historical_price_{start_date}_{end_date}.csv', index=True)
+```
+
+## 4.2. Xuất dữ liệu ra Google Sheets
+
+Phương thức này được thiết kế riêng để xuất dữ liệu trực tiếp từ Google Colab sang Google Sheets (sẽ không hoạt động nếu chạy ở môi trường local, không thiết lập môi trường tương đồng Colab). Tham khảo cách làm chi tiết trong file demo, mục `III. Data Export`
+
+
+# V. 🙋‍♂️ Thông tin liên hệ
 
 Bạn có thể kết nối với tác giả qua các hình thức sau. Trong trường hợp cần hỗ trợ nhanh, bạn có thể chọn nhắn tin qua Messenger hoặc Linkedin, tôi sẽ phản hồi ngay lập tức nếu có thể trong hầu hết các trường hợp.
 
 <div id="badges" align="center">
   <a href="https://www.linkedin.com/in/thinh-vu">
     <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
   </a>
@@ -770,35 +1047,37 @@
   </a>
   </a>
     <a href="https://github.com/thinh-vu">
     <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="Github Badge"/>
   </a>
 </div>
 
-# V. 💪 Hỗ trợ phát triển dự án vnstock
+# VI. 💪 Hỗ trợ phát triển dự án vnstock
 
 Nếu bạn nhận thấy giá trị từ vnstock và các dự án mã nguồn mở của tôi, bạn có thể hỗ trợ phát triển chúng bằng cách quyên góp hoặc đơn giản là gửi tặng tôi một ly cà phê để cảm ơn.
 Bạn có thể chọn 1 trong 3 hình thức đóng góp bao gồm Momo, Chuyển khoản ngân hàng và Gửi tiền qua Paypal. Sự đóng góp của bạn sẽ giúp tôi duy trì phí lưu trữ blog và tiếp tục tạo ra nội dung chất lượng cao. Cảm ơn sự ủng hộ của bạn!
 
 - [Paypal](https://paypal.me/thinhvuphoto?country.x=VN&locale.x=en_US)
+
 - ![momo-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/momo-qr-thinhvu.jpeg)
+  
 - ![vcb-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/vcb-qr-thinhvu.jpg)
 
-# VI. ⚖ Tuyên bố miễn trừ trách nhiệm
+# VII. ⚖ Tuyên bố miễn trừ trách nhiệm
 vnstock được phát triển nhằm mục đích cung cấp các công cụ nghiên cứu đơn giản và miễn phí, nhằm giúp người nghiên cứu tiếp cận và phân tích dữ liệu chứng khoán một cách dễ dàng. Dữ liệu được cung cấp phụ thuộc vào nguồn cấp dữ liệu, do đó, khi sử dụng, bạn cần thận trọng và cân nhắc.
 
 💰 Trong bất kỳ trường hợp nào, người sử dụng hoàn toàn chịu trách nhiệm về quyết định sử dụng dữ liệu trích xuất từ vnstock và chịu trách nhiệm với bất kỳ tổn thất nào có thể phát sinh. Bạn nên tự mình đảm bảo tính chính xác và đáng tin cậy của dữ liệu trước khi sử dụng chúng.
 
 Việc sử dụng dữ liệu chứng khoán và quyết định đầu tư là hoạt động có rủi ro và có thể gây mất mát tài sản. Bạn nên tìm kiếm lời khuyên từ các chuyên gia tài chính và tuân thủ các quy định pháp luật về chứng khoán tại Việt Nam và quốc tế khi tham gia vào hoạt động giao dịch chứng khoán.
 
 Xin lưu ý rằng vnstock không chịu trách nhiệm và không có bất kỳ trách nhiệm pháp lý nào đối với bất kỳ tổn thất hoặc thiệt hại nào phát sinh từ việc sử dụng gói phần mềm này.
 
 🐱‍👤 vnstock được thiết kế hoàn toàn cho mục đích phân tích và thực hành nghiên cứu đầu tư. Mọi hình thức sử dụng không đúng mục đích hoặc việc sử dụng trái phép thư viện với mục đích xấu như tấn công public API hay gây hại cho hệ thống thông qua từ chối truy cập hoặc các hành động tương tự, hoàn toàn nằm ngoài phạm vi sử dụng dự định và không thuộc trách nhiệm của nhóm phát triển.
 
-# VII. Bản quyền và giấy phép
+# VII. 🔑 Bản quyền và giấy phép
 
 
 ```
 Bản quyền (c) 2022 Thinh Vu | thinh-vu @ Github | MIT
 
 Được cấp phép theo quyền tự do, miễn phí, cho bất kỳ cá nhân nào nhận được một bản sao của phần mềm này và các tệp tài liệu liên quan (gọi chung là "Phần mềm"), để sử dụng Phần mềm mà không có bất kỳ hạn chế nào, bao gồm nhưng không giới hạn quyền sử dụng, sao chép, sửa đổi, hợp nhất, xuất bản, phân phối, cấp phép lại và/hoặc bán các bản sao của Phần mềm, và cho phép những người nhận Phần mềm được nhúng vào Phần mềm này, tuân thủ các điều kiện sau đây:
```

### Comparing `vnstock-0.1.8/README.md` & `vnstock-0.1.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 </div>
 
 ---
 
 🌐 View in **[English](https://github.com/thinh-vu/vnstock/blob/main/README-en.md)**
 
 MỤC LỤC
+
 - [I. 🎤 Giới thiệu](#i--giới-thiệu)
-- [II. 📚 Hướng dẫn sử dụng cho người mới](#ii-hướng-dẫn-sử-dụng-cho-người-mới)
+- [II. 📚 Hướng dẫn sử dụng cho người mới](#ii--hướng-dẫn-sử-dụng-cho-người-mới)
 - [III. 💻 Cách sử dụng các hàm trong vnstock](#iii--cách-sử-dụng-các-hàm-trong-vnstock)
-- [IV. 🙋‍♂️ Contact Information](#iv-️-contact-information)
-- [V. 💪 Hỗ trợ phát triển dự án vnstock](#v--hỗ-trợ-phát-triển-dự-án-vnstock)
-- [VI. ⚖ Tuyên bố miễn trừ trách nhiệm](#vi--tuyên-bố-miễn-trừ-trách-nhiệm)
+- [IV. Xuất, Lưu trữ, Chia sẻ dữ liệu](#iv-xuất-lưu-trữ-chia-sẻ-dữ-liệu)
+- [V. 🙋‍♂️ Thông tin liên hệ](#v-️-thông-tin-liên-hệ)
+- [VI. 💪 Hỗ trợ phát triển dự án vnstock](#vi--hỗ-trợ-phát-triển-dự-án-vnstock)
+- [VII. ⚖ Tuyên bố miễn trừ trách nhiệm](#vii--tuyên-bố-miễn-trừ-trách-nhiệm)
 - [VII. Bản quyền và giấy phép](#vii-bản-quyền-và-giấy-phép)
 
+
 # I. 🎤 Giới thiệu
 ## 1.1. Giới thiệu chung
 vnstock là thư viện Python được thiết kế để tải dữ liệu chứng khoán Việt Nam một cách dễ dàng và miễn phí. vnstock sử dụng các nguồn cấp dữ liệu đáng tin cậy, bao gồm nhưng không giới hạn từ công ty chứng khoán và công ty phân tích thị trường tại Việt Nam. Gói thư viện được thiết kế dựa trên nguyên tắc về sự đơn giản và mã nguồn mở, hầu hết các hàm được viết dựa trên thư viện request và pandas có sẵn trên môi trường Google Colab do đó người dùng không cần cài đặt thêm các gói thư viện kèm theo.
 
 ## 1.2. Tính năng chính
 vnstock cung cấp nhiều tính năng đa dạng như tải dữ liệu lịch sử giá, thông tin công ty niêm yết, thông tin thị trường cho tất cả các mã chứng khoán niêm yết.
 
@@ -30,20 +33,41 @@
 
 ## 1.4. Tips
 - Theo dõi những cập nhật về thay đổi của vnstock bằng tính năng `Watch`. Hiện tại vnstock được cập nhật thường xuyên hàng tuần qua nhánh `beta`, vì vậy theo dõi repo này giúp bạn luôn nắm bắt được kịp thời những thay đổi mới nhất.
 - Đánh dấu yêu thích repo `vnstock` bằng tính năng `Star`. Đây cũng là cách giúp vnstock có thể tiếp cận tới nhiều người quan tâm hơn.
 
 <details>
   <summary> Minh họa tính năng Watch và Star </summary>
+  
 ![watch-star](https://github.com/thinh-vu/vnstock/blob/beta/src/vnstock-watch-and-star.png?raw=true)
 
 </details>
 
 ## 1.5. Đóng góp xây dựng mã nguồn vnstock
-- Bạn có thể đóng góp xây dựng vnstock thông qua nhiều hình thức khác nhau, trong đó có việc xây dựng và cải tiến mã nguồn hoặc dịch tài liệu của dự án. Để bắt đầu, bạn có thể `folk` repo này về tài khoản của mình, sửa đổi mã nguồn và tạo `pull request` để yêu cầu cập nhật mã nguồn. Sau khi kiểm tra các thay đổi và phê duyệt, mã nguồn do bạn đóng góp sẽ được gộp vào vnstock.
+- Bạn có thể đóng góp xây dựng vnstock thông qua nhiều hình thức khác nhau, trong đó có việc xây dựng và cải tiến mã nguồn hoặc dịch tài liệu của dự án. 
+- Để bắt đầu, bạn có thể `folk` nhánh `beta` của repo này về tài khoản của mình, sửa đổi mã nguồn và tạo `pull request` để yêu cầu cập nhật mã nguồn. Sau khi kiểm tra các thay đổi và phê duyệt, mã nguồn do bạn đóng góp sẽ được gộp vào vnstock.
+- Lưu ý: Những thay đổi do bạn đóng góp sẽ được phát hành trong phiên bản tiếp theo của `vnstock` trên Pypi.org đồng thời với những cập nhật của tác giả trên nhánh `beta`.
+
+## 1.6. Hoàn thành khảo sát về vnstock
+> vnstock là một dự án tôi tâm huyết, đầu tư nhiều thời gian để phát triển giúp bản thân và cộng đồng tiếp cận nguồn dữ liệu chứng khoán miễn phí và đáng tin cậy.
+
+Hoàn thành bản khảo sát: [Tại đây](https://forms.gle/zaJnbgUCjjL1GoTF6)
+Để đảm bảo rằng vnstock phát triển theo hướng đáp ứng nhu cầu của bạn, tôi rất mong nhận được phản hồi từ bạn. Bạn là người dùng quan trọng của vnstock và ý kiến của bạn sẽ giúp chúng tôi xây dựng một kế hoạch phát triển vnstock một cách toàn diện.
+
+## 1.7. Dịch vụ "code dạo", gây quỹ phát triển dự án
+
+Ngoài ra, để gây quỹ phát triển dự án, tôi cũng cung cấp dịch vụ "code dạo" theo đặt hàng bao gồm nhưng không giới hạn với các hoạt động dưới đây:
+- Tải dữ liệu thị trường
+- Viết workflow quét dữ liệu, cập nhật cơ sở dữ liệu, vv
+- Thiết lập dự án phân tích chứng khoán toàn diện
+- Tạo bộ lọc cổ phiếu độc quyền
+- Tạo robot giao dịch qua API
+- Cung cấp API dữ liệu độc quyền
+
+Nếu bạn nào quan tâm và có nhu cầu, vui lòng [inbox](https://www.messenger.com/t/mr.thinh.ueh) để trao đổi thêm. Hoạt động này cũng giúp tôi hiểu thêm về những ứng dụng thực tế và phát triển vnstock trong tương lai.
 
 # II. 📚 Hướng dẫn sử dụng cho người mới
 ## 2.1. Tài nguyên quan trọng
 
 ### 2.1.2 Blog
 
 👉 Để biết thêm thông tin và minh hoạ về cách sử dụng, bạn vui lòng truy cập bài viết trên blog của tôi, có sẵn bằng tiếng Việt/Anh [tại đây](https://thinhvu.com/2022/09/22/vnstock-api-tai-du-lieu-chung-khoan-python?utm_source=github&utm_medium=vnstock).
@@ -72,14 +96,17 @@
 
 </details>
 
 ### 2.1.4. Xây dựng cộng đồng vnstock
 
 🖐 Nếu bạn thấy thư viện này có giá trị và muốn hỗ trợ tác giả duy trì vnstock dưới dạng mã nguồn mở, miễn phí thì có thể tham gia ủng hộ gây quỹ phát triển dự án này. Để biết thêm chi tiết, vui lòng tham khảo bài viết trên blog sau: [Cùng nhau xây dựng cộng đồng VNStock vững mạnh](https://thinhvu.com/2023/04/15/xay-dung-cong-dong-vnstock-vung-manh/).
 
+- Tham gia nhóm vnstock trên Facebook: [Tại đây](https://www.facebook.com/groups/vnstock)
+- Tham gia Discord channel: [Tại đây](https://discord.gg/qJvxJcChJ3)
+
 <details>
   <summary>Ủng hộ quỹ phát triển vnstock</summary>
   Nếu vnstock giúp ích cho bạn, hãy đóng góp quỹ phát triển ứng dụng này theo một trong hai hình thức sau gồm chuyển khoản ngân hàng hoặc Momo. Mọi khoản đóng góp đều đáng trân quý và là động lực giúp tác giả duy trì vnstock luôn hữu ích, miễn phí, và dễ tiếp cận cho cộng đồng.
 
   - ![vcb-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/vcb-qr-thinhvu.jpg)
   - ![momo-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/momo-qr-thinhvu.jpeg)
 
@@ -129,15 +156,17 @@
 
 Để nạp các hàm của vnstock vào dự án Python của bạn, cần `import` chúng thông qua câu lệnh như dưới đây. Như vậy mọi thứ đã sẵn sàng để truy cập dữ liệu do vnstock cung cấp thông qua các hàm được liệt kê trong tài liệu hướng dẫn.
 
 ```python
 from vnstock import *
 ```
 
-## 3.1 📰 Danh sách các công ty niêm yết
+## 3.1. ☑ Danh sách cổ phiếu niêm yết (Listing)
+
+### 3.1.1. 📰 Danh sách các công ty niêm yết
 ```python
 listing_companies()
 ```
 Hàm này đọc dữ liệu từ tệp csv đính kèm trên Github theo mặc định (trong thư mục /data của repo này). Bởi danh sách các công ty niêm yết thường không thay đổi liên tục nên việc này không gây trở ngại nhiều.
 
 <details>
   <summary>Output</summary>
@@ -148,15 +177,18 @@
 0    VVS   UpcomIndex  Công ty Cổ phần Đầu tư Phát triển Máy Việt Nam  Đầu tư Phát triển Máy Việt Nam            DN          CT  ...  False  False  False  False  False  False
 1    XDC   UpcomIndex   Công ty TNHH MTV Xây dựng Công trình Tân Cảng    Xây dựng Công trình Tân Cảng            DN          CT  ...  False  False  False  False  False  False
 2    HSV   UpcomIndex           Công ty Cổ phần Tập đoàn HSV Việt Nam                Gang Thép Hà Nội            DN          CT  ...  False  False  False  False  False  False
 ```
 
 </details>
 
-## 3.2. Tổng quan về công ty
+## 3.2. 🏳 Phân tích cơ bản (Fundamental Analysis)
+
+### 3.2.1. 🏚 Thông tin tổng quan công ty
+
 ```python
 company_overview('TCB')
 ```
 
 <details>
   <summary>Output</summary>
 
@@ -164,29 +196,168 @@
   >>> company_overview('TCB')
     exchange    shortName  industryID industryIDv2   industry  ... deltaInMonth deltaInYear  outstandingShare  issueShare  ticker
   0     HOSE  Techcombank         289         8355  Ngân hàng  ...       -0.027      -0.038            3510.9      3510.9     TCB
   ```
 
 </details>
 
-## 3.3. 📈 Truy xuất dữ liệu giá lịch sử
+### 3.2.2. 🧧 Lịch sử chi trả cổ tức
+
+```python
+dividend_history("VNM")
+```
+
+<details>
+  <summary>Output</summary>
+
+```
+   exerciseDate  cashYear  cashDividendPercentage issueMethod
+0      10/01/22      2021                    0.14        cash
+1      07/09/21      2021                    0.15        cash
+2      07/06/21      2020                    0.11        cash
+3      05/01/21      2020                    0.10        cash
+```
+</details>
+
+## 3.3. 💰 Phân tích tài chính (Financial Analysis)
+
+### 3.3.1. Bộ chỉ số tài chính
+```python
+financial_ratio(symbol="TCB", report_range='yearly', is_all=False)
+```
+Trong đó:
+- `report_range` nhận 1 trong 2 giá trị: `yearly` cho phép trả về chỉ số theo năm, `quarterly` trả về dữ liệu theo quý
+- `is_all` có giá trị mặc định là `True` cho phép lấy chỉ số qua tất cả các kỳ (năm hoặc quý), `False` cho phép lấy các kỳ gần nhất (5 năm hoặc 10 quý gần đây).
+
+<details>
+  <summary>Output</summary>
+
+  ```
+>>> financial_ratio('TCB', 'yearly')
+year                      2022   2021   2020   2019   2018
+ticker                     TCB    TCB    TCB    TCB    TCB
+priceToEarning             4.5    9.7    9.0    8.2   10.7
+priceToBook                0.8    1.9    1.5    1.3    1.8
+roe                      0.197  0.217  0.181  0.178  0.215
+roa                      0.032  0.036   0.03  0.029  0.029
+earningPerShare           5729   5132   3504   2869   2410
+bookValuePerShare        32248  26452  21214  17679  14749
+interestMargin           0.053  0.057  0.049  0.043  0.041
+nonInterestOnToi         0.259   0.28  0.307  0.323  0.379
+badDebtPercentage        0.007  0.007  0.005  0.013  0.018
+provisionOnBadDebt       1.573  1.629   1.71  0.948  0.851
+costOfFinancing          0.028  0.022  0.031  0.038  0.041
+equityOnTotalAsset       0.162  0.164   0.17  0.162  0.161
+equityOnLoan              0.27  0.268  0.269  0.269  0.324
+costToIncome             0.328  0.301  0.319  0.347  0.318
+equityOnLiability          0.2    0.2    0.2    0.2    0.2
+epsChange                0.116  0.465  0.221  0.191  0.313
+assetOnEquity              6.2    6.1    5.9    6.2    6.2
+preProvisionOnToi        0.537  0.554  0.542   0.52  0.542
+postTaxOnToi               0.5  0.497  0.465  0.485  0.462
+loanOnEarnAsset          0.684  0.665  0.681  0.649  0.537
+loanOnAsset              0.602  0.611  0.631  0.602  0.498
+loanOnDeposit            1.173  1.104    1.0  0.998  0.794
+depositOnEarnAsset       0.583  0.603   0.68  0.651  0.676
+badDebtOnAsset           0.004  0.004  0.003  0.008  0.009
+liquidityOnLiability     0.347  0.382  0.372  0.411  0.531
+payableOnEquity            5.2    5.1    4.9    5.2    5.2
+cancelDebt               0.002  0.004  0.013  0.002  0.008
+bookValuePerShareChange  0.219  0.247    0.2  0.199  0.923
+creditGrowth             0.211  0.252  0.202  0.443 -0.006
+  ```
+</details>
+
+
+### 3.3.2. 💵 Báo cáo kết quả kinh doanh, cân đối kế toán và lưu chuyển tiền tệ
+
+#### 3.3.2.1. 📄 Báo cáo kinh doanh
+
+![income_statement](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_income_statement.png)
+```python
+financial_flow(symbol="TCB", report_type='incomestatement', report_range='quarterly')
+```
+
+
+<details>
+  <summary>Output</summary>
+
+```
+        ticker  revenue  yearRevenueGrowth  quarterRevenueGrowth costOfGoodSold grossProfit  ...  investProfit  serviceProfit  otherProfit  provisionExpense operationIncome  ebitda
+index                                                                                        ...
+2021-Q4    TCB     7245              0.328                 0.074           None        None  ...           279           2103          532              -627            6767    None
+2021-Q3    TCB     6742              0.310                 0.023           None        None  ...           384           1497          156              -589            6151    None
+2021-Q2    TCB     6588              0.674                 0.076           None        None  ...           717           1457          444              -598            6615    None
+2021-Q1    TCB     6124              0.454                 0.122           None        None  ...           812           1325          671              -851            6369    None
+```
+</details>
+
+#### 3.3.2.2. 🧾 Bảng cân đối kế toán
+
+![balance_sheet](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_balancesheet.png)
+```python
+financial_flow(symbol="TCB", report_type='balancesheet', report_range='quarterly')
+```
+
+<details>
+  <summary>Output</summary>
+
+```
+        ticker shortAsset  cash shortInvest shortReceivable inventory longAsset  fixedAsset  ...  payableInterest  receivableInterest deposit otherDebt  fund  unDistributedIncome  minorShareHolderProfit  payable
+index                                                                                        ...
+
+2021-Q4    TCB       None  3579        None            None      None      None        7224  ...             3098                5808  314753     33680  9156                47469                     845   475756
+2021-Q3    TCB       None  3303        None            None      None      None        7106  ...             3074                6224  316376     34003  6784                45261                     753   453251
+2021-Q2    TCB       None  3554        None            None      None      None        6739  ...             2643                5736  289335     27678  6790                40924                     659   420403
+2021-Q1    TCB       None  4273        None            None      None      None        4726  ...             2897                5664  287446     26035  6790                36213                     563   3837
+```
+</details>
+
+#### 3.3.2.3. 💶 Báo cáo lưu chuyển tiền tệ
 
-> Phiên bản API hiện tại cho phép truy cập giá lịch sử tối đa đến ngày 2012-03-20 đối với tất cả mã cổ phiếu. Nếu bạn có nhu cầu lấy lịch sử giá từ thời điểm thị trường chứng khoán bắt đầu hoạt động (REE là mã cổ phiếu có giao dịch sớm nhất thị trường vào 2000-07-31), hãy là một thành viên của [ vnstock membership](https://www.facebook.com/groups/vnstock) để được hỗ trợ.
+```python
+financial_flow(symbol="TCB", report_type='cashflow', report_range='quarterly')
+```
 
-vnstock cho phép người dùng **tải xuống dữ liệu lịch sử giao dịch cổ phiếu** với theo 5 mức độ chi tiết theo khoảng thời gian bao gồm: 1 phút, 15 phút, 30 phút, 1 giờ, 1 ngày. Trong ví dụ dưới đây, dữ liệu giá được truy xuất theo cấp độ ngày. Đơn vị giá mặc định là VND.
+<details>
+  <summary>Output</summary>
+
+```
+        ticker  investCost  fromInvest  fromFinancial  fromSale  freeCashFlow
+index
+2021-Q4    TCB        -280        -276              0     -9328             0
+2021-Q3    TCB        -180        -179             60     17974             0
+2021-Q2    TCB        -337        -282              0     11205             0
+2021-Q1    TCB        -143        -143              0     -6954             0
+```
+</details>
+
+## 3.4. Phân tích kỹ thuật (Technical Analysis)
+
+### 3.4.1 📈 Truy xuất dữ liệu giá lịch sử
+
+> Phiên bản API hiện tại cho phép truy cập giá lịch sử tối đa đến ngày 2012-03-20 đối với tất cả mã cổ phiếu. Nếu bạn có nhu cầu lấy lịch sử giá từ thời điểm thị trường chứng khoán bắt đầu hoạt động (REE là mã cổ phiếu có giao dịch sớm nhất thị trường vào 2000-07-31), hãy là một thành viên của [vnstock membership](https://www.facebook.com/groups/vnstock) để được hỗ trợ.
+
+vnstock cho phép người dùng tải xuống dữ liệu lịch sử giao dịch của `mã cổ phiếu, chỉ số, hợp đồng phái sinh`.
+- Dữ liệu `cổ phiếu` và `chỉ số` hỗ trợ 5 mức độ chi tiết theo khoảng thời gian bao gồm: 1 phút, 15 phút, 30 phút, 1 giờ, 1 ngày. 
+- Dữ liệu `phái sinh` hỗ trợ 8 mức độ chi tiết theo khoảng thời gian bao gồm: 1 phút, 3 phút, 5 phút, 15 phút, 30 phút, 45 phút, 1 giờ, 1 ngày
+- Trường dữ liệu `time` sẽ là giá trị ngày tháng `YYYY-mm-dd` nếu `resolution` nhập vào là `1D`, trong khi `resolution` là cấp độ phút và giờ sẽ cho thêm thông tin thời gian giờ/phút.
+- Đơn vị giá OHLC được làm tròn, chỉ lấy phần nguyên. Đơn vị tính là VND.
+
+Trong ví dụ dưới đây, dữ liệu giá được truy xuất theo cấp độ ngày.
 
 ```python
 df =  stock_historical_data(symbol='GMD', 
                             start_date="2021-01-01", 
                             end_date='2022-02-25', resolution='1D', type='stock')
 print(df)
 ```
 - Mới: 
-  - Giá trị mà tham số `resolution` có thể nhận là `1D` (mặc định, 1 ngày), '1' (1 phút), 15 (15 phút), 30 (30 phút), '1H' (hàng giờ).
-  - `type = 'stock'` cho phép lấy dữ liệu giá của mã cổ cổ phiếu, `type = 'index'` cho phép lấy dữ liệu giá của mã chỉ số. Các mã chỉ số hỗ trợ bao gồm: VNINDEX, VN30, HNX, HNX30, UPCOM, VNXALLSHARE, VN30F1M, VN30F2M, VN30F1Q, VN30F2Q
+  - Giá trị mà tham số `resolution` có thể nhận là `1D` (mặc định, 1 ngày), '1' (1 phút), 3 (3 phút), 5 (5 phút), 15 (15 phút), 30 (30 phút), 45 (45 phút), '1H' (hàng giờ).
+  - `type = 'stock'` cho phép lấy dữ liệu giá của mã cổ cổ phiếu, `type = 'index'` cho phép lấy dữ liệu giá của mã chỉ số, và `type='derivative` cho phép lấy dữ liệu phái sinh. Các mã được hỗ trợ bao gồm (nhưng không giới hạn): VNINDEX, VN30, HNX, HNX30, UPCOM, VNXALLSHARE, VN30F1M, VN30F2M, VN30F1Q, VN30F2Q
 
 Bạn cũng có thể viết hàm theo dạng rút gọn như dưới đây, điều này đúng với tất cả các hàm, miễn là thông số được nhập vào đúng thứ tự:
 
   - Lấy dữ liệu lịch sử cổ phiếu
   ```python
   df = stock_historical_data("GMD", "2021-01-01", "2022-02-25", "1D", 'stock')
   print(df)
@@ -207,26 +378,38 @@
 
 - Lấy dữ liệu lịch sử của mã chỉ số
 ```python
 df = stock_historical_data("VNINDEX", "2021-01-01", "2022-02-25", "1D", 'index')
 print(df)
 ```
 
-## 3.4. 📊 Bảng giá
+- Lấy dữ liệu lịch sử của hợp đồng phái sinh
+```python
+df = stock_historical_data("VN30F1M", "2023-07-01", "2023-07-24", "1D", 'derivative')
+print(df)
+```
+
+## 3.5. Lựa chọn cổ phiếu (Stock Screening)
+
+### 3.5.1. So sánh các cổ phiếu tiềm năng
+
+#### 3.5.1.1. 📊 Bảng giá (Price board)
 
 Bạn có thể tải xuống bảng giá của một danh sách các cổ phiếu được chọn để phân tích, thiết lập thuật toán dễ dàng hơn (khi xuất ra Google Sheets/Excel) so với việc xem trực tiếp trên bảng giá của các công ty chứng khoán.
 
 <details>
-  <summary>Bảng giá</summary>
+  <summary>Minh họa Bảng giá TCBS</summary>
 
   ![price_board](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_trading_board_sector.png)
 
 </details>
 
-### 3.4.1. Thông tin bước giá, khối lượng và khớp lệnh
+
+##### a. Thông tin bước giá, khối lượng và khớp lệnh
+
 ```python
 price_depth('TCB,SSI,VND')
 ```
 Sử dụng hàm này cho phép thống kê các bước giá và khối lượng trên bảng giá của một hoặc một danh sách các mã cổ phiếu. Bạn có thể sử dụng kết hợp hàm này với hàm `price_board` để kết hợp các thông tin đa dạng về giá, khối lượng, chỉ số, thông tin giao dịch để chọn lọc và theo dõi cổ phiếu theo mục đích sử dụng của mình.
 
 <details>
   <summary>Output</summary>
@@ -237,15 +420,16 @@
 1   SSI           28400     30350    26450      28450      100      28400     9850      28350  ...    30640      28550     22730      28600    48410          1610280   142759     17353  803963854     
 2   VND           17950     19200    16700      18450    11620      18400    38790      18350  ...    73180      18550     87830      18600   223700          4360710   152966      8355  932083910     
 
 [3 rows x 22 columns]
 
 </details>
 
-### 3.4.2. Thông tin giao dịch bổ sung và các chỉ số
+
+##### b. Thông tin giao dịch bổ sung và các chỉ số
 
 ```
 price_board('TCB,SSI,VND')
 ```
 Hàm này cho phép tải về thông tin giá, khối lượng và các chỉ số quan trọng cho một hoặc một danh sách mã cổ phiếu. Sử dụng kết hợp với hàm `price_depth` cho hiệu quả tốt nhất.
 
 <details>
@@ -256,114 +440,17 @@
   Mã CP  Giá Khớp Lệnh  KLBD/TB5D  T.độ GD  KLGD ròng(CM)  ...  vnid1m  vnid3m  vnid1y  vnipe    vnipb
 0   TCB        48600.0        0.6     0.49         -23200  ...    -3.7    -2.0    22.4  17.99  2.46159
 1   SSI        43300.0        0.5     0.50        -112200  ...    -3.7    -2.0    22.4  17.99  2.46159
 2   VND        32600.0        0.7     0.68          37300  ...    -3.7    -2.0    22.4  17.99  2.46159
 ```
 </details>
 
-## 3.5. 🔥 Dữ liệu khớp lệnh trong ngày giao dịch
-
-<details>
-  <summary>Minh hoạ giao diện TCBS</summary>
-
-  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen1.png)
-  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen2.png)
-
-</details>
-vnstock cho phép người dùng tải xuống dữ liệu khớp lệnh trong ngày giao dịch theo thời gian thực. Nếu mốc thời gian bạn truy cứu rơi vào Thứ Bảy, Chủ Nhật thì dữ liệu nhận được thể hiện cho ngày giao dịch của Thứ 6 của tuần đó.
-
-```python
-df =  stock_intraday_data(symbol='TCB', 
-                            page_size=500)
-print(df)
-```
-
-<details>
-  <summary>Terminal output</summary>
-
-  ```{r, engine='python', count_lines}
->>> stock_intraday_data('TCB', 500)
-
-  ticker      time  orderType investorType  volume  averagePrice  orderCount
-0    TCB  14:29:55  Sell Down        SHEEP    1000       32700.0           1
-1    TCB  14:29:47     Buy Up        SHEEP     200       32750.0           1
-2    TCB  14:29:44  Sell Down         WOLF    8000       32700.0          14
-3    TCB  14:29:41  Sell Down        SHEEP    1000       32700.0           5
-4    TCB  14:29:36  Sell Down         WOLF   23800       32700.0          10
-  ```
-
-</details>
-
-<details>
-  <summary>Giải thích ý nghĩa chỉ số</summary>
-  • Khi 1 lệnh lớn (từ Cá mập, tay to, tổ chức....) mua chủ động (hoặc bán chủ động) được đưa vào Sàn, thường thì nó sẽ được khớp với nhiều lệnh nhỏ đang chờ bán (hoặc chờ mua). Nếu chỉ nhìn realtime theo từng lệnh khớp riêng lẻ, thì sẽ không thể phát hiện được các lệnh to (của Cá mập, tay to...) vừa được đẩy vào Sàn. Vì vậy, chúng tôi "cộng dồn" các lệnh khớp này lại (phát sinh bởi 1 lệnh lớn chủ động vào sàn trong 1 khoảng thời gian rất nhanh) để giúp NĐT phát hiện các lệnh lớn (của Cá mập, tay to....) chính xác hơn. Lệnh Cá mập sẽ được tô xanh (cho Mua chủ động) và đỏ (cho Bán chủ động). 
 
-  • Cá mập: (CM - SHARK) nhà đầu tư tay to, tổ chức, đầu tư lớn, dẫn dắt thị trường. Giá trị 1 lệnh đặt > 1 tỷ đồng/lệnh đặt. Đồ thị 1N dùng số liệu 1 phút cho 60’ gần nhất; 1W là tổng mỗi 15’ cho 1 tuần; 1M là tổng hàng ngày cho 1 tháng
-
-  • Sói già: (SG - WOLF) nhà đầu tư kinh nghiệm, giá trị lệnh đặt cao. Giá trị 1 lệnh đặt từ 200 tr đến 1 tỷ đồng/lệnh đặt.
-
-  • Cừu non: (CN - SHEEP) nhà đầu tư nhỏ lẻ, giá trị giao dịch và mua bán chủ động thấp. Giá trị 1 lệnh đặt Mua hoặc Bán chủ động < 200 triệu đồng/lệnh đặt vào.
-
-  • Mua chủ động (hay Buy Up) là khi NĐT thực hiện chủ động mua lên qua việc đặt lệnh mua với giá bằng giá dư bán gần nhất để có thể khớp luôn. Như thế, giá khớp cho lệnh này thường sẽ đẩy giá khớp lên cao hơn thị giá trước đó.
-
-  • Bán chủ động (hay Sell Down) là khi NĐT thực hiện chủ động Bán dưới giá hiện tại (hay thị giá) của cổ phiếu bằng việc đặt lệnh bán với giá bán bằng giá dư mua gần nhất để khớp ngay. Và như thế, thị giá sẽ bị kéo xuống thấp hơn so với thị giá trước đó. Thống kê khối lượng giao dich theo Mua CĐ và Bán CĐ dùng để đánh giá tương quan giữa cung (Bán CĐ) và cầu (Mua CĐ) trên giao dịch khớp lệnh thực tế, nhằm nhận định tương đối về sự vận động của xu hướng dòng tiền. Khi tỷ lệ % Mua CĐ trên (Tổng Mua và Bán CĐ) lớn hơn 50%, đồng nghĩa với việc thị trường đang có xu hướng mua vào nhiều hơn bán ra và ngược lại, qua đó xác định được dòng tiền vào/ra với mỗi cổ phiếu. Khi tỷ lệ này cao đột biến (>70% hay <30%) so với điểm cân bằng (50%) , đó là tín hiệu của việc mua hoặc bán bất chấp của thị trường.
-
-</details>
-
-## 3.6. 💰 Các chỉ số tài chính
-
-### 3.6.1. Bộ chỉ số tài chính của một mã cổ phiếu
-```python
-financial_ratio(symbol="TCB", report_range='yearly', is_all=False)
-```
-Trong đó:
-- `report_range` nhận 1 trong 2 giá trị: `yearly` cho phép trả về chỉ số theo năm, `quarterly` trả về dữ liệu theo quý
-- `is_all` có giá trị mặc định là `True` cho phép lấy chỉ số qua tất cả các kỳ (năm hoặc quý), `False` cho phép lấy các kỳ gần nhất (5 năm hoặc 10 quý gần đây).
-
-<details>
-  <summary>Output</summary>
-
-  ```
->>> financial_ratio('TCB', 'yearly')
-year                      2022   2021   2020   2019   2018
-ticker                     TCB    TCB    TCB    TCB    TCB
-priceToEarning             4.5    9.7    9.0    8.2   10.7
-priceToBook                0.8    1.9    1.5    1.3    1.8
-roe                      0.197  0.217  0.181  0.178  0.215
-roa                      0.032  0.036   0.03  0.029  0.029
-earningPerShare           5729   5132   3504   2869   2410
-bookValuePerShare        32248  26452  21214  17679  14749
-interestMargin           0.053  0.057  0.049  0.043  0.041
-nonInterestOnToi         0.259   0.28  0.307  0.323  0.379
-badDebtPercentage        0.007  0.007  0.005  0.013  0.018
-provisionOnBadDebt       1.573  1.629   1.71  0.948  0.851
-costOfFinancing          0.028  0.022  0.031  0.038  0.041
-equityOnTotalAsset       0.162  0.164   0.17  0.162  0.161
-equityOnLoan              0.27  0.268  0.269  0.269  0.324
-costToIncome             0.328  0.301  0.319  0.347  0.318
-equityOnLiability          0.2    0.2    0.2    0.2    0.2
-epsChange                0.116  0.465  0.221  0.191  0.313
-assetOnEquity              6.2    6.1    5.9    6.2    6.2
-preProvisionOnToi        0.537  0.554  0.542   0.52  0.542
-postTaxOnToi               0.5  0.497  0.465  0.485  0.462
-loanOnEarnAsset          0.684  0.665  0.681  0.649  0.537
-loanOnAsset              0.602  0.611  0.631  0.602  0.498
-loanOnDeposit            1.173  1.104    1.0  0.998  0.794
-depositOnEarnAsset       0.583  0.603   0.68  0.651  0.676
-badDebtOnAsset           0.004  0.004  0.003  0.008  0.009
-liquidityOnLiability     0.347  0.382  0.372  0.411  0.531
-payableOnEquity            5.2    5.1    4.9    5.2    5.2
-cancelDebt               0.002  0.004  0.013  0.002  0.008
-bookValuePerShareChange  0.219  0.247    0.2  0.199  0.923
-creditGrowth             0.211  0.252  0.202  0.443 -0.006
-  ```
-</details>
+#### 3.5.1.2. 🏭 Phân tích chỉ số các cổ phiếu cùng ngành (Industry Analysis)
 
-## 3.7. So sánh cổ phiếu
-### 3.7.1. 🏭 Phân tích chỉ số các cổ phiếu cùng ngành
 ```python
 industry_analysis("VNM", lang='vi)
 ```
 - Trả về thông tin các mã cổ phiếu cùng ngành với mã cổ phiếu nằm trong cùng nhóm ngành với mã `VNM`.
 - Tham số `lang='vi` mặc định trả về tên các chỉ số bằng tiếng Việt, đổi thành `en` để giữ nguyên chỉ số với tên tiếng Anh.
 
 - Trong đó các chỉ số sau được thể hiện dưới dạng thập phân sử dụng để thể hiện chỉ số dưới dạng %: 
@@ -399,15 +486,16 @@
 Doanh thu quý gần nhất         NaN  -0.094 -0.252  0.093 -0.302  -0.057 -0.181  0.031 -0.352 -0.067  -0.31 -0.675 -0.197 -0.134 -0.123  0.102  -0.122 -0.142  0.009
 LNST năm tới                   NaN   0.285   0.26  0.173 -0.202   0.074  0.047 -0.719 -0.041   0.04 -0.939  0.116  6.025 -0.034   0.09 -0.155   0.813  0.022    NaN
 Doanh thu năm tới              NaN     0.2    0.3  0.162  0.283     0.1    0.1   -0.7   0.05   0.05   0.03   0.15   -0.5    0.1    0.3  -0.08   -0.06   0.02    NaN
 RSI                            NaN    50.7   43.1   71.8   24.0    28.5   59.2   33.7   68.2   53.5   46.6   44.1   51.1   32.3   55.5   55.3    33.3   54.8   61.1
 ```
 </details>
 
-### 3.7.2. 🔬 So sánh các chỉ số của danh sách các cổ phiếu tùy chọn
+
+#### 3.5.1.3. 🔬 So sánh các chỉ số của danh sách các cổ phiếu tùy chọn
 ```python
 stock_ls_analysis("TCB, BID, CEO, GMD", lang='vi')
 ```
 
 <details>
   <summary>Output</summary>
 
@@ -419,188 +507,327 @@
 1    CEO   17062  66300             1           183.2 -0.8          5.7               81.8       0.0  ...           7.8       -0.099     -0.086            NaN         3.002      -1.469      -0.2  51.9  82.0
 2    BID  225357  44550            -3            21.3  0.4          2.6                NaN       0.0  ...           NaN        0.115      0.154          0.083         0.000         NaN       NaN  49.1  34.0
 3    TCB  178003  50700             1             9.9  0.2          1.9                NaN       0.0  ...           NaN        0.418      0.255          0.059         0.157         NaN       NaN  45.2  28.0
 ```
 
 </details>
 
-### 3.7.4. 💵 Báo cáo kết quả kinh doanh, cân đối kế toán và lưu chuyển tiền tệ
 
-#### 3.7.4.1. 📄 Báo cáo kinh doanh
+#### 3.5.1.4. ⭐ Đánh giá xếp hạng 
+##### a. Đánh giá chung
+![general_rating](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/general_rating.png)
 
-![income_statement](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_income_statement.png)
 ```python
-financial_flow(symbol="TCB", report_type='incomestatement', report_range='quarterly')
+general_rating("VNM")
 ```
 
-
 <details>
   <summary>Output</summary>
 
 ```
-        ticker  revenue  yearRevenueGrowth  quarterRevenueGrowth costOfGoodSold grossProfit  ...  investProfit  serviceProfit  otherProfit  provisionExpense operationIncome  ebitda
-index                                                                                        ...
-2021-Q4    TCB     7245              0.328                 0.074           None        None  ...           279           2103          532              -627            6767    None
-2021-Q3    TCB     6742              0.310                 0.023           None        None  ...           384           1497          156              -589            6151    None
-2021-Q2    TCB     6588              0.674                 0.076           None        None  ...           717           1457          444              -598            6615    None
-2021-Q1    TCB     6124              0.454                 0.122           None        None  ...           812           1325          671              -851            6369    None
+   stockRating  valuation  financialHealth  businessModel  businessOperation  rsRating  taScore  ... ticker highestPrice  lowestPrice  priceChange3m  priceChange1y  beta   alpha
+0          2.4        1.5              4.8            3.0                3.2       1.0      1.0  ...    VNM     102722.2      78600.0         -0.092         -0.232  0.49 -0.0014
 ```
 </details>
 
-#### 3.7.4.2. 🧾 Bảng cân đối kế toán
-
-![balance_sheet](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_balancesheet.png)
+##### b. 🌱 Đánh giá mô hình kinh doanh
 ```python
-financial_flow(symbol="TCB", report_type='balancesheet', report_range='quarterly')
+biz_model_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-        ticker shortAsset  cash shortInvest shortReceivable inventory longAsset  fixedAsset  ...  payableInterest  receivableInterest deposit otherDebt  fund  unDistributedIncome  minorShareHolderProfit  payable
-index                                                                                        ...
-
-2021-Q4    TCB       None  3579        None            None      None      None        7224  ...             3098                5808  314753     33680  9156                47469                     845   475756
-2021-Q3    TCB       None  3303        None            None      None      None        7106  ...             3074                6224  316376     34003  6784                45261                     753   453251
-2021-Q2    TCB       None  3554        None            None      None      None        6739  ...             2643                5736  289335     27678  6790                40924                     659   420403
-2021-Q1    TCB       None  4273        None            None      None      None        4726  ...             2897                5664  287446     26035  6790                36213                     563   3837
+  ticker  businessModel  businessEfficiency  assetQuality  cashFlowQuality  bom  businessAdministration  productService  businessAdvantage  companyPosition  industry  operationRisk
+0    VNM            3.0                   3             3                3    3                       3               3                  3                3         3              3
 ```
 </details>
 
-#### 3.7.4.3. 💶 Báo cáo lưu chuyển tiền tệ
-
+##### c. 🎮 Đánh giá hiệu quả hoạt động
 ```python
-financial_flow(symbol="TCB", report_type='cashflow', report_range='quarterly')
+biz_operation_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-        ticker  investCost  fromInvest  fromFinancial  fromSale  freeCashFlow
-index
-2021-Q4    TCB        -280        -276              0     -9328             0
-2021-Q3    TCB        -180        -179             60     17974             0
-2021-Q2    TCB        -337        -282              0     11205             0
-2021-Q1    TCB        -143        -143              0     -6954             0
+      industryEn loanGrowth depositGrowth netInterestIncomeGrowth netInterestMargin  ... last5yearsFCFFGrowth lastYearGrossProfitMargin lastYearOperatingProfitMargin  lastYearNetProfitMargin  TOIGrowth
+0  Food Products       None          None                    None              None  ...                    2                         5                             3                        4       None
 ```
 </details>
 
-## 3.8. 🧧 Lịch sử chi trả cổ tức
-
+##### d. 📑 Đánh giá sức khỏe tài chính
 ```python
-dividend_history("VNM")
+financial_health_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-   exerciseDate  cashYear  cashDividendPercentage issueMethod
-0      10/01/22      2021                    0.14        cash
-1      07/09/21      2021                    0.15        cash
-2      07/06/21      2020                    0.11        cash
-3      05/01/21      2020                    0.10        cash
+      industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
+0  Food Products        None             None         None             None    VNM              4.8              4             5           5                 5              5
 ```
 </details>
 
-## 3.9. ⭐ Đánh giá xếp hạng 
-### 3.9.1. Đánh giá chung
-![general_rating](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/general_rating.png)
-
+##### e. 💲 Đánh giá về Định giá
 ```python
-general_rating("VNM")
+valuation_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-   stockRating  valuation  financialHealth  businessModel  businessOperation  rsRating  taScore  ... ticker highestPrice  lowestPrice  priceChange3m  priceChange1y  beta   alpha
-0          2.4        1.5              4.8            3.0                3.2       1.0      1.0  ...    VNM     102722.2      78600.0         -0.092         -0.232  0.49 -0.0014
+      industryEn ticker  valuation  pe  pb  ps  evebitda  dividendRate
+0  Food Products    VNM        1.5   2   1   1         1             3
 ```
 </details>
 
-### 3.9.2. 🌱 Đánh giá mô hình kinh doanh
+##### f. 💳 Sức khỏe tài chính theo ngành
 ```python
-biz_model_rating("VNM")
+industry_financial_health("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-  ticker  businessModel  businessEfficiency  assetQuality  cashFlowQuality  bom  businessAdministration  productService  businessAdvantage  companyPosition  industry  operationRisk
-0    VNM            3.0                   3             3                3    3                       3               3                  3                3         3              3
+  industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
+0       None        None             None         None             None    VNM              3.4              4             4           3                 3              3
 ```
 </details>
 
-### 3.9.3. 🎮 Đánh giá hiệu quả hoạt động
-```python
-biz_operation_rating("VNM")
-```
+### 3.5.2. 🔎 Bộ lọc cổ phiếu
+
+Bộ lọc cổ phiếu là một hàm cho phép bạn truy vấn và lọc các cổ phiếu theo nhiều tiêu chí đa dạng dựa trên dữ liệu phân tích của TCBS. Hàm này sẽ trả về một DataFrame chứa các thông tin toàn diện về các cổ phiếu thỏa mãn điều kiện lọc của bạn. Bạn có thể dùng DataFrame này để tiếp tục phân tích, biểu diễn hoặc xuất ra dữ liệu dạng bảng tính. Đây là cập nhật ưu việt giúp bạn tiết kiệm thời gian và công sức đáng kể khi làm việc với dữ liệu cổ phiếu, đồng thời cho phép lập trình để lọc là cập nhật danh sách cổ phiếu hiệu quả không cần sử dụng giao diện web từ công ty chứng khoán.
 
 <details>
-  <summary>Output</summary>
+  <summary> Bộ lọc cổ phiếu TCBS </summary>
+
+  ![stock_scanner](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/stock_scanner_tcbs.png)
 
-```
-      industryEn loanGrowth depositGrowth netInterestIncomeGrowth netInterestMargin  ... last5yearsFCFFGrowth lastYearGrossProfitMargin lastYearOperatingProfitMargin  lastYearNetProfitMargin  TOIGrowth
-0  Food Products       None          None                    None              None  ...                    2                         5                             3                        4       None
-```
 </details>
 
-### 3.9.4. 📑 Đánh giá sức khỏe tài chính
-```python
-financial_health_rating("VNM")
-```
+Tham số
+- params (dict): một từ điển chứa các tham số và giá trị của chúng cho việc lọc cổ phiếu. Các `key` là tên của các bộ lọc, và các `value` là một giá trị đơn hoặc một tupple gồm hai giá trị (min và max) cho bộ lọc đó. Đây là ví dụ cho tham số params được thiết lập đúng:
+
+```python
+params = {
+            "exchangeName": "HOSE",
+            "marketCap": (100, 1000),
+            "pe": (10, 20),
+            "dividendYield": (5, 10),
+            "tcbsRecommend": "BUY",
+            "size": 50
+        }
+
+# Áp dụng bộ lọc với hàm để lấy kết quả
+get_stock_screening_insights(params)
+```
+
+<details>
+
+<summary>Các bộ lọc gợi ý và tiêu chí hỗ trợ bao gồm</summary>
+
+  a. BỘ LỌC GỢI Ý (PRESET)
+
+    > Sử dụng các tiêu chí lọc như sau để thiết lập tham số params.
+
+    - CANSLIM: epsGrowth1Year, lastQuarterProfitGrowth, roe, avgTradingValue20Day, relativeStrength1Month
+    - Giá trị: roe, pe, avgTradingValue20Day
+    - Cổ tức cao: dividendYield, avgTradingValue20Day
+    - Phá nền mua: avgTradingValue20Day, forecastVolumeRatio, breakout: 'BULLISH'
+    - Giá tăng + Đột biến khối lượng: avgTradingValue20Day, forecastVolumeRatio
+    - Vượt đỉnh 52 tuần: avgTradingValue20Day, priceBreakOut52Week: 'BREAK_OUT'
+    - Phá đáy 52 tuần: avgTradingValue20Day, priceWashOut52Week: 'WASH_OUT'
+    - Uptrend ngắn hạn: avgTradingValue20Day, uptrend: 'buy-signal'
+    - Vượt trội ngắn hạn: relativeStrength3Day, 
+    - Tăng trưởng: epsGrowth1Year, roe, avgTradingValue20Day
+
+  b. THÔNG TIN CHUNG
+
+    - exchangeName: sàn giao dịch của cổ phiếu, ví dụ "HOSE", "HNX", hoặc "UPCOM". Bạn có thể dùng dấu phẩy để phân tách nhiều sàn, ví dụ "HOSE,HNX,UPCOM".
+    - hasFinancialReport: Có báo cáo tài chính gần nhất. `1` nghĩa là có, `0` nghĩa là không.
+    - industryName: Lọc các cổ phiếu theo ngành cụ thể. Giá trị dạng `Retail` cho ngành Bán lẻ. Các giá trị khác có thể là:
+      - `Insurance`: Bảo hiểm
+      - `Real Estate`: Bất động sản
+      - `Technology`: Công nghệ thông tin
+      - `Oil & Gas`: Dầu khí
+      - `Financial Services`: Dịch vụ tài chính
+      - `Utilities`: Điện, nước, xăng dầu và khí đốt
+      - `Travel & Leisure`: Du lịch và giải trí
+      - `Industrial Goods & Services`: Hàng và dịch vụ công nghiệp
+      - `Personal & Household Goods`: Hàng cá nhân và gia dụng
+      - `Chemicals`: Hóa chất
+      - `Banks`: Ngân hàng
+      - `Automobiles & Parts`: Ô tô và phụ tùng
+      - `Basic Resources`: Tài nguyên cơ bản
+      - `Food & Beverage`: Thực phẩm và đồ uống
+      - `Media`: Truyền thông
+      - `Telecommunications`: Viễn thông
+      - `Construction & Materials`: Xây dựng và vật liệu
+      - `Health Care`: Y tế
+      - marketCap: vốn hóa thị trường của cổ phiếu tính bằng tỷ VND.
+      - priceNearRealtime: giá hiện tại của cổ phiếu tính bằng VND.
+      - foreignVolumePercent: tỷ lệ phần trăm khối lượng nước ngoài trong tổng khối lượng.
+      - alpha: lợi nhuận vượt trội của cổ phiếu so với lợi nhuận thị trường.
+      - beta: độ biến động của cổ phiếu so với thị trường.
+      - freeTransferRate: tỷ lệ phần trăm cổ phiếu có thể chuyển nhượng tự do.
+  
+  c. TĂNG TRƯỞNG
 
-<details>
-  <summary>Output</summary>
+    - revenueGrowth1Year: tốc độ tăng trưởng doanh thu trong năm qua.
+    - revenueGrowth5Year: tốc độ tăng trưởng doanh thu trung bình trong 5 năm qua.
+    - epsGrowth1Year: tốc độ tăng trưởng lợi nhuận trên mỗi cổ phiếu trong năm qua.
+    - epsGrowth5Year: tốc độ tăng trưởng lợi nhuận trên mỗi cổ phiếu trung bình trong 5 năm qua.
+    - lastQuarterRevenueGrowth: tốc độ tăng trưởng doanh thu trong quý gần nhất.
+    - secondQuarterRevenueGrowth: tốc độ tăng trưởng doanh thu trong quý thứ hai.
+    - lastQuarterProfitGrowth: tốc độ tăng trưởng lợi nhuận trong quý gần nhất.
+    - secondQuarterProfitGrowth: tốc độ tăng trưởng lợi nhuận trong quý thứ hai.
+  
+  d. CHỈ SỐ TÀI CHÍNH
+  
+    - grossMargin: tỷ suất lợi nhuận gộp của cổ phiếu.
+    - netMargin: tỷ suất lợi nhuận ròng của cổ phiếu.
+    - roe: tỷ suất sinh lời về vốn chủ sở hữu của cổ phiếu.
+    - doe: tỷ suất cổ tức về vốn chủ sở hữu của cổ phiếu.
+    - dividendYield: tỷ suất cổ tức của cổ phiếu.
+    - eps: lợi nhuận trên mỗi cổ phiếu của cổ phiếu tính bằng VND.
+    - pe: tỷ số giá/lợi nhuận của cổ phiếu.
+    - pb: tỷ số giá/giá trị sổ sách của cổ phiếu.
+    - evEbitda: tỷ số giá trị doanh nghiệp/lợi nhuận trước thuế, lãi vay, khấu hao và amortization của cổ phiếu.
+    - netCashPerMarketCap: tỷ số tiền mặt ròng/vốn hóa thị trường của cổ phiếu.
+    - netCashPerTotalAssets: tỷ số tiền mặt ròng/tổng tài sản của cổ phiếu.
+    - profitForTheLast4Quarters: tổng lợi nhuận trong 4 quý gần nhất của cổ phiếu tính bằng tỷ VND.
+  
+  e. BIẾN ĐỘNG GIÁ & KHỐI LƯỢNG
+
+    - suddenlyHighVolumeMatching: tín hiệu chỉ ra nếu có sự tăng đột biến khối lượng khớp lệnh cho cổ phiếu này. 0 nghĩa là không, 1 nghĩa là có.
+    - totalTradingValue: tổng giá trị giao dịch của cổ phiếu này tính bằng tỷ VND hôm nay.
+    - avgTradingValue5Day: giá trị giao dịch trung bình của cổ phiếu này tính bằng tỷ VND trong 5 ngày.
+    - avgTradingValue10Day: giá trị giao dịch trung bình của cổ phiếu này tính bằng tỷ VND trong 10 ngày.
+    - avgTradingValue20Day: giá trị giao dịch trung bình của cổ phiếu này tính bằng tỷ VND trong 20 ngày.
+    - priceGrowth1Week: tốc độ tăng trưởng giá của cổ phiếu trong tuần qua.
+    - priceGrowth1Month: tốc độ tăng trưởng giá của cổ phiếu trong tháng qua.
+    - percent1YearFromPeak: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá cao nhất trong 1 năm.
+    - percentAwayFromHistoricalPeak: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá cao nhất lịch sử.
+    - percent1YearFromBottom: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá thấp nhất trong 1 năm.
+    - percentOffHistoricalBottom: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá thấp nhất lịch sử.
+    - priceVsSMA5: mối quan hệ giữa giá hiện tại và SMA 5 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSma10: mối quan hệ giữa giá hiện tại và SMA 10 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSMA20: mối quan hệ giữa giá hiện tại và SMA 20 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSma50: mối quan hệ giữa giá hiện tại và SMA 50 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSMA100: mối quan hệ giữa giá hiện tại và SMA 100 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - forecastVolumeRatio: tỷ số giữa khối lượng dự báo và khối lượng thực tế của cổ phiếu hôm nay.
+    - volumeVsVSma5: tỷ số giữa khối lượng hiện tại và SMA khối lượng 5 ngày của cổ phiếu.
+    - volumeVsVSma10: tỷ số giữa khối lượng hiện tại và SMA khối lượng 10 ngày của cổ phiếu.
+    - volumeVsVSma20: tỷ số giữa khối lượng hiện tại và SMA khối lượng 20 ngày của cổ phiếu.
+    - volumeVsVSma50: tỷ số giữa khối lượng hiện tại và SMA khối lượng 50 ngày của cổ phiếu.
+  
+  f. HÀNH VI THỊ TRƯỜNG
+
+    - strongBuyPercentage: tỷ lệ phần trăm tín hiệu mua mạnh cho cổ phiếu này dựa trên phân tích kỹ thuật.
+    - activeBuyPercentage: tỷ lệ phần trăm tín hiệu mua tích cực cho cổ phiếu này dựa trên phân tích kỹ thuật.
+    - foreignTransaction: loại giao dịch nước ngoài cho cổ phiếu này hôm nay. Các giá trị có thể là "buyMoreThanSell", "sellMoreThanBuy", hoặc "noTransaction".
+    - foreignBuySell20Session: giá trị mua bán ròng nước ngoài cho cổ phiếu này tính bằng tỷ VND trong 20 phiên.
+    - numIncreaseContinuousDay: số ngày liên tiếp cổ phiếu này tăng giá.
+    - numDecreaseContinuousDay: số ngày liên tiếp cổ phiếu này giảm giá.
+  
+  g. TÍN HIỆU KỸ THUẬT
+
+    - rsi14: chỉ số sức mạnh tương đối (RSI) của cổ phiếu với chu kỳ 14 ngày.
+    - rsi14Status: trạng thái của RSI cho cổ phiếu này. Các giá trị có thể là "intoOverBought", "intoOverSold", "outOfOverBought", hoặc "outOfOverSold".
+    - tcbsBuySellSignal: tín hiệu mua bán cho cổ phiếu này dựa trên phân tích của TCBS. Các giá trị có thể là "BUY" hoặc "SELL".
+    - priceBreakOut52Week: tín hiệu chỉ ra nếu có sự đột phá giá cho cổ phiếu này trong 52 tuần. Các giá trị có thể là "BREAK_OUT" hoặc "NO_BREAK_OUT".
+    - priceWashOut52Week: tín hiệu chỉ ra nếu có sự rửa giá cho cổ phiếu này trong 52 tuần. Các giá trị có thể là "WASH_OUT" hoặc "NO_WASH_OUT".
+    - macdHistogram: tín hiệu chỉ ra nếu có tín hiệu MACD histogram cho cổ phiếu này. Các giá trị có thể là "macdHistGT0Increase", "macdHistGT0Decrease", "macdHistLT0Increase", hoặc "macdHistLT0Decrease".
+    - relativeStrength3Day: sức mạnh tương đối của cổ phiếu so với thị trường trong 3 ngày.
+    - relativeStrength1Month: sức mạnh tương đối của cổ phiếu so với thị trường trong 1 tháng.
+    - relativeStrength3Month: sức mạnh tương đối của cổ phiếu so với thị trường trong 3 tháng.
+    - relativeStrength1Year: sức mạnh tương đối của cổ phiếu so với thị trường trong 1 năm.
+    - tcRS: sức mạnh tương đối của TCBS của cổ phiếu so với thị trường.
+    - sarVsMacdHist: tín hiệu chỉ ra nếu có tín hiệu SAR vs MACD histogram cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+  
+  h. TÍN HIỆU MUA/BÁN
+
+    - bollingBandSignal: tín hiệu chỉ ra nếu có tín hiệu Bollinger Band cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+    - dmiSignal: tín hiệu chỉ ra nếu có tín hiệu chỉ số chuyển động hướng (DMI) cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+    - uptrend: tín hiệu chỉ ra nếu có tín hiệu xu hướng tăng cho cổ phiếu này. Các giá trị có thể là "buy-signal" hoặc "sell-signal".
+    - breakout: tín hiệu chỉ ra nếu có tín hiệu đột phá cho cổ phiếu này. Các giá trị có thể là "BULLISH" hoặc "BEARISH".
+  
+  i. TCBS ĐÁNH GIÁ
+
+    - tcbsRecommend: tín hiệu chỉ ra nếu có khuyến nghị của TCBS cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+    - stockRating: điểm đánh giá cổ phiếu cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
+    - businessModel: điểm đánh giá mô hình kinh doanh cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
+    - businessOperation: điểm đánh giá hoạt động kinh doanh cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
+    - financialHealth: điểm đánh giá sức khỏe tài chính cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
 
-```
-      industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
-0  Food Products        None             None         None             None    VNM              4.8              4             5           5                 5              5
-```
 </details>
 
-### 3.9.5. 💲 Đánh giá về Định giá
-```python
-valuation_rating("VNM")
-```
+
+## 3.6. 🔥 Dữ liệu khớp lệnh trong ngày giao dịch
 
 <details>
-  <summary>Output</summary>
+  <summary>Minh hoạ giao diện TCBS</summary>
+
+  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen1.png)
+  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen2.png)
 
-```
-      industryEn ticker  valuation  pe  pb  ps  evebitda  dividendRate
-0  Food Products    VNM        1.5   2   1   1         1             3
-```
 </details>
+vnstock cho phép người dùng tải xuống dữ liệu khớp lệnh trong ngày giao dịch theo thời gian thực. Nếu mốc thời gian bạn truy cứu rơi vào Thứ Bảy, Chủ Nhật thì dữ liệu nhận được thể hiện cho ngày giao dịch của Thứ 6 của tuần đó.
 
-## 3.10.  💳 Sức khỏe tài chính theo ngành
 ```python
-industry_financial_health("VNM")
+df =  stock_intraday_data(symbol='TCB', 
+                            page_size=500)
+print(df)
 ```
 
 <details>
-  <summary>Output</summary>
+  <summary>Terminal output</summary>
+
+  ```{r, engine='python', count_lines}
+>>> stock_intraday_data('TCB', 500)
+
+  ticker      time  orderType investorType  volume  averagePrice  orderCount
+0    TCB  14:29:55  Sell Down        SHEEP    1000       32700.0           1
+1    TCB  14:29:47     Buy Up        SHEEP     200       32750.0           1
+2    TCB  14:29:44  Sell Down         WOLF    8000       32700.0          14
+3    TCB  14:29:41  Sell Down        SHEEP    1000       32700.0           5
+4    TCB  14:29:36  Sell Down         WOLF   23800       32700.0          10
+  ```
+
+</details>
+
+<details>
+  <summary>Giải thích ý nghĩa chỉ số</summary>
+  • Khi 1 lệnh lớn (từ Cá mập, tay to, tổ chức....) mua chủ động (hoặc bán chủ động) được đưa vào Sàn, thường thì nó sẽ được khớp với nhiều lệnh nhỏ đang chờ bán (hoặc chờ mua). Nếu chỉ nhìn realtime theo từng lệnh khớp riêng lẻ, thì sẽ không thể phát hiện được các lệnh to (của Cá mập, tay to...) vừa được đẩy vào Sàn. Vì vậy, chúng tôi "cộng dồn" các lệnh khớp này lại (phát sinh bởi 1 lệnh lớn chủ động vào sàn trong 1 khoảng thời gian rất nhanh) để giúp NĐT phát hiện các lệnh lớn (của Cá mập, tay to....) chính xác hơn. Lệnh Cá mập sẽ được tô xanh (cho Mua chủ động) và đỏ (cho Bán chủ động). 
+
+  • Cá mập: (CM - SHARK) nhà đầu tư tay to, tổ chức, đầu tư lớn, dẫn dắt thị trường. Giá trị 1 lệnh đặt > 1 tỷ đồng/lệnh đặt. Đồ thị 1N dùng số liệu 1 phút cho 60’ gần nhất; 1W là tổng mỗi 15’ cho 1 tuần; 1M là tổng hàng ngày cho 1 tháng
+
+  • Sói già: (SG - WOLF) nhà đầu tư kinh nghiệm, giá trị lệnh đặt cao. Giá trị 1 lệnh đặt từ 200 tr đến 1 tỷ đồng/lệnh đặt.
+
+  • Cừu non: (CN - SHEEP) nhà đầu tư nhỏ lẻ, giá trị giao dịch và mua bán chủ động thấp. Giá trị 1 lệnh đặt Mua hoặc Bán chủ động < 200 triệu đồng/lệnh đặt vào.
+
+  • Mua chủ động (hay Buy Up) là khi NĐT thực hiện chủ động mua lên qua việc đặt lệnh mua với giá bằng giá dư bán gần nhất để có thể khớp luôn. Như thế, giá khớp cho lệnh này thường sẽ đẩy giá khớp lên cao hơn thị giá trước đó.
+
+  • Bán chủ động (hay Sell Down) là khi NĐT thực hiện chủ động Bán dưới giá hiện tại (hay thị giá) của cổ phiếu bằng việc đặt lệnh bán với giá bán bằng giá dư mua gần nhất để khớp ngay. Và như thế, thị giá sẽ bị kéo xuống thấp hơn so với thị giá trước đó. Thống kê khối lượng giao dich theo Mua CĐ và Bán CĐ dùng để đánh giá tương quan giữa cung (Bán CĐ) và cầu (Mua CĐ) trên giao dịch khớp lệnh thực tế, nhằm nhận định tương đối về sự vận động của xu hướng dòng tiền. Khi tỷ lệ % Mua CĐ trên (Tổng Mua và Bán CĐ) lớn hơn 50%, đồng nghĩa với việc thị trường đang có xu hướng mua vào nhiều hơn bán ra và ngược lại, qua đó xác định được dòng tiền vào/ra với mỗi cổ phiếu. Khi tỷ lệ này cao đột biến (>70% hay <30%) so với điểm cân bằng (50%) , đó là tín hiệu của việc mua hoặc bán bất chấp của thị trường.
 
-```
-  industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
-0       None        None             None         None             None    VNM              3.4              4             4           3                 3              3
-```
 </details>
 
-## 3.11. 🌏 Thông tin thị trường
+
+## 3.7. 🌏 Thông tin thị trường
 
 <details>
-  <summary>Tạm ngưng hoạt động do SSI từ chối truy cập</summary>
+  <summary>Tạm ngưng hoạt động, chờ nâng cấp APIs</summary>
 
-### 3.11.1. Các mã cổ phiếu đứng đầu theo tiêu chí xếp loại 
+### 3.7.1. Các mã cổ phiếu đứng đầu theo tiêu chí xếp loại 
 
 <details>
   <summary>SSI Top Stocks</summary>
 
 Top Breakout (Đột phá) > Top Gainers (Tăng giá) > Top Losers (Giảm giá) > Top Value (Giá trị) > Top Volume (Khối lượng)
 ![top_mover](./src/ssi_top_breakout_gainer_loser.png)
 
@@ -622,15 +849,15 @@
 1          3270200.0     1.088892e+11  ...  {'organCode': 'STB', 'rtd7': 18173.6958318461,...  {'organCode': 'STB', 'sma20Past4': 34332.5, 's...
 2          1456800.0     4.199166e+10  ...  {'organCode': 'FUEVFVND', 'rtd7': None, 'rtd11...  {'organCode': 'FUEVFVND', 'sma20Past4': 27993....
 3          1033300.0     1.281170e+10  ...  {'organCode': 'FLC', 'rtd7': 12898.0038031343,...  {'organCode': 'FLC', 'sma20Past4': 12062.5, 's...
 4           998600.0     5.324337e+10  ...  {'organCode': 'NLG', 'rtd7': 23318.1252311207,...  {'organCode': 'NLG', 'sma20Past4': 52385.0, 's...
 ```
 </details>
 
-### 3.11.2. Thông tin giao dịch nhà đầu tư nước ngoài (NDTNN)
+### 3.7.2. Thông tin giao dịch nhà đầu tư nước ngoài (NDTNN)
 Trong ví dụ dưới đây, thể hiện giao dịch mua vào của NDTNN.
 
 ```python
 fr_trade_heatmap ('All', 'FrBuyVol')
 ```
 <details>
   <summary>Output</summary>
@@ -649,15 +876,15 @@
   2        ELC   ELC     4100.0            0.049197  ...       10650.0      9270.0  Công nghệ Thông tin  0.034816
   3        ITD   ITD     2000.0            0.068548  ...       13250.0     11550.0  Công nghệ Thông tin  0.034816
 
   [92 rows x 10 columns]
   ```
 </details>
 
-### 3.11.3. Biến động của các nhóm chỉ số
+### 3.7.3. Biến động của các nhóm chỉ số
 ![latest_indices](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/get_latest_indices.png)
 
 Thông tin các nhóm chỉ số phổ biến của thị trường chứng khoán Việt Nam.
 
 ```python
 get_latest_indices()
 ```
@@ -692,16 +919,16 @@
 21        0         VNSI     1715.37  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
 22        0        VNSML     1140.40  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
 23        0        VNUTI      874.84  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
 24        0        VNX50     1805.33  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
   ```
 </details>
 
-### 3.11.4. Dữ liệu chuyên sâu theo nhóm chỉ số cụ thể
-![index_series_data](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/get_index_series_data.png)
+### 3.7.4. Dữ liệu chuyên sâu theo nhóm chỉ số cụ thể
+![index_series_data](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/get_index_series_data.png)
 
 ```python
 get_index_series(index_code='VNINDEX', time_range='OneYear')
 ```
 - Nhà cung cấp dữ liệu: SSI iBoard sử dụng dữ liệu từ FiinTrade.
 - Sử dụng một trong các mã chỉ số sau để tra cứu:
   
@@ -737,15 +964,65 @@
 
   [246 rows x 14 columns]
   ```
 </details>
 
 </details>
 
-# IV. 🙋‍♂️ Contact Information
+## 3.8. 🛡 Thị trường Phái Sinh
+
+### 3.8.1. Dữ liệu giá lịch sử
+
+> Xem chi tiết mục [3.4.1 📈 Truy xuất dữ liệu giá lịch sử](#341--truy-xuất-dữ-liệu-giá-lịch-sử) cùng với thông tin giá chứng khoán cơ sở.
+
+### 3.8.2. Dữ liệu khớp lệnh lịch sử
+
+<details>
+
+<summary>Minh họa bảng dữ liệu khớp lệnh Phái sinh - CK Rồng Việt </summary>
+
+![livedragon_derivative_match](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/livedragon_derivative_history_match.png)
+
+</details>
+
+Để truy vấn dữ liệu từ hàm này, bạn cần có cookie người dùng (không cần đăng nhập) của chứng khoán Rồng Việt. Các bước thực hiện như sau:
+  1. Truy cập `https://livedragon.vdsc.com.vn/all/all.rv`
+  2. Mở `Developer Tools` trên trình duyệt, sử dụng F12 hoặc `Ctrl` + `Shift` + `I` trên Windows hoặc `Cmd` + `Option` + `I` trên macOS
+  3. Chuyển đến tab `Network` và chọn mục `Fetch/XHR`
+  4. Mở bất kỳ mục request nào trong tab này, tìm mục `Header` của request
+  5. Tìm và copy giá trị của `Cookie` trong request này để điền vào bước tiếp theo dưới đây trước khi gọi hàm
+
+```python
+cookie = 'GIÁ TRỊ COOKIE CẦN PASTE VÀO ĐÂY'
+derivatives_historical_match (symbol='VN30F2308', date='2023-07-24', cookie=cookie)
+```
+
+# IV. 🚚 Xuất, Lưu trữ, Chia sẻ dữ liệu
+
+> Để xuất, lưu trữ và chia sẻ dữ liệu với vnstock, bạn có rất nhiều sự lựa chọn kể cả sử dụng cơ sở dữ liệu, bảng tính (Excel, Google Sheets) và nhiều hình thức khác. Dữ liệu tiêu chuẩn tạo ra bởi vnstock là các pandas DataFrame do đó bạn có thể biến đổi và lưu trữ/chia sẻ dữ liệu dễ dàng với cách thức tiêu chuẩn của python. Dưới đây là hướng dẫn cơ bản với cách thức xuất dữ liệu ra csv và Google Sheets.
+
+## 4.1. Xuất dữ liệu ra csv
+
+Dành cho những bạn mới làm quen Python và Pandas có thể sử dụng dữ liệu từ vnstock dễ dàng với công cụ bảng tính quen thuộc. Bạn có thể xuất dữ liệu từ hàm bất kỳ ra csv và mở bằng Excel hoặc upload lên Google Drive và mở bằng Google Sheets.
+
+```python
+start_date = '2023-06-01'
+end_date = '2023-07-24'
+# Truy xuất dữ liệu
+df = stock_historical_data('TCB', start_date, end_date)
+# Xuất dữ liệu ra csv, chèn ngày tháng và mã CP
+df.to_csv(f'THƯ-MỤC-CỦA-BẠN/TCB_historical_price_{start_date}_{end_date}.csv', index=True)
+```
+
+## 4.2. Xuất dữ liệu ra Google Sheets
+
+Phương thức này được thiết kế riêng để xuất dữ liệu trực tiếp từ Google Colab sang Google Sheets (sẽ không hoạt động nếu chạy ở môi trường local, không thiết lập môi trường tương đồng Colab). Tham khảo cách làm chi tiết trong file demo, mục `III. Data Export`
+
+
+# V. 🙋‍♂️ Thông tin liên hệ
 
 Bạn có thể kết nối với tác giả qua các hình thức sau. Trong trường hợp cần hỗ trợ nhanh, bạn có thể chọn nhắn tin qua Messenger hoặc Linkedin, tôi sẽ phản hồi ngay lập tức nếu có thể trong hầu hết các trường hợp.
 
 <div id="badges" align="center">
   <a href="https://www.linkedin.com/in/thinh-vu">
     <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
   </a>
@@ -756,35 +1033,37 @@
   </a>
   </a>
     <a href="https://github.com/thinh-vu">
     <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="Github Badge"/>
   </a>
 </div>
 
-# V. 💪 Hỗ trợ phát triển dự án vnstock
+# VI. 💪 Hỗ trợ phát triển dự án vnstock
 
 Nếu bạn nhận thấy giá trị từ vnstock và các dự án mã nguồn mở của tôi, bạn có thể hỗ trợ phát triển chúng bằng cách quyên góp hoặc đơn giản là gửi tặng tôi một ly cà phê để cảm ơn.
 Bạn có thể chọn 1 trong 3 hình thức đóng góp bao gồm Momo, Chuyển khoản ngân hàng và Gửi tiền qua Paypal. Sự đóng góp của bạn sẽ giúp tôi duy trì phí lưu trữ blog và tiếp tục tạo ra nội dung chất lượng cao. Cảm ơn sự ủng hộ của bạn!
 
 - [Paypal](https://paypal.me/thinhvuphoto?country.x=VN&locale.x=en_US)
+
 - ![momo-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/momo-qr-thinhvu.jpeg)
+  
 - ![vcb-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/vcb-qr-thinhvu.jpg)
 
-# VI. ⚖ Tuyên bố miễn trừ trách nhiệm
+# VII. ⚖ Tuyên bố miễn trừ trách nhiệm
 vnstock được phát triển nhằm mục đích cung cấp các công cụ nghiên cứu đơn giản và miễn phí, nhằm giúp người nghiên cứu tiếp cận và phân tích dữ liệu chứng khoán một cách dễ dàng. Dữ liệu được cung cấp phụ thuộc vào nguồn cấp dữ liệu, do đó, khi sử dụng, bạn cần thận trọng và cân nhắc.
 
 💰 Trong bất kỳ trường hợp nào, người sử dụng hoàn toàn chịu trách nhiệm về quyết định sử dụng dữ liệu trích xuất từ vnstock và chịu trách nhiệm với bất kỳ tổn thất nào có thể phát sinh. Bạn nên tự mình đảm bảo tính chính xác và đáng tin cậy của dữ liệu trước khi sử dụng chúng.
 
 Việc sử dụng dữ liệu chứng khoán và quyết định đầu tư là hoạt động có rủi ro và có thể gây mất mát tài sản. Bạn nên tìm kiếm lời khuyên từ các chuyên gia tài chính và tuân thủ các quy định pháp luật về chứng khoán tại Việt Nam và quốc tế khi tham gia vào hoạt động giao dịch chứng khoán.
 
 Xin lưu ý rằng vnstock không chịu trách nhiệm và không có bất kỳ trách nhiệm pháp lý nào đối với bất kỳ tổn thất hoặc thiệt hại nào phát sinh từ việc sử dụng gói phần mềm này.
 
 🐱‍👤 vnstock được thiết kế hoàn toàn cho mục đích phân tích và thực hành nghiên cứu đầu tư. Mọi hình thức sử dụng không đúng mục đích hoặc việc sử dụng trái phép thư viện với mục đích xấu như tấn công public API hay gây hại cho hệ thống thông qua từ chối truy cập hoặc các hành động tương tự, hoàn toàn nằm ngoài phạm vi sử dụng dự định và không thuộc trách nhiệm của nhóm phát triển.
 
-# VII. Bản quyền và giấy phép
+# VII. 🔑 Bản quyền và giấy phép
 
 
 ```
 Bản quyền (c) 2022 Thinh Vu | thinh-vu @ Github | MIT
 
 Được cấp phép theo quyền tự do, miễn phí, cho bất kỳ cá nhân nào nhận được một bản sao của phần mềm này và các tệp tài liệu liên quan (gọi chung là "Phần mềm"), để sử dụng Phần mềm mà không có bất kỳ hạn chế nào, bao gồm nhưng không giới hạn quyền sử dụng, sao chép, sửa đổi, hợp nhất, xuất bản, phân phối, cấp phép lại và/hoặc bán các bản sao của Phần mềm, và cho phép những người nhận Phần mềm được nhúng vào Phần mềm này, tuân thủ các điều kiện sau đây:
```

### Comparing `vnstock-0.1.8/setup.cfg` & `vnstock-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e73 746f 636b 0d0a 7665 7273   = vnstock..vers
-00000020: 696f 6e20 3d20 302e 312e 380d 0a61 7574  ion = 0.1.8..aut
+00000020: 696f 6e20 3d20 302e 312e 390d 0a61 7574  ion = 0.1.9..aut
 00000030: 686f 7220 3d20 5468 696e 6820 5675 0d0a  hor = Thinh Vu..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 206d  author_email = m
 00000050: 7274 6869 6e68 406c 6976 652e 636f 6d0d  rthinh@live.com.
 00000060: 0a64 6573 6372 6970 7469 6f6e 203d 2056  .description = V
 00000070: 6965 746e 616d 2053 746f 636b 204d 6172  ietnam Stock Mar
 00000080: 6b65 7420 4461 7461 0d0a 6c6f 6e67 5f64  ket Data..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `vnstock-0.1.8/vnstock/stock.py` & `vnstock-0.1.9/vnstock/stock.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # from .utils import *
 import pandas as pd
 import requests
 from pandas import json_normalize
 from io import BytesIO
 import time
 from datetime import datetime, timedelta
+import json
 
 # API request config for SSI API endpoints
 ssi_headers = {
         'Connection': 'keep-alive',
         'sec-ch-ua': '"Not A;Brand";v="99", "Chromium";v="98", "Google Chrome";v="98"',
         'DNT': '1',
         'sec-ch-ua-mobile': '?0',
@@ -70,14 +71,34 @@
   'Sec-Fetch-Site': 'same-site',
   'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36',
   'sec-ch-ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Google Chrome";v="114"',
   'sec-ch-ua-mobile': '?0',
   'sec-ch-ua-platform': '"Windows"'
 }
 
+# Rong Viet - Live Dragon
+rv_cookie = 'RV08835624=080035c91e77d96a1dcd7d9668d15032dca1c5c44e92ef5bbacedcc05701ff85c9486d38fb81e83857d5672616b9e3546504ee4846; _ga_KN4YPTLVCF=GS1.1.1690211515.1.0.1690211515.0.0.0; _gid=GA1.3.1634163694.1690211515; _gat_gtag_UA_120090926_1=1; _fbp=fb.2.1690211516077.1111198076; JSESSIONID=BFEB38A8B8419EEEC39DF45490E1B22D; vdsc-liv=\u00210CIhC2srW+VXY3rGJTT3LEhTmJvzwWLF5bKAMvgEjULUV+lBtkyTYFCLv7njgHRB4TgCdXik8NDWPQ==; hideMarketChartCKName=0; allCustomGroupsCkName=ALL_DEFAULT_GROUP_ID%23%23%23%23%23%23%23%23CTD%3BDHG%3BDRC%3BFPT%3BHPG%3BHSG%3BKDC%3BMWG%3BNT2%3BPAC%3BPC1%3BPNJ%3BTAC%3BVCB%3BVDS%3BVGC%3BVJC%3BVNM%3B%23%23%23%23%23%23%23%23T%C3%B9y%20ch%E1%BB%8Dn; rv_avraaaaaaaaaaaaaaaa_session_=DPHJFAEBJMBKENBPDOLDBOKIJCPLBLGFPHHGOCJEHFLMNGOGJINNIAOOIOPCNEILMDODFNCOCEGJIMDEHDNABIPKIJNKFFJCBEHPHADOFOLCEJEFFABNAAMIOLLMAEFI; _ga=GA1.1.1224611093.1690211515; _ga_D36ML1235R=GS1.1.1690211525.1.1.1690211543.0.0.0; RV9cd20160034=08557ab163ab2000054ec4478471ef19572f6aa45f46e6023a0505610ff398cf65052602d337f301084048ab69113000c7d3b36391060024abdc7de0506ec20cf57eadcbff388725325c25c6632a4cbda9a1e282112bd2a9d7d1e1c4471b850a'
+
+rv_headers = {
+  'Accept': 'application/json, text/javascript, */*; q=0.01',
+  'Accept-Language': 'en-US,en;q=0.9',
+  'Connection': 'keep-alive',
+  'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8',
+  'DNT': '1',
+  'Origin': 'https://livedragon.vdsc.com.vn',
+  'Sec-Fetch-Dest': 'empty',
+  'Sec-Fetch-Mode': 'cors',
+  'Sec-Fetch-Site': 'same-origin',
+  'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1788.0',
+  'X-Requested-With': 'XMLHttpRequest',
+  'sec-ch-ua': '"Edge";v="114", "Chromium";v="114", "Not=A?Brand";v="24"',
+  'sec-ch-ua-mobile': '?0',
+  'sec-ch-ua-platform': '"Windows"'
+}
+
 def api_request(url, headers=ssi_headers):
     r = requests.get(url, headers).json()
     return r
 
 ## STOCK LISTING
 def listing_companies (path='https://raw.githubusercontent.com/thinh-vu/vnstock/beta/data/listing_companies_enhanced-2023.csv'):
     """
@@ -102,23 +123,48 @@
             'noShareholders', 'foreignPercent', 'outstandingShare', 'issueShare',
             'establishedYear', 'noEmployees',  
             'stockRating', 'deltaInWeek', 'deltaInMonth', 'deltaInYear', 
             'shortName', 'industryEn', 'industryID', 'industryIDv2', 'website']]
     return df
 
 ## STOCK TRADING HISTORICAL DATA
-
 def stock_historical_data (symbol, start_date='2023-06-01', end_date='2023-06-17', resolution='1D', type='stock', headers=entrade_headers): # DNSE source (will be published on vnstock)
     """
     Get historical price data from entrade.com.vn. The unit price is VND.
     Parameters:
         symbol (str): ticker of a stock or index. Available indices are: VNINDEX, VN30, HNX, HNX30, UPCOM, VNXALLSHARE, VN30F1M, VN30F2M, VN30F1Q, VN30F2Q
         from_date (str): start date of the historical price data
         to_date (str): end date of the historical price data
         resolution (str): resolution of the historical price data. Default is '1D' (daily), other options are '1' (1 minute), 15 (15 minutes), 30 (30 minutes), '1H' (hourly)
+        type (str): stock, index, or derivative. Default is 'stock'
+        headers (dict): headers of the request
+    Returns:
+        :obj:`pandas.DataFrame`:
+        | time | open | high | low | close | volume |
+        | ----------- | ---- | ---- | --- | ----- | ------ |
+        | YYYY-mm-dd  | xxxx | xxxx | xxx | xxxxx | xxxxxx |
+    """
+    # if type is stock or index, call the function stock_ohlc
+    if type == 'stock' or type == 'index':
+        df = stock_ohlc(symbol, start_date, end_date, resolution, type, headers)
+    # if type is derivative, call the function derivatives_ohlc
+    elif type == 'derivative':
+        df = derivatives_ohlc(symbol, start_date, end_date, resolution, headers)
+    else:
+        raise ValueError('type must be stock, index or derivative')
+    return df
+
+def stock_ohlc (symbol, start_date='2023-06-01', end_date='2023-06-17', resolution='1D', type='stock', headers=entrade_headers): # DNSE source (will be published on vnstock)
+    """
+    Get historical price data from entrade.com.vn. The unit price is VND.
+    Parameters:
+        symbol (str): ticker of a stock or index. Available indices are: VNINDEX, VN30, HNX, HNX30, UPCOM, VNXALLSHARE, VN30F1M, VN30F2M, VN30F1Q, VN30F2Q
+        from_date (str): start date of the historical price data
+        to_date (str): end date of the historical price data
+        resolution (str): resolution of the historical price data. Default is '1D' (daily), other options are '1' (1 minute), 15 (15 minutes), 30 (30 minutes), '1H' (hourly)
         type (str): stock or index. Default is 'stock'
         headers (dict): headers of the request
     Returns:
         :obj:`pandas.DataFrame`:
         | time | open | high | low | close | volume |
         | ----------- | ---- | ---- | --- | ----- | ------ |
         | YYYY-mm-dd  | xxxx | xxxx | xxx | xxxxx | xxxxxx |
@@ -129,24 +175,60 @@
     from_timestamp = int(datetime.strptime(start_date, '%Y-%m-%d').timestamp())
     to_timestamp = int(datetime.strptime(end_date, '%Y-%m-%d').timestamp())
     url = f"https://services.entrade.com.vn/chart-api/v2/ohlcs/{type}?from={from_timestamp}&to={to_timestamp}&symbol={symbol}&resolution={resolution}"
     response = requests.request("GET", url, headers=headers).json()
     df = pd.DataFrame(response)
     df['t'] = pd.to_datetime(df['t'], unit='s') # convert timestamp to datetime
     df = df.rename(columns={'t': 'time', 'o': 'open', 'h': 'high', 'l': 'low', 'c': 'close', 'v': 'volume'}).drop(columns=['nextTime'])
+    # add symbol column
+    df['ticker'] = symbol
     df['time'] = df['time'].dt.tz_localize('UTC').dt.tz_convert('Asia/Ho_Chi_Minh')
     # if resolution is 1D, then convert time to date
     if resolution == '1D':
         df['time'] = df['time'].dt.date
     else:
         pass
     # convert open, high, low, close to VND
     df[['open', 'high', 'low', 'close']] = df[['open', 'high', 'low', 'close']] * 1000
     # convert open, high, low, close to int
     df[['open', 'high', 'low', 'close']] = df[['open', 'high', 'low', 'close']].astype(int)
+    # if resolution is 1D, then convert time to date
+    return df
+
+def derivatives_ohlc (symbol='VN30F1M', from_date='2023-04-01', to_date='2023-07-12', resolution='1D', headers=entrade_headers):
+    """
+    Get derivatives historical price from DNSE
+    Parameters:
+        symbol (str): derivative symbol
+        from_date (str): start date of the historical price data, format is 'YYYY-MM-DD'
+        to_date (str): end date of the historical price data, format is 'YYYY-MM-DD'
+        resolution (str): resolution of the historical price data. Default is '1D' (daily), other options are '1' (1 minute), 3 (3 minutes), 5 (5 minutes), 15 (15 minutes), 30 (30 minutes), 45 (45 minutes), '1H' (hourly), '2H' (2 hours), '4H' (4 hours), '1W' (weekly), '1M' (monthly)
+        headers (dict): headers of the request
+    """
+    # convert from_date, to_date to timestamp
+    from_timestamp = int(datetime.strptime(from_date, '%Y-%m-%d').timestamp())
+    to_timestamp = int(datetime.strptime(to_date, '%Y-%m-%d').timestamp())
+    # create url
+    url = f"https://services.entrade.com.vn/chart-api/v2/ohlcs/derivative?from={from_timestamp}&to={to_timestamp}&symbol={symbol}&resolution={resolution}"
+    # send request to get response
+    response = requests.request("GET", url, headers=headers).json()
+    df = pd.DataFrame(response)
+    # convert timestamp to datetime
+    df['t'] = pd.to_datetime(df['t'], unit='s')
+    # convert o, h, l, c to int
+    df[['o', 'h', 'l', 'c']] = df[['o', 'h', 'l', 'c']].astype(int)
+    # rename columns, t for time, o for open, h for high, l for low, c for close, v for volume and drop the nextTime column
+    df = df.rename(columns={'t': 'time', 'o': 'open', 'h': 'high', 'l': 'low', 'c': 'close', 'v': 'volume'}).drop(columns=['nextTime'])
+    # add symbol column
+    df['ticker'] = symbol
+    # convert time from utc to Asia/Ho_Chi_Minh timezone
+    df['time'] = df['time'].dt.tz_localize('UTC').dt.tz_convert('Asia/Ho_Chi_Minh')
+    # if resolution is 1D, convert time to date
+    if resolution == '1D':
+        df['time'] = df['time'].dt.date
     return df
 
 ## TRADING PRICE TABLE
 def price_depth (stock_list='VPB,TCB', headers=vps_headers):
     """
     This function returns the trading price board of a target stocks list.
     Args:
@@ -173,16 +255,19 @@
     # drop columns named from g1 to g6
     df.drop(columns=['id', 'mc', 'g1', 'g2', 'g3', 'g4', 'g5', 'g6'], inplace=True)
     # rearrange columns name by this order: Mã CP, Giá tham chiếu, Giá Trần, Giá Sàn, Giá mua 3, KL mua 3, Giá mua 2, KL mua 2, Giá mua 1, KL mua 1, Giá khớp lệnh, KL Khớp lệnh, +/- (Khớp lệnh), % (Khớp lệnh), Giá bán 1, KL bán 1, Giá bán 2, KL bán 2, Giá bán 3, KL bán 3, Tổng Khối Lượng, ĐTNN Mua, ĐTNN Bán
     df = df[['Mã CP', 'Giá tham chiếu', 'Giá Trần', 'Giá Sàn', 'Giá mua 3', 'KL mua 3', 'Giá mua 2', 'KL mua 2', 'Giá mua 1', 'KL mua 1', 'Giá khớp lệnh', 'KL Khớp lệnh', 'Giá bán 1', 'KL bán 1', 'Giá bán 2', 'KL bán 2', 'Giá bán 3', 'KL bán 3', 'Tổng Khối Lượng', 'ĐTNN Mua', 'ĐTNN Bán', 'ĐTNN Room']]
     # for all columns has "Giá" in the name, convert to value then multiply by 1000, set as integer
     for col in df.columns:
         if 'Giá' in col:
-            df[col] = df[col].astype(float)*1000
-            df[col] = df[col].astype(int)
+            try:
+                df[col] = df[col].astype(float)*1000
+                df[col] = df[col].astype(int)
+            except:
+                pass
     return df
 
 def price_board (symbol_ls):
     """
     This function returns the trading price board of a target stocks list.
     Args:
         symbol_ls (:obj:`str`, required): STRING list of symbols separated by "," without any space. Ex: "TCB,SSI,BID"
@@ -588,7 +673,161 @@
     Retrieve the latest indices values
     """
     url = "https://fiin-market.ssi.com.vn/MarketInDepth/GetLatestIndices?language=vi&pageSize=999999&status=1"
     payload={}
     response = requests.request("GET", url, headers=headers, data=payload)
     result = json_normalize(response.json()['items'])
     return result
+
+# -----------------------------------------------------------------
+# STOCK SCREENER
+
+def get_stock_screening (exchange='HOSE,HNX,UPCOM', epsGrowth1Year_min=0, epsGrowth1Year_max=1000000, lastQuarterProfitGrowth_min=0, lastQuarterProfitGrowth_max=10000000, roe_min=0, roe_max=10000, avgTradingValue20Day_min=10, avgTradingValue20Day_max=1000000000000, relativeStrength1Month_min=0, relativeStrength1Month_max=100, size=1700, headers=tcbs_headers):
+    """
+    Get stock screening insights from TCBS Stock Screener
+    Parameters:
+        exchange (str): exchange of the stock, default is 'HOSE,HNX,UPCOM'
+        epsGrowth1Year_min (int): minimum value of epsGrowth1Year, default is 0
+        epsGrowth1Year_max (int): maximum value of epsGrowth1Year, default is 1000000
+        lastQuarterProfitGrowth_min (int): minimum value of lastQuarterProfitGrowth, default is 0
+        lastQuarterProfitGrowth_max (int): maximum value of lastQuarterProfitGrowth, default is 10000000
+        roe_min (int): minimum value of roe, default is 0
+        roe_max (int): maximum value of roe, default is 10000
+        avgTradingValue20Day_min (int): minimum value of avgTradingValue20Day, default is 10
+        avgTradingValue20Day_max (int): maximum value of avgTradingValue20Day, default is 1000000000000
+        relativeStrength1Month_min (int): minimum value of relativeStrength1Month, default is 0
+        relativeStrength1Month_max (int): maximum value of relativeStrength1Month, default is 100
+        size (int): number of data points per page. Default is 30. You can increase this parameter to about 1700 to get all data in one trading day.
+        headers (dict): headers of the request. You can ignore this parameter.
+    """
+    url = "https://apipubaws.tcbs.com.vn/ligo/v1/watchlist/preview"
+    payload = json.dumps({
+        "tcbsID": None,
+        "filters": [
+            {
+                "key": "exchangeName",
+                "value": exchange,
+                "operator": "="
+            },
+            {
+                "key": "epsGrowth1Year",
+                "operator": ">=",
+                "value": epsGrowth1Year_min
+            },
+            {
+                "key": "epsGrowth1Year",
+                "operator": "<=",
+                "value": epsGrowth1Year_max
+            },
+            {
+                "key": "lastQuarterProfitGrowth",
+                "operator": ">=",
+                "value": lastQuarterProfitGrowth_min
+            },
+            {
+                "key": "lastQuarterProfitGrowth",
+                "operator": "<=",
+                "value": lastQuarterProfitGrowth_max
+            },
+            {
+                "key": "roe",
+                "operator": ">=",
+                "value": roe_min
+            },
+            {
+                "key": "roe",
+                "operator": "<=",
+                "value": roe_max
+            },
+            {
+                "key": "avgTradingValue20Day",
+                "operator": ">=",
+                "value": avgTradingValue20Day_min
+            },
+            {
+                "key": "avgTradingValue20Day",
+                "operator": "<=",
+                "value": avgTradingValue20Day_max
+            },
+            {
+                "key": "relativeStrength1Month",
+                "operator": ">=",
+                "value": relativeStrength1Month_min
+            },
+            {
+                "key": "relativeStrength1Month",
+                "operator": "<=",
+                "value": relativeStrength1Month_max
+            }
+        ],
+        "size": size
+    })
+    # send request to get response
+    response = requests.request("POST", url, headers=headers, data=payload).json()
+    df = pd.DataFrame(response['searchData']['pageContent'])
+    return df
+
+
+# -----------------------------------------------------------------
+# DERIVATIVES
+
+# A function to get derivatives data from livedragon
+def derivatives_historical_match (symbol='VN30F2308', date='2023-07-24', cookie=rv_cookie, headers=rv_headers):
+    """
+    Get derivatives historical price data from Live Dragon website (CK Rong Viet)
+    Parameters:
+        symbol (str, required): ticker of the stock
+        date (str, required): date of the historical price data
+        cookie (str, required): cookie of the request. Visit https://livedragon.vdsc.com.vn/all/all.rv. Open Developer Tools (F12 or Ctrl + Shift + I or Cmd + Option + I on macOS) > Navigate to Network > Choose Fetch/XHR > Select any request > Find Cookie in Header > Copy value.
+        headers (dict): headers of the request. You can ignore this parameter.
+    """
+    # add cookie to headers
+    headers['Cookie'] = cookie
+    url = "https://livedragon.vdsc.com.vn/general/intradaySearch.rv"
+    # convert date to dd/mm/yyyy format
+    date = datetime.strptime(date, '%Y-%m-%d').strftime('%d/%m/%Y')
+    payload = f"stockCode={symbol}&boardDate={date}"
+    response = requests.request("POST", url, headers=headers, data=payload).json()
+    df = pd.DataFrame(response['list'])
+    # move `Code` column to the first column
+    df = df[['Code'] + [col for col in df.columns if col != 'Code']]
+    return df
+
+
+# DATA EXPORT
+
+# # Import required modules
+# from google.colab import auth
+# auth.authenticate_user()
+# import gspread
+# from google.auth import default
+# from gspread_dataframe import set_with_dataframe
+
+# # A function to export data to Google Sheets, support either with a whole sheet or a specific range
+# def export_to_sheets (dataframe, sheet_file='vnstock_data_export', sheet_name=None, target_range=None, max_rows=1000, max_cols=30):
+#     """
+#     Export dataframe to Google Sheets
+#     Parameters:
+#         dataframe (pandas.DataFrame): Dataframe to export
+#         sheet_file (str): Name of the Google Sheets file to export to
+#         sheet_name (str): Name of the sheet to export to
+#         target_range (str): Range to export to, e.g. 'A1:B2'
+#         max_rows (int): Maximum number of rows to create the Google Sheets file.
+#         max_cols (int): Maximum number of columns to create the Google Sheets file.
+#     """
+#     # If sheet_name is not specified, use the default sheet name
+#     creds, _ = default()
+#     gc = gspread.authorize(creds)
+#     sh = gc.create(sheet_file)
+#     if sheet_name is None:
+#         worksheet = gc.open(sheet_file).sheet1
+#     else:
+#         worksheet = sh.add_worksheet(title=sheet_name, rows=max_rows, cols=max_cols)
+#     # If range is not specified, export the whole dataframe, else export the dataframe to the specified range
+#     if range is None:
+#         set_with_dataframe(worksheet, dataframe, include_index=False, include_column_header=True, resize=True)
+#     else:
+#         cell_list = worksheet.range(target_range)
+#         for cell, value in zip(cell_list, df.values.flatten()):
+#             cell.value = value
+#         worksheet.update_cells(cell_list)
+#     print('Exported to Google Sheets successfully!')
```

### Comparing `vnstock-0.1.8/vnstock/utils.py` & `vnstock-0.1.9/vnstock/utils.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.1.8/vnstock.egg-info/PKG-INFO` & `vnstock-0.1.9/vnstock.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock
-Version: 0.1.8
+Version: 0.1.9
 Summary: Vietnam Stock Market Data
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: mrthinh@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,22 +20,25 @@
 </div>
 
 ---
 
 🌐 View in **[English](https://github.com/thinh-vu/vnstock/blob/main/README-en.md)**
 
 MỤC LỤC
+
 - [I. 🎤 Giới thiệu](#i--giới-thiệu)
-- [II. 📚 Hướng dẫn sử dụng cho người mới](#ii-hướng-dẫn-sử-dụng-cho-người-mới)
+- [II. 📚 Hướng dẫn sử dụng cho người mới](#ii--hướng-dẫn-sử-dụng-cho-người-mới)
 - [III. 💻 Cách sử dụng các hàm trong vnstock](#iii--cách-sử-dụng-các-hàm-trong-vnstock)
-- [IV. 🙋‍♂️ Contact Information](#iv-️-contact-information)
-- [V. 💪 Hỗ trợ phát triển dự án vnstock](#v--hỗ-trợ-phát-triển-dự-án-vnstock)
-- [VI. ⚖ Tuyên bố miễn trừ trách nhiệm](#vi--tuyên-bố-miễn-trừ-trách-nhiệm)
+- [IV. Xuất, Lưu trữ, Chia sẻ dữ liệu](#iv-xuất-lưu-trữ-chia-sẻ-dữ-liệu)
+- [V. 🙋‍♂️ Thông tin liên hệ](#v-️-thông-tin-liên-hệ)
+- [VI. 💪 Hỗ trợ phát triển dự án vnstock](#vi--hỗ-trợ-phát-triển-dự-án-vnstock)
+- [VII. ⚖ Tuyên bố miễn trừ trách nhiệm](#vii--tuyên-bố-miễn-trừ-trách-nhiệm)
 - [VII. Bản quyền và giấy phép](#vii-bản-quyền-và-giấy-phép)
 
+
 # I. 🎤 Giới thiệu
 ## 1.1. Giới thiệu chung
 vnstock là thư viện Python được thiết kế để tải dữ liệu chứng khoán Việt Nam một cách dễ dàng và miễn phí. vnstock sử dụng các nguồn cấp dữ liệu đáng tin cậy, bao gồm nhưng không giới hạn từ công ty chứng khoán và công ty phân tích thị trường tại Việt Nam. Gói thư viện được thiết kế dựa trên nguyên tắc về sự đơn giản và mã nguồn mở, hầu hết các hàm được viết dựa trên thư viện request và pandas có sẵn trên môi trường Google Colab do đó người dùng không cần cài đặt thêm các gói thư viện kèm theo.
 
 ## 1.2. Tính năng chính
 vnstock cung cấp nhiều tính năng đa dạng như tải dữ liệu lịch sử giá, thông tin công ty niêm yết, thông tin thị trường cho tất cả các mã chứng khoán niêm yết.
 
@@ -44,20 +47,41 @@
 
 ## 1.4. Tips
 - Theo dõi những cập nhật về thay đổi của vnstock bằng tính năng `Watch`. Hiện tại vnstock được cập nhật thường xuyên hàng tuần qua nhánh `beta`, vì vậy theo dõi repo này giúp bạn luôn nắm bắt được kịp thời những thay đổi mới nhất.
 - Đánh dấu yêu thích repo `vnstock` bằng tính năng `Star`. Đây cũng là cách giúp vnstock có thể tiếp cận tới nhiều người quan tâm hơn.
 
 <details>
   <summary> Minh họa tính năng Watch và Star </summary>
+  
 ![watch-star](https://github.com/thinh-vu/vnstock/blob/beta/src/vnstock-watch-and-star.png?raw=true)
 
 </details>
 
 ## 1.5. Đóng góp xây dựng mã nguồn vnstock
-- Bạn có thể đóng góp xây dựng vnstock thông qua nhiều hình thức khác nhau, trong đó có việc xây dựng và cải tiến mã nguồn hoặc dịch tài liệu của dự án. Để bắt đầu, bạn có thể `folk` repo này về tài khoản của mình, sửa đổi mã nguồn và tạo `pull request` để yêu cầu cập nhật mã nguồn. Sau khi kiểm tra các thay đổi và phê duyệt, mã nguồn do bạn đóng góp sẽ được gộp vào vnstock.
+- Bạn có thể đóng góp xây dựng vnstock thông qua nhiều hình thức khác nhau, trong đó có việc xây dựng và cải tiến mã nguồn hoặc dịch tài liệu của dự án. 
+- Để bắt đầu, bạn có thể `folk` nhánh `beta` của repo này về tài khoản của mình, sửa đổi mã nguồn và tạo `pull request` để yêu cầu cập nhật mã nguồn. Sau khi kiểm tra các thay đổi và phê duyệt, mã nguồn do bạn đóng góp sẽ được gộp vào vnstock.
+- Lưu ý: Những thay đổi do bạn đóng góp sẽ được phát hành trong phiên bản tiếp theo của `vnstock` trên Pypi.org đồng thời với những cập nhật của tác giả trên nhánh `beta`.
+
+## 1.6. Hoàn thành khảo sát về vnstock
+> vnstock là một dự án tôi tâm huyết, đầu tư nhiều thời gian để phát triển giúp bản thân và cộng đồng tiếp cận nguồn dữ liệu chứng khoán miễn phí và đáng tin cậy.
+
+Hoàn thành bản khảo sát: [Tại đây](https://forms.gle/zaJnbgUCjjL1GoTF6)
+Để đảm bảo rằng vnstock phát triển theo hướng đáp ứng nhu cầu của bạn, tôi rất mong nhận được phản hồi từ bạn. Bạn là người dùng quan trọng của vnstock và ý kiến của bạn sẽ giúp chúng tôi xây dựng một kế hoạch phát triển vnstock một cách toàn diện.
+
+## 1.7. Dịch vụ "code dạo", gây quỹ phát triển dự án
+
+Ngoài ra, để gây quỹ phát triển dự án, tôi cũng cung cấp dịch vụ "code dạo" theo đặt hàng bao gồm nhưng không giới hạn với các hoạt động dưới đây:
+- Tải dữ liệu thị trường
+- Viết workflow quét dữ liệu, cập nhật cơ sở dữ liệu, vv
+- Thiết lập dự án phân tích chứng khoán toàn diện
+- Tạo bộ lọc cổ phiếu độc quyền
+- Tạo robot giao dịch qua API
+- Cung cấp API dữ liệu độc quyền
+
+Nếu bạn nào quan tâm và có nhu cầu, vui lòng [inbox](https://www.messenger.com/t/mr.thinh.ueh) để trao đổi thêm. Hoạt động này cũng giúp tôi hiểu thêm về những ứng dụng thực tế và phát triển vnstock trong tương lai.
 
 # II. 📚 Hướng dẫn sử dụng cho người mới
 ## 2.1. Tài nguyên quan trọng
 
 ### 2.1.2 Blog
 
 👉 Để biết thêm thông tin và minh hoạ về cách sử dụng, bạn vui lòng truy cập bài viết trên blog của tôi, có sẵn bằng tiếng Việt/Anh [tại đây](https://thinhvu.com/2022/09/22/vnstock-api-tai-du-lieu-chung-khoan-python?utm_source=github&utm_medium=vnstock).
@@ -86,14 +110,17 @@
 
 </details>
 
 ### 2.1.4. Xây dựng cộng đồng vnstock
 
 🖐 Nếu bạn thấy thư viện này có giá trị và muốn hỗ trợ tác giả duy trì vnstock dưới dạng mã nguồn mở, miễn phí thì có thể tham gia ủng hộ gây quỹ phát triển dự án này. Để biết thêm chi tiết, vui lòng tham khảo bài viết trên blog sau: [Cùng nhau xây dựng cộng đồng VNStock vững mạnh](https://thinhvu.com/2023/04/15/xay-dung-cong-dong-vnstock-vung-manh/).
 
+- Tham gia nhóm vnstock trên Facebook: [Tại đây](https://www.facebook.com/groups/vnstock)
+- Tham gia Discord channel: [Tại đây](https://discord.gg/qJvxJcChJ3)
+
 <details>
   <summary>Ủng hộ quỹ phát triển vnstock</summary>
   Nếu vnstock giúp ích cho bạn, hãy đóng góp quỹ phát triển ứng dụng này theo một trong hai hình thức sau gồm chuyển khoản ngân hàng hoặc Momo. Mọi khoản đóng góp đều đáng trân quý và là động lực giúp tác giả duy trì vnstock luôn hữu ích, miễn phí, và dễ tiếp cận cho cộng đồng.
 
   - ![vcb-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/vcb-qr-thinhvu.jpg)
   - ![momo-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/momo-qr-thinhvu.jpeg)
 
@@ -143,15 +170,17 @@
 
 Để nạp các hàm của vnstock vào dự án Python của bạn, cần `import` chúng thông qua câu lệnh như dưới đây. Như vậy mọi thứ đã sẵn sàng để truy cập dữ liệu do vnstock cung cấp thông qua các hàm được liệt kê trong tài liệu hướng dẫn.
 
 ```python
 from vnstock import *
 ```
 
-## 3.1 📰 Danh sách các công ty niêm yết
+## 3.1. ☑ Danh sách cổ phiếu niêm yết (Listing)
+
+### 3.1.1. 📰 Danh sách các công ty niêm yết
 ```python
 listing_companies()
 ```
 Hàm này đọc dữ liệu từ tệp csv đính kèm trên Github theo mặc định (trong thư mục /data của repo này). Bởi danh sách các công ty niêm yết thường không thay đổi liên tục nên việc này không gây trở ngại nhiều.
 
 <details>
   <summary>Output</summary>
@@ -162,15 +191,18 @@
 0    VVS   UpcomIndex  Công ty Cổ phần Đầu tư Phát triển Máy Việt Nam  Đầu tư Phát triển Máy Việt Nam            DN          CT  ...  False  False  False  False  False  False
 1    XDC   UpcomIndex   Công ty TNHH MTV Xây dựng Công trình Tân Cảng    Xây dựng Công trình Tân Cảng            DN          CT  ...  False  False  False  False  False  False
 2    HSV   UpcomIndex           Công ty Cổ phần Tập đoàn HSV Việt Nam                Gang Thép Hà Nội            DN          CT  ...  False  False  False  False  False  False
 ```
 
 </details>
 
-## 3.2. Tổng quan về công ty
+## 3.2. 🏳 Phân tích cơ bản (Fundamental Analysis)
+
+### 3.2.1. 🏚 Thông tin tổng quan công ty
+
 ```python
 company_overview('TCB')
 ```
 
 <details>
   <summary>Output</summary>
 
@@ -178,29 +210,168 @@
   >>> company_overview('TCB')
     exchange    shortName  industryID industryIDv2   industry  ... deltaInMonth deltaInYear  outstandingShare  issueShare  ticker
   0     HOSE  Techcombank         289         8355  Ngân hàng  ...       -0.027      -0.038            3510.9      3510.9     TCB
   ```
 
 </details>
 
-## 3.3. 📈 Truy xuất dữ liệu giá lịch sử
+### 3.2.2. 🧧 Lịch sử chi trả cổ tức
+
+```python
+dividend_history("VNM")
+```
+
+<details>
+  <summary>Output</summary>
+
+```
+   exerciseDate  cashYear  cashDividendPercentage issueMethod
+0      10/01/22      2021                    0.14        cash
+1      07/09/21      2021                    0.15        cash
+2      07/06/21      2020                    0.11        cash
+3      05/01/21      2020                    0.10        cash
+```
+</details>
+
+## 3.3. 💰 Phân tích tài chính (Financial Analysis)
+
+### 3.3.1. Bộ chỉ số tài chính
+```python
+financial_ratio(symbol="TCB", report_range='yearly', is_all=False)
+```
+Trong đó:
+- `report_range` nhận 1 trong 2 giá trị: `yearly` cho phép trả về chỉ số theo năm, `quarterly` trả về dữ liệu theo quý
+- `is_all` có giá trị mặc định là `True` cho phép lấy chỉ số qua tất cả các kỳ (năm hoặc quý), `False` cho phép lấy các kỳ gần nhất (5 năm hoặc 10 quý gần đây).
+
+<details>
+  <summary>Output</summary>
+
+  ```
+>>> financial_ratio('TCB', 'yearly')
+year                      2022   2021   2020   2019   2018
+ticker                     TCB    TCB    TCB    TCB    TCB
+priceToEarning             4.5    9.7    9.0    8.2   10.7
+priceToBook                0.8    1.9    1.5    1.3    1.8
+roe                      0.197  0.217  0.181  0.178  0.215
+roa                      0.032  0.036   0.03  0.029  0.029
+earningPerShare           5729   5132   3504   2869   2410
+bookValuePerShare        32248  26452  21214  17679  14749
+interestMargin           0.053  0.057  0.049  0.043  0.041
+nonInterestOnToi         0.259   0.28  0.307  0.323  0.379
+badDebtPercentage        0.007  0.007  0.005  0.013  0.018
+provisionOnBadDebt       1.573  1.629   1.71  0.948  0.851
+costOfFinancing          0.028  0.022  0.031  0.038  0.041
+equityOnTotalAsset       0.162  0.164   0.17  0.162  0.161
+equityOnLoan              0.27  0.268  0.269  0.269  0.324
+costToIncome             0.328  0.301  0.319  0.347  0.318
+equityOnLiability          0.2    0.2    0.2    0.2    0.2
+epsChange                0.116  0.465  0.221  0.191  0.313
+assetOnEquity              6.2    6.1    5.9    6.2    6.2
+preProvisionOnToi        0.537  0.554  0.542   0.52  0.542
+postTaxOnToi               0.5  0.497  0.465  0.485  0.462
+loanOnEarnAsset          0.684  0.665  0.681  0.649  0.537
+loanOnAsset              0.602  0.611  0.631  0.602  0.498
+loanOnDeposit            1.173  1.104    1.0  0.998  0.794
+depositOnEarnAsset       0.583  0.603   0.68  0.651  0.676
+badDebtOnAsset           0.004  0.004  0.003  0.008  0.009
+liquidityOnLiability     0.347  0.382  0.372  0.411  0.531
+payableOnEquity            5.2    5.1    4.9    5.2    5.2
+cancelDebt               0.002  0.004  0.013  0.002  0.008
+bookValuePerShareChange  0.219  0.247    0.2  0.199  0.923
+creditGrowth             0.211  0.252  0.202  0.443 -0.006
+  ```
+</details>
+
+
+### 3.3.2. 💵 Báo cáo kết quả kinh doanh, cân đối kế toán và lưu chuyển tiền tệ
+
+#### 3.3.2.1. 📄 Báo cáo kinh doanh
+
+![income_statement](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_income_statement.png)
+```python
+financial_flow(symbol="TCB", report_type='incomestatement', report_range='quarterly')
+```
+
+
+<details>
+  <summary>Output</summary>
+
+```
+        ticker  revenue  yearRevenueGrowth  quarterRevenueGrowth costOfGoodSold grossProfit  ...  investProfit  serviceProfit  otherProfit  provisionExpense operationIncome  ebitda
+index                                                                                        ...
+2021-Q4    TCB     7245              0.328                 0.074           None        None  ...           279           2103          532              -627            6767    None
+2021-Q3    TCB     6742              0.310                 0.023           None        None  ...           384           1497          156              -589            6151    None
+2021-Q2    TCB     6588              0.674                 0.076           None        None  ...           717           1457          444              -598            6615    None
+2021-Q1    TCB     6124              0.454                 0.122           None        None  ...           812           1325          671              -851            6369    None
+```
+</details>
+
+#### 3.3.2.2. 🧾 Bảng cân đối kế toán
+
+![balance_sheet](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_balancesheet.png)
+```python
+financial_flow(symbol="TCB", report_type='balancesheet', report_range='quarterly')
+```
+
+<details>
+  <summary>Output</summary>
+
+```
+        ticker shortAsset  cash shortInvest shortReceivable inventory longAsset  fixedAsset  ...  payableInterest  receivableInterest deposit otherDebt  fund  unDistributedIncome  minorShareHolderProfit  payable
+index                                                                                        ...
+
+2021-Q4    TCB       None  3579        None            None      None      None        7224  ...             3098                5808  314753     33680  9156                47469                     845   475756
+2021-Q3    TCB       None  3303        None            None      None      None        7106  ...             3074                6224  316376     34003  6784                45261                     753   453251
+2021-Q2    TCB       None  3554        None            None      None      None        6739  ...             2643                5736  289335     27678  6790                40924                     659   420403
+2021-Q1    TCB       None  4273        None            None      None      None        4726  ...             2897                5664  287446     26035  6790                36213                     563   3837
+```
+</details>
+
+#### 3.3.2.3. 💶 Báo cáo lưu chuyển tiền tệ
 
-> Phiên bản API hiện tại cho phép truy cập giá lịch sử tối đa đến ngày 2012-03-20 đối với tất cả mã cổ phiếu. Nếu bạn có nhu cầu lấy lịch sử giá từ thời điểm thị trường chứng khoán bắt đầu hoạt động (REE là mã cổ phiếu có giao dịch sớm nhất thị trường vào 2000-07-31), hãy là một thành viên của [ vnstock membership](https://www.facebook.com/groups/vnstock) để được hỗ trợ.
+```python
+financial_flow(symbol="TCB", report_type='cashflow', report_range='quarterly')
+```
 
-vnstock cho phép người dùng **tải xuống dữ liệu lịch sử giao dịch cổ phiếu** với theo 5 mức độ chi tiết theo khoảng thời gian bao gồm: 1 phút, 15 phút, 30 phút, 1 giờ, 1 ngày. Trong ví dụ dưới đây, dữ liệu giá được truy xuất theo cấp độ ngày. Đơn vị giá mặc định là VND.
+<details>
+  <summary>Output</summary>
+
+```
+        ticker  investCost  fromInvest  fromFinancial  fromSale  freeCashFlow
+index
+2021-Q4    TCB        -280        -276              0     -9328             0
+2021-Q3    TCB        -180        -179             60     17974             0
+2021-Q2    TCB        -337        -282              0     11205             0
+2021-Q1    TCB        -143        -143              0     -6954             0
+```
+</details>
+
+## 3.4. Phân tích kỹ thuật (Technical Analysis)
+
+### 3.4.1 📈 Truy xuất dữ liệu giá lịch sử
+
+> Phiên bản API hiện tại cho phép truy cập giá lịch sử tối đa đến ngày 2012-03-20 đối với tất cả mã cổ phiếu. Nếu bạn có nhu cầu lấy lịch sử giá từ thời điểm thị trường chứng khoán bắt đầu hoạt động (REE là mã cổ phiếu có giao dịch sớm nhất thị trường vào 2000-07-31), hãy là một thành viên của [vnstock membership](https://www.facebook.com/groups/vnstock) để được hỗ trợ.
+
+vnstock cho phép người dùng tải xuống dữ liệu lịch sử giao dịch của `mã cổ phiếu, chỉ số, hợp đồng phái sinh`.
+- Dữ liệu `cổ phiếu` và `chỉ số` hỗ trợ 5 mức độ chi tiết theo khoảng thời gian bao gồm: 1 phút, 15 phút, 30 phút, 1 giờ, 1 ngày. 
+- Dữ liệu `phái sinh` hỗ trợ 8 mức độ chi tiết theo khoảng thời gian bao gồm: 1 phút, 3 phút, 5 phút, 15 phút, 30 phút, 45 phút, 1 giờ, 1 ngày
+- Trường dữ liệu `time` sẽ là giá trị ngày tháng `YYYY-mm-dd` nếu `resolution` nhập vào là `1D`, trong khi `resolution` là cấp độ phút và giờ sẽ cho thêm thông tin thời gian giờ/phút.
+- Đơn vị giá OHLC được làm tròn, chỉ lấy phần nguyên. Đơn vị tính là VND.
+
+Trong ví dụ dưới đây, dữ liệu giá được truy xuất theo cấp độ ngày.
 
 ```python
 df =  stock_historical_data(symbol='GMD', 
                             start_date="2021-01-01", 
                             end_date='2022-02-25', resolution='1D', type='stock')
 print(df)
 ```
 - Mới: 
-  - Giá trị mà tham số `resolution` có thể nhận là `1D` (mặc định, 1 ngày), '1' (1 phút), 15 (15 phút), 30 (30 phút), '1H' (hàng giờ).
-  - `type = 'stock'` cho phép lấy dữ liệu giá của mã cổ cổ phiếu, `type = 'index'` cho phép lấy dữ liệu giá của mã chỉ số. Các mã chỉ số hỗ trợ bao gồm: VNINDEX, VN30, HNX, HNX30, UPCOM, VNXALLSHARE, VN30F1M, VN30F2M, VN30F1Q, VN30F2Q
+  - Giá trị mà tham số `resolution` có thể nhận là `1D` (mặc định, 1 ngày), '1' (1 phút), 3 (3 phút), 5 (5 phút), 15 (15 phút), 30 (30 phút), 45 (45 phút), '1H' (hàng giờ).
+  - `type = 'stock'` cho phép lấy dữ liệu giá của mã cổ cổ phiếu, `type = 'index'` cho phép lấy dữ liệu giá của mã chỉ số, và `type='derivative` cho phép lấy dữ liệu phái sinh. Các mã được hỗ trợ bao gồm (nhưng không giới hạn): VNINDEX, VN30, HNX, HNX30, UPCOM, VNXALLSHARE, VN30F1M, VN30F2M, VN30F1Q, VN30F2Q
 
 Bạn cũng có thể viết hàm theo dạng rút gọn như dưới đây, điều này đúng với tất cả các hàm, miễn là thông số được nhập vào đúng thứ tự:
 
   - Lấy dữ liệu lịch sử cổ phiếu
   ```python
   df = stock_historical_data("GMD", "2021-01-01", "2022-02-25", "1D", 'stock')
   print(df)
@@ -221,26 +392,38 @@
 
 - Lấy dữ liệu lịch sử của mã chỉ số
 ```python
 df = stock_historical_data("VNINDEX", "2021-01-01", "2022-02-25", "1D", 'index')
 print(df)
 ```
 
-## 3.4. 📊 Bảng giá
+- Lấy dữ liệu lịch sử của hợp đồng phái sinh
+```python
+df = stock_historical_data("VN30F1M", "2023-07-01", "2023-07-24", "1D", 'derivative')
+print(df)
+```
+
+## 3.5. Lựa chọn cổ phiếu (Stock Screening)
+
+### 3.5.1. So sánh các cổ phiếu tiềm năng
+
+#### 3.5.1.1. 📊 Bảng giá (Price board)
 
 Bạn có thể tải xuống bảng giá của một danh sách các cổ phiếu được chọn để phân tích, thiết lập thuật toán dễ dàng hơn (khi xuất ra Google Sheets/Excel) so với việc xem trực tiếp trên bảng giá của các công ty chứng khoán.
 
 <details>
-  <summary>Bảng giá</summary>
+  <summary>Minh họa Bảng giá TCBS</summary>
 
   ![price_board](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_trading_board_sector.png)
 
 </details>
 
-### 3.4.1. Thông tin bước giá, khối lượng và khớp lệnh
+
+##### a. Thông tin bước giá, khối lượng và khớp lệnh
+
 ```python
 price_depth('TCB,SSI,VND')
 ```
 Sử dụng hàm này cho phép thống kê các bước giá và khối lượng trên bảng giá của một hoặc một danh sách các mã cổ phiếu. Bạn có thể sử dụng kết hợp hàm này với hàm `price_board` để kết hợp các thông tin đa dạng về giá, khối lượng, chỉ số, thông tin giao dịch để chọn lọc và theo dõi cổ phiếu theo mục đích sử dụng của mình.
 
 <details>
   <summary>Output</summary>
@@ -251,15 +434,16 @@
 1   SSI           28400     30350    26450      28450      100      28400     9850      28350  ...    30640      28550     22730      28600    48410          1610280   142759     17353  803963854     
 2   VND           17950     19200    16700      18450    11620      18400    38790      18350  ...    73180      18550     87830      18600   223700          4360710   152966      8355  932083910     
 
 [3 rows x 22 columns]
 
 </details>
 
-### 3.4.2. Thông tin giao dịch bổ sung và các chỉ số
+
+##### b. Thông tin giao dịch bổ sung và các chỉ số
 
 ```
 price_board('TCB,SSI,VND')
 ```
 Hàm này cho phép tải về thông tin giá, khối lượng và các chỉ số quan trọng cho một hoặc một danh sách mã cổ phiếu. Sử dụng kết hợp với hàm `price_depth` cho hiệu quả tốt nhất.
 
 <details>
@@ -270,114 +454,17 @@
   Mã CP  Giá Khớp Lệnh  KLBD/TB5D  T.độ GD  KLGD ròng(CM)  ...  vnid1m  vnid3m  vnid1y  vnipe    vnipb
 0   TCB        48600.0        0.6     0.49         -23200  ...    -3.7    -2.0    22.4  17.99  2.46159
 1   SSI        43300.0        0.5     0.50        -112200  ...    -3.7    -2.0    22.4  17.99  2.46159
 2   VND        32600.0        0.7     0.68          37300  ...    -3.7    -2.0    22.4  17.99  2.46159
 ```
 </details>
 
-## 3.5. 🔥 Dữ liệu khớp lệnh trong ngày giao dịch
-
-<details>
-  <summary>Minh hoạ giao diện TCBS</summary>
-
-  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen1.png)
-  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen2.png)
-
-</details>
-vnstock cho phép người dùng tải xuống dữ liệu khớp lệnh trong ngày giao dịch theo thời gian thực. Nếu mốc thời gian bạn truy cứu rơi vào Thứ Bảy, Chủ Nhật thì dữ liệu nhận được thể hiện cho ngày giao dịch của Thứ 6 của tuần đó.
-
-```python
-df =  stock_intraday_data(symbol='TCB', 
-                            page_size=500)
-print(df)
-```
-
-<details>
-  <summary>Terminal output</summary>
-
-  ```{r, engine='python', count_lines}
->>> stock_intraday_data('TCB', 500)
-
-  ticker      time  orderType investorType  volume  averagePrice  orderCount
-0    TCB  14:29:55  Sell Down        SHEEP    1000       32700.0           1
-1    TCB  14:29:47     Buy Up        SHEEP     200       32750.0           1
-2    TCB  14:29:44  Sell Down         WOLF    8000       32700.0          14
-3    TCB  14:29:41  Sell Down        SHEEP    1000       32700.0           5
-4    TCB  14:29:36  Sell Down         WOLF   23800       32700.0          10
-  ```
-
-</details>
-
-<details>
-  <summary>Giải thích ý nghĩa chỉ số</summary>
-  • Khi 1 lệnh lớn (từ Cá mập, tay to, tổ chức....) mua chủ động (hoặc bán chủ động) được đưa vào Sàn, thường thì nó sẽ được khớp với nhiều lệnh nhỏ đang chờ bán (hoặc chờ mua). Nếu chỉ nhìn realtime theo từng lệnh khớp riêng lẻ, thì sẽ không thể phát hiện được các lệnh to (của Cá mập, tay to...) vừa được đẩy vào Sàn. Vì vậy, chúng tôi "cộng dồn" các lệnh khớp này lại (phát sinh bởi 1 lệnh lớn chủ động vào sàn trong 1 khoảng thời gian rất nhanh) để giúp NĐT phát hiện các lệnh lớn (của Cá mập, tay to....) chính xác hơn. Lệnh Cá mập sẽ được tô xanh (cho Mua chủ động) và đỏ (cho Bán chủ động). 
 
-  • Cá mập: (CM - SHARK) nhà đầu tư tay to, tổ chức, đầu tư lớn, dẫn dắt thị trường. Giá trị 1 lệnh đặt > 1 tỷ đồng/lệnh đặt. Đồ thị 1N dùng số liệu 1 phút cho 60’ gần nhất; 1W là tổng mỗi 15’ cho 1 tuần; 1M là tổng hàng ngày cho 1 tháng
-
-  • Sói già: (SG - WOLF) nhà đầu tư kinh nghiệm, giá trị lệnh đặt cao. Giá trị 1 lệnh đặt từ 200 tr đến 1 tỷ đồng/lệnh đặt.
-
-  • Cừu non: (CN - SHEEP) nhà đầu tư nhỏ lẻ, giá trị giao dịch và mua bán chủ động thấp. Giá trị 1 lệnh đặt Mua hoặc Bán chủ động < 200 triệu đồng/lệnh đặt vào.
-
-  • Mua chủ động (hay Buy Up) là khi NĐT thực hiện chủ động mua lên qua việc đặt lệnh mua với giá bằng giá dư bán gần nhất để có thể khớp luôn. Như thế, giá khớp cho lệnh này thường sẽ đẩy giá khớp lên cao hơn thị giá trước đó.
-
-  • Bán chủ động (hay Sell Down) là khi NĐT thực hiện chủ động Bán dưới giá hiện tại (hay thị giá) của cổ phiếu bằng việc đặt lệnh bán với giá bán bằng giá dư mua gần nhất để khớp ngay. Và như thế, thị giá sẽ bị kéo xuống thấp hơn so với thị giá trước đó. Thống kê khối lượng giao dich theo Mua CĐ và Bán CĐ dùng để đánh giá tương quan giữa cung (Bán CĐ) và cầu (Mua CĐ) trên giao dịch khớp lệnh thực tế, nhằm nhận định tương đối về sự vận động của xu hướng dòng tiền. Khi tỷ lệ % Mua CĐ trên (Tổng Mua và Bán CĐ) lớn hơn 50%, đồng nghĩa với việc thị trường đang có xu hướng mua vào nhiều hơn bán ra và ngược lại, qua đó xác định được dòng tiền vào/ra với mỗi cổ phiếu. Khi tỷ lệ này cao đột biến (>70% hay <30%) so với điểm cân bằng (50%) , đó là tín hiệu của việc mua hoặc bán bất chấp của thị trường.
-
-</details>
-
-## 3.6. 💰 Các chỉ số tài chính
-
-### 3.6.1. Bộ chỉ số tài chính của một mã cổ phiếu
-```python
-financial_ratio(symbol="TCB", report_range='yearly', is_all=False)
-```
-Trong đó:
-- `report_range` nhận 1 trong 2 giá trị: `yearly` cho phép trả về chỉ số theo năm, `quarterly` trả về dữ liệu theo quý
-- `is_all` có giá trị mặc định là `True` cho phép lấy chỉ số qua tất cả các kỳ (năm hoặc quý), `False` cho phép lấy các kỳ gần nhất (5 năm hoặc 10 quý gần đây).
-
-<details>
-  <summary>Output</summary>
-
-  ```
->>> financial_ratio('TCB', 'yearly')
-year                      2022   2021   2020   2019   2018
-ticker                     TCB    TCB    TCB    TCB    TCB
-priceToEarning             4.5    9.7    9.0    8.2   10.7
-priceToBook                0.8    1.9    1.5    1.3    1.8
-roe                      0.197  0.217  0.181  0.178  0.215
-roa                      0.032  0.036   0.03  0.029  0.029
-earningPerShare           5729   5132   3504   2869   2410
-bookValuePerShare        32248  26452  21214  17679  14749
-interestMargin           0.053  0.057  0.049  0.043  0.041
-nonInterestOnToi         0.259   0.28  0.307  0.323  0.379
-badDebtPercentage        0.007  0.007  0.005  0.013  0.018
-provisionOnBadDebt       1.573  1.629   1.71  0.948  0.851
-costOfFinancing          0.028  0.022  0.031  0.038  0.041
-equityOnTotalAsset       0.162  0.164   0.17  0.162  0.161
-equityOnLoan              0.27  0.268  0.269  0.269  0.324
-costToIncome             0.328  0.301  0.319  0.347  0.318
-equityOnLiability          0.2    0.2    0.2    0.2    0.2
-epsChange                0.116  0.465  0.221  0.191  0.313
-assetOnEquity              6.2    6.1    5.9    6.2    6.2
-preProvisionOnToi        0.537  0.554  0.542   0.52  0.542
-postTaxOnToi               0.5  0.497  0.465  0.485  0.462
-loanOnEarnAsset          0.684  0.665  0.681  0.649  0.537
-loanOnAsset              0.602  0.611  0.631  0.602  0.498
-loanOnDeposit            1.173  1.104    1.0  0.998  0.794
-depositOnEarnAsset       0.583  0.603   0.68  0.651  0.676
-badDebtOnAsset           0.004  0.004  0.003  0.008  0.009
-liquidityOnLiability     0.347  0.382  0.372  0.411  0.531
-payableOnEquity            5.2    5.1    4.9    5.2    5.2
-cancelDebt               0.002  0.004  0.013  0.002  0.008
-bookValuePerShareChange  0.219  0.247    0.2  0.199  0.923
-creditGrowth             0.211  0.252  0.202  0.443 -0.006
-  ```
-</details>
+#### 3.5.1.2. 🏭 Phân tích chỉ số các cổ phiếu cùng ngành (Industry Analysis)
 
-## 3.7. So sánh cổ phiếu
-### 3.7.1. 🏭 Phân tích chỉ số các cổ phiếu cùng ngành
 ```python
 industry_analysis("VNM", lang='vi)
 ```
 - Trả về thông tin các mã cổ phiếu cùng ngành với mã cổ phiếu nằm trong cùng nhóm ngành với mã `VNM`.
 - Tham số `lang='vi` mặc định trả về tên các chỉ số bằng tiếng Việt, đổi thành `en` để giữ nguyên chỉ số với tên tiếng Anh.
 
 - Trong đó các chỉ số sau được thể hiện dưới dạng thập phân sử dụng để thể hiện chỉ số dưới dạng %: 
@@ -413,15 +500,16 @@
 Doanh thu quý gần nhất         NaN  -0.094 -0.252  0.093 -0.302  -0.057 -0.181  0.031 -0.352 -0.067  -0.31 -0.675 -0.197 -0.134 -0.123  0.102  -0.122 -0.142  0.009
 LNST năm tới                   NaN   0.285   0.26  0.173 -0.202   0.074  0.047 -0.719 -0.041   0.04 -0.939  0.116  6.025 -0.034   0.09 -0.155   0.813  0.022    NaN
 Doanh thu năm tới              NaN     0.2    0.3  0.162  0.283     0.1    0.1   -0.7   0.05   0.05   0.03   0.15   -0.5    0.1    0.3  -0.08   -0.06   0.02    NaN
 RSI                            NaN    50.7   43.1   71.8   24.0    28.5   59.2   33.7   68.2   53.5   46.6   44.1   51.1   32.3   55.5   55.3    33.3   54.8   61.1
 ```
 </details>
 
-### 3.7.2. 🔬 So sánh các chỉ số của danh sách các cổ phiếu tùy chọn
+
+#### 3.5.1.3. 🔬 So sánh các chỉ số của danh sách các cổ phiếu tùy chọn
 ```python
 stock_ls_analysis("TCB, BID, CEO, GMD", lang='vi')
 ```
 
 <details>
   <summary>Output</summary>
 
@@ -433,188 +521,327 @@
 1    CEO   17062  66300             1           183.2 -0.8          5.7               81.8       0.0  ...           7.8       -0.099     -0.086            NaN         3.002      -1.469      -0.2  51.9  82.0
 2    BID  225357  44550            -3            21.3  0.4          2.6                NaN       0.0  ...           NaN        0.115      0.154          0.083         0.000         NaN       NaN  49.1  34.0
 3    TCB  178003  50700             1             9.9  0.2          1.9                NaN       0.0  ...           NaN        0.418      0.255          0.059         0.157         NaN       NaN  45.2  28.0
 ```
 
 </details>
 
-### 3.7.4. 💵 Báo cáo kết quả kinh doanh, cân đối kế toán và lưu chuyển tiền tệ
 
-#### 3.7.4.1. 📄 Báo cáo kinh doanh
+#### 3.5.1.4. ⭐ Đánh giá xếp hạng 
+##### a. Đánh giá chung
+![general_rating](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/general_rating.png)
 
-![income_statement](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_income_statement.png)
 ```python
-financial_flow(symbol="TCB", report_type='incomestatement', report_range='quarterly')
+general_rating("VNM")
 ```
 
-
 <details>
   <summary>Output</summary>
 
 ```
-        ticker  revenue  yearRevenueGrowth  quarterRevenueGrowth costOfGoodSold grossProfit  ...  investProfit  serviceProfit  otherProfit  provisionExpense operationIncome  ebitda
-index                                                                                        ...
-2021-Q4    TCB     7245              0.328                 0.074           None        None  ...           279           2103          532              -627            6767    None
-2021-Q3    TCB     6742              0.310                 0.023           None        None  ...           384           1497          156              -589            6151    None
-2021-Q2    TCB     6588              0.674                 0.076           None        None  ...           717           1457          444              -598            6615    None
-2021-Q1    TCB     6124              0.454                 0.122           None        None  ...           812           1325          671              -851            6369    None
+   stockRating  valuation  financialHealth  businessModel  businessOperation  rsRating  taScore  ... ticker highestPrice  lowestPrice  priceChange3m  priceChange1y  beta   alpha
+0          2.4        1.5              4.8            3.0                3.2       1.0      1.0  ...    VNM     102722.2      78600.0         -0.092         -0.232  0.49 -0.0014
 ```
 </details>
 
-#### 3.7.4.2. 🧾 Bảng cân đối kế toán
-
-![balance_sheet](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/financial_balancesheet.png)
+##### b. 🌱 Đánh giá mô hình kinh doanh
 ```python
-financial_flow(symbol="TCB", report_type='balancesheet', report_range='quarterly')
+biz_model_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-        ticker shortAsset  cash shortInvest shortReceivable inventory longAsset  fixedAsset  ...  payableInterest  receivableInterest deposit otherDebt  fund  unDistributedIncome  minorShareHolderProfit  payable
-index                                                                                        ...
-
-2021-Q4    TCB       None  3579        None            None      None      None        7224  ...             3098                5808  314753     33680  9156                47469                     845   475756
-2021-Q3    TCB       None  3303        None            None      None      None        7106  ...             3074                6224  316376     34003  6784                45261                     753   453251
-2021-Q2    TCB       None  3554        None            None      None      None        6739  ...             2643                5736  289335     27678  6790                40924                     659   420403
-2021-Q1    TCB       None  4273        None            None      None      None        4726  ...             2897                5664  287446     26035  6790                36213                     563   3837
+  ticker  businessModel  businessEfficiency  assetQuality  cashFlowQuality  bom  businessAdministration  productService  businessAdvantage  companyPosition  industry  operationRisk
+0    VNM            3.0                   3             3                3    3                       3               3                  3                3         3              3
 ```
 </details>
 
-#### 3.7.4.3. 💶 Báo cáo lưu chuyển tiền tệ
-
+##### c. 🎮 Đánh giá hiệu quả hoạt động
 ```python
-financial_flow(symbol="TCB", report_type='cashflow', report_range='quarterly')
+biz_operation_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-        ticker  investCost  fromInvest  fromFinancial  fromSale  freeCashFlow
-index
-2021-Q4    TCB        -280        -276              0     -9328             0
-2021-Q3    TCB        -180        -179             60     17974             0
-2021-Q2    TCB        -337        -282              0     11205             0
-2021-Q1    TCB        -143        -143              0     -6954             0
+      industryEn loanGrowth depositGrowth netInterestIncomeGrowth netInterestMargin  ... last5yearsFCFFGrowth lastYearGrossProfitMargin lastYearOperatingProfitMargin  lastYearNetProfitMargin  TOIGrowth
+0  Food Products       None          None                    None              None  ...                    2                         5                             3                        4       None
 ```
 </details>
 
-## 3.8. 🧧 Lịch sử chi trả cổ tức
-
+##### d. 📑 Đánh giá sức khỏe tài chính
 ```python
-dividend_history("VNM")
+financial_health_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-   exerciseDate  cashYear  cashDividendPercentage issueMethod
-0      10/01/22      2021                    0.14        cash
-1      07/09/21      2021                    0.15        cash
-2      07/06/21      2020                    0.11        cash
-3      05/01/21      2020                    0.10        cash
+      industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
+0  Food Products        None             None         None             None    VNM              4.8              4             5           5                 5              5
 ```
 </details>
 
-## 3.9. ⭐ Đánh giá xếp hạng 
-### 3.9.1. Đánh giá chung
-![general_rating](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/general_rating.png)
-
+##### e. 💲 Đánh giá về Định giá
 ```python
-general_rating("VNM")
+valuation_rating("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-   stockRating  valuation  financialHealth  businessModel  businessOperation  rsRating  taScore  ... ticker highestPrice  lowestPrice  priceChange3m  priceChange1y  beta   alpha
-0          2.4        1.5              4.8            3.0                3.2       1.0      1.0  ...    VNM     102722.2      78600.0         -0.092         -0.232  0.49 -0.0014
+      industryEn ticker  valuation  pe  pb  ps  evebitda  dividendRate
+0  Food Products    VNM        1.5   2   1   1         1             3
 ```
 </details>
 
-### 3.9.2. 🌱 Đánh giá mô hình kinh doanh
+##### f. 💳 Sức khỏe tài chính theo ngành
 ```python
-biz_model_rating("VNM")
+industry_financial_health("VNM")
 ```
 
 <details>
   <summary>Output</summary>
 
 ```
-  ticker  businessModel  businessEfficiency  assetQuality  cashFlowQuality  bom  businessAdministration  productService  businessAdvantage  companyPosition  industry  operationRisk
-0    VNM            3.0                   3             3                3    3                       3               3                  3                3         3              3
+  industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
+0       None        None             None         None             None    VNM              3.4              4             4           3                 3              3
 ```
 </details>
 
-### 3.9.3. 🎮 Đánh giá hiệu quả hoạt động
-```python
-biz_operation_rating("VNM")
-```
+### 3.5.2. 🔎 Bộ lọc cổ phiếu
+
+Bộ lọc cổ phiếu là một hàm cho phép bạn truy vấn và lọc các cổ phiếu theo nhiều tiêu chí đa dạng dựa trên dữ liệu phân tích của TCBS. Hàm này sẽ trả về một DataFrame chứa các thông tin toàn diện về các cổ phiếu thỏa mãn điều kiện lọc của bạn. Bạn có thể dùng DataFrame này để tiếp tục phân tích, biểu diễn hoặc xuất ra dữ liệu dạng bảng tính. Đây là cập nhật ưu việt giúp bạn tiết kiệm thời gian và công sức đáng kể khi làm việc với dữ liệu cổ phiếu, đồng thời cho phép lập trình để lọc là cập nhật danh sách cổ phiếu hiệu quả không cần sử dụng giao diện web từ công ty chứng khoán.
 
 <details>
-  <summary>Output</summary>
+  <summary> Bộ lọc cổ phiếu TCBS </summary>
+
+  ![stock_scanner](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/stock_scanner_tcbs.png)
 
-```
-      industryEn loanGrowth depositGrowth netInterestIncomeGrowth netInterestMargin  ... last5yearsFCFFGrowth lastYearGrossProfitMargin lastYearOperatingProfitMargin  lastYearNetProfitMargin  TOIGrowth
-0  Food Products       None          None                    None              None  ...                    2                         5                             3                        4       None
-```
 </details>
 
-### 3.9.4. 📑 Đánh giá sức khỏe tài chính
-```python
-financial_health_rating("VNM")
-```
+Tham số
+- params (dict): một từ điển chứa các tham số và giá trị của chúng cho việc lọc cổ phiếu. Các `key` là tên của các bộ lọc, và các `value` là một giá trị đơn hoặc một tupple gồm hai giá trị (min và max) cho bộ lọc đó. Đây là ví dụ cho tham số params được thiết lập đúng:
+
+```python
+params = {
+            "exchangeName": "HOSE",
+            "marketCap": (100, 1000),
+            "pe": (10, 20),
+            "dividendYield": (5, 10),
+            "tcbsRecommend": "BUY",
+            "size": 50
+        }
+
+# Áp dụng bộ lọc với hàm để lấy kết quả
+get_stock_screening_insights(params)
+```
+
+<details>
+
+<summary>Các bộ lọc gợi ý và tiêu chí hỗ trợ bao gồm</summary>
+
+  a. BỘ LỌC GỢI Ý (PRESET)
+
+    > Sử dụng các tiêu chí lọc như sau để thiết lập tham số params.
+
+    - CANSLIM: epsGrowth1Year, lastQuarterProfitGrowth, roe, avgTradingValue20Day, relativeStrength1Month
+    - Giá trị: roe, pe, avgTradingValue20Day
+    - Cổ tức cao: dividendYield, avgTradingValue20Day
+    - Phá nền mua: avgTradingValue20Day, forecastVolumeRatio, breakout: 'BULLISH'
+    - Giá tăng + Đột biến khối lượng: avgTradingValue20Day, forecastVolumeRatio
+    - Vượt đỉnh 52 tuần: avgTradingValue20Day, priceBreakOut52Week: 'BREAK_OUT'
+    - Phá đáy 52 tuần: avgTradingValue20Day, priceWashOut52Week: 'WASH_OUT'
+    - Uptrend ngắn hạn: avgTradingValue20Day, uptrend: 'buy-signal'
+    - Vượt trội ngắn hạn: relativeStrength3Day, 
+    - Tăng trưởng: epsGrowth1Year, roe, avgTradingValue20Day
+
+  b. THÔNG TIN CHUNG
+
+    - exchangeName: sàn giao dịch của cổ phiếu, ví dụ "HOSE", "HNX", hoặc "UPCOM". Bạn có thể dùng dấu phẩy để phân tách nhiều sàn, ví dụ "HOSE,HNX,UPCOM".
+    - hasFinancialReport: Có báo cáo tài chính gần nhất. `1` nghĩa là có, `0` nghĩa là không.
+    - industryName: Lọc các cổ phiếu theo ngành cụ thể. Giá trị dạng `Retail` cho ngành Bán lẻ. Các giá trị khác có thể là:
+      - `Insurance`: Bảo hiểm
+      - `Real Estate`: Bất động sản
+      - `Technology`: Công nghệ thông tin
+      - `Oil & Gas`: Dầu khí
+      - `Financial Services`: Dịch vụ tài chính
+      - `Utilities`: Điện, nước, xăng dầu và khí đốt
+      - `Travel & Leisure`: Du lịch và giải trí
+      - `Industrial Goods & Services`: Hàng và dịch vụ công nghiệp
+      - `Personal & Household Goods`: Hàng cá nhân và gia dụng
+      - `Chemicals`: Hóa chất
+      - `Banks`: Ngân hàng
+      - `Automobiles & Parts`: Ô tô và phụ tùng
+      - `Basic Resources`: Tài nguyên cơ bản
+      - `Food & Beverage`: Thực phẩm và đồ uống
+      - `Media`: Truyền thông
+      - `Telecommunications`: Viễn thông
+      - `Construction & Materials`: Xây dựng và vật liệu
+      - `Health Care`: Y tế
+      - marketCap: vốn hóa thị trường của cổ phiếu tính bằng tỷ VND.
+      - priceNearRealtime: giá hiện tại của cổ phiếu tính bằng VND.
+      - foreignVolumePercent: tỷ lệ phần trăm khối lượng nước ngoài trong tổng khối lượng.
+      - alpha: lợi nhuận vượt trội của cổ phiếu so với lợi nhuận thị trường.
+      - beta: độ biến động của cổ phiếu so với thị trường.
+      - freeTransferRate: tỷ lệ phần trăm cổ phiếu có thể chuyển nhượng tự do.
+  
+  c. TĂNG TRƯỞNG
 
-<details>
-  <summary>Output</summary>
+    - revenueGrowth1Year: tốc độ tăng trưởng doanh thu trong năm qua.
+    - revenueGrowth5Year: tốc độ tăng trưởng doanh thu trung bình trong 5 năm qua.
+    - epsGrowth1Year: tốc độ tăng trưởng lợi nhuận trên mỗi cổ phiếu trong năm qua.
+    - epsGrowth5Year: tốc độ tăng trưởng lợi nhuận trên mỗi cổ phiếu trung bình trong 5 năm qua.
+    - lastQuarterRevenueGrowth: tốc độ tăng trưởng doanh thu trong quý gần nhất.
+    - secondQuarterRevenueGrowth: tốc độ tăng trưởng doanh thu trong quý thứ hai.
+    - lastQuarterProfitGrowth: tốc độ tăng trưởng lợi nhuận trong quý gần nhất.
+    - secondQuarterProfitGrowth: tốc độ tăng trưởng lợi nhuận trong quý thứ hai.
+  
+  d. CHỈ SỐ TÀI CHÍNH
+  
+    - grossMargin: tỷ suất lợi nhuận gộp của cổ phiếu.
+    - netMargin: tỷ suất lợi nhuận ròng của cổ phiếu.
+    - roe: tỷ suất sinh lời về vốn chủ sở hữu của cổ phiếu.
+    - doe: tỷ suất cổ tức về vốn chủ sở hữu của cổ phiếu.
+    - dividendYield: tỷ suất cổ tức của cổ phiếu.
+    - eps: lợi nhuận trên mỗi cổ phiếu của cổ phiếu tính bằng VND.
+    - pe: tỷ số giá/lợi nhuận của cổ phiếu.
+    - pb: tỷ số giá/giá trị sổ sách của cổ phiếu.
+    - evEbitda: tỷ số giá trị doanh nghiệp/lợi nhuận trước thuế, lãi vay, khấu hao và amortization của cổ phiếu.
+    - netCashPerMarketCap: tỷ số tiền mặt ròng/vốn hóa thị trường của cổ phiếu.
+    - netCashPerTotalAssets: tỷ số tiền mặt ròng/tổng tài sản của cổ phiếu.
+    - profitForTheLast4Quarters: tổng lợi nhuận trong 4 quý gần nhất của cổ phiếu tính bằng tỷ VND.
+  
+  e. BIẾN ĐỘNG GIÁ & KHỐI LƯỢNG
+
+    - suddenlyHighVolumeMatching: tín hiệu chỉ ra nếu có sự tăng đột biến khối lượng khớp lệnh cho cổ phiếu này. 0 nghĩa là không, 1 nghĩa là có.
+    - totalTradingValue: tổng giá trị giao dịch của cổ phiếu này tính bằng tỷ VND hôm nay.
+    - avgTradingValue5Day: giá trị giao dịch trung bình của cổ phiếu này tính bằng tỷ VND trong 5 ngày.
+    - avgTradingValue10Day: giá trị giao dịch trung bình của cổ phiếu này tính bằng tỷ VND trong 10 ngày.
+    - avgTradingValue20Day: giá trị giao dịch trung bình của cổ phiếu này tính bằng tỷ VND trong 20 ngày.
+    - priceGrowth1Week: tốc độ tăng trưởng giá của cổ phiếu trong tuần qua.
+    - priceGrowth1Month: tốc độ tăng trưởng giá của cổ phiếu trong tháng qua.
+    - percent1YearFromPeak: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá cao nhất trong 1 năm.
+    - percentAwayFromHistoricalPeak: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá cao nhất lịch sử.
+    - percent1YearFromBottom: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá thấp nhất trong 1 năm.
+    - percentOffHistoricalBottom: tỷ lệ phần trăm thay đổi của cổ phiếu từ giá thấp nhất lịch sử.
+    - priceVsSMA5: mối quan hệ giữa giá hiện tại và SMA 5 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSma10: mối quan hệ giữa giá hiện tại và SMA 10 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSMA20: mối quan hệ giữa giá hiện tại và SMA 20 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSma50: mối quan hệ giữa giá hiện tại và SMA 50 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - priceVsSMA100: mối quan hệ giữa giá hiện tại và SMA 100 ngày của cổ phiếu. Các giá trị có thể là "ABOVE", "BELOW", "CROSS_ABOVE", hoặc "CROSS_BELOW".
+    - forecastVolumeRatio: tỷ số giữa khối lượng dự báo và khối lượng thực tế của cổ phiếu hôm nay.
+    - volumeVsVSma5: tỷ số giữa khối lượng hiện tại và SMA khối lượng 5 ngày của cổ phiếu.
+    - volumeVsVSma10: tỷ số giữa khối lượng hiện tại và SMA khối lượng 10 ngày của cổ phiếu.
+    - volumeVsVSma20: tỷ số giữa khối lượng hiện tại và SMA khối lượng 20 ngày của cổ phiếu.
+    - volumeVsVSma50: tỷ số giữa khối lượng hiện tại và SMA khối lượng 50 ngày của cổ phiếu.
+  
+  f. HÀNH VI THỊ TRƯỜNG
+
+    - strongBuyPercentage: tỷ lệ phần trăm tín hiệu mua mạnh cho cổ phiếu này dựa trên phân tích kỹ thuật.
+    - activeBuyPercentage: tỷ lệ phần trăm tín hiệu mua tích cực cho cổ phiếu này dựa trên phân tích kỹ thuật.
+    - foreignTransaction: loại giao dịch nước ngoài cho cổ phiếu này hôm nay. Các giá trị có thể là "buyMoreThanSell", "sellMoreThanBuy", hoặc "noTransaction".
+    - foreignBuySell20Session: giá trị mua bán ròng nước ngoài cho cổ phiếu này tính bằng tỷ VND trong 20 phiên.
+    - numIncreaseContinuousDay: số ngày liên tiếp cổ phiếu này tăng giá.
+    - numDecreaseContinuousDay: số ngày liên tiếp cổ phiếu này giảm giá.
+  
+  g. TÍN HIỆU KỸ THUẬT
+
+    - rsi14: chỉ số sức mạnh tương đối (RSI) của cổ phiếu với chu kỳ 14 ngày.
+    - rsi14Status: trạng thái của RSI cho cổ phiếu này. Các giá trị có thể là "intoOverBought", "intoOverSold", "outOfOverBought", hoặc "outOfOverSold".
+    - tcbsBuySellSignal: tín hiệu mua bán cho cổ phiếu này dựa trên phân tích của TCBS. Các giá trị có thể là "BUY" hoặc "SELL".
+    - priceBreakOut52Week: tín hiệu chỉ ra nếu có sự đột phá giá cho cổ phiếu này trong 52 tuần. Các giá trị có thể là "BREAK_OUT" hoặc "NO_BREAK_OUT".
+    - priceWashOut52Week: tín hiệu chỉ ra nếu có sự rửa giá cho cổ phiếu này trong 52 tuần. Các giá trị có thể là "WASH_OUT" hoặc "NO_WASH_OUT".
+    - macdHistogram: tín hiệu chỉ ra nếu có tín hiệu MACD histogram cho cổ phiếu này. Các giá trị có thể là "macdHistGT0Increase", "macdHistGT0Decrease", "macdHistLT0Increase", hoặc "macdHistLT0Decrease".
+    - relativeStrength3Day: sức mạnh tương đối của cổ phiếu so với thị trường trong 3 ngày.
+    - relativeStrength1Month: sức mạnh tương đối của cổ phiếu so với thị trường trong 1 tháng.
+    - relativeStrength3Month: sức mạnh tương đối của cổ phiếu so với thị trường trong 3 tháng.
+    - relativeStrength1Year: sức mạnh tương đối của cổ phiếu so với thị trường trong 1 năm.
+    - tcRS: sức mạnh tương đối của TCBS của cổ phiếu so với thị trường.
+    - sarVsMacdHist: tín hiệu chỉ ra nếu có tín hiệu SAR vs MACD histogram cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+  
+  h. TÍN HIỆU MUA/BÁN
+
+    - bollingBandSignal: tín hiệu chỉ ra nếu có tín hiệu Bollinger Band cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+    - dmiSignal: tín hiệu chỉ ra nếu có tín hiệu chỉ số chuyển động hướng (DMI) cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+    - uptrend: tín hiệu chỉ ra nếu có tín hiệu xu hướng tăng cho cổ phiếu này. Các giá trị có thể là "buy-signal" hoặc "sell-signal".
+    - breakout: tín hiệu chỉ ra nếu có tín hiệu đột phá cho cổ phiếu này. Các giá trị có thể là "BULLISH" hoặc "BEARISH".
+  
+  i. TCBS ĐÁNH GIÁ
+
+    - tcbsRecommend: tín hiệu chỉ ra nếu có khuyến nghị của TCBS cho cổ phiếu này. Các giá trị có thể là "BUY" hoặc "SELL".
+    - stockRating: điểm đánh giá cổ phiếu cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
+    - businessModel: điểm đánh giá mô hình kinh doanh cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
+    - businessOperation: điểm đánh giá hoạt động kinh doanh cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
+    - financialHealth: điểm đánh giá sức khỏe tài chính cho cổ phiếu này dựa trên phân tích của TCBS. Điểm từ 1 đến 5, với 5 là tốt nhất.
 
-```
-      industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
-0  Food Products        None             None         None             None    VNM              4.8              4             5           5                 5              5
-```
 </details>
 
-### 3.9.5. 💲 Đánh giá về Định giá
-```python
-valuation_rating("VNM")
-```
+
+## 3.6. 🔥 Dữ liệu khớp lệnh trong ngày giao dịch
 
 <details>
-  <summary>Output</summary>
+  <summary>Minh hoạ giao diện TCBS</summary>
+
+  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen1.png)
+  ![intraday](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/tcbs_intraday_screen2.png)
 
-```
-      industryEn ticker  valuation  pe  pb  ps  evebitda  dividendRate
-0  Food Products    VNM        1.5   2   1   1         1             3
-```
 </details>
+vnstock cho phép người dùng tải xuống dữ liệu khớp lệnh trong ngày giao dịch theo thời gian thực. Nếu mốc thời gian bạn truy cứu rơi vào Thứ Bảy, Chủ Nhật thì dữ liệu nhận được thể hiện cho ngày giao dịch của Thứ 6 của tuần đó.
 
-## 3.10.  💳 Sức khỏe tài chính theo ngành
 ```python
-industry_financial_health("VNM")
+df =  stock_intraday_data(symbol='TCB', 
+                            page_size=500)
+print(df)
 ```
 
 <details>
-  <summary>Output</summary>
+  <summary>Terminal output</summary>
+
+  ```{r, engine='python', count_lines}
+>>> stock_intraday_data('TCB', 500)
+
+  ticker      time  orderType investorType  volume  averagePrice  orderCount
+0    TCB  14:29:55  Sell Down        SHEEP    1000       32700.0           1
+1    TCB  14:29:47     Buy Up        SHEEP     200       32750.0           1
+2    TCB  14:29:44  Sell Down         WOLF    8000       32700.0          14
+3    TCB  14:29:41  Sell Down        SHEEP    1000       32700.0           5
+4    TCB  14:29:36  Sell Down         WOLF   23800       32700.0          10
+  ```
+
+</details>
+
+<details>
+  <summary>Giải thích ý nghĩa chỉ số</summary>
+  • Khi 1 lệnh lớn (từ Cá mập, tay to, tổ chức....) mua chủ động (hoặc bán chủ động) được đưa vào Sàn, thường thì nó sẽ được khớp với nhiều lệnh nhỏ đang chờ bán (hoặc chờ mua). Nếu chỉ nhìn realtime theo từng lệnh khớp riêng lẻ, thì sẽ không thể phát hiện được các lệnh to (của Cá mập, tay to...) vừa được đẩy vào Sàn. Vì vậy, chúng tôi "cộng dồn" các lệnh khớp này lại (phát sinh bởi 1 lệnh lớn chủ động vào sàn trong 1 khoảng thời gian rất nhanh) để giúp NĐT phát hiện các lệnh lớn (của Cá mập, tay to....) chính xác hơn. Lệnh Cá mập sẽ được tô xanh (cho Mua chủ động) và đỏ (cho Bán chủ động). 
+
+  • Cá mập: (CM - SHARK) nhà đầu tư tay to, tổ chức, đầu tư lớn, dẫn dắt thị trường. Giá trị 1 lệnh đặt > 1 tỷ đồng/lệnh đặt. Đồ thị 1N dùng số liệu 1 phút cho 60’ gần nhất; 1W là tổng mỗi 15’ cho 1 tuần; 1M là tổng hàng ngày cho 1 tháng
+
+  • Sói già: (SG - WOLF) nhà đầu tư kinh nghiệm, giá trị lệnh đặt cao. Giá trị 1 lệnh đặt từ 200 tr đến 1 tỷ đồng/lệnh đặt.
+
+  • Cừu non: (CN - SHEEP) nhà đầu tư nhỏ lẻ, giá trị giao dịch và mua bán chủ động thấp. Giá trị 1 lệnh đặt Mua hoặc Bán chủ động < 200 triệu đồng/lệnh đặt vào.
+
+  • Mua chủ động (hay Buy Up) là khi NĐT thực hiện chủ động mua lên qua việc đặt lệnh mua với giá bằng giá dư bán gần nhất để có thể khớp luôn. Như thế, giá khớp cho lệnh này thường sẽ đẩy giá khớp lên cao hơn thị giá trước đó.
+
+  • Bán chủ động (hay Sell Down) là khi NĐT thực hiện chủ động Bán dưới giá hiện tại (hay thị giá) của cổ phiếu bằng việc đặt lệnh bán với giá bán bằng giá dư mua gần nhất để khớp ngay. Và như thế, thị giá sẽ bị kéo xuống thấp hơn so với thị giá trước đó. Thống kê khối lượng giao dich theo Mua CĐ và Bán CĐ dùng để đánh giá tương quan giữa cung (Bán CĐ) và cầu (Mua CĐ) trên giao dịch khớp lệnh thực tế, nhằm nhận định tương đối về sự vận động của xu hướng dòng tiền. Khi tỷ lệ % Mua CĐ trên (Tổng Mua và Bán CĐ) lớn hơn 50%, đồng nghĩa với việc thị trường đang có xu hướng mua vào nhiều hơn bán ra và ngược lại, qua đó xác định được dòng tiền vào/ra với mỗi cổ phiếu. Khi tỷ lệ này cao đột biến (>70% hay <30%) so với điểm cân bằng (50%) , đó là tín hiệu của việc mua hoặc bán bất chấp của thị trường.
 
-```
-  industryEn loanDeposit badLoanGrossLoan badLoanAsset provisionBadLoan ticker  financialHealth  netDebtEquity  currentRatio  quickRatio  interestCoverage  netDebtEBITDA
-0       None        None             None         None             None    VNM              3.4              4             4           3                 3              3
-```
 </details>
 
-## 3.11. 🌏 Thông tin thị trường
+
+## 3.7. 🌏 Thông tin thị trường
 
 <details>
-  <summary>Tạm ngưng hoạt động do SSI từ chối truy cập</summary>
+  <summary>Tạm ngưng hoạt động, chờ nâng cấp APIs</summary>
 
-### 3.11.1. Các mã cổ phiếu đứng đầu theo tiêu chí xếp loại 
+### 3.7.1. Các mã cổ phiếu đứng đầu theo tiêu chí xếp loại 
 
 <details>
   <summary>SSI Top Stocks</summary>
 
 Top Breakout (Đột phá) > Top Gainers (Tăng giá) > Top Losers (Giảm giá) > Top Value (Giá trị) > Top Volume (Khối lượng)
 ![top_mover](./src/ssi_top_breakout_gainer_loser.png)
 
@@ -636,15 +863,15 @@
 1          3270200.0     1.088892e+11  ...  {'organCode': 'STB', 'rtd7': 18173.6958318461,...  {'organCode': 'STB', 'sma20Past4': 34332.5, 's...
 2          1456800.0     4.199166e+10  ...  {'organCode': 'FUEVFVND', 'rtd7': None, 'rtd11...  {'organCode': 'FUEVFVND', 'sma20Past4': 27993....
 3          1033300.0     1.281170e+10  ...  {'organCode': 'FLC', 'rtd7': 12898.0038031343,...  {'organCode': 'FLC', 'sma20Past4': 12062.5, 's...
 4           998600.0     5.324337e+10  ...  {'organCode': 'NLG', 'rtd7': 23318.1252311207,...  {'organCode': 'NLG', 'sma20Past4': 52385.0, 's...
 ```
 </details>
 
-### 3.11.2. Thông tin giao dịch nhà đầu tư nước ngoài (NDTNN)
+### 3.7.2. Thông tin giao dịch nhà đầu tư nước ngoài (NDTNN)
 Trong ví dụ dưới đây, thể hiện giao dịch mua vào của NDTNN.
 
 ```python
 fr_trade_heatmap ('All', 'FrBuyVol')
 ```
 <details>
   <summary>Output</summary>
@@ -663,15 +890,15 @@
   2        ELC   ELC     4100.0            0.049197  ...       10650.0      9270.0  Công nghệ Thông tin  0.034816
   3        ITD   ITD     2000.0            0.068548  ...       13250.0     11550.0  Công nghệ Thông tin  0.034816
 
   [92 rows x 10 columns]
   ```
 </details>
 
-### 3.11.3. Biến động của các nhóm chỉ số
+### 3.7.3. Biến động của các nhóm chỉ số
 ![latest_indices](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/get_latest_indices.png)
 
 Thông tin các nhóm chỉ số phổ biến của thị trường chứng khoán Việt Nam.
 
 ```python
 get_latest_indices()
 ```
@@ -706,16 +933,16 @@
 21        0         VNSI     1715.37  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
 22        0        VNSML     1140.40  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
 23        0        VNUTI      874.84  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
 24        0        VNX50     1805.33  2023-01-19T00:00:00  ...         0.0      0.0    0.0          None
   ```
 </details>
 
-### 3.11.4. Dữ liệu chuyên sâu theo nhóm chỉ số cụ thể
-![index_series_data](https://raw.githubusercontent.com/thinh-vu/vnstock/main/src/get_index_series_data.png)
+### 3.7.4. Dữ liệu chuyên sâu theo nhóm chỉ số cụ thể
+![index_series_data](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/get_index_series_data.png)
 
 ```python
 get_index_series(index_code='VNINDEX', time_range='OneYear')
 ```
 - Nhà cung cấp dữ liệu: SSI iBoard sử dụng dữ liệu từ FiinTrade.
 - Sử dụng một trong các mã chỉ số sau để tra cứu:
   
@@ -751,15 +978,65 @@
 
   [246 rows x 14 columns]
   ```
 </details>
 
 </details>
 
-# IV. 🙋‍♂️ Contact Information
+## 3.8. 🛡 Thị trường Phái Sinh
+
+### 3.8.1. Dữ liệu giá lịch sử
+
+> Xem chi tiết mục [3.4.1 📈 Truy xuất dữ liệu giá lịch sử](#341--truy-xuất-dữ-liệu-giá-lịch-sử) cùng với thông tin giá chứng khoán cơ sở.
+
+### 3.8.2. Dữ liệu khớp lệnh lịch sử
+
+<details>
+
+<summary>Minh họa bảng dữ liệu khớp lệnh Phái sinh - CK Rồng Việt </summary>
+
+![livedragon_derivative_match](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/livedragon_derivative_history_match.png)
+
+</details>
+
+Để truy vấn dữ liệu từ hàm này, bạn cần có cookie người dùng (không cần đăng nhập) của chứng khoán Rồng Việt. Các bước thực hiện như sau:
+  1. Truy cập `https://livedragon.vdsc.com.vn/all/all.rv`
+  2. Mở `Developer Tools` trên trình duyệt, sử dụng F12 hoặc `Ctrl` + `Shift` + `I` trên Windows hoặc `Cmd` + `Option` + `I` trên macOS
+  3. Chuyển đến tab `Network` và chọn mục `Fetch/XHR`
+  4. Mở bất kỳ mục request nào trong tab này, tìm mục `Header` của request
+  5. Tìm và copy giá trị của `Cookie` trong request này để điền vào bước tiếp theo dưới đây trước khi gọi hàm
+
+```python
+cookie = 'GIÁ TRỊ COOKIE CẦN PASTE VÀO ĐÂY'
+derivatives_historical_match (symbol='VN30F2308', date='2023-07-24', cookie=cookie)
+```
+
+# IV. 🚚 Xuất, Lưu trữ, Chia sẻ dữ liệu
+
+> Để xuất, lưu trữ và chia sẻ dữ liệu với vnstock, bạn có rất nhiều sự lựa chọn kể cả sử dụng cơ sở dữ liệu, bảng tính (Excel, Google Sheets) và nhiều hình thức khác. Dữ liệu tiêu chuẩn tạo ra bởi vnstock là các pandas DataFrame do đó bạn có thể biến đổi và lưu trữ/chia sẻ dữ liệu dễ dàng với cách thức tiêu chuẩn của python. Dưới đây là hướng dẫn cơ bản với cách thức xuất dữ liệu ra csv và Google Sheets.
+
+## 4.1. Xuất dữ liệu ra csv
+
+Dành cho những bạn mới làm quen Python và Pandas có thể sử dụng dữ liệu từ vnstock dễ dàng với công cụ bảng tính quen thuộc. Bạn có thể xuất dữ liệu từ hàm bất kỳ ra csv và mở bằng Excel hoặc upload lên Google Drive và mở bằng Google Sheets.
+
+```python
+start_date = '2023-06-01'
+end_date = '2023-07-24'
+# Truy xuất dữ liệu
+df = stock_historical_data('TCB', start_date, end_date)
+# Xuất dữ liệu ra csv, chèn ngày tháng và mã CP
+df.to_csv(f'THƯ-MỤC-CỦA-BẠN/TCB_historical_price_{start_date}_{end_date}.csv', index=True)
+```
+
+## 4.2. Xuất dữ liệu ra Google Sheets
+
+Phương thức này được thiết kế riêng để xuất dữ liệu trực tiếp từ Google Colab sang Google Sheets (sẽ không hoạt động nếu chạy ở môi trường local, không thiết lập môi trường tương đồng Colab). Tham khảo cách làm chi tiết trong file demo, mục `III. Data Export`
+
+
+# V. 🙋‍♂️ Thông tin liên hệ
 
 Bạn có thể kết nối với tác giả qua các hình thức sau. Trong trường hợp cần hỗ trợ nhanh, bạn có thể chọn nhắn tin qua Messenger hoặc Linkedin, tôi sẽ phản hồi ngay lập tức nếu có thể trong hầu hết các trường hợp.
 
 <div id="badges" align="center">
   <a href="https://www.linkedin.com/in/thinh-vu">
     <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
   </a>
@@ -770,35 +1047,37 @@
   </a>
   </a>
     <a href="https://github.com/thinh-vu">
     <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="Github Badge"/>
   </a>
 </div>
 
-# V. 💪 Hỗ trợ phát triển dự án vnstock
+# VI. 💪 Hỗ trợ phát triển dự án vnstock
 
 Nếu bạn nhận thấy giá trị từ vnstock và các dự án mã nguồn mở của tôi, bạn có thể hỗ trợ phát triển chúng bằng cách quyên góp hoặc đơn giản là gửi tặng tôi một ly cà phê để cảm ơn.
 Bạn có thể chọn 1 trong 3 hình thức đóng góp bao gồm Momo, Chuyển khoản ngân hàng và Gửi tiền qua Paypal. Sự đóng góp của bạn sẽ giúp tôi duy trì phí lưu trữ blog và tiếp tục tạo ra nội dung chất lượng cao. Cảm ơn sự ủng hộ của bạn!
 
 - [Paypal](https://paypal.me/thinhvuphoto?country.x=VN&locale.x=en_US)
+
 - ![momo-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/momo-qr-thinhvu.jpeg)
+  
 - ![vcb-qr](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/src/vcb-qr-thinhvu.jpg)
 
-# VI. ⚖ Tuyên bố miễn trừ trách nhiệm
+# VII. ⚖ Tuyên bố miễn trừ trách nhiệm
 vnstock được phát triển nhằm mục đích cung cấp các công cụ nghiên cứu đơn giản và miễn phí, nhằm giúp người nghiên cứu tiếp cận và phân tích dữ liệu chứng khoán một cách dễ dàng. Dữ liệu được cung cấp phụ thuộc vào nguồn cấp dữ liệu, do đó, khi sử dụng, bạn cần thận trọng và cân nhắc.
 
 💰 Trong bất kỳ trường hợp nào, người sử dụng hoàn toàn chịu trách nhiệm về quyết định sử dụng dữ liệu trích xuất từ vnstock và chịu trách nhiệm với bất kỳ tổn thất nào có thể phát sinh. Bạn nên tự mình đảm bảo tính chính xác và đáng tin cậy của dữ liệu trước khi sử dụng chúng.
 
 Việc sử dụng dữ liệu chứng khoán và quyết định đầu tư là hoạt động có rủi ro và có thể gây mất mát tài sản. Bạn nên tìm kiếm lời khuyên từ các chuyên gia tài chính và tuân thủ các quy định pháp luật về chứng khoán tại Việt Nam và quốc tế khi tham gia vào hoạt động giao dịch chứng khoán.
 
 Xin lưu ý rằng vnstock không chịu trách nhiệm và không có bất kỳ trách nhiệm pháp lý nào đối với bất kỳ tổn thất hoặc thiệt hại nào phát sinh từ việc sử dụng gói phần mềm này.
 
 🐱‍👤 vnstock được thiết kế hoàn toàn cho mục đích phân tích và thực hành nghiên cứu đầu tư. Mọi hình thức sử dụng không đúng mục đích hoặc việc sử dụng trái phép thư viện với mục đích xấu như tấn công public API hay gây hại cho hệ thống thông qua từ chối truy cập hoặc các hành động tương tự, hoàn toàn nằm ngoài phạm vi sử dụng dự định và không thuộc trách nhiệm của nhóm phát triển.
 
-# VII. Bản quyền và giấy phép
+# VII. 🔑 Bản quyền và giấy phép
 
 
 ```
 Bản quyền (c) 2022 Thinh Vu | thinh-vu @ Github | MIT
 
 Được cấp phép theo quyền tự do, miễn phí, cho bất kỳ cá nhân nào nhận được một bản sao của phần mềm này và các tệp tài liệu liên quan (gọi chung là "Phần mềm"), để sử dụng Phần mềm mà không có bất kỳ hạn chế nào, bao gồm nhưng không giới hạn quyền sử dụng, sao chép, sửa đổi, hợp nhất, xuất bản, phân phối, cấp phép lại và/hoặc bán các bản sao của Phần mềm, và cho phép những người nhận Phần mềm được nhúng vào Phần mềm này, tuân thủ các điều kiện sau đây:
```

