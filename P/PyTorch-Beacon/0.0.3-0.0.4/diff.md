# Comparing `tmp/PyTorch-Beacon-0.0.3.tar.gz` & `tmp/PyTorch-Beacon-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTorch-Beacon-0.0.3.tar", last modified: Wed Jul 19 11:02:43 2023, max compression
+gzip compressed data, was "PyTorch-Beacon-0.0.4.tar", last modified: Tue Jul 25 11:56:25 2023, max compression
```

## Comparing `PyTorch-Beacon-0.0.3.tar` & `PyTorch-Beacon-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 11:02:43.189994 PyTorch-Beacon-0.0.3/
--rw-rw-rw-   0        0        0     1050 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.3/LICENCE
--rw-rw-rw-   0        0        0      532 2023-07-19 11:02:43.187999 PyTorch-Beacon-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-19 11:02:43.161070 PyTorch-Beacon-0.0.3/PyTorch_Beacon.egg-info/
--rw-rw-rw-   0        0        0      532 2023-07-19 11:02:42.000000 PyTorch-Beacon-0.0.3/PyTorch_Beacon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-07-19 11:02:43.000000 PyTorch-Beacon-0.0.3/PyTorch_Beacon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 11:02:42.000000 PyTorch-Beacon-0.0.3/PyTorch_Beacon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-19 11:02:42.000000 PyTorch-Beacon-0.0.3/PyTorch_Beacon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      208 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 11:02:43.185007 PyTorch-Beacon-0.0.3/beacon/
--rw-rw-rw-   0        0        0       97 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.3/beacon/__init__.py
--rw-rw-rw-   0        0        0     1246 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.3/beacon/dataloading.py
--rw-rw-rw-   0        0        0      483 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.3/beacon/metrics.py
--rw-rw-rw-   0        0        0     2005 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.3/beacon/training.py
--rw-rw-rw-   0        0        0     2533 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.3/beacon/utils.py
--rw-rw-rw-   0        0        0      463 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-19 11:02:43.189994 PyTorch-Beacon-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 11:56:25.430587 PyTorch-Beacon-0.0.4/
+-rw-rw-rw-   0        0        0     1050 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.4/LICENCE
+-rw-rw-rw-   0        0        0      532 2023-07-25 11:56:25.429582 PyTorch-Beacon-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-25 11:56:25.401651 PyTorch-Beacon-0.0.4/PyTorch_Beacon.egg-info/
+-rw-rw-rw-   0        0        0      532 2023-07-25 11:56:25.000000 PyTorch-Beacon-0.0.4/PyTorch_Beacon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-07-25 11:56:25.000000 PyTorch-Beacon-0.0.4/PyTorch_Beacon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 11:56:25.000000 PyTorch-Beacon-0.0.4/PyTorch_Beacon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-25 11:56:25.000000 PyTorch-Beacon-0.0.4/PyTorch_Beacon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      208 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 11:56:25.426583 PyTorch-Beacon-0.0.4/beacon/
+-rw-rw-rw-   0        0        0      122 2023-07-22 18:00:51.000000 PyTorch-Beacon-0.0.4/beacon/__init__.py
+-rw-rw-rw-   0        0        0     1215 2023-07-21 11:27:50.000000 PyTorch-Beacon-0.0.4/beacon/dataloading.py
+-rw-rw-rw-   0        0        0      483 2023-07-19 10:52:38.000000 PyTorch-Beacon-0.0.4/beacon/metrics.py
+-rw-rw-rw-   0        0        0     3018 2023-07-25 11:52:02.000000 PyTorch-Beacon-0.0.4/beacon/module.py
+-rw-rw-rw-   0        0        0     2024 2023-07-21 11:39:09.000000 PyTorch-Beacon-0.0.4/beacon/training.py
+-rw-rw-rw-   0        0        0     2551 2023-07-19 17:13:10.000000 PyTorch-Beacon-0.0.4/beacon/utils.py
+-rw-rw-rw-   0        0        0      463 2023-07-20 11:51:57.000000 PyTorch-Beacon-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 11:56:25.431571 PyTorch-Beacon-0.0.4/setup.cfg
```

### Comparing `PyTorch-Beacon-0.0.3/LICENCE` & `PyTorch-Beacon-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `PyTorch-Beacon-0.0.3/PKG-INFO` & `PyTorch-Beacon-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTorch-Beacon
-Version: 0.0.3
+Version: 0.0.4
 Summary: A lightweight helper library for PyTorch
 Author-email: Luke Ye <lukelele2001@gmail.com>
 Project-URL: Homepage, https://github.com/Lukelele/PyTorch-Beacon
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `PyTorch-Beacon-0.0.3/PyTorch_Beacon.egg-info/PKG-INFO` & `PyTorch-Beacon-0.0.4/PyTorch_Beacon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTorch-Beacon
-Version: 0.0.3
+Version: 0.0.4
 Summary: A lightweight helper library for PyTorch
 Author-email: Luke Ye <lukelele2001@gmail.com>
 Project-URL: Homepage, https://github.com/Lukelele/PyTorch-Beacon
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `PyTorch-Beacon-0.0.3/beacon/dataloading.py` & `PyTorch-Beacon-0.0.4/beacon/dataloading.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import os
 from torchvision import datasets, transforms
 from torch.utils.data import DataLoader
 
 
-NUM_WORKERS = os.cpu_count()
-
-
 def from_path(dataset_dir: str, batch_size: int = 32, transform: transforms.Compose = transforms.ToTensor(), shuffle=True, dataset_type=datasets.ImageFolder, pin_memory=True):
     dataset = dataset_type(dataset_dir, transform=transform)
     labels = dataset.classes
     dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, pin_memory=pin_memory)
 
     return dataloader, labels
```

