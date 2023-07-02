# Comparing `tmp/torchility-0.7.3.tar.gz` & `tmp/torchility-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.7.3.tar", last modified: Fri Jun  2 07:24:35 2023, max compression
+gzip compressed data, was "torchility-0.7.5.tar", last modified: Sun Jul  2 13:36:06 2023, max compression
```

## Comparing `torchility-0.7.3.tar` & `torchility-0.7.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.732027 torchility-0.7.3/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.3/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2215 2023-06-02 07:24:35.731440 torchility-0.7.3/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1736 2023-05-28 14:40:21.000000 torchility-0.7.3/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.707110 torchility-0.7.3/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1873 2023-05-28 13:25:54.000000 torchility-0.7.3/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.3/examples/10-model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.3/examples/11-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2625 2023-05-28 13:29:46.000000 torchility-0.7.3/examples/2-metrics_basic.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.3/examples/3-metrics_more.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.3/examples/4-callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.3/examples/5-lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.3/examples/6-optimizer.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.3/examples/7-interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.3/examples/8-multi_dataloaders.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.3/examples/9-reset_train_dataloader.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.708698 torchility-0.7.3/imgs/
--rw-r--r--   0 liuchen    (501) staff       (20)   119040 2023-05-28 14:38:16.000000 torchility-0.7.3/imgs/data_flow.png
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-06-02 07:24:35.732350 torchility-0.7.3/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.3/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.717083 torchility-0.7.3/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-06-02 07:24:15.000000 torchility-0.7.3/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.727469 torchility-0.7.3/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.3/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.3/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.3/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.3/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)     9796 2023-05-27 15:05:14.000000 torchility-0.7.3/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.3/torchility/datamodule.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.3/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.3/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6732 2023-06-02 07:24:04.000000 torchility-0.7.3/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5695 2023-05-23 02:30:35.000000 torchility-0.7.3/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 15:21:26.000000 torchility-0.7.3/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.730782 torchility-0.7.3/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       97 2023-05-28 01:59:22.000000 torchility-0.7.3/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2647 2023-05-21 03:41:57.000000 torchility-0.7.3/torchility/utils/metric_utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.3/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.3/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.7.3/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-06-02 07:24:35.723794 torchility-0.7.3/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2215 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      998 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-06-02 07:24:35.000000 torchility-0.7.3/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 13:36:06.593858 torchility-0.7.5/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.7.5/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-02 13:36:06.593270 torchility-0.7.5/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1716 2023-06-02 07:34:33.000000 torchility-0.7.5/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 13:36:06.573509 torchility-0.7.5/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1873 2023-05-28 13:25:54.000000 torchility-0.7.5/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.7.5/examples/10-model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.7.5/examples/11-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2608 2023-06-02 07:33:31.000000 torchility-0.7.5/examples/2-metrics_basic.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2064 2023-05-21 03:49:55.000000 torchility-0.7.5/examples/3-metrics_more.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1738 2023-05-19 08:52:25.000000 torchility-0.7.5/examples/4-callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.7.5/examples/5-lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1563 2023-05-16 01:20:14.000000 torchility-0.7.5/examples/6-optimizer.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.7.5/examples/7-interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2531 2023-05-19 12:30:31.000000 torchility-0.7.5/examples/8-multi_dataloaders.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1623 2023-05-16 00:41:34.000000 torchility-0.7.5/examples/9-reset_train_dataloader.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 13:36:06.574440 torchility-0.7.5/imgs/
+-rw-r--r--   0 liuchen    (501) staff       (20)   119040 2023-05-28 14:38:16.000000 torchility-0.7.5/imgs/data_flow.png
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-07-02 13:36:06.594047 torchility-0.7.5/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1163 2023-05-27 06:45:49.000000 torchility-0.7.5/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 13:36:06.580695 torchility-0.7.5/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-07-02 13:34:53.000000 torchility-0.7.5/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 13:36:06.586912 torchility-0.7.5/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.7.5/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1656 2023-05-23 02:30:14.000000 torchility-0.7.5/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.7.5/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.7.5/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     9796 2023-07-02 13:33:31.000000 torchility-0.7.5/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.7.5/torchility/datamodule.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.7.5/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.7.5/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6732 2023-06-02 07:24:04.000000 torchility-0.7.5/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5811 2023-06-27 04:58:49.000000 torchility-0.7.5/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    12469 2023-05-27 15:21:26.000000 torchility-0.7.5/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 13:36:06.592401 torchility-0.7.5/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)       97 2023-05-28 01:59:22.000000 torchility-0.7.5/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2645 2023-06-27 06:54:19.000000 torchility-0.7.5/torchility/utils/metric_utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.7.5/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6816 2023-05-18 13:11:06.000000 torchility-0.7.5/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.7.5/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-07-02 13:36:06.583768 torchility-0.7.5/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2195 2023-07-02 13:36:06.000000 torchility-0.7.5/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)      998 2023-07-02 13:36:06.000000 torchility-0.7.5/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-07-02 13:36:06.000000 torchility-0.7.5/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)      112 2023-07-02 13:36:06.000000 torchility-0.7.5/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-07-02 13:36:06.000000 torchility-0.7.5/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.7.3/LICENSE` & `torchility-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/PKG-INFO` & `torchility-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.3
+Version: 0.7.5
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -28,20 +28,14 @@
 - torchmetrics>=0.11,<0.12
 - matplotlib>=3.3
 - pyyaml>=5.4
 - tensorboardX>=2.6
 
 ## Usage
 
