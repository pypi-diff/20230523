# Comparing `tmp/mmenot-0.9.1-py3-none-any.whl.zip` & `tmp/mmenot-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 24230 bytes, number of entries: 16
--rw-r--r--  2.0 unx        0 b- defN 23-May-19 09:36 mmenot/__init__.py
--rw-r--r--  2.0 unx     2935 b- defN 23-May-17 06:09 mmenot/exporter.py
--rw-r--r--  2.0 unx     5489 b- defN 23-May-17 06:09 mmenot/labels.py
--rw-r--r--  2.0 unx     5930 b- defN 23-May-18 12:45 mmenot/loops.py
--rw-r--r--  2.0 unx     1456 b- defN 23-May-19 09:31 mmenot/patches.py
--rw-r--r--  2.0 unx     5458 b- defN 23-May-19 09:31 mmenot/pruner.py
--rw-r--r--  2.0 unx      633 b- defN 23-May-17 06:09 mmenot/runner.py
--rw-r--r--  2.0 unx     3034 b- defN 23-May-17 06:09 mmenot/tester.py
--rw-r--r--  2.0 unx     4989 b- defN 23-May-17 06:09 mmenot/trainer.py
--rw-r--r--  2.0 unx    11638 b- defN 23-May-18 12:45 mmenot/utils.py
--rw-rw-rw-  2.0 unx    11338 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    14257 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      139 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1208 b- defN 23-May-19 09:36 mmenot-0.9.1.dist-info/RECORD
-16 files, 68603 bytes uncompressed, 22278 bytes compressed:  67.5%
+Zip file size: 24434 bytes, number of entries: 16
+-rw-r--r--  2.0 unx        0 b- defN 23-May-23 15:58 mmenot/__init__.py
+-rw-r--r--  2.0 unx     2977 b- defN 23-May-23 12:05 mmenot/exporter.py
+-rw-r--r--  2.0 unx     5553 b- defN 23-May-23 12:05 mmenot/labels.py
+-rw-r--r--  2.0 unx     6060 b- defN 23-May-23 12:05 mmenot/loops.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-May-23 12:05 mmenot/patches.py
+-rw-r--r--  2.0 unx     5726 b- defN 23-May-23 12:05 mmenot/pruner.py
+-rw-r--r--  2.0 unx      633 b- defN 23-May-23 12:05 mmenot/runner.py
+-rw-r--r--  2.0 unx     3074 b- defN 23-May-23 12:05 mmenot/tester.py
+-rw-r--r--  2.0 unx     5030 b- defN 23-May-23 12:05 mmenot/trainer.py
+-rw-r--r--  2.0 unx    11727 b- defN 23-May-23 15:48 mmenot/utils.py
+-rw-rw-rw-  2.0 unx    11338 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14257 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      139 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1208 b- defN 23-May-23 15:58 mmenot-0.9.2.dist-info/RECORD
+16 files, 69277 bytes uncompressed, 22482 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: mmenot/trainer.py
 Comment: 
 
 Filename: mmenot/utils.py
 Comment: 
 
-Filename: mmenot-0.9.1.dist-info/LICENSE
+Filename: mmenot-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: mmenot-0.9.1.dist-info/METADATA
+Filename: mmenot-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: mmenot-0.9.1.dist-info/WHEEL
+Filename: mmenot-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: mmenot-0.9.1.dist-info/entry_points.txt
+Filename: mmenot-0.9.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mmenot-0.9.1.dist-info/top_level.txt
+Filename: mmenot-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mmenot-0.9.1.dist-info/RECORD
+Filename: mmenot-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mmenot/exporter.py

```diff
@@ -73,7 +73,11 @@
             save_path = osp.join(args.work_dir, save_file)
             start = partition_cfg['start']
             end = partition_cfg['end']
             dynamic_axes = partition_cfg.get('dynamic_axes', None)
 
             extract_model(origin_ir_file, start, end, dynamic_axes=dynamic_axes, save_file=save_path)
     logger.info(f'torch2onnx finished. Results saved to {args.work_dir}')
+
+
+if __name__ == '__main__':
+    export()
```

## mmenot/labels.py

```diff
@@ -110,14 +110,15 @@
     model = model.to(device=baseline_model_device)  # move model to original device
     return labels_to_prune
 
 
 def labels_optimal_hw_aware(
     pruning_info: ModelPruningInfo,
     parameter: float,
+    n_search_steps: int,
     model: nn.Module,
     input_shape: Tuple[int, int],
     logger: MMLogger,
     deploy_cfg: str,
     model_cfg: str,
     host: str,
     port: int,
@@ -151,11 +152,12 @@
     target_latency = baseline_latency * acceleration_ratio
     logger.info(f'Target latency: {target_latency}')
 
     label_selector = OptimalPruningLabelSelector(
         model=model,
         latency_calculation_function=latency_calculation_function,
         target_latency=target_latency,
+        n_search_steps=n_search_steps,
     )
 
     labels_to_prune = label_selector.select(pruning_info)
     return labels_to_prune
```

## mmenot/loops.py

