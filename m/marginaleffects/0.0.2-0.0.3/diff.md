# Comparing `tmp/marginaleffects-0.0.2.tar.gz` & `tmp/marginaleffects-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marginaleffects-0.0.2.tar", max compression
+gzip compressed data, was "marginaleffects-0.0.3.tar", max compression
```

## Comparing `marginaleffects-0.0.2.tar` & `marginaleffects-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-06-23 12:35:22.380022 marginaleffects-0.0.2/LICENSE
--rw-r--r--   0        0        0    21414 2023-07-03 14:49:27.431095 marginaleffects-0.0.2/README.md
--rw-r--r--   0        0        0      213 2023-07-17 11:30:51.590734 marginaleffects-0.0.2/marginaleffects/__init__.py
--rw-r--r--   0        0        0     1002 2023-07-02 17:04:59.766245 marginaleffects-0.0.2/marginaleffects/by.py
--rw-r--r--   0        0        0    12500 2023-07-17 17:09:56.076355 marginaleffects-0.0.2/marginaleffects/comparisons.py
--rw-r--r--   0        0        0     1293 2023-07-03 19:04:37.399801 marginaleffects-0.0.2/marginaleffects/datagrid.py
--rw-r--r--   0        0        0     1573 2023-07-17 21:14:19.192874 marginaleffects-0.0.2/marginaleffects/equivalence.py
--rw-r--r--   0        0        0     3159 2023-07-02 17:04:59.766245 marginaleffects-0.0.2/marginaleffects/estimands.py
--rw-r--r--   0        0        0      797 2023-07-03 18:53:03.449912 marginaleffects-0.0.2/marginaleffects/hypotheses.py
--rw-r--r--   0        0        0     6910 2023-07-03 19:04:37.439801 marginaleffects-0.0.2/marginaleffects/hypothesis.py
--rw-r--r--   0        0        0     4741 2023-07-17 11:52:55.980428 marginaleffects-0.0.2/marginaleffects/predictions.py
--rw-r--r--   0        0        0    13808 2023-07-19 22:18:46.711146 marginaleffects-0.0.2/marginaleffects/sanity.py
--rw-r--r--   0        0        0     1349 2023-07-03 14:55:05.161013 marginaleffects-0.0.2/marginaleffects/slopes.py
--rw-r--r--   0        0        0      399 2023-07-03 19:04:37.399801 marginaleffects-0.0.2/marginaleffects/transform.py
--rw-r--r--   0        0        0     2283 2023-07-17 22:00:12.872288 marginaleffects-0.0.2/marginaleffects/uncertainty.py
--rw-r--r--   0        0        0     2926 2023-07-18 18:34:41.336491 marginaleffects-0.0.2/marginaleffects/utils.py
--rw-r--r--   0        0        0      771 2023-07-19 22:19:02.601143 marginaleffects-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    22069 1970-01-01 00:00:00.000000 marginaleffects-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-23 12:22:21.334170 marginaleffects-0.0.3/LICENSE
+-rw-r--r--   0        0        0    23288 2023-07-24 22:11:24.850825 marginaleffects-0.0.3/README.md
+-rw-r--r--   0        0        0      213 2023-07-03 23:36:04.163006 marginaleffects-0.0.3/marginaleffects/__init__.py
+-rw-r--r--   0        0        0     1002 2023-07-01 14:37:00.809371 marginaleffects-0.0.3/marginaleffects/by.py
+-rw-r--r--   0        0        0     1958 2023-07-24 01:30:03.435871 marginaleffects-0.0.3/marginaleffects/classes.py
+-rw-r--r--   0        0        0    12629 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/comparisons.py
+-rw-r--r--   0        0        0     1293 2023-07-03 23:29:26.413040 marginaleffects-0.0.3/marginaleffects/datagrid.py
+-rw-r--r--   0        0        0     1573 2023-07-22 00:54:29.376618 marginaleffects-0.0.3/marginaleffects/equivalence.py
+-rw-r--r--   0        0        0     3159 2023-07-01 12:13:24.451354 marginaleffects-0.0.3/marginaleffects/estimands.py
+-rw-r--r--   0        0        0      803 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/hypotheses.py
+-rw-r--r--   0        0        0     6910 2023-07-03 23:29:26.413040 marginaleffects-0.0.3/marginaleffects/hypothesis.py
+-rw-r--r--   0        0        0     4870 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/predictions.py
+-rw-r--r--   0        0        0    13777 2023-07-23 15:35:08.210252 marginaleffects-0.0.3/marginaleffects/sanity.py
+-rw-r--r--   0        0        0     1361 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/slopes.py
+-rw-r--r--   0        0        0      399 2023-07-03 23:29:26.423040 marginaleffects-0.0.3/marginaleffects/transform.py
+-rw-r--r--   0        0        0     2287 2023-07-23 23:25:01.616114 marginaleffects-0.0.3/marginaleffects/uncertainty.py
+-rw-r--r--   0        0        0     2926 2023-07-22 00:54:29.376618 marginaleffects-0.0.3/marginaleffects/utils.py
+-rw-r--r--   0        0        0      771 2023-07-24 22:11:12.810825 marginaleffects-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    23943 1970-01-01 00:00:00.000000 marginaleffects-0.0.3/PKG-INFO
```

### Comparing `marginaleffects-0.0.2/LICENSE` & `marginaleffects-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.2/README.md` & `marginaleffects-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: marginaleffects
+Version: 0.0.3
+Summary: 
+Author: Vincent Arel-Bundock
+Author-email: vincent.arel-bundock@umontreal.ca
+Requires-Python: >=3.9,<3.13
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.25.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: polars (>=0.18.3,<0.19.0)
+Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
+Requires-Dist: scipy (>1.10.0)
+Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
+Description-Content-Type: text/markdown
+
 # `marginaleffects` for Python
 
 The `marginaleffects` package allows `Python` users to compute and plot
 three principal quantities of interest: (1) predictions, (2)
 comparisons, and (3) slopes. In addition, the package includes a
 convenience function to compute a fourth estimand, “marginal means”,
 which is a special case of averaged predictions. `marginaleffects` can
@@ -97,16 +116,16 @@
 ```
 
                                 OLS Regression Results                            
     ==============================================================================
     Dep. Variable:                    mpg   R-squared:                       0.896
     Model:                            OLS   Adj. R-squared:                  0.866
     Method:                 Least Squares   F-statistic:                     29.55
-    Date:                Sun, 02 Jul 2023   Prob (F-statistic):           2.60e-10
-    Time:                        21:01:20   Log-Likelihood:                -66.158
+    Date:                Mon, 24 Jul 2023   Prob (F-statistic):           2.60e-10
+    Time:                        18:11:21   Log-Likelihood:                -66.158
     No. Observations:                  32   AIC:                             148.3
     Df Residuals:                      24   BIC:                             160.0
     Df Model:                           7                                         
     Covariance Type:            nonrobust                                         
     ==============================================================================
                      coef    std err          t      P>|t|      [0.025      0.975]
     ------------------------------------------------------------------------------
@@ -141,21 +160,23 @@
 pre = predictions(mod)
 
 pre.shape
 
 print(pre.head())
 ```
 
-    | rowid | estimate  | std_error | statistic | … | vs  | am  | gear | carb |
-    |-------|-----------|-----------|-----------|---|-----|-----|------|------|
-    | 0     | 22.488569 | 0.884149  | 25.43528  | … | 0   | 1   | 4    | 4    |
-    | 1     | 20.801859 | 1.194205  | 17.419002 | … | 0   | 1   | 4    | 4    |
-    | 2     | 25.264652 | 0.708531  | 35.657806 | … | 1   | 1   | 4    | 1    |
-    | 3     | 20.255492 | 0.704464  | 28.753051 | … | 1   | 0   | 3    | 1    |
-    | 4     | 16.997817 | 0.711866  | 23.877839 | … | 0   | 0   | 3    | 2    |
+    | Estimate | Std.Error | z    | P(>|z|) | S    | [    | ]    |
+    |----------|-----------|------|---------|------|------|------|
+    | 22.5     | 0.884     | 25.4 | 0       | inf  | 20.7 | 24.3 |
+    | 20.8     | 1.19      | 17.4 | 4e-15   | 47.8 | 18.3 | 23.3 |
+    | 25.3     | 0.709     | 35.7 | 0       | inf  | 23.8 | 26.7 |
+    | 20.3     | 0.704     | 28.8 | 0       | inf  | 18.8 | 21.7 |
+    | 17       | 0.712     | 23.9 | 0       | inf  | 15.5 | 18.5 |
+
+    Columns: rowid, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 #### Comparisons: Differences, Ratios, Log-Odds, Lift, etc.
 
 Now, we use the `comparisons()` function to compute the difference in
 predicted outcome when each of the predictors is incremented by 1 unit
 (one predictor at a time, holding all others constant). Once again,
 comparisons are unit-level quantities. And since there are 3 predictors