-### Data Flow
-
-<center>
-    <img src="imgs/data_flow.png" width="60%"/>
-</center>
-
 ### Example
 
 - MNIST
 
 ```python
 from torchility import Trainer
 import torch
@@ -86,7 +80,14 @@
 trainer.fit(train_dl, val_dl)
 # test
 trainer.test(test_dl)
 ```
 
 - See the `examples` for more examples 
 
+### Data Flow
+
+<img src="imgs/data_flow.png" width="60%"/>
+
+
+
+
```

### Comparing `torchility-0.7.3/README.md` & `torchility-0.7.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,14 @@
 - torchmetrics>=0.11,<0.12
 - matplotlib>=3.3
 - pyyaml>=5.4
 - tensorboardX>=2.6
 
 ## Usage
 
-### Data Flow
-
-<center>
-    <img src="imgs/data_flow.png" width="60%"/>
-</center>
-
 ### Example
 
 - MNIST
 
 ```python
 from torchility import Trainer
 import torch
@@ -67,8 +61,14 @@
 trainer = Trainer(model, F.cross_entropy, opt, epochs=2)
 # train and validate
 trainer.fit(train_dl, val_dl)
 # test
 trainer.test(test_dl)
 ```
 
-- See the `examples` for more examples 
+- See the `examples` for more examples 
+
+### Data Flow
+
+<img src="imgs/data_flow.png" width="60%"/>
+
+
```

### Comparing `torchility-0.7.3/examples/1-mnist.py` & `torchility-0.7.5/examples/1-mnist.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/examples/10-model_analysis.py` & `torchility-0.7.5/examples/10-model_analysis.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/examples/11-graph_node_clasification_DGL.py` & `torchility-0.7.5/examples/11-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/examples/2-metrics_basic.py` & `torchility-0.7.5/examples/2-metrics_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,12 @@
 def acc3(preds, targets):
     """同时计算多个指标"""
     preds = preds.argmax(1)
     return {'a':(preds == targets).float().mean(), 'b':(preds == targets).float().mean()}
 
 trainer = Trainer(model, F.cross_entropy, opt, epochs=10,
                   metrics=[acc, acc1, acc2, acc3],    # 指定计算指标，默认在train、val和test中都会计算
-                  val_frac=2                          # 每2个epoch做一次验证
+                  val_freq=2                          # 每2个epoch做一次验证
                   )
-progress = trainer.fit(train_dl, val_dl)              # 训练、验证
+trainer.fit(train_dl, val_dl)                         # 训练、验证
 
 trainer.test(test_dl)                                 # 测试
