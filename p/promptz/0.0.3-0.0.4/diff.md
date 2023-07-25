# Comparing `tmp/promptz-0.0.3.tar.gz` & `tmp/promptz-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptz-0.0.3.tar", last modified: Tue Jul 25 16:15:07 2023, max compression
+gzip compressed data, was "promptz-0.0.4.tar", last modified: Tue Jul 25 16:18:30 2023, max compression
```

## Comparing `promptz-0.0.3.tar` & `promptz-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:15:07.398233 promptz-0.0.3/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:15:07.398233 promptz-0.0.3/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)    14608 2023-07-25 15:57:54.000000 promptz-0.0.3/README.md
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:15:07.398233 promptz-0.0.3/promptz/
--rw-r--r--   0 rjl       (1000) rjl       (1000)    43438 2023-07-25 16:05:27.000000 promptz-0.0.3/promptz/__init__.py
--rw-r--r--   0 rjl       (1000) rjl       (1000)      151 2023-05-17 11:33:35.000000 promptz-0.0.3/promptz/main.py
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:15:07.398233 promptz-0.0.3/promptz.egg-info/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:15:07.000000 promptz-0.0.3/promptz.egg-info/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)      178 2023-07-25 16:15:07.000000 promptz-0.0.3/promptz.egg-info/SOURCES.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-25 16:15:07.000000 promptz-0.0.3/promptz.egg-info/dependency_links.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-25 16:15:07.000000 promptz-0.0.3/promptz.egg-info/top_level.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-25 16:15:07.398233 promptz-0.0.3/setup.cfg
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:14:54.000000 promptz-0.0.3/setup.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:18:30.952749 promptz-0.0.4/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:18:30.952749 promptz-0.0.4/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    14608 2023-07-25 15:57:54.000000 promptz-0.0.4/README.md
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:18:30.952749 promptz-0.0.4/promptz/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    40426 2023-07-25 16:17:50.000000 promptz-0.0.4/promptz/__init__.py
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      151 2023-05-17 11:33:35.000000 promptz-0.0.4/promptz/main.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:18:30.952749 promptz-0.0.4/promptz.egg-info/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:18:30.000000 promptz-0.0.4/promptz.egg-info/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      178 2023-07-25 16:18:30.000000 promptz-0.0.4/promptz.egg-info/SOURCES.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-25 16:18:30.000000 promptz-0.0.4/promptz.egg-info/dependency_links.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-25 16:18:30.000000 promptz-0.0.4/promptz.egg-info/top_level.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-25 16:18:30.952749 promptz-0.0.4/setup.cfg
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:18:18.000000 promptz-0.0.4/setup.py
```

### Comparing `promptz-0.0.3/README.md` & `promptz-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `promptz-0.0.3/promptz/__init__.py` & `promptz-0.0.4/promptz/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from PIL import Image
 import matplotlib.pyplot as plt
 import torch
 from torch import nn
 import numpy as np
 import pandas as pd
 from jinja2 import Template
-from faker import Faker
 from pythonjsonlogger import jsonlogger
 from pydantic import BaseModel, ValidationError, validate_model
 from pydantic.fields import ModelField
 from pydantic import EmailStr, IPvAnyAddress, PositiveInt, NegativeInt, NameEmail, ConstrainedStr, ConstrainedBytes
 from datetime import datetime, date, time, timedelta
 from transformers import PreTrainedModel, PreTrainedTokenizer, LlamaForCausalLM, LlamaTokenizer
 from diffusers import DiffusionPipeline
@@ -216,87 +215,28 @@
 class MockLLM(LLM):
     response_length: int 
     output = None
 
     def __init__(self, response_length=1000, output=None):
         self.response_length = response_length
         self.output = output
-        self.fake = Faker()
 
     def generate(self, x, tools=None, **kwargs):
         if self.output is None:
             response = 'This is a mock response.'
         elif isinstance(self.output, BaseModel):
-            response = self._create_output(x).json()
+            response = ''
         return Response(
             raw=response,
             metrics=Metrics(
                 model='mock',
                 input_tokens=len(x),
                 output_tokens=self.response_length,
             ),
         )
-    
-    def _get_field_data(self, model_field: ModelField):
-        field_info = model_field.field_info
-        field_type = model_field.outer_type_
-
-        if field_type is str:
-            return self.fake.pystr(min_chars=field_info.min_length or 10, max_chars=field_info.max_length or 140)
-        elif field_type is int:
-            return self.fake.random_int(min=field_info.ge or 0, max=field_info.le or 1000)
-        elif field_type is EmailStr:
-            return self.fake.email()
-        elif field_type is IPvAnyAddress:
-            return self.fake.ipv4_public(network=False)
-        elif field_type is PositiveInt:
-            return self.fake.pyint(min_value=1)
-        elif field_type is NegativeInt:
-            return -self.fake.pyint(min_value=1)
-        elif field_type is datetime:
-            return self.fake.date_time_this_decade()
-        elif field_type is date:
-            return self.fake.date_object()
-        elif field_type is time:
-            return self.fake.time_object()
-        elif field_type is timedelta:
-            return timedelta(days=self.fake.random_digit())
-        elif field_type is uuid.UUID:
-            return uuid.uuid4()
-        elif field_type is NameEmail:
-            return f"{self.fake.name()} <{self.fake.email()}>"
-        elif field_type is ConstrainedStr:
-            return self.fake.pystr(min_chars=field_info.min_length or 10, max_chars=field_info.max_length or 140)
-        elif field_type is ConstrainedBytes:
-            return self.fake.binary(length=field_info.max_length)
-        elif hasattr(field_type, '__origin__'):
-            if field_type.__origin__ is list:
-                inner_type = field_type.__args__[0]
-                inner_field = ModelField(name=model_field.name, type_=inner_type, class_validators={}, model_config=model_field.model_config)
-                return [self.get_field_data(inner_field) for _ in range(5)] # Generate a list of 5 elements
-            elif field_type.__origin__ is dict:
-                inner_type = field_type.__args__[1]
-                inner_field = ModelField(name=model_field.name, type_=inner_type, class_validators={}, model_config=model_field.model_config)
-                return {f'key{i}': self.get_field_data(inner_field) for i in range(5)} # Generate a dictionary of 5 key-value pairs
-        elif issubclass(field_type, BaseModel):
-            return self._create_output(field_type)
-
-    def _create_output(self, x):
-        generated_data = {}
-
-        for field, field_type in self.output.__annotations__.items():
-            model_field = ModelField(name=field, type_=field_type, class_validators={}, model_config=self.output.__config__)
-            generated_data[field] = self._get_field_data(model_field)
-
-        validated_data, _, err = validate_model(self.output, generated_data)
-        if err:
-            raise err
-
-        instance = self.output(**validated_data)
-        return instance
 
 
 class GPT(LLM):
     model = 'text-davinci-003'
 
     def __init__(self, model=None):
         self.model = model or self.model
```