@@ -165,79 +186,87 @@
 cmp = comparisons(mod)
 
 cmp.shape
 
 print(cmp.head())
 ```
 
-    | rowid | term | contrast | estimate  | … | vs  | am  | gear | carb |
-    |-------|------|----------|-----------|---|-----|-----|------|------|
-    | 0     | hp   | +1       | -0.036906 | … | 0   | 1   | 4    | 4    |
-    | 1     | hp   | +1       | -0.028689 | … | 0   | 1   | 4    | 4    |
-    | 2     | hp   | +1       | -0.046572 | … | 1   | 1   | 4    | 1    |
-    | 3     | hp   | +1       | -0.042271 | … | 1   | 0   | 3    | 1    |
-    | 4     | hp   | +1       | -0.039018 | … | 0   | 0   | 3    | 2    |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S    | [       | ]       |
+    |------|----------|----------|-----------|---|---------|------|---------|---------|
+    | hp   | +1       | -0.0369  | 0.0185    | … | 0.0575  | 4.12 | -0.0751 | 0.00128 |
+    | hp   | +1       | -0.0287  | 0.0156    | … | 0.0788  | 3.67 | -0.0609 | 0.00357 |
+    | hp   | +1       | -0.0466  | 0.0226    | … | 0.0502  | 4.32 | -0.0932 | 4.6e-05 |
+    | hp   | +1       | -0.0423  | 0.0133    | … | 0.00401 | 7.96 | -0.0697 | -0.0149 |
+    | hp   | +1       | -0.039   | 0.0134    | … | 0.00769 | 7.02 | -0.0667 | -0.0113 |
+
+    Columns: rowid, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, predicted, predicted_lo, predicted_hi, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 The `comparisons()` function allows customized queries. For example,
 what happens to the predicted outcome when the `hp` variable increases
 from 100 to 120?
 
 ``` python
 cmp = comparisons(mod, variables = {"hp": [120, 100]})
 print(cmp)
 ```
 
-    | rowid | term | contrast  | estimate | … | vs  | am  | gear | carb |
-    |-------|------|-----------|----------|---|-----|-----|------|------|
-    | 0     | hp   | 100 - 120 | 0.738111 | … | 0   | 1   | 4    | 4    |
-    | 1     | hp   | 100 - 120 | 0.573787 | … | 0   | 1   | 4    | 4    |
-    | 2     | hp   | 100 - 120 | 0.931433 | … | 1   | 1   | 4    | 1    |
-    | 3     | hp   | 100 - 120 | 0.845426 | … | 1   | 0   | 3    | 1    |
-    | …     | …    | …         | …        | … | …   | …   | …    | …    |
-    | 28    | hp   | 100 - 120 | 0.383687 | … | 0   | 1   | 5    | 4    |
-    | 29    | hp   | 100 - 120 | 0.64145  | … | 0   | 1   | 5    | 6    |
-    | 30    | hp   | 100 - 120 | 0.125924 | … | 0   | 1   | 5    | 8    |
-    | 31    | hp   | 100 - 120 | 0.635006 | … | 1   | 1   | 4    | 2    |
+    | Term | Contrast  | Estimate | Std.Error | … | P(>|z|) | S     | 2.5%      | 97.5% |
+    |------|-----------|----------|-----------|---|---------|-------|-----------|-------|
+    | hp   | 100 - 120 | 0.738    | 0.37      | … | 0.0576  | 4.12  | -0.0256   | 1.5   |
+    | hp   | 100 - 120 | 0.574    | 0.313     | … | 0.0788  | 3.67  | -0.0713   | 1.22  |
+    | hp   | 100 - 120 | 0.931    | 0.452     | … | 0.0502  | 4.32  | -0.000918 | 1.86  |
+    | hp   | 100 - 120 | 0.845    | 0.266     | … | 0.00401 | 7.96  | 0.297     | 1.39  |
+    | …    | …         | …        | …         | … | …       | …     | …         | …     |
+    | hp   | 100 - 120 | 0.384    | 0.27      | … | 0.168   | 2.57  | -0.173    | 0.941 |
+    | hp   | 100 - 120 | 0.641    | 0.334     | … | 0.0671  | 3.9   | -0.0488   | 1.33  |
+    | hp   | 100 - 120 | 0.126    | 0.272     | … | 0.648   | 0.626 | -0.436    | 0.688 |
+    | hp   | 100 - 120 | 0.635    | 0.332     | … | 0.068   | 3.88  | -0.0507   | 1.32  |
+
+    Columns: rowid, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, predicted, predicted_lo, predicted_hi, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 What happens to the predicted outcome when the `wt` variable increases
 by 1 standard deviation about its mean?
 
 ``` python
 cmp = comparisons(mod, variables = {"hp": "sd"})
 print(cmp)
 ```
 
-    | rowid | term | contrast           | estimate  | … | vs  | am  | gear | carb |
-    |-------|------|--------------------|-----------|---|-----|-----|------|------|
-    | 0     | hp   | +68.56286848932059 | -2.530351 | … | 0   | 1   | 4    | 4    |
-    | 1     | hp   | +68.56286848932059 | -1.967025 | … | 0   | 1   | 4    | 4    |
-    | 2     | hp   | +68.56286848932059 | -3.193087 | … | 1   | 1   | 4    | 1    |
-    | 3     | hp   | +68.56286848932059 | -2.89824  | … | 1   | 0   | 3    | 1    |
-    | …     | …    | …                  | …         | … | …   | …   | …    | …    |
-    | 28    | hp   | +68.56286848932059 | -1.315334 | … | 0   | 1   | 5    | 4    |
-    | 29    | hp   | +68.56286848932059 | -2.198983 | … | 0   | 1   | 5    | 6    |
-    | 30    | hp   | +68.56286848932059 | -0.431686 | … | 0   | 1   | 5    | 8    |
-    | 31    | hp   | +68.56286848932059 | -2.176891 | … | 1   | 1   | 4    | 2    |
+    | Term | Contrast           | Estimate | Std.Error | … | P(>|z|) | S     | 2.5%  | 97.5%   |
+    |------|--------------------|----------|-----------|---|---------|-------|-------|---------|
+    | hp   | +68.56286848932059 | -2.53    | 1.27      | … | 0.0576  | 4.12  | -5.15 | 0.0878  |
+    | hp   | +68.56286848932059 | -1.97    | 1.07      | … | 0.0788  | 3.67  | -4.18 | 0.245   |
+    | hp   | +68.56286848932059 | -3.19    | 1.55      | … | 0.0502  | 4.32  | -6.39 | 0.00315 |
+    | hp   | +68.56286848932059 | -2.9     | 0.911     | … | 0.00401 | 7.96  | -4.78 | -1.02   |
+    | …    | …                  | …        | …         | … | …       | …     | …     | …       |
+    | hp   | +68.56286848932059 | -1.32    | 0.925     | … | 0.168   | 2.57  | -3.22 | 0.594   |
+    | hp   | +68.56286848932059 | -2.2     | 1.15      | … | 0.0671  | 3.9   | -4.57 | 0.167   |
+    | hp   | +68.56286848932059 | -0.432   | 0.933     | … | 0.648   | 0.626 | -2.36 | 1.49    |
+    | hp   | +68.56286848932059 | -2.18    | 1.14      | … | 0.068   | 3.88  | -4.53 | 0.174   |
+
+    Columns: rowid, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, predicted, predicted_lo, predicted_hi, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 The `comparisons()` function also allows users to specify arbitrary
 functions of predictions, with the `comparison` argument. For example,
 what is the average ratio between predicted Miles per Gallon after an
 increase of 50 units in Horsepower?
 
 ``` python
 cmp = comparisons(
   mod,
   variables = {"hp": 50},
   comparison = "ratioavg")
 print(cmp)
 ```
 
-    | term | contrast | estimate | std_error | … | p_value | s_value | conf_low | conf_high |
-    |------|----------|----------|-----------|---|---------|---------|----------|-----------|
-    | hp   | +50      | 0.909534 | 0.029058  | … | 0.0     | inf     | 0.84956  | 0.969507  |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S   | 2.5% | 97.5% |
+    |------|----------|----------|-----------|---|---------|-----|------|-------|
+    | hp   | +50      | 0.91     | 0.0291    | … | 0       | inf | 0.85 | 0.97  |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 #### Slopes: Derivatives and elasticities
 
 Consider a logistic regression model with a single predictor:
 
 ``` python
 url = "https://vincentarelbundock.github.io/Rdatasets/csv/datasets/mtcars.csv"
