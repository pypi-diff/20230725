# Comparing `tmp/torch4keras-0.1.0.tar.gz` & `tmp/torch4keras-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4keras-0.1.0.tar", last modified: Mon Jul 24 13:32:48 2023, max compression
+gzip compressed data, was "torch4keras-0.1.0.post2.tar", last modified: Tue Jul 25 16:05:39 2023, max compression
```

## Comparing `torch4keras-0.1.0.tar` & `torch4keras-0.1.0.post2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 13:32:48.543826 torch4keras-0.1.0/
--rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     7963 2023-07-24 13:32:48.542829 torch4keras-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7709 2023-07-24 12:53:02.000000 torch4keras-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 13:32:48.543826 torch4keras-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      522 2023-07-22 16:30:44.000000 torch4keras-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 13:32:48.524417 torch4keras-0.1.0/torch4keras/
--rw-rw-rw-   0        0        0        0 2023-05-30 14:28:06.000000 torch4keras-0.1.0/torch4keras/__init__.py
--rw-rw-rw-   0        0        0    53316 2023-07-24 12:53:02.000000 torch4keras-0.1.0/torch4keras/callbacks.py
--rw-rw-rw-   0        0        0    31227 2023-07-24 12:53:02.000000 torch4keras-0.1.0/torch4keras/model.py
--rw-rw-rw-   0        0        0    17219 2023-07-24 12:53:02.000000 torch4keras-0.1.0/torch4keras/snippets.py
-drwxrwxrwx   0        0        0        0 2023-07-24 13:32:48.541824 torch4keras-0.1.0/torch4keras.egg-info/
--rw-rw-rw-   0        0        0     7963 2023-07-24 13:32:48.000000 torch4keras-0.1.0/torch4keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-24 13:32:48.000000 torch4keras-0.1.0/torch4keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 13:32:48.000000 torch4keras-0.1.0/torch4keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-24 13:32:48.000000 torch4keras-0.1.0/torch4keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 16:05:39.880020 torch4keras-0.1.0.post2/
+-rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.1.0.post2/LICENSE
+-rw-rw-rw-   0        0        0     8165 2023-07-25 16:05:39.870512 torch4keras-0.1.0.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     7905 2023-07-25 16:05:19.000000 torch4keras-0.1.0.post2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-25 16:05:39.880020 torch4keras-0.1.0.post2/setup.cfg
+-rw-rw-rw-   0        0        0      528 2023-07-25 15:47:02.000000 torch4keras-0.1.0.post2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:05:39.864512 torch4keras-0.1.0.post2/torch4keras/
+-rw-rw-rw-   0        0        0        0 2023-05-30 14:28:06.000000 torch4keras-0.1.0.post2/torch4keras/__init__.py
+-rw-rw-rw-   0        0        0    50431 2023-07-25 15:59:20.000000 torch4keras-0.1.0.post2/torch4keras/callbacks.py
+-rw-rw-rw-   0        0        0    31097 2023-07-25 15:49:22.000000 torch4keras-0.1.0.post2/torch4keras/model.py
+-rw-rw-rw-   0        0        0    17218 2023-07-25 15:39:03.000000 torch4keras-0.1.0.post2/torch4keras/snippets.py
+drwxrwxrwx   0        0        0        0 2023-07-25 16:05:39.869512 torch4keras-0.1.0.post2/torch4keras.egg-info/
+-rw-rw-rw-   0        0        0     8165 2023-07-25 16:05:39.000000 torch4keras-0.1.0.post2/torch4keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-25 16:05:39.000000 torch4keras-0.1.0.post2/torch4keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 16:05:39.000000 torch4keras-0.1.0.post2/torch4keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-25 16:05:39.000000 torch4keras-0.1.0.post2/torch4keras.egg-info/top_level.txt
```

### Comparing `torch4keras-0.1.0/LICENSE` & `torch4keras-0.1.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch4keras-0.1.0/PKG-INFO` & `torch4keras-0.1.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.1.0
+Version: 0.1.0.post2
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -71,30 +71,32 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
-- **v0.1.0**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
+- **v0.1.0.post2**: 20230725 修复v0.1.0的bug，主要是进度条和log的标签平滑的问题
+- **v0.1.0**: 20230724 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **v0.0.9**：20230716 增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **v0.0.8**：20230625 增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **v0.0.7.post3**: 20230517 修复保存scheduler
 - **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
