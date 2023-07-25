# Comparing `tmp/bert4torch-0.3.1.tar.gz` & `tmp/bert4torch-0.3.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert4torch-0.3.1.tar", last modified: Mon Jul 24 16:10:44 2023, max compression
+gzip compressed data, was "bert4torch-0.3.1.post2.tar", last modified: Tue Jul 25 16:14:03 2023, max compression
```

## Comparing `bert4torch-0.3.1.tar` & `bert4torch-0.3.1.post2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.773348 bert4torch-0.3.1/
--rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.3.1/LICENSE
--rw-rw-rw-   0        0        0    27568 2023-07-24 16:10:44.771352 bert4torch-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    27316 2023-07-24 16:05:28.000000 bert4torch-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.728347 bert4torch-0.3.1/bert4torch/
--rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.3.1/bert4torch/__init__.py
--rw-rw-rw-   0        0        0     3228 2023-06-30 17:02:35.000000 bert4torch-0.3.1/bert4torch/activations.py
--rw-rw-rw-   0        0        0    10939 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/callbacks.py
--rw-rw-rw-   0        0        0    40539 2023-07-19 13:35:56.000000 bert4torch-0.3.1/bert4torch/generation.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.743347 bert4torch-0.3.1/bert4torch/layers/
--rw-rw-rw-   0        0        0      296 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/layers/__init__.py
--rw-rw-rw-   0        0        0    25499 2023-07-19 14:29:14.000000 bert4torch-0.3.1/bert4torch/layers/attention.py
--rw-rw-rw-   0        0        0     8515 2023-07-15 16:04:22.000000 bert4torch-0.3.1/bert4torch/layers/core.py
--rw-rw-rw-   0        0        0    12699 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/layers/crf.py
--rw-rw-rw-   0        0        0     4738 2023-07-20 15:32:46.000000 bert4torch-0.3.1/bert4torch/layers/global_point.py
--rw-rw-rw-   0        0        0    17536 2023-07-22 13:42:00.000000 bert4torch-0.3.1/bert4torch/layers/misc.py
--rw-rw-rw-   0        0        0    13868 2023-07-19 14:29:40.000000 bert4torch-0.3.1/bert4torch/layers/position_encoding.py
--rw-rw-rw-   0        0        0    16281 2023-07-21 13:58:57.000000 bert4torch-0.3.1/bert4torch/layers/transformer_block.py
--rw-rw-rw-   0        0        0    16631 2023-06-26 16:27:26.000000 bert4torch-0.3.1/bert4torch/losses.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.768351 bert4torch-0.3.1/bert4torch/models/
--rw-rw-rw-   0        0        0     7712 2023-07-18 14:14:06.000000 bert4torch-0.3.1/bert4torch/models/__init__.py
--rw-rw-rw-   0        0        0     7811 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/albert.py
--rw-rw-rw-   0        0        0     6913 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/bart.py
--rw-rw-rw-   0        0        0    20254 2023-07-16 10:07:15.000000 bert4torch-0.3.1/bert4torch/models/base.py
--rw-rw-rw-   0        0        0    18082 2023-07-11 14:03:23.000000 bert4torch-0.3.1/bert4torch/models/bert.py
--rw-rw-rw-   0        0        0      760 2023-07-22 15:51:05.000000 bert4torch-0.3.1/bert4torch/models/bloom.py
--rw-rw-rw-   0        0        0     4283 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/deberta.py
--rw-rw-rw-   0        0        0     2233 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/electra.py
--rw-rw-rw-   0        0        0      932 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/erinie.py
--rw-rw-rw-   0        0        0     1728 2023-07-11 14:03:23.000000 bert4torch-0.3.1/bert4torch/models/gau_alpha.py
--rw-rw-rw-   0        0        0    10808 2023-07-22 14:30:17.000000 bert4torch-0.3.1/bert4torch/models/glm.py
--rw-rw-rw-   0        0        0     4566 2023-07-22 13:03:58.000000 bert4torch-0.3.1/bert4torch/models/gpt.py
--rw-rw-rw-   0        0        0     2294 2023-07-22 13:18:50.000000 bert4torch-0.3.1/bert4torch/models/llama.py
--rw-rw-rw-   0        0        0      457 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/nezha.py
--rw-rw-rw-   0        0        0     2399 2023-07-11 14:03:23.000000 bert4torch-0.3.1/bert4torch/models/roformer.py
--rw-rw-rw-   0        0        0    10336 2023-07-21 13:58:57.000000 bert4torch-0.3.1/bert4torch/models/t5.py
--rw-rw-rw-   0        0        0     6769 2023-07-22 13:26:18.000000 bert4torch-0.3.1/bert4torch/models/transformer.py
--rw-rw-rw-   0        0        0     9219 2023-07-20 15:32:46.000000 bert4torch-0.3.1/bert4torch/models/transformer_xl.py
--rw-rw-rw-   0        0        0     2469 2023-07-06 12:55:22.000000 bert4torch-0.3.1/bert4torch/models/uie.py
--rw-rw-rw-   0        0        0     4808 2023-07-20 15:32:46.000000 bert4torch-0.3.1/bert4torch/models/xlnet.py
--rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.3.1/bert4torch/optimizers.py
--rw-rw-rw-   0        0        0    20808 2023-07-16 10:34:11.000000 bert4torch-0.3.1/bert4torch/quantization.py
--rw-rw-rw-   0        0        0    23410 2023-07-16 10:34:24.000000 bert4torch-0.3.1/bert4torch/snippets.py
--rw-rw-rw-   0        0        0    35456 2023-07-13 15:00:01.000000 bert4torch-0.3.1/bert4torch/tokenizers.py
-drwxrwxrwx   0        0        0        0 2023-07-24 16:10:44.732346 bert4torch-0.3.1/bert4torch.egg-info/
--rw-rw-rw-   0        0        0    27568 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-24 16:10:44.000000 bert4torch-0.3.1/bert4torch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 16:10:44.774347 bert4torch-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-07-24 16:05:33.000000 bert4torch-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.875301 bert4torch-0.3.1.post2/
+-rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.3.1.post2/LICENSE
+-rw-rw-rw-   0        0        0    27580 2023-07-25 16:14:03.874314 bert4torch-0.3.1.post2/PKG-INFO
+-rw-rw-rw-   0        0        0    27322 2023-07-25 16:13:19.000000 bert4torch-0.3.1.post2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.831302 bert4torch-0.3.1.post2/bert4torch/
+-rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.3.1.post2/bert4torch/__init__.py
+-rw-rw-rw-   0        0        0     3228 2023-06-30 17:02:35.000000 bert4torch-0.3.1.post2/bert4torch/activations.py
+-rw-rw-rw-   0        0        0    10939 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/callbacks.py
+-rw-rw-rw-   0        0        0    40539 2023-07-19 13:35:56.000000 bert4torch-0.3.1.post2/bert4torch/generation.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.846301 bert4torch-0.3.1.post2/bert4torch/layers/
+-rw-rw-rw-   0        0        0      296 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/layers/__init__.py
+-rw-rw-rw-   0        0        0    25499 2023-07-19 14:29:14.000000 bert4torch-0.3.1.post2/bert4torch/layers/attention.py
+-rw-rw-rw-   0        0        0     8515 2023-07-15 16:04:22.000000 bert4torch-0.3.1.post2/bert4torch/layers/core.py
+-rw-rw-rw-   0        0        0    12699 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/layers/crf.py
+-rw-rw-rw-   0        0        0     4738 2023-07-20 15:32:46.000000 bert4torch-0.3.1.post2/bert4torch/layers/global_point.py
+-rw-rw-rw-   0        0        0    17536 2023-07-22 13:42:00.000000 bert4torch-0.3.1.post2/bert4torch/layers/misc.py
+-rw-rw-rw-   0        0        0    13868 2023-07-19 14:29:40.000000 bert4torch-0.3.1.post2/bert4torch/layers/position_encoding.py
+-rw-rw-rw-   0        0        0    16281 2023-07-21 13:58:57.000000 bert4torch-0.3.1.post2/bert4torch/layers/transformer_block.py
+-rw-rw-rw-   0        0        0    16631 2023-06-26 16:27:26.000000 bert4torch-0.3.1.post2/bert4torch/losses.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.872309 bert4torch-0.3.1.post2/bert4torch/models/
+-rw-rw-rw-   0        0        0     7712 2023-07-18 14:14:06.000000 bert4torch-0.3.1.post2/bert4torch/models/__init__.py
+-rw-rw-rw-   0        0        0     7811 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/albert.py
+-rw-rw-rw-   0        0        0     6913 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/bart.py
+-rw-rw-rw-   0        0        0    20254 2023-07-16 10:07:15.000000 bert4torch-0.3.1.post2/bert4torch/models/base.py
+-rw-rw-rw-   0        0        0    18082 2023-07-11 14:03:23.000000 bert4torch-0.3.1.post2/bert4torch/models/bert.py
+-rw-rw-rw-   0        0        0      760 2023-07-22 15:51:05.000000 bert4torch-0.3.1.post2/bert4torch/models/bloom.py
+-rw-rw-rw-   0        0        0     4283 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/deberta.py
+-rw-rw-rw-   0        0        0     2233 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/electra.py
+-rw-rw-rw-   0        0        0      932 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/erinie.py
+-rw-rw-rw-   0        0        0     1728 2023-07-11 14:03:23.000000 bert4torch-0.3.1.post2/bert4torch/models/gau_alpha.py
+-rw-rw-rw-   0        0        0    10808 2023-07-22 14:30:17.000000 bert4torch-0.3.1.post2/bert4torch/models/glm.py
+-rw-rw-rw-   0        0        0     4566 2023-07-22 13:03:58.000000 bert4torch-0.3.1.post2/bert4torch/models/gpt.py
+-rw-rw-rw-   0        0        0     2294 2023-07-22 13:18:50.000000 bert4torch-0.3.1.post2/bert4torch/models/llama.py
+-rw-rw-rw-   0        0        0      457 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/nezha.py
+-rw-rw-rw-   0        0        0     2399 2023-07-11 14:03:23.000000 bert4torch-0.3.1.post2/bert4torch/models/roformer.py
+-rw-rw-rw-   0        0        0    10336 2023-07-21 13:58:57.000000 bert4torch-0.3.1.post2/bert4torch/models/t5.py
+-rw-rw-rw-   0        0        0     6769 2023-07-22 13:26:18.000000 bert4torch-0.3.1.post2/bert4torch/models/transformer.py
+-rw-rw-rw-   0        0        0     9219 2023-07-20 15:32:46.000000 bert4torch-0.3.1.post2/bert4torch/models/transformer_xl.py
+-rw-rw-rw-   0        0        0     2469 2023-07-06 12:55:22.000000 bert4torch-0.3.1.post2/bert4torch/models/uie.py
+-rw-rw-rw-   0        0        0     4808 2023-07-20 15:32:46.000000 bert4torch-0.3.1.post2/bert4torch/models/xlnet.py
+-rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.3.1.post2/bert4torch/optimizers.py
+-rw-rw-rw-   0        0        0    20808 2023-07-16 10:34:11.000000 bert4torch-0.3.1.post2/bert4torch/quantization.py
+-rw-rw-rw-   0        0        0    23410 2023-07-16 10:34:24.000000 bert4torch-0.3.1.post2/bert4torch/snippets.py
+-rw-rw-rw-   0        0        0    35456 2023-07-13 15:00:01.000000 bert4torch-0.3.1.post2/bert4torch/tokenizers.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:14:03.837291 bert4torch-0.3.1.post2/bert4torch.egg-info/
+-rw-rw-rw-   0        0        0    27580 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-25 16:14:03.000000 bert4torch-0.3.1.post2/bert4torch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 16:14:03.875301 bert4torch-0.3.1.post2/setup.cfg
+-rw-rw-rw-   0        0        0      563 2023-07-25 16:12:24.000000 bert4torch-0.3.1.post2/setup.py
```

### Comparing `bert4torch-0.3.1/LICENSE` & `bert4torch-0.3.1.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/PKG-INFO` & `bert4torch-0.3.1.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert4torch
-Version: 0.3.1
+Version: 0.3.1.post2
 Summary: an elegant bert4torch
 Home-page: https://github.com/Tongjilibo/bert4torch
 Author: Tongjilibo
 License: MIT Licence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -85,15 +85,15 @@
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
-- **v0.3.1**：20230725 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
+- **v0.3.1.post2**：20230726 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
@@ -110,15 +110,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
-| 0.3.1          | 0.1.0           |
+| 0.3.1.post2    | 0.1.0.post2     |
 | 0.3.0          | 0.0.9           |
 | 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