-
-print(progress)
```

### Comparing `torchility-0.7.3/examples/3-metrics_more.py` & `torchility-0.7.5/examples/3-metrics_more.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/examples/4-callbacks.py` & `torchility-0.7.5/examples/4-callbacks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/examples/5-lr_find.py` & `torchility-0.7.5/examples/5-lr_find.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/examples/6-optimizer.py` & `torchility-0.7.5/examples/6-optimizer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/examples/7-interpreter.py` & `torchility-0.7.5/examples/7-interpreter.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/examples/8-multi_dataloaders.py` & `torchility-0.7.5/examples/8-multi_dataloaders.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/examples/9-reset_train_dataloader.py` & `torchility-0.7.5/examples/9-reset_train_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/imgs/data_flow.png` & `torchility-0.7.5/imgs/data_flow.png`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/setup.py` & `torchility-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/callbacks/common.py` & `torchility-0.7.5/torchility/callbacks/common.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/callbacks/interpreters.py` & `torchility-0.7.5/torchility/callbacks/interpreters.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/callbacks/performances.py` & `torchility-0.7.5/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/callbacks/progress.py` & `torchility-0.7.5/torchility/callbacks/progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     def on_train_batch_end(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule", outputs, batch, batch_idx: int):
         self.train_batch_id = batch_idx + 1
         c_epoch, num_epoch, c_batch, num_batch = self.get_info(trainer, 'train')
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = 'TRAIN >'
         info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in outputs.items()])
-        print(f"{progress} {stage} {info}", end="\r", flush=True)
+        print(f"\r{progress} {stage} {info}", end="", flush=True)
         return super().on_train_batch_end(trainer, pl_module, outputs, batch, batch_idx)
 
     def on_train_epoch_end(self, trainer, pl_module):
         train_c_epoch, train_num_epoch, _, train_num_batch = self.get_info(trainer, 'train')
         _, _, _, val_num_batch = self.get_info(trainer, 'val')
 
         train_info_dict = self.get_epoch_loss(trainer, 'train')
@@ -115,24 +115,24 @@
 
     def on_validation_batch_end(self, trainer, pl_module, outputs, batch, batch_idx, dataloader_idx: int = 0):
         self.val_batch_id = batch_idx + 1
         c_epoch, num_epoch, c_batch, num_batch  = self.get_info(trainer, 'val')
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = '  VAL >'
         info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in outputs.items()])
-        print(f"{progress} {stage} {info}", end="\r", flush=True)
+        print(f"\r{progress} {stage} {info}", end="", flush=True)
         return super().on_validation_batch_end(trainer, pl_module, outputs, batch, batch_idx, dataloader_idx)
 
     def on_test_batch_end(self, trainer, pl_module, outputs, batch, batch_idx: int, dataloader_idx: int = 0):
         self.test_batch_id = batch_idx + 1
         c_epoch, num_epoch, c_batch, num_batch = self.get_info(trainer, 'test')
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = ' TEST >'
         info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in outputs.items()])
-        print(f"{progress} {stage} {info}", end="\r", flush=True)
+        print(f"\r{progress} {stage} {info}", end="", flush=True)
         return super().on_test_batch_end(trainer, pl_module, outputs, batch, batch_idx, dataloader_idx)
 
     def on_test_epoch_end(self, trainer, pl_module):
         c_epoch, num_epoch, c_batch, num_batch = self.get_info(trainer, 'test')
         info_dict = self.get_epoch_loss(trainer, 'test')
         info_dict.update(trainer.test_epoch_metric_values)
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
```

### Comparing `torchility-0.7.3/torchility/datamodule.py` & `torchility-0.7.5/torchility/datamodule.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/hooks.py` & `torchility-0.7.5/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/losses.py` & `torchility-0.7.5/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/metrics.py` & `torchility-0.7.5/torchility/metrics.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/tasks.py` & `torchility-0.7.5/torchility/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,19 @@
 
         return metric_values
 
     def test_step(self, batch, batch_nb, dataloader_idx=0):                   # 测试步
         do_loss = self.do_test_loss
         if isinstance(do_loss, (list, tuple)):
             do_loss = dataloader_idx in do_loss