@@ -254,17 +283,19 @@
 slope of the prediction function at `mpg = 24`?
 
 ``` python
 mfx = slopes(mod, newdata = datagrid(mpg = 24, newdata = mtcars))
 print(mfx)
 ```
 
-    | term | contrast | estimate | std_error | … | p_value  | s_value   | conf_low | conf_high |
-    |------|----------|----------|-----------|---|----------|-----------|----------|-----------|
-    | mpg  | dY/dX    | 0.066534 | 0.01779   | … | 0.000776 | 10.331677 | 0.030203 | 0.102866  |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|)  | S    | 2.5%   | 97.5% |
+    |------|----------|----------|-----------|---|----------|------|--------|-------|
+    | mpg  | dY/dX    | 0.0665   | 0.0178    | … | 0.000798 | 10.3 | 0.0301 | 0.103 |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 This is equivalent to the result we obtain by taking the analytical
 derivative using the chain rule:
 
 ``` python
 from scipy.stats import logistic
 beta_0 = mod.params.iloc[0]
@@ -279,37 +310,43 @@
 values:
 
 ``` python
 mfx = slopes(mod, newdata = "mean")
 print(mfx)
 ```
 
-    | term | contrast | estimate | std_error | … | p_value  | s_value  | conf_low | conf_high |
-    |------|----------|----------|-----------|---|----------|----------|----------|-----------|
-    | mpg  | dY/dX    | 0.073235 | 0.028289  | … | 0.014712 | 6.086849 | 0.015461 | 0.13101   |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S    | 2.5%   | 97.5% |
+    |------|----------|----------|-----------|---|---------|------|--------|-------|
+    | mpg  | dY/dX    | 0.0732   | 0.0283    | … | 0.0148  | 6.08 | 0.0154 | 0.131 |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 ``` python
 mfx = slopes(mod, newdata = "median")
 print(mfx)
 ```
 
-    | term | contrast | estimate | std_error | … | p_value  | s_value  | conf_low | conf_high |
-    |------|----------|----------|-----------|---|----------|----------|----------|-----------|
-    | mpg  | dY/dX    | 0.067875 | 0.025298  | … | 0.011754 | 6.410751 | 0.01621  | 0.119539  |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S    | 2.5%   | 97.5% |
+    |------|----------|----------|-----------|---|---------|------|--------|-------|
+    | mpg  | dY/dX    | 0.0679   | 0.0253    | … | 0.0118  | 6.41 | 0.0162 | 0.12  |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 We can also compute an “average slope” or “average marginaleffects”
 
 ``` python
 mfx = avg_slopes(mod)
 print(mfx)
 ```
 
-    | term | contrast    | estimate | std_error | … | p_value  | s_value   | conf_low | conf_high |
-    |------|-------------|----------|-----------|---|----------|-----------|----------|-----------|
-    | mpg  | mean(dY/dX) | 0.046486 | 0.008864  | … | 0.000012 | 16.384139 | 0.028382 | 0.06459   |
+    | Term | Contrast    | Estimate | Std.Error | … | P(>|z|)  | S    | 2.5%   | 97.5%  |
+    |------|-------------|----------|-----------|---|----------|------|--------|--------|
+    | mpg  | mean(dY/dX) | 0.0465   | 0.00886   | … | 1.16e-05 | 16.4 | 0.0284 | 0.0646 |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 Which again is equivalent to the analytical result:
 
 ``` python
 np.mean(beta_1 * logistic.pdf(beta_0 + beta_1 * mtcars["mpg"]))
 ```
 
@@ -327,18 +364,20 @@
 `newdata` accepts data frames like this:
 
 ``` python
 pre = predictions(mod, newdata = mtcars.tail(2))
 print(pre)
 ```
 
-    | rowid | estimate | std_error | statistic | … | vs  | am  | gear | carb |
-    |-------|----------|-----------|-----------|---|-----|-----|------|------|
-    | 0     | 0.119402 | 0.077817  | 1.534391  | … | 0   | 1   | 5    | 8    |
-    | 1     | 0.49172  | 0.119614  | 4.110899  | … | 1   | 1   | 4    | 2    |
+    | Estimate | Std.Error | z    | P(>|z|)  | S    | 2.5%    | 97.5% |
+    |----------|-----------|------|----------|------|---------|-------|
+    | 0.119    | 0.0778    | 1.53 | 0.136    | 2.88 | -0.0396 | 0.278 |
+    | 0.492    | 0.12      | 4.11 | 0.000281 | 11.8 | 0.247   | 0.736 |
+
+    Columns: rowid, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 The [`datagrid` function gives us a powerful way to define a grid of
 predictors.](https://vincentarelbundock.github.io/marginaleffects/reference/datagrid.html)
 All the variables not mentioned explicitly in `datagrid()` are fixed to
 their mean or mode:
 
 ``` python
@@ -348,20 +387,22 @@
     newdata = mtcars,
     am = [0, 1],
     wt = [mtcars["wt"].max(), mtcars["wt"].min()]))
 
 print(pre)
 ```
 
-    | rowid | estimate | std_error | statistic | … | qsec     | vs     | gear   | carb   |
-    |-------|----------|-----------|-----------|---|----------|--------|--------|--------|
-    | 0     | 0.3929   | 0.108367  | 3.625643  | … | 17.84875 | 0.4375 | 3.6875 | 2.8125 |
-    | 1     | 0.3929   | 0.108367  | 3.625643  | … | 17.84875 | 0.4375 | 3.6875 | 2.8125 |
-    | 2     | 0.3929   | 0.108367  | 3.625643  | … | 17.84875 | 0.4375 | 3.6875 | 2.8125 |
-    | 3     | 0.3929   | 0.108367  | 3.625643  | … | 17.84875 | 0.4375 | 3.6875 | 2.8125 |
+    | Estimate | Std.Error | z    | P(>|z|) | S    | 2.5%  | 97.5% |
+    |----------|-----------|------|---------|------|-------|-------|
+    | 0.393    | 0.108     | 3.63 | 0.00106 | 9.89 | 0.172 | 0.614 |
+    | 0.393    | 0.108     | 3.63 | 0.00106 | 9.89 | 0.172 | 0.614 |
+    | 0.393    | 0.108     | 3.63 | 0.00106 | 9.89 | 0.172 | 0.614 |
+    | 0.393    | 0.108     | 3.63 | 0.00106 | 9.89 | 0.172 | 0.614 |
+
+    Columns: rowid, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, am, wt, , mpg, cyl, disp, hp, drat, qsec, vs, gear, carb
 
 ## Averaging
 
 Since predictions, comparisons, and slopes are conditional quantities,
 they can be a bit unwieldy. Often, it can be useful to report a
 one-number summary instead of one estimate per observation. Instead of
 presenting “conditional” estimates, some methodologists recommend
@@ -380,17 +421,19 @@
 predicted outcome in the `mtcars` dataset:
 
 ``` python
 pre = avg_predictions(mod)
 print(pre)
 ```
 
-    | estimate | std_error | statistic | p_value  | s_value   | conf_low | conf_high |
-    |----------|-----------|-----------|----------|-----------|----------|-----------|
-    | 0.40625  | 0.068786  | 5.906026  | 0.000002 | 19.072686 | 0.265771 | 0.546729  |
+    | Estimate | Std.Error | z    | P(>|z|)  | S    | 2.5%  | 97.5% |
+    |----------|-----------|------|----------|------|-------|-------|
+    | 0.406    | 0.0688    | 5.91 | 1.81e-06 | 19.1 | 0.266 | 0.547 |
+
+    Columns: estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 This is equivalent to manual computation by:
 
 ``` python
 np.mean(mod.predict())
 ```
 
@@ -400,18 +443,20 @@
 allows us to marginalize within sub-groups of the data. For example,
 
 ``` python
 cmp = avg_comparisons(mod, by = "am")
 print(cmp)
 ```
 
-    | am  | term | contrast | estimate | … | p_value   | s_value   | conf_low | conf_high |
-    |-----|------|----------|----------|---|-----------|-----------|----------|-----------|
-    | 1   | mpg  | +1       | 0.044926 | … | 1.4198e-7 | 22.747797 | 0.031486 | 0.058365  |
-    | 0   | mpg  | +1       | 0.04751  | … | 0.000284  | 11.779712 | 0.023884 | 0.071135  |
+    | am | Term | Contrast | Estimate | … | P(>|z|)  | S    | 2.5%   | 97.5%  |
+    |----|------|----------|----------|---|----------|------|--------|--------|
+    | 1  | mpg  | +1       | 0.0449   | … | 1.44e-07 | 22.7 | 0.0315 | 0.0584 |
+    | 0  | mpg  | +1       | 0.0475   | … | 0.000285 | 11.8 | 0.0239 | 0.0711 |
+
+    Columns: am, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 Marginal Means are a special case of predictions, which are marginalized
 (or averaged) across a balanced grid of categorical predictors. To
 illustrate, we estimate a new model with categorical predictors:
 
 ``` python
 dat = mtcars \
