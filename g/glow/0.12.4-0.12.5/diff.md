# Comparing `tmp/glow-0.12.4.tar.gz` & `tmp/glow-0.12.5.tar.gz`

## Comparing `glow-0.12.4.tar` & `glow-0.12.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.4/examples/__init__.py
--rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.4/examples/cifar10.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.4/examples/gan.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/__init__.py
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/cli.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/cli.pyi
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/distributed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/py.typed
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/api/__init__.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/api/config.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/api/exporting.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/__init__.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_coro.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_import_hook.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_more.py
--rw-r--r--   0        0        0    14592 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_parallel.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_parallel.pyi
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_patch_len.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_patch_print.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_patch_scipy.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_profile.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_profile.pyi
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_reduction.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_repr.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_sizeof.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_thread_quota.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/_uuid.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/debug.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/__init__.py
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/cache.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/cache.pyi
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/concurrency.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/concurrency.pyi
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/reusable.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/core/wrap/util.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/io/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/io/_sound.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/io/_svg.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/metrics/__init__.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/metrics/base.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/metrics/confusion.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/metrics/raw.py
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/__init__.py
--rw-r--r--   0        0        0     8168 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/_loader.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/_sampler.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/_trainer.py
--rw-r--r--   0        0        0    13042 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/amp.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/driver.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/functional.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/optimizers.py
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/plot.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/proto.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/util.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/__init__.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/aggregates.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/context.py
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/convnets.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/lazy.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/simple.py
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/transformers.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/util.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/nn/modules/vision.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/__init__.py
--rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/classes.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/core.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/functional/__init__.py
--rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/functional/core.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.4/src/glow/transforms/functional/numba.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.4/test/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.4/test/run_metrics.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_api.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_batch.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_buffered.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_cli.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_iter.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_loader.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_shm.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_thread_pool.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_timed.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_timer.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.4/test/test_uuid.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.4/LICENSE
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.4/README.md
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 glow-0.12.4/pyproject.toml
--rw-r--r--   0        0        0     5137 2020-02-02 00:00:00.000000 glow-0.12.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.5/examples/__init__.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 glow-0.12.5/examples/cifar10.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 glow-0.12.5/examples/gan.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/__init__.py
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/cli.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/cli.pyi
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/distributed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/py.typed
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/api/__init__.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/api/config.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/api/exporting.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/__init__.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_coro.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_import_hook.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_more.py
+-rw-r--r--   0        0        0    15170 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_parallel.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_parallel.pyi
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_patch_len.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_patch_print.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_patch_scipy.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_profile.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_profile.pyi
+-rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_reduction.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_repr.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_sizeof.py
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_thread_quota.py
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/_uuid.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/debug.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/__init__.py
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/cache.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/cache.pyi
+-rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/concurrency.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/concurrency.pyi
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/reusable.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/core/wrap/util.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/io/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/io/_sound.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/io/_svg.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/metrics/__init__.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/metrics/base.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/metrics/confusion.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/metrics/raw.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/__init__.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/_loader.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/_sampler.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/_trainer.py
+-rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/amp.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/driver.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/functional.py
+-rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/optimizers.py
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/plot.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/proto.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/util.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/__init__.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/aggregates.py
+-rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/context.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/convnets.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/lazy.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/simple.py
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/transformers.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/util.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/nn/modules/vision.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/__init__.py
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/classes.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/core.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/functional/__init__.py
+-rw-r--r--   0        0        0     3891 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/functional/core.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 glow-0.12.5/src/glow/transforms/functional/numba.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.12.5/test/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 glow-0.12.5/test/run_metrics.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_api.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_batch.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_buffered.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_cli.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_iter.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_loader.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_shm.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_thread_pool.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_timed.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_timer.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.12.5/test/test_uuid.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.12.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 glow-0.12.5/LICENSE
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 glow-0.12.5/README.md
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 glow-0.12.5/pyproject.toml
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 glow-0.12.5/PKG-INFO
```

### Comparing `glow-0.12.4/examples/cifar10.py` & `glow-0.12.5/examples/cifar10.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/cli.py` & `glow-0.12.5/src/glow/cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/cli.pyi` & `glow-0.12.5/src/glow/cli.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/distributed.py` & `glow-0.12.5/src/glow/distributed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/api/config.py` & `glow-0.12.5/src/glow/api/config.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/api/exporting.py` & `glow-0.12.5/src/glow/api/exporting.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/__init__.py` & `glow-0.12.5/src/glow/core/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_coro.py` & `glow-0.12.5/src/glow/core/_coro.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_import_hook.py` & `glow-0.12.5/src/glow/core/_import_hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     This will result in a proxy callback being registered which will defer
     loading of the specified module containing the callback function until
     required.
 
     Simplified version of wrapt.register_post_import_hook.
     """
     with _LOCK:
-        global _INITIALIZED
+        global _INITIALIZED  # noqa: PLW0603
         if not _INITIALIZED:
             _INITIALIZED = True
             sys.meta_path.insert(0, _ImportHookFinder())
 
         if (module := sys.modules.get(name)) is not None:
             hook(module)
         else:
```

### Comparing `glow-0.12.4/src/glow/core/_more.py` & `glow-0.12.5/src/glow/core/_more.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_parallel.py` & `glow-0.12.5/src/glow/core/_parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 import os
 import signal
 import sys
 import warnings
 import weakref
 from collections.abc import Callable, Iterable, Iterator, Sized
 from concurrent.futures import Executor, Future
+from concurrent.futures import TimeoutError as _TimeoutError
 from contextlib import ExitStack, contextmanager
 from cProfile import Profile
 from functools import partial
-from itertools import chain, filterfalse, islice, starmap
+from itertools import chain, islice, starmap
 from multiprocessing.managers import BaseManager
 from operator import methodcaller
 from pstats import Stats
 from queue import Empty, SimpleQueue
 from threading import Lock
 from time import perf_counter, sleep
 from typing import Protocol, TypeVar, cast
@@ -80,17 +81,19 @@
     import torch
     if torch.version.cuda and torch.version.cuda >= '11.7.0':
         # It's expected that torch will fix .nv_fatb readonly flag in its DLLs
         # See https://stackoverflow.com/a/69489193/9868257
         return
 
     if psutil is None:
-        warnings.warn('Max process count may be calculated incorrectly, '
-                      'leading to application crash or even BSOD. '
-                      'Install psutil to avoid that')
+        warnings.warn(
+            'Max process count may be calculated incorrectly, '
+            'leading to application crash or even BSOD. '
+            'Install psutil to avoid that',
+            stacklevel=3)
         return
 
     # Overcommit on Windows is forbidden, thus VMS planning is necessary
     vms: int = psutil.Process().memory_info().vms
     free_vms: int = psutil.virtual_memory().free + psutil.swap_memory().free
     yield free_vms // vms
 
@@ -98,39 +101,48 @@
 def max_cpu_count(upper_bound: int = sys.maxsize, mp: bool = False) -> int:
     return min(_get_cpu_count_limits(upper_bound, mp))
 
 
 _PATIENCE = 0.01
 
 
-def _ki_call(fn: Callable[..., _T], *exc: type[BaseException]) -> _T:
+def _retry_call(fn: Callable[..., _T], *exc: type[BaseException]) -> _T:
     # See issues
     # https://bugs.python.org/issue29971
     # https://github.com/dask/dask/pull/2144#issuecomment-290556996
     # https://github.com/dask/dask/pull/2144/files
     while True:
         try:
             return fn(timeout=_PATIENCE)
         except exc:
             sleep(0)  # Force switch to another thread to proceed
 
 
 if sys.platform == 'win32':
-    from concurrent.futures import TimeoutError as _TimeoutError
 
     def _result(f: Future[_T]) -> _T:
-        return _ki_call(f.result, _TimeoutError)
+        return _retry_call(f.result, _TimeoutError)
 else:
     _result = Future.result
 
 
-def _get_q_get(q: _Queue[_T]) -> Callable[[], _T]:
+def _result_or_cancel(f: Future[_T]) -> _T:
+    try:
+        try:
+            return _result(f)
+        finally:
+            f.cancel()
+    finally:
+        del f
+
+
+def _q_get_fn(q: _Queue[_T]) -> Callable[[], _T]:
     if sys.platform != 'win32':
         return q.get
-    return partial(_ki_call, q.get, Empty)
+    return partial(_retry_call, q.get, Empty)
 
 
 # ---------------------------- pool initialization ----------------------------
 
 
 def _mp_profile():
     """Multiprocessed profiler"""
@@ -221,15 +233,15 @@
         mgr = _get_manager(executor)
         if isinstance(mgr, BaseManager):
             s.enter_context(mgr)
 
         ev: _Event = mgr.Event()
         q: _Queue[_T | _Empty] = mgr.Queue(latency)
         self._task = executor.submit(_consume, iterable, q, ev)  # type: ignore
-        self._get = q_get = _get_q_get(q)
+        self._get = q_get = _q_get_fn(q)
 
         # If main killed, wakes up consume to check ev
         # Otherwise collects 2nd _empty from q.
         # Called 2nd
         s.callback(q_get)
 
         # If main killed, signals consume to stop.
@@ -281,15 +293,17 @@
             return self.size
 
     def update(self, start_time: float, fut: Future[Sized]):
         # Compute as soon as future became done, discard later if not needed
         duration = perf_counter() - start_time
 
         try:
-            r = fut.result()  # Do not disturb Future._condition for nothing
+            # Cannot time out, as future is always completed at this point.
+            # Though it's unknown whether it succeeded or not, so use EAFP
+            r = fut.result()
         except BaseException:  # noqa: BLE001
             return
 
         with self.lock:
             if len(r) != self.size:
                 return
             self.duration = ((0.8 * self.duration + 0.2 * duration)
@@ -324,40 +338,49 @@
     size = _AutoSize()
     while args := [*islice(args_zip, size.suggest())]:
         f = make_future(*args)
         f.add_done_callback(partial(size.update, perf_counter()))
         yield f
 
 
-def _get_unwrap_iter(s: ExitStack, todo: set[Future[_T]],
-                     get_f: Callable[[], Future[_T]],
-                     fs: Iterator[Future[_T]]) -> Iterator[_T]:
+def _get_unwrap_iter(s: ExitStack, qsize: int,
+                     get_done_f: Callable[[], Future[_T]],
+                     fs_scheduler: Iterator) -> Iterator[_T]:
     with s:
-        while todo:
-            f = get_f()
-            todo.remove(f)
+        if not qsize:  # No tasks to do
+            return
+
+        # Unwrap 1st / schedule `N-qsize` / unwrap `qsize-1`
+        for _ in chain([None], fs_scheduler, range(qsize - 1)):
 
-            yield _result(f)  # wait with timeout
-            todo.update(islice(fs, 1))
+            # Retrieve done task, exactly `N` calls
+            yield _result_or_cancel(get_done_f())
 
 
 def _unwrap(s: ExitStack, fs: Iterable[Future[_T]], qsize: int | None,
             order: bool) -> Iterator[_T]:
     q = SimpleQueue[Future[_T]]()
+
+    # If `order`, then `q` has "PENDING"/"RUNNING"/"DONE" tasks,
+    # otherwise it only has "DONE" tasks.
     q_put = q.put if order else methodcaller('add_done_callback', q.put)
 
-    # As q.put always gives falsy None, filterfalse to call it as a side effect
-    fs = filterfalse(q_put, fs)  # type: ignore[arg-type]
+    # On each `next()` schedules new task
+    fs_scheduler = map(q_put, fs)  # type: ignore[call-overload]
     try:
-        todo = set(islice(fs, qsize))  # Prefetch
+        # Fetch up to `qsize` tasks to pre-fill `q`
+        qsize = sum(1 for _ in islice(fs_scheduler, qsize))
+
     except BaseException:
-        s.close()  # Unwind here on an error
+        # Unwind stack here on an error
+        s.close()
         raise
+
     else:
-        return _get_unwrap_iter(s, todo, _get_q_get(q), fs)
+        return _get_unwrap_iter(s, qsize, _q_get_fn(q), fs_scheduler)
 
 
 def _batch_invoke(func: Callable[..., _T], *items: tuple) -> list[_T]:
     return [*starmap(func, items)]
 
 
 def starmap_n(func: Callable[..., _T],
@@ -411,15 +434,15 @@
         return starmap(func, iterable)  # Fallback to single thread
 
     if mp and chunksize is None and prefetch is None:
         raise ValueError('With multiprocessing either chunksize or prefetch '
                          'must be not None')
 
     if prefetch is not None:
-        prefetch += max_workers
+        prefetch = max(prefetch + max_workers, 1)
 
     it = iter(iterable)
     s = ExitStack()
     submit = s.enter_context(_get_executor(max_workers, mp)).submit
 
     if mp:
         func = move_to_shmem(func)
```

### Comparing `glow-0.12.4/src/glow/core/_parallel.pyi` & `glow-0.12.5/src/glow/core/_parallel.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_patch_len.py` & `glow-0.12.5/src/glow/core/_patch_len.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_patch_print.py` & `glow-0.12.5/src/glow/core/_patch_print.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_patch_scipy.py` & `glow-0.12.5/src/glow/core/_patch_scipy.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,17 @@
     if (sys.platform != 'win32'
             or _FORTRAN_FLAG in os.environ  # Patch is already applied
             or not [*_get_conda_libs()]):  # Only Anaconda's SciPy is affected
         return
 
     os.environ[_FORTRAN_FLAG] = '1'  # Child will inherit this, and work fine
 
-    warnings.warn('Ctrl-C on Windows is broken when scipy is from conda. '
-                  'Please use scipy from PyPI')
+    msg = ('Ctrl-C on Windows is broken when scipy is from conda. '
+           'Please use scipy from PyPI')
+    warnings.warn(msg, stacklevel=2)
+
     if 'scipy.stats' in sys.modules:
-        warnings.warn('Cannot fix handling of Ctrl-C in current process. '
-                      'Import glow before scipy.stats to fix this.')
+        msg2 = ('Cannot fix handling of Ctrl-C in current process. '
+                'Import glow before scipy.stats to fix this.')
+        warnings.warn(msg2, stacklevel=2)
     else:
         _patch_handler_and_load_scipy()
```

### Comparing `glow-0.12.4/src/glow/core/_profile.py` & `glow-0.12.5/src/glow/core/_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 _THIS = None
 
 
 @contextmanager
 def memprof(name_or_callback: str | Callable[[float], object] | None = None,
             /) -> Iterator[None]:
-    global _THIS
+    global _THIS  # noqa: PLW0603
     if _THIS is None:
         import psutil
         _THIS = psutil.Process()
 
     init = _THIS.memory_info().rss
     try:
         yield
```

### Comparing `glow-0.12.4/src/glow/core/_profile.pyi` & `glow-0.12.5/src/glow/core/_profile.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_reduction.py` & `glow-0.12.5/src/glow/core/_reduction.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_repr.py` & `glow-0.12.5/src/glow/core/_repr.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_sizeof.py` & `glow-0.12.5/src/glow/core/_sizeof.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/_thread_quota.py` & `glow-0.12.5/src/glow/core/_thread_quota.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 from collections import deque
 from collections.abc import Callable
 from concurrent.futures import Executor, Future
 from concurrent.futures._base import LOGGER
 from concurrent.futures.thread import _WorkItem
 from queue import Empty, SimpleQueue
-from threading import Lock, Thread, _register_atexit
+from threading import _register_atexit  # type: ignore[attr-defined]
+from threading import Lock, Thread
 from typing import TypeVar
 from weakref import WeakKeyDictionary, WeakSet
 
 # TODO: investigate hangups when _TIMEOUT <= .01
 _TIMEOUT = 1
 _MIN_IDLE = 10
 
@@ -42,15 +43,15 @@
 _shutdown_lock = Lock()
 _executors = WeakSet['ThreadQuota']()
 _workers = WeakKeyDictionary[Thread, _Pipe]()
 _idle = deque[_Pipe]()
 
 
 def _python_exit():
-    global _shutdown
+    global _shutdown  # noqa: PLW0603
     with _shutdown_lock:
         _shutdown = True
 
     for e in _executors:
         e.shutdown(cancel_futures=True)
     *items, = _workers.items()
     for _, q in items:
@@ -96,15 +97,15 @@
             _executors.add(self)
 
     def submit(self, fn, /, *args, **kwargs):
         with self._shutdown_lock, _shutdown_lock:
             if self._shutdown or _shutdown:
                 raise RuntimeError('cannot schedule futures after shutdown')
 
-            f = Future()
+            f = Future()  # type: ignore[var-annotated]
             self._work_queue.append(_WorkItem(f, fn, args, kwargs))
 
             if _safe_call(self._idle.pop):  # Pool is not maximized yet
                 if not (q := _safe_call(_idle.pop)):
                     q = _Pipe()
                     w = Thread(target=_worker, args=(q, ))
                     w.start()
```

### Comparing `glow-0.12.4/src/glow/core/_uuid.py` & `glow-0.12.5/src/glow/core/_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/debug.py` & `glow-0.12.5/src/glow/core/debug.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/wrap/cache.py` & `glow-0.12.5/src/glow/core/wrap/cache.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/wrap/cache.pyi` & `glow-0.12.5/src/glow/core/wrap/cache.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/wrap/concurrency.py` & `glow-0.12.5/src/glow/core/wrap/concurrency.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,34 +63,34 @@
             return r
 
 
 def call_once(fn: _ZeroArgsF) -> _ZeroArgsF:
     """Makes `fn()` callable a singleton.
     DO NOT USE with recursive functions"""
     def wrapper():
-        return f.result()
+        return uf.result()
 
-    fn._future = f = _UFuture(fn)  # type: ignore[attr-defined]
+    fn._future = uf = _UFuture(fn)  # type: ignore[attr-defined]
     return cast(_ZeroArgsF, update_wrapper(wrapper, fn))
 
 
 def shared_call(fn: _F) -> _F:
     """Merges concurrent calls to `fn` with the same `args` to single one.
     DO NOT USE with recursive functions"""
     fs = WeakValueDictionary[Hashable, _UFuture]()
     lock = Lock()
 
     def wrapper(*args, **kwargs):
         key = make_key(*args, **kwargs)
 
         with lock:  # Create only one task per args-kwargs set
-            if not (f := fs.get(key)):
-                fs[key] = f = _UFuture(partial(fn, *args, **kwargs))
+            if not (uf := fs.get(key)):
+                fs[key] = uf = _UFuture(partial(fn, *args, **kwargs))
 
-        return f.result()
+        return uf.result()
 
     return cast(_F, update_wrapper(wrapper, fn))
 
 
 # ----------------------------- batch collation ------------------------------
 
 
@@ -133,21 +133,21 @@
     try:
         *results, = func([x for _, x in batch])
         assert len(results) == len(batch)
     except BaseException as exc:  # noqa: BLE001
         for f, _ in batch:
             f.set_exception(exc)
     else:
-        # TODO: use zip(strict=True) for python3.10+
+        # TODO: use zip(strict=True) for python3.10+ when 3.9 is EOL
         for (f, _), r in zip(batch, results):
             f.set_result(r)
 
 
 def _start_fetch_compute(func, workers, batch_size, timeout):
-    q = SimpleQueue()
+    q = SimpleQueue()  # type: ignore[var-annotated]
     lock = Lock()
 
     def loop():
         while True:
             # Because of lock, _fetch_batch could be inlined into wrapper,
             # and dispatch to thread pool could be done from there,
             # thus allowing usage of scalable ThreadPool
@@ -201,26 +201,27 @@
             pool_timeout=pool_timeout)
 
     assert callable(func)
     assert workers >= 1
     q = _start_fetch_compute(func, workers, batch_size, timeout)
 
     def wrapper(items):
-        fs = {Future(): item for item in items}
+        fs = {Future(): item for item in items}  # type: ignore[var-annotated]
         try:
             for f_x in fs.items():
-                q.put(f_x)
-            if wait(fs, pool_timeout, return_when='FIRST_EXCEPTION').not_done:
-                raise TimeoutError
-
-        except BaseException:  # Cancel all not yet submitted futures
-            while fs:
-                fs.popitem()[0].cancel()
-            raise
+                q.put(f_x)  # Schedule task
+            dnd = wait(fs, pool_timeout, return_when='FIRST_EXCEPTION')
 
-        return [f.result() for f in fs]
+        finally:  # Cancel all not-yet-running tasks, we're beyond deadline
+            for f in fs:
+                f.cancel()
+
+        if dnd.not_done:  # Some tasks timed out
+            del dnd, fs  # ? Break reference cycle
+            raise TimeoutError
+        return [f.result() for f in fs]  # Cannot time out - all are done
 
     # TODO: if func is instance method - recreate wrapper per instance
     # TODO: find how to distinguish between
     # TODO:  not yet bound method and plain function
     # TODO:  maybe implement __get__ on wrapper
     return update_wrapper(wrapper, func)
```

### Comparing `glow-0.12.4/src/glow/core/wrap/concurrency.pyi` & `glow-0.12.5/src/glow/core/wrap/concurrency.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/wrap/reusable.py` & `glow-0.12.5/src/glow/core/wrap/reusable.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/core/wrap/util.py` & `glow-0.12.5/src/glow/core/wrap/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/io/_sound.py` & `glow-0.12.5/src/glow/io/_sound.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/io/_svg.py` & `glow-0.12.5/src/glow/io/_svg.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/metrics/__init__.py` & `glow-0.12.5/src/glow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/metrics/base.py` & `glow-0.12.5/src/glow/metrics/base.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/metrics/confusion.py` & `glow-0.12.5/src/glow/metrics/confusion.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/metrics/raw.py` & `glow-0.12.5/src/glow/metrics/raw.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/__init__.py` & `glow-0.12.5/src/glow/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/_loader.py` & `glow-0.12.5/src/glow/nn/_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,16 @@
     if max_workers is None:
         max_workers = max_cpu_count(_NUM_CPUS, mp)
 
     if isinstance(dataset, IterableDataset):
         if not mp and max_workers != 0:
             warnings.warn(
                 'For iterable-style datasets multithreading is not supported. '
-                'Setting max_workers to 0')
+                'Setting max_workers to 0',
+                stacklevel=2)
             max_workers = 0
 
         if (ddp := get_ddp_info()) and ddp.world > 1:
             raise ValueError(
                 'For iterable-style datasets distributed use is not '
                 'supported')
```

### Comparing `glow-0.12.4/src/glow/nn/_sampler.py` & `glow-0.12.5/src/glow/nn/_sampler.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/_trainer.py` & `glow-0.12.5/src/glow/nn/_trainer.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/amp.py` & `glow-0.12.5/src/glow/nn/amp.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,15 +366,15 @@
       FP32 (unlike layernorm/groupnorm), thus it may cause stability issues.
       Unless you'll find a way to register batchnorm as op promoting to FP32
       in autocast mode.
       https://pytorch.org/docs/stable/amp.html#ops-that-can-autocast-to-float32
     """
     if _fp16_is_definitely_not_available():  # None can FP16, disable it anyway
         if dtype != torch.float:
