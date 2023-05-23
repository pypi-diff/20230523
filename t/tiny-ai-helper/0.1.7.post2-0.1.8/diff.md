# Comparing `tmp/tiny_ai_helper-0.1.7.post2.tar.gz` & `tmp/tiny_ai_helper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_ai_helper-0.1.7.post2.tar", last modified: Mon May 22 15:10:22 2023, max compression
+gzip compressed data, was "tiny_ai_helper-0.1.8.tar", last modified: Tue May 23 17:26:19 2023, max compression
```

## Comparing `tiny_ai_helper-0.1.7.post2.tar` & `tiny_ai_helper-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-22 15:10:22.059851 tiny_ai_helper-0.1.7.post2/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.7.post2/LICENSE
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      790 2023-05-22 15:10:22.055851 tiny_ai_helper-0.1.7.post2/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.7.post2/README.md
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-05-22 15:10:22.059851 tiny_ai_helper-0.1.7.post2/setup.cfg
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1031 2023-05-22 15:08:47.000000 tiny_ai_helper-0.1.7.post2/setup.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-22 15:10:22.055851 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    14107 2023-05-01 18:50:11.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/Model.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    10452 2023-04-30 10:47:53.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/Trainer.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      369 2023-05-22 15:08:38.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/__init__.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/layers.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/mp.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    20035 2023-05-22 13:38:21.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper/utils.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-22 15:10:22.055851 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      790 2023-05-22 15:10:22.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-05-22 15:10:22.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-05-22 15:10:22.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-05-22 15:10:22.000000 tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/top_level.txt
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-23 17:26:19.861100 tiny_ai_helper-0.1.8/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.8/LICENSE
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-23 17:26:19.861100 tiny_ai_helper-0.1.8/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.8/README.md
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-05-23 17:26:19.861100 tiny_ai_helper-0.1.8/setup.cfg
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-05-23 16:45:08.000000 tiny_ai_helper-0.1.8/setup.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-23 17:26:19.857100 tiny_ai_helper-0.1.8/tiny_ai_helper/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    16082 2023-05-23 17:23:20.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/Model.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    10452 2023-04-30 10:47:53.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/Trainer.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      310 2023-05-23 16:45:14.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/__init__.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     6522 2023-05-23 10:24:05.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/layers.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/mp.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    21782 2023-05-23 14:05:17.000000 tiny_ai_helper-0.1.8/tiny_ai_helper/utils.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-05-23 17:26:19.861100 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-05-23 17:26:19.000000 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-05-23 17:26:19.000000 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-05-23 17:26:19.000000 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-05-23 17:26:19.000000 tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/top_level.txt
```

### Comparing `tiny_ai_helper-0.1.7.post2/LICENSE` & `tiny_ai_helper-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7.post2/PKG-INFO` & `tiny_ai_helper-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny_ai_helper
-Version: 0.1.7.post2
+Version: 0.1.8
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

