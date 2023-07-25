# Comparing `tmp/OneOnOne-0.6947.tar.gz` & `tmp/OneOnOne-0.6948.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OneOnOne-0.6947.tar", last modified: Mon Jul 24 16:17:39 2023, max compression
+gzip compressed data, was "OneOnOne-0.6948.tar", last modified: Tue Jul 25 07:28:27 2023, max compression
```

## Comparing `OneOnOne-0.6947.tar` & `OneOnOne-0.6948.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-24 16:17:39.961927 OneOnOne-0.6947/
--rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6947/LICENSE
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-24 16:17:39.957548 OneOnOne-0.6947/OneOnOne/
--rw-r--r--   0 sohinib    (501) staff       (20)    55595 2023-07-24 16:02:42.000000 OneOnOne-0.6947/OneOnOne/__init__.py
--rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6947/OneOnOne/classes.py
--rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6947/OneOnOne/classification.py
--rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6947/OneOnOne/contextdecider.py
--rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6947/OneOnOne/htmlparser.py
--rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6947/OneOnOne/questionanswer.py
--rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6947/OneOnOne/sampling.py
-drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-24 16:17:39.961065 OneOnOne-0.6947/OneOnOne.egg-info/
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-24 16:17:39.000000 OneOnOne-0.6947/OneOnOne.egg-info/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-24 16:17:39.000000 OneOnOne-0.6947/OneOnOne.egg-info/SOURCES.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-24 16:17:39.000000 OneOnOne-0.6947/OneOnOne.egg-info/dependency_links.txt
--rw-r--r--   0 sohinib    (501) staff       (20)      166 2023-07-24 16:17:39.000000 OneOnOne-0.6947/OneOnOne.egg-info/requires.txt
--rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-24 16:17:39.000000 OneOnOne-0.6947/OneOnOne.egg-info/top_level.txt
--rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-24 16:17:39.961527 OneOnOne-0.6947/PKG-INFO
--rw-r--r--   0 sohinib    (501) staff       (20)     3491 2023-07-24 15:56:25.000000 OneOnOne-0.6947/README.md
--rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-24 16:17:39.962036 OneOnOne-0.6947/setup.cfg
--rw-r--r--   0 sohinib    (501) staff       (20)     1972 2023-07-24 14:41:14.000000 OneOnOne-0.6947/setup.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-25 07:28:27.457652 OneOnOne-0.6948/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1076 2023-07-10 14:29:42.000000 OneOnOne-0.6948/LICENSE
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-25 07:28:27.450254 OneOnOne-0.6948/OneOnOne/
+-rw-r--r--   0 sohinib    (501) staff       (20)    55677 2023-07-25 06:44:50.000000 OneOnOne-0.6948/OneOnOne/__init__.py
+-rw-r--r--   0 sohinib    (501) staff       (20)  3312680 2023-07-07 06:05:06.000000 OneOnOne-0.6948/OneOnOne/classes.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    13595 2023-07-19 15:12:53.000000 OneOnOne-0.6948/OneOnOne/classification.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     5894 2023-07-22 03:02:07.000000 OneOnOne-0.6948/OneOnOne/contextdecider.py
+-rw-r--r--   0 sohinib    (501) staff       (20)      936 2023-07-19 15:12:54.000000 OneOnOne-0.6948/OneOnOne/htmlparser.py
+-rw-r--r--   0 sohinib    (501) staff       (20)     3047 2023-07-19 17:26:04.000000 OneOnOne-0.6948/OneOnOne/questionanswer.py
+-rw-r--r--   0 sohinib    (501) staff       (20)    20836 2023-07-19 15:12:54.000000 OneOnOne-0.6948/OneOnOne/sampling.py
+drwxr-xr-x   0 sohinib    (501) staff       (20)        0 2023-07-25 07:28:27.456045 OneOnOne-0.6948/OneOnOne.egg-info/
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)      351 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/SOURCES.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        1 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/dependency_links.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)      166 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/requires.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)        9 2023-07-25 07:28:27.000000 OneOnOne-0.6948/OneOnOne.egg-info/top_level.txt
+-rw-r--r--   0 sohinib    (501) staff       (20)     1578 2023-07-25 07:28:27.456916 OneOnOne-0.6948/PKG-INFO
+-rw-r--r--   0 sohinib    (501) staff       (20)     3491 2023-07-24 15:56:25.000000 OneOnOne-0.6948/README.md
+-rw-r--r--   0 sohinib    (501) staff       (20)       38 2023-07-25 07:28:27.457914 OneOnOne-0.6948/setup.cfg
+-rw-r--r--   0 sohinib    (501) staff       (20)     1972 2023-07-25 07:28:16.000000 OneOnOne-0.6948/setup.py
```

### Comparing `OneOnOne-0.6947/LICENSE` & `OneOnOne-0.6948/LICENSE`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6947/OneOnOne/__init__.py` & `OneOnOne-0.6948/OneOnOne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def __init__(self, model_type="resnet50", dataset="cifar10", samplingtype="none"):
         warnings.filterwarnings("ignore")
 
         self.model_type=model_type.lower()
         self.dataset=dataset.lower()
         self.samplingtype=samplingtype.lower()
 
-        self.map={"resnet50_cifar10_none":"1YVG0lAnpBfM_MB7ctV1vHcslb6O-3Vbm","resnet50_cifar10_leastconfidence":"1fSJYo5VOppTkgWb-Fu2Sf_JL4s9JUmoK","resnet50_cifar10_mixed":"","resnet50_cifar10_margin":"","efficientnetb6_cifar10_none":"16Wqfx7mcEhssZksF1yUAUEG6mkhMSeme","efficientnetb6_tinyimagenet_none":"1pGX8zB99ugqcvPohxykPC1JLM0Ld0L-D"}
+        self.map={"resnet50_cifar10_none":"1YVG0lAnpBfM_MB7ctV1vHcslb6O-3Vbm","resnet50_cifar10_leastconfidence":"1fSJYo5VOppTkgWb-Fu2Sf_JL4s9JUmoK","resnet50_cifar10_none_initial_10k":"1NOicX1WgVzgRPWwWM_LzPyNvnu5st5Kd","resnet50_cifar10_mixedbayes":"","resnet50_cifar10_margin":"","efficientnetb6_cifar10_none":"16Wqfx7mcEhssZksF1yUAUEG6mkhMSeme","efficientnetb6_tinyimagenet_none":"1pGX8zB99ugqcvPohxykPC1JLM0Ld0L-D"}
 
         if self.dataset=="tinyimagenet":
             self.model_type="efficientnetb6"
             self.samplingtype="none"
 
         self.model_name=f'{self.model_type}_{self.dataset}_{self.samplingtype}'
 
@@ -931,15 +931,15 @@
         self.X_train_copy=copy.deepcopy(self.X_train[self.first_data_samples:self.X_train.shape[0]])
         self.y_train_copy=copy.deepcopy(self.y_train[self.first_data_samples:self.X_train.shape[0]])
 
         for i in range(0,self.first_data_samples):
           self.y.append(self.y_train[i])
           self.x.append(self.X_train[i])
 
-        while (eval_metrics[1] < self.goal / 100)&(self.jump <= X_train_copy.shape[0]):
+        while (eval_metrics[1] < self.goal / 100)&(self.jump <= self.X_train_copy.shape[0]):
 
             total_index=[*range(0, self.X_train_copy.shape[0], 1)]
             y_predicted = self.model.predict(self.X_train_copy)
 
             if self.samplingtype== "margin":
               values = self.get_margin(y_predicted)
             elif self.samplingtype== "leastconfidence":
```