-- **20230721**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
+- **20230725**: 修复v0.1.0的bug，主要是进度条和log的标签平滑的问题
+- **20230724**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
```

### Comparing `torch4keras-0.1.0/README.md` & `torch4keras-0.1.0.post2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,30 +61,32 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
-- **v0.1.0**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
+- **v0.1.0.post2**: 20230725 修复v0.1.0的bug，主要是进度条和log的标签平滑的问题
+- **v0.1.0**: 20230724 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **v0.0.9**：20230716 增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **v0.0.8**：20230625 增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **v0.0.7.post3**: 20230517 修复保存scheduler
 - **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
-- **20230721**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
+- **20230725**: 修复v0.1.0的bug，主要是进度条和log的标签平滑的问题
+- **20230724**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
```

### Comparing `torch4keras-0.1.0/setup.py` & `torch4keras-0.1.0.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='torch4keras',
-    version='v0.1.0',
+    version='v0.1.0.post2',
     description='Use torch like keras',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License',
     url='https://github.com/Tongjilibo/torch4keras',
     author='Tongjilibo',
     install_requires=[],
```

### Comparing `torch4keras-0.1.0/torch4keras/callbacks.py` & `torch4keras-0.1.0.post2/torch4keras/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def update(self, current, values=None):
         """Updates the progress bar."""
         values = values or []
         for k, v in values:
             if k not in self.stateful_metrics:
                 if k not in self._values:
                     self._values[k] = [v * (current - self._seen_so_far), current - self._seen_so_far]
-                elif (self.smooth_interval is not None) and (current % self.smooth_interval == 0):
+                elif (self.smooth_interval is not None) and (current % self.smooth_interval == 1):
                     # 如果定义了累积smooth_interval，则需要重新累计
                     self._values[k] = [v, 1]
                 else:
                     self._values[k][0] += v * (current - self._seen_so_far)
                     self._values[k][1] += (current - self._seen_so_far)
             else:
                 # Stateful metrics output a numeric value.  This representation
@@ -324,54 +324,14 @@
         pass
     def on_dataloader_end(self, logs=None):
         pass
     def on_train_step_end(self, logs=None):
         pass
 
 
-class BaseLogger(Callback):
-    """计算metrics的均值, 默认是callbacks中第一项, 主要是为History服务
-    
-    :param stateful_metrics: List[str], 仅保留状态信息的指标
-    """
-    def __init__(self, stateful_metrics=None, **kwargs):
-        super(BaseLogger, self).__init__(**kwargs)
-        self.stateful_metrics = _process_stateful_metrics(stateful_metrics)
-
-    def on_epoch_begin(self, global_step, epoch, logs=None):
-        self.seen = 0
-        self.totals = {}
-
-    def on_batch_end(self, global_step, local_step, logs=None):
-        logs = logs or {}
-        batch_size = logs.get('size', 0)
-        self.seen += batch_size
-
-        for k, v in logs.items():
-            if k in self.stateful_metrics:
-                self.totals[k] = v
-            else:
-                if k in self.totals:
-                    self.totals[k] += v * batch_size
-                else:
-                    self.totals[k] = v * batch_size
-
-    def on_epoch_end(self, global_step, epoch, logs=None):
-        '''在epoch_end对指标计算epoch的均值
-        '''
-        if logs is not None:
-            for k in self.params['metrics']:
-                if k in self.totals:
-                    # Make value available to next callbacks.
-                    if k in self.stateful_metrics:
-                        logs[k] = self.totals[k]
-                    else:
-                        logs[k] = self.totals[k] / self.seen
-
-
 class TerminateOnNaN(Callback):
     """Loss出现NAN停止训练"""
     def on_batch_end(self, global_step, local_step, logs=None):
         logs = logs or {}
         loss = logs.get('loss')
         if loss is not None:
             if np.isnan(loss) or np.isinf(loss):
@@ -422,24 +382,17 @@
 
     def on_batch_end(self, global_step=None, local_step=None, logs=None):
         logs = logs or {}
         self.seen += 1
         log_values = [(k, logs[k]) for k in self.params['metrics'] if k in logs]
         # Skip progbar update for the last batch;
         # will be handled by on_epoch_end.