### Comparing `tiny_ai_helper-0.1.7.post2/setup.py` & `tiny_ai_helper-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from setuptools import setup, find_packages
 from os.path import abspath, dirname, join
 
 setup(
 	name="tiny_ai_helper",
-	version="0.1.7-2",
+	version="0.1.8",
 	description="Tiny AI Helper for PyTorch",
 	long_description=open(join(abspath(dirname(__file__)), 'README.md'), encoding='utf-8').read(),
 	long_description_content_type='text/markdown',
 	author="Ildar Bikmamatov",
 	author_email="support@bayrell.org",
 	license="MIT License",
 	url = "https://github.com/bayrell/ai_helper",
```

### Comparing `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/Model.py` & `tiny_ai_helper-0.1.8/tiny_ai_helper/Model.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,136 +5,129 @@
 # Copyright (с) Ildar Bikmamatov 2022 - 2023 <support@bayrell.org>
 # License: MIT
 ##
 
 import torch, time, json, math, gc, os
 from torch.utils.data import DataLoader, TensorDataset
 from .utils import TransformDataset, list_files, \
-    get_default_device, batch_to, tensor_size, load_json, summary
+    get_default_device, batch_to, tensor_size, load_json, summary, fit
 
 
 class Model:
     
-    def __init__(self, module=None, name=None):
+    def __init__(self, module=None):
         self.device = None
         self.transform_x = None
         self.transform_y = None
         self.module = module
         self.optimizer = None
         self.scheduler = None
         self.loss = None
+        self.loss_reduction = 'mean'
+        self.loss_precision = 9
+        self.best_metrics = ["val_acc_value", "rel", "epoch"]
         self.acc_fn = None
-        self.name = name
-        self.model_path = None
+        self.name = module.__class__.__name__
+        self.prefix_name = ""
         self.epoch = 0
         self.history = {}
-    
-    
-    def set_transform_x(self, transform_x):
-        self.transform_x = transform_x
-        return self
-    
-    
-    def set_transform_y(self, transform_y):
-        self.transform_y = transform_y
-        return self
+        self.min_lr = 1e-5
+        self.max_best_models = 10
+        self.model_path = ""
+        self.repository_path = ""
+        self.set_repository_path("model")
     
     
     def set_module(self, module):
         self.module = module
         return self
     
-    
     def set_optimizer(self, optimizer):
         self.optimizer = optimizer
         return self
     
-    
     def set_loss(self, loss):
         self.loss = loss
         return self
     
-    
     def set_scheduler(self, scheduler):
         self.scheduler = scheduler
         return self
     
-    
     def set_acc(self, acc):
         self.acc_fn = acc
         return self
     
-    
     def set_name(self, name):
         self.name = name
+        self.set_repository_path(self.repository_path)
         return self
     
+    def set_prefix_name(self, prefix_name):
+        self.prefix_name = prefix_name
+        self.set_repository_path(self.repository_path)
+        return self
     
     def set_path(self, model_path):
         self.model_path = model_path
         return self
     
+    def set_repository_path(self, repository_path):
+        self.repository_path = repository_path
+        self.model_path = os.path.join(repository_path, self.get_full_name())
+        return self
+    
+    def get_full_name(self):
+        if self.prefix_name != "":
+            return self.name + "_" + self.prefix_name
+        return self.name
     
-    def init(self, acc=None, optimizer=None, loss=None, scheduler=None,
-        lr=1e-3, transform_x=None, transform_y=None):
+    
+    def init(self):
         
         """
         Init model
         """
         
-        if acc is not None:
-            self.acc_fn = acc
-        
-        if transform_x is not None:
-            self.transform_x = transform_x
-        
-        if transform_y is not None:
-            self.transform_y = transform_y
-        
-        if loss is not None:
-            self.loss = loss
-        
-        if optimizer is not None:
-            self.optimizer = optimizer
-        
-        if scheduler is not None:
-            self.scheduler = scheduler
-        
         if self.loss is None:
             self.loss = torch.nn.MSELoss()
         
         if self.optimizer is None:
             try:
-                self.optimizer = torch.optim.Adam(self.module.parameters(), lr=lr)
+                self.optimizer = torch.optim.Adam(self.module.parameters(), lr=1e-3)
             except:
                 pass
         
         if self.scheduler is None and self.optimizer is not None:
             self.scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau( self.optimizer )
         
+        return self
+    
     
     def to(self, device):
         self.module = self.module.to(device)
         self.device = device
+        return self
     
-    
-    def to_gpu(self):
-        self.to( get_default_device() )
+    def to_cuda(self):
+        self.to( torch.device('cuda') if torch.cuda.is_available() else torch.device('cpu') )
+        return self
     
     
     def to_cpu(self):
         self.to( torch.device("cpu") )
-    
+        return self
     
     def train(self):
         self.module.train()
-    
+        return self
     
     def eval(self):
         self.module.eval()
+        return self
     
     
     def load_file(self, file_path):
         
         """
         Load model from file
         """
@@ -227,15 +220,15 @@
         
         """
         Save train status
         """
         
         # Get metrics
         save_metrics = {}
-        save_metrics["name"] = self.name
+        save_metrics["name"] = self.get_full_name()
         save_metrics["epoch"] = self.epoch
         save_metrics["history"] = self.history.copy()
         save_metrics["module"] = self.module.state_dict()
         save_metrics["optimizer"] = self.optimizer.state_dict()
         save_metrics["scheduler"] = self.scheduler.state_dict()
         save_metrics["loss"] = self.loss.state_dict()
         
@@ -266,99 +259,145 @@
         }
         json_str = json.dumps(obj, indent=2)
         file = open(file_name, "w")
         file.write(json_str)
         file.close()
     
     
