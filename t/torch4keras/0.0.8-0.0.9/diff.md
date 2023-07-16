# Comparing `tmp/torch4keras-0.0.8.tar.gz` & `tmp/torch4keras-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4keras-0.0.8.tar", last modified: Sun Jun 25 15:00:44 2023, max compression
+gzip compressed data, was "torch4keras-0.0.9.tar", last modified: Sun Jul 16 10:02:37 2023, max compression
```

## Comparing `torch4keras-0.0.8.tar` & `torch4keras-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 15:00:44.504998 torch4keras-0.0.8/
--rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     7252 2023-06-25 15:00:44.502000 torch4keras-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6998 2023-06-25 14:58:24.000000 torch4keras-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-25 15:00:44.504998 torch4keras-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      522 2023-05-21 14:39:27.000000 torch4keras-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:00:44.492006 torch4keras-0.0.8/torch4keras/
--rw-rw-rw-   0        0        0        0 2023-05-30 14:28:06.000000 torch4keras-0.0.8/torch4keras/__init__.py
--rw-rw-rw-   0        0        0    51485 2023-06-10 11:46:06.000000 torch4keras-0.0.8/torch4keras/callbacks.py
--rw-rw-rw-   0        0        0    28907 2023-06-10 16:08:50.000000 torch4keras-0.0.8/torch4keras/model.py
--rw-rw-rw-   0        0        0    13928 2023-06-10 03:46:15.000000 torch4keras-0.0.8/torch4keras/snippets.py
-drwxrwxrwx   0        0        0        0 2023-06-25 15:00:44.500993 torch4keras-0.0.8/torch4keras.egg-info/
--rw-rw-rw-   0        0        0     7252 2023-06-25 15:00:44.000000 torch4keras-0.0.8/torch4keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-06-25 15:00:44.000000 torch4keras-0.0.8/torch4keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 15:00:44.000000 torch4keras-0.0.8/torch4keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-25 15:00:44.000000 torch4keras-0.0.8/torch4keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 10:02:37.006085 torch4keras-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     7489 2023-07-16 10:02:37.005087 torch4keras-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7235 2023-07-16 09:59:31.000000 torch4keras-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:02:37.006085 torch4keras-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      522 2023-07-16 10:01:39.000000 torch4keras-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:02:36.998088 torch4keras-0.0.9/torch4keras/
+-rw-rw-rw-   0        0        0        0 2023-05-30 14:28:06.000000 torch4keras-0.0.9/torch4keras/__init__.py
+-rw-rw-rw-   0        0        0    51485 2023-06-10 11:46:06.000000 torch4keras-0.0.9/torch4keras/callbacks.py
+-rw-rw-rw-   0        0        0    28990 2023-07-07 13:01:23.000000 torch4keras-0.0.9/torch4keras/model.py
+-rw-rw-rw-   0        0        0    17329 2023-07-12 15:43:50.000000 torch4keras-0.0.9/torch4keras/snippets.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:02:37.003083 torch4keras-0.0.9/torch4keras.egg-info/
+-rw-rw-rw-   0        0        0     7489 2023-07-16 10:02:36.000000 torch4keras-0.0.9/torch4keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-16 10:02:36.000000 torch4keras-0.0.9/torch4keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:02:36.000000 torch4keras-0.0.9/torch4keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-16 10:02:36.000000 torch4keras-0.0.9/torch4keras.egg-info/top_level.txt
```

### Comparing `torch4keras-0.0.8/LICENSE` & `torch4keras-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torch4keras-0.0.8/PKG-INFO` & `torch4keras-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.0.8
+Version: 0.0.9
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -71,27 +71,29 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.0.9**：20230716 增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
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
+- **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
```

### Comparing `torch4keras-0.0.8/README.md` & `torch4keras-0.0.9/torch4keras.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: torch4keras
+Version: 0.0.9
+Summary: Use torch like keras
+Home-page: https://github.com/Tongjilibo/torch4keras
+Author: Tongjilibo
+License: Apache License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # torch4keras
 **Use torch like keras**
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
@@ -61,27 +71,29 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.0.9**：20230716 增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
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
+- **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
```

### Comparing `torch4keras-0.0.8/setup.py` & `torch4keras-0.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='torch4keras',
-    version='v0.0.8',
+    version='v0.0.9',
     description='Use torch like keras',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License',
     url='https://github.com/Tongjilibo/torch4keras',
     author='Tongjilibo',
     install_requires=[],