-            warnings.warn('Neither of active devices support FP16, disable it')
+            warnings.warn('CUDA cannot FP16, fallback to FP32', stacklevel=2)
         dtype = torch.float
     elif dtype is None:  # Some GPU's can do FP16, automatic choice, enable
         dtype = torch.half
 
     if dtype != torch.half:
         return Grads(opt, sched)
     if not max_retries:
```

### Comparing `glow-0.12.4/src/glow/nn/driver.py` & `glow-0.12.5/src/glow/nn/driver.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/functional.py` & `glow-0.12.5/src/glow/nn/functional.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/optimizers.py` & `glow-0.12.5/src/glow/nn/optimizers.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/plot.py` & `glow-0.12.5/src/glow/nn/plot.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/proto.py` & `glow-0.12.5/src/glow/nn/proto.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/util.py` & `glow-0.12.5/src/glow/nn/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/modules/__init__.py` & `glow-0.12.5/src/glow/nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/modules/aggregates.py` & `glow-0.12.5/src/glow/nn/modules/aggregates.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         return checkpoint(closure, *xs)
 
     def forward(self, xs: list[torch.Tensor]) -> torch.Tensor:
         if torch.jit.is_scripting() or torch.jit.is_tracing():
             # checkpoint fails with JIT
             return self.cat(xs)
 