-    def predict(self, x, batch_size=64):
+    def do_training(self, max_epochs):
+        
+        """
+        Returns True if model is need to train
+        """
+        
+        if self.epoch >= max_epochs:
+            return False
+        
+        if self.optimizer.param_groups[0]["lr"] < self.min_lr:
+            return False
+        
+        return True
+    
+    
+    def fit(self, train_dataset, val_dataset,
+        batch_size=32, epochs=10
+    ):
+        fit(self, train_dataset, val_dataset,
+            batch_size=batch_size, epochs=epochs)
+    
+    
+    def predict(self, x):
         
         """
         Predict
         """
-         
-        if self.transform_x is not None:
-            x = self.transform_x(x)
         
-        if self.device:
-            x = x.to( self.device )
+        batch_transform = getattr(self.module, "batch_transform", None)
         
-        y = self.module(x)
+        with torch.no_grad():
+            
+            x = x.to(self.device)
+            if batch_transform:
+                x, _ = batch_transform(x)
+            
+            self.module.eval()
+            y = self.module(x)
         
         return y
     
     
-    def predict_dataset(self, dataset, predict, batch_size=64, predict_obj=None):
+    def predict_dataset(self, dataset, predict, batch_size=64, obj=None):
         
         """
         Predict dataset
         """
         
         loader = DataLoader(
             dataset,
             batch_size=batch_size,
             drop_last=False,
             shuffle=False
         )
         
-        self.module.eval()
+        batch_transform = getattr(self.module, "batch_transform", None)
         
-        pos = 0
-        next_pos = 0
-        dataset_count = len(dataset)
-        time_start = time.time()
+        with torch.no_grad():
         
-        for batch_x, batch_y in loader:
-            
-            if self.transform_x:
-                batch_x = self.transform_x(batch_x)
+            self.module.eval()
             
-            if self.device:
-                batch_x = batch_to(batch_x, self.device)
+            pos = 0
+            next_pos = 0
+            dataset_count = len(dataset)
+            time_start = time.time()
             
-            batch_predict = self.module(batch_x)
-            predict(batch_x, batch_y, batch_predict, predict_obj)
-            
-            # Show progress
-            pos = pos + len(batch_x)
-            if pos > next_pos:
-                next_pos = pos + 16
-                t = str(round(time.time() - time_start))
-                print ("\r" + str(math.floor(pos / dataset_count * 100)) + "% " + t + "s", end='')
-            
-            del batch_x, batch_y, batch_predict
-            
-            # Clear cache
-            if torch.cuda.is_available():
-                torch.cuda.empty_cache()
+            for batch_x, batch_y in loader:
+                
+                x_batch = x_batch.to(self.device)
+                y_batch = y_batch.to(self.device)
+                
+                if batch_transform:
+                    x_batch, y_batch = batch_transform(x_batch, y_batch)
+                
+                batch_predict = self.module(batch_x)
+                predict(batch_x, batch_y, batch_predict, obj)
+                
+                # Show progress
+                pos = pos + len(batch_x)
+                if pos > next_pos:
+                    next_pos = pos + 16
+                    t = str(round(time.time() - time_start))
+                    print ("\r" + str(math.floor(pos / dataset_count * 100)) + "% " + t + "s", end='')
+                
+                del batch_x, batch_y, batch_predict
+                
+                # Clear cache
+                if torch.cuda.is_available():
+                    torch.cuda.empty_cache()
+                
+                gc.collect()
             