```

### Comparing `torch4keras-0.0.8/torch4keras/callbacks.py` & `torch4keras-0.0.9/torch4keras/callbacks.py`

 * *Files identical despite different names*

### Comparing `torch4keras-0.0.8/torch4keras/model.py` & `torch4keras-0.0.9/torch4keras/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,25 +422,26 @@
         # 加载优化器，断点续训使用
         if scheduler_path:
             state_dict = torch.load(scheduler_path, map_location='cpu')
             self.scheduler.load_state_dict(state_dict)
         # 加载训练进度参数，断点续训使用
         self.load_steps_params(step_params_path)
 
-    def save_to_checkpoint(self, model_path=None, optimizer_path=None, scheduler_path=None, step_params_path=None, verbose=0):
+    def save_to_checkpoint(self, model_path=None, optimizer_path=None, scheduler_path=None, step_params_path=None, mapping={}, verbose=0):
         '''同时保存模型、优化器、训练过程参数、scheduler
 
         :param model_path: str, 模型文件路径
         :param optimizer_path: str, 优化器文件路径
         :param scheduler_path: str, scheduler文件路径
         :param step_params_path: str, 训练过程参数保存路径
+        :param mapping: dict, 模型文件的mapping
         '''
         verbose_str = ''
         if model_path:
-            self.save_weights(model_path)
+            self.save_weights(model_path, mapping=mapping)
             verbose_str += f'Model weights successfuly saved to {model_path}.\n'
         if optimizer_path:
             save_dir = os.path.dirname(optimizer_path)
             os.makedirs(save_dir, exist_ok=True)
             torch.save(self.optimizer.state_dict(), optimizer_path)
             verbose_str += f'Optimizer successfuly saved to {optimizer_path}.\n'
         if scheduler_path and (self.scheduler is not None):
```

### Comparing `torch4keras-0.0.8/torch4keras/snippets.py` & `torch4keras-0.0.9/torch4keras/snippets.py`

 * *Files 12% similar despite different names*

```diff
@@ -306,27 +306,49 @@
     s = str(obj)
     color_code = color_dict.get(color,"")
     display  = display_type_dict.get(display_type,"")
     out = '\033[{};{}m'.format(display,color_code)+s+'\033[0m'
     return out 
 
 
-def info_level_prefix(string, level=0):
+def log_level(string, level=0, verbose=1):
     '''在字符串前面加上有颜色的[INFO][WARNING][ERROR]字样'''
     if level in {0, 'i', 'info', 'INFO'}:
-        res = colorful('[INFO]', color='green') + string
+        res = log_info(string, verbose)
     elif level in {1, 'w', 'warn', 'warning', 'WARN', 'WARNING'}:
-        res = colorful('[WARNING]', color='yellow') + string
+        res = log_warn(string, verbose)
     elif level == {2, 'e', 'error', 'ERROR'}:
-        res = colorful('[ERROR]', color='red') + string
+        res = log_error(string, verbose)
     elif level == 1:
         res = string
     return res
+info_level_prefix = log_level
+
+
+def log_info(string, verbose=1):
+    res = colorful('[INFO]', color='green') + ' ' + string.strip()
+    if verbose != 0:
+        print(res)
+    return res
+
+
+def log_warn(string, verbose=1):
+    res = colorful('[WARNING]', color='yellow') + ' ' + string.strip()
+    if verbose != 0:
+        print(res)
+    return res
+
+
+def log_error(string, verbose=1):
+    res = colorful('[ERROR]', color='red') + ' ' + string.strip()
+    if verbose != 0:
+        print(res)
+    return res
+
 
-   
 def print_trainable_parameters(module):
     """打印可训练的参数量"""
     trainable_params = 0
     all_param = 0
     for _, param in module.named_parameters():
         num_params = param.numel()
         # if using DS Zero 3 and the weights are initialized empty
@@ -350,17 +372,79 @@
             tuples = [(k, v) for k, v in module.__dict__.items() if torch.is_tensor(v)]
             return tuples
 
         gen = parameter._named_members(get_members_fn=find_tensor_attributes)
         first_tuple = next(gen)
         return first_tuple[1].device
 
+
 class DottableDict(dict):
     '''支持点操作符的字典'''
     def __init__(self, *args, **kwargs):
         dict.__init__(self, *args, **kwargs)
         self.__dict__ = self
     def allowDotting(self, state=True):
         if state:
             self.__dict__ = self
         else:
             self.__dict__ = dict()