@@ -438,21 +483,22 @@
 ```
 
 ``` python
 cmp = avg_comparisons(mod_cat)
 print(cmp)
 ```
 
-    | term | contrast     | estimate  | std_error | … | p_value  | s_value  | conf_low  | conf_high |
-    |------|--------------|-----------|-----------|---|----------|----------|-----------|-----------|
-    | hp   | +1           | -0.044244 | 0.014576  | … | 0.005266 | 7.569022 | -0.074151 | -0.014337 |
-    | am   | mean(True) - | 4.157856  | 1.25655   | … | 0.00266  | 8.554463 | 1.579629  | 6.736084  |
-    |      | mean(False)  |           |           |   |          |          |           |           |
-    | cyl  | 6 - 4        | -3.924578 | 1.537515  | … | 0.016663 | 5.907182 | -7.079298 | -0.769859 |
-    | cyl  | 8 - 4        | -3.533414 | 2.502788  | … | 0.169433 | 2.561213 | -8.668711 | 1.601883  |
+    | Term | Contrast                 | Estimate | Std.Error | … | P(>|z|) | S    | 2.5%    | 97.5%   |
+    |------|--------------------------|----------|-----------|---|---------|------|---------|---------|
+    | hp   | +1                       | -0.0442  | 0.0146    | … | 0.00527 | 7.57 | -0.0742 | -0.0143 |
+    | cyl  | 6 - 4                    | -3.92    | 1.54      | … | 0.0167  | 5.91 | -7.08   | -0.77   |
+    | cyl  | 8 - 4                    | -3.53    | 2.5       | … | 0.169   | 2.56 | -8.67   | 1.6     |
+    | am   | mean(True) - mean(False) | 4.16     | 1.26      | … | 0.00266 | 8.55 | 1.58    | 6.74    |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 ## Hypothesis and equivalence tests
 
 The `hypotheses()` function and the `hypothesis` argument can be used to
 conduct linear and non-linear hypothesis tests on model coefficients, or
 on any of the quantities computed by the functions introduced above.
 
@@ -490,27 +536,32 @@
 cmp = comparisons(
   mod,
   variables = "drat",
   newdata = datagrid(newdata = mtcars, qsec = range(mtcars["qsec"])))
 print(cmp)
 ```
 
-    | rowid | term | contrast | estimate  | … | vs     | am      | gear   | carb   |
-    |-------|------|----------|-----------|---|--------|---------|--------|--------|
-    | 0     | drat | +1       | 10.241374 | … | 0.4375 | 0.40625 | 3.6875 | 2.8125 |
-    | 1     | drat | +1       | 5.223926  | … | 0.4375 | 0.40625 | 3.6875 | 2.8125 |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S    | 2.5%   | 97.5% |
+    |------|----------|----------|-----------|---|---------|------|--------|-------|
+    | drat | +1       | 10.2     | 5.16      | … | 0.0571  | 4.13 | -0.331 | 20.8  |
+    | drat | +1       | 5.22     | 3.79      | … | 0.179   | 2.48 | -2.54  | 13    |
+
+    Columns: rowid, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, predicted, predicted_lo, predicted_hi, qsec, , mpg, cyl, disp, hp, drat, wt, vs, am, gear, carb
 
 Are these two contrasts significantly different from one another? To
 test this, we can use the `hypothesis` argument:
 
 ``` python
 cmp = comparisons(
   mod,
   hypothesis = "b1 = b2",
   variables = "drat",
   newdata = datagrid(newdata = mtcars, qsec = range(mtcars["qsec"])))
 print(cmp)
 ```
 
-    | term  | estimate | std_error | statistic | p_value  | s_value  | conf_low   | conf_high |
-    |-------|----------|-----------|-----------|----------|----------|------------|-----------|
-    | b1=b2 | 5.017448 | 8.519298  | 0.588951  | 0.560616 | 0.834915 | -12.433542 | 22.468439 |
+    | Term  | Estimate | Std.Error | z     | P(>|z|) | S     | 2.5%  | 97.5% |
+    |-------|----------|-----------|-------|---------|-------|-------|-------|
+    | b1=b2 | 5.02     | 8.52      | 0.589 | 0.561   | 0.835 | -12.4 | 22.5  |
+
+    Columns: term, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
+
```

### Comparing `marginaleffects-0.0.2/marginaleffects/by.py` & `marginaleffects-0.0.3/marginaleffects/by.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.2/marginaleffects/comparisons.py` & `marginaleffects-0.0.3/marginaleffects/comparisons.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 from .estimands import estimands
 from .hypothesis import get_hypothesis
 from .predictions import get_predictions
 from .sanity import sanitize_newdata, sanitize_variables, sanitize_vcov
 from .transform import get_transform
 from .uncertainty import get_jacobian, get_se, get_z_p_ci
 from .utils import get_pad, sort_columns, upcast
+from .classes import MarginaleffectsDataFrame
 
 
 def comparisons(
     model,
     variables=None,
     newdata=None,
     comparison="difference",
     vcov=True,
-    conf_int=0.95,
+    conf_level=0.95,
     by=False,
     wts=None,
     hypothesis=None,
     equivalence=None,
     transform=None,
     eps=1e-4,
 ):
@@ -252,43 +253,45 @@
 
     out = outer(model.params.to_numpy())
 
     if vcov is not None and vcov is not False:
         J = get_jacobian(func=outer, coefs=model.params.to_numpy())
         se = get_se(J, V)
         out = out.with_columns(pl.Series(se).alias("std_error"))
-        out = get_z_p_ci(out, model, conf_int=conf_int)
+        out = get_z_p_ci(out, model, conf_level=conf_level)
 
     out = get_transform(out, transform=transform)
     out = get_equivalence(out, equivalence=equivalence, df=np.inf)
     out = sort_columns(out, by=by)
+
+    out = MarginaleffectsDataFrame(out, by=by, conf_level=conf_level)
     return out
 
 
 def avg_comparisons(
     model,
     variables=None,
     newdata=None,
     comparison="difference",
     vcov=True,
-    conf_int=0.95,
+    conf_level=0.95,
     by=True,
     wts=None,
     hypothesis=None,
     equivalence=None,
     transform=None,
     eps=1e-4,
 ):
     out = comparisons(
         model=model,
         variables=variables,
         newdata=newdata,
         comparison=comparison,
         vcov=vcov,
-        conf_int=conf_int,
+        conf_level=conf_level,
         by=by,
         wts=wts,
         hypothesis=hypothesis,
         equivalence=equivalence,
         transform=transform,
         eps=eps,
     )
```

### Comparing `marginaleffects-0.0.2/marginaleffects/datagrid.py` & `marginaleffects-0.0.3/marginaleffects/datagrid.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.2/marginaleffects/equivalence.py` & `marginaleffects-0.0.3/marginaleffects/equivalence.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.2/marginaleffects/estimands.py` & `marginaleffects-0.0.3/marginaleffects/estimands.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.2/marginaleffects/hypotheses.py` & `marginaleffects-0.0.3/marginaleffects/hypotheses.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 from .hypothesis import get_hypothesis
 from .sanity import sanitize_vcov
 from .uncertainty import get_jacobian, get_se, get_z_p_ci
 from .utils import sort_columns
 
 