@@ -128,15 +128,15 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
-- **20230725**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
+- **20230726**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
```

### Comparing `bert4torch-0.3.1/README.md` & `bert4torch-0.3.1.post2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
-- **v0.3.1**：20230725 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
+- **v0.3.1.post2**：20230726 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
@@ -100,15 +100,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
-| 0.3.1          | 0.1.0           |
+| 0.3.1.post2    | 0.1.0.post2     |
 | 0.3.0          | 0.0.9           |
 | 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
@@ -118,15 +118,15 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
-- **20230725**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
+- **20230726**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
```

### Comparing `bert4torch-0.3.1/bert4torch/activations.py` & `bert4torch-0.3.1.post2/bert4torch/activations.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/callbacks.py` & `bert4torch-0.3.1.post2/bert4torch/callbacks.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/generation.py` & `bert4torch-0.3.1.post2/bert4torch/generation.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/layers/attention.py` & `bert4torch-0.3.1.post2/bert4torch/layers/attention.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/layers/core.py` & `bert4torch-0.3.1.post2/bert4torch/layers/core.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/layers/crf.py` & `bert4torch-0.3.1.post2/bert4torch/layers/crf.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/layers/global_point.py` & `bert4torch-0.3.1.post2/bert4torch/layers/global_point.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/layers/misc.py` & `bert4torch-0.3.1.post2/bert4torch/layers/misc.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/layers/position_encoding.py` & `bert4torch-0.3.1.post2/bert4torch/layers/position_encoding.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/layers/transformer_block.py` & `bert4torch-0.3.1.post2/bert4torch/layers/transformer_block.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/losses.py` & `bert4torch-0.3.1.post2/bert4torch/losses.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/__init__.py` & `bert4torch-0.3.1.post2/bert4torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/albert.py` & `bert4torch-0.3.1.post2/bert4torch/models/albert.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/bart.py` & `bert4torch-0.3.1.post2/bert4torch/models/bart.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/base.py` & `bert4torch-0.3.1.post2/bert4torch/models/base.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/bert.py` & `bert4torch-0.3.1.post2/bert4torch/models/bert.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/bloom.py` & `bert4torch-0.3.1.post2/bert4torch/models/bloom.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/deberta.py` & `bert4torch-0.3.1.post2/bert4torch/models/deberta.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/electra.py` & `bert4torch-0.3.1.post2/bert4torch/models/electra.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/erinie.py` & `bert4torch-0.3.1.post2/bert4torch/models/erinie.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/gau_alpha.py` & `bert4torch-0.3.1.post2/bert4torch/models/gau_alpha.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/glm.py` & `bert4torch-0.3.1.post2/bert4torch/models/glm.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/gpt.py` & `bert4torch-0.3.1.post2/bert4torch/models/gpt.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/llama.py` & `bert4torch-0.3.1.post2/bert4torch/models/llama.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/roformer.py` & `bert4torch-0.3.1.post2/bert4torch/models/roformer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/t5.py` & `bert4torch-0.3.1.post2/bert4torch/models/t5.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/transformer.py` & `bert4torch-0.3.1.post2/bert4torch/models/transformer.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/transformer_xl.py` & `bert4torch-0.3.1.post2/bert4torch/models/transformer_xl.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/uie.py` & `bert4torch-0.3.1.post2/bert4torch/models/uie.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/models/xlnet.py` & `bert4torch-0.3.1.post2/bert4torch/models/xlnet.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/optimizers.py` & `bert4torch-0.3.1.post2/bert4torch/optimizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/quantization.py` & `bert4torch-0.3.1.post2/bert4torch/quantization.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/snippets.py` & `bert4torch-0.3.1.post2/bert4torch/snippets.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch/tokenizers.py` & `bert4torch-0.3.1.post2/bert4torch/tokenizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/bert4torch.egg-info/PKG-INFO` & `bert4torch-0.3.1.post2/bert4torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert4torch
-Version: 0.3.1
+Version: 0.3.1.post2
 Summary: an elegant bert4torch
 Home-page: https://github.com/Tongjilibo/bert4torch
 Author: Tongjilibo
 License: MIT Licence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -85,15 +85,15 @@
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
-- **v0.3.1**：20230725 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
+- **v0.3.1.post2**：20230726 修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
@@ -110,15 +110,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
-| 0.3.1          | 0.1.0           |
+| 0.3.1.post2    | 0.1.0.post2     |
 | 0.3.0          | 0.0.9           |
 | 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
@@ -128,15 +128,15 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
-- **20230725**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
+- **20230726**：修改baichuan的alibi逻辑，增加bloom, 简化decoder架构代码(gpt, llama, chatglm均继承decoder)
 - **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
 - **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
```

### Comparing `bert4torch-0.3.1/bert4torch.egg-info/SOURCES.txt` & `bert4torch-0.3.1.post2/bert4torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bert4torch-0.3.1/setup.py` & `bert4torch-0.3.1.post2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='bert4torch',
-    version='v0.3.1',
+    version='v0.3.1.post2',
     description='an elegant bert4torch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT Licence',
     url='https://github.com/Tongjilibo/bert4torch',
     author='Tongjilibo',
-    install_requires=['torch>1.6', 'torch4keras==0.1.0'],
+    install_requires=['torch>1.6', 'torch4keras==0.1.0.post2'],
     packages=find_packages()
 )
```