```diff
@@ -52,26 +52,28 @@
         input_shape: Tuple[int, int],
         host: str,
         port: int,
         endpoint: str,
         deploy_cfg: str,
         model_cfg: str,
         max_prunable_labels: int = 4096,
+        n_search_steps: int = 200,
         entry_point: str = 'forward',
         one_batch_only: bool = False,
         max_epochs: int = 1,
         val_begin: int = 1,
         val_interval: int = 1,
         dynamic_intervals=None,
     ) -> None:
         del val_begin, val_interval, dynamic_intervals, max_epochs
         super().__init__(runner=runner, dataloader=dataloader, max_epochs=1)
         self.runner: Runner  # for static analyzer
 
         self._max_prunable_labels = max_prunable_labels
+        self._n_search_steps = n_search_steps
         self._pruning_parameter = pruning_parameter
         self._input_shape: Tuple[int, int] = input_shape
         self._entry_point = entry_point
         self._one_batch_only = one_batch_only
 
         if pruning_type not in self._LABEL_SELECTOR_REGISTRY:
             raise ValueError(
@@ -139,14 +141,15 @@
         if self._pruning_type != 'optimal-hw-aware':
             self.runner.logger.info(f'MMACs: {count_mmac(self.runner.model, self._input_shape)}')
 
         label_selector = self._LABEL_SELECTOR_REGISTRY[self._pruning_type]
         labels_to_prune = label_selector(
             pruning_info=pruning_info,
             parameter=self._pruning_parameter,
+            n_search_steps=self._n_search_steps,
             model=self.runner.model,
             logger=self.runner.logger,
             input_shape=self._input_shape,
             deploy_cfg=self._deploy_cfg,
             model_cfg=self._model_cfg,
             host=self._host,
             port=self._port,
```

## mmenot/pruner.py

```diff
@@ -45,14 +45,20 @@
     )
     parser.add_argument(
         '--max-prunable-labels',
         type=int,
         default=4096,
         help='maximum number of labels in group which can be pruned',
     )
+    parser.add_argument(
+        '--n-search-steps',
+        type=int,
+        default=200,
+        help='number of search steps for optimal-hw-aware pruning',
+    )
     parser.add_argument('--entry-point', type=str, default='forward', help='pruning entry-point')
     parser.add_argument('--one-batch-only', nargs='?', const=True, default=False, help='prune on one batch only')
     parser.add_argument('--enable-logging', nargs='?', const=True, default=False, help='enable logging')
     parser.add_argument('--disable-cudnn', nargs='?', const=True, default=False, help='disable cudnn')
     parser.add_argument('--host', nargs='?', type=str, default='', help='latency measurement server host')
     parser.add_argument('--port', nargs='?', type=int, default=0, help='latency measurement server port')
     parser.add_argument(
@@ -121,20 +127,25 @@
 
     if args.checkpoint:
         cfg['model'] = args.checkpoint  # replace model config by checkpoint path
 
     cfg['train_cfg']['pruning_type'] = args.pruning_type
     cfg['train_cfg']['pruning_parameter'] = args.pruning_parameter
     cfg['train_cfg']['max_prunable_labels'] = args.max_prunable_labels
+    cfg['train_cfg']['n_search_steps'] = args.n_search_steps
     cfg['train_cfg']['input_shape'] = tuple(args.input_shape)
     cfg['train_cfg']['entry_point'] = args.entry_point
     cfg['train_cfg']['one_batch_only'] = args.one_batch_only
     cfg['train_cfg']['host'] = args.host
     cfg['train_cfg']['port'] = args.port
     cfg['train_cfg']['endpoint'] = args.endpoint
     cfg['train_cfg']['deploy_cfg'] = args.deploy_cfg
     cfg['train_cfg']['model_cfg'] = args.config
     cfg['train_cfg']['type'] = 'EpochBasedPruningLoop'
     cfg['train_cfg'].pop('max_iters', None)  # remove max_iters for EpochBasedPruningLoop
 
     runner = PruningRunner.from_cfg(cfg)
     runner.train()
+
+
+if __name__ == '__main__':
+    prune()
```

## mmenot/tester.py

```diff
@@ -74,7 +74,11 @@
     else:
         # build customized runner from the registry
         # if 'runner_type' is set in the cfg
         runner = RUNNERS.build(cfg)  # type: ignore
 
     # start testing
     runner.test()
+
+
+if __name__ == '__main__':
+    test()
```

## mmenot/trainer.py

```diff
@@ -122,7 +122,11 @@
     else:
         # build customized runner from the registry
         # if 'runner_type' is set in the cfg
         runner = RUNNERS.build(cfg)  # type: ignore
 
     # start training
     runner.train()
+
+
+if __name__ == '__main__':
+    train()
```

## mmenot/utils.py

```diff
@@ -13,14 +13,15 @@
 import onnx
 import torch
 from enot_latency_server.client import measure_latency_remote
 from fvcore.nn.flop_count import FlopCountAnalysis
 from mmdeploy.apis import extract_model
 from mmdeploy.apis import get_predefined_partition_cfg
 from mmdeploy.apis import torch2onnx
+from mmdeploy.core import reset_mark_function_count
 from mmdeploy.utils import get_partition_config
 from mmdeploy.utils import load_config
 from mmengine.config import Config
 from mmengine.config import ConfigDict
 from mmengine.dist import master_only
 from mmengine.fileio import FileClient
 from mmengine.fileio import join_path
@@ -276,14 +277,16 @@
 
         _get_input_shape = mmdeploy.utils.get_input_shape
         mmdeploy.utils.get_input_shape = lambda _: input_shape
 
         _build_pytorch_model = mmdeploy.codebase.base.task.BaseTask.build_pytorch_model
         mmdeploy.codebase.base.task.BaseTask.build_pytorch_model = lambda *args, **kwargs: model_  # type: ignore
 
+        reset_mark_function_count()
+
         torch2onnx(
             img=np.random.rand(16, 16, 3),
             work_dir=tempdir,
             save_file='model.onnx',
             deploy_cfg=deploy_cfg,
             model_cfg=model_cfg,
         )
```

## Comparing `mmenot-0.9.1.dist-info/LICENSE` & `mmenot-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mmenot-0.9.1.dist-info/METADATA` & `mmenot-0.9.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmenot
-Version: 0.9.1
+Version: 0.9.2
 Summary: ENOT Framework integration package for OpenMMLab codebase
 Author-email: ENOT LLC <enot@enot.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