-        if self.verbose and self.seen < self.target:
-            self.progbar.update(self.seen, log_values)
-            logs.update(self.progbar._smooth_values)  # 如果进度条是平滑的，那这里的logs也覆盖掉
-
-    def on_epoch_end(self, global_step=None, epoch=None, logs=None):
-        logs = logs or {}
-        log_values = [(k, logs[k]) for k in self.params['metrics'] if k in logs]
         if self.verbose:
             self.progbar.update(self.seen, log_values)
-            logs.update(self.progbar._smooth_values)
+            logs.update(self.progbar._smooth_values)  # 如果进度条是平滑的，那这里的logs也覆盖掉
     
     def on_train_end(self, logs=None):
         if self.verbose:
             time_start = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             print('%s - Finish Training' % (time_start))
         
 
@@ -463,38 +416,30 @@
     def on_batch_end(self, global_step=None, local_step=None, logs=None):
         self.seen += 1
         logs_new = self.smooth_values(self.seen, logs or {})
         log_values = [(k, logs_new[k]) for k in self.params['metrics'] if k in logs_new]
 
         # Skip progbar update for the last batch;
         # will be handled by on_epoch_end.
-        if self.verbose and self.seen < self.target:
-            self.progbar.n = self.seen
-            self.progbar.refresh()
-            self.progbar.set_postfix(log_values)
-            logs.update(self._smooth_values)
-
-    def on_epoch_end(self, global_step=None, epoch=None, logs=None):
-        logs_new = self.smooth_values(self.seen, logs or {})
-        log_values = [(k, logs_new[k]) for k in self.params['metrics'] if k in logs_new]
         if self.verbose:
             self.progbar.n = self.seen
             self.progbar.refresh()
             self.progbar.set_postfix(log_values)
             logs.update(self._smooth_values)
-            self.progbar.close()
+            if self.seen >= self.target:
+                self.progbar.close()
     
     def smooth_values(self, current, values=None):
         '''从Progbar迁移过来'''
         values = values or []
         for k, v in values.items():
             if k not in self.stateful_metrics:
                 if k not in self._values:
                     self._values[k] = [v * (current - self._seen_so_far), current - self._seen_so_far]
-                elif (self.smooth_interval is not None) and (current % self.smooth_interval == 0):
+                elif (self.smooth_interval is not None) and (current % self.smooth_interval == 1):
                     # 如果定义了累积smooth_interval，则需要重新累计
                     self._values[k] = [v, 1]
                 else:
                     self._values[k][0] += v * (current - self._seen_so_far)
                     self._values[k][1] += (current - self._seen_so_far)
             else:
                 self._values[k] = [v, 1]
@@ -539,26 +484,20 @@
     def on_batch_end(self, global_step=None, local_step=None, logs=None):
         self.seen += 1
         logs_new = self.smooth_values(self.seen, logs or {})
         logs_new = {k:logs_new[k].strip() for k in self.params['metrics'] if k in logs_new}
 
         # Skip progbar update for the last batch;
         # will be handled by on_epoch_end.
-        if self.verbose and self.seen < self.target:
-            self.progbar.update(self.seen, **logs_new)
-            logs.update(self._smooth_values)
-
-    def on_epoch_end(self, global_step=None, epoch=None, logs=None):
-        logs_new = self.smooth_values(self.seen, logs or {})
-        logs_new = {k:logs_new[k].strip() for k in self.params['metrics'] if k in logs_new}
         if self.verbose:
             self.progbar.update(self.seen, **logs_new)
             logs.update(self._smooth_values)
-            self.progbar.finish()
-    
+            if self.seen >= self.target:
+                self.progbar.finish()
+
 
 class History(Callback):
     """指标历史，默认是fit的返回项, 这里仅记录epoch_end的指标"""
     def on_train_begin(self, logs=None):
         self.epoch = []
         self.history = {}
 