-        loss, preds, targets, _ = self.do_forward(batch, do_loss)
+        loss, preds, targets, batch_size = self.do_forward(batch, do_loss)
 
         metric_values = {}
         if loss is not None:
+            self.log('test_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
             if self.multi_test_dataloaders:
                 metric_values[f'loss/{dataloader_idx}'] = loss
             else:
                 metric_values['loss'] = loss
 
         preds, targets = detach_clone(preds), detach_clone(targets)
         if self.metrics:
```

### Comparing `torchility-0.7.3/torchility/trainer.py` & `torchility-0.7.5/torchility/trainer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/utils/metric_utils.py` & `torchility-0.7.5/torchility/utils/metric_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 def set_metric_attr(metric, name=None, stages=None, dl_idx:int=None, simple_cumulate=None, log:bool=None, on_bar:bool=None):
     """
     Args:
         metric:   指标
         name:     指标名
         stages:   在哪些阶段运行，取值为 'train', 'val', 'test' 或者它们组成的列表，默认值 ['train', 'val', 'test']
         dl_idx:   验证或测试阶段使用多个dataloader时，指标运行在哪个dataloader之上，默认值 -1 表示所有的dataloader
-        simple_cumulate: MetricBase子类是否采用简单累积方式计算Epoch指标（利用batch_size累积指标值，效率高但不适用于基于混淆矩阵的指标），默认为False
+        simple_cumulate: MetricBase子类是否采用简单累积方式计算Epoch指标（利用batch_size累积指标值，效率高但不适用于基于混淆矩阵的指标），默认为True
         log:      是否将计算结果记入日志，默认值 True
         on_bar:   指标是否在pytorch_lightning内置的进度条上显示，默认值 True
     """
     # 默认属性取值
-    attr = {'name': None, 'stages': ['train', 'val', 'test'], 'dl_idx': -1, 'simple_cumulate': False, 'log': True, 'on_bar': True}
+    attr = {'name': None, 'stages': ['train', 'val', 'test'], 'dl_idx': -1, 'simple_cumulate': True, 'log': True, 'on_bar': True}
 
     if isinstance(metric, (tuple, list)):
         assert len(metric) == 2, "'`metric` should be a tuple of (metric_name, metric_callable) or (metric_callable, metric_name)"
         if callable(metric[0]):      # (metric_callable, dataloader_idx)
             metric, name_ = metric
         elif callable(metric[1]):    # (metric_name, metric_callable)
             name_, metric = metric
```

### Comparing `torchility-0.7.3/torchility/utils/plots.py` & `torchility-0.7.5/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/utils/utils.py` & `torchility-0.7.5/torchility/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility/utils/yaml_config.py` & `torchility-0.7.5/torchility/utils/yaml_config.py`

 * *Files identical despite different names*

### Comparing `torchility-0.7.3/torchility.egg-info/PKG-INFO` & `torchility-0.7.5/torchility.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.7.3
+Version: 0.7.5
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -28,20 +28,14 @@
 - torchmetrics>=0.11,<0.12
 - matplotlib>=3.3
 - pyyaml>=5.4
 - tensorboardX>=2.6
 
 ## Usage
 
-### Data Flow
-
-<center>
-    <img src="imgs/data_flow.png" width="60%"/>
-</center>
-
 ### Example
 
 - MNIST
 
 ```python
 from torchility import Trainer
 import torch
@@ -86,7 +80,14 @@
 trainer.fit(train_dl, val_dl)
 # test
 trainer.test(test_dl)
 ```
 
 - See the `examples` for more examples 
 
+### Data Flow
+
+<img src="imgs/data_flow.png" width="60%"/>
+
+
+
+
```

### Comparing `torchility-0.7.3/torchility.egg-info/SOURCES.txt` & `torchility-0.7.5/torchility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