-            gc.collect()
-        
-        print ("\nOk")
+            print ("\nOk")
     
     
-    def get_metrics(self, metric_name):
+    def get_metrics(self, metric_name, convert=False):
         
         """
         Returns metrics by name
         """
         
+        def convert_value(value, metric_name):
+            if (
+                metric_name == "train_acc" or
+                metric_name == "train_acc_value" or
+                metric_name == "val_acc" or
+                metric_name == "val_acc_value" or
+                metric_name == "epoch"
+            ):
+                return -value
+            return value
+        
         res = []
         epochs = list(self.history.keys())
         for index in epochs:
             
             epoch = self.history[index]
             res2 = [ index ]
             
             if isinstance(metric_name, list):
                 for name in metric_name:
-                    res2.append( epoch[name] if name in epoch else 0 )
+                    value = epoch[name] if name in epoch else 0
+                    if convert:
+                        value = convert_value(value, name)
+                    res2.append( value )
             
             else:
-                res2.append( epoch[metric_name] if metric_name in epoch else 0 )
+                value = epoch[metric_name] if metric_name in epoch else 0
+                if convert:
+                    value = convert_value(value, metric_name)
+                res2.append( value )
             
             res.append(res2)
             
         return res
     
     
     def get_the_best_epoch(self):
@@ -374,20 +413,16 @@
     
     def get_the_best_epochs_indexes(self, epoch_count=5):
         
         """
         Returns best epoch indexes
         """
         
-        metrics = self.get_metrics(["acc_val", "acc_rel"])
-        
-        def get_key(item):
-            return [100 - item[1], item[2]]
-
-        metrics.sort(key=get_key)
+        metrics = self.get_metrics(self.best_metrics, convert=True)
+        metrics.sort(key=lambda x: x[1:])
         
         res = []
         res_count = 0
         metrics_len = len(metrics)
         loss_val_last = 100
         for index in range(metrics_len):
             
@@ -402,15 +437,15 @@
                 break
         
         res = [ res[index][0] for index in range(len(res)) ]
         
         return res
     
     
-    def save_the_best_models(self, epoch_count=5):
+    def save_the_best_models(self):
         
         """
         Save the best models
         """
         
         def detect_type(file_name):
             
@@ -422,14 +457,16 @@
             result = re.match(r'^model-(?P<id>[0-9]+)\.data$', file_name)
             if result:
                 return "model", int(result.group("id"))
             
             return file_type, epoch_index
         
         
+        epoch_count = self.max_best_models
+        
         if self.epoch > 0 and epoch_count > 0 and os.path.isdir(self.model_path):
             
             epoch_indexes = self.get_the_best_epochs_indexes(epoch_count)
             epoch_indexes.append( self.epoch )
             
             files = list_files( self.model_path )
             
@@ -440,24 +477,23 @@
                     epoch_index > 0 and \
                     not (epoch_index in epoch_indexes):
                     
                     file_path = os.path.join( self.model_path, file_name )
                     os.unlink(file_path)
     
     
-    def summary(self, x):
+    def summary(self, x, y=None):
         
         """
         Show model summary
         """
         