-def hypotheses(model, hypothesis=None, conf_int=0.95, vcov=True):
+def hypotheses(model, hypothesis=None, conf_level=0.95, vcov=True):
     # sanity checks
     V = sanitize_vcov(vcov, model)
 
     # estimands
     def fun(x):
         out = pl.DataFrame({"estimate": x})
         out = get_hypothesis(out, hypothesis=hypothesis)
         return out
 
     out = fun(np.array(model.params))
     if vcov is not None:
         J = get_jacobian(fun, model.params.to_numpy())
         se = get_se(J, V)
         out = out.with_columns(pl.Series(se).alias("std_error"))
-        out = get_z_p_ci(out, model, conf_int=conf_int)
+        out = get_z_p_ci(out, model, conf_level=conf_level)
     out = sort_columns(out, by=None)
     return out
```

### Comparing `marginaleffects-0.0.2/marginaleffects/hypothesis.py` & `marginaleffects-0.0.3/marginaleffects/hypothesis.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.2/marginaleffects/predictions.py` & `marginaleffects-0.0.3/marginaleffects/predictions.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .by import get_by
 from .equivalence import get_equivalence
 from .hypothesis import get_hypothesis
 from .sanity import sanitize_newdata, sanitize_vcov
 from .transform import get_transform
 from .uncertainty import get_jacobian, get_se, get_z_p_ci
 from .utils import sort_columns
+from .classes import MarginaleffectsDataFrame
 
 
 def get_predictions(model, params, newdata: pl.DataFrame):
     if isinstance(newdata, np.ndarray):
         exog = newdata
     else:
         y, exog = patsy.dmatrices(model.model.formula, newdata.to_pandas())
