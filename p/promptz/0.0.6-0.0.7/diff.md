# Comparing `tmp/promptz-0.0.6.tar.gz` & `tmp/promptz-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptz-0.0.6.tar", last modified: Tue Jul 25 16:23:18 2023, max compression
+gzip compressed data, was "promptz-0.0.7.tar", last modified: Tue Jul 25 16:38:40 2023, max compression
```

## Comparing `promptz-0.0.6.tar` & `promptz-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:23:18.126548 promptz-0.0.6/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:23:18.126548 promptz-0.0.6/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)    14608 2023-07-25 15:57:54.000000 promptz-0.0.6/README.md
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:23:18.126548 promptz-0.0.6/promptz/
--rw-r--r--   0 rjl       (1000) rjl       (1000)    40171 2023-07-25 16:20:12.000000 promptz-0.0.6/promptz/__init__.py
--rw-r--r--   0 rjl       (1000) rjl       (1000)      151 2023-05-17 11:33:35.000000 promptz-0.0.6/promptz/main.py
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:23:18.126548 promptz-0.0.6/promptz.egg-info/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)      208 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/SOURCES.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/dependency_links.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)     2122 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/requires.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-25 16:23:18.000000 promptz-0.0.6/promptz.egg-info/top_level.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-25 16:23:18.126548 promptz-0.0.6/setup.cfg
--rw-r--r--   0 rjl       (1000) rjl       (1000)      278 2023-07-25 16:23:00.000000 promptz-0.0.6/setup.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:38:40.459707 promptz-0.0.7/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:38:40.459707 promptz-0.0.7/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    14608 2023-07-25 15:57:54.000000 promptz-0.0.7/README.md
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:38:40.459707 promptz-0.0.7/promptz/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    38967 2023-07-25 16:37:29.000000 promptz-0.0.7/promptz/__init__.py
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      151 2023-05-17 11:33:35.000000 promptz-0.0.7/promptz/main.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:38:40.459707 promptz-0.0.7/promptz.egg-info/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      208 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/SOURCES.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/dependency_links.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)     2089 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/requires.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/top_level.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-25 16:38:40.459707 promptz-0.0.7/setup.cfg
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      278 2023-07-25 16:37:35.000000 promptz-0.0.7/setup.py
```

### Comparing `promptz-0.0.6/README.md` & `promptz-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `promptz-0.0.6/promptz/__init__.py` & `promptz-0.0.7/promptz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,26 @@
-import sys
 import os
-import io
-from io import BytesIO
 import inspect
 import logging
 import random
 import uuid
 import textwrap
-import base64
 import json
 from json import JSONDecodeError
 from enum import Enum
 from typing import Type, Callable, List, Tuple, Dict, Union, Any, Literal 
 from abc import abstractmethod
-from PIL import Image
-import matplotlib.pyplot as plt
 import torch
 from torch import nn
 import numpy as np
 import pandas as pd
 from jinja2 import Template
-from pydantic import BaseModel, ValidationError, validate_model
-from pydantic.fields import ModelField
-from pydantic import EmailStr, IPvAnyAddress, PositiveInt, NegativeInt, NameEmail, ConstrainedStr, ConstrainedBytes
-from datetime import datetime, date, time, timedelta
+from pydantic import BaseModel, ValidationError 
+from datetime import datetime
 from transformers import PreTrainedModel, PreTrainedTokenizer, LlamaForCausalLM, LlamaTokenizer
-from diffusers import DiffusionPipeline
 import openai
 from openai.error import RateLimitError
 import chromadb
 import colorama
 
 colorama.just_fix_windows_console()
 
@@ -303,46 +294,14 @@
                 model=f'{self.__class__.__name__}.{self.model}',
                 input_tokens=output.usage.get('prompt_tokens'),
                 output_tokens=output.usage.get('completion_tokens')
             ),
         )
 
 
-class ImageResponse(Response):
-
-    def __repr__(self) -> str:
-        image_bytes = base64.b64decode(self.content)
-        image = Image.open(io.BytesIO(image_bytes))
-        plt.imshow(image)
-        plt.axis('off')
-        plt.show()
-        return ''
-
-
-class HuggingfaceDiffuser(LLM):
-    pipeline: DiffusionPipeline
-
-    def __init__(self, pipeline=None, model=None):
-        self.pipeline = pipeline
-    
-    def generate(self, x, **kwargs) -> Response:
-        output = self.pipeline(x)
-        image = output.images[0]
-        buffered = BytesIO()
-        image.save(buffered, format="PNG")
-        image_str = base64.b64encode(buffered.getvalue()).decode()
-        return Response(
-            raw=image,
-            metrics=Metrics(
-                model=f'{self.__class__.__name__}',
-                input_tokens=len(x),
-            ),
-        )
-
-
 class HuggingfaceTransformer(LLM):
     model: PreTrainedModel
     tokenizer: PreTrainedTokenizer
     max_length: int
 
     def __init__(self, model, tokenizer, max_length=50, **kwargs):
         self.model = model
```

### Comparing `promptz-0.0.6/promptz.egg-info/requires.txt` & `promptz-0.0.7/promptz.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 Jinja2==3.1.2
 MarkupSafe==2.1.3
-Pillow==10.0.0
 PyPika==0.48.9
 PyYAML==6.0.1
 Pygments==2.15.1
 aiohttp==3.8.5
 aiosignal==1.3.1
 anyio==3.7.1
 asttokens==2.2.1
@@ -21,15 +20,14 @@
 colorama==0.4.6
 coloredlogs==15.0.1
 comm==0.1.3
 contourpy==1.1.0
 cycler==0.11.0
 debugpy==1.6.7
 decorator==5.1.1
-diffusers==0.18.2
 exceptiongroup==1.1.2
 executing==1.2.0
 fastapi==0.99.1
 filelock==3.12.2
 fire==0.5.0
 flatbuffers==23.5.26
 fonttools==4.41.1
```