-        if len(self) and any([x.requires_grad for x in xs]):
+        if len(self) and any([x.requires_grad for x in xs]):  # noqa: C419
             return self._cp_proxy(xs)
 
         return self.cat(xs)
 
 
 def pre_norm(*fn: nn.Module, norm: LazyNormFn = LazyLayerNorm) -> Residual:
     """Returns input + fn(norm(input))"""
```

### Comparing `glow-0.12.4/src/glow/nn/modules/context.py` & `glow-0.12.5/src/glow/nn/modules/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
         >>> ctx.conv(64, 4, stride=2)  # fail
         ```
         """
         if kernel is None:
             kernel = self._get_k(stride, overlap)
 
         elif stride == 1 and kernel % 2 == 0:
-            warnings.warn(f'Parity is altered because of {kernel=}')
+            warnings.warn(
+                f'Parity is altered because of {kernel=}', stacklevel=2)
 
         elif stride != 1 and kernel != self.parity:
             raise ValueError(f'Used kernel does not match used parity '
                              f'({self.parity=}). Network is likely to break')
 
         padding = self._get_p(kernel, stride, dilation)
         groups = groups or dim
```

### Comparing `glow-0.12.4/src/glow/nn/modules/convnets.py` & `glow-0.12.5/src/glow/nn/modules/convnets.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/modules/lazy.py` & `glow-0.12.5/src/glow/nn/modules/lazy.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/modules/simple.py` & `glow-0.12.5/src/glow/nn/modules/simple.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/modules/transformers.py` & `glow-0.12.5/src/glow/nn/modules/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,17 @@
         if _IS_TORCH_1_12 and not self.training and not self.reattention:
             in_w, in_b, out_w, out_b = (self.to_qkv[0].weight,
                                         self.to_qkv[0].bias,
                                         self.to_out[1].weight,
                                         self.to_out[1].bias)
             tensor_args = (x, in_w, in_b, out_w, out_b)
             if ((_TORCH_MHA_AUTOCAST or not torch.is_autocast_enabled())
-                    and not (torch.is_grad_enabled()
-                             and any([t.requires_grad for t in tensor_args]))):
+                    and not (torch.is_grad_enabled() and any([  # noqa: C419
+                        t.requires_grad for t in tensor_args
+                    ]))):
                 if torch.is_autocast_enabled():
                     # torch uses slowpath, but this allows it go fast
                     dtype = torch.get_autocast_gpu_dtype()
                     if in_b.dtype != dtype:
                         in_b = in_b.to(dtype)
                 out, _ = torch._native_multi_head_attention(
                     x, x, x, self.dim, self.heads, in_w, in_b, out_w, out_b,
```

### Comparing `glow-0.12.4/src/glow/nn/modules/util.py` & `glow-0.12.5/src/glow/nn/modules/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/nn/modules/vision.py` & `glow-0.12.5/src/glow/nn/modules/vision.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/transforms/__init__.py` & `glow-0.12.5/src/glow/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/transforms/classes.py` & `glow-0.12.5/src/glow/transforms/classes.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/transforms/core.py` & `glow-0.12.5/src/glow/transforms/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/transforms/functional/core.py` & `glow-0.12.5/src/glow/transforms/functional/core.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/src/glow/transforms/functional/numba.py` & `glow-0.12.5/src/glow/transforms/functional/numba.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/run_metrics.py` & `glow-0.12.5/test/run_metrics.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_api.py` & `glow-0.12.5/test/test_api.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_batch.py` & `glow-0.12.5/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_buffered.py` & `glow-0.12.5/test/test_buffered.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_cli.py` & `glow-0.12.5/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_iter.py` & `glow-0.12.5/test/test_iter.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_loader.py` & `glow-0.12.5/test/test_loader.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_shm.py` & `glow-0.12.5/test/test_shm.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_thread_pool.py` & `glow-0.12.5/test/test_thread_pool.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_timed.py` & `glow-0.12.5/test/test_timed.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/test/test_uuid.py` & `glow-0.12.5/test/test_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/LICENSE` & `glow-0.12.5/LICENSE`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/README.md` & `glow-0.12.5/README.md`

 * *Files identical despite different names*

### Comparing `glow-0.12.4/pyproject.toml` & `glow-0.12.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 only-packages = true
 
 [project]
 name = "glow"
-version = "0.12.4"
+version = "0.12.5"
 description = "Functional Python tools with a PyTorch flavour"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = []
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
@@ -60,15 +60,15 @@
     "flake8-pie",
     "flake8-pyi",
     "flake8-pyproject",
     "flake8-simplify",
     "isort",
     "mypy~=1.1.1",
     "pytest~=6.0",
-    "ruff",
+    "ruff~=0.0.269",
     "yapf==0.33.0",
 ]
 dev = [
     "glow[dev-core]",
     "flake8-alphabetize",
     # "flake8-class-attributes-order",
     # "flake8-newspaper-style",
```

### Comparing `glow-0.12.4/PKG-INFO` & `glow-0.12.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glow
-Version: 0.12.4
+Version: 0.12.5
 Summary: Functional Python tools with a PyTorch flavour
 Project-URL: homepage, https://github.com/arquolo/glow
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Paul Maevskikh
@@ -57,15 +57,15 @@
 Requires-Dist: flake8-pyi; extra == 'dev-core'
 Requires-Dist: flake8-pyproject; extra == 'dev-core'
 Requires-Dist: flake8-simplify; extra == 'dev-core'
 Requires-Dist: flake8~=6.0.0; extra == 'dev-core'
 Requires-Dist: isort; extra == 'dev-core'
 Requires-Dist: mypy~=1.1.1; extra == 'dev-core'
 Requires-Dist: pytest~=6.0; extra == 'dev-core'
-Requires-Dist: ruff; extra == 'dev-core'
+Requires-Dist: ruff~=0.0.269; extra == 'dev-core'
 Requires-Dist: yapf==0.33.0; extra == 'dev-core'
 Provides-Extra: dev-wemake
 Requires-Dist: glow[dev-core]; extra == 'dev-wemake'
 Requires-Dist: wemake-python-styleguide~=0.15.0; extra == 'dev-wemake'
 Provides-Extra: io
 Requires-Dist: sounddevice; extra == 'io'
 Requires-Dist: soundfile; extra == 'io'
```