@@ -33,15 +34,15 @@
         )
     p = p.with_columns(pl.col("rowid").cast(pl.Int32))
     return p
 
 
 def predictions(
     model,
-    conf_int=0.95,
+    conf_level=0.95,
     vcov=True,
     by=False,
     newdata=None,
     hypothesis=None,
     equivalence=None,
     transform=None,
     wts=None,
@@ -104,35 +105,37 @@
         return out
 
     out = fun(model.params)
     if vcov is not None:
         J = get_jacobian(fun, model.params)
         se = get_se(J, V)
         out = out.with_columns(pl.Series(se).alias("std_error"))
-        out = get_z_p_ci(out, model, conf_int=conf_int)
+        out = get_z_p_ci(out, model, conf_level=conf_level)
     out = get_transform(out, transform=transform)
     out = get_equivalence(out, equivalence=equivalence)
     out = sort_columns(out, by=by)
+
+    out = MarginaleffectsDataFrame(out, by=by, conf_level=conf_level)
     return out
 
 
 def avg_predictions(
     model,
-    conf_int=0.95,
+    conf_level=0.95,
     vcov=True,
     by=True,
     newdata=None,
     hypothesis=None,
     equivalence=None,
     transform=None,
     wts=None,
 ):
     out = predictions(
         model=model,
-        conf_int=conf_int,
+        conf_level=conf_level,
         vcov=vcov,
         by=by,
         newdata=newdata,
         hypothesis=hypothesis,
         equivalence=equivalence,
         transform=transform,
         wts=wts,
```

### Comparing `marginaleffects-0.0.2/marginaleffects/sanity.py` & `marginaleffects-0.0.3/marginaleffects/sanity.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,24 +47,24 @@
     elif isinstance(newdata, str) and newdata == "median":
         out = datagrid(newdata=modeldata, FUN_numeric=lambda x: x.median())
 
     elif isinstance(newdata, pd.DataFrame):
         out = pl.from_pandas(newdata)
         
     else:
-        raise ValueError("No values for newdata.")
+        out = newdata
 
-    if "rowid" in out.columns:
-        raise ValueError(
-            "The newdata has a column named 'rowid', which is not allowed."
-        )
-    else:
-        out = out.with_columns(
-            pl.Series(range(out.height), dtype=pl.Int32).alias("rowid")
-        )
+    # if "rowid" in out.columns:
+    #     raise ValueError(
+    #         "The newdata has a column named 'rowid', which is not allowed."
+    #     )
+    # else:
+    out = out.with_columns(
+        pl.Series(range(out.height), dtype=pl.Int32).alias("rowid")
+    )
 
     if wts is not None:
         if (isinstance(wts, str) is False) or (wts not in out.columns):
             raise ValueError(f"`newdata` does not have a column named '{wts}'.")
 
     xnames = get_variables_names(variables=None, model=model, newdata=out)
     ynames = model.model.data.ynames
```

### Comparing `marginaleffects-0.0.2/marginaleffects/slopes.py` & `marginaleffects-0.0.3/marginaleffects/slopes.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def slopes(
     model,
     variables=None,
     newdata=None,
     slope="dydx",
     vcov=True,
-    conf_int=0.95,
+    conf_level=0.95,
     by=False,
     hypothesis=None,
     equivalence=None,
     wts=None,
     eps=1e-4,
 ):
     assert isinstance(eps, float)
@@ -21,15 +21,15 @@
 
     out = comparisons(
         model=model,
         variables=variables,
         newdata=newdata,
         comparison=slope,
         vcov=vcov,
-        conf_int=conf_int,
+        conf_level=conf_level,
         by=by,
         hypothesis=hypothesis,
         equivalence=equivalence,
         wts=wts,
         eps=eps,
     )
     return out
@@ -37,30 +37,30 @@
 
 def avg_slopes(
     model,
     variables=None,
     newdata=None,
     slope="dydx",
     vcov=True,
-    conf_int=0.95,
+    conf_level=0.95,
     by=True,
     wts=None,
     hypothesis=None,
     equivalence=None,
     eps=1e-4,
 ):
     if slope not in ["dydx", "eyex", "eydx", "dyex"]:
         raise ValueError("slope must be one of 'dydx', 'eyex', 'eydx', 'dyex'")
     out = slopes(
         model=model,
         variables=variables,
         newdata=newdata,
         slope=slope,
         vcov=vcov,
-        conf_int=conf_int,
+        conf_level=conf_level,
         by=by,
         wts=wts,
         hypothesis=hypothesis,
         equivalence=equivalence,
         eps=eps,
     )
```

### Comparing `marginaleffects-0.0.2/marginaleffects/uncertainty.py` & `marginaleffects-0.0.3/marginaleffects/uncertainty.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 
 
 def get_se(J, V):
     se = np.sqrt(np.sum((J @ V) * J, axis=1))
     return se
 
 
-def get_z_p_ci(df, model, conf_int):
+def get_z_p_ci(df, model, conf_level):
     if "std_error" not in df.columns:
         return df
     df = df.with_columns((pl.col("estimate") / pl.col("std_error")).alias("statistic"))
     if hasattr(model, "df_resid") and isinstance(model.df_resid, float):
         dof = model.df_resid
     else:
         dof = np.Inf
-    critical_value = stats.t.ppf((1 + conf_int) / 2, dof)
+    critical_value = stats.t.ppf((1 + conf_level) / 2, dof)
 
     df = df.with_columns(
         (pl.col("estimate") - critical_value * pl.col("std_error")).alias("conf_low")
     )
     df = df.with_columns(
         (pl.col("estimate") + critical_value * pl.col("std_error")).alias("conf_high")
     )
```

### Comparing `marginaleffects-0.0.2/marginaleffects/utils.py` & `marginaleffects-0.0.3/marginaleffects/utils.py`

 * *Files identical despite different names*

### Comparing `marginaleffects-0.0.2/pyproject.toml` & `marginaleffects-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marginaleffects"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Vincent Arel-Bundock <vincent.arel-bundock@umontreal.ca>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 pandas = "^2.0.2"
```

### Comparing `marginaleffects-0.0.2/PKG-INFO` & `marginaleffects-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: marginaleffects
-Version: 0.0.2
-Summary: 
-Author: Vincent Arel-Bundock
-Author-email: vincent.arel-bundock@umontreal.ca
-Requires-Python: >=3.9,<3.13
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.25.0,<2.0.0)
-Requires-Dist: pandas (>=2.0.2,<3.0.0)
-Requires-Dist: polars (>=0.18.3,<0.19.0)
-Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
-Requires-Dist: scipy (>1.10.0)
-Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
-Description-Content-Type: text/markdown
-
 # `marginaleffects` for Python
 
 The `marginaleffects` package allows `Python` users to compute and plot
 three principal quantities of interest: (1) predictions, (2)
 comparisons, and (3) slopes. In addition, the package includes a
 convenience function to compute a fourth estimand, “marginal means”,
 which is a special case of averaged predictions. `marginaleffects` can
@@ -116,16 +97,16 @@
 ```
 
                                 OLS Regression Results                            
     ==============================================================================
     Dep. Variable:                    mpg   R-squared:                       0.896
     Model:                            OLS   Adj. R-squared:                  0.866
     Method:                 Least Squares   F-statistic:                     29.55
-    Date:                Sun, 02 Jul 2023   Prob (F-statistic):           2.60e-10
-    Time:                        21:01:20   Log-Likelihood:                -66.158
+    Date:                Mon, 24 Jul 2023   Prob (F-statistic):           2.60e-10
+    Time:                        18:11:21   Log-Likelihood:                -66.158
     No. Observations:                  32   AIC:                             148.3
     Df Residuals:                      24   BIC:                             160.0
     Df Model:                           7                                         
     Covariance Type:            nonrobust                                         
     ==============================================================================
                      coef    std err          t      P>|t|      [0.025      0.975]
     ------------------------------------------------------------------------------
@@ -160,21 +141,23 @@
 pre = predictions(mod)
 
 pre.shape
 
 print(pre.head())
 ```
 
-    | rowid | estimate  | std_error | statistic | … | vs  | am  | gear | carb |
-    |-------|-----------|-----------|-----------|---|-----|-----|------|------|
-    | 0     | 22.488569 | 0.884149  | 25.43528  | … | 0   | 1   | 4    | 4    |
-    | 1     | 20.801859 | 1.194205  | 17.419002 | … | 0   | 1   | 4    | 4    |
-    | 2     | 25.264652 | 0.708531  | 35.657806 | … | 1   | 1   | 4    | 1    |
-    | 3     | 20.255492 | 0.704464  | 28.753051 | … | 1   | 0   | 3    | 1    |
-    | 4     | 16.997817 | 0.711866  | 23.877839 | … | 0   | 0   | 3    | 2    |
+    | Estimate | Std.Error | z    | P(>|z|) | S    | [    | ]    |
+    |----------|-----------|------|---------|------|------|------|
+    | 22.5     | 0.884     | 25.4 | 0       | inf  | 20.7 | 24.3 |
+    | 20.8     | 1.19      | 17.4 | 4e-15   | 47.8 | 18.3 | 23.3 |
+    | 25.3     | 0.709     | 35.7 | 0       | inf  | 23.8 | 26.7 |
+    | 20.3     | 0.704     | 28.8 | 0       | inf  | 18.8 | 21.7 |
+    | 17       | 0.712     | 23.9 | 0       | inf  | 15.5 | 18.5 |
+
+    Columns: rowid, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 #### Comparisons: Differences, Ratios, Log-Odds, Lift, etc.
 
 Now, we use the `comparisons()` function to compute the difference in
 predicted outcome when each of the predictors is incremented by 1 unit
 (one predictor at a time, holding all others constant). Once again,
 comparisons are unit-level quantities. And since there are 3 predictors
@@ -184,79 +167,87 @@
 cmp = comparisons(mod)
 
 cmp.shape
 
 print(cmp.head())
 ```
 
-    | rowid | term | contrast | estimate  | … | vs  | am  | gear | carb |
-    |-------|------|----------|-----------|---|-----|-----|------|------|
-    | 0     | hp   | +1       | -0.036906 | … | 0   | 1   | 4    | 4    |
-    | 1     | hp   | +1       | -0.028689 | … | 0   | 1   | 4    | 4    |
-    | 2     | hp   | +1       | -0.046572 | … | 1   | 1   | 4    | 1    |
-    | 3     | hp   | +1       | -0.042271 | … | 1   | 0   | 3    | 1    |
-    | 4     | hp   | +1       | -0.039018 | … | 0   | 0   | 3    | 2    |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S    | [       | ]       |
+    |------|----------|----------|-----------|---|---------|------|---------|---------|
+    | hp   | +1       | -0.0369  | 0.0185    | … | 0.0575  | 4.12 | -0.0751 | 0.00128 |
+    | hp   | +1       | -0.0287  | 0.0156    | … | 0.0788  | 3.67 | -0.0609 | 0.00357 |
+    | hp   | +1       | -0.0466  | 0.0226    | … | 0.0502  | 4.32 | -0.0932 | 4.6e-05 |
+    | hp   | +1       | -0.0423  | 0.0133    | … | 0.00401 | 7.96 | -0.0697 | -0.0149 |
+    | hp   | +1       | -0.039   | 0.0134    | … | 0.00769 | 7.02 | -0.0667 | -0.0113 |
+
+    Columns: rowid, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, predicted, predicted_lo, predicted_hi, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 The `comparisons()` function allows customized queries. For example,
 what happens to the predicted outcome when the `hp` variable increases
 from 100 to 120?
 
 ``` python
 cmp = comparisons(mod, variables = {"hp": [120, 100]})
 print(cmp)
 ```
 
-    | rowid | term | contrast  | estimate | … | vs  | am  | gear | carb |
-    |-------|------|-----------|----------|---|-----|-----|------|------|
-    | 0     | hp   | 100 - 120 | 0.738111 | … | 0   | 1   | 4    | 4    |
-    | 1     | hp   | 100 - 120 | 0.573787 | … | 0   | 1   | 4    | 4    |
-    | 2     | hp   | 100 - 120 | 0.931433 | … | 1   | 1   | 4    | 1    |
-    | 3     | hp   | 100 - 120 | 0.845426 | … | 1   | 0   | 3    | 1    |
-    | …     | …    | …         | …        | … | …   | …   | …    | …    |
-    | 28    | hp   | 100 - 120 | 0.383687 | … | 0   | 1   | 5    | 4    |
-    | 29    | hp   | 100 - 120 | 0.64145  | … | 0   | 1   | 5    | 6    |
-    | 30    | hp   | 100 - 120 | 0.125924 | … | 0   | 1   | 5    | 8    |
-    | 31    | hp   | 100 - 120 | 0.635006 | … | 1   | 1   | 4    | 2    |
+    | Term | Contrast  | Estimate | Std.Error | … | P(>|z|) | S     | 2.5%      | 97.5% |
+    |------|-----------|----------|-----------|---|---------|-------|-----------|-------|
+    | hp   | 100 - 120 | 0.738    | 0.37      | … | 0.0576  | 4.12  | -0.0256   | 1.5   |
+    | hp   | 100 - 120 | 0.574    | 0.313     | … | 0.0788  | 3.67  | -0.0713   | 1.22  |
+    | hp   | 100 - 120 | 0.931    | 0.452     | … | 0.0502  | 4.32  | -0.000918 | 1.86  |
+    | hp   | 100 - 120 | 0.845    | 0.266     | … | 0.00401 | 7.96  | 0.297     | 1.39  |
+    | …    | …         | …        | …         | … | …       | …     | …         | …     |
+    | hp   | 100 - 120 | 0.384    | 0.27      | … | 0.168   | 2.57  | -0.173    | 0.941 |
+    | hp   | 100 - 120 | 0.641    | 0.334     | … | 0.0671  | 3.9   | -0.0488   | 1.33  |
+    | hp   | 100 - 120 | 0.126    | 0.272     | … | 0.648   | 0.626 | -0.436    | 0.688 |
+    | hp   | 100 - 120 | 0.635    | 0.332     | … | 0.068   | 3.88  | -0.0507   | 1.32  |
+
+    Columns: rowid, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, predicted, predicted_lo, predicted_hi, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 What happens to the predicted outcome when the `wt` variable increases
 by 1 standard deviation about its mean?
 
 ``` python
 cmp = comparisons(mod, variables = {"hp": "sd"})
 print(cmp)
 ```
 
-    | rowid | term | contrast           | estimate  | … | vs  | am  | gear | carb |
-    |-------|------|--------------------|-----------|---|-----|-----|------|------|
-    | 0     | hp   | +68.56286848932059 | -2.530351 | … | 0   | 1   | 4    | 4    |
-    | 1     | hp   | +68.56286848932059 | -1.967025 | … | 0   | 1   | 4    | 4    |
-    | 2     | hp   | +68.56286848932059 | -3.193087 | … | 1   | 1   | 4    | 1    |
-    | 3     | hp   | +68.56286848932059 | -2.89824  | … | 1   | 0   | 3    | 1    |
-    | …     | …    | …                  | …         | … | …   | …   | …    | …    |
-    | 28    | hp   | +68.56286848932059 | -1.315334 | … | 0   | 1   | 5    | 4    |
-    | 29    | hp   | +68.56286848932059 | -2.198983 | … | 0   | 1   | 5    | 6    |
-    | 30    | hp   | +68.56286848932059 | -0.431686 | … | 0   | 1   | 5    | 8    |
-    | 31    | hp   | +68.56286848932059 | -2.176891 | … | 1   | 1   | 4    | 2    |
+    | Term | Contrast           | Estimate | Std.Error | … | P(>|z|) | S     | 2.5%  | 97.5%   |
+    |------|--------------------|----------|-----------|---|---------|-------|-------|---------|
+    | hp   | +68.56286848932059 | -2.53    | 1.27      | … | 0.0576  | 4.12  | -5.15 | 0.0878  |
+    | hp   | +68.56286848932059 | -1.97    | 1.07      | … | 0.0788  | 3.67  | -4.18 | 0.245   |
+    | hp   | +68.56286848932059 | -3.19    | 1.55      | … | 0.0502  | 4.32  | -6.39 | 0.00315 |
+    | hp   | +68.56286848932059 | -2.9     | 0.911     | … | 0.00401 | 7.96  | -4.78 | -1.02   |
+    | …    | …                  | …        | …         | … | …       | …     | …     | …       |
+    | hp   | +68.56286848932059 | -1.32    | 0.925     | … | 0.168   | 2.57  | -3.22 | 0.594   |
+    | hp   | +68.56286848932059 | -2.2     | 1.15      | … | 0.0671  | 3.9   | -4.57 | 0.167   |
+    | hp   | +68.56286848932059 | -0.432   | 0.933     | … | 0.648   | 0.626 | -2.36 | 1.49    |
+    | hp   | +68.56286848932059 | -2.18    | 1.14      | … | 0.068   | 3.88  | -4.53 | 0.174   |
+
+    Columns: rowid, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, predicted, predicted_lo, predicted_hi, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 The `comparisons()` function also allows users to specify arbitrary
 functions of predictions, with the `comparison` argument. For example,
 what is the average ratio between predicted Miles per Gallon after an
 increase of 50 units in Horsepower?
 
 ``` python
 cmp = comparisons(
   mod,
   variables = {"hp": 50},
   comparison = "ratioavg")
 print(cmp)
 ```
 
-    | term | contrast | estimate | std_error | … | p_value | s_value | conf_low | conf_high |
-    |------|----------|----------|-----------|---|---------|---------|----------|-----------|
-    | hp   | +50      | 0.909534 | 0.029058  | … | 0.0     | inf     | 0.84956  | 0.969507  |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S   | 2.5% | 97.5% |
+    |------|----------|----------|-----------|---|---------|-----|------|-------|
+    | hp   | +50      | 0.91     | 0.0291    | … | 0       | inf | 0.85 | 0.97  |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 #### Slopes: Derivatives and elasticities
 
 Consider a logistic regression model with a single predictor:
 
 ``` python
 url = "https://vincentarelbundock.github.io/Rdatasets/csv/datasets/mtcars.csv"
@@ -273,17 +264,19 @@
 slope of the prediction function at `mpg = 24`?
 
 ``` python
 mfx = slopes(mod, newdata = datagrid(mpg = 24, newdata = mtcars))
 print(mfx)
 ```
 
-    | term | contrast | estimate | std_error | … | p_value  | s_value   | conf_low | conf_high |
-    |------|----------|----------|-----------|---|----------|-----------|----------|-----------|
-    | mpg  | dY/dX    | 0.066534 | 0.01779   | … | 0.000776 | 10.331677 | 0.030203 | 0.102866  |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|)  | S    | 2.5%   | 97.5% |
+    |------|----------|----------|-----------|---|----------|------|--------|-------|
+    | mpg  | dY/dX    | 0.0665   | 0.0178    | … | 0.000798 | 10.3 | 0.0301 | 0.103 |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 This is equivalent to the result we obtain by taking the analytical
 derivative using the chain rule:
 
 ``` python
 from scipy.stats import logistic
 beta_0 = mod.params.iloc[0]
@@ -298,37 +291,43 @@
 values:
 
 ``` python
 mfx = slopes(mod, newdata = "mean")
 print(mfx)
 ```
 
-    | term | contrast | estimate | std_error | … | p_value  | s_value  | conf_low | conf_high |
-    |------|----------|----------|-----------|---|----------|----------|----------|-----------|
-    | mpg  | dY/dX    | 0.073235 | 0.028289  | … | 0.014712 | 6.086849 | 0.015461 | 0.13101   |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S    | 2.5%   | 97.5% |
+    |------|----------|----------|-----------|---|---------|------|--------|-------|
+    | mpg  | dY/dX    | 0.0732   | 0.0283    | … | 0.0148  | 6.08 | 0.0154 | 0.131 |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 ``` python
 mfx = slopes(mod, newdata = "median")
 print(mfx)
 ```
 
-    | term | contrast | estimate | std_error | … | p_value  | s_value  | conf_low | conf_high |
-    |------|----------|----------|-----------|---|----------|----------|----------|-----------|
-    | mpg  | dY/dX    | 0.067875 | 0.025298  | … | 0.011754 | 6.410751 | 0.01621  | 0.119539  |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S    | 2.5%   | 97.5% |
+    |------|----------|----------|-----------|---|---------|------|--------|-------|
+    | mpg  | dY/dX    | 0.0679   | 0.0253    | … | 0.0118  | 6.41 | 0.0162 | 0.12  |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 We can also compute an “average slope” or “average marginaleffects”
 
 ``` python
 mfx = avg_slopes(mod)
 print(mfx)
 ```
 
-    | term | contrast    | estimate | std_error | … | p_value  | s_value   | conf_low | conf_high |
-    |------|-------------|----------|-----------|---|----------|-----------|----------|-----------|
-    | mpg  | mean(dY/dX) | 0.046486 | 0.008864  | … | 0.000012 | 16.384139 | 0.028382 | 0.06459   |
+    | Term | Contrast    | Estimate | Std.Error | … | P(>|z|)  | S    | 2.5%   | 97.5%  |
+    |------|-------------|----------|-----------|---|----------|------|--------|--------|
+    | mpg  | mean(dY/dX) | 0.0465   | 0.00886   | … | 1.16e-05 | 16.4 | 0.0284 | 0.0646 |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 Which again is equivalent to the analytical result:
 
 ``` python
 np.mean(beta_1 * logistic.pdf(beta_0 + beta_1 * mtcars["mpg"]))
 ```
 
@@ -346,18 +345,20 @@
 `newdata` accepts data frames like this:
 
 ``` python
 pre = predictions(mod, newdata = mtcars.tail(2))
 print(pre)
 ```
 
-    | rowid | estimate | std_error | statistic | … | vs  | am  | gear | carb |
-    |-------|----------|-----------|-----------|---|-----|-----|------|------|
-    | 0     | 0.119402 | 0.077817  | 1.534391  | … | 0   | 1   | 5    | 8    |
-    | 1     | 0.49172  | 0.119614  | 4.110899  | … | 1   | 1   | 4    | 2    |
+    | Estimate | Std.Error | z    | P(>|z|)  | S    | 2.5%    | 97.5% |
+    |----------|-----------|------|----------|------|---------|-------|
+    | 0.119    | 0.0778    | 1.53 | 0.136    | 2.88 | -0.0396 | 0.278 |
+    | 0.492    | 0.12      | 4.11 | 0.000281 | 11.8 | 0.247   | 0.736 |
+
+    Columns: rowid, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, , mpg, cyl, disp, hp, drat, wt, qsec, vs, am, gear, carb
 
 The [`datagrid` function gives us a powerful way to define a grid of
 predictors.](https://vincentarelbundock.github.io/marginaleffects/reference/datagrid.html)
 All the variables not mentioned explicitly in `datagrid()` are fixed to
 their mean or mode:
 
 ``` python