@@ -944,33 +883,30 @@
     赋值需要分栏目的用'/'进行分隔
     若每隔一定steps对验证集评估，则Tensorboard的interval设置成和Evaluater一致或者约数，保证Tensorboard能记录到
 
     :param log_dir: str, tensorboard文件的保存路径
     :param method: str, 控制是按照epoch还是step来计算，默认为'epoch', 可选{'step', 'epoch'}
     :param interval: int, 保存tensorboard的间隔
     :param prefix: str, tensorboard分栏的前缀，默认为'train'
-    :param on_epoch_end_scalar_epoch: bool, epoch结束后是横轴是按照epoch还是global_step来记录
     '''
-    def __init__(self, log_dir, method='epoch', interval=10, prefix='train', on_epoch_end_scalar_epoch=True, **kwargs):
+    def __init__(self, log_dir, method='epoch', interval=10, prefix='train', **kwargs):
         super(Tensorboard, self).__init__(**kwargs)
         assert method in {'step', 'epoch'}, 'Args `method` only support `step` or `epoch`'
         self.method = method
         self.interval = interval
         self.prefix = prefix+'/' if len(prefix.strip()) > 0 else ''  # 控制默认的前缀，用于区分栏目
-        self.on_epoch_end_scalar_epoch = on_epoch_end_scalar_epoch  # 控制on_epoch_end记录的是epoch还是global_step
 
         from tensorboardX import SummaryWriter
         os.makedirs(log_dir, exist_ok=True)
         self.writer = SummaryWriter(log_dir=str(log_dir))  # prepare summary writer
 
     def on_epoch_end(self, global_step, epoch, logs=None):
         if self.method == 'epoch':
             # 默认记录的是epoch
-            log_step = epoch+1 if self.on_epoch_end_scalar_epoch else global_step+1
-            self.process(log_step, logs)
+            self.process(epoch+1, logs)
 
     def on_batch_end(self, global_step, local_step, logs=None):
         # 默认记录的是global_step
         if (self.method == 'step') and ((global_step+1) % self.interval == 0):
             self.process(global_step+1, logs)
 
     def process(self, iteration, logs):
@@ -1055,30 +991,30 @@
         self.mail_host = mail_host
         self.mail_user = mail_user
         self.mail_pwd = mail_pwd
         self.sender = sender
 
     def on_epoch_end(self, global_step, epoch, logs=None):
         if self.method == 'epoch':
-            msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k!='size'}, indent=2, ensure_ascii=False)
+            msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k not in SKIP_METRICS}, indent=2, ensure_ascii=False)
             subject = f'[INFO] Epoch {epoch+1} performance'
             if self.subject != '':
                 subject = self.subject + ' | ' + subject
             self._email(subject, msg)
 
     def on_batch_end(self, global_step, local_step, logs=None):
         if (self.method == 'step') and ((global_step+1) % self.interval == 0):
-            msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k!='size'}, indent=2, ensure_ascii=False)
+            msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k not in SKIP_METRICS}, indent=2, ensure_ascii=False)
             subject = f'[INFO] Step {global_step} performance'
             if self.subject != '':
                 subject = self.subject + ' | ' + subject
             self._email(subject, msg)
 
     def on_train_end(self, logs=None):
-        msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k!='size'}, indent=2, ensure_ascii=False)
+        msg = json.dumps({k:f'{v:.5f}' for k,v in logs.items() if k not in SKIP_METRICS}, indent=2, ensure_ascii=False)
         subject = f'[INFO] Finish training'
         if self.subject != '':
             subject = self.subject + ' | ' + subject
         self._email(subject, msg)
 
     def _email(self, subject, msg):
         send_email(self.receivers, subject=subject, msg=msg, mail_host=self.mail_host,
```

### Comparing `torch4keras-0.1.0/torch4keras/model.py` & `torch4keras-0.1.0.post2/torch4keras/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torch import nn
 import torch
 from torch4keras.snippets import DottableDict, metric_mapping, get_parameter_device, log_info, log_warn, log_error, print_trainable_parameters, colorful
-from torch4keras.callbacks import KerasProgbar, TqdmProgbar, ProgressBar2Progbar, Callback, CallbackList, BaseLogger, History
+from torch4keras.callbacks import KerasProgbar, TqdmProgbar, ProgressBar2Progbar, Callback, CallbackList, History
 from collections import OrderedDict
 from inspect import isfunction
 import os
 import json
 import math
 
 
@@ -41,15 +41,15 @@
         :param optimizer: 优化器
         :param scheduler: scheduler
         :param clip_grad_norm: bool, 是否使用梯度裁剪, 默认为False
         :param mixed_precision: bool, 是否使用混合精度，默认为False
         :param metrics: str/List[str]/dict, 训练过程中需要打印的指标, loss相关指标默认会打印, 目前支持accuracy, 也支持自定义metric，形式为{key: func}
         :param grad_accumulation_steps: int, 梯度累积步数，默认为1
         :param bar: str, 使用进度条的种类，从kwargs中解析，默认为keras, 可选keras, tqdm, progressbar2
-        :param progbar_config: 进度条的配置，如果使用指标平滑会更新到后续其他callbacks中（比如Logger），实现进度条显示和日志会保持一致
+        :param progbar_config: 进度条的配置，默认是对整个epoch计算均值指标
             bar: str, 默认为keras
             stateful_metrics: List[str], 表示不使用指标平滑仅进行状态记录的metric，指标抖动会更加明显，默认为None表示使用指标平滑
             smooth_interval: int, 表示指标平滑时候的累计步数，默认为None表示对整个epoch进行平滑
             width: int, keras进度条下表示进度条的长度
 
         :return: None
         '''
