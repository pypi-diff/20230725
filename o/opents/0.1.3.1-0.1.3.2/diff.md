# Comparing `tmp/opents-0.1.3.1-py3-none-any.whl.zip` & `tmp/opents-0.1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 8952 bytes, number of entries: 15
+Zip file size: 9232 bytes, number of entries: 14
 -rw-rw-r--  2.0 unx       54 b- defN 23-Jun-20 07:42 opents/__init__.py
 -rw-rw-r--  2.0 unx       14 b- defN 23-Jun-20 07:42 opents/data/__init__.py
--rw-rw-r--  2.0 unx     6306 b- defN 23-Jun-20 13:04 opents/data/generate_datasets.py
--rw-rw-r--  2.0 unx       93 b- defN 23-Jul-17 07:47 opents/datasets/__init__.py
--rw-rw-r--  2.0 unx    11434 b- defN 23-Jul-17 07:47 opents/datasets/datasets.py
+-rw-rw-r--  2.0 unx       31 b- defN 23-Jul-25 07:22 opents/datasets/__init__.py
+-rw-rw-r--  2.0 unx     6800 b- defN 23-Jul-25 11:51 opents/datasets/datasets.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jul-17 07:06 opents/evaluate/__init__.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jul-17 07:53 opents/nn/__init__.py
--rw-rw-r--  2.0 unx       17 b- defN 23-Jul-17 07:12 opents/nn/models/__init__.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jun-06 11:07 opents/nn/models/fcn.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-28 15:32 opents/utils/__init__.py
--rw-rw-r--  2.0 unx     4750 b- defN 23-Jul-17 07:45 opents/utils/data_utils.py
--rw-rw-r--  2.0 unx     1975 b- defN 23-Jul-17 07:57 opents-0.1.3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 07:57 opents-0.1.3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jul-17 07:57 opents-0.1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1188 b- defN 23-Jul-17 07:57 opents-0.1.3.1.dist-info/RECORD
-15 files, 28189 bytes uncompressed, 6974 bytes compressed:  75.3%
+-rw-rw-r--  2.0 unx       23 b- defN 23-Jul-24 12:48 opents/nn/__init__.py
+-rw-rw-r--  2.0 unx       20 b- defN 23-Jul-24 12:14 opents/nn/models/__init__.py
+-rw-rw-r--  2.0 unx     3861 b- defN 23-Jul-25 07:05 opents/nn/models/fcn.py
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 12:11 opents/utils/__init__.py
+-rw-rw-r--  2.0 unx    10171 b- defN 23-Jul-25 12:53 opents/utils/data_utils.py
+-rw-rw-r--  2.0 unx     2198 b- defN 23-Jul-25 13:28 opents-0.1.3.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 13:28 opents-0.1.3.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-25 13:28 opents-0.1.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1101 b- defN 23-Jul-25 13:28 opents-0.1.3.2.dist-info/RECORD
+14 files, 24464 bytes uncompressed, 7394 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -1,16 +1,13 @@
 Filename: opents/__init__.py
 Comment: 
 
 Filename: opents/data/__init__.py
 Comment: 
 
-Filename: opents/data/generate_datasets.py
-Comment: 
-
 Filename: opents/datasets/__init__.py
 Comment: 
 
 Filename: opents/datasets/datasets.py
 Comment: 
 
 Filename: opents/evaluate/__init__.py
@@ -27,20 +24,20 @@
 
 Filename: opents/utils/__init__.py
 Comment: 
 
 Filename: opents/utils/data_utils.py
 Comment: 
 
-Filename: opents-0.1.3.1.dist-info/METADATA
+Filename: opents-0.1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: opents-0.1.3.1.dist-info/WHEEL
+Filename: opents-0.1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: opents-0.1.3.1.dist-info/top_level.txt
+Filename: opents-0.1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: opents-0.1.3.1.dist-info/RECORD
+Filename: opents-0.1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opents/datasets/__init__.py