@@ -367,20 +368,22 @@
     newdata = mtcars,
     am = [0, 1],
     wt = [mtcars["wt"].max(), mtcars["wt"].min()]))
 
 print(pre)
 ```
 
-    | rowid | estimate | std_error | statistic | … | qsec     | vs     | gear   | carb   |
-    |-------|----------|-----------|-----------|---|----------|--------|--------|--------|
-    | 0     | 0.3929   | 0.108367  | 3.625643  | … | 17.84875 | 0.4375 | 3.6875 | 2.8125 |
-    | 1     | 0.3929   | 0.108367  | 3.625643  | … | 17.84875 | 0.4375 | 3.6875 | 2.8125 |
-    | 2     | 0.3929   | 0.108367  | 3.625643  | … | 17.84875 | 0.4375 | 3.6875 | 2.8125 |
-    | 3     | 0.3929   | 0.108367  | 3.625643  | … | 17.84875 | 0.4375 | 3.6875 | 2.8125 |
+    | Estimate | Std.Error | z    | P(>|z|) | S    | 2.5%  | 97.5% |
+    |----------|-----------|------|---------|------|-------|-------|
+    | 0.393    | 0.108     | 3.63 | 0.00106 | 9.89 | 0.172 | 0.614 |
+    | 0.393    | 0.108     | 3.63 | 0.00106 | 9.89 | 0.172 | 0.614 |
+    | 0.393    | 0.108     | 3.63 | 0.00106 | 9.89 | 0.172 | 0.614 |
+    | 0.393    | 0.108     | 3.63 | 0.00106 | 9.89 | 0.172 | 0.614 |
+
+    Columns: rowid, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, am, wt, , mpg, cyl, disp, hp, drat, qsec, vs, gear, carb
 
 ## Averaging
 
 Since predictions, comparisons, and slopes are conditional quantities,
 they can be a bit unwieldy. Often, it can be useful to report a
 one-number summary instead of one estimate per observation. Instead of
 presenting “conditional” estimates, some methodologists recommend
@@ -399,17 +402,19 @@
 predicted outcome in the `mtcars` dataset:
 
 ``` python
 pre = avg_predictions(mod)
 print(pre)
 ```
 
-    | estimate | std_error | statistic | p_value  | s_value   | conf_low | conf_high |
-    |----------|-----------|-----------|----------|-----------|----------|-----------|
-    | 0.40625  | 0.068786  | 5.906026  | 0.000002 | 19.072686 | 0.265771 | 0.546729  |
+    | Estimate | Std.Error | z    | P(>|z|)  | S    | 2.5%  | 97.5% |
+    |----------|-----------|------|----------|------|-------|-------|
+    | 0.406    | 0.0688    | 5.91 | 1.81e-06 | 19.1 | 0.266 | 0.547 |
+
+    Columns: estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 This is equivalent to manual computation by:
 
 ``` python
 np.mean(mod.predict())
 ```
 
@@ -419,18 +424,20 @@
 allows us to marginalize within sub-groups of the data. For example,
 
 ``` python
 cmp = avg_comparisons(mod, by = "am")
 print(cmp)
 ```
 
-    | am  | term | contrast | estimate | … | p_value   | s_value   | conf_low | conf_high |
-    |-----|------|----------|----------|---|-----------|-----------|----------|-----------|
-    | 1   | mpg  | +1       | 0.044926 | … | 1.4198e-7 | 22.747797 | 0.031486 | 0.058365  |
-    | 0   | mpg  | +1       | 0.04751  | … | 0.000284  | 11.779712 | 0.023884 | 0.071135  |
+    | am | Term | Contrast | Estimate | … | P(>|z|)  | S    | 2.5%   | 97.5%  |
+    |----|------|----------|----------|---|----------|------|--------|--------|
+    | 1  | mpg  | +1       | 0.0449   | … | 1.44e-07 | 22.7 | 0.0315 | 0.0584 |
+    | 0  | mpg  | +1       | 0.0475   | … | 0.000285 | 11.8 | 0.0239 | 0.0711 |
+
+    Columns: am, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 Marginal Means are a special case of predictions, which are marginalized
 (or averaged) across a balanced grid of categorical predictors. To
 illustrate, we estimate a new model with categorical predictors:
 
 ``` python
 dat = mtcars \