+
+
+def auto_set_cuda_devices(best_num: Optional[int] = None) -> str:
+    """
+    这段代码是一个名为 auto_set_cuda_devices 的函数，它接受一个可选的整数参数 best_num。该函数用于自动设置环境变量 CUDA_VISIBLE_DEVICES，以便在多个 GPU 设备中选择最佳的 GPU 设备。
+    首先，该函数检查环境变量 CUDA_VISIBLE_DEVICES 是否已经设置。如果已经设置，则发出警告并返回当前设置的值。
+    如果 best_num 等于 -1，则将环境变量 CUDA_VISIBLE_DEVICES 设置为 -1 并返回。
+    接下来，该函数尝试使用 nvidia-smi 命令查询 GPU 设备的信息。如果命令不存在，则发出警告并将环境变量 CUDA_VISIBLE_DEVICES 设置为 -1 并返回。
+    如果未指定 best_num，则从环境变量 LOCAL_WORLD_SIZE 中获取值。然后将其转换为整数。
+    接下来，该函数解析 nvidia-smi 命令的输出，并计算每个 GPU 设备的得分。得分由 GPU 利用率和可用内存计算得出。
+    最后，该函数选择得分最高的 best_num 个 GPU 设备，并将其索引作为字符串连接起来。然后将环境变量 CUDA_VISIBLE_DEVICES 设置为该字符串并返回。
+    """
+    import subprocess
+
+    # 无需重复设置
+    if "CUDA_VISIBLE_DEVICES" in os.environ:
+        print(info_level_prefix("Environment variable `CUDA_VISIBLE_DEVICES` has already been set", 'w'))
+        return os.environ["CUDA_VISIBLE_DEVICES"]
+
+    if best_num == -1:
+        print(info_level_prefix(f"SET CUDA_VISIBLE_DEVICES=-1"))
+        os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
+        return "-1"
+
+    try:
+        p = subprocess.Popen(
+            ["nvidia-smi",
+             "--query-gpu=index,utilization.gpu,memory.total,memory.free",
+             "--format=csv,noheader,nounits"],
+            stdout=subprocess.PIPE)
+    except FileNotFoundError:
+        print(info_level_prefix("`nvidia-smi` not exists"), 'e')
+        os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
+        return "-1"
+
+    if best_num is None:
+        best_num = os.environ.get("LOCAL_WORLD_SIZE", 1)
+    best_num = int(best_num)
+
+    stdout, _ = p.communicate()
+    outputs = stdout.decode("utf-8")
+    lines = outputs.split(os.linesep)
+
+    scores = []
+    for item in lines:
+        item_arr = item.split(",")
+        if len(item_arr) != 4:
+            continue
+        gpu_score = 100 - int(item_arr[1].strip())
+        memory_score = 100 * (int(item_arr[3].strip()) / int(item_arr[2].strip()))
+        score = gpu_score + memory_score
+        scores.append(score)
+
+    best_num = min(best_num, len(scores))
+    topk_idx = (-np.asarray(scores)).argsort()[:best_num]
+
+    topk_idx_str = ",".join(map(str, topk_idx))
+    print(info_level_prefix(f"SET CUDA_VISIBLE_DEVICES={topk_idx_str}"))
+    os.environ["CUDA_VISIBLE_DEVICES"] = topk_idx_str
+
+    return topk_idx_str
```

### Comparing `torch4keras-0.0.8/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: torch4keras
-Version: 0.0.8
-Summary: Use torch like keras
-Home-page: https://github.com/Tongjilibo/torch4keras
-Author: Tongjilibo
-License: Apache License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # torch4keras
 **Use torch like keras**
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
@@ -71,27 +61,29 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.0.9**：20230716 增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
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
+- **20230716**：增加auto_set_cuda_devices自动选择显卡，增加log_info，log_warn, log_error等小函数
 - **20230625**：增加EmailCallback和WandbCallback, 增加AccelerateTrainer和DeepSpeedTrainer, grad_accumulation_steps内算一个batch，修改Trainer中部分成员函数
 - **20230517**：Checkpoint Calback增加保存scheduler, save_weights可自行创建目录，Logger, Tensorboard模块加入lr, 修改predict和add_trainer
 - **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
 - **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
 - **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
```