```diff
@@ -1 +1 @@
-from .datasets import UCRDataset, UEADataset, OpenUCRDataset, OpenUEADataset, GenerateDataset
+from .datasets import TSDataset
```

## opents/datasets/datasets.py

```diff
@@ -1,13 +1,14 @@
 # coding=utf-8
 
 import pandas as pd
 import torch
 import numpy as np
-from opents.utils.data_utils import data_file_type, get_dataset_root_path, split_train_test
+from opents.utils.data_utils import data_file_type, get_dataset_root_path
+from torch import cat
 
 class Dataset:
     def __init__(
             self,
             dataset_name,
             dataset_root_path=None,
             datasets_root_name=None,
@@ -98,143 +99,45 @@
             
             # Retrieve the values of all new labels and store them in 'train_label'.
             y_train = np.vectorize(transform.get)(train_labels)
 
             # Retrieve all label values from the test set and store them in 'test_label'.
             y_test = np.vectorize(transform.get)(test_labels) 
 
-
+        x_train, y_train, x_test, y_test = torch.tensor(x_train).to(torch.float), torch.tensor(y_train).long(), torch.tensor(x_test).to(torch.float), torch.tensor(y_test).long()
+        # x_train, y_train, x_test, y_test = x_train.to(torch.float32), y_train.to(torch.long), x_test.to(torch.float32), y_test.to(torch.long)
         # Add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
         return x_train, y_train, x_test, y_test
 
-    def opents_dataset(self):
-        """ The path to read the UCR or UEA file, including the path of the training file and the path of the testing file.
-        Args:
-            dataset(string):Define a variable 'dataset_name' for the name of each file, which can be used to locate the training and testing file paths for each function.
-        Returns:
-            for UCR:add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
-            for UEA:return the train data, new label of train data, test data, and new label of test data.
-        """
-        train_file_df, test_file_df = data_file_type(self.dataset_name, self.dataset_root_path, self.datasets_root_name) 
-
-        if self.datasets_root_name.lower() == 'ucr': 
-            # merge the train and test file into a full data
-            all_data_df = pd.concat([train_file_df, test_file_df], axis=0)
-        
-            # Create a two-dimensional tensor file from the data in the all files.
-            all_tensor = torch.tensor(all_data_df.values)
-
-            # Here, we extract the distinct labels from each dataset.
-            all_labels = torch.unique(all_tensor[:, 0])
-            
-            # Store the labels in a dictionary, where the key is the original label and the value is the count of that label.
-            transform = {}
-
-            for i, l in enumerate(all_labels):
-                transform[l.item()] = i
-
-            # Convert the data into a list.
-            all_array = all_tensor.tolist()
-            all_array = np.array(all_array)
-
-            # Retrieve the time-series data, excluding the labels. 
-            all = all_array[:, 1:].astype(np.float64)
-
-            # Retrieve the values of all new labels and store them in 'train_label'.
-            y_all = np.vectorize(transform.get)(all_array[:, 0])
-            
-            # Add an extra dimension to the train data and test data, then return the train data, new label of train data, test data, and new label of test data.
-            x_all = all[..., np.newaxis]
-
-            x_train, y_train, x_test, y_test = split_train_test(x_all=x_all, y_all=y_all, train_percentage=self.train_percentage, open_percentage=self.open_percentage)
-
-        elif self.datasets_root_name.lower() == 'uea':
-            
-            all_data_df = pd.concat([train_file_df, test_file_df], axis=0)
-
-            all_data_df = all_data_df.reset_index(drop=True)
-            all_dataset_name = self.dataset_name + "_TRAIN"
-
-            # Store the train data and test data in list, and extend its dimention to 3.
-            all_array = np.array(all_data_df[all_dataset_name].tolist())
-            x_all = all_array.view((np.float64, len(all_array.dtype.names)))
-            
-            # Here, we extract the distinct labels from each dataset.
-            all_labels = torch.tensor(pd.to_numeric(all_data_df['target'], errors='coerce'))
-            y_all = torch.unique(all_labels)
-            
-            transform = {}
-
-            for i, l in enumerate(y_all):
-                transform[l.item()] = i
-            
-            # Retrieve the values of all new labels and store them in 'train_label'.
-            y_all = np.vectorize(transform.get)(all_labels)
-
-            x_train, y_train, x_test, y_test = split_train_test(x_all=x_all, y_all=y_all, train_percentage=self.train_percentage, open_percentage=self.open_percentage)
-
-        return  x_train, y_train, x_test, y_test
 
     
 
 class TSDataset(Dataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None):
-        super().__init__(dataset_name, dataset_root_path, datasets_name)
+    """
+    This class is a child of the Dataset class. It aims to handle time-series data.
 
-    
-class UCRDataset(TSDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR'):
-        super().__init__(dataset_name, dataset_root_path, datasets_name)
-        self.datasets_name = datasets_name
-        self.x_train, self.y_train, self.x_test, self.y_test = self.ts_dataset()
-    
-    def __iter__(self):
-        yield from (self.x_train, self.y_train, self.x_test, self.y_test)
-
-class UEADataset(TSDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UEA'):
+    Attributes:
+    ------------
+    dataset_name (str): Name of the dataset
+    dataset_root_path (str, optional): Root path of the dataset. Default is None.
+    datasets_name (str, optional): Name of the Root datasets. eg:ucr or uea. Default is None.
+    x_train (numpy.ndarray): The training data.
+    y_train (numpy.ndarray): The labels of the training data.
+    x_test (numpy.ndarray): The testing data.
+    y_test (numpy.ndarray): The labels of the testing data.
+
+    Methods:
+    ------------
+    __init__(self, dataset_name, dataset_root_path=None, datasets_name=None):
+        Initializes the TSDataset object with the given parameters and loads the dataset using ts_dataset() function.
+    
+    load(self):
+        Returns the loaded dataset including x_train, y_train, x_test, y_test.
+    """
+    def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None):
         super().__init__(dataset_name, dataset_root_path, datasets_name)
         self.datasets_name = datasets_name
         self.x_train, self.y_train, self.x_test, self.y_test = self.ts_dataset()
     
-    def __iter__(self):
-        yield from (self.x_train, self.y_train, self.x_test, self.y_test)
-
-
-
-class OpenDataset(Dataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name=None, split=True, train_percentage=None,open_percentage=None, random_state=None):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split, train_percentage, open_percentage, random_state)
-
-    
-class OpenUCRDataset(OpenDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UCR', split=True, train_percentage=None,open_percentage=None, random_state=None):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split, train_percentage, open_percentage, random_state)
-        self.datasets_name = datasets_name
-
-        self.x_train, self.y_train, self.x_test, self.y_test = self.opents_dataset()
-    
-    def __iter__(self):
-        yield from (self.x_train, self.y_train, self.x_test, self.y_test)
-
-class OpenUEADataset(OpenDataset):
-    def __init__(self, dataset_name, dataset_root_path=None, datasets_name='UEA', split=True, train_percentage=None,open_percentage=None, random_state=None):
-        super().__init__(dataset_name, dataset_root_path, datasets_name, split, train_percentage, open_percentage, random_state)
-        self.datasets_name = datasets_name
-
-        self.x_train, self.y_train, self.x_test, self.y_test = self.opents_dataset()
-    
-    def __iter__(self):
-        yield from (self.x_train, self.y_train, self.x_test, self.y_test)
-   
-class GenerateDataset(Dataset):
-    def __init__(self, data, targets):
-        self.data = data
-        self.targets = targets
-    
-    def __getitem__(self, index):
-        x = self.data[index]
-        y = self.targets[index]
-        return x, y
+    def load(self):
+        return self.x_train, self.y_train, self.x_test, self.y_test
     
-    def __len__(self):
-        return len(self.data)
```