@@ -457,21 +464,22 @@
 ```
 
 ``` python
 cmp = avg_comparisons(mod_cat)
 print(cmp)
 ```
 
-    | term | contrast     | estimate  | std_error | … | p_value  | s_value  | conf_low  | conf_high |
-    |------|--------------|-----------|-----------|---|----------|----------|-----------|-----------|
-    | hp   | +1           | -0.044244 | 0.014576  | … | 0.005266 | 7.569022 | -0.074151 | -0.014337 |
-    | am   | mean(True) - | 4.157856  | 1.25655   | … | 0.00266  | 8.554463 | 1.579629  | 6.736084  |
-    |      | mean(False)  |           |           |   |          |          |           |           |
-    | cyl  | 6 - 4        | -3.924578 | 1.537515  | … | 0.016663 | 5.907182 | -7.079298 | -0.769859 |
-    | cyl  | 8 - 4        | -3.533414 | 2.502788  | … | 0.169433 | 2.561213 | -8.668711 | 1.601883  |
+    | Term | Contrast                 | Estimate | Std.Error | … | P(>|z|) | S    | 2.5%    | 97.5%   |
+    |------|--------------------------|----------|-----------|---|---------|------|---------|---------|
+    | hp   | +1                       | -0.0442  | 0.0146    | … | 0.00527 | 7.57 | -0.0742 | -0.0143 |
+    | cyl  | 6 - 4                    | -3.92    | 1.54      | … | 0.0167  | 5.91 | -7.08   | -0.77   |
+    | cyl  | 8 - 4                    | -3.53    | 2.5       | … | 0.169   | 2.56 | -8.67   | 1.6     |
+    | am   | mean(True) - mean(False) | 4.16     | 1.26      | … | 0.00266 | 8.55 | 1.58    | 6.74    |
+
+    Columns: term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
 
 ## Hypothesis and equivalence tests
 
 The `hypotheses()` function and the `hypothesis` argument can be used to
 conduct linear and non-linear hypothesis tests on model coefficients, or
 on any of the quantities computed by the functions introduced above.
 
@@ -509,28 +517,31 @@
 cmp = comparisons(
   mod,
   variables = "drat",
   newdata = datagrid(newdata = mtcars, qsec = range(mtcars["qsec"])))
 print(cmp)
 ```
 
-    | rowid | term | contrast | estimate  | … | vs     | am      | gear   | carb   |
-    |-------|------|----------|-----------|---|--------|---------|--------|--------|
-    | 0     | drat | +1       | 10.241374 | … | 0.4375 | 0.40625 | 3.6875 | 2.8125 |
-    | 1     | drat | +1       | 5.223926  | … | 0.4375 | 0.40625 | 3.6875 | 2.8125 |
+    | Term | Contrast | Estimate | Std.Error | … | P(>|z|) | S    | 2.5%   | 97.5% |
+    |------|----------|----------|-----------|---|---------|------|--------|-------|
+    | drat | +1       | 10.2     | 5.16      | … | 0.0571  | 4.13 | -0.331 | 20.8  |
+    | drat | +1       | 5.22     | 3.79      | … | 0.179   | 2.48 | -2.54  | 13    |
+
+    Columns: rowid, term, contrast, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high, predicted, predicted_lo, predicted_hi, qsec, , mpg, cyl, disp, hp, drat, wt, vs, am, gear, carb
 
 Are these two contrasts significantly different from one another? To
 test this, we can use the `hypothesis` argument:
 
 ``` python
 cmp = comparisons(
   mod,
   hypothesis = "b1 = b2",
   variables = "drat",
   newdata = datagrid(newdata = mtcars, qsec = range(mtcars["qsec"])))
 print(cmp)
 ```
 
-    | term  | estimate | std_error | statistic | p_value  | s_value  | conf_low   | conf_high |
-    |-------|----------|-----------|-----------|----------|----------|------------|-----------|
-    | b1=b2 | 5.017448 | 8.519298  | 0.588951  | 0.560616 | 0.834915 | -12.433542 | 22.468439 |
+    | Term  | Estimate | Std.Error | z     | P(>|z|) | S     | 2.5%  | 97.5% |
+    |-------|----------|-----------|-------|---------|-------|-------|-------|
+    | b1=b2 | 5.02     | 8.52      | 0.589 | 0.561   | 0.835 | -12.4 | 22.5  |
 
+    Columns: term, estimate, std_error, statistic, p_value, s_value, conf_low, conf_high
```