### Comparing `PyTorch-Beacon-0.0.3/beacon/training.py` & `PyTorch-Beacon-0.0.4/beacon/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 from . import metrics
 import numpy as np
 from tqdm.auto import tqdm
 
 
-def fit(model: torch.nn.Module, dataloader: torch.utils.data.DataLoader, loss_type=torch.nn.MSELoss, optimiser=torch.optim.SGD, accuracy_func=metrics.categorical_accuracy, epochs=100, lr=0.01, device="cpu"):
+def fit(model: torch.nn.Module, dataloader: torch.utils.data.DataLoader, optimiser=torch.optim.Adam, loss_type=torch.nn.CrossEntropyLoss, accuracy_func=metrics.categorical_accuracy, epochs=100, lr=0.01, device="cpu"):
     model.to(device)
 
     loss_func = loss_type()
     optimiser = optimiser(model.parameters(), lr=lr)
 
     losses = np.zeros(epochs)
     accuracies = np.zeros(epochs)
@@ -37,15 +37,15 @@
         epoch_accuracy = batch_accuracy / len(dataloader)
         losses[epoch] = epoch_loss.item()
         accuracies[epoch] = epoch_accuracy.item()
 
     return losses, accuracies
 
 
-def evaluate(model: torch.nn.Module, dataloader: torch.utils.data.DataLoader, loss_type=torch.nn.MSELoss, accuracy_func=metrics.categorical_accuracy, device="cpu"):
+def evaluate(model: torch.nn.Module, dataloader: torch.utils.data.DataLoader, loss_type=torch.nn.CrossEntropyLoss, accuracy_func=metrics.categorical_accuracy, device="cpu"):
     model.to(device)
     model.eval()
 
     loss_func = loss_type()
 
     loss = 0
     accuracy = 0
```

### Comparing `PyTorch-Beacon-0.0.3/beacon/utils.py` & `PyTorch-Beacon-0.0.4/beacon/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from PIL import Image
 import torch
 from torchvision import transforms
 
 
-########################   Saving and Loading   ########################
+###########################   Saving and Loading   ###########################
 
 
 def save_model(model: torch.nn.Module, save_directory: str, model_name: str):
     target_directory = Path(save_directory)
     target_directory.mkdir(parents=True, exist_ok=True)
 
     assert model_name.endswith(".pth") or model_name.endswith(".pt")
@@ -18,15 +18,15 @@
 
 
 def load_model(model: torch.nn.Module, model_state_path: str):
     model_state = torch.load(model_state_path)
     model.load_state_dict(model_state)
 
 
-######################   For Image Classification   ######################
+########################   For Image Classification   ########################
 
 
 def get_image_tensor_from_path(image_path: str):
     image = Image.open(image_path)
     image_tensor = transforms.ToTensor()(image).unsqueeze_(0)
     image.close()
 
@@ -49,30 +49,31 @@
     
 
 def display_image_from_tensor(image_tensor: torch.Tensor):
     image = transforms.ToPILImage()(image_tensor)
     image.show()
 
 
-def classify(model: torch.nn.Module, image: torch.Tensor, labels: list, return_image=False, device="cpu"):
+def classify(model: torch.nn.Module, image: torch.Tensor, labels: list, device="cpu"):
     model.to(device)
     model.eval()
 
     with torch.inference_mode():
         y_pred = model(image.to(device))
         y_prob = torch.softmax(y_pred, dim=1)
         y_pred = torch.argmax(y_prob, dim=1)
 
-    if return_image:
-        return labels[y_pred.item()], y_prob, get_image_from_tensor(image)
-    else:
-        return labels[y_pred.item()], y_prob
+    labels_list = torch.zeros(len(y_pred))
+        
+    for i, y in enumerate(y_pred):
+        labels_list[i] = labels[y.item()].item()
+    return labels_list, y_prob
 
 
-##########################   Misc   ##########################
+################################   Misc   ################################
 
 
 def dataloader_to_tensor(dataloader: torch.utils.data.DataLoader, batch_count: int = 0):
     data_tensor = None
     label_tensor = None
     
     for batch, (data, label) in enumerate(dataloader):
```