## opents/nn/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6672 6f6d 202e 6d6f 6465 6c73 2069 6d70  from .models imp
+00000010: 6f72 7420 4643 4e                        ort FCN
```

## opents/nn/models/__init__.py

```diff
@@ -1 +1 @@
-from . import FCN
+from .fcn import FCN
```

## opents/nn/models/fcn.py

```diff
@@ -1,61 +1,105 @@
 import torch
 import torch.nn as nn
 
 class FCN(nn.Module):
-
-    def __init__(self, input_size, unit_list, output_size, num_classes, num_cnns, kernel_size=30, stride=1, dropout=0.5,padding='same'):
+    """
+    Fully Connected Network (FCN) for timeseries classification.
+    """
+    def __init__(self, in_channels, unit_list, out_channels, num_classes, num_cnns, kernel_size=30, stride=1, dropout=0.5, padding='same'):
+        """
+        Constructor for the FCN class.
+
+        Args:
+            in_channels (int): Number of input channels.
+            unit_list (list): List of number of units in each layer.
+            out_channels (int): Number of output channels.
+            num_classes (int): Number of classes for classification.
+            num_cnns (int): Number of convolutional layers.
+            kernel_size (int, optional): Size of the kernel for the convolutional layers. Defaults to 30.
+            stride (int, optional): Stride for the convolutional layers. Defaults to 1.
+            dropout (float, optional): Dropout rate. Defaults to 0.5.
+            padding (str, optional): Padding type for the convolutional layers. Defaults to 'same'.
+        """
         super(FCN, self).__init__()