### Comparing `OneOnOne-0.6947/OneOnOne/classes.py` & `OneOnOne-0.6948/OneOnOne/classes.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6947/OneOnOne/classification.py` & `OneOnOne-0.6948/OneOnOne/classification.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6947/OneOnOne/contextdecider.py` & `OneOnOne-0.6948/OneOnOne/contextdecider.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6947/OneOnOne/htmlparser.py` & `OneOnOne-0.6948/OneOnOne/htmlparser.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6947/OneOnOne/questionanswer.py` & `OneOnOne-0.6948/OneOnOne/questionanswer.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6947/OneOnOne/sampling.py` & `OneOnOne-0.6948/OneOnOne/sampling.py`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6947/OneOnOne.egg-info/PKG-INFO` & `OneOnOne-0.6948/OneOnOne.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6947
+Version: 0.6948
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6947/PKG-INFO` & `OneOnOne-0.6948/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OneOnOne
-Version: 0.6947
+Version: 0.6948
 Summary: A package for pre-trained image classification and context-decider for question-answering chatbots.
 Author: Sohini Bhattacharya
 Author-email: mail.sohinibhattacharya@gmail.com
 Keywords: python,image-classification,active-learning-sampling,question-answering,pre-trained models,tiny-image-net,cifar10
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `OneOnOne-0.6947/README.md` & `OneOnOne-0.6948/README.md`

 * *Files identical despite different names*

### Comparing `OneOnOne-0.6947/setup.py` & `OneOnOne-0.6948/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION=0.6947
+VERSION=0.6948
 
 DESCRIPTION="A package for pre-trained image classification and context-decider for question-answering chatbots."
 LONG_DESCRIPTION="Your one-stop destination to utilize image-classification models with just one line of code. A library meant to simplify your life by providing you with pre-trained models like ResNet50, EfficientNetVB6, VGG19, etc. You can simply opt for training your own models from scratch by just tweaking a few values. If you want to try popular active-learning sampling methods on image classification, no need to worry! This library has got you covered. Along with that for simple-bridging and basic into NLP, we have context-deciders, HTML parsers and simple chatbot object classes, to create an interface similar to Google Lens. You input an image or item that you are curious about and you can ask one-on-one questions from the chatbot. This is made possible by using the tiny imagenet dataset. This library is being actively updated and new features are being added frequently. New datasets and pre-trained models will be updated soon. Feel free to share your feedback! I would really appreciate it!"
 CLASSIFIERS=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Education',
     'License :: OSI Approved :: MIT License',
```