-        summary(self.module, x,
+        summary(self.module, x, y,
             device=self.device,
-            model_name=self.name,
-            transform_x=self.transform_x,
+            model_name=self.get_full_name()
         )
     
     
     def draw_history_ax(self, ax, metrics=[], label=None, legend=True, convert=None):
         
         """
         Draw history to axes
@@ -473,59 +509,73 @@
         if label:
             ax.set_xlabel( label )
         
         if legend:
             ax.legend()
     
     
-    def draw_history(self, metrics=[]):
+    def draw_history(self):
         
         """
         Draw history
         """
         
         import matplotlib.pyplot as plt
         
         fig, ax = plt.subplots(1, 2, figsize=(10, 4))
         self.draw_history_ax(ax[0],
-            ["acc_train", "acc_val"],
+            ["train_acc_value", "val_acc_value"],
             label="Accuracy",
             convert=lambda x: x * 100
         )
         self.draw_history_ax(ax[1],
-            ["loss_train", "loss_val"],
+            ["train_loss", "val_loss"],
             label="Loss"
         )
         plt.show()
     
     
-    def show_history(self):
+    def print_history(self):
         
         h = list(self.history.keys())
         h.sort()
         
         for epoch in h:
-            
-            res = self.history[epoch]
-            
-            acc_train = res["acc_train"] if "acc_train" in res else 0
-            acc_val = res["acc_val"] if "acc_val" in res else 0
-            acc_rel = res["acc_rel"] if "acc_rel" in res else 0
-            loss_train = res["loss_train"] if "loss_train" in res else 0
-            loss_val = res["loss_val"] if "loss_val" in res else 0
-            res_lr = res["res_lr"] if "res_lr" in res else 0
-            time = res["time"] if "time" in res else 0
-            
-            acc_train = str(round(acc_train * 10000) / 100)
-            acc_val = str(round(acc_val * 10000) / 100)
-            acc_train = acc_train.ljust(5, "0")
-            acc_val = acc_val.ljust(5, "0")
-            acc_rel_str = str(round(acc_rel * 100) / 100).ljust(4, "0")
-            loss_train = '%.3e' % loss_train
-            loss_val = '%.3e' % loss_val
-            res_lr_str = str(res_lr)
-            
-            print (f"Epoch {epoch}, " +
-                f"acc: {acc_train}%, acc_val: {acc_val}%, rel: {acc_rel_str}, " +
-                f"loss: {loss_train}, loss_val: {loss_val}, lr: {res_lr_str}, " +
-                f"t: {time}s"
-            )
+            s = self.get_epoch_string(epoch)
+            print(s)
+    
+    
+    def get_epoch_string(self, epoch):
+        
+        res = self.history[epoch]
+        
+        # Get epoch status
+        t = res["time"] if "time" in res else 0
+        train_acc = res["train_acc"] if "train_acc" in res else 0
+        train_loss = res["train_loss"] if "train_loss" in res else 0
+        train_count = res["train_count"] if "train_count" in res else 0
+        val_acc = res["val_acc"] if "val_acc" in res else 0
+        val_loss = res["val_loss"] if "val_loss" in res else 0
+        val_count = res["val_count"] if "val_count" in res else 0
+        res_lr = res["res_lr"] if "res_lr" in res else []
+        res_lr_str = str(res_lr)
+        
+        # Get result
+        f = "{:."+str(self.loss_precision)+"f}"
+        train_loss = f.format(train_loss)
+        val_loss = f.format(val_loss)
+        train_acc = round(train_acc / train_count * 10000) / 100
+        val_acc = round(val_acc / val_count * 10000) / 100
+        
+        msg = []
+        msg.append(f'\rEpoch: {epoch}')
+        
+        if self.acc_fn is not None:
+            acc_rel = "{:.4f}".format(train_acc / val_acc) if val_acc > 0 else 0
+            msg.append(f'train_acc: {train_acc}%, val_acc: {val_acc}%, rel: {acc_rel}')
+        
+        msg.append(f'train_loss: {train_loss}, val_loss: {val_loss}')
+        msg.append(f'lr: {res_lr_str}, t: {t}s')
+        
+        return ", ".join(msg)
+        
+
```

### Comparing `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/Trainer.py` & `tiny_ai_helper-0.1.8/tiny_ai_helper/Trainer.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/layers.py` & `tiny_ai_helper-0.1.8/tiny_ai_helper/layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,88 +9,102 @@
 import torch
 import numpy as np
 from typing import overload
 from PIL import Image, ImageDraw
 from .utils import resize_image
 
 
+class Lambda(torch.nn.Module):
+    
+    """
+    Lambda layer
+    """
+    
+    def __init__(self, f):
+        torch.nn.Module.__init__(self)
+        self.f=f
+    
+    def forward(self, x):
+        return self.f(x)
+
+
 class InsertFirstAxis(torch.nn.Module):
     
     """
     Insert first Axis for convolution layer
     """
     
-    def __call__(self, t):
+    def forward(self, t):
         t = t[:,None,:]
         return t
 
 
 class InsertLastAxis(torch.nn.Module):
     
     """
     Insert last Axis for convolution layer
     """
     
-    def __call__(self, t):
+    def forward(self, t):
         t = t[:,None]
         return t
 
 
 class MoveRGBToEnd(torch.nn.Module):
         
-    def __call__(self, t):
+    def forward(self, t):
         l = len(t.shape)
         t = torch.moveaxis(t, l-3, l-1)
         return t
 
 
 class MoveRGBToBegin(torch.nn.Module):
         
-    def __call__(self, t):
+    def forward(self, t):
         l = len(t.shape)
         t = torch.moveaxis(t, l-1, l-3)
         return t
 
 
 class ToIntImage(torch.nn.Module):
     
-    def __call__(self, t):
+    def forward(self, t):
         
         t = t * 255
         t = t.to(torch.uint8)
         
         return t
 
 
 class ToFloatImage(torch.nn.Module):
     
-    def __call__(self, t):
+    def forward(self, t):
         
         t = t.to(torch.float)
         t = t / 255.0
         
         return t
 
 
 class ToFloat(torch.nn.Module):
     
-    def __call__(self, t):
+    def forward(self, t):
         
         t = t.to(torch.float)
         
         return t
 
 
 class ReadImage(torch.nn.Module):
     
     def __init__(self, mode=None):
-        
+        torch.nn.Module.__init__(self)
         self.mode=mode
     
-    def __call__(self, batch):
+    def forward(self, batch):
         
         res = []
         for t in batch:
         
             t = Image.open(t)
             
             if self.mode is not None and self.mode != t.mode:
@@ -99,15 +113,15 @@
             res.append(t)
         
         return res
 
 
 class ImageToTensor(torch.nn.Module):
     
-    def __call__(self, batch):
+    def forward(self, batch):
         
         res = torch.tensor([])
         for t in batch:
             
             t = torch.from_numpy( np.array(t) )
             t = t[None, :]
             res = torch.cat( (res, t) )
@@ -121,15 +135,15 @@
         
         torch.nn.Module.__init__(self)
         
         self.size = size
         self.contain = contain
         self.color = color
     
-    def __call__(self, batch):
+    def forward(self, batch):
         
         res = []
         for t in batch:
             t = resize_image(t, self.size, contain=self.contain, color=self.color)
             res.append(t)
         
         return res
@@ -144,15 +158,15 @@
         torch.nn.Module.__init__(self)
         
         self.mean = mean
         self.std = std
         self.inplace = inplace
         self.normalize = torchvision.transforms.Normalize(mean=mean, std=std, inplace=inplace)
     
-    def __call__(self, t):
+    def forward(self, t):
         
         t = self.normalize(t)
         
         return t
     
     def extra_repr(self) -> str:
         return 'mean={}, std={}, inplace={}'.format(
@@ -195,15 +209,17 @@
     def state_dict(self, *args, destination=None, prefix='', keep_vars=False):
         pass
     
     
 class Stacking(torch.nn.Module):
     
     def __init__(self, *args, is_tensor_list=True):
+        
         torch.nn.Module.__init__(self)
+        
         for i, module in enumerate(args):
             self.add_module(str(i), module)
         
         self.is_tensor_list = is_tensor_list
     
     def forward(self, tensor_list):
         
@@ -236,17 +252,18 @@
                     prefix=prefix + m + '.',
                     keep_vars=keep_vars
                 )
 
 
 class Pipe():
     def __init__(self, *args):
+        torch.nn.Module.__init__(self)
         self.pipe = args
     
-    def __call__(self, value):
+    def forward(self, value):
         for fn in self.pipe:
             value = fn(value)
         return value
 
 
 class ModuleRemoveLastClassifier(PreparedModule):
```

### Comparing `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/mp.py` & `tiny_ai_helper-0.1.8/tiny_ai_helper/mp.py`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.7.post2/tiny_ai_helper/utils.py` & `tiny_ai_helper-0.1.8/tiny_ai_helper/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 ##
 # Tiny ai helper
 # Copyright (с) Ildar Bikmamatov 2022 - 2023 <support@bayrell.org>
 # License: MIT
 ##
 
-import torch, math, json, os, re
+import torch, math, json, os, re, time
 import numpy as np
 from torch import nn
+from torch.utils.data import Dataset, DataLoader
 from PIL import Image, ImageDraw
 
 
 class TransformDataset(torch.utils.data.Dataset):
     
     def __init__(self, dataset, transform_x=None, transform_y=None):
         self.dataset = dataset
@@ -619,68 +620,78 @@
         print( format_row(["", "Layer", "Output", "Params"], info_sizes) )
         print( "-" * width )
         
         for _, value in enumerate(values):
             print( format_row(value, info_sizes) )
         
         print( "-" * width )
-        if model_name is not None:
+        if model_name is not None and model_name != module.__class__.__name__:
             print( f"Model name: {model_name}" )
-        print( f"Total params: {res['params_count']}" )
-        print( f"Trainable params: {res['params_train_count']}" )
-        print( f"Total size: {res['total_size']} MiB" )
+        print( f"Total params: {res['params_count']:_}".replace('_', ' ') )
+        print( f"Trainable params: {res['params_train_count']:_}".replace('_', ' ') )
+        #print( f"Total size: {res['total_size']} MiB" )
         print( "=" * width )
 
 
-def fit(model, train_dataset, val_dataset,
-    batch_size=64, epochs=10, device=None,
-    min_lr=1e-5, reduction='mean'
-):
+def compile(module):
+    from .Model import Model
+    return Model(module)
+
+
+def fit(model, train_dataset, val_dataset, batch_size=64, epochs=10):
+    
+    device = model.device
     
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
     
-    module = model.module
-    optimizer = model.optimizer
-    scheduler = model.scheduler
-    loss_fn = model.loss
-    
-    batch_transform = getattr(module, "batch_transform", None)
-    
     train_loader = DataLoader(
         train_dataset,
         batch_size=batch_size,
         drop_last=False,
         shuffle=True
     )
     val_loader = DataLoader(
         val_dataset,
         batch_size=batch_size,
         drop_last=False,
         shuffle=False
     )
     
-    module = module.to(device)
+    acc_fn = model.acc_fn
+    device = model.device
+    loss_fn = model.loss
+    min_lr = model.min_lr
+    module = model.module
+    optimizer = model.optimizer
+    scheduler = model.scheduler
+    
+    batch_transform = getattr(module, "batch_transform", None)
     
-    print ("Start train")
+    print ("Start train on " + device)
     try:
-        for epoch in range(epochs):
+        while model.do_training(epochs):
             
             time_start = time.time()
             train_count = 0
             train_loss = 0
             train_iter = 0
+            train_acc = 0
             val_count = 0
             val_loss = 0
             val_iter = 0
+            val_acc = 0
             total_count = len(train_dataset) + len(val_dataset)
             pos = 0
             
+            model.epoch = model.epoch + 1
+            epoch = model.epoch
+            
             # train mode
-            module.train()
+            model.train()
             
             for x_batch, y_batch in train_loader:
                 
                 # data to device
                 x_batch = x_batch.to(device)
                 y_batch = y_batch.to(device)
                 if batch_transform:
@@ -699,27 +710,38 @@
                 batch_len = len(x_batch[0]) \
                     if isinstance(x_batch, tuple) or isinstance(x_batch, list) \
                     else len(x_batch)
                 train_loss += loss
                 train_count += batch_len
                 train_iter += 1
                 pos += batch_len
+                
+                train_acc_val = 0
 
+                # Calc accuracy
+                if acc_fn is not None:
+                    train_acc += acc_fn(y_pred, y_batch)
+                    train_acc_val = round(train_acc / train_count * 10000) / 100
+                
                 del x_batch, y_batch, y_pred, loss
 
                 if torch.cuda.is_available():
                     torch.cuda.empty_cache()
                 
-                print(f"\r{round(pos / total_count * 100)}%", end="")
-
+                iter_value = round(pos / total_count * 100)
+                if train_acc_val > 0:
+                    print(f"\rEpoch: {epoch}, {iter_value}%, acc: " + str(train_acc_val), end="")
+                else:
+                    print(f"\rEpoch: {epoch}, {iter_value}%", end="")
+            
             
             with torch.no_grad():
 
                 # testing mode
-                module.eval()
+                model.eval()
                 
                 for x_batch, y_batch in val_loader:
                     
                     # data to device
                     x_batch = x_batch.to(device)
                     y_batch = y_batch.to(device)
                     if batch_transform:
@@ -734,58 +756,75 @@
                         if isinstance(x_batch, tuple) or isinstance(x_batch, list) \
                         else len(x_batch)
                     val_loss += loss
                     val_count += batch_len
                     val_iter += 1
                     pos += batch_len
                     
+                    val_acc_val = 0
+                    
+                    # Calc accuracy
+                    if acc_fn is not None:
+                        val_acc += acc_fn(y_pred, y_batch)
+                        val_acc_val = round(val_acc / val_count * 10000) / 100
+                    
                     del x_batch, y_batch, y_pred, loss
 
                     if torch.cuda.is_available():
                         torch.cuda.empty_cache()
                     
-                    print(f"\r{round(pos / total_count * 100)}%", end="")
+                    iter_value = round(pos / total_count * 100)
+                    if val_acc_val > 0:
+                        print(f"\rEpoch: {epoch}, {iter_value}%, acc: " + str(val_acc_val), end="")
+                    else:
+                        print(f"\rEpoch: {epoch}, {iter_value}%", end="")
+            
             
-            if reduction == "mean":
+            if model.loss_reduction == "mean":
                 train_loss = (train_loss / train_iter).item()
                 val_loss = (val_loss / val_iter).item()
             
-            elif reduction == "sum":
+            elif model.loss_reduction == "sum":
                 train_loss = (train_loss / train_count).item()
                 val_loss = (val_loss / val_count).item()
             
-            scheduler.step(val_loss)
+            if scheduler is not None:
+               scheduler.step(val_loss)
             
             # Current lr
             res_lr = []
             for param_group in optimizer.param_groups:
                 res_lr.append( round(param_group['lr'], 7) )
-            res_lr_str = str(res_lr)
             
             time_end = time.time()
             t = round(time_end - time_start)
             
+            train_acc_value = (train_acc / train_count) if train_count > 0 else 0
+            val_acc_value = (val_acc / val_count) if train_count > 0 else 0
+            
             h = {
-                "loss_train": train_loss,
-                "loss_val": val_loss,
-                "count_train": train_count,
-                "count_val": val_count,
+                "epoch": epoch,
+                "rel": (train_acc_value / val_acc_value) if val_acc_value > 0 else 0,
                 "res_lr": res_lr,
                 "time": t,
+                "train_acc": train_acc,
+                "train_acc_value": train_acc_value,
+                "train_count": train_count,
+                "train_loss": train_loss,
+                "val_acc": val_acc,
+                "val_acc_value": val_acc_value,
+                "val_count": val_count,
+                "val_loss": val_loss,
             }
             
             model.history[epoch] = h
+            print( model.get_epoch_string(epoch) )
             
-            # Print result
-            train_loss = "{:.9f}".format(train_loss)
-            val_loss = "{:.9f}".format(val_loss)
-            
-            print(f'\repoch: {epoch + 1}, ' +
-                'train_loss: {train_loss}, val_loss: {val_loss}, ' +
-                'lr: {res_lr_str}, t: {t}s')
+            model.save_epoch()
+            model.save_the_best_models()
             
             if res_lr[0] < min_lr:
                 break
 
         print ("Ok")
 
     except KeyboardInterrupt:
```

### Comparing `tiny_ai_helper-0.1.7.post2/tiny_ai_helper.egg-info/PKG-INFO` & `tiny_ai_helper-0.1.8/tiny_ai_helper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-ai-helper
-Version: 0.1.7.post2
+Version: 0.1.8
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