-        self.input_size = input_size
+        self.in_channels = in_channels
         self.unit_list = unit_list
-        self.output_size = output_size
+        self.out_channels = out_channels
         self.num_classes = num_classes
         self.num_cnns = num_cnns
         self.kernel = kernel_size
         self.stride = stride
         self.dropout = dropout
-        self.padding = "same"
+        self.padding = padding
 
         self.convs = nn.ModuleList()
 
         # first cnns layer
-        self.convs.append(nn.Conv1d(self.input_size, self.unit_list[0], kernel_size=self.kernel, stride=self.stride, padding=self.padding if self.stride == 1 else self.kernel // 2))
+        self.convs.append(nn.Conv1d(self.in_channels, self.unit_list[0], kernel_size=self.kernel, stride=self.stride, padding=self.padding if self.stride == 1 else self.kernel // 2))
         self.convs.append(nn.ReLU())
         self.convs.append(nn.Dropout(self.dropout))
+
         # other cnns layers: except first cnns layer
         for unit_num in range(len(self.unit_list)):
             for cnns_num in range(self.num_cnns):
                     self.convs.append(Residual(nn.Conv1d(self.unit_list[unit_num], self.unit_list[unit_num], kernel_size=self.kernel, padding=self.padding)))
                     self.convs.append(nn.ReLU())
                     self.convs.append(nn.Dropout(self.dropout))
             if unit_num == len(self.unit_list) - 1:
                  break
             self.convs.append(nn.Conv1d(self.unit_list[unit_num], self.unit_list[unit_num + 1], kernel_size=self.kernel, stride=self.stride, padding=self.padding))
             self.convs.append(nn.ReLU())
             self.convs.append(nn.Dropout(self.dropout))
         
         # the last linear layer
-        self.fc = nn.Linear(unit_list[-1], num_classes)
+        self.fc = nn.Linear(unit_list[-1] * 2, num_classes)
     
     def forward(self, inputs):
+        """
+        Defines the computation performed at every call.
+
+        Args:
+            inputs (torch.Tensor): Input tensor.
+
+        Returns:
+            torch.Tensor: Output tensor after passing through the network.
+        """
         x = inputs
         x = x.transpose(1, 2)
         
         for layer in self.convs:
             x = layer(x)
         x = x.transpose(1, 2)
 
         # last layer
-        torch.cat([x.mean(dim=1), x.max(dim=1)[0]], dim=-1)
+        x = torch.cat([x.mean(dim=1), x.max(dim=1)[0]], dim=-1)
         x = nn.Dropout(0.5)(x)
         x = self.fc(x)
 
         return x
 
 class Residual(nn.Module):
+    """
+    Implements the Residual Block for the FCN.
+    """
     def __init__(self, model):
-         super().__init__()
-         self.model = model
+        """
+        Constructor for the Residual class.
+
+        Args:
+            model (nn.Module): The base model/block on which residual connections will be used.
+        """
+        super().__init__()
+        self.model = model
 
     def forward(self, x):
+        """
+        Defines the computation performed at every call.
+
+        Args:
+            x (torch.Tensor): Input tensor.
+
+        Returns:
+            torch.Tensor: Output tensor after adding the input tensor and the output from the base model/block.
+        """
         h = self.model(x)
         return x + h
```

## opents/utils/__init__.py

```diff
@@ -0,0 +1,6 @@
+00000000: 6672 6f6d 202e 6461 7461 5f75 7469 6c73  from .data_utils
+00000010: 2069 6d70 6f72 7420 5261 6e64 6f6d 5370   import RandomSp
+00000020: 6c69 744f 7065 6e44 6174 6173 6574 2c20  litOpenDataset, 
+00000030: 5261 6e64 6f6d 5370 6c69 744f 7065 6e41  RandomSplitOpenA
+00000040: 6c6c 4461 7461 7365 742c 2072 656c 6162  llDataset, relab
+00000050: 656c 5f66 726f 6d5f 7a65 726f            el_from_zero
```

## opents/utils/data_utils.py

```diff
@@ -2,31 +2,51 @@
 import requests
 import zipfile 
 import pandas as pd
 from scipy.io import arff
 import numpy as np
 import random
 from sklearn.model_selection import train_test_split
-from torch.utils.data import Dataset
+import torch
+from sklearn.preprocessing import LabelEncoder
 
 DEFAULT_DATASETS_ROOT = "data"
 
 def download_file(url, datasets_name, datasets_root_path):
+    """
+    Downloads a file from the specified URL to a destination path.
+
+    Args:
+        url (str): URL of the file to download.
+        datasets_name (str): Name of the dataset being downloaded.
+        datasets_root_path (str): The destination path where the downloaded file will be stored.
+    """
     response = requests.get(url)
     if response.status_code == 200:
         with open(datasets_root_path, 'wb') as file:
             file.write(response.content)
         print(datasets_name + "is successfully downloaded")
     else:
         print(datasets_name + "is not successfully downloaded")
 
 
 def get_dataset_root_path(dataset_root_path=None, dataset_name=None, datasets_name=None,
                           datasets_root_path=DEFAULT_DATASETS_ROOT):
+    """
+    Gets the root path of the dataset. If the dataset is not found, it downloads and extracts it.
 
+    Args:
+        dataset_root_path (str, optional): The root path of the dataset. Defaults to None.
+        dataset_name (str, optional): Name of the dataset. Defaults to None.
+        datasets_name (str, optional): Name of the datasets (either 'UCR' or 'UEA'). Defaults to None.
+        datasets_root_path (str, optional): The root path of the datasets. Defaults to DEFAULT_DATASETS_ROOT.
+
+    Returns:
+        str: The root path of the dataset.
+    """
     if dataset_name is None:
         print("Please provide a valid dataset name.")
         return None
     
     if dataset_root_path is None:
         dataset_root_path = os.path.join(datasets_root_path, dataset_name)
     dataset_root_path = os.path.abspath(dataset_root_path)
@@ -56,15 +76,26 @@
         else:
             print("the dataset is not contain in our contain, please use the Dataset command")
     else:
         print(dataset_name + "is available")
     return dataset_root_path
 
 def data_file_type(dataset_name,dataset_root_path=None, datasets_root_name=None, all_file_path=None):
+    """
+    Determines the data file type based on the dataset name, and reads the data from each file in the dataset.
 
+    Args:
+        dataset_name (str): Name of the dataset.
+        dataset_root_path (str, optional): The root path of the dataset. Defaults to None.
+        datasets_root_name (str, optional): Name of the datasets (either 'UCR' or 'UEA'). Defaults to None.
+        all_file_path (str, optional): All file path. Defaults to None.
+
+    Returns:
+        pandas.DataFrame, pandas.DataFrame: DataFrames containing the training and testing data.
+    """
     if datasets_root_name.lower() == "ucr":
         # Define the paths for the training and testing sets.
         train_file_path = os.path.join(dataset_root_path, dataset_name, dataset_name + "_TRAIN.tsv")
         test_file_path = os.path.join(dataset_root_path, dataset_name, dataset_name + "_TEST.tsv")
         # Read the data from each file in the training set and testing set using the pandas library, which is a library for data processing.
         train_file_df = pd.read_csv(train_file_path, sep='\t', header=None)
         test_file_df = pd.read_csv(test_file_path, sep='\t', header=None)
@@ -76,31 +107,116 @@
         train_data_arff = arff.loadarff(train_file_path)
         train_file_df = pd.DataFrame(train_data_arff[0])
         test_data_arff = arff.loadarff(test_file_path)
         test_file_df = pd.DataFrame(test_data_arff[0])
     return train_file_df, test_file_df
 
 
-def split_train_test(x_all, y_all, train_percentage=0.5, open_percentage=0.5, open_random=42, train_random_state=42):
-
-    # Get unique labels and calculate the number of labels to select for the test set
-    y_unique = np.unique(y_all)
-    y_open_nums = int(len(y_unique) * open_percentage)
 
-    # if the number of y_open is 0, it indicates that the dataset has not open data.
-    if y_open_nums == 0:
-        raise ValueError("The number of open label data is 0, please change the percentage.")
+class RandomSplitOpenDataset:
+    """
+    A class used to represent a dataset that is randomly split into training and testing sets.
+
+    Attributes:
+        x_train (numpy.ndarray): The input features for the training set.
+        y_train (numpy.ndarray): The labels for the training set.
+        x_test (numpy.ndarray): The input features for the testing set.
+        y_test (numpy.ndarray): The labels for the testing set.
+        train_size_rate (float): The percentage of samples to include in the training set.
+        open_label_rate (float): The percentage of unique labels to select for the open set.
+        train_random_state (int): Random seed for splitting the data into training and testing sets.
+        open_random_state (int): Random seed for selecting open set labels.
+    """
+    def __init__(
+            self,
+            x_train,
+            y_train,
+            x_test,
+            y_test,
+            train_size_rate=0.5,
+            open_label_rate=0.5,
+            train_random_state=42,
+            open_random_state=42
+            ):
+        
+        self.x_train = x_train
+        self.y_train = y_train
+        self.x_test = x_test
+        self.y_test = y_test
+        self.train_size_rate = train_size_rate
+        self.open_label_rate = open_label_rate
+        self.train_random_state = train_random_state
+        self.open_random_state = open_random_state
+        
+        self.x_train, self.y_train, self.x_test, self.y_test = x_train.numpy(), y_train.numpy(), x_test.numpy(), y_test.numpy()
+
+    def load(self):
+        """
+        Loads the dataset and splits it into training and testing sets.
+
+        Returns:
+            torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor: Tensors containing the input features and labels for the training and testing sets.
+        """
+        self.all_features = np.concatenate([self.x_train, self.x_test], axis=0)
+        self.all_labels = np.concatenate([self.y_train, self.y_test], axis=0)
+        # Get unique labels and calculate the number of labels to select for the test set
+        unique_labels = np.unique(self.all_labels)
+        y_open_nums = int(len(unique_labels) * self.train_size_rate)
+
+        # if the number of y_open is 0, it indicates that the dataset has not open data.
+        if y_open_nums == 0:
+            raise ValueError("The number of open label data is 0, please change the percentage.")
+
+        # fix the seed of random
+        random.seed(self.train_random_state)
+
+        # choose the y_open and unselected_labels in y_all. the labels in the y_open and unselected_labels are unique. 
+        self.selected_open_labels = random.sample(list(unique_labels), y_open_nums)
+        unselected_labels = [_ for _ in unique_labels if _ not in self.selected_open_labels]
+
+        x_train, x_test, y_train, y_test = train_test_split(self.all_features, self.all_labels, train_size=self.train_size_rate, random_state=self.train_random_state, stratify=self.all_labels)
+
+        mask = np.isin(y_train, self.selected_open_labels, invert=True)
+        x_train = x_train[mask]
+        y_train = y_train[mask]
+        
+        x_train, y_train, x_test, y_test = torch.tensor(x_train), torch.tensor(y_train).long(), torch.tensor(x_test), torch.tensor(y_test).long()
+
+        return x_train, y_train, x_test, y_test
+        
+class RandomSplitOpenAllDataset(RandomSplitOpenDataset):
+    def __init__(self, x_train, y_train, x_test, y_test, train_size_rate, open_label_rate, train_random_state=42, open_random_state=42):
+        super().__init__(x_train, y_train, x_test, y_test, train_size_rate, open_label_rate, train_random_state, open_random_state)
+    
+    def load(self):
+        x_train, y_train, x_test, y_test = super().load()
+        x_train, y_train, x_test, y_test = x_train.numpy(), y_train.numpy(), x_test.numpy(), y_test.numpy() 
 
-    # fix the seed of random
-    random.seed(open_random)
+        mask = np.isin(y_test, self.selected_open_labels, invert=True)
+        unmask = ~mask
+        x_test, last_x_test = x_test[mask], x_test[unmask]
+        y_test, last_y_test = y_test[mask], y_test[unmask]
 
-    # choose the y_open and y_not_open in y_all. the labels in the y_open and y_not_open are unique. 
-    y_open_select = random.sample(list(y_unique), y_open_nums)
-    y_not_open = [_ for _ in y_unique if _ not in y_open_select]
 
-    x_train, x_test, y_train, y_test = train_test_split(x_all, y_all, train_size=train_percentage,random_state=train_random_state, stratify=y_all)
+        x_train, y_train, x_test, y_test, last_x_test, last_y_test = torch.tensor(x_train), torch.tensor(y_train).long(), torch.tensor(x_test), torch.tensor(y_test).long(), torch.tensor(last_x_test), torch.tensor(last_y_test).long()
+        
+        return x_train, y_train, x_test, y_test, last_x_test, last_y_test
 
-    mask = np.isin(y_train, y_open_select, invert=True)
-    x_train = x_train[mask]
-    y_train = y_train[mask]
 
-    return x_train, y_train, x_test, y_test
+def relabel_from_zero(*args):
+    
+    if len(args) > 2:
+        raise ValueError("Too many arguments. This function expects 1 or 2 arguments.") 
+    encoder = LabelEncoder()
+
+    if len(args) == 1:
+        labels = args[0].numpy()
+        labels = encoder.fit_transform(labels)
+        labels = torch.tensor(labels).long()
+        return labels
+    if len(args) == 2:
+        y_train, y_test = args[0].numpy(), args[1].numpy()
+        encoder.fit(np.concatenate([y_train, y_test]))
+        y_train = encoder.transform(y_train)
+        y_test = encoder.transform(y_test)
+        y_train, y_test = torch.tensor(y_train).long(),torch.tensor(y_test).long()
+        return y_train, y_test
```

## Comparing `opents-0.1.3.1.dist-info/METADATA` & `opents-0.1.3.2.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: opents
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: OpenTS is a friendly Python Library for time series analysis
 Home-page: https://github.com/PyOpenTS/PyOpenTS
 Author: hushuguo
 Author-email: husg8217@mails.jlu.edu.cn
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: tqdm
 
 # PyOpenTS
 
 PyOpenTS is a library specifically designed to integrate methods and modules for time series. Its purpose is to allow users of this library to call and modify time series modules in a simpler and more convenient way. By using PyOpenTS, you can simplify the time series code process and reliably provide time series related module functions.  
 
+## Homepage and Documentation
+
++ Homepage: [https://github.com/PyOpenTS/PyOpenTS](https://github.com/PyOpenTS/PyOpenTS)
++ Documentation: [https://opents.readthedocs.io/en/latest/](https://opents.readthedocs.io/en/latest/)
+
 ## Our Goal
 
 Our goal is to simplify the process of handling time series code so that users can more easily tackle various time series problems. Whether you are a data scientist, an engineer, a researcher, or someone interested in time series, PyOpenTS will be a powerful tool for you.  
 
 ## Features
 
 * A clean API for quickly calling and modifying time series modules
```

## Comparing `opents-0.1.3.1.dist-info/RECORD` & `opents-0.1.3.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 opents/__init__.py,sha256=xRL8tSUxNiTSIygSIrQ0Y2i_guxRW_SNhljbNkCKNP4,54
 opents/data/__init__.py,sha256=E_iP2Kb-in3dJvXIMmvTbcBz6OrHVHDGFEwC-Qakdj0,14
-opents/data/generate_datasets.py,sha256=vh1CbEDm-UlIBhFIVJMivpFInA4xqoKLzyJJx_FuHso,6306
-opents/datasets/__init__.py,sha256=8suQnWyzx2SXO4kFV6rv1KgiLUOhLKFsY53X8L44BTI,93
-opents/datasets/datasets.py,sha256=S-hDRevnzg1GnxbFgI5pwPUivNDSr3S2i6N6w66AxPI,11434
+opents/datasets/__init__.py,sha256=Il-hXgnDs4L3Afz9rCX_OY_y4JSInjBMGn0kcJbV4jY,31
+opents/datasets/datasets.py,sha256=oRYDZO-JrV6zSZuHN0vOsgxQjhq5FWUhYFem7e7vxE4,6800
 opents/evaluate/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-opents/nn/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-opents/nn/models/__init__.py,sha256=LwMI4SOx--2aYe7HpFcLx1BS0uo1MIRi0aPIhgtgGmM,17
-opents/nn/models/fcn.py,sha256=ai9WyAY9oogE7Pmn8zD5o2hakV9AHCgXhYafPDUVJJ4,2259
-opents/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-opents/utils/data_utils.py,sha256=qDgX557rcXaSuxUSSdUcmCTCpPsAqyffL1Y6_KFn81Y,4750
-opents-0.1.3.1.dist-info/METADATA,sha256=TGGnREH4l2aTLLhmKXOuU9xM44jq_l0GFEJtFIrJa9k,1975
-opents-0.1.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-opents-0.1.3.1.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
-opents-0.1.3.1.dist-info/RECORD,,
+opents/nn/__init__.py,sha256=6uEDX0GQ3Z3aaZsVf3r9dnlWK2k-VeWh3uqEqHgA8vo,23
+opents/nn/models/__init__.py,sha256=b1LlF1f44wRZ4S4cGD7jT4TXHs3CEHJv-Q3ylsK8O-E,20
+opents/nn/models/fcn.py,sha256=N1s0JQyj_V4LiueWLY-ZZhTMpOIEqyJ4vXmRktplhnk,3861
+opents/utils/__init__.py,sha256=yz0eMqw6MGe9pEgENz1hCRkJgtYeVuOEtObEKHKorUs,92
+opents/utils/data_utils.py,sha256=dyQ9eK49ef16LwiyDpXrxr7_8-4eg40t48VXuAiJHr8,10171
+opents-0.1.3.2.dist-info/METADATA,sha256=8RQbB_KHQiftp96gXxtevJZcmezqcWgwg7TY2ED3D44,2198
+opents-0.1.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+opents-0.1.3.2.dist-info/top_level.txt,sha256=VMPO4pjOtyRL1h-EZc31aY2v5787ZqAKkOzzbkgw300,7
+opents-0.1.3.2.dist-info/RECORD,,
```