@@ -230,15 +230,15 @@
             callbacks = []
         elif isinstance(callbacks, Callback):
             callbacks = [callbacks]
         for callback in callbacks:
             assert isinstance(callback, Callback), "Args `callbacks` only support Callback() inputs"
 
         history = History()
-        callbacks_ = [BaseLogger(**self.progbar_config)]
+        callbacks_ = []
 
         # 进度条
         progbarlogger = None
         if self.verbose:
             if self.progbar_config['bar'] == 'keras':
                 progbarlogger = KerasProgbar(**self.progbar_config)
             elif self.progbar_config['bar'] == 'tqdm':
```

### Comparing `torch4keras-0.1.0/torch4keras/snippets.py` & `torch4keras-0.1.0.post2/torch4keras/snippets.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
     #登录并发送邮件
     try:
         smtpObj = smtplib.SMTP() 
         smtpObj.connect(mail_host, 25)  # 连接到服务器
         smtpObj.login(mail_user, mail_pwd)  # 登录到服务器
         smtpObj.sendmail(sender, receivers, message.as_string())  # 发送
         smtpObj.quit()  # 退出
-        print('[INFO] Send email success')
+        log_info('Send email success')
     except smtplib.SMTPException as e:
         log_error('Send email error : '+str(e))
         return str(e)
 
 
 def email_when_error(receivers, **configs):
     """装饰器，异常则发邮件
@@ -353,15 +353,15 @@
         # if using DS Zero 3 and the weights are initialized empty
         if num_params == 0 and hasattr(param, "ds_numel"):
             num_params = param.ds_numel
 
         all_param += num_params
         if param.requires_grad:
             trainable_params += num_params
-    print(f"trainable params: {trainable_params} || all params: {all_param} || trainable%: {100 * trainable_params / all_param}")
+    log_info(f"trainable params: {trainable_params} || all params: {all_param} || trainable%: {100 * trainable_params / all_param}")
 
 
 def get_parameter_device(parameter):
     '''获取device, 从transformers包迁移过来'''
     try:
         return next(parameter.parameters()).device
     except StopIteration:
```

### Comparing `torch4keras-0.1.0/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.1.0.post2/torch4keras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.1.0
+Version: 0.1.0.post2
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -71,30 +71,32 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
-- **v0.1.0**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
+- **v0.1.0.post2**: 20230725 修复v0.1.0的bug，主要是进度条和log的标签平滑的问题
+- **v0.1.0**: 20230724 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **v0.0.9**：20230716 增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **v0.0.8**：20230625 增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **v0.0.7.post3**: 20230517 修复保存scheduler
 - **v0.0.7.post2**: 20230517 Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
-- **20230721**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
+- **20230725**: 修复v0.1.0的bug，主要是进度条和log的标签平滑的问题
+- **20230724**: 允许调整进度条的显示参数, 进度条和日志同步（如果进度条平滑了则日志也平滑）, 自动把tensor转到model.device上, 允许打印第一个batch来检查样本
 - **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
```

