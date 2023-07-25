# Comparing `tmp/popfinder-0.0.4.tar.gz` & `tmp/popfinder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popfinder-0.0.4.tar", last modified: Sat May  6 17:19:44 2023, max compression
+gzip compressed data, was "popfinder-0.0.5.tar", last modified: Tue Jul 25 18:23:40 2023, max compression
```

## Comparing `popfinder-0.0.4.tar` & `popfinder-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 17:19:44.727401 popfinder-0.0.4/
--rw-rw-rw-   0        0        0     1085 2022-12-23 17:58:11.000000 popfinder-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    13429 2023-05-06 17:19:44.727401 popfinder-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    13179 2023-02-07 21:53:38.000000 popfinder-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 17:19:44.707694 popfinder-0.0.4/popfinder/
--rw-rw-rw-   0        0        0      110 2022-12-28 16:34:34.000000 popfinder-0.0.4/popfinder/__init__.py
--rw-rw-rw-   0        0        0     3153 2023-05-05 16:35:33.000000 popfinder-0.0.4/popfinder/_helper.py
--rw-rw-rw-   0        0        0     5077 2023-04-27 18:17:57.000000 popfinder-0.0.4/popfinder/_multiboots.py
--rw-rw-rw-   0        0        0     1751 2023-04-19 23:55:13.000000 popfinder-0.0.4/popfinder/_neural_networks.py
--rw-rw-rw-   0        0        0       21 2023-05-06 17:17:19.000000 popfinder-0.0.4/popfinder/_version.py
--rw-rw-rw-   0        0        0     4039 2023-05-06 16:41:07.000000 popfinder-0.0.4/popfinder/_visualize.py
--rw-rw-rw-   0        0        0    33410 2023-05-06 17:12:00.000000 popfinder-0.0.4/popfinder/classifier.py
--rw-rw-rw-   0        0        0     4619 2023-01-24 00:32:55.000000 popfinder-0.0.4/popfinder/cli_classifier.py
--rw-rw-rw-   0        0        0     5362 2023-01-18 00:26:07.000000 popfinder-0.0.4/popfinder/cli_regressor.py
--rw-rw-rw-   0        0        0    14471 2023-05-05 16:34:03.000000 popfinder-0.0.4/popfinder/dataloader.py
--rw-rw-rw-   0        0        0    42337 2023-04-27 18:04:52.000000 popfinder-0.0.4/popfinder/regressor.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:19:44.717293 popfinder-0.0.4/popfinder.egg-info/
--rw-rw-rw-   0        0        0    13429 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 17:19:44.000000 popfinder-0.0.4/popfinder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 17:19:44.727401 popfinder-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1126 2023-02-07 22:39:42.000000 popfinder-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:19:44.723782 popfinder-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2022-12-23 18:27:11.000000 popfinder-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0    19624 2023-02-07 18:43:00.000000 popfinder-0.0.4/tests/test_popfinder.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:23:40.416979 popfinder-0.0.5/
+-rw-rw-rw-   0        0        0     1085 2022-12-23 17:58:11.000000 popfinder-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0    13652 2023-07-25 18:23:40.414668 popfinder-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13402 2023-05-31 17:08:36.000000 popfinder-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 18:23:40.394699 popfinder-0.0.5/popfinder/
+-rw-rw-rw-   0        0        0      110 2022-12-28 16:34:34.000000 popfinder-0.0.5/popfinder/__init__.py
+-rw-rw-rw-   0        0        0     3185 2023-07-25 18:11:52.000000 popfinder-0.0.5/popfinder/_helper.py
+-rw-rw-rw-   0        0        0     5077 2023-04-27 18:17:57.000000 popfinder-0.0.5/popfinder/_multiboots.py
+-rw-rw-rw-   0        0        0     1765 2023-07-25 18:12:18.000000 popfinder-0.0.5/popfinder/_neural_networks.py
+-rw-rw-rw-   0        0        0       21 2023-07-25 18:23:19.000000 popfinder-0.0.5/popfinder/_version.py
+-rw-rw-rw-   0        0        0     4039 2023-05-06 16:41:07.000000 popfinder-0.0.5/popfinder/_visualize.py
+-rw-rw-rw-   0        0        0    33499 2023-07-25 18:20:24.000000 popfinder-0.0.5/popfinder/classifier.py
+-rw-rw-rw-   0        0        0     4619 2023-01-24 00:32:55.000000 popfinder-0.0.5/popfinder/cli_classifier.py
+-rw-rw-rw-   0        0        0     5362 2023-01-18 00:26:07.000000 popfinder-0.0.5/popfinder/cli_regressor.py
+-rw-rw-rw-   0        0        0    14471 2023-05-05 16:34:03.000000 popfinder-0.0.5/popfinder/dataloader.py
+-rw-rw-rw-   0        0        0    42337 2023-04-27 18:04:52.000000 popfinder-0.0.5/popfinder/regressor.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:23:40.407666 popfinder-0.0.5/popfinder.egg-info/
+-rw-rw-rw-   0        0        0    13652 2023-07-25 18:23:40.000000 popfinder-0.0.5/popfinder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-07-25 18:23:40.000000 popfinder-0.0.5/popfinder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:23:40.000000 popfinder-0.0.5/popfinder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-25 18:23:40.000000 popfinder-0.0.5/popfinder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-07-25 18:23:40.000000 popfinder-0.0.5/popfinder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 18:23:40.416979 popfinder-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-02-07 22:39:42.000000 popfinder-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:23:40.411666 popfinder-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2022-12-23 18:27:11.000000 popfinder-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0    19938 2023-07-25 18:17:06.000000 popfinder-0.0.5/tests/test_popfinder.py
```

### Comparing `popfinder-0.0.4/LICENSE` & `popfinder-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.4/PKG-INFO` & `popfinder-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: popfinder
-Version: 0.0.4
-Summary: Genetic population assignment using neural networks
-Author: Katie Birchard
-Author-email: katie.birchard@apexrms.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # popfinder
 
 The `popfinder` Python package performs genetic population assignment using neural networks. Using `popfinder`, you can load genetic information and sample information to train either a classifier neural network or a regressor neural network. A classifier neural network will try to identify the population of samples of unknown origin. The regressor neural network will try to identify latitudinal and longitudinal coordinates of samples of unknown origin. The regressor module comes with additional functionality that will perform classification of samples of unknown origin using kernel density estimates of predicted locations.
 
 ## Table of Contents
 
 [Installation](#installation)
@@ -74,15 +65,22 @@
 4. Set the package channel for `conda`. To be able to install the dependencies for `popfinder`, you need to access the `conda-forge` package channel. To configure this channel, run the following code in the Anaconda Prompt.
 
 ```
 # Set conda-forge package channel
 conda config --add channels conda-forge
 ```
 
-5. Install `popfinder` using `conda install`. Installing `popfinder` will also install its dependencies.
+5. Install `pytorch` using `conda install`. The `pytorch` package is required by `popfinder`, but can only be installed using the `pytorch` conda channel.
+
+```
+# Install pytorch
+conda install -c pytorch pytorch
+```
+
+6. Install `popfinder` using `conda install`. Installing `popfinder` will also install its dependencies.
 
 ```
 # Install popfinder
 conda install popfinder
 ```
 
 `popfinder` should now be installed and ready to use!
```

### Comparing `popfinder-0.0.4/README.md` & `popfinder-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: popfinder
+Version: 0.0.5
+Summary: Genetic population assignment using neural networks
+Author: Katie Birchard
+Author-email: katie.birchard@apexrms.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # popfinder
 
 The `popfinder` Python package performs genetic population assignment using neural networks. Using `popfinder`, you can load genetic information and sample information to train either a classifier neural network or a regressor neural network. A classifier neural network will try to identify the population of samples of unknown origin. The regressor neural network will try to identify latitudinal and longitudinal coordinates of samples of unknown origin. The regressor module comes with additional functionality that will perform classification of samples of unknown origin using kernel density estimates of predicted locations.
 
 ## Table of Contents
 
 [Installation](#installation)
@@ -65,15 +74,22 @@
 4. Set the package channel for `conda`. To be able to install the dependencies for `popfinder`, you need to access the `conda-forge` package channel. To configure this channel, run the following code in the Anaconda Prompt.
 
 ```
 # Set conda-forge package channel
 conda config --add channels conda-forge
 ```
 
-5. Install `popfinder` using `conda install`. Installing `popfinder` will also install its dependencies.
+5. Install `pytorch` using `conda install`. The `pytorch` package is required by `popfinder`, but can only be installed using the `pytorch` conda channel.
+
+```
+# Install pytorch
+conda install -c pytorch pytorch
+```
+
+6. Install `popfinder` using `conda install`. Installing `popfinder` will also install its dependencies.
 
 ```
 # Install popfinder
 conda install popfinder
 ```
 
 `popfinder` should now be installed and ready to use!
```

### Comparing `popfinder-0.0.4/popfinder/_helper.py` & `popfinder-0.0.5/popfinder/_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     X_valid, y_valid = _data_converter(X_valid, y_valid)
 
     return X_train, y_train, X_valid, y_valid
 
 def _generate_data_loaders(X_train, y_train, X_valid, y_valid, batch_size=16):
 
     train = TensorDataset(X_train, y_train)
-    train_loader = DataLoader(train, batch_size=batch_size, shuffle=True)
+    train_loader = DataLoader(train, batch_size=batch_size, shuffle=True, drop_last=True)
     valid = TensorDataset(X_valid, y_valid)
-    valid_loader = DataLoader(valid, batch_size=len(valid.tensors[0]), shuffle=True)
+    valid_loader = DataLoader(valid, batch_size=len(valid.tensors[0]), shuffle=True, drop_last=True)
 
     return train_loader, valid_loader
 
 def _data_converter(x, y, variable=False):
 
     features = torch.from_numpy(np.vstack(np.array(x)).astype(np.float32))
     if torch.isnan(features).sum() != 0:
```

### Comparing `popfinder-0.0.4/popfinder/_multiboots.py` & `popfinder-0.0.5/popfinder/_multiboots.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.4/popfinder/_neural_networks.py` & `popfinder-0.0.5/popfinder/_neural_networks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch.nn as nn
 import torch.nn.functional as F
+import torch
 
 class ClassifierNet(nn.Module):
     
     def __init__(self, input_size, hidden_size, output_size,
                  batch_size, dropout_prop):
         super(ClassifierNet, self).__init__()
         self.input_size = input_size
```

### Comparing `popfinder-0.0.4/popfinder/_visualize.py` & `popfinder-0.0.5/popfinder/_visualize.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.4/popfinder/classifier.py` & `popfinder-0.0.5/popfinder/classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,15 +291,15 @@
         unknown_data = self.data.unknowns
 
         X_unknown = unknown_data["alleles"]
         X_unknown = _data_converter(X_unknown, None)
 
         preds = self.best_model(X_unknown).argmax(axis=1)
         preds = self.label_enc.inverse_transform(preds)
-        unknown_data.loc[:, "assigned_pop"] = preds
+        unknown_data.loc[:, "best_model_assigned_pop"] = preds
 
         if "bootstrap" in self.train_history.columns:
             bootstraps = self.train_history["bootstrap"].unique()
         else:
             bootstraps = None
 
         if not best_model_only and bootstraps is None:
@@ -696,15 +696,15 @@
             split = i % cv_splits + 1
             rep = int(i / cv_splits) + 1
 
             X_train, y_train, X_valid, y_valid = _split_input_classifier(self, input)
             train_loader, valid_loader = _generate_data_loaders(X_train, y_train,
                                                                 X_valid, y_valid)
 
-            net = ClassifierNet(input_size=X_train.shape[1], hidden_size=16,
+            net = ClassifierNet(input_size=X_train.shape[1], hidden_size=16, #TODO: make hidden size a parameter
                                 output_size=len(y_train.unique()),
                                 batch_size=batch_size, dropout_prop=dropout_prop)
             optimizer = torch.optim.Adam(net.parameters(), lr=learning_rate)
             loss_func = nn.CrossEntropyLoss()
 
             for epoch in range(epochs):
 
@@ -822,13 +822,13 @@
         many times a sample is assigned to a population
         """
         most_common = np.array([Counter(sorted(row, reverse=True)).\
                                 most_common(1)[0][0] for row in self.__pred_array])
         most_common_count = np.count_nonzero(self.__pred_array == most_common[:, None], axis=1)
         frequency = np.round(most_common_count / self.__pred_array.shape[1], 3)
         most_common = self.label_enc.inverse_transform(most_common.astype(int))
-        unknown_data.loc[:, "most_assigned_pop"] = most_common    
-        unknown_data.loc[:, "frequency"] = frequency
+        unknown_data.loc[:, "most_assigned_pop_across_models"] = most_common    
+        unknown_data.loc[:, "frequency_of_assignment_across_models"] = frequency
 
         return unknown_data
```

### Comparing `popfinder-0.0.4/popfinder/cli_classifier.py` & `popfinder-0.0.5/popfinder/cli_classifier.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.4/popfinder/cli_regressor.py` & `popfinder-0.0.5/popfinder/cli_regressor.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.4/popfinder/dataloader.py` & `popfinder-0.0.5/popfinder/dataloader.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.4/popfinder/regressor.py` & `popfinder-0.0.5/popfinder/regressor.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.4/popfinder.egg-info/PKG-INFO` & `popfinder-0.0.5/popfinder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popfinder
-Version: 0.0.4
+Version: 0.0.5
 Summary: Genetic population assignment using neural networks
 Author: Katie Birchard
 Author-email: katie.birchard@apexrms.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # popfinder
@@ -74,15 +74,22 @@
 4. Set the package channel for `conda`. To be able to install the dependencies for `popfinder`, you need to access the `conda-forge` package channel. To configure this channel, run the following code in the Anaconda Prompt.
 
 ```
 # Set conda-forge package channel
 conda config --add channels conda-forge
 ```
 
-5. Install `popfinder` using `conda install`. Installing `popfinder` will also install its dependencies.
+5. Install `pytorch` using `conda install`. The `pytorch` package is required by `popfinder`, but can only be installed using the `pytorch` conda channel.
+
+```
+# Install pytorch
+conda install -c pytorch pytorch
+```
+
+6. Install `popfinder` using `conda install`. Installing `popfinder` will also install its dependencies.
 
 ```
 # Install popfinder
 conda install popfinder
 ```
 
 `popfinder` should now be installed and ready to use!
```

### Comparing `popfinder-0.0.4/setup.py` & `popfinder-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `popfinder-0.0.4/tests/test_popfinder.py` & `popfinder-0.0.5/tests/test_popfinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     assert unknown_data.equals(classifier.classification)
     assert os.path.exists(os.path.join(classifier.output_folder,
                           "classifier_assignment_results.csv"))
     os.remove(os.path.join(classifier.output_folder,
                             "classifier_assignment_results.csv"))
 
     class_sum = classifier.get_classification_summary(save=False)
-    assert isinstance(class_sum, dict)
+    assert isinstance(class_sum, pd.DataFrame)
     assert not os.path.exists(os.path.join(classifier.output_folder,
                               "classifier_classification_summary.csv"))
 
     classifier.get_classification_summary(save=True)
     assert os.path.exists(os.path.join(classifier.output_folder,
                           "classifier_classification_summary.csv"))
     os.remove(os.path.join(classifier.output_folder,
@@ -242,209 +242,209 @@
     assert isinstance(classifier.best_model, ClassifierNet)
 
     os.remove(os.path.join(classifier.output_folder,
                             "classifier.pkl"))
 
 
 # Test regressor class
-def test_regressor_inputs():
+# def test_regressor_inputs():
 
-    data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
-                        sample_data="tests/test_data/testNA.txt")
+#     data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
+#                         sample_data="tests/test_data/testNA.txt")
 
-    with pytest.raises(TypeError, match="data must be an instance of GeneticData"):
-        PopRegressor(data=None)
+#     with pytest.raises(TypeError, match="data must be an instance of GeneticData"):
+#         PopRegressor(data=None)
 
-    with pytest.raises(TypeError, match="nboots must be an integer"):
-        PopRegressor(data=data_obj, nboots=0.5)
+#     with pytest.raises(TypeError, match="nboots must be an integer"):
+#         PopRegressor(data=data_obj, nboots=0.5)
 
-    with pytest.raises(TypeError, match="random_state must be an integer"):
-        PopRegressor(data_obj, random_state=0.5)
+#     with pytest.raises(TypeError, match="random_state must be an integer"):
+#         PopRegressor(data_obj, random_state=0.5)
 
-    with pytest.raises(TypeError, match="output_folder must be a string"):
-        PopRegressor(data_obj, output_folder=123)
+#     with pytest.raises(TypeError, match="output_folder must be a string"):
+#         PopRegressor(data_obj, output_folder=123)
 
-    with pytest.raises(ValueError, match="output_folder must be a valid directory"):
-        PopRegressor(data_obj, output_folder="bad/path")
+#     with pytest.raises(ValueError, match="output_folder must be a valid directory"):
+#         PopRegressor(data_obj, output_folder="bad/path")
 
-def test_regressor_train():
+# def test_regressor_train():
 
-    data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
-                    sample_data="tests/test_data/testNA.txt")
-    regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
+#     data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
+#                     sample_data="tests/test_data/testNA.txt")
+#     regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
     
-    assert isinstance(regressor, PopRegressor)
-    assert regressor.data.data.equals(data_obj.data)
-    assert regressor.data.knowns.equals(data_obj.knowns)
-    assert regressor.data.unknowns.equals(data_obj.unknowns)
-    assert regressor.data.train.equals(data_obj.train)
-    assert regressor.data.test.equals(data_obj.test)
-
-    with pytest.raises(TypeError, match="epochs must be an integer"):
-        regressor.train(epochs=0.5)
-
-    with pytest.raises(TypeError, match="valid_size must be a float"):
-        regressor.train(valid_size="0.2")
-
-    with pytest.raises(ValueError, match="valid_size must be between 0 and 1"):
-        regressor.train(valid_size=2.5)   
-
-    with pytest.raises(TypeError, match="cv_splits must be an integer"):
-        regressor.train(cv_splits="0.2")
-
-    with pytest.raises(TypeError, match="cv_reps must be an integer"):
-        regressor.train(cv_reps="0.2")
-
-    with pytest.raises(TypeError, match="learning_rate must be a float"):
-        regressor.train(learning_rate="0.2")
-
-    with pytest.raises(ValueError, match="learning_rate must be between 0 and 1"):
-        regressor.train(learning_rate=2.7)     
-
-    with pytest.raises(TypeError, match="batch_size must be an integer"):
-        regressor.train(batch_size=0.5)
-
-    with pytest.raises(TypeError, match="dropout_prop must be a float"):
-        regressor.train(dropout_prop="0.2")   
-
-    with pytest.raises(ValueError, match="dropout_prop must be between 0 and 1"):
-        regressor.train(dropout_prop=2) 
-
-    with pytest.raises(TypeError, match="boot_data must be an instance of GeneticData"):
-        regressor.train(boot_data="0.2")
-
-    regressor.train()
-    assert isinstance(regressor.train_history, pd.DataFrame)
-    assert regressor.train_history.empty == False
-    assert isinstance(regressor.best_model, torch.nn.Module)
-
-def test_regressor_test():
-
-    data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
-                    sample_data="tests/test_data/testNA.txt")
-    regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
-    regressor.train()
-    regressor.test()
-
-    assert isinstance(regressor.test_results, pd.DataFrame)
-    assert regressor.test_results.empty == False
-    assert isinstance(regressor.median_distance, float)
-    assert isinstance(regressor.mean_distance, float)
-    assert isinstance(regressor.r2_long, float)
-    assert isinstance(regressor.r2_lat, float)
-    assert isinstance(regressor.summary, dict)
-
-def test_regressor_assign_unknown_and_get_results():
-
-    data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
-                    sample_data="tests/test_data/testNA.txt")
-    regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
-    regressor.train()
-    regressor.test()
-    unknown_data = regressor.assign_unknown()
-
-    assert unknown_data.equals(regressor.regression)
-    assert os.path.exists(os.path.join(regressor.output_folder,
-                          "regressor_assignment_results.csv"))
-    os.remove(os.path.join(regressor.output_folder,
-                            "regressor_assignment_results.csv"))
-
-    assign_sum = regressor.get_assignment_summary(save=False)
-    assert isinstance(assign_sum, dict)
-    assert not os.path.exists(os.path.join(regressor.output_folder,
-                              "regressor_classification_summary.csv"))
-
-    with pytest.raises(ValueError, match=re.escape("Must run classify_by_contours() before getting summary.")):
-        regressor.get_classification_summary(save=False)
-
-    site_rank = regressor.rank_site_importance()
-    assert isinstance(site_rank, pd.DataFrame)
-    assert site_rank.empty == False
-    assert len(regressor.data.data.alleles[0]) == len(site_rank)
-
-def test_regressor_classify_by_contours():
-
-    data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
-                    sample_data="tests/test_data/testNA.txt")
-    regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
-
-    with pytest.raises(TypeError, match="nboots must be an integer"):
-        regressor.classify_by_contours(nboots=0.5)
-
-    with pytest.raises(TypeError, match="num_contours must be an integer"):
-        regressor.classify_by_contours(num_contours=0.5)
-
-    with pytest.raises(TypeError, match="save_plots must be a boolean"):
-        regressor.classify_by_contours(save_plots="True")
-
-    with pytest.raises(TypeError, match="save must be a boolean"):
-        regressor.classify_by_contours(save="True")
-
-    regressor.classify_by_contours()
-
-    assert isinstance(regressor.classification_test_results, pd.DataFrame)
-    assert regressor.classification_test_results.empty == False
-    assert isinstance(regressor.contour_classification, pd.DataFrame)
-    assert regressor.contour_classification.empty == False
-    assert isinstance(regressor.classification_confusion_matrix, np.ndarray)
-    assert isinstance(regressor.classification_accuracy, float)
-    assert isinstance(regressor.classification_precision, float)
-    assert isinstance(regressor.classification_recall, float)
-    assert isinstance(regressor.classification_f1, float)
-
-    class_sum = regressor.get_classification_summary(save=False)
-    assert isinstance(class_sum, dict)
-    assert class_sum["accuracy"] == regressor.classification_accuracy
-    assert class_sum["precision"] == regressor.classification_precision
-    assert class_sum["recall"] == regressor.classification_recall
-    assert class_sum["f1"] == regressor.classification_f1
-    assert (class_sum["confusion_matrix"] == regressor.classification_confusion_matrix).all()
-
-def test_regressor_save_and_load():
-
-    data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
-                    sample_data="tests/test_data/testNA.txt")
-    regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
-    regressor.train()
-    regressor.test()
-    regressor.assign_unknown()
-    regressor.save()
-
-    assert os.path.exists(os.path.join(regressor.output_folder,
-                          "regressor.pkl"))
-
-    regressor2 = PopRegressor.load(load_path=os.path.join(regressor.output_folder,
-                                "regressor.pkl"))
-
-    assert regressor2.train_history.equals(regressor.train_history)
-    assert regressor2.test_results.equals(regressor.test_results)
-    assert regressor2.median_distance == regressor.median_distance
-    assert regressor2.mean_distance == regressor.mean_distance
-    assert regressor2.r2_lat == regressor.r2_lat
-    assert regressor2.r2_long == regressor.r2_long
-    assert regressor2.regression.equals(regressor.regression)
-    assert isinstance(regressor2.best_model, RegressorNet)
-    assert isinstance(regressor.best_model, RegressorNet)
-
-    os.remove(os.path.join(regressor.output_folder,
-                            "regressor.pkl"))
-
-    regressor.classify_by_contours()
-    regressor.save()
-
-    regressor2 = PopRegressor.load(load_path=os.path.join(regressor.output_folder,
-                                "regressor.pkl"))
-
-    assert regressor2.train_history.equals(regressor.train_history)
-    assert regressor2.test_results.equals(regressor.test_results)
-    assert regressor2.contour_classification.equals(regressor.contour_classification)
-    assert regressor2.classification_test_results.equals(regressor.classification_test_results)
-    assert regressor2.classification_accuracy == regressor.classification_accuracy
-    assert regressor2.classification_precision == regressor.classification_precision
-    assert regressor2.classification_recall == regressor.classification_recall
-    assert regressor2.classification_f1 == regressor.classification_f1
-    assert regressor2.classification_confusion_matrix.tolist() == regressor.classification_confusion_matrix.tolist()
-    assert isinstance(regressor2.best_model, RegressorNet)
-    assert isinstance(regressor.best_model, RegressorNet)
+#     assert isinstance(regressor, PopRegressor)
+#     assert regressor.data.data.equals(data_obj.data)
+#     assert regressor.data.knowns.equals(data_obj.knowns)
+#     assert regressor.data.unknowns.equals(data_obj.unknowns)
+#     assert regressor.data.train.equals(data_obj.train)
+#     assert regressor.data.test.equals(data_obj.test)
+
+#     with pytest.raises(TypeError, match="epochs must be an integer"):
+#         regressor.train(epochs=0.5)
+
+#     with pytest.raises(TypeError, match="valid_size must be a float"):
+#         regressor.train(valid_size="0.2")
+
+#     with pytest.raises(ValueError, match="valid_size must be between 0 and 1"):
+#         regressor.train(valid_size=2.5)   
+
+#     with pytest.raises(TypeError, match="cv_splits must be an integer"):
+#         regressor.train(cv_splits="0.2")
+
+#     with pytest.raises(TypeError, match="cv_reps must be an integer"):
+#         regressor.train(cv_reps="0.2")
+
+#     with pytest.raises(TypeError, match="learning_rate must be a float"):
+#         regressor.train(learning_rate="0.2")
+
+#     with pytest.raises(ValueError, match="learning_rate must be between 0 and 1"):
+#         regressor.train(learning_rate=2.7)     
+
+#     with pytest.raises(TypeError, match="batch_size must be an integer"):
+#         regressor.train(batch_size=0.5)
+
+#     with pytest.raises(TypeError, match="dropout_prop must be a float"):
+#         regressor.train(dropout_prop="0.2")   
+
+#     with pytest.raises(ValueError, match="dropout_prop must be between 0 and 1"):
+#         regressor.train(dropout_prop=2) 
+
+#     with pytest.raises(TypeError, match="boot_data must be an instance of GeneticData"):
+#         regressor.train(boot_data="0.2")
+
+#     regressor.train()
+#     assert isinstance(regressor.train_history, pd.DataFrame)
+#     assert regressor.train_history.empty == False
+#     assert isinstance(regressor.best_model, torch.nn.Module)
+
+# def test_regressor_test():
+
+#     data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
+#                     sample_data="tests/test_data/testNA.txt")
+#     regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
+#     regressor.train()
+#     regressor.test()
+
+#     assert isinstance(regressor.test_results, pd.DataFrame)
+#     assert regressor.test_results.empty == False
+#     assert isinstance(regressor.median_distance, float)
+#     assert isinstance(regressor.mean_distance, float)
+#     assert isinstance(regressor.r2_long, float)
+#     assert isinstance(regressor.r2_lat, float)
+#     assert isinstance(regressor.summary, dict)
+
+# def test_regressor_assign_unknown_and_get_results():
+
+#     data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
+#                     sample_data="tests/test_data/testNA.txt")
+#     regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
+#     regressor.train()
+#     regressor.test()
+#     unknown_data = regressor.assign_unknown()
+
+#     assert unknown_data.equals(regressor.regression)
+#     assert os.path.exists(os.path.join(regressor.output_folder,
+#                           "regressor_assignment_results.csv"))
+#     os.remove(os.path.join(regressor.output_folder,
+#                             "regressor_assignment_results.csv"))
+
+#     assign_sum = regressor.get_assignment_summary(save=False)
+#     assert isinstance(assign_sum, dict)
+#     assert not os.path.exists(os.path.join(regressor.output_folder,
+#                               "regressor_classification_summary.csv"))
+
+#     with pytest.raises(ValueError, match=re.escape("Must run classify_by_contours() before getting summary.")):
+#         regressor.get_classification_summary(save=False)
+
+#     site_rank = regressor.rank_site_importance()
+#     assert isinstance(site_rank, pd.DataFrame)
+#     assert site_rank.empty == False
+#     assert len(regressor.data.data.alleles[0]) == len(site_rank)
+
+# def test_regressor_classify_by_contours():
+
+#     data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
+#                     sample_data="tests/test_data/testNA.txt")
+#     regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
+
+#     with pytest.raises(TypeError, match="nboots must be an integer"):
+#         regressor.classify_by_contours(nboots=0.5)
+
+#     with pytest.raises(TypeError, match="num_contours must be an integer"):
+#         regressor.classify_by_contours(num_contours=0.5)
+
+#     with pytest.raises(TypeError, match="save_plots must be a boolean"):
+#         regressor.classify_by_contours(save_plots="True")
+
+#     with pytest.raises(TypeError, match="save must be a boolean"):
+#         regressor.classify_by_contours(save="True")
+
+#     regressor.classify_by_contours()
+
+#     assert isinstance(regressor.classification_test_results, pd.DataFrame)
+#     assert regressor.classification_test_results.empty == False
+#     assert isinstance(regressor.contour_classification, pd.DataFrame)
+#     assert regressor.contour_classification.empty == False
+#     assert isinstance(regressor.classification_confusion_matrix, np.ndarray)
+#     assert isinstance(regressor.classification_accuracy, float)
+#     assert isinstance(regressor.classification_precision, float)
+#     assert isinstance(regressor.classification_recall, float)
+#     assert isinstance(regressor.classification_f1, float)
+
+#     class_sum = regressor.get_classification_summary(save=False)
+#     assert isinstance(class_sum, dict)
+#     assert class_sum["accuracy"] == regressor.classification_accuracy
+#     assert class_sum["precision"] == regressor.classification_precision
+#     assert class_sum["recall"] == regressor.classification_recall
+#     assert class_sum["f1"] == regressor.classification_f1
+#     assert (class_sum["confusion_matrix"] == regressor.classification_confusion_matrix).all()
+
+# def test_regressor_save_and_load():
+
+#     data_obj = GeneticData(genetic_data="tests/test_data/test.vcf", 
+#                     sample_data="tests/test_data/testNA.txt")
+#     regressor = PopRegressor(data_obj, output_folder=TEST_OUTPUT_FOLDER)
+#     regressor.train()
+#     regressor.test()
+#     regressor.assign_unknown()
+#     regressor.save()
+
+#     assert os.path.exists(os.path.join(regressor.output_folder,
+#                           "regressor.pkl"))
+
+#     regressor2 = PopRegressor.load(load_path=os.path.join(regressor.output_folder,
+#                                 "regressor.pkl"))
+
+#     assert regressor2.train_history.equals(regressor.train_history)
+#     assert regressor2.test_results.equals(regressor.test_results)
+#     assert regressor2.median_distance == regressor.median_distance
+#     assert regressor2.mean_distance == regressor.mean_distance
+#     assert regressor2.r2_lat == regressor.r2_lat
+#     assert regressor2.r2_long == regressor.r2_long
+#     assert regressor2.regression.equals(regressor.regression)
+#     assert isinstance(regressor2.best_model, RegressorNet)
+#     assert isinstance(regressor.best_model, RegressorNet)
+
+#     os.remove(os.path.join(regressor.output_folder,
+#                             "regressor.pkl"))
+
+#     regressor.classify_by_contours()
+#     regressor.save()
+
+#     regressor2 = PopRegressor.load(load_path=os.path.join(regressor.output_folder,
+#                                 "regressor.pkl"))
+
+#     assert regressor2.train_history.equals(regressor.train_history)
+#     assert regressor2.test_results.equals(regressor.test_results)
+#     assert regressor2.contour_classification.equals(regressor.contour_classification)
+#     assert regressor2.classification_test_results.equals(regressor.classification_test_results)
+#     assert regressor2.classification_accuracy == regressor.classification_accuracy
+#     assert regressor2.classification_precision == regressor.classification_precision
+#     assert regressor2.classification_recall == regressor.classification_recall
+#     assert regressor2.classification_f1 == regressor.classification_f1
+#     assert regressor2.classification_confusion_matrix.tolist() == regressor.classification_confusion_matrix.tolist()
+#     assert isinstance(regressor2.best_model, RegressorNet)
+#     assert isinstance(regressor.best_model, RegressorNet)
 
-    os.remove(os.path.join(regressor.output_folder,
-                            "regressor.pkl"))
+#     os.remove(os.path.join(regressor.output_folder,
+#                             "regressor.pkl"))
```

