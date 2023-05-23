# Comparing `tmp/mmpretrain-1.0.0rc7.tar.gz` & `tmp/mmpretrain-1.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmpretrain-1.0.0rc7.tar", last modified: Fri Apr  7 10:25:18 2023, max compression
+gzip compressed data, was "dist/mmpretrain-1.0.0rc8.tar", last modified: Tue May 23 03:25:07 2023, max compression
```

## Comparing `mmpretrain-1.0.0rc7.tar` & `mmpretrain-1.0.0rc8.tar`

### file list

```diff
@@ -1,1270 +1,1415 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18892 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15478 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/cifar100_bs16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/cifar10_bs16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/cub_bs8_384.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/cub_bs8_448.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet21k_bs128.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_mbv3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_medium_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_small_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_revvit_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_medium_384.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_small_384.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_vig_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_196.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_336.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_560.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_pil_bicubic_384.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_beitv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_davit_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_levit_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a3.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_simmim_192.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_swin_192.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_byol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_mocov2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_pil_bicubic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_pil_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs512_mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs512_mocov3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_autoaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_384.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_448.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_convmixer_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_deit3_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_deit3_384.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_edgenext_256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_mixer_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_pil_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_pil_resize_autoaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_384.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_t2t_224.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs8_pil_bicubic_320.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/inshop_bs32_448.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/pipelines/auto_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/pipelines/rand_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/voc_bs16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/conformer/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/conformer/base-p16.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/conformer/small-p16.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/conformer/small-p32.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/conformer/tiny-p16.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convmixer/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convmixer/convmixer-1024-20.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convmixer/convmixer-1536-20.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convmixer/convmixer-768-32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-xlarge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/atto.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/femto.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/huge.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/large.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/nano.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/pico.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/tiny.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/davit/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/davit/davit-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/davit/davit-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/davit/davit-tiny.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-base-p16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-base-p16-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-huge-p14-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-large-p16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-large-p16-384.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-medium-p16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-small-p16-224.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-small-p16-384.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/densenet/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/densenet/densenet121.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/densenet/densenet161.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/densenet/densenet169.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/densenet/densenet201.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/edgenext/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-xsmall.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-xxsmall.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientformer-l1.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_b3.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_b4.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_b5.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_b6.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_b7.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_b8.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_em.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_es.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_l2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_b0.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_b1.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_b3.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_l.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_m.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_xl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/eva/
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/eva/eva-g.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/eva/eva-l.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-base-gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large-gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large-gf384.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-small-gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-tiny-gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-tiny.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hrnet/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w18.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w30.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w32.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w40.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w44.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w48.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w64.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/levit-256-p16.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mae_vit-base-p16.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mixmim/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mixmim/mixmim_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mlp_mixer_base_patch16.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mlp_mixer_large_patch16.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v2_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_large_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_050_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_075_imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_imagenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobileone/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s0.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s1.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s2.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilevit/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilevit/mobilevit_s.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilevit/mobilevit_xs.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilevit/mobilevit_xxs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mvit/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-large.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-tiny.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_m36.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_m48.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s12.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s24.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s36.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/regnet/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_1.6gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_12gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_3.2gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_4.0gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_400mf.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_6.4gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_8.0gf.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_800mf.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/replknet-31B_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/replknet-31L_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/replknet-XL_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/repmlp-base_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/repvgg-A0_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/repvgg-B3_lbs-mixup_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/res2net101-w26-s4.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/res2net50-w14-s8.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/res2net50-w26-s4.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/res2net50-w26-s6.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/res2net50-w26-s8.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/res2net50-w48-s2.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnest101.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnest200.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnest269.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnest50.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet101_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet152.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet152_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet18.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet18_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet34.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet34_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet34_gem.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet50_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet50_cifar_cutmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet50_cifar_mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet50_cutmix.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet50_label_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet50_mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnetv1c50.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnetv1d101.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnetv1d152.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnetv1d50.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnext152_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnext50_32x4d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/revvit/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/revvit/revvit-base.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/revvit/revvit-small.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/seresnet101.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/seresnet50.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/seresnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/seresnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/shufflenet_v1_1x.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/shufflenet_v2_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/base_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/base_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/large_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/large_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/small_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/tiny_224.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/base_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/base_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/large_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/large_384.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/small_256.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/tiny_256.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-14.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-19.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-24.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/tinyvit/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-11m.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-21m.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-5m.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/tnt_s_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/twins_pcpvt_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/twins_svt_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/van/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/van/van_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/van/van_large.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/van/van_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/van/van_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vgg11.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vgg11bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vgg13.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vgg13bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vgg16bn.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vgg19bn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/vig_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/vig_small.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/vig_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vit-base-p16.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vit-base-p32.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vit-large-p16.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vit-large-p32.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/wide-resnet50.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/cifar10_bs128.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/cub_bs64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_revvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_swin.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_coslr.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_linearlr_bn_nowd.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_AdamW.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_adamw_levit.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_coslr.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_rsb.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_140e.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_200e_coslr_warmup.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_coslr.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_coslr_coswd_300e.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_epochstep.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs4096_AdamW.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_lars_coslr_200e.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_lars_coslr_90e.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_sgd_coslr_100e.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_sgd_coslr_200e.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_sgd_steplr_100e.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/arcface/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/arcface/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/arcface/resnet50-arcface_8xb32_inshop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/barlowtwins/
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/barlowtwins/barlowtwins_resnet50_8xb256-coslr-1000e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/barlowtwins/barlowtwins_resnet50_8xb256-coslr-300e_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/barlowtwins/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/barlowtwins/benchmarks/resnet50_8xb32-linear-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/barlowtwins/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/beit_beit-base-p16_8xb256-amp-coslr-300e_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-1600e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-300e_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50-c4_ms-1x_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50_fpn_ms-1x_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/benchmarks/resnet50_8xb512-linear-coslr-90e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/byol_resnet50_16xb256-coslr-200e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cae/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cae/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cae/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cae/cae_beit-base-p16_8xb256-amp-coslr-300e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cae/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-448px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-448px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/conformer/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/conformer/conformer-base-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/conformer/conformer-small-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/conformer/conformer-small-p32_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/conformer/conformer-tiny-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/conformer/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convmixer/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convmixer/convmixer-1024-20_10xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convmixer/convmixer-1536-20_10xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convmixer/convmixer-768-32_10xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convmixer/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-small_32xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-small_32xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-tiny_32xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-tiny_32xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-atto_32xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-base_32xb32_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-base_32xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-femto_32xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k-512px.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-large_32xb32_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-large_32xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-nano_32xb32_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-nano_32xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-pico_32xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-tiny_32xb32_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-tiny_32xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cspnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cspnet/cspdarknet50_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cspnet/cspresnet50_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cspnet/cspresnext50_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cspnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/csra/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/csra/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/csra/resnet101-csra_1xb16_voc07-448px.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/davit/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/davit/davit-base_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/davit/davit-small_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/davit/davit-tiny_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/davit/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-base-distilled_16xb32_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-base-distilled_16xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-base_16xb32_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-base_16xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-small-distilled_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-small_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-tiny-distilled_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-tiny_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-base-p16_64xb32_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-base-p16_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-huge-p14_64xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-large-p16_64xb16_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-large-p16_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-medium-p16_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-small-p16_64xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-small-p16_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densecl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densecl/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densecl/benchmarks/resnet50_8xb32-linear-steplr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densecl/densecl_resnet50_8xb32-coslr-200e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densecl/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densenet/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densenet/densenet121_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densenet/densenet161_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densenet/densenet169_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densenet/densenet201_4xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densenet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-base_8xb256-usi_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-base_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-small_8xb256-usi_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-small_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-xsmall_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-xxsmall_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientformer/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientformer/efficientformer-l1_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientformer/efficientformer-l3_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientformer/efficientformer-l7_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientformer/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b0_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b0_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b1_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b1_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b2_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b2_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b3_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b3_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b4_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b4_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b5_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b5_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b6_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b6_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b7_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b7_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b8_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b8_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-em_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-es_8xb32-01norm_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-l2_8xb32_in1k-475px.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-l2_8xb8_in1k-800px.py
--rw-r--r--   0 runner    (1001) docker     (123)    25083 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b0_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b1_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b2_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b3_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-l_8xb32_in1k-480px.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-l_8xb32_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-m_8xb32_in1k-480px.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-m_8xb32_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-s_8xb32_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-s_8xb32_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-xl_8xb32_in1k-512px.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-xl_8xb32_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb2048-linear-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-g-p14_8xb16_in1k-336px.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-g-p14_8xb16_in1k-560px.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-g-p14_headless.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-g-p16_headless.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-l-p14_8xb16_in1k-196px.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-l-p14_8xb16_in1k-336px.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-l-p14_headless.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-mae-style_vit-base-p16_16xb256-coslr-400e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hornet/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hornet/hornet-base-gf_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hornet/hornet-base_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hornet/hornet-small-gf_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hornet/hornet-small_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hornet/hornet-tiny-gf_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hornet/hornet-tiny_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hornet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/hrnet-w18_4xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/hrnet-w30_4xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/hrnet-w32_4xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/hrnet-w40_4xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/hrnet-w44_4xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/hrnet-w48_4xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/hrnet-w64_4xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/inception_v3/inception-v3_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/inception_v3/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/lenet/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/lenet/lenet5_mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/deploy/levit-128_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/deploy/levit-128s_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/deploy/levit-192_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/deploy/levit-256_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/deploy/levit-384_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/levit-128_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/levit-128s_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/levit-192_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/levit-256_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/levit-384_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-base-p16_8xb2048-linear-coslr-90e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-huge-p14_32xb8-coslr-50e_in1k-448px.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-huge-p14_8xb128-coslr-50e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-large-p16_8xb128-coslr-50e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-large-p16_8xb2048-linear-coslr-90e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-1600e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-300e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-400e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-800e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-huge-p14_8xb512-amp-coslr-1600e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-1600e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-300e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-400e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-800e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/maskfeat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/maskfeat/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/maskfeat/benchmarks/vit-base-p16_8xb256-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/maskfeat/maskfeat_vit-base-p16_8xb256-amp-coslr-300e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/maskfeat/metafile.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/benchmarks/vit-base-p16_8xb2048-linear-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/milan_vit-base-p16_16xb256-amp-coslr-400e_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mixmim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mixmim/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mixmim/benchmarks/mixmim-base_8xb128-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mixmim/benchmarks/mixmim-base_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mixmim/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mixmim/mixmim_mixmim-base_16xb128-coslr-300e_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mlp_mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mlp_mixer/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mlp_mixer/mlp-mixer-base-p16_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mlp_mixer/mlp-mixer-large-p16_64xb64_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v2/mobilenet-v2_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-large_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small-050_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small-075_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small_8xb16_cifar10.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s0_deploy_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s1_deploy_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s2_deploy_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s3_deploy_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s4_deploy_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s0_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s1_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s2_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s3_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s4_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilevit/
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilevit/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilevit/mobilevit-small_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilevit/mobilevit-xsmall_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilevit/mobilevit-xxsmall_8xb128_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov2/benchmarks/resnet50_8xb32-linear-steplr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov2/mocov2_resnet50_8xb32-coslr-200e_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/resnet50_8xb128-linear-coslr-90e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/vit-base-p16_8xb128-linear-coslr-90e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/vit-base-p16_8xb64-coslr-150e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/vit-large-p16_8xb64-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/vit-small-p16_8xb128-linear-coslr-90e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-300e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-800e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_vit-base-p16_16xb256-amp-coslr-300e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_vit-large-p16_64xb64-amp-coslr-300e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_vit-small-p16_16xb256-amp-coslr-300e_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/mvitv2-base_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/mvitv2-large_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/mvitv2-small_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/mvitv2-tiny_8xb256_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-m36_32xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-m48_32xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-s12_32xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-s24_32xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-s36_32xb128_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-1.6gf_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-12gf_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-3.2gf_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-4.0gf_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-400mf_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-6.4gf_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-8.0gf_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-800mf_8xb128_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/deploy/replknet-31B-deploy_32xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/deploy/replknet-31B-deploy_32xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/deploy/replknet-31L-deploy_32xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/deploy/replknet-XL-deploy_32xb64_in1k-320px.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/replknet-31B_32xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/replknet-31B_32xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/replknet-31L_32xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/replknet-XL_32xb64_in1k-320px.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repmlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repmlp/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repmlp/repmlp-base_8xb64_in1k-256px.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repmlp/repmlp-base_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repmlp/repmlp-base_delopy_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repmlp/repmlp-base_deploy_8xb64_in1k-256px.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-A0_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-A0_deploy_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-A1_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-A2_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-B0_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-B1_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-B1g2_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-B1g4_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-B2_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-B2g4_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-B3_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-B3g4_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-D2se_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/res2net/
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/res2net/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/res2net/res2net101-w26-s4_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/res2net/res2net50-w14-s8_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/res2net/res2net50-w26-s8_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/_randaug_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/resnest101_32xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/resnest200_64xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/resnest269_64xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/resnest50_32xb64_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/
--rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet101_8xb16_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet101_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet152_8xb16_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet152_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet18_8xb16_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet18_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet34_8xb16_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet34_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_32xb64-warmup-coslr_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_32xb64-warmup-lbs_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_32xb64-warmup_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb128_coslr-90e_in21k.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb16-mixup_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb16_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb16_cifar100.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a1-600e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a2-300e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a3-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb32-coslr-preciseBN_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb32-coslr_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb32-cutmix_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb32-fp16-dynamic_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb32-fp16_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb32-lbs_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb32-mixup_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb8_cub.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnetv1c101_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnetv1c152_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnetv1c50_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnetv1d101_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnetv1d152_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnetv1d50_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnext/
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnext/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnext/resnext101-32x4d_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnext/resnext101-32x8d_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnext/resnext152-32x4d_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnext/resnext50-32x4d_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/revvit/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/revvit/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/revvit/revvit-base_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/revvit/revvit-small_8xb256_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-m36-deploy_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-m36-deploy_8xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-m48-deploy_8xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-m48-deploy_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-s12-deploy_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-s12-deploy_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-s24-deploy_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-s24-deploy_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-s36-deploy_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/deploy/riformer-s36-deploy_8xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-m36_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-m36_8xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-m48_8xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-m48_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s12_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s12_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s24_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s24_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s36_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s36_8xb64_in1k-384px.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/seresnet/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/seresnet/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/seresnet/seresnet101_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/seresnet/seresnet50_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/seresnet/seresnext101-32x4d_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/seresnet/seresnext50-32x4d_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/shufflenet_v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/shufflenet_v1/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/shufflenet_v1/shufflenet-v1-1x_16xb64_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/shufflenet_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/shufflenet_v2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/shufflenet_v2/shufflenet-v2-1x_16xb64_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/benchmarks/resnet50_8xb512-linear-coslr-90e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/simclr_resnet50_16xb256-coslr-200e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/simclr_resnet50_16xb256-coslr-800e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/simclr_resnet50_8xb32-coslr-200e_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/benchmarks/swin-base-w6_8xb256-coslr-100e_in1k-192px.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/benchmarks/swin-base-w7_8xb256-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/benchmarks/swin-large-w14_8xb256-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_16xb128-amp-coslr-100e_in1k-192px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_16xb128-amp-coslr-800e_in1k-192px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_8xb256-amp-coslr-100e_in1k-192px.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/simmim_swin-large-w12_16xb128-amp-coslr-800e_in1k-192px.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simsiam/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simsiam/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simsiam/benchmarks/resnet50_8xb512-linear-coslr-90e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simsiam/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simsiam/simsiam_resnet50_8xb32-coslr-100e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simsiam/simsiam_resnet50_8xb32-coslr-200e_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swav/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swav/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swav/benchmarks/resnet50_8xb512-linear-coslr-90e_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swav/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swav/swav_resnet50_8xb32-mcrop-coslr-200e_in1k-224px-96px.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/swin-base_16xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/swin-base_16xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/swin-large_16xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/swin-large_16xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/swin-large_8xb8_cub-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/swin-small_16xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/swin-tiny_16xb64_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w12_8xb128_in21k-192px.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w16_16xb64_in1k-256px.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w16_in21k-pre_16xb64_in1k-256px.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w24_in21k-pre_16xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w8_16xb64_in1k-256px.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-large-w12_8xb128_in21k-192px.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-large-w16_in21k-pre_16xb64_in1k-256px.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-large-w24_in21k-pre_16xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-small-w16_16xb64_in1k-256px.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-small-w8_16xb64_in1k-256px.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-tiny-w16_16xb64_in1k-256px.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-tiny-w8_16xb64_in1k-256px.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/t2t_vit/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/t2t_vit/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-14_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-19_8xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-24_8xb64_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-11m-distill_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-11m_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k-512px.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-21m_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-5m-distill_8xb256_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-5m_8xb256_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tnt/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tnt/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tnt/tnt-s-p16_16xb64_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/twins-pcpvt-base_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/twins-pcpvt-large_16xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/twins-pcpvt-small_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/twins-svt-base_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/twins-svt-large_16xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/twins-svt-small_8xb128_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/van-base_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/van-large_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/van-small_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/van-tiny_8xb128_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg11_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg11bn_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg13_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg13bn_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg16_8xb16_voc.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg16_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg16bn_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg19_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg19bn_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/pvig-base_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/pvig-medium_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/pvig-small_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/pvig-tiny_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/vig-base_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/vig-small_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/vig-tiny_8xb128_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_32xb128-mae_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_4xb544-ipu_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_64xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p32_64xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p32_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-large-p16_64xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-large-p16_64xb64_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-large-p32_64xb64_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-large-p32_64xb64_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/wrn/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/wrn/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/wrn/wide-resnet101_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/wrn/wide-resnet50_8xb32_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/wrn/wide-resnet50_timm_8xb32_in1k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/
--rw-r--r--   0 runner    (1001) docker     (123)    28291 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/metafile.yml
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-large-24-p16_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-large-24-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-large-24-p8_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-large-24-p8_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-medium-24-p16_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-medium-24-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-medium-24-p8_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-medium-24-p8_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-nano-12-p16_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-nano-12-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-nano-12-p8_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-nano-12-p8_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-12-p16_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-12-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-12-p8_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-12-p8_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-24-p16_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-24-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-24-p8_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-24-p8_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p16_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p8_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p8_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p16_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p16_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p8_8xb128_in1k-384px.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p8_8xb128_in1k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-07 10:25:16.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/model-index.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/analyze_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/analyze_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/eval_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/get_flops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_dist_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_dist_train_c4.sh
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_dist_train_fpn.sh
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_train_c4.sh
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_train_fpn.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmsegmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_dist_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_dist_train.sh
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_slurm_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_slurm_train.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/dataset_converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/dataset_converters/convert_imagenet_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/dataset_converters/convert_inaturalist.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/dist_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/dist_train.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/kfold-cross-valid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/misc/print_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/misc/verify_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/clip_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/convnext_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/davit_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/deit3_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/edgenext_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/efficientnet_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/efficientnetv2_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/eva_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/hornet2mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/levit2mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/mixmim_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/mlpmixer_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/mobilenetv2_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/publish_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/reparameterize_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/replknet_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/repvgg_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/revvit_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/shufflenetv2_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/tinyvit_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/torchvision_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/twins2mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/van2mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/vgg_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/vig_to_mmpretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/slurm_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/slurm_train.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/torchserve/
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/torchserve/mmpretrain2torchserve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/torchserve/mmpretrain_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/torchserve/test_torchserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/visualization/browse_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/visualization/vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/visualization/vis_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/visualization/vis_tsne.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/apis/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/apis/image_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/apis/image_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/apis/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    38321 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/cub.py
--rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/inshop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/multi_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/places205.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/samplers/repeat_aug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48570 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/auto_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    56203 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/class_num_check_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/densecl_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/margin_head_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/precise_bn_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/retriever_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/simsiam_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/swav_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/switch_recipe_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/visualization_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/adan_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/layer_decay_optim_wrapper_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/functional/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24925 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/multi_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/multi_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)    31789 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/single_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/voc_multi_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/alexnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/base_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)    22489 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/convmixer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/convnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    25507 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/cspnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    30645 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/davit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/deit.py
--rw-r--r--   0 runner    (1001) docker     (123)    17185 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/deit3.py
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/edgenext.py
--rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/efficientformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18959 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/hornet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/lenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/levit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19834 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mixmim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mlp_mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mobileone.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mobilevit.py
--rw-r--r--   0 runner    (1001) docker     (123)    26094 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mvit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/poolformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/regnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/replknet.py
--rw-r--r--   0 runner    (1001) docker     (123)    22849 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/repmlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    22087 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/repvgg.py
--rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/res2net.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    23819 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/resnet_cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    24265 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/revvit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/riformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/seresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/seresnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/shufflenet_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/shufflenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/swin_transformer_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/t2t_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/timm_backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)    26505 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/tinyvit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/tnt.py
--rw-r--r--   0 runner    (1001) docker     (123)    30218 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/twins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/van.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/vgg.py
--rw-r--r--   0 runner    (1001) docker     (123)    31677 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/vig.py
--rw-r--r--   0 runner    (1001) docker     (123)    18440 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/backbones/xcit.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/beitv1_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/beitv2_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/cae_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/cls_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/conformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/contrastive_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/deit_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/efficientformer_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/latent_heads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/levit_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/linear_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/mae_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/margin_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/mim_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/mixmim_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/mocov3_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/multi_label_cls_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/multi_label_csra_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/multi_label_linear_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/multi_task_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/simmim_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/stacked_head.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/swav_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/vig_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/heads/vision_transformer_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/asymmetric_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/cae_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/cosine_similarity_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/label_smooth_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/reconstruction_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/seesaw_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/swav_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/beitv2_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/cae_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/densecl_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/gap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/gem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/hr_fuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/linear_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/mae_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/milan_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/mixmim_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/mocov2_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/nonlinear_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/simmim_neck.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/necks/swav_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/retrievers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/retrievers/image2image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/barlowtwins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/byol.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/cae.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/densecl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/eva.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/mae.py
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/maskfeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/milan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/mixmim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/moco.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/mocov3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/simclr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/simmim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/swav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/tta/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/tta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/tta/score_tta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44577 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/cutmix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/resizemix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/channel_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/clip_generator_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    22155 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/layer_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/res_layer_extra_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/models/utils/vector_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/structures/data_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/structures/multi_task_data_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/structures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/utils/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/mmpretrain/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/mmpretrain/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18892 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63599 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 10:25:17.000000 mmpretrain-1.0.0rc7/mmpretrain.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/requirements/mminstall.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/requirements/optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/requirements/readthedocs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-07 10:25:18.000000 mmpretrain-1.0.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-07 10:25:14.000000 mmpretrain-1.0.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/cifar100_bs16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/cifar10_bs16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/coco_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/coco_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/coco_vg_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/coco_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/cub_bs8_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/cub_bs8_448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet21k_bs128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_mbv3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_medium_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_small_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_revvit_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_medium_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_small_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_vig_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_196.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_336.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_560.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_pil_bicubic_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_beitv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_davit_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_levit_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_simmim_192.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_swin_192.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_byol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_mocov2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_pil_bicubic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_pil_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs512_mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs512_mocov3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_autoaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_convmixer_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_deit3_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_deit3_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_edgenext_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_mixer_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_pil_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_pil_resize_autoaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_t2t_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs8_pil_bicubic_320.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/inshop_bs32_448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/nlvr2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/pipelines/auto_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/pipelines/rand_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/refcoco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/voc_bs16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/conformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/conformer/base-p16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/conformer/small-p16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/conformer/small-p32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/conformer/tiny-p16.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convmixer/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convmixer/convmixer-1024-20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convmixer/convmixer-1536-20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convmixer/convmixer-768-32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-xlarge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/atto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/femto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/huge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/nano.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/pico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/tiny.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/davit/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/davit/davit-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/davit/davit-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/davit/davit-tiny.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-base-p16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-base-p16-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-huge-p14-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-large-p16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-large-p16-384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-medium-p16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-small-p16-224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-small-p16-384.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/densenet/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/densenet/densenet121.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/densenet/densenet161.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/densenet/densenet169.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/densenet/densenet201.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/edgenext/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-xsmall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-xxsmall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientformer-l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_b3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_b4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_b5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_b6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_b7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_b8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_l2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_b0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_b1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_b2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_b3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_l.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientnet_v2/efficientnetv2_xl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/eva/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/eva/eva-g.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/eva/eva-l.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-base-gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large-gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large-gf384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-small-gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-tiny-gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-tiny.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w30.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w40.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w44.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w48.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hrnet/hrnet-w64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/levit-256-p16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mae_vit-base-p16.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mixmim/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mixmim/mixmim_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mlp_mixer_base_patch16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mlp_mixer_large_patch16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v2_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_large_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_050_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_075_imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_imagenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobileone/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobileone/mobileone_s4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilevit/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilevit/mobilevit_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilevit/mobilevit_xs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilevit/mobilevit_xxs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mvit/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-tiny.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_m36.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_m48.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s24.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s36.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/regnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_1.6gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_12gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_3.2gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_4.0gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_400mf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_6.4gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_8.0gf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/regnet/regnetx_800mf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/replknet-31B_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/replknet-31L_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/replknet-XL_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/repmlp-base_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/repvgg-A0_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/repvgg-B3_lbs-mixup_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/res2net101-w26-s4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/res2net50-w14-s8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/res2net50-w26-s4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/res2net50-w26-s6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/res2net50-w26-s8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/res2net50-w48-s2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnest101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnest200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnest269.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnest50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet101_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet152_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet18_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet34.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet34_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet34_gem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet50_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet50_cifar_cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet50_cifar_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet50_cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet50_label_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet50_mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnetv1c50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnetv1d101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnetv1d152.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnetv1d50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnext152_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnext50_32x4d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/revvit/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/revvit/revvit-base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/revvit/revvit-small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/seresnet101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/seresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/seresnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/seresnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/shufflenet_v1_1x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/shufflenet_v2_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/base_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/base_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/large_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/large_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/small_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/tiny_224.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/base_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/base_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/large_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/large_384.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/small_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/tiny_256.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-14.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-19.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-24.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/tinyvit/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-11m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-21m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-5m.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/tnt_s_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/twins_pcpvt_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/twins_svt_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/van/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/van/van_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/van/van_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/van/van_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/van/van_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vgg11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vgg11bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vgg13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vgg13bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vgg16bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vgg19bn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/vig_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/vig_small.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/vig_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vit-base-p16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vit-base-p32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vit-large-p16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vit-large-p32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/wide-resnet50.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/cifar10_bs128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/cub_bs64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_revvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_swin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_coslr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_linearlr_bn_nowd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_AdamW.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_adamw_levit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_coslr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_rsb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_140e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_200e_coslr_warmup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_coslr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_coslr_coswd_300e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_epochstep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs4096_AdamW.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_lars_coslr_200e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_lars_coslr_90e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_sgd_coslr_100e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_sgd_coslr_200e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_sgd_steplr_100e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/arcface/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/arcface/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/arcface/resnet50-arcface_8xb32_inshop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/barlowtwins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/barlowtwins/barlowtwins_resnet50_8xb256-coslr-1000e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/barlowtwins/barlowtwins_resnet50_8xb256-coslr-300e_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/barlowtwins/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/barlowtwins/benchmarks/resnet50_8xb32-linear-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/barlowtwins/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/beit_beit-base-p16_8xb256-amp-coslr-300e_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-1600e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-300e_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip/blip-base_8xb16_refcoco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip/blip-base_8xb32_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip/blip-base_8xb32_nlvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip/blip-base_8xb32_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip/blip-base_8xb32_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip2/blip2-opt2.7b_8xb16_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip2/blip2-opt2.7b_8xb32_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip2/blip2_8xb32_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/blip2/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50-c4_ms-1x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50_fpn_ms-1x_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/benchmarks/resnet50_8xb512-linear-coslr-90e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/byol_resnet50_16xb256-coslr-200e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cae/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cae/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cae/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cae/cae_beit-base-p16_8xb256-amp-coslr-300e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cae/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/chinese_clip/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/chinese_clip/cn-clip_resnet50_zeroshot-cls_cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/chinese_clip/cn-clip_vit-base-p16_zeroshot-cls_cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/chinese_clip/cn-clip_vit-huge-p14_zeroshot-cls_cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/chinese_clip/cn-clip_vit-large-p14_zeroshot-cls_cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/chinese_clip/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)    11724 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-448px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-448px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-large-p14_headless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/conformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/conformer/conformer-base-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/conformer/conformer-small-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/conformer/conformer-small-p32_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/conformer/conformer-tiny-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/conformer/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convmixer/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convmixer/convmixer-1024-20_10xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convmixer/convmixer-1536-20_10xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convmixer/convmixer-768-32_10xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convmixer/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-small_32xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-small_32xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-tiny_32xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-tiny_32xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15777 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-atto_32xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-base_32xb32_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-base_32xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-femto_32xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k-512px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-large_32xb32_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-large_32xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-nano_32xb32_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-nano_32xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-pico_32xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-tiny_32xb32_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-tiny_32xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cspnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cspnet/cspdarknet50_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cspnet/cspresnet50_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cspnet/cspresnext50_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cspnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/csra/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/csra/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/csra/resnet101-csra_1xb16_voc07-448px.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/davit/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/davit/davit-base_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/davit/davit-small_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/davit/davit-tiny_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/davit/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-base-distilled_16xb32_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-base-distilled_16xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-base_16xb32_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-base_16xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-small-distilled_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-small_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-tiny-distilled_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-tiny_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-base-p16_64xb32_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-base-p16_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-huge-p14_64xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-large-p16_64xb16_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-large-p16_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-medium-p16_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-small-p16_64xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-small-p16_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densecl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densecl/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densecl/benchmarks/resnet50_8xb32-linear-steplr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densecl/densecl_resnet50_8xb32-coslr-200e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densecl/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densenet/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densenet/densenet121_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densenet/densenet161_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densenet/densenet169_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densenet/densenet201_4xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densenet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/dinov2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/dinov2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/dinov2/vit-base-p14_dinov2-pre_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/dinov2/vit-giant-p14_dinov2-pre_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/dinov2/vit-large-p14_dinov2-pre_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/dinov2/vit-small-p14_dinov2-pre_headless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-base_8xb256-usi_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-base_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-small_8xb256-usi_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-small_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-xsmall_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-xxsmall_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientformer/efficientformer-l1_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientformer/efficientformer-l3_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientformer/efficientformer-l7_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientformer/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b0_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b0_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b1_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b1_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b2_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b2_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b3_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b3_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b4_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b4_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b5_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b5_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b6_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b6_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b7_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b7_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b8_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b8_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-em_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-es_8xb32-01norm_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-l2_8xb32_in1k-475px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-l2_8xb8_in1k-800px.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25083 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b0_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b1_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b2_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b3_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-l_8xb32_in1k-480px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-l_8xb32_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-m_8xb32_in1k-480px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-m_8xb32_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-s_8xb32_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-s_8xb32_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-xl_8xb32_in1k-512px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-xl_8xb32_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb2048-linear-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-g-p14_8xb16_in1k-336px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-g-p14_8xb16_in1k-560px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-g-p14_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-g-p16_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-l-p14_8xb16_in1k-196px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-l-p14_8xb16_in1k-336px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-l-p14_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-mae-style_vit-base-p16_16xb256-coslr-400e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/eva02-base-p14_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/eva02-base-p14_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/eva02-large-p14_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/eva02-large-p14_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/eva02-small-p14_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/eva02-small-p14_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/eva02-tiny-p14_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/eva02-tiny-p14_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8019 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva02/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/flamingo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/flamingo/flamingo_fewshot_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/flamingo/flamingo_fewshot_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/flamingo/flamingo_zeroshot_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/flamingo/flamingo_zeroshot_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/flamingo/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/glip/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/glip/glip-l_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/glip/glip-t_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/glip/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hornet/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hornet/hornet-base-gf_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hornet/hornet-base_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hornet/hornet-small-gf_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hornet/hornet-small_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hornet/hornet-tiny-gf_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hornet/hornet-tiny_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hornet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/hrnet-w18_4xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/hrnet-w30_4xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/hrnet-w32_4xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/hrnet-w40_4xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/hrnet-w44_4xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/hrnet-w48_4xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/hrnet-w64_4xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/inception_v3/inception-v3_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/inception_v3/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/lenet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/lenet/lenet5_mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/deploy/levit-128_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/deploy/levit-128s_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/deploy/levit-192_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/deploy/levit-256_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/deploy/levit-384_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/levit-128_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/levit-128s_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/levit-192_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/levit-256_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/levit-384_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-base-p16_8xb2048-linear-coslr-90e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-huge-p14_32xb8-coslr-50e_in1k-448px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-huge-p14_8xb128-coslr-50e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-large-p16_8xb128-coslr-50e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-large-p16_8xb2048-linear-coslr-90e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-1600e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-300e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-400e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-800e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-huge-p14_8xb512-amp-coslr-1600e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-1600e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-300e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-400e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-800e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/maskfeat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/maskfeat/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/maskfeat/benchmarks/vit-base-p16_8xb256-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/maskfeat/maskfeat_vit-base-p16_8xb256-amp-coslr-300e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/maskfeat/metafile.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/benchmarks/vit-base-p16_8xb2048-linear-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/milan_vit-base-p16_16xb256-amp-coslr-400e_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mixmim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mixmim/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mixmim/benchmarks/mixmim-base_8xb128-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mixmim/benchmarks/mixmim-base_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mixmim/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mixmim/mixmim_mixmim-base_16xb128-coslr-300e_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mlp_mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mlp_mixer/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mlp_mixer/mlp-mixer-base-p16_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mlp_mixer/mlp-mixer-large-p16_64xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v2/mobilenet-v2_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-large_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small-050_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small-075_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small_8xb16_cifar10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s0_deploy_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s1_deploy_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s2_deploy_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s3_deploy_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/deploy/mobileone-s4_deploy_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s0_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s1_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s2_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s3_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s4_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilevit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilevit/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilevit/mobilevit-small_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilevit/mobilevit-xsmall_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilevit/mobilevit-xxsmall_8xb128_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov2/benchmarks/resnet50_8xb32-linear-steplr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov2/mocov2_resnet50_8xb32-coslr-200e_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/resnet50_8xb128-linear-coslr-90e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/vit-base-p16_8xb128-linear-coslr-90e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/vit-base-p16_8xb64-coslr-150e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/vit-large-p16_8xb64-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/vit-small-p16_8xb128-linear-coslr-90e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-300e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-800e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_vit-base-p16_16xb256-amp-coslr-300e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_vit-large-p16_64xb64-amp-coslr-300e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_vit-small-p16_16xb256-amp-coslr-300e_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/mvitv2-base_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/mvitv2-large_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/mvitv2-small_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/mvitv2-tiny_8xb256_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/ofa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/ofa/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/ofa/ofa-base_finetuned_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/ofa/ofa-base_finetuned_refcoco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/ofa/ofa-base_finetuned_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/ofa/ofa-base_zeroshot_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/ofa/ofa-large_zeroshot_vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-m36_32xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-m48_32xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-s12_32xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-s24_32xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-s36_32xb128_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-1.6gf_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-12gf_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-3.2gf_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-4.0gf_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-400mf_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-6.4gf_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-8.0gf_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-800mf_8xb128_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/deploy/replknet-31B-deploy_32xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/deploy/replknet-31B-deploy_32xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/deploy/replknet-31L-deploy_32xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/deploy/replknet-XL-deploy_32xb64_in1k-320px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/replknet-31B_32xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/replknet-31B_32xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/replknet-31L_32xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/replknet-XL_32xb64_in1k-320px.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repmlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repmlp/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repmlp/repmlp-base_8xb64_in1k-256px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repmlp/repmlp-base_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repmlp/repmlp-base_delopy_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repmlp/repmlp-base_deploy_8xb64_in1k-256px.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-A0_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-A0_deploy_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-A1_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-A2_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-B0_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-B1_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-B1g2_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-B1g4_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-B2_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-B2g4_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-B3_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-B3g4_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-D2se_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/res2net/
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/res2net/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/res2net/res2net101-w26-s4_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/res2net/res2net50-w14-s8_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/res2net/res2net50-w26-s8_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/_randaug_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/resnest101_32xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/resnest200_64xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/resnest269_64xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/resnest50_32xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet101_8xb16_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet101_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet152_8xb16_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet152_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet18_8xb16_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet18_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet34_8xb16_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet34_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_32xb64-warmup-coslr_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_32xb64-warmup-lbs_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_32xb64-warmup_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb128_coslr-90e_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb16-mixup_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb16_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb16_cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a1-600e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a2-300e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a3-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb32-coslr-preciseBN_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb32-coslr_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb32-cutmix_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb32-fp16-dynamic_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb32-fp16_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb32-lbs_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb32-mixup_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb8_cub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnetv1c101_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnetv1c152_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnetv1c50_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnetv1d101_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnetv1d152_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnetv1d50_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnext/
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnext/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnext/resnext101-32x4d_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnext/resnext101-32x8d_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnext/resnext152-32x4d_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnext/resnext50-32x4d_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/revvit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/revvit/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/revvit/revvit-base_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/revvit/revvit-small_8xb256_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-m36-deploy_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-m36-deploy_8xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-m48-deploy_8xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-m48-deploy_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-s12-deploy_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-s12-deploy_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-s24-deploy_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-s24-deploy_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-s36-deploy_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/deploy/riformer-s36-deploy_8xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-m36_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-m36_8xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-m48_8xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-m48_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s12_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s12_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s24_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s24_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s36_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s36_8xb64_in1k-384px.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/sam/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/sam/vit-base-p16_sam_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/sam/vit-huge-p16_sam_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/sam/vit-large-p16_sam_headless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/seresnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/seresnet/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/seresnet/seresnet101_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/seresnet/seresnet50_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/seresnet/seresnext101-32x4d_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/seresnet/seresnext50-32x4d_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/shufflenet_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/shufflenet_v1/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/shufflenet_v1/shufflenet-v1-1x_16xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/shufflenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/shufflenet_v2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/shufflenet_v2/shufflenet-v2-1x_16xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/benchmarks/resnet50_8xb512-linear-coslr-90e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/simclr_resnet50_16xb256-coslr-200e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/simclr_resnet50_16xb256-coslr-800e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/simclr_resnet50_8xb32-coslr-200e_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/benchmarks/swin-base-w6_8xb256-coslr-100e_in1k-192px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/benchmarks/swin-base-w7_8xb256-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/benchmarks/swin-large-w14_8xb256-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_16xb128-amp-coslr-100e_in1k-192px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_16xb128-amp-coslr-800e_in1k-192px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_8xb256-amp-coslr-100e_in1k-192px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/simmim_swin-large-w12_16xb128-amp-coslr-800e_in1k-192px.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simsiam/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simsiam/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simsiam/benchmarks/resnet50_8xb512-linear-coslr-90e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simsiam/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simsiam/simsiam_resnet50_8xb32-coslr-100e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simsiam/simsiam_resnet50_8xb32-coslr-200e_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swav/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swav/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swav/benchmarks/resnet50_8xb512-linear-coslr-90e_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swav/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swav/swav_resnet50_8xb32-mcrop-coslr-200e_in1k-224px-96px.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/swin-base_16xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/swin-base_16xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/swin-large_16xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/swin-large_16xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/swin-large_8xb8_cub-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/swin-small_16xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/swin-tiny_16xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w12_8xb128_in21k-192px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w16_16xb64_in1k-256px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w16_in21k-pre_16xb64_in1k-256px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w24_in21k-pre_16xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w8_16xb64_in1k-256px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-large-w12_8xb128_in21k-192px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-large-w16_in21k-pre_16xb64_in1k-256px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-large-w24_in21k-pre_16xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-small-w16_16xb64_in1k-256px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-small-w8_16xb64_in1k-256px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-tiny-w16_16xb64_in1k-256px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-tiny-w8_16xb64_in1k-256px.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/t2t_vit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/t2t_vit/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-14_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-19_8xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-24_8xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-11m-distill_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-11m_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k-512px.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-21m_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-5m-distill_8xb256_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-5m_8xb256_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tnt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tnt/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tnt/tnt-s-p16_16xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/twins-pcpvt-base_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/twins-pcpvt-large_16xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/twins-pcpvt-small_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/twins-svt-base_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/twins-svt-large_16xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/twins-svt-small_8xb128_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/van-base_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/van-large_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/van-small_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/van-tiny_8xb128_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg11_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg11bn_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg13_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg13bn_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg16_8xb16_voc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg16_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg16bn_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg19_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg19bn_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/pvig-base_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/pvig-medium_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/pvig-small_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/pvig-tiny_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/vig-base_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/vig-small_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/vig-tiny_8xb128_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_32xb128-mae_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_4xb544-ipu_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_64xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p32_64xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p32_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-large-p16_64xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-large-p16_64xb64_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-large-p32_64xb64_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-large-p32_64xb64_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/wrn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/wrn/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/wrn/wide-resnet101_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/wrn/wide-resnet50_8xb32_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/wrn/wide-resnet50_timm_8xb32_in1k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/
+-rw-r--r--   0 runner    (1001) docker     (123)    28291 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/metafile.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-large-24-p16_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-large-24-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-large-24-p8_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-large-24-p8_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-medium-24-p16_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-medium-24-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-medium-24-p8_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-medium-24-p8_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-nano-12-p16_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-nano-12-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-nano-12-p8_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-nano-12-p8_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-12-p16_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-12-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-12-p8_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-12-p8_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-24-p16_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-24-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-24-p8_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-24-p8_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p16_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p8_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p8_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p16_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p16_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p8_8xb128_in1k-384px.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p8_8xb128_in1k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/model-index.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/analyze_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/analyze_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/eval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/get_flops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_dist_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_dist_train_c4.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_dist_train_fpn.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_train_c4.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_train_fpn.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmsegmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_dist_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_dist_train.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_slurm_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_slurm_train.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/dataset_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/dataset_converters/convert_imagenet_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/dataset_converters/convert_inaturalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/dist_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/dist_train.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8957 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/kfold-cross-valid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/misc/print_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/misc/verify_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/clip_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/convnext_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/davit_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/deit3_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/edgenext_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/efficientnet_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/efficientnetv2_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/eva02_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/eva_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/glip_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/hornet2mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/levit2mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/mixmim_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/mlpmixer_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/mobilenetv2_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/ofa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/publish_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/reparameterize_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/replknet_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/repvgg_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/revvit_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/shufflenetv2_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/tinyvit_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/torchvision_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/twins2mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/van2mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/vgg_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/vig_to_mmpretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/slurm_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/slurm_train.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/torchserve/
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/torchserve/mmpretrain2torchserve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/torchserve/mmpretrain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/torchserve/test_torchserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/visualization/browse_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/visualization/vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/visualization/vis_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/visualization/vis_tsne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/image_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/image_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10928 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/image_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23773 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/multimodal_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/nlvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/visual_grounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/apis/visual_question_answering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/caltech101.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58132 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/coco_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/coco_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/coco_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/cub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10408 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/dtd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/fgvcaircraft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/flamingo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/flowers102.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/food101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/inshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11053 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/multi_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/nlvr2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/oxfordiiitpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/places205.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/refcoco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/samplers/repeat_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/samplers/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/scienceqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/stanfordcars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/sun397.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48878 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/auto_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63637 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/vg_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/visual_genome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/class_num_check_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/densecl_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/margin_head_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/precise_bn_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/retriever_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/simsiam_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/swav_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/switch_recipe_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/warmup_param_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/adan_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/layer_decay_optim_wrapper_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/engine/runners/retrieval_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24925 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/multi_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/scienceqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31789 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/single_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/visual_grounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/voc_multi_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/alexnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/base_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22489 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/convmixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25507 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/cspnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30645 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/davit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/deit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17185 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/deit3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/edgenext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/efficientformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18959 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/hornet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23396 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18806 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/lenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18201 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/levit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19834 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mixmim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mlp_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18955 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mobileone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mobilevit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26094 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/poolformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/regnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/replknet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22849 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/repmlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22087 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/repvgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/res2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24500 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/resnet_cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24265 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/revvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/riformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/seresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/seresnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/shufflenet_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/shufflenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23638 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/swin_transformer_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16685 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/t2t_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/timm_backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26505 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/tinyvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/tnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30218 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/van.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31677 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/vig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19677 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/vit_eva02.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27014 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/vit_sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29245 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/backbones/xcit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/beitv1_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/beitv2_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/cae_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/conformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/contrastive_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/deit_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/efficientformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/grounding_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/itc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/itm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/latent_heads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/levit_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/linear_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/mae_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/margin_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/mim_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/mixmim_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/mocov3_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/multi_label_cls_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/multi_label_csra_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/multi_label_linear_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/multi_task_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/seq_gen_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/simmim_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/stacked_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/swav_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/vig_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/vision_transformer_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/heads/vqa_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/asymmetric_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/cae_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/cosine_similarity_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/label_smooth_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/reconstruction_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/seesaw_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/swav_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip/blip_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip/blip_grounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip/blip_nlvr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28731 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip/blip_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10422 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip/blip_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52002 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip/language_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip2/
+-rw-r--r--   0 runner    (1001) docker     (123)    32118 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip2/Qformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip2/blip2_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip2/blip2_opt_vqa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21891 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip2/blip2_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48175 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/blip2/modeling_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/chinese_clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/chinese_clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/chinese_clip/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16720 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/chinese_clip/chinese_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/chinese_clip/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/flamingo/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/flamingo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/flamingo/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/flamingo/flamingo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/flamingo/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/flamingo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/ofa/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/ofa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/ofa/ofa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64644 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/multimodal/ofa/ofa_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/beitv2_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/cae_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/densecl_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/gap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/gem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/hr_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/linear_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6939 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/mae_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/milan_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/mixmim_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/mocov2_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/nonlinear_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/simmim_neck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/necks/swav_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/retrievers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/retrievers/image2image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/barlowtwins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/byol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/cae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/densecl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/eva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/maskfeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/milan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/mixmim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/moco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/mocov3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/simmim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/swav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/tta/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/tta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/tta/score_tta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45478 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/resizemix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/channel_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13411 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/clip_generator_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25992 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/layer_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/res_layer_extra_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/swiglu_ffn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/models/utils/vector_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/structures/data_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/structures/multi_task_data_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/structures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/utils/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/utils/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33454 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/mmpretrain/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    69771 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/mmpretrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/requirements/mminstall.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/requirements/multimodal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/requirements/optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/requirements/readthedocs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-23 03:25:07.000000 mmpretrain-1.0.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-23 03:25:03.000000 mmpretrain-1.0.0rc8/setup.py
```

### Comparing `mmpretrain-1.0.0rc7/PKG-INFO` & `mmpretrain-1.0.0rc8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,321 +1,328 @@
-Metadata-Version: 2.1
-Name: mmpretrain
-Version: 1.0.0rc7
-Summary: OpenMMLab Model Pretraining Toolbox and Benchmark
-Home-page: https://github.com/open-mmlab/mmpretrain
-Author: MMPretrain Contributors
-Author-email: openmmlab@gmail.com
-License: Apache License 2.0
-Description: <div align="center">
-        
-        <img src="resources/mmpt-logo.png" width="600"/>
-          <div>&nbsp;</div>
-          <div align="center">
-            <b><font size="5">OpenMMLab website</font></b>
-            <sup>
-              <a href="https://openmmlab.com">
-                <i><font size="4">HOT</font></i>
-              </a>
-            </sup>
-            &nbsp;&nbsp;&nbsp;&nbsp;
-            <b><font size="5">OpenMMLab platform</font></b>
-            <sup>
-              <a href="https://platform.openmmlab.com">
-                <i><font size="4">TRY IT OUT</font></i>
-              </a>
-            </sup>
-          </div>
-          <div>&nbsp;</div>
-        
-        [![PyPI](https://img.shields.io/pypi/v/mmpretrain)](https://pypi.org/project/mmpretrain)
-        [![Docs](https://img.shields.io/badge/docs-latest-blue)](https://mmpretrain.readthedocs.io/en/latest/)
-        [![Build Status](https://github.com/open-mmlab/mmpretrain/workflows/build/badge.svg)](https://github.com/open-mmlab/mmpretrain/actions)
-        [![codecov](https://codecov.io/gh/open-mmlab/mmpretrain/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmpretrain)
-        [![license](https://img.shields.io/github/license/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/blob/main/LICENSE)
-        [![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/issues)
-        [![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/issues)
-        
-        [📘 Documentation](https://mmpretrain.readthedocs.io/en/latest/) |
-        [🛠️ Installation](https://mmpretrain.readthedocs.io/en/latest/get_started.html#installation) |
-        [👀 Model Zoo](https://mmpretrain.readthedocs.io/en/latest/modelzoo_statistics.html) |
-        [🆕 Update News](https://mmpretrain.readthedocs.io/en/latest/notes/changelog.html) |
-        [🤔 Reporting Issues](https://github.com/open-mmlab/mmpretrain/issues/new/choose)
-        
-        <img src="https://user-images.githubusercontent.com/36138628/230307505-4727ad0a-7d71-4069-939d-b499c7e272b7.png" width="400"/>
-        
-        English | [简体中文](/README_zh-CN.md)
-        
-        </div>
-        
-        </div>
-        
-        <div align="center">
-          <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://discord.gg/raweFPmdzG" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
-          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-          <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
-            <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
-        </div>
-        
-        ## Introduction
-        
-        MMPreTrain is an open source pre-training toolbox based on PyTorch. It is a part of the [OpenMMLab](https://openmmlab.com/) project.
-        
-        The `main` branch works with **PyTorch 1.8+**.
-        
-        ### Major features
-        
-        - Various backbones and pretrained models
-        - Rich training strategies(supervised learning, self-supervised learning, etc.)
-        - Bag of training tricks
-        - Large-scale training configs
-        - High efficiency and extensibility
-        - Powerful toolkits for model analysis and experiments
-        
-        ## What's new
-        
-        🌟 v1.0.0rc7 was released in 07/04/2023
-        
-        - Integrated Self-supervised learning algorithms from **MMSelfSup**, such as **MAE**, **BEiT**, etc.
-        - Support **RIFormer**, a simple but effective vision backbone by removing token mixer.
-        - Add t-SNE visualization.
-        - Refactor dataset pipeline visualization.
-        
-        Update of previous versions
-        
-        - Support **LeViT**, **XCiT**, **ViG**, **ConvNeXt-V2**, **EVA**, **RevViT**, **EfficientnetV2**, **CLIP**, **TinyViT** and **MixMIM** backbones.
-        - Reproduce the training accuracy of **ConvNeXt** and **RepVGG**.
-        - Support confusion matrix calculation and plot.
-        - Support **multi-task** training and testing.
-        - Support Test-time Augmentation.
-        - Upgrade API to get pre-defined models of MMPreTrain.
-        - Refactor BEiT backbone and support v1/v2 inference.
-        
-        This release introduced a brand new and flexible training & test engine, but it's still in progress. Welcome
-        to try according to [the documentation](https://mmpretrain.readthedocs.io/en/latest/).
-        
-        And there are some BC-breaking changes. Please check [the migration tutorial](https://mmpretrain.readthedocs.io/en/latest/migration.html).
-        
-        Please refer to [changelog](https://mmpretrain.readthedocs.io/en/latest/notes/changelog.html) for more details and other release history.
-        
-        ## Installation
-        
-        Below are quick steps for installation:
-        
-        ```shell
-        conda create -n open-mmlab python=3.8 pytorch==1.10.1 torchvision==0.11.2 cudatoolkit=11.3 -c pytorch -y
-        conda activate open-mmlab
-        pip install openmim
-        git clone https://github.com/open-mmlab/mmpretrain.git
-        cd mmpretrain
-        mim install -e .
-        ```
-        
-        Please refer to [installation documentation](https://mmpretrain.readthedocs.io/en/latest/get_started.html) for more detailed installation and dataset preparation.
-        
-        ## User Guides
-        
-        We provided a series of tutorials about the basic usage of MMPreTrain for new users:
-        
-        - [Learn about Configs](https://mmpretrain.readthedocs.io/en/latest/user_guides/config.html)
-        - [Prepare Dataset](https://mmpretrain.readthedocs.io/en/latest/user_guides/dataset_prepare.html)
-        - [Inference with existing models](https://mmpretrain.readthedocs.io/en/latest/user_guides/inference.html)
-        - [Train](https://mmpretrain.readthedocs.io/en/latest/user_guides/train.html)
-        - [Test](https://mmpretrain.readthedocs.io/en/latest/user_guides/test.html)
-        - [Downstream tasks](https://mmpretrain.readthedocs.io/en/latest/user_guides/downstream.html)
-        
-        For more information, please refer to [our documentation](https://mmpretrain.readthedocs.io/en/latest/).
-        
-        ## Model zoo
-        
-        Results and models are available in the [model zoo](https://mmpretrain.readthedocs.io/en/latest/modelzoo_statistics.html).
-        
-        <div align="center">
-          <b>Overview</b>
-        </div>
-        <table align="center">
-          <tbody>
-            <tr align="center" valign="bottom">
-              <td>
-                <b>Supported Backbones</b>
-              </td>
-              <td>
-                <b>Self-supervised Learning</b>
-              </td>
-              <td>
-                <b>Others</b>
-              </td>
-            </tr>
-            <tr valign="top">
-              <td>
-                <ul>
-                <li><a href="configs/vgg">VGG</a></li>
-                <li><a href="configs/resnet">ResNet</a></li>
-                <li><a href="configs/resnext">ResNeXt</a></li>
-                <li><a href="configs/seresnet">SE-ResNet</a></li>
-                <li><a href="configs/seresnet">SE-ResNeXt</a></li>
-                <li><a href="configs/regnet">RegNet</a></li>
-                <li><a href="configs/shufflenet_v1">ShuffleNet V1</a></li>
-                <li><a href="configs/shufflenet_v2">ShuffleNet V2</a></li>
-                <li><a href="configs/mobilenet_v2">MobileNet V2</a></li>
-                <li><a href="configs/mobilenet_v3">MobileNet V3</a></li>
-                <li><a href="configs/swin_transformer">Swin-Transformer</a></li>
-                <li><a href="configs/swin_transformer_v2">Swin-Transformer V2</a></li>
-                <li><a href="configs/repvgg">RepVGG</a></li>
-                <li><a href="configs/vision_transformer">Vision-Transformer</a></li>
-                <li><a href="configs/tnt">Transformer-in-Transformer</a></li>
-                <li><a href="configs/res2net">Res2Net</a></li>
-                <li><a href="configs/mlp_mixer">MLP-Mixer</a></li>
-                <li><a href="configs/deit">DeiT</a></li>
-                <li><a href="configs/deit3">DeiT-3</a></li>
-                <li><a href="configs/conformer">Conformer</a></li>
-                <li><a href="configs/t2t_vit">T2T-ViT</a></li>
-                <li><a href="configs/twins">Twins</a></li>
-                <li><a href="configs/efficientnet">EfficientNet</a></li>
-                <li><a href="configs/edgenext">EdgeNeXt</a></li>
-                <li><a href="configs/convnext">ConvNeXt</a></li>
-                <li><a href="configs/hrnet">HRNet</a></li>
-                <li><a href="configs/van">VAN</a></li>
-                <li><a href="configs/convmixer">ConvMixer</a></li>
-                <li><a href="configs/cspnet">CSPNet</a></li>
-                <li><a href="configs/poolformer">PoolFormer</a></li>
-                <li><a href="configs/inception_v3">Inception V3</a></li>
-                <li><a href="configs/mobileone">MobileOne</a></li>
-                <li><a href="configs/efficientformer">EfficientFormer</a></li>
-                <li><a href="configs/mvit">MViT</a></li>
-                <li><a href="configs/hornet">HorNet</a></li>
-                <li><a href="configs/mobilevit">MobileViT</a></li>
-                <li><a href="configs/davit">DaViT</a></li>
-                <li><a href="configs/replknet">RepLKNet</a></li>
-                <li><a href="configs/beit">BEiT</a></li>
-                <li><a href="configs/mixmim">MixMIM</a></li>
-                <li><a href="configs/efficientnet_v2">EfficientNet V2</a></li>
-                <li><a href="configs/revvit">RevViT</a></li>
-                <li><a href="configs/convnext_v2">ConvNeXt V2</a></li>
-                <li><a href="configs/vig">ViG</a></li>
-                <li><a href="configs/xcit">XCiT</a></li>
-                <li><a href="configs/levit">LeViT</a></li>
-                <li><a href="configs/riformer">RIFormer</a></li>
-                </ul>
-              </td>
-              <td>
-                <ul>
-                <li><a href="configs/mocov2">MoCo V1 (CVPR'2020)</a></li>
-                <li><a href="configs/simclr">SimCLR (ICML'2020)</a></li>
-                <li><a href="configs/mocov2">MoCo V2 (arXiv'2020)</a></li>
-                <li><a href="configs/byol">BYOL (NeurIPS'2020)</a></li>
-                <li><a href="configs/swav">SwAV (NeurIPS'2020)</a></li>
-                <li><a href="configs/densecl">DenseCL (CVPR'2021)</a></li>
-                <li><a href="configs/simsiam">SimSiam (CVPR'2021)</a></li>
-                <li><a href="configs/barlowtwins">Barlow Twins (ICML'2021)</a></li>
-                <li><a href="configs/mocov3">MoCo V3 (ICCV'2021)</a></li>
-                <li><a href="configs/beit">BEiT (ICLR'2022)</a></li>
-                <li><a href="configs/mae">MAE (CVPR'2022)</a></li>
-                <li><a href="configs/simmim">SimMIM (CVPR'2022)</a></li>
-                <li><a href="configs/maskfeat">MaskFeat (CVPR'2022)</a></li>
-                <li><a href="configs/cae">CAE (arXiv'2022)</a></li>
-                <li><a href="configs/milan">MILAN (arXiv'2022)</a></li>
-                <li><a href="configs/beitv2">BEiT V2 (arXiv'2022)</a></li>
-                <li><a href="configs/eva">EVA (CVPR'2023)</a></li>
-                <li><a href="configs/mixmim">MixMIM (arXiv'2022)</a></li>
-                </ul>
-              </td>
-              <td>
-              Image Retrieval Task:
-                <ul>
-                <li><a href="configs/arcface">ArcFace (CVPR'2019)</a></li>
-                </ul>
-              Training&Test Tips:
-                <ul>
-                <li><a href="https://arxiv.org/abs/1909.13719">RandAug</a></li>
-                <li><a href="https://arxiv.org/abs/1805.09501">AutoAug</a></li>
-                <li><a href="mmpretrain/datasets/samplers/repeat_aug.py">RepeatAugSampler</a></li>
-                <li><a href="mmpretrain/models/tta/score_tta.py">TTA</a></li>
-                <li>...</li>
-                </ul>
-              </td>
-          </tbody>
-        </table>
-        
-        ## Contributing
-        
-        We appreciate all contributions to improve MMPreTrain.
-        Please refer to [CONTRUBUTING](https://mmpretrain.readthedocs.io/en/latest/notes/contribution_guide.html) for the contributing guideline.
-        
-        ## Acknowledgement
-        
-        MMPreTrain is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors who implement their methods or add new features, as well as users who give valuable feedbacks.
-        We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and supporting their own academic research.
-        
-        ## Citation
-        
-        If you find this project useful in your research, please consider cite:
-        
-        ```BibTeX
-        @misc{2023mmpretrain,
-            title={OpenMMLab's Pre-training Toolbox and Benchmark},
-            author={MMPreTrain Contributors},
-            howpublished = {\url{https://github.com/open-mmlab/mmpretrain}},
-            year={2023}
-        }
-        ```
-        
-        ## License
-        
-        This project is released under the [Apache 2.0 license](LICENSE).
-        
-        ## Projects in OpenMMLab
-        
-        - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
-        - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
-        - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
-        - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
-        - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
-        - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
-        - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
-        - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-        - [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
-        - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
-        - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-        - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
-        - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
-        - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
-        - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
-        - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-        - [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing toolbox.
-        - [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
-        - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
-        
-Keywords: computer vision,image classification,unsupervised learning,self-supervised learning
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: tests
-Provides-Extra: optional
-Provides-Extra: mim
+<div align="center">
+
+<img src="resources/mmpt-logo.png" width="600"/>
+  <div>&nbsp;</div>
+  <div align="center">
+    <b><font size="5">OpenMMLab website</font></b>
+    <sup>
+      <a href="https://openmmlab.com">
+        <i><font size="4">HOT</font></i>
+      </a>
+    </sup>
+    &nbsp;&nbsp;&nbsp;&nbsp;
+    <b><font size="5">OpenMMLab platform</font></b>
+    <sup>
+      <a href="https://platform.openmmlab.com">
+        <i><font size="4">TRY IT OUT</font></i>
+      </a>
+    </sup>
+  </div>
+  <div>&nbsp;</div>
+
+[![PyPI](https://img.shields.io/pypi/v/mmpretrain)](https://pypi.org/project/mmpretrain)
+[![Docs](https://img.shields.io/badge/docs-latest-blue)](https://mmpretrain.readthedocs.io/en/latest/)
+[![Build Status](https://github.com/open-mmlab/mmpretrain/workflows/build/badge.svg)](https://github.com/open-mmlab/mmpretrain/actions)
+[![codecov](https://codecov.io/gh/open-mmlab/mmpretrain/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmpretrain)
+[![license](https://img.shields.io/github/license/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/blob/main/LICENSE)
+[![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/issues)
+[![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/issues)
+
+[📘 Documentation](https://mmpretrain.readthedocs.io/en/latest/) |
+[🛠️ Installation](https://mmpretrain.readthedocs.io/en/latest/get_started.html#installation) |
+[👀 Model Zoo](https://mmpretrain.readthedocs.io/en/latest/modelzoo_statistics.html) |
+[🆕 Update News](https://mmpretrain.readthedocs.io/en/latest/notes/changelog.html) |
+[🤔 Reporting Issues](https://github.com/open-mmlab/mmpretrain/issues/new/choose)
+
+<img src="https://user-images.githubusercontent.com/36138628/230307505-4727ad0a-7d71-4069-939d-b499c7e272b7.png" width="400"/>
+
+English | [简体中文](/README_zh-CN.md)
+
+</div>
+
+</div>
+
+<div align="center">
+  <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://discord.gg/raweFPmdzG" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
+  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+  <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
+    <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
+</div>
+
+## Introduction
+
+MMPreTrain is an open source pre-training toolbox based on PyTorch. It is a part of the [OpenMMLab](https://openmmlab.com/) project.
+
+The `main` branch works with **PyTorch 1.8+**.
+
+### Major features
+
+- Various backbones and pretrained models
+- Rich training strategies (supervised learning, self-supervised learning, multi-modality learning etc.)
+- Bag of training tricks
+- Large-scale training configs
+- High efficiency and extensibility
+- Powerful toolkits for model analysis and experiments
+- Various out-of-box inference tasks.
+  - Image Classification
+  - Image Caption
+  - Visual Question Answering
+  - Visual Grounding
+  - Retrieval (Image-To-Image, Text-To-Image, Image-To-Text)
+
+https://github.com/open-mmlab/mmpretrain/assets/26739999/e4dcd3a2-f895-4d1b-a351-fbc74a04e904
+
+## What's new
+
+🌟 v1.0.0rc8 was released in 22/05/2023
+
+- Support multiple **multi-modal** algorithms and inferencers. You can explore these features by the [gradio demo](https://github.com/open-mmlab/mmpretrain/tree/main/projects/gradio_demo)!
+- Add EVA-02, Dino-V2, ViT-SAM and GLIP backbones.
+- Register torchvision transforms into MMPretrain, you can now easily integrate torchvision's data augmentations in MMPretrain. See [the doc](https://mmpretrain.readthedocs.io/en/latest/api/data_process.html#torchvision-transforms)
+
+🌟 v1.0.0rc7 was released in 07/04/2023
+
+- Integrated Self-supervised learning algorithms from **MMSelfSup**, such as **MAE**, **BEiT**, etc.
+- Support **RIFormer**, a simple but effective vision backbone by removing token mixer.
+- Add t-SNE visualization.
+- Refactor dataset pipeline visualization.
+
+Update of previous versions
+
+- Support **LeViT**, **XCiT**, **ViG**, **ConvNeXt-V2**, **EVA**, **RevViT**, **EfficientnetV2**, **CLIP**, **TinyViT** and **MixMIM** backbones.
+- Reproduce the training accuracy of **ConvNeXt** and **RepVGG**.
+- Support confusion matrix calculation and plot.
+- Support **multi-task** training and testing.
+- Support Test-time Augmentation.
+- Upgrade API to get pre-defined models of MMPreTrain.
+- Refactor BEiT backbone and support v1/v2 inference.
+
+This release introduced a brand new and flexible training & test engine, but it's still in progress. Welcome
+to try according to [the documentation](https://mmpretrain.readthedocs.io/en/latest/).
+
+And there are some BC-breaking changes. Please check [the migration tutorial](https://mmpretrain.readthedocs.io/en/latest/migration.html).
+
+Please refer to [changelog](https://mmpretrain.readthedocs.io/en/latest/notes/changelog.html) for more details and other release history.
+
+## Installation
+
+Below are quick steps for installation:
+
+```shell
+conda create -n open-mmlab python=3.8 pytorch==1.10.1 torchvision==0.11.2 cudatoolkit=11.3 -c pytorch -y
+conda activate open-mmlab
+pip install openmim
+git clone https://github.com/open-mmlab/mmpretrain.git
+cd mmpretrain
+mim install -e .
+```
+
+Please refer to [installation documentation](https://mmpretrain.readthedocs.io/en/latest/get_started.html) for more detailed installation and dataset preparation.
+
+For multi-modality models support, please install the extra dependencies by:
+
+```shell
+mim install -e ".[multimodal]"
+```
+
+## User Guides
+
+We provided a series of tutorials about the basic usage of MMPreTrain for new users:
+
+- [Learn about Configs](https://mmpretrain.readthedocs.io/en/latest/user_guides/config.html)
+- [Prepare Dataset](https://mmpretrain.readthedocs.io/en/latest/user_guides/dataset_prepare.html)
+- [Inference with existing models](https://mmpretrain.readthedocs.io/en/latest/user_guides/inference.html)
+- [Train](https://mmpretrain.readthedocs.io/en/latest/user_guides/train.html)
+- [Test](https://mmpretrain.readthedocs.io/en/latest/user_guides/test.html)
+- [Downstream tasks](https://mmpretrain.readthedocs.io/en/latest/user_guides/downstream.html)
+
+For more information, please refer to [our documentation](https://mmpretrain.readthedocs.io/en/latest/).
+
+## Model zoo
+
+Results and models are available in the [model zoo](https://mmpretrain.readthedocs.io/en/latest/modelzoo_statistics.html).
+
+<div align="center">
+  <b>Overview</b>
+</div>
+<table align="center">
+  <tbody>
+    <tr align="center" valign="bottom">
+      <td>
+        <b>Supported Backbones</b>
+      </td>
+      <td>
+        <b>Self-supervised Learning</b>
+      </td>
+      <td>
+        <b>Multi-Modality Algorithms</b>
+      </td>
+      <td>
+        <b>Others</b>
+      </td>
+    </tr>
+    <tr valign="top">
+      <td>
+        <ul>
+        <li><a href="configs/vgg">VGG</a></li>
+        <li><a href="configs/resnet">ResNet</a></li>
+        <li><a href="configs/resnext">ResNeXt</a></li>
+        <li><a href="configs/seresnet">SE-ResNet</a></li>
+        <li><a href="configs/seresnet">SE-ResNeXt</a></li>
+        <li><a href="configs/regnet">RegNet</a></li>
+        <li><a href="configs/shufflenet_v1">ShuffleNet V1</a></li>
+        <li><a href="configs/shufflenet_v2">ShuffleNet V2</a></li>
+        <li><a href="configs/mobilenet_v2">MobileNet V2</a></li>
+        <li><a href="configs/mobilenet_v3">MobileNet V3</a></li>
+        <li><a href="configs/swin_transformer">Swin-Transformer</a></li>
+        <li><a href="configs/swin_transformer_v2">Swin-Transformer V2</a></li>
+        <li><a href="configs/repvgg">RepVGG</a></li>
+        <li><a href="configs/vision_transformer">Vision-Transformer</a></li>
+        <li><a href="configs/tnt">Transformer-in-Transformer</a></li>
+        <li><a href="configs/res2net">Res2Net</a></li>
+        <li><a href="configs/mlp_mixer">MLP-Mixer</a></li>
+        <li><a href="configs/deit">DeiT</a></li>
+        <li><a href="configs/deit3">DeiT-3</a></li>
+        <li><a href="configs/conformer">Conformer</a></li>
+        <li><a href="configs/t2t_vit">T2T-ViT</a></li>
+        <li><a href="configs/twins">Twins</a></li>
+        <li><a href="configs/efficientnet">EfficientNet</a></li>
+        <li><a href="configs/edgenext">EdgeNeXt</a></li>
+        <li><a href="configs/convnext">ConvNeXt</a></li>
+        <li><a href="configs/hrnet">HRNet</a></li>
+        <li><a href="configs/van">VAN</a></li>
+        <li><a href="configs/convmixer">ConvMixer</a></li>
+        <li><a href="configs/cspnet">CSPNet</a></li>
+        <li><a href="configs/poolformer">PoolFormer</a></li>
+        <li><a href="configs/inception_v3">Inception V3</a></li>
+        <li><a href="configs/mobileone">MobileOne</a></li>
+        <li><a href="configs/efficientformer">EfficientFormer</a></li>
+        <li><a href="configs/mvit">MViT</a></li>
+        <li><a href="configs/hornet">HorNet</a></li>
+        <li><a href="configs/mobilevit">MobileViT</a></li>
+        <li><a href="configs/davit">DaViT</a></li>
+        <li><a href="configs/replknet">RepLKNet</a></li>
+        <li><a href="configs/beit">BEiT</a></li>
+        <li><a href="configs/mixmim">MixMIM</a></li>
+        <li><a href="configs/efficientnet_v2">EfficientNet V2</a></li>
+        <li><a href="configs/revvit">RevViT</a></li>
+        <li><a href="configs/convnext_v2">ConvNeXt V2</a></li>
+        <li><a href="configs/vig">ViG</a></li>
+        <li><a href="configs/xcit">XCiT</a></li>
+        <li><a href="configs/levit">LeViT</a></li>
+        <li><a href="configs/riformer">RIFormer</a></li>
+        <li><a href="configs/glip">GLIP</a></li>
+        </ul>
+      </td>
+      <td>
+        <ul>
+        <li><a href="configs/mocov2">MoCo V1 (CVPR'2020)</a></li>
+        <li><a href="configs/simclr">SimCLR (ICML'2020)</a></li>
+        <li><a href="configs/mocov2">MoCo V2 (arXiv'2020)</a></li>
+        <li><a href="configs/byol">BYOL (NeurIPS'2020)</a></li>
+        <li><a href="configs/swav">SwAV (NeurIPS'2020)</a></li>
+        <li><a href="configs/densecl">DenseCL (CVPR'2021)</a></li>
+        <li><a href="configs/simsiam">SimSiam (CVPR'2021)</a></li>
+        <li><a href="configs/barlowtwins">Barlow Twins (ICML'2021)</a></li>
+        <li><a href="configs/mocov3">MoCo V3 (ICCV'2021)</a></li>
+        <li><a href="configs/beit">BEiT (ICLR'2022)</a></li>
+        <li><a href="configs/mae">MAE (CVPR'2022)</a></li>
+        <li><a href="configs/simmim">SimMIM (CVPR'2022)</a></li>
+        <li><a href="configs/maskfeat">MaskFeat (CVPR'2022)</a></li>
+        <li><a href="configs/cae">CAE (arXiv'2022)</a></li>
+        <li><a href="configs/milan">MILAN (arXiv'2022)</a></li>
+        <li><a href="configs/beitv2">BEiT V2 (arXiv'2022)</a></li>
+        <li><a href="configs/eva">EVA (CVPR'2023)</a></li>
+        <li><a href="configs/mixmim">MixMIM (arXiv'2022)</a></li>
+        </ul>
+      </td>
+      <td>
+        <ul>
+        <li><a href="configs/blip">BLIP (arxiv'2022)</a></li>
+        <li><a href="configs/blip2">BLIP-2 (arxiv'2023)</a></li>
+        <li><a href="configs/ofa">OFA (CoRR'2022)</a></li>
+        <li><a href="configs/flamingo">Flamingo (NeurIPS'2022)</a></li>
+        <li><a href="configs/chinese_clip">Chinese CLIP (arxiv'2022)</a></li>
+        </ul>
+      </td>
+      <td>
+      Image Retrieval Task:
+        <ul>
+        <li><a href="configs/arcface">ArcFace (CVPR'2019)</a></li>
+        </ul>
+      Training&Test Tips:
+        <ul>
+        <li><a href="https://arxiv.org/abs/1909.13719">RandAug</a></li>
+        <li><a href="https://arxiv.org/abs/1805.09501">AutoAug</a></li>
+        <li><a href="mmpretrain/datasets/samplers/repeat_aug.py">RepeatAugSampler</a></li>
+        <li><a href="mmpretrain/models/tta/score_tta.py">TTA</a></li>
+        <li>...</li>
+        </ul>
+      </td>
+  </tbody>
+</table>
+
+## Contributing
+
+We appreciate all contributions to improve MMPreTrain.
+Please refer to [CONTRUBUTING](https://mmpretrain.readthedocs.io/en/latest/notes/contribution_guide.html) for the contributing guideline.
+
+## Acknowledgement
+
+MMPreTrain is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors who implement their methods or add new features, as well as users who give valuable feedbacks.
+We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and supporting their own academic research.
+
+## Citation
+
+If you find this project useful in your research, please consider cite:
+
+```BibTeX
+@misc{2023mmpretrain,
+    title={OpenMMLab's Pre-training Toolbox and Benchmark},
+    author={MMPreTrain Contributors},
+    howpublished = {\url{https://github.com/open-mmlab/mmpretrain}},
+    year={2023}
+}
+```
+
+## License
+
+This project is released under the [Apache 2.0 license](LICENSE).
+
+## Projects in OpenMMLab
+
+- [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
+- [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
+- [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
+- [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
+- [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
+- [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
+- [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
+- [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
+- [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
+- [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
+- [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
+- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
+- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
+- [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
+- [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
+- [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
+- [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
+- [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
+- [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
+- [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
+- [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
+- [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+- [Playground](https://github.com/open-mmlab/playground): A central hub for gathering and showcasing amazing projects built upon OpenMMLab.
```

#### html2text {}

```diff
@@ -1,11 +1,7 @@
-Metadata-Version: 2.1 Name: mmpretrain Version: 1.0.0rc7 Summary: OpenMMLab
-Model Pretraining Toolbox and Benchmark Home-page: https://github.com/open-
-mmlab/mmpretrain Author: MMPretrain Contributors Author-email:
-openmmlab@gmail.com License: Apache License 2.0 Description:
                            [resources/mmpt-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
  [![PyPI](https://img.shields.io/pypi/v/mmpretrain)](https://pypi.org/project/
  mmpretrain) [![Docs](https://img.shields.io/badge/docs-latest-blue)](https://
 mmpretrain.readthedocs.io/en/latest/) [![Build Status](https://github.com/open-
@@ -26,18 +22,29 @@
  Issues](https://github.com/open-mmlab/mmpretrain/issues/new/choose) [https://
  user-images.githubusercontent.com/36138628/230307505-4727ad0a-7d71-4069-939d-
          b499c7e272b7.png] English | [ç®ä½ä¸­æ](/README_zh-CN.md)
 
 ## Introduction MMPreTrain is an open source pre-training toolbox based on
 PyTorch. It is a part of the [OpenMMLab](https://openmmlab.com/) project. The
 `main` branch works with **PyTorch 1.8+**. ### Major features - Various
-backbones and pretrained models - Rich training strategies(supervised learning,
-self-supervised learning, etc.) - Bag of training tricks - Large-scale training
-configs - High efficiency and extensibility - Powerful toolkits for model
-analysis and experiments ## What's new ð v1.0.0rc7 was released in 07/04/
+backbones and pretrained models - Rich training strategies (supervised
+learning, self-supervised learning, multi-modality learning etc.) - Bag of
+training tricks - Large-scale training configs - High efficiency and
+extensibility - Powerful toolkits for model analysis and experiments - Various
+out-of-box inference tasks. - Image Classification - Image Caption - Visual
+Question Answering - Visual Grounding - Retrieval (Image-To-Image, Text-To-
+Image, Image-To-Text) https://github.com/open-mmlab/mmpretrain/assets/26739999/
+e4dcd3a2-f895-4d1b-a351-fbc74a04e904 ## What's new ð v1.0.0rc8 was released
+in 22/05/2023 - Support multiple **multi-modal** algorithms and inferencers.
+You can explore these features by the [gradio demo](https://github.com/open-
+mmlab/mmpretrain/tree/main/projects/gradio_demo)! - Add EVA-02, Dino-V2, ViT-
+SAM and GLIP backbones. - Register torchvision transforms into MMPretrain, you
+can now easily integrate torchvision's data augmentations in MMPretrain. See
+[the doc](https://mmpretrain.readthedocs.io/en/latest/api/
+data_process.html#torchvision-transforms) ð v1.0.0rc7 was released in 07/04/
 2023 - Integrated Self-supervised learning algorithms from **MMSelfSup**, such
 as **MAE**, **BEiT**, etc. - Support **RIFormer**, a simple but effective
 vision backbone by removing token mixer. - Add t-SNE visualization. - Refactor
 dataset pipeline visualization. Update of previous versions - Support
 **LeViT**, **XCiT**, **ViG**, **ConvNeXt-V2**, **EVA**, **RevViT**,
 **EfficientnetV2**, **CLIP**, **TinyViT** and **MixMIM** backbones. - Reproduce
 the training accuracy of **ConvNeXt** and **RepVGG**. - Support confusion
@@ -52,62 +59,68 @@
 mmpretrain.readthedocs.io/en/latest/notes/changelog.html) for more details and
 other release history. ## Installation Below are quick steps for installation:
 ```shell conda create -n open-mmlab python=3.8 pytorch==1.10.1
 torchvision==0.11.2 cudatoolkit=11.3 -c pytorch -y conda activate open-mmlab
 pip install openmim git clone https://github.com/open-mmlab/mmpretrain.git cd
 mmpretrain mim install -e . ``` Please refer to [installation documentation]
 (https://mmpretrain.readthedocs.io/en/latest/get_started.html) for more
-detailed installation and dataset preparation. ## User Guides We provided a
-series of tutorials about the basic usage of MMPreTrain for new users: - [Learn
-about Configs](https://mmpretrain.readthedocs.io/en/latest/user_guides/
-config.html) - [Prepare Dataset](https://mmpretrain.readthedocs.io/en/latest/
-user_guides/dataset_prepare.html) - [Inference with existing models](https://
+detailed installation and dataset preparation. For multi-modality models
+support, please install the extra dependencies by: ```shell mim install -e ".
+[multimodal]" ``` ## User Guides We provided a series of tutorials about the
+basic usage of MMPreTrain for new users: - [Learn about Configs](https://
+mmpretrain.readthedocs.io/en/latest/user_guides/config.html) - [Prepare
+Dataset](https://mmpretrain.readthedocs.io/en/latest/user_guides/
+dataset_prepare.html) - [Inference with existing models](https://
 mmpretrain.readthedocs.io/en/latest/user_guides/inference.html) - [Train]
 (https://mmpretrain.readthedocs.io/en/latest/user_guides/train.html) - [Test]
 (https://mmpretrain.readthedocs.io/en/latest/user_guides/test.html) -
 [Downstream tasks](https://mmpretrain.readthedocs.io/en/latest/user_guides/
 downstream.html) For more information, please refer to [our documentation]
 (https://mmpretrain.readthedocs.io/en/latest/). ## Model zoo Results and models
 are available in the [model zoo](https://mmpretrain.readthedocs.io/en/latest/
 modelzoo_statistics.html).
                                    Overview
-    Supported Backbones    Self-supervised Learning                Others
-    * VGG                     * MoCo_V1_(CVPR'2020)  Image Retrieval Task:
-    * ResNet                  * SimCLR_(ICML'2020)       * ArcFace_(CVPR'2019)
-    * ResNeXt                 * MoCo_V2_(arXiv'2020) Training&Test Tips:
-    * SE-ResNet               * BYOL_(NeurIPS'2020)      * RandAug
-    * SE-ResNeXt              * SwAV_(NeurIPS'2020)      * AutoAug
-    * RegNet                  * DenseCL_(CVPR'2021)      * RepeatAugSampler
-    * ShuffleNet_V1           * SimSiam_(CVPR'2021)      * TTA
-    * ShuffleNet_V2           * Barlow_Twins_            * ...
-    * MobileNet_V2              (ICML'2021)
-    * MobileNet_V3            * MoCo_V3_(ICCV'2021)
-    * Swin-Transformer        * BEiT_(ICLR'2022)
-    * Swin-Transformer_V2     * MAE_(CVPR'2022)
-    * RepVGG                  * SimMIM_(CVPR'2022)
-    * Vision-Transformer      * MaskFeat_(CVPR'2022)
-    * Transformer-in-         * CAE_(arXiv'2022)
-      Transformer             * MILAN_(arXiv'2022)
-    * Res2Net                 * BEiT_V2_(arXiv'2022)
-    * MLP-Mixer               * EVA_(CVPR'2023)
-    * DeiT                    * MixMIM_(arXiv'2022)
-    * DeiT-3
-    * Conformer
-    * T2T-ViT
-    * Twins
-    * EfficientNet
-    * EdgeNeXt
-    * ConvNeXt
-    * HRNet
-    * VAN
-    * ConvMixer
-    * CSPNet
-    * PoolFormer
-    * Inception_V3
-    * MobileOne
+                         Self-supervised       Multi-Modality
+ Supported Backbones         Learning            Algorithms                 Others
+    * VGG                 * MoCo_V1_           * BLIP_          Image Retrieval Task:
+    * ResNet                (CVPR'2020)          (arxiv'2022)       * ArcFace_
+    * ResNeXt             * SimCLR_            * BLIP-2_              (CVPR'2019)
+    * SE-ResNet             (ICML'2020)          (arxiv'2023)   Training&Test Tips:
+    * SE-ResNeXt          * MoCo_V2_           * OFA_               * RandAug
+    * RegNet                (arXiv'2020)         (CoRR'2022)        * AutoAug
+    * ShuffleNet_V1       * BYOL_              * Flamingo_          * RepeatAugSampler
+    * ShuffleNet_V2         (NeurIPS'2020)       (NeurIPS'2022)     * TTA
+    * MobileNet_V2        * SwAV_              * Chinese_CLIP_      * ...
+    * MobileNet_V3          (NeurIPS'2020)       (arxiv'2022)
+    * Swin-               * DenseCL_
+      Transformer           (CVPR'2021)
+    * Swin-               * SimSiam_
+      Transformer_V2        (CVPR'2021)
+    * RepVGG              * Barlow_Twins_
+    * Vision-               (ICML'2021)
+      Transformer         * MoCo_V3_
+    * Transformer-in-       (ICCV'2021)
+      Transformer         * BEiT_
+    * Res2Net               (ICLR'2022)
+    * MLP-Mixer           * MAE_
+    * DeiT                  (CVPR'2022)
+    * DeiT-3              * SimMIM_
+    * Conformer             (CVPR'2022)
+    * T2T-ViT             * MaskFeat_
+    * Twins                 (CVPR'2022)
+    * EfficientNet        * CAE_
+    * EdgeNeXt              (arXiv'2022)
+    * ConvNeXt            * MILAN_
+    * HRNet                 (arXiv'2022)
+    * VAN                 * BEiT_V2_
+    * ConvMixer             (arXiv'2022)
+    * CSPNet              * EVA_
+    * PoolFormer            (CVPR'2023)
+    * Inception_V3        * MixMIM_
+    * MobileOne             (arXiv'2022)
     * EfficientFormer
     * MViT
     * HorNet
     * MobileViT
     * DaViT
     * RepLKNet
     * BEiT
@@ -115,14 +128,15 @@
     * EfficientNet_V2
     * RevViT
     * ConvNeXt_V2
     * ViG
     * XCiT
     * LeViT
     * RIFormer
+    * GLIP
 ## Contributing We appreciate all contributions to improve MMPreTrain. Please
 refer to [CONTRUBUTING](https://mmpretrain.readthedocs.io/en/latest/notes/
 contribution_guide.html) for the contributing guideline. ## Acknowledgement
 MMPreTrain is an open source project that is contributed by researchers and
 engineers from various colleges and companies. We appreciate all the
 contributors who implement their methods or add new features, as well as users
 who give valuable feedbacks. We wish that the toolbox and benchmark could serve
@@ -155,23 +169,14 @@
 OpenMMLab self-supervised learning toolbox and benchmark. - [MMRazor](https://
 github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and
 benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab
 fewshot learning toolbox and benchmark. - [MMAction2](https://github.com/open-
 mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and
 benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
 video perception toolbox and benchmark. - [MMFlow](https://github.com/open-
-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMEditing]
-(https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing
-toolbox. - [MMGeneration](https://github.com/open-mmlab/mmgeneration):
-OpenMMLab image and video generative models toolbox. - [MMDeploy](https://
-github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
-Keywords: computer vision,image classification,unsupervised learning,self-
-supervised learning Platform: UNKNOWN Classifier: Development Status :: 4 -
-Beta Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Requires-Python: >=3.7 Description-Content-Type: text/
-markdown Provides-Extra: all Provides-Extra: tests Provides-Extra: optional
-Provides-Extra: mim
+mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMagic](https:/
+/github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and
+**I**ntelligent **C**reation toolbox. - [MMGeneration](https://github.com/open-
+mmlab/mmgeneration): OpenMMLab image and video generative models toolbox. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. - [Playground](https://github.com/open-mmlab/playground): A central
+hub for gathering and showcasing amazing projects built upon OpenMMLab.
```

### Comparing `mmpretrain-1.0.0rc7/README.md` & `mmpretrain-1.0.0rc8/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,294 +1,356 @@
-<div align="center">
-
-<img src="resources/mmpt-logo.png" width="600"/>
-  <div>&nbsp;</div>
-  <div align="center">
-    <b><font size="5">OpenMMLab website</font></b>
-    <sup>
-      <a href="https://openmmlab.com">
-        <i><font size="4">HOT</font></i>
-      </a>
-    </sup>
-    &nbsp;&nbsp;&nbsp;&nbsp;
-    <b><font size="5">OpenMMLab platform</font></b>
-    <sup>
-      <a href="https://platform.openmmlab.com">
-        <i><font size="4">TRY IT OUT</font></i>
-      </a>
-    </sup>
-  </div>
-  <div>&nbsp;</div>
-
-[![PyPI](https://img.shields.io/pypi/v/mmpretrain)](https://pypi.org/project/mmpretrain)
-[![Docs](https://img.shields.io/badge/docs-latest-blue)](https://mmpretrain.readthedocs.io/en/latest/)
-[![Build Status](https://github.com/open-mmlab/mmpretrain/workflows/build/badge.svg)](https://github.com/open-mmlab/mmpretrain/actions)
-[![codecov](https://codecov.io/gh/open-mmlab/mmpretrain/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmpretrain)
-[![license](https://img.shields.io/github/license/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/blob/main/LICENSE)
-[![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/issues)
-[![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/issues)
-
-[📘 Documentation](https://mmpretrain.readthedocs.io/en/latest/) |
-[🛠️ Installation](https://mmpretrain.readthedocs.io/en/latest/get_started.html#installation) |
-[👀 Model Zoo](https://mmpretrain.readthedocs.io/en/latest/modelzoo_statistics.html) |
-[🆕 Update News](https://mmpretrain.readthedocs.io/en/latest/notes/changelog.html) |
-[🤔 Reporting Issues](https://github.com/open-mmlab/mmpretrain/issues/new/choose)
-
-<img src="https://user-images.githubusercontent.com/36138628/230307505-4727ad0a-7d71-4069-939d-b499c7e272b7.png" width="400"/>
-
-English | [简体中文](/README_zh-CN.md)
-
-</div>
-
-</div>
-
-<div align="center">
-  <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://discord.gg/raweFPmdzG" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
-  <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
-  <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
-    <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
-</div>
-
-## Introduction
-
-MMPreTrain is an open source pre-training toolbox based on PyTorch. It is a part of the [OpenMMLab](https://openmmlab.com/) project.
-
-The `main` branch works with **PyTorch 1.8+**.
-
-### Major features
-
-- Various backbones and pretrained models
-- Rich training strategies(supervised learning, self-supervised learning, etc.)
-- Bag of training tricks
-- Large-scale training configs
-- High efficiency and extensibility
-- Powerful toolkits for model analysis and experiments
-
-## What's new
-
-🌟 v1.0.0rc7 was released in 07/04/2023
-
-- Integrated Self-supervised learning algorithms from **MMSelfSup**, such as **MAE**, **BEiT**, etc.
-- Support **RIFormer**, a simple but effective vision backbone by removing token mixer.
-- Add t-SNE visualization.
-- Refactor dataset pipeline visualization.
-
-Update of previous versions
-
-- Support **LeViT**, **XCiT**, **ViG**, **ConvNeXt-V2**, **EVA**, **RevViT**, **EfficientnetV2**, **CLIP**, **TinyViT** and **MixMIM** backbones.
-- Reproduce the training accuracy of **ConvNeXt** and **RepVGG**.
-- Support confusion matrix calculation and plot.
-- Support **multi-task** training and testing.
-- Support Test-time Augmentation.
-- Upgrade API to get pre-defined models of MMPreTrain.
-- Refactor BEiT backbone and support v1/v2 inference.
-
-This release introduced a brand new and flexible training & test engine, but it's still in progress. Welcome
-to try according to [the documentation](https://mmpretrain.readthedocs.io/en/latest/).
-
-And there are some BC-breaking changes. Please check [the migration tutorial](https://mmpretrain.readthedocs.io/en/latest/migration.html).
-
-Please refer to [changelog](https://mmpretrain.readthedocs.io/en/latest/notes/changelog.html) for more details and other release history.
-
-## Installation
-
-Below are quick steps for installation:
-
-```shell
-conda create -n open-mmlab python=3.8 pytorch==1.10.1 torchvision==0.11.2 cudatoolkit=11.3 -c pytorch -y
-conda activate open-mmlab
-pip install openmim
-git clone https://github.com/open-mmlab/mmpretrain.git
-cd mmpretrain
-mim install -e .
-```
-
-Please refer to [installation documentation](https://mmpretrain.readthedocs.io/en/latest/get_started.html) for more detailed installation and dataset preparation.
-
-## User Guides
-
-We provided a series of tutorials about the basic usage of MMPreTrain for new users:
-
-- [Learn about Configs](https://mmpretrain.readthedocs.io/en/latest/user_guides/config.html)
-- [Prepare Dataset](https://mmpretrain.readthedocs.io/en/latest/user_guides/dataset_prepare.html)
-- [Inference with existing models](https://mmpretrain.readthedocs.io/en/latest/user_guides/inference.html)
-- [Train](https://mmpretrain.readthedocs.io/en/latest/user_guides/train.html)
-- [Test](https://mmpretrain.readthedocs.io/en/latest/user_guides/test.html)
-- [Downstream tasks](https://mmpretrain.readthedocs.io/en/latest/user_guides/downstream.html)
-
-For more information, please refer to [our documentation](https://mmpretrain.readthedocs.io/en/latest/).
-
-## Model zoo
-
-Results and models are available in the [model zoo](https://mmpretrain.readthedocs.io/en/latest/modelzoo_statistics.html).
-
-<div align="center">
-  <b>Overview</b>
-</div>
-<table align="center">
-  <tbody>
-    <tr align="center" valign="bottom">
-      <td>
-        <b>Supported Backbones</b>
-      </td>
-      <td>
-        <b>Self-supervised Learning</b>
-      </td>
-      <td>
-        <b>Others</b>
-      </td>
-    </tr>
-    <tr valign="top">
-      <td>
-        <ul>
-        <li><a href="configs/vgg">VGG</a></li>
-        <li><a href="configs/resnet">ResNet</a></li>
-        <li><a href="configs/resnext">ResNeXt</a></li>
-        <li><a href="configs/seresnet">SE-ResNet</a></li>
-        <li><a href="configs/seresnet">SE-ResNeXt</a></li>
-        <li><a href="configs/regnet">RegNet</a></li>
-        <li><a href="configs/shufflenet_v1">ShuffleNet V1</a></li>
-        <li><a href="configs/shufflenet_v2">ShuffleNet V2</a></li>
-        <li><a href="configs/mobilenet_v2">MobileNet V2</a></li>
-        <li><a href="configs/mobilenet_v3">MobileNet V3</a></li>
-        <li><a href="configs/swin_transformer">Swin-Transformer</a></li>
-        <li><a href="configs/swin_transformer_v2">Swin-Transformer V2</a></li>
-        <li><a href="configs/repvgg">RepVGG</a></li>
-        <li><a href="configs/vision_transformer">Vision-Transformer</a></li>
-        <li><a href="configs/tnt">Transformer-in-Transformer</a></li>
-        <li><a href="configs/res2net">Res2Net</a></li>
-        <li><a href="configs/mlp_mixer">MLP-Mixer</a></li>
-        <li><a href="configs/deit">DeiT</a></li>
-        <li><a href="configs/deit3">DeiT-3</a></li>
-        <li><a href="configs/conformer">Conformer</a></li>
-        <li><a href="configs/t2t_vit">T2T-ViT</a></li>
-        <li><a href="configs/twins">Twins</a></li>
-        <li><a href="configs/efficientnet">EfficientNet</a></li>
-        <li><a href="configs/edgenext">EdgeNeXt</a></li>
-        <li><a href="configs/convnext">ConvNeXt</a></li>
-        <li><a href="configs/hrnet">HRNet</a></li>
-        <li><a href="configs/van">VAN</a></li>
-        <li><a href="configs/convmixer">ConvMixer</a></li>
-        <li><a href="configs/cspnet">CSPNet</a></li>
-        <li><a href="configs/poolformer">PoolFormer</a></li>
-        <li><a href="configs/inception_v3">Inception V3</a></li>
-        <li><a href="configs/mobileone">MobileOne</a></li>
-        <li><a href="configs/efficientformer">EfficientFormer</a></li>
-        <li><a href="configs/mvit">MViT</a></li>
-        <li><a href="configs/hornet">HorNet</a></li>
-        <li><a href="configs/mobilevit">MobileViT</a></li>
-        <li><a href="configs/davit">DaViT</a></li>
-        <li><a href="configs/replknet">RepLKNet</a></li>
-        <li><a href="configs/beit">BEiT</a></li>
-        <li><a href="configs/mixmim">MixMIM</a></li>
-        <li><a href="configs/efficientnet_v2">EfficientNet V2</a></li>
-        <li><a href="configs/revvit">RevViT</a></li>
-        <li><a href="configs/convnext_v2">ConvNeXt V2</a></li>
-        <li><a href="configs/vig">ViG</a></li>
-        <li><a href="configs/xcit">XCiT</a></li>
-        <li><a href="configs/levit">LeViT</a></li>
-        <li><a href="configs/riformer">RIFormer</a></li>
-        </ul>
-      </td>
-      <td>
-        <ul>
-        <li><a href="configs/mocov2">MoCo V1 (CVPR'2020)</a></li>
-        <li><a href="configs/simclr">SimCLR (ICML'2020)</a></li>
-        <li><a href="configs/mocov2">MoCo V2 (arXiv'2020)</a></li>
-        <li><a href="configs/byol">BYOL (NeurIPS'2020)</a></li>
-        <li><a href="configs/swav">SwAV (NeurIPS'2020)</a></li>
-        <li><a href="configs/densecl">DenseCL (CVPR'2021)</a></li>
-        <li><a href="configs/simsiam">SimSiam (CVPR'2021)</a></li>
-        <li><a href="configs/barlowtwins">Barlow Twins (ICML'2021)</a></li>
-        <li><a href="configs/mocov3">MoCo V3 (ICCV'2021)</a></li>
-        <li><a href="configs/beit">BEiT (ICLR'2022)</a></li>
-        <li><a href="configs/mae">MAE (CVPR'2022)</a></li>
-        <li><a href="configs/simmim">SimMIM (CVPR'2022)</a></li>
-        <li><a href="configs/maskfeat">MaskFeat (CVPR'2022)</a></li>
-        <li><a href="configs/cae">CAE (arXiv'2022)</a></li>
-        <li><a href="configs/milan">MILAN (arXiv'2022)</a></li>
-        <li><a href="configs/beitv2">BEiT V2 (arXiv'2022)</a></li>
-        <li><a href="configs/eva">EVA (CVPR'2023)</a></li>
-        <li><a href="configs/mixmim">MixMIM (arXiv'2022)</a></li>
-        </ul>
-      </td>
-      <td>
-      Image Retrieval Task:
-        <ul>
-        <li><a href="configs/arcface">ArcFace (CVPR'2019)</a></li>
-        </ul>
-      Training&Test Tips:
-        <ul>
-        <li><a href="https://arxiv.org/abs/1909.13719">RandAug</a></li>
-        <li><a href="https://arxiv.org/abs/1805.09501">AutoAug</a></li>
-        <li><a href="mmpretrain/datasets/samplers/repeat_aug.py">RepeatAugSampler</a></li>
-        <li><a href="mmpretrain/models/tta/score_tta.py">TTA</a></li>
-        <li>...</li>
-        </ul>
-      </td>
-  </tbody>
-</table>
-
-## Contributing
-
-We appreciate all contributions to improve MMPreTrain.
-Please refer to [CONTRUBUTING](https://mmpretrain.readthedocs.io/en/latest/notes/contribution_guide.html) for the contributing guideline.
-
-## Acknowledgement
-
-MMPreTrain is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors who implement their methods or add new features, as well as users who give valuable feedbacks.
-We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and supporting their own academic research.
-
-## Citation
-
-If you find this project useful in your research, please consider cite:
-
-```BibTeX
-@misc{2023mmpretrain,
-    title={OpenMMLab's Pre-training Toolbox and Benchmark},
-    author={MMPreTrain Contributors},
-    howpublished = {\url{https://github.com/open-mmlab/mmpretrain}},
-    year={2023}
-}
-```
-
-## License
-
-This project is released under the [Apache 2.0 license](LICENSE).
-
-## Projects in OpenMMLab
-
-- [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
-- [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
-- [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
-- [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
-- [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
-- [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
-- [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
-- [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
-- [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
-- [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
-- [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
-- [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
-- [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
-- [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
-- [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
-- [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
-- [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
-- [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
-- [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-- [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing toolbox.
-- [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
-- [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+Metadata-Version: 2.1
+Name: mmpretrain
+Version: 1.0.0rc8
+Summary: OpenMMLab Model Pretraining Toolbox and Benchmark
+Home-page: https://github.com/open-mmlab/mmpretrain
+Author: MMPretrain Contributors
+Author-email: openmmlab@gmail.com
+License: Apache License 2.0
+Description: <div align="center">
+        
+        <img src="resources/mmpt-logo.png" width="600"/>
+          <div>&nbsp;</div>
+          <div align="center">
+            <b><font size="5">OpenMMLab website</font></b>
+            <sup>
+              <a href="https://openmmlab.com">
+                <i><font size="4">HOT</font></i>
+              </a>
+            </sup>
+            &nbsp;&nbsp;&nbsp;&nbsp;
+            <b><font size="5">OpenMMLab platform</font></b>
+            <sup>
+              <a href="https://platform.openmmlab.com">
+                <i><font size="4">TRY IT OUT</font></i>
+              </a>
+            </sup>
+          </div>
+          <div>&nbsp;</div>
+        
+        [![PyPI](https://img.shields.io/pypi/v/mmpretrain)](https://pypi.org/project/mmpretrain)
+        [![Docs](https://img.shields.io/badge/docs-latest-blue)](https://mmpretrain.readthedocs.io/en/latest/)
+        [![Build Status](https://github.com/open-mmlab/mmpretrain/workflows/build/badge.svg)](https://github.com/open-mmlab/mmpretrain/actions)
+        [![codecov](https://codecov.io/gh/open-mmlab/mmpretrain/branch/main/graph/badge.svg)](https://codecov.io/gh/open-mmlab/mmpretrain)
+        [![license](https://img.shields.io/github/license/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/blob/main/LICENSE)
+        [![open issues](https://isitmaintained.com/badge/open/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/issues)
+        [![issue resolution](https://isitmaintained.com/badge/resolution/open-mmlab/mmpretrain.svg)](https://github.com/open-mmlab/mmpretrain/issues)
+        
+        [📘 Documentation](https://mmpretrain.readthedocs.io/en/latest/) |
+        [🛠️ Installation](https://mmpretrain.readthedocs.io/en/latest/get_started.html#installation) |
+        [👀 Model Zoo](https://mmpretrain.readthedocs.io/en/latest/modelzoo_statistics.html) |
+        [🆕 Update News](https://mmpretrain.readthedocs.io/en/latest/notes/changelog.html) |
+        [🤔 Reporting Issues](https://github.com/open-mmlab/mmpretrain/issues/new/choose)
+        
+        <img src="https://user-images.githubusercontent.com/36138628/230307505-4727ad0a-7d71-4069-939d-b499c7e272b7.png" width="400"/>
+        
+        English | [简体中文](/README_zh-CN.md)
+        
+        </div>
+        
+        </div>
+        
+        <div align="center">
+          <a href="https://openmmlab.medium.com/" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219255827-67c1a27f-f8c5-46a9-811d-5e57448c61d1.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://discord.gg/raweFPmdzG" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/218347213-c080267f-cbb6-443e-8532-8e1ed9a58ea9.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://twitter.com/OpenMMLab" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/218346637-d30c8a0f-3eba-4699-8131-512fb06d46db.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://www.youtube.com/openmmlab" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/218346691-ceb2116a-465a-40af-8424-9f30d2348ca9.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://space.bilibili.com/1293512903" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219026751-d7d14cce-a7c9-4e82-9942-8375fca65b99.png" width="3%" alt="" /></a>
+          <img src="https://user-images.githubusercontent.com/25839884/218346358-56cc8e2f-a2b8-487f-9088-32480cceabcf.png" width="3%" alt="" />
+          <a href="https://www.zhihu.com/people/openmmlab" style="text-decoration:none;">
+            <img src="https://user-images.githubusercontent.com/25839884/219026120-ba71e48b-6e94-4bd4-b4e9-b7d175b5e362.png" width="3%" alt="" /></a>
+        </div>
+        
+        ## Introduction
+        
+        MMPreTrain is an open source pre-training toolbox based on PyTorch. It is a part of the [OpenMMLab](https://openmmlab.com/) project.
+        
+        The `main` branch works with **PyTorch 1.8+**.
+        
+        ### Major features
+        
+        - Various backbones and pretrained models
+        - Rich training strategies (supervised learning, self-supervised learning, multi-modality learning etc.)
+        - Bag of training tricks
+        - Large-scale training configs
+        - High efficiency and extensibility
+        - Powerful toolkits for model analysis and experiments
+        - Various out-of-box inference tasks.
+          - Image Classification
+          - Image Caption
+          - Visual Question Answering
+          - Visual Grounding
+          - Retrieval (Image-To-Image, Text-To-Image, Image-To-Text)
+        
+        https://github.com/open-mmlab/mmpretrain/assets/26739999/e4dcd3a2-f895-4d1b-a351-fbc74a04e904
+        
+        ## What's new
+        
+        🌟 v1.0.0rc8 was released in 22/05/2023
+        
+        - Support multiple **multi-modal** algorithms and inferencers. You can explore these features by the [gradio demo](https://github.com/open-mmlab/mmpretrain/tree/main/projects/gradio_demo)!
+        - Add EVA-02, Dino-V2, ViT-SAM and GLIP backbones.
+        - Register torchvision transforms into MMPretrain, you can now easily integrate torchvision's data augmentations in MMPretrain. See [the doc](https://mmpretrain.readthedocs.io/en/latest/api/data_process.html#torchvision-transforms)
+        
+        🌟 v1.0.0rc7 was released in 07/04/2023
+        
+        - Integrated Self-supervised learning algorithms from **MMSelfSup**, such as **MAE**, **BEiT**, etc.
+        - Support **RIFormer**, a simple but effective vision backbone by removing token mixer.
+        - Add t-SNE visualization.
+        - Refactor dataset pipeline visualization.
+        
+        Update of previous versions
+        
+        - Support **LeViT**, **XCiT**, **ViG**, **ConvNeXt-V2**, **EVA**, **RevViT**, **EfficientnetV2**, **CLIP**, **TinyViT** and **MixMIM** backbones.
+        - Reproduce the training accuracy of **ConvNeXt** and **RepVGG**.
+        - Support confusion matrix calculation and plot.
+        - Support **multi-task** training and testing.
+        - Support Test-time Augmentation.
+        - Upgrade API to get pre-defined models of MMPreTrain.
+        - Refactor BEiT backbone and support v1/v2 inference.
+        
+        This release introduced a brand new and flexible training & test engine, but it's still in progress. Welcome
+        to try according to [the documentation](https://mmpretrain.readthedocs.io/en/latest/).
+        
+        And there are some BC-breaking changes. Please check [the migration tutorial](https://mmpretrain.readthedocs.io/en/latest/migration.html).
+        
+        Please refer to [changelog](https://mmpretrain.readthedocs.io/en/latest/notes/changelog.html) for more details and other release history.
+        
+        ## Installation
+        
+        Below are quick steps for installation:
+        
+        ```shell
+        conda create -n open-mmlab python=3.8 pytorch==1.10.1 torchvision==0.11.2 cudatoolkit=11.3 -c pytorch -y
+        conda activate open-mmlab
+        pip install openmim
+        git clone https://github.com/open-mmlab/mmpretrain.git
+        cd mmpretrain
+        mim install -e .
+        ```
+        
+        Please refer to [installation documentation](https://mmpretrain.readthedocs.io/en/latest/get_started.html) for more detailed installation and dataset preparation.
+        
+        For multi-modality models support, please install the extra dependencies by:
+        
+        ```shell
+        mim install -e ".[multimodal]"
+        ```
+        
+        ## User Guides
+        
+        We provided a series of tutorials about the basic usage of MMPreTrain for new users:
+        
+        - [Learn about Configs](https://mmpretrain.readthedocs.io/en/latest/user_guides/config.html)
+        - [Prepare Dataset](https://mmpretrain.readthedocs.io/en/latest/user_guides/dataset_prepare.html)
+        - [Inference with existing models](https://mmpretrain.readthedocs.io/en/latest/user_guides/inference.html)
+        - [Train](https://mmpretrain.readthedocs.io/en/latest/user_guides/train.html)
+        - [Test](https://mmpretrain.readthedocs.io/en/latest/user_guides/test.html)
+        - [Downstream tasks](https://mmpretrain.readthedocs.io/en/latest/user_guides/downstream.html)
+        
+        For more information, please refer to [our documentation](https://mmpretrain.readthedocs.io/en/latest/).
+        
+        ## Model zoo
+        
+        Results and models are available in the [model zoo](https://mmpretrain.readthedocs.io/en/latest/modelzoo_statistics.html).
+        
+        <div align="center">
+          <b>Overview</b>
+        </div>
+        <table align="center">
+          <tbody>
+            <tr align="center" valign="bottom">
+              <td>
+                <b>Supported Backbones</b>
+              </td>
+              <td>
+                <b>Self-supervised Learning</b>
+              </td>
+              <td>
+                <b>Multi-Modality Algorithms</b>
+              </td>
+              <td>
+                <b>Others</b>
+              </td>
+            </tr>
+            <tr valign="top">
+              <td>
+                <ul>
+                <li><a href="configs/vgg">VGG</a></li>
+                <li><a href="configs/resnet">ResNet</a></li>
+                <li><a href="configs/resnext">ResNeXt</a></li>
+                <li><a href="configs/seresnet">SE-ResNet</a></li>
+                <li><a href="configs/seresnet">SE-ResNeXt</a></li>
+                <li><a href="configs/regnet">RegNet</a></li>
+                <li><a href="configs/shufflenet_v1">ShuffleNet V1</a></li>
+                <li><a href="configs/shufflenet_v2">ShuffleNet V2</a></li>
+                <li><a href="configs/mobilenet_v2">MobileNet V2</a></li>
+                <li><a href="configs/mobilenet_v3">MobileNet V3</a></li>
+                <li><a href="configs/swin_transformer">Swin-Transformer</a></li>
+                <li><a href="configs/swin_transformer_v2">Swin-Transformer V2</a></li>
+                <li><a href="configs/repvgg">RepVGG</a></li>
+                <li><a href="configs/vision_transformer">Vision-Transformer</a></li>
+                <li><a href="configs/tnt">Transformer-in-Transformer</a></li>
+                <li><a href="configs/res2net">Res2Net</a></li>
+                <li><a href="configs/mlp_mixer">MLP-Mixer</a></li>
+                <li><a href="configs/deit">DeiT</a></li>
+                <li><a href="configs/deit3">DeiT-3</a></li>
+                <li><a href="configs/conformer">Conformer</a></li>
+                <li><a href="configs/t2t_vit">T2T-ViT</a></li>
+                <li><a href="configs/twins">Twins</a></li>
+                <li><a href="configs/efficientnet">EfficientNet</a></li>
+                <li><a href="configs/edgenext">EdgeNeXt</a></li>
+                <li><a href="configs/convnext">ConvNeXt</a></li>
+                <li><a href="configs/hrnet">HRNet</a></li>
+                <li><a href="configs/van">VAN</a></li>
+                <li><a href="configs/convmixer">ConvMixer</a></li>
+                <li><a href="configs/cspnet">CSPNet</a></li>
+                <li><a href="configs/poolformer">PoolFormer</a></li>
+                <li><a href="configs/inception_v3">Inception V3</a></li>
+                <li><a href="configs/mobileone">MobileOne</a></li>
+                <li><a href="configs/efficientformer">EfficientFormer</a></li>
+                <li><a href="configs/mvit">MViT</a></li>
+                <li><a href="configs/hornet">HorNet</a></li>
+                <li><a href="configs/mobilevit">MobileViT</a></li>
+                <li><a href="configs/davit">DaViT</a></li>
+                <li><a href="configs/replknet">RepLKNet</a></li>
+                <li><a href="configs/beit">BEiT</a></li>
+                <li><a href="configs/mixmim">MixMIM</a></li>
+                <li><a href="configs/efficientnet_v2">EfficientNet V2</a></li>
+                <li><a href="configs/revvit">RevViT</a></li>
+                <li><a href="configs/convnext_v2">ConvNeXt V2</a></li>
+                <li><a href="configs/vig">ViG</a></li>
+                <li><a href="configs/xcit">XCiT</a></li>
+                <li><a href="configs/levit">LeViT</a></li>
+                <li><a href="configs/riformer">RIFormer</a></li>
+                <li><a href="configs/glip">GLIP</a></li>
+                </ul>
+              </td>
+              <td>
+                <ul>
+                <li><a href="configs/mocov2">MoCo V1 (CVPR'2020)</a></li>
+                <li><a href="configs/simclr">SimCLR (ICML'2020)</a></li>
+                <li><a href="configs/mocov2">MoCo V2 (arXiv'2020)</a></li>
+                <li><a href="configs/byol">BYOL (NeurIPS'2020)</a></li>
+                <li><a href="configs/swav">SwAV (NeurIPS'2020)</a></li>
+                <li><a href="configs/densecl">DenseCL (CVPR'2021)</a></li>
+                <li><a href="configs/simsiam">SimSiam (CVPR'2021)</a></li>
+                <li><a href="configs/barlowtwins">Barlow Twins (ICML'2021)</a></li>
+                <li><a href="configs/mocov3">MoCo V3 (ICCV'2021)</a></li>
+                <li><a href="configs/beit">BEiT (ICLR'2022)</a></li>
+                <li><a href="configs/mae">MAE (CVPR'2022)</a></li>
+                <li><a href="configs/simmim">SimMIM (CVPR'2022)</a></li>
+                <li><a href="configs/maskfeat">MaskFeat (CVPR'2022)</a></li>
+                <li><a href="configs/cae">CAE (arXiv'2022)</a></li>
+                <li><a href="configs/milan">MILAN (arXiv'2022)</a></li>
+                <li><a href="configs/beitv2">BEiT V2 (arXiv'2022)</a></li>
+                <li><a href="configs/eva">EVA (CVPR'2023)</a></li>
+                <li><a href="configs/mixmim">MixMIM (arXiv'2022)</a></li>
+                </ul>
+              </td>
+              <td>
+                <ul>
+                <li><a href="configs/blip">BLIP (arxiv'2022)</a></li>
+                <li><a href="configs/blip2">BLIP-2 (arxiv'2023)</a></li>
+                <li><a href="configs/ofa">OFA (CoRR'2022)</a></li>
+                <li><a href="configs/flamingo">Flamingo (NeurIPS'2022)</a></li>
+                <li><a href="configs/chinese_clip">Chinese CLIP (arxiv'2022)</a></li>
+                </ul>
+              </td>
+              <td>
+              Image Retrieval Task:
+                <ul>
+                <li><a href="configs/arcface">ArcFace (CVPR'2019)</a></li>
+                </ul>
+              Training&Test Tips:
+                <ul>
+                <li><a href="https://arxiv.org/abs/1909.13719">RandAug</a></li>
+                <li><a href="https://arxiv.org/abs/1805.09501">AutoAug</a></li>
+                <li><a href="mmpretrain/datasets/samplers/repeat_aug.py">RepeatAugSampler</a></li>
+                <li><a href="mmpretrain/models/tta/score_tta.py">TTA</a></li>
+                <li>...</li>
+                </ul>
+              </td>
+          </tbody>
+        </table>
+        
+        ## Contributing
+        
+        We appreciate all contributions to improve MMPreTrain.
+        Please refer to [CONTRUBUTING](https://mmpretrain.readthedocs.io/en/latest/notes/contribution_guide.html) for the contributing guideline.
+        
+        ## Acknowledgement
+        
+        MMPreTrain is an open source project that is contributed by researchers and engineers from various colleges and companies. We appreciate all the contributors who implement their methods or add new features, as well as users who give valuable feedbacks.
+        We wish that the toolbox and benchmark could serve the growing research community by providing a flexible toolkit to reimplement existing methods and supporting their own academic research.
+        
+        ## Citation
+        
+        If you find this project useful in your research, please consider cite:
+        
+        ```BibTeX
+        @misc{2023mmpretrain,
+            title={OpenMMLab's Pre-training Toolbox and Benchmark},
+            author={MMPreTrain Contributors},
+            howpublished = {\url{https://github.com/open-mmlab/mmpretrain}},
+            year={2023}
+        }
+        ```
+        
+        ## License
+        
+        This project is released under the [Apache 2.0 license](LICENSE).
+        
+        ## Projects in OpenMMLab
+        
+        - [MMEngine](https://github.com/open-mmlab/mmengine): OpenMMLab foundational library for training deep learning models.
+        - [MMCV](https://github.com/open-mmlab/mmcv): OpenMMLab foundational library for computer vision.
+        - [MIM](https://github.com/open-mmlab/mim): MIM installs OpenMMLab packages.
+        - [MMEval](https://github.com/open-mmlab/mmeval): A unified evaluation library for multiple machine learning libraries.
+        - [MMPreTrain](https://github.com/open-mmlab/mmpretrain): OpenMMLab pre-training toolbox and benchmark.
+        - [MMDetection](https://github.com/open-mmlab/mmdetection): OpenMMLab detection toolbox and benchmark.
+        - [MMDetection3D](https://github.com/open-mmlab/mmdetection3d): OpenMMLab's next-generation platform for general 3D object detection.
+        - [MMRotate](https://github.com/open-mmlab/mmrotate): OpenMMLab rotated object detection toolbox and benchmark.
+        - [MMYOLO](https://github.com/open-mmlab/mmyolo): OpenMMLab YOLO series toolbox and benchmark.
+        - [MMSegmentation](https://github.com/open-mmlab/mmsegmentation): OpenMMLab semantic segmentation toolbox and benchmark.
+        - [MMOCR](https://github.com/open-mmlab/mmocr): OpenMMLab text detection, recognition, and understanding toolbox.
+        - [MMPose](https://github.com/open-mmlab/mmpose): OpenMMLab pose estimation toolbox and benchmark.
+        - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
+        - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
+        - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
+        - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
+        - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
+        - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
+        - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
+        - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
+        - [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
+        - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+        - [Playground](https://github.com/open-mmlab/playground): A central hub for gathering and showcasing amazing projects built upon OpenMMLab.
+        
+Keywords: computer vision,image classification,unsupervised learning,self-supervised learning
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: tests
+Provides-Extra: optional
+Provides-Extra: mim
+Provides-Extra: multimodal
```

#### html2text {}

```diff
@@ -1,7 +1,11 @@
+Metadata-Version: 2.1 Name: mmpretrain Version: 1.0.0rc8 Summary: OpenMMLab
+Model Pretraining Toolbox and Benchmark Home-page: https://github.com/open-
+mmlab/mmpretrain Author: MMPretrain Contributors Author-email:
+openmmlab@gmail.com License: Apache License 2.0 Description:
                            [resources/mmpt-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
  [![PyPI](https://img.shields.io/pypi/v/mmpretrain)](https://pypi.org/project/
  mmpretrain) [![Docs](https://img.shields.io/badge/docs-latest-blue)](https://
 mmpretrain.readthedocs.io/en/latest/) [![Build Status](https://github.com/open-
@@ -22,18 +26,29 @@
  Issues](https://github.com/open-mmlab/mmpretrain/issues/new/choose) [https://
  user-images.githubusercontent.com/36138628/230307505-4727ad0a-7d71-4069-939d-
          b499c7e272b7.png] English | [ç®ä½ä¸­æ](/README_zh-CN.md)
 
 ## Introduction MMPreTrain is an open source pre-training toolbox based on
 PyTorch. It is a part of the [OpenMMLab](https://openmmlab.com/) project. The
 `main` branch works with **PyTorch 1.8+**. ### Major features - Various
-backbones and pretrained models - Rich training strategies(supervised learning,
-self-supervised learning, etc.) - Bag of training tricks - Large-scale training
-configs - High efficiency and extensibility - Powerful toolkits for model
-analysis and experiments ## What's new ð v1.0.0rc7 was released in 07/04/
+backbones and pretrained models - Rich training strategies (supervised
+learning, self-supervised learning, multi-modality learning etc.) - Bag of
+training tricks - Large-scale training configs - High efficiency and
+extensibility - Powerful toolkits for model analysis and experiments - Various
+out-of-box inference tasks. - Image Classification - Image Caption - Visual
+Question Answering - Visual Grounding - Retrieval (Image-To-Image, Text-To-
+Image, Image-To-Text) https://github.com/open-mmlab/mmpretrain/assets/26739999/
+e4dcd3a2-f895-4d1b-a351-fbc74a04e904 ## What's new ð v1.0.0rc8 was released
+in 22/05/2023 - Support multiple **multi-modal** algorithms and inferencers.
+You can explore these features by the [gradio demo](https://github.com/open-
+mmlab/mmpretrain/tree/main/projects/gradio_demo)! - Add EVA-02, Dino-V2, ViT-
+SAM and GLIP backbones. - Register torchvision transforms into MMPretrain, you
+can now easily integrate torchvision's data augmentations in MMPretrain. See
+[the doc](https://mmpretrain.readthedocs.io/en/latest/api/
+data_process.html#torchvision-transforms) ð v1.0.0rc7 was released in 07/04/
 2023 - Integrated Self-supervised learning algorithms from **MMSelfSup**, such
 as **MAE**, **BEiT**, etc. - Support **RIFormer**, a simple but effective
 vision backbone by removing token mixer. - Add t-SNE visualization. - Refactor
 dataset pipeline visualization. Update of previous versions - Support
 **LeViT**, **XCiT**, **ViG**, **ConvNeXt-V2**, **EVA**, **RevViT**,
 **EfficientnetV2**, **CLIP**, **TinyViT** and **MixMIM** backbones. - Reproduce
 the training accuracy of **ConvNeXt** and **RepVGG**. - Support confusion
@@ -48,62 +63,68 @@
 mmpretrain.readthedocs.io/en/latest/notes/changelog.html) for more details and
 other release history. ## Installation Below are quick steps for installation:
 ```shell conda create -n open-mmlab python=3.8 pytorch==1.10.1
 torchvision==0.11.2 cudatoolkit=11.3 -c pytorch -y conda activate open-mmlab
 pip install openmim git clone https://github.com/open-mmlab/mmpretrain.git cd
 mmpretrain mim install -e . ``` Please refer to [installation documentation]
 (https://mmpretrain.readthedocs.io/en/latest/get_started.html) for more
-detailed installation and dataset preparation. ## User Guides We provided a
-series of tutorials about the basic usage of MMPreTrain for new users: - [Learn
-about Configs](https://mmpretrain.readthedocs.io/en/latest/user_guides/
-config.html) - [Prepare Dataset](https://mmpretrain.readthedocs.io/en/latest/
-user_guides/dataset_prepare.html) - [Inference with existing models](https://
+detailed installation and dataset preparation. For multi-modality models
+support, please install the extra dependencies by: ```shell mim install -e ".
+[multimodal]" ``` ## User Guides We provided a series of tutorials about the
+basic usage of MMPreTrain for new users: - [Learn about Configs](https://
+mmpretrain.readthedocs.io/en/latest/user_guides/config.html) - [Prepare
+Dataset](https://mmpretrain.readthedocs.io/en/latest/user_guides/
+dataset_prepare.html) - [Inference with existing models](https://
 mmpretrain.readthedocs.io/en/latest/user_guides/inference.html) - [Train]
 (https://mmpretrain.readthedocs.io/en/latest/user_guides/train.html) - [Test]
 (https://mmpretrain.readthedocs.io/en/latest/user_guides/test.html) -
 [Downstream tasks](https://mmpretrain.readthedocs.io/en/latest/user_guides/
 downstream.html) For more information, please refer to [our documentation]
 (https://mmpretrain.readthedocs.io/en/latest/). ## Model zoo Results and models
 are available in the [model zoo](https://mmpretrain.readthedocs.io/en/latest/
 modelzoo_statistics.html).
                                    Overview
-    Supported Backbones    Self-supervised Learning                Others
-    * VGG                     * MoCo_V1_(CVPR'2020)  Image Retrieval Task:
-    * ResNet                  * SimCLR_(ICML'2020)       * ArcFace_(CVPR'2019)
-    * ResNeXt                 * MoCo_V2_(arXiv'2020) Training&Test Tips:
-    * SE-ResNet               * BYOL_(NeurIPS'2020)      * RandAug
-    * SE-ResNeXt              * SwAV_(NeurIPS'2020)      * AutoAug
-    * RegNet                  * DenseCL_(CVPR'2021)      * RepeatAugSampler
-    * ShuffleNet_V1           * SimSiam_(CVPR'2021)      * TTA
-    * ShuffleNet_V2           * Barlow_Twins_            * ...
-    * MobileNet_V2              (ICML'2021)
-    * MobileNet_V3            * MoCo_V3_(ICCV'2021)
-    * Swin-Transformer        * BEiT_(ICLR'2022)
-    * Swin-Transformer_V2     * MAE_(CVPR'2022)
-    * RepVGG                  * SimMIM_(CVPR'2022)
-    * Vision-Transformer      * MaskFeat_(CVPR'2022)
-    * Transformer-in-         * CAE_(arXiv'2022)
-      Transformer             * MILAN_(arXiv'2022)
-    * Res2Net                 * BEiT_V2_(arXiv'2022)
-    * MLP-Mixer               * EVA_(CVPR'2023)
-    * DeiT                    * MixMIM_(arXiv'2022)
-    * DeiT-3
-    * Conformer
-    * T2T-ViT
-    * Twins
-    * EfficientNet
-    * EdgeNeXt
-    * ConvNeXt
-    * HRNet
-    * VAN
-    * ConvMixer
-    * CSPNet
-    * PoolFormer
-    * Inception_V3
-    * MobileOne
+                         Self-supervised       Multi-Modality
+ Supported Backbones         Learning            Algorithms                 Others
+    * VGG                 * MoCo_V1_           * BLIP_          Image Retrieval Task:
+    * ResNet                (CVPR'2020)          (arxiv'2022)       * ArcFace_
+    * ResNeXt             * SimCLR_            * BLIP-2_              (CVPR'2019)
+    * SE-ResNet             (ICML'2020)          (arxiv'2023)   Training&Test Tips:
+    * SE-ResNeXt          * MoCo_V2_           * OFA_               * RandAug
+    * RegNet                (arXiv'2020)         (CoRR'2022)        * AutoAug
+    * ShuffleNet_V1       * BYOL_              * Flamingo_          * RepeatAugSampler
+    * ShuffleNet_V2         (NeurIPS'2020)       (NeurIPS'2022)     * TTA
+    * MobileNet_V2        * SwAV_              * Chinese_CLIP_      * ...
+    * MobileNet_V3          (NeurIPS'2020)       (arxiv'2022)
+    * Swin-               * DenseCL_
+      Transformer           (CVPR'2021)
+    * Swin-               * SimSiam_
+      Transformer_V2        (CVPR'2021)
+    * RepVGG              * Barlow_Twins_
+    * Vision-               (ICML'2021)
+      Transformer         * MoCo_V3_
+    * Transformer-in-       (ICCV'2021)
+      Transformer         * BEiT_
+    * Res2Net               (ICLR'2022)
+    * MLP-Mixer           * MAE_
+    * DeiT                  (CVPR'2022)
+    * DeiT-3              * SimMIM_
+    * Conformer             (CVPR'2022)
+    * T2T-ViT             * MaskFeat_
+    * Twins                 (CVPR'2022)
+    * EfficientNet        * CAE_
+    * EdgeNeXt              (arXiv'2022)
+    * ConvNeXt            * MILAN_
+    * HRNet                 (arXiv'2022)
+    * VAN                 * BEiT_V2_
+    * ConvMixer             (arXiv'2022)
+    * CSPNet              * EVA_
+    * PoolFormer            (CVPR'2023)
+    * Inception_V3        * MixMIM_
+    * MobileOne             (arXiv'2022)
     * EfficientFormer
     * MViT
     * HorNet
     * MobileViT
     * DaViT
     * RepLKNet
     * BEiT
@@ -111,14 +132,15 @@
     * EfficientNet_V2
     * RevViT
     * ConvNeXt_V2
     * ViG
     * XCiT
     * LeViT
     * RIFormer
+    * GLIP
 ## Contributing We appreciate all contributions to improve MMPreTrain. Please
 refer to [CONTRUBUTING](https://mmpretrain.readthedocs.io/en/latest/notes/
 contribution_guide.html) for the contributing guideline. ## Acknowledgement
 MMPreTrain is an open source project that is contributed by researchers and
 engineers from various colleges and companies. We appreciate all the
 contributors who implement their methods or add new features, as well as users
 who give valuable feedbacks. We wish that the toolbox and benchmark could serve
@@ -151,12 +173,25 @@
 OpenMMLab self-supervised learning toolbox and benchmark. - [MMRazor](https://
 github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and
 benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab
 fewshot learning toolbox and benchmark. - [MMAction2](https://github.com/open-
 mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and
 benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
 video perception toolbox and benchmark. - [MMFlow](https://github.com/open-
-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMEditing]
-(https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing
-toolbox. - [MMGeneration](https://github.com/open-mmlab/mmgeneration):
-OpenMMLab image and video generative models toolbox. - [MMDeploy](https://
-github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMagic](https:/
+/github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and
+**I**ntelligent **C**reation toolbox. - [MMGeneration](https://github.com/open-
+mmlab/mmgeneration): OpenMMLab image and video generative models toolbox. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. - [Playground](https://github.com/open-mmlab/playground): A central
+hub for gathering and showcasing amazing projects built upon OpenMMLab.
+Keywords: computer vision,image classification,unsupervised learning,self-
+supervised learning Platform: UNKNOWN Classifier: Development Status :: 4 -
+Beta Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Requires-Python: >=3.7 Description-Content-Type: text/
+markdown Provides-Extra: all Provides-Extra: tests Provides-Extra: optional
+Provides-Extra: mim Provides-Extra: multimodal
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/cifar100_bs16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/cifar100_bs16.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 ]
 
 train_dataloader = dict(
     batch_size=16,
     num_workers=2,
     dataset=dict(
         type=dataset_type,
-        data_prefix='data/cifar100',
-        test_mode=False,
+        data_root='data/cifar100',
+        split='train',
         pipeline=train_pipeline),
     sampler=dict(type='DefaultSampler', shuffle=True),
 )
 
 val_dataloader = dict(
     batch_size=16,
     num_workers=2,
     dataset=dict(
         type=dataset_type,
-        data_prefix='data/cifar100/',
-        test_mode=True,
+        data_root='data/cifar100/',
+        split='test',
         pipeline=test_pipeline),
     sampler=dict(type='DefaultSampler', shuffle=False),
 )
 val_evaluator = dict(type='Accuracy', topk=(1, ))
 
 test_dataloader = val_dataloader
 test_evaluator = val_evaluator
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/cifar10_bs16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/cifar10_bs16.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 ]
 
 train_dataloader = dict(
     batch_size=16,
     num_workers=2,
     dataset=dict(
         type=dataset_type,
-        data_prefix='data/cifar10',
-        test_mode=False,
+        data_root='data/cifar10',
+        split='train',
         pipeline=train_pipeline),
     sampler=dict(type='DefaultSampler', shuffle=True),
 )
 
 val_dataloader = dict(
     batch_size=16,
     num_workers=2,
     dataset=dict(
         type=dataset_type,
-        data_prefix='data/cifar10/',
-        test_mode=True,
+        data_root='data/cifar10/',
+        split='test',
         pipeline=test_pipeline),
     sampler=dict(type='DefaultSampler', shuffle=False),
 )
 val_evaluator = dict(type='Accuracy', topk=(1, ))
 
 test_dataloader = val_dataloader
 test_evaluator = val_evaluator
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/cub_bs8_384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/cub_bs8_448.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 # dataset settings
 dataset_type = 'CUB'
 data_preprocessor = dict(
     num_classes=200,
-    # RGB format normalization parameters
     mean=[123.675, 116.28, 103.53],
     std=[58.395, 57.12, 57.375],
     # convert image from BGR to RGB
     to_rgb=True,
 )
 
 train_pipeline = [
     dict(type='LoadImageFromFile'),
-    dict(type='Resize', scale=510),
-    dict(type='RandomCrop', crop_size=384),
+    dict(type='Resize', scale=600),
+    dict(type='RandomCrop', crop_size=448),
     dict(type='RandomFlip', prob=0.5, direction='horizontal'),
     dict(type='PackInputs'),
 ]
 
 test_pipeline = [
     dict(type='LoadImageFromFile'),
-    dict(type='Resize', scale=510),
-    dict(type='CenterCrop', crop_size=384),
+    dict(type='Resize', scale=600),
+    dict(type='CenterCrop', crop_size=448),
     dict(type='PackInputs'),
 ]
 
 train_dataloader = dict(
     batch_size=8,
     num_workers=2,
     dataset=dict(
         type=dataset_type,
         data_root='data/CUB_200_2011',
-        test_mode=False,
+        split='train',
         pipeline=train_pipeline),
     sampler=dict(type='DefaultSampler', shuffle=True),
 )
 
 val_dataloader = dict(
     batch_size=8,
     num_workers=2,
     dataset=dict(
         type=dataset_type,
         data_root='data/CUB_200_2011',
-        test_mode=True,
+        split='test',
         pipeline=test_pipeline),
     sampler=dict(type='DefaultSampler', shuffle=False),
 )
 val_evaluator = dict(type='Accuracy', topk=(1, ))
 
 test_dataloader = val_dataloader
 test_evaluator = val_evaluator
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/cub_bs8_448.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/cub_bs8_384.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 # dataset settings
 dataset_type = 'CUB'
 data_preprocessor = dict(
     num_classes=200,
+    # RGB format normalization parameters
     mean=[123.675, 116.28, 103.53],
     std=[58.395, 57.12, 57.375],
     # convert image from BGR to RGB
     to_rgb=True,
 )
 
 train_pipeline = [
     dict(type='LoadImageFromFile'),
-    dict(type='Resize', scale=600),
-    dict(type='RandomCrop', crop_size=448),
+    dict(type='Resize', scale=510),
+    dict(type='RandomCrop', crop_size=384),
     dict(type='RandomFlip', prob=0.5, direction='horizontal'),
     dict(type='PackInputs'),
 ]
 
 test_pipeline = [
     dict(type='LoadImageFromFile'),
-    dict(type='Resize', scale=600),
-    dict(type='CenterCrop', crop_size=448),
+    dict(type='Resize', scale=510),
+    dict(type='CenterCrop', crop_size=384),
     dict(type='PackInputs'),
 ]
 
 train_dataloader = dict(
     batch_size=8,
     num_workers=2,
     dataset=dict(
         type=dataset_type,
         data_root='data/CUB_200_2011',
-        test_mode=False,
+        split='train',
         pipeline=train_pipeline),
     sampler=dict(type='DefaultSampler', shuffle=True),
 )
 
 val_dataloader = dict(
     batch_size=8,
     num_workers=2,
     dataset=dict(
         type=dataset_type,
         data_root='data/CUB_200_2011',
-        test_mode=True,
+        split='test',
         pipeline=test_pipeline),
     sampler=dict(type='DefaultSampler', shuffle=False),
 )
 val_evaluator = dict(type='Accuracy', topk=(1, ))
 
 test_dataloader = val_dataloader
 test_evaluator = val_evaluator
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet21k_bs128.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet21k_bs128.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_mbv3.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_mbv3.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_medium_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_medium_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_small_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_small_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_revvit_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_revvit_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_medium_384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_medium_384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_small_384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_small_384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_vig_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_vig_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_196.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_196.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_336.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_336.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_560.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_560.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_pil_bicubic_384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_pil_bicubic_384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_beitv2.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_beitv2.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_davit_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_davit_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_levit_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_levit_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a12.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a12.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a3.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a3.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_simmim_192.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_simmim_192.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_swin_192.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_swin_192.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_byol.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_byol.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_mocov2.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_mocov2.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_pil_bicubic.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_pil_bicubic.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_pil_resize.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_pil_resize.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_simclr.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs32_simclr.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs512_mae.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs512_mae.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs512_mocov3.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs512_mocov3.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_autoaug.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_autoaug.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_448.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_clip_448.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_convmixer_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_convmixer_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_deit3_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_deit3_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_deit3_384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_deit3_384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_edgenext_256.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_edgenext_256.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_mixer_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_mixer_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_pil_resize.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_pil_resize.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_pil_resize_autoaug.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_pil_resize_autoaug.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_256.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_256.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_t2t_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_t2t_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs8_pil_bicubic_320.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/imagenet_bs8_pil_bicubic_320.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/inshop_bs32_448.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/inshop_bs32_448.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/pipelines/auto_aug.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/pipelines/auto_aug.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/pipelines/rand_aug.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/pipelines/rand_aug.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/datasets/voc_bs16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/datasets/voc_bs16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/default_runtime.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/default_runtime.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/conformer/base-p16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/conformer/base-p16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/conformer/small-p16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/conformer/small-p16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/conformer/small-p32.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/conformer/small-p32.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/conformer/tiny-p16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/conformer/tiny-p16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-large.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-large.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-small.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-small.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-tiny.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-tiny.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext/convnext-xlarge.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext/convnext-xlarge.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/huge.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/huge.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/large.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/large.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/convnext_v2/tiny.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/convnext_v2/tiny.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-base-p16-224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-base-p16-224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-base-p16-384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-base-p16-384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-huge-p14-224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-huge-p14-224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-large-p16-224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-large-p16-224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-large-p16-384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-large-p16-384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-medium-p16-224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-medium-p16-224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-small-p16-224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-small-p16-224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/deit3/deit3-small-p16-384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/deit3/deit3-small-p16-384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-small.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-small.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-xsmall.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-xsmall.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-xxsmall.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/edgenext/edgenext-xxsmall.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/efficientformer-l1.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/efficientformer-l1.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/eva/eva-g.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/eva/eva-g.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/eva/eva-l.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/eva/eva-l.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-base-gf.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-base-gf.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large-gf.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large-gf.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large-gf384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large-gf384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-large.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-small-gf.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-small-gf.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-small.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-small.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-tiny-gf.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-tiny-gf.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/hornet/hornet-tiny.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/hornet/hornet-tiny.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/levit-256-p16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/levit-256-p16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mae_vit-base-p16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mae_vit-base-p16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mixmim/mixmim_base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mixmim/mixmim_base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mlp_mixer_base_patch16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mlp_mixer_base_patch16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mlp_mixer_large_patch16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mlp_mixer_large_patch16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_large_imagenet.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_large_imagenet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_050_imagenet.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_050_imagenet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_075_imagenet.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_075_imagenet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_imagenet.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mobilenet_v3/mobilenet_v3_small_imagenet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-large.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-large.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-small.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-small.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-tiny.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/mvit/mvitv2-tiny.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_m36.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_m36.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_m48.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_m48.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s12.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s12.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s24.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s24.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s36.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/poolformer/poolformer_s36.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/replknet-31B_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/replknet-31B_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/repvgg-B3_lbs-mixup_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/repvgg-B3_lbs-mixup_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnest101.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnest101.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnest200.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnest200.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnest269.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnest269.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnest50.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnest50.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet50_cifar_cutmix.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet50_cifar_cutmix.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/resnet50_cutmix.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/resnet50_cutmix.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/revvit/revvit-base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/revvit/revvit-base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/revvit/revvit-small.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/revvit/revvit-small.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/base_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/base_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/small_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/small_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer/tiny_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer/tiny_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/base_256.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/base_256.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/base_384.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/base_384.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/small_256.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/small_256.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/tiny_256.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/swin_transformer_v2/tiny_256.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-14.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-14.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-19.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-19.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-24.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/t2t-vit-t-24.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-11m.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-11m.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-21m.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-21m.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-5m.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/tinyvit/tinyvit-5m.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/tnt_s_patch16_224.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/tnt_s_patch16_224.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/twins_pcpvt_base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/twins_pcpvt_base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/twins_svt_base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/twins_svt_base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/van/van_small.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/van/van_small.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/van/van_tiny.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/van/van_tiny.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_medium.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_medium.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_small.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_small.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_tiny.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/pyramid_vig_tiny.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/vig_base.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/vig_base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/vig_small.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/vig_small.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vig/vig_tiny.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vig/vig_tiny.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vit-base-p16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vit-base-p16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vit-base-p32.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vit-base-p32.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vit-large-p16.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vit-large-p16.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/models/vit-large-p32.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/models/vit-large-p32.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/cub_bs64.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/cub_bs64.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_conformer.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_conformer.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_revvit.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_revvit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_swin.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_adamw_swin.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_coslr.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_coslr.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_linearlr_bn_nowd.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs1024_linearlr_bn_nowd.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_AdamW.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_AdamW.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_adamw_levit.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_adamw_levit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_coslr.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_coslr.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_rsb.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs2048_rsb.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_200e_coslr_warmup.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_200e_coslr_warmup.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_coslr_coswd_300e.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs256_coslr_coswd_300e.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs4096_AdamW.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_bs4096_AdamW.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/_base_/schedules/imagenet_lars_coslr_200e.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/_base_/schedules/imagenet_lars_coslr_200e.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/arcface/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/arcface/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/arcface/resnet50-arcface_8xb32_inshop.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/arcface/resnet50-arcface_8xb32_inshop.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/barlowtwins/barlowtwins_resnet50_8xb256-coslr-1000e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/barlowtwins/barlowtwins_resnet50_8xb256-coslr-1000e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/barlowtwins/barlowtwins_resnet50_8xb256-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/barlowtwins/barlowtwins_resnet50_8xb256-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/barlowtwins/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/barlowtwins/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/beit_beit-base-p16_8xb256-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/beit_beit-base-p16_8xb256-amp-coslr-300e_in1k.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     type='BEiT',
     backbone=dict(
         type='BEiTPretrainViT',
         arch='base',
         patch_size=16,
         drop_path_rate=0.1,
         final_norm=True,
+        out_type='raw',
         layer_scale_init_value=0.1,
         init_cfg=[
             dict(type='TruncNormal', std=0.02, layer='Linear'),
             dict(type='TruncNormal', std=0.02, layer='Conv2d'),
             dict(type='Constant', layer='LayerNorm', val=1.0, bias=0.0)
         ]),
     neck=None,
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-1600e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-1600e_in1k.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     backbone=dict(
         type='BEiTPretrainViT',
         arch='base',
         patch_size=16,
         out_indices=[-4, -1],
         drop_path_rate=drop_path_rate,
         final_norm=False,
+        out_type='raw',
         layer_scale_init_value=layer_scale_init_value,
         init_cfg=[
             dict(type='TruncNormal', std=0.02, layer='Linear'),
             dict(type='TruncNormal', std=0.02, layer='Conv2d'),
             dict(type='Constant', layer='LayerNorm', val=1.0, bias=0.0)
         ]),
     neck=dict(
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-300e_in1k.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     backbone=dict(
         type='BEiTPretrainViT',
         arch='base',
         patch_size=16,
         out_indices=[-4, -1],
         drop_path_rate=drop_path_rate,
         final_norm=False,
+        out_type='raw',
         layer_scale_init_value=layer_scale_init_value,
         init_cfg=[
             dict(type='TruncNormal', std=0.02, layer='Linear'),
             dict(type='TruncNormal', std=0.02, layer='Conv2d'),
             dict(type='Constant', layer='LayerNorm', val=1.0, bias=0.0)
         ]),
     neck=dict(
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/beitv2/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/beitv2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50-c4_ms-1x_coco.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50-c4_ms-1x_coco.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50_fpn_ms-1x_coco.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50_fpn_ms-1x_coco.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/byol_resnet50_16xb256-coslr-200e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/byol_resnet50_16xb256-coslr-200e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/byol/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/byol/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cae/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cae/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cae/cae_beit-base-p16_8xb256-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cae/cae_beit-base-p16_8xb256-amp-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cae/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cae/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/metafile.yml`

 * *Files 5% similar despite different names*

```diff
@@ -290,7 +290,19 @@
           Top 5 Accuracy: 98.02
         Task: Image Classification
     Weights: https://download.openmmlab.com/mmclassification/v0/clip/clip-vit-base-p16_laion2b-in12k-pre_3rdparty_in1k-384px_20221220-84ed0cc0.pth
     Config: configs/clip/vit-base-p16_pt-64xb64_in1k-384px.py
     Converted From:
       Code: https://github.com/rwightman/pytorch-image-models
       Weights: https://huggingface.co/timm/vit_base_patch16_clip_384.laion2b_ft_in12k_in1k
+  - Name: vit-large-p14_clip-openai-pre_3rdparty
+    Metadata:
+      FLOPs: 59696580608
+      Parameters: 303302656
+      Training Data:
+        - OpenAI
+    In Collection: CLIP
+    Weights: https://download.openmmlab.com/mmclassification/v0/clip/vit-large-p14_clip-openai-pre_3rdparty_20230517-95e2af0b.pth
+    Config: configs/clip/vit-large-p14_headless.py
+    Converted From:
+      Code: https://github.com/mlfoundations/open_clip
+      Weights: https://openaipublic.azureedge.net/clip/models/b8cca3fd41ae0c99ba7e8951adf17d267cdb84cd88be6f7c2e0eca1737a03836/ViT-L-14.pt
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-448px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-448px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-448px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-448px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/conformer/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/conformer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convmixer/convmixer-1024-20_10xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convmixer/convmixer-1024-20_10xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convmixer/convmixer-1536-20_10xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convmixer/convmixer-1536-20_10xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convmixer/convmixer-768-32_10xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convmixer/convmixer-768-32_10xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convmixer/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convmixer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in21k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-base_32xb128_in21k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in21k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-large_64xb64_in21k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-small_32xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-small_32xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-small_32xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-small_32xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-tiny_32xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-tiny_32xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-tiny_32xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-tiny_32xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in21k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/convnext-xlarge_64xb64_in21k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-atto_32xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-atto_32xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-base_32xb32_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-base_32xb32_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-base_32xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-base_32xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-femto_32xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-femto_32xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k-512px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k-512px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-huge_32xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-large_32xb32_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-large_32xb32_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-large_32xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-large_32xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-nano_32xb32_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-nano_32xb32_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-nano_32xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-nano_32xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-pico_32xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-pico_32xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-tiny_32xb32_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-tiny_32xb32_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/convnext-v2-tiny_32xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/convnext-v2-tiny_32xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/convnext_v2/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/convnext_v2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cspnet/cspdarknet50_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cspnet/cspdarknet50_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cspnet/cspresnet50_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cspnet/cspresnet50_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cspnet/cspresnext50_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cspnet/cspresnext50_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/cspnet/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/cspnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/csra/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/csra/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/csra/resnet101-csra_1xb16_voc07-448px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/csra/resnet101-csra_1xb16_voc07-448px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/davit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/davit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-base-distilled_16xb32_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-base-distilled_16xb32_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-base-distilled_16xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-base-distilled_16xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-base_16xb32_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-base_16xb32_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-base_16xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-base_16xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-small-distilled_4xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-small-distilled_4xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-small_4xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-small_4xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-tiny-distilled_4xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-tiny-distilled_4xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/deit-tiny_4xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/deit-tiny_4xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-base-p16_64xb32_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-base-p16_64xb32_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-base-p16_64xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-base-p16_64xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-huge-p14_64xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-huge-p14_64xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-large-p16_64xb16_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-large-p16_64xb16_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-large-p16_64xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-large-p16_64xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-medium-p16_64xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-medium-p16_64xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-small-p16_64xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-small-p16_64xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/deit3-small-p16_64xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/deit3-small-p16_64xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/deit3/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/deit3/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densecl/densecl_resnet50_8xb32-coslr-200e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densecl/densecl_resnet50_8xb32-coslr-200e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densecl/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densecl/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/densenet/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/densenet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-base_8xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-base_8xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-small_8xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-small_8xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-xsmall_8xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-xsmall_8xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/edgenext-xxsmall_8xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/edgenext-xxsmall_8xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/edgenext/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/edgenext/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientformer/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientformer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b0_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b0_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b0_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b0_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b1_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b1_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b1_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b1_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b2_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b2_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b2_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b2_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b3_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b3_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b3_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b3_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b4_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b4_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b4_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b4_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b5_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b5_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b5_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b5_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b6_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b6_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b6_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b6_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b7_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b7_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b7_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b7_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b8_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b8_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-b8_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-b8_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-em_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-em_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-es_8xb32-01norm_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-es_8xb32-01norm_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-l2_8xb32_in1k-475px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-l2_8xb32_in1k-475px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/efficientnet-l2_8xb8_in1k-800px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/efficientnet-l2_8xb8_in1k-800px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b0_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b0_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b1_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b1_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b2_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b2_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b3_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-b3_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-l_8xb32_in1k-480px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-l_8xb32_in1k-480px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-m_8xb32_in1k-480px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-m_8xb32_in1k-480px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-s_8xb32_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-s_8xb32_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-s_8xb32_in21k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-s_8xb32_in21k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-xl_8xb32_in1k-512px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/efficientnetv2-xl_8xb32_in1k-512px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/efficientnet_v2/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/efficientnet_v2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb2048-linear-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb2048-linear-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-g-p14_headless.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-g-p14_headless.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-g-p16_headless.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-g-p16_headless.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-l-p14_headless.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-l-p14_headless.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/eva-mae-style_vit-base-p16_16xb256-coslr-400e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/eva-mae-style_vit-base-p16_16xb256-coslr-400e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/eva/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/eva/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hornet/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hornet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/hrnet/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/hrnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/inception_v3/inception-v3_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/inception_v3/inception-v3_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/inception_v3/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/inception_v3/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/lenet/lenet5_mnist.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/lenet/lenet5_mnist.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/levit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/levit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-base-p16_8xb2048-linear-coslr-90e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-base-p16_8xb2048-linear-coslr-90e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-huge-p14_32xb8-coslr-50e_in1k-448px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-huge-p14_32xb8-coslr-50e_in1k-448px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-huge-p14_8xb128-coslr-50e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-huge-p14_8xb128-coslr-50e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-large-p16_8xb128-coslr-50e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-large-p16_8xb128-coslr-50e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/benchmarks/vit-large-p16_8xb2048-linear-coslr-90e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/benchmarks/vit-large-p16_8xb2048-linear-coslr-90e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-1600e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-1600e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-400e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-400e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-800e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-base-p16_8xb512-amp-coslr-800e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-huge-p14_8xb512-amp-coslr-1600e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-huge-p14_8xb512-amp-coslr-1600e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-1600e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-1600e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-400e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-400e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-800e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/mae_vit-large-p16_8xb512-amp-coslr-800e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mae/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mae/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/maskfeat/benchmarks/vit-base-p16_8xb256-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/maskfeat/benchmarks/vit-base-p16_8xb256-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/maskfeat/maskfeat_vit-base-p16_8xb256-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/maskfeat/maskfeat_vit-base-p16_8xb256-amp-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/maskfeat/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/maskfeat/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/benchmarks/vit-base-p16_8xb2048-linear-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/benchmarks/vit-base-p16_8xb2048-linear-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/milan/milan_vit-base-p16_16xb256-amp-coslr-400e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/milan/milan_vit-base-p16_16xb256-amp-coslr-400e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mixmim/benchmarks/mixmim-base_8xb128-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mixmim/benchmarks/mixmim-base_8xb128-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mixmim/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mixmim/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mixmim/mixmim_mixmim-base_16xb128-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mixmim/mixmim_mixmim-base_16xb128-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mlp_mixer/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mlp_mixer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v2/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-large_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-large_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small-050_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small-050_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small-075_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small-075_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilenet_v3/mobilenet-v3-small_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s0_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s0_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s1_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s1_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s2_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s2_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s3_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s3_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobileone/mobileone-s4_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobileone/mobileone-s4_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilevit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilevit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilevit/mobilevit-small_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilevit/mobilevit-small_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilevit/mobilevit-xsmall_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilevit/mobilevit-xsmall_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mobilevit/mobilevit-xxsmall_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mobilevit/mobilevit-xxsmall_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov2/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov2/mocov2_resnet50_8xb32-coslr-200e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov2/mocov2_resnet50_8xb32-coslr-200e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/resnet50_8xb128-linear-coslr-90e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/resnet50_8xb128-linear-coslr-90e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/vit-base-p16_8xb128-linear-coslr-90e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/vit-base-p16_8xb128-linear-coslr-90e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/vit-base-p16_8xb64-coslr-150e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/vit-base-p16_8xb64-coslr-150e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/vit-large-p16_8xb64-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/vit-large-p16_8xb64-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/benchmarks/vit-small-p16_8xb128-linear-coslr-90e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/benchmarks/vit-small-p16_8xb128-linear-coslr-90e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-800e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_resnet50_8xb512-amp-coslr-800e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_vit-base-p16_16xb256-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_vit-base-p16_16xb256-amp-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_vit-large-p16_64xb64-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_vit-large-p16_64xb64-amp-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mocov3/mocov3_vit-small-p16_16xb256-amp-coslr-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mocov3/mocov3_vit-small-p16_16xb256-amp-coslr-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/mvitv2-base_8xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/mvitv2-base_8xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/mvitv2-large_8xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/mvitv2-large_8xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/mvitv2-small_8xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/mvitv2-small_8xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/mvit/mvitv2-tiny_8xb256_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/mvit/mvitv2-tiny_8xb256_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-m36_32xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-m36_32xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-m48_32xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-m48_32xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-s12_32xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-s12_32xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-s24_32xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-s24_32xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/poolformer/poolformer-s36_32xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/poolformer/poolformer-s36_32xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-12gf_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-12gf_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-3.2gf_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-3.2gf_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-4.0gf_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-4.0gf_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-400mf_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-400mf_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-6.4gf_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-6.4gf_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/regnet/regnetx-8.0gf_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/regnet/regnetx-8.0gf_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/replknet/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/replknet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repmlp/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repmlp/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repmlp/repmlp-base_8xb64_in1k-256px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repmlp/repmlp-base_8xb64_in1k-256px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repmlp/repmlp-base_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repmlp/repmlp-base_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-A0_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-A0_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-B3_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-B3_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/repvgg/repvgg-D2se_8xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/repvgg/repvgg-D2se_8xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/res2net/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/res2net/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/_randaug_policies.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/_randaug_policies.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/resnest101_32xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/resnest101_32xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/resnest200_64xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/resnest200_64xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/resnest269_64xb32_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/resnest269_64xb32_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnest/resnest50_32xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnest/resnest50_32xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a1-600e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a1-600e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a2-300e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a2-300e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a3-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb256-rsb-a3-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnet/resnet50_8xb8_cub.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnet/resnet50_8xb8_cub.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/resnext/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/resnext/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/revvit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/revvit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-m36_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-m36_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-m36_8xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-m36_8xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-m48_8xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-m48_8xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-m48_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-m48_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s12_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s12_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s12_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s12_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s24_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s24_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s24_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s24_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s36_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s36_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/riformer/riformer-s36_8xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/riformer/riformer-s36_8xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/seresnet/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/seresnet/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/shufflenet_v1/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/shufflenet_v1/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/shufflenet_v2/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/shufflenet_v2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/simclr_resnet50_16xb256-coslr-200e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/simclr_resnet50_16xb256-coslr-200e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/simclr_resnet50_16xb256-coslr-800e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/simclr_resnet50_16xb256-coslr-800e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simclr/simclr_resnet50_8xb32-coslr-200e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simclr/simclr_resnet50_8xb32-coslr-200e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/benchmarks/swin-base-w6_8xb256-coslr-100e_in1k-192px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/benchmarks/swin-base-w6_8xb256-coslr-100e_in1k-192px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/benchmarks/swin-base-w7_8xb256-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/benchmarks/swin-base-w7_8xb256-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/benchmarks/swin-large-w14_8xb256-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/benchmarks/swin-large-w14_8xb256-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_16xb128-amp-coslr-800e_in1k-192px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_16xb128-amp-coslr-800e_in1k-192px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_8xb256-amp-coslr-100e_in1k-192px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/simmim_swin-base-w6_8xb256-amp-coslr-100e_in1k-192px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simmim/simmim_swin-large-w12_16xb128-amp-coslr-800e_in1k-192px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simmim/simmim_swin-large-w12_16xb128-amp-coslr-800e_in1k-192px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simsiam/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simsiam/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simsiam/simsiam_resnet50_8xb32-coslr-100e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simsiam/simsiam_resnet50_8xb32-coslr-100e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/simsiam/simsiam_resnet50_8xb32-coslr-200e_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/simsiam/simsiam_resnet50_8xb32-coslr-200e_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swav/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swav/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swav/swav_resnet50_8xb32-mcrop-coslr-200e_in1k-224px-96px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swav/swav_resnet50_8xb32-mcrop-coslr-200e_in1k-224px-96px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer/swin-large_8xb8_cub-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer/swin-large_8xb8_cub-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w12_8xb128_in21k-192px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-base-w12_8xb128_in21k-192px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-large-w12_8xb128_in21k-192px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/swin_transformer_v2/swinv2-large-w12_8xb128_in21k-192px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/t2t_vit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/t2t_vit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-14_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-14_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-19_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-19_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-24_8xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/t2t_vit/t2t-vit-t-24_8xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k-512px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tinyvit/tinyvit-21m-distill_8xb256_in1k-512px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tnt/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tnt/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/tnt/tnt-s-p16_16xb64_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/tnt/tnt-s-p16_16xb64_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/twins-pcpvt-base_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/twins-pcpvt-base_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/twins/twins-svt-base_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/twins/twins-svt-base_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/van-base_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/van-base_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/van-large_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/van-large_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/van-small_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/van-small_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/van/van-tiny_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/van/van-tiny_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vgg/vgg16_8xb16_voc.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vgg/vgg16_8xb16_voc.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vig/pvig-base_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vig/pvig-base_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_32xb128-mae_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_32xb128-mae_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_4xb544-ipu_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_4xb544-ipu_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_64xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p16_64xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-base-p32_64xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-base-p32_64xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-large-p16_64xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-large-p16_64xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/vision_transformer/vit-large-p32_64xb64_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/vision_transformer/vit-large-p32_64xb64_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/wrn/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/wrn/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/metafile.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/metafile.yml`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-large-24-p16_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-large-24-p16_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-large-24-p16_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-large-24-p16_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-large-24-p8_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-large-24-p8_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-large-24-p8_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-large-24-p8_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-medium-24-p16_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-medium-24-p16_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-medium-24-p16_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-medium-24-p16_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-medium-24-p8_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-medium-24-p8_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-medium-24-p8_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-medium-24-p8_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-nano-12-p16_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-nano-12-p16_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-nano-12-p16_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-nano-12-p16_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-nano-12-p8_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-nano-12-p8_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-nano-12-p8_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-nano-12-p8_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-12-p16_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-12-p16_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-12-p16_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-12-p16_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-12-p8_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-12-p8_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-12-p8_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-12-p8_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-24-p16_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-24-p16_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-24-p16_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-24-p16_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-24-p8_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-24-p8_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-small-24-p8_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-small-24-p8_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p16_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p16_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p16_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p16_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p8_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p8_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p8_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-12-p8_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p16_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p16_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p16_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p16_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p8_8xb128_in1k-384px.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p8_8xb128_in1k-384px.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p8_8xb128_in1k.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/configs/xcit/xcit-tiny-24-p8_8xb128_in1k.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/model-index.yml` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/model-index.yml`

 * *Files 2% similar despite different names*

```diff
@@ -62,8 +62,17 @@
   - configs/swav/metafile.yml
   - configs/mae/metafile.yml
   - configs/simmim/metafile.yml
   - configs/barlowtwins/metafile.yml
   - configs/cae/metafile.yml
   - configs/maskfeat/metafile.yml
   - configs/milan/metafile.yml
+  - configs/ofa/metafile.yml
   - configs/riformer/metafile.yml
+  - configs/sam/metafile.yml
+  - configs/glip/metafile.yml
+  - configs/eva02/metafile.yml
+  - configs/dinov2/metafile.yml
+  - configs/blip/metafile.yml
+  - configs/flamingo/metafile.yml
+  - configs/blip2/metafile.yml
+  - configs/chinese_clip/metafile.yml
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/analyze_logs.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/analyze_logs.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/analyze_results.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/analyze_results.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/confusion_matrix.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/eval_metric.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/eval_metric.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/analysis_tools/get_flops.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/analysis_tools/get_flops.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_dist_train_c4.sh` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_dist_train_c4.sh`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_train_c4.sh` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_train_c4.sh`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_train_fpn.sh` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmdetection/mim_slurm_train_fpn.sh`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_slurm_train.sh` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/benchmarks/mmsegmentation/mim_slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/dataset_converters/convert_imagenet_subsets.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/dataset_converters/convert_imagenet_subsets.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/dataset_converters/convert_inaturalist.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/dataset_converters/convert_inaturalist.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/kfold-cross-valid.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/kfold-cross-valid.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/misc/print_config.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/misc/print_config.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/misc/verify_dataset.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/misc/verify_dataset.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/clip_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/clip_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/convnext_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/convnext_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/davit_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/davit_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/deit3_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/deit3_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/edgenext_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/edgenext_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/efficientnet_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/efficientnet_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/efficientnetv2_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/efficientnetv2_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/eva_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/eva_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/hornet2mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/hornet2mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/levit2mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/levit2mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/mixmim_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/mixmim_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/mlpmixer_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/mlpmixer_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/mobilenetv2_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/mobilenetv2_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/publish_model.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/publish_model.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/reparameterize_model.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/reparameterize_model.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/replknet_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/replknet_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/repvgg_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/repvgg_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/revvit_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/revvit_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/shufflenetv2_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/shufflenetv2_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/tinyvit_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/tinyvit_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/torchvision_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/torchvision_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/twins2mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/twins2mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/van2mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/van2mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/vgg_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/vgg_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/model_converters/vig_to_mmpretrain.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/model_converters/vig_to_mmpretrain.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/slurm_test.sh` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/slurm_test.sh`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/slurm_train.sh` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/slurm_train.sh`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/test.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/test.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/torchserve/mmpretrain2torchserve.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/torchserve/mmpretrain2torchserve.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/torchserve/mmpretrain_handler.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/torchserve/mmpretrain_handler.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/torchserve/test_torchserver.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/torchserve/test_torchserver.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/train.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/train.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/visualization/browse_dataset.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/visualization/browse_dataset.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/visualization/vis_cam.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/visualization/vis_cam.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/visualization/vis_scheduler.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/visualization/vis_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/.mim/tools/visualization/vis_tsne.py` & `mmpretrain-1.0.0rc8/mmpretrain/.mim/tools/visualization/vis_tsne.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .apis import *  # noqa: F401, F403
 from .version import __version__
 
 mmcv_minimum_version = '2.0.0rc4'
 mmcv_maximum_version = '2.1.0'
 mmcv_version = digit_version(mmcv.__version__)
 
-mmengine_minimum_version = '0.5.0'
+mmengine_minimum_version = '0.7.1'
 mmengine_maximum_version = '1.0.0'
 mmengine_version = digit_version(mmengine.__version__)
 
 assert (mmcv_version >= digit_version(mmcv_minimum_version)
         and mmcv_version < digit_version(mmcv_maximum_version)), \
     f'MMCV=={mmcv.__version__} is used but incompatible. ' \
     f'Please install mmcv>={mmcv_minimum_version}, <{mmcv_maximum_version}.'
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/apis/feature_extractor.py` & `mmpretrain-1.0.0rc8/mmpretrain/apis/nlvr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,145 +1,150 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from typing import Callable, List, Optional, Union
+from copy import deepcopy
+from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from mmcv.image import imread
 from mmengine.config import Config
 from mmengine.dataset import Compose, default_collate
-from mmengine.device import get_device
-from mmengine.infer import BaseInferencer
-from mmengine.model import BaseModel
-from mmengine.runner import load_checkpoint
 
 from mmpretrain.registry import TRANSFORMS
-from .model import get_model, list_models
+from mmpretrain.structures import DataSample
+from .base import BaseInferencer
+from .model import list_models
 
-ModelType = Union[BaseModel, str, Config]
-InputType = Union[str, np.ndarray, list]
+InputType = Tuple[Union[str, np.ndarray], Union[str, np.ndarray], str]
+InputsType = Union[List[InputType], InputType]
 
 
-class FeatureExtractor(BaseInferencer):
-    """The inferencer for extract features.
+class NLVRInferencer(BaseInferencer):
+    """The inferencer for Natural Language for Visual Reasoning.
 
     Args:
-        model (BaseModel | str | Config): A model name or a path to the confi
+        model (BaseModel | str | Config): A model name or a path to the config
             file, or a :obj:`BaseModel` object. The model name can be found
-            by ``FeatureExtractor.list_models()``.
-        pretrained (bool | str): When use name to specify model, you can
-            use ``True`` to load the pre-defined pretrained weights. And you
-            can also use a string to specify the path or link of weights to
-            load. Defaults to True.
-        device (str, optional): Device to run inference. If None, use CPU or
-            the device of the input model. Defaults to None.
+            by ``NLVRInferencer.list_models()`` and you can also
+            query it in :doc:`/modelzoo_statistics`.
+        pretrained (str, optional): Path to the checkpoint. If None, it will
+            try to find a pre-defined weight from the model you specified
+            (only work if the ``model`` is a model name). Defaults to None.
+        device (str, optional): Device to run inference. If None, the available
+            device will be automatically used. Defaults to None.
+        **kwargs: Other keyword arguments to initialize the model (only work if
+            the ``model`` is a model name).
     """
 
-    def __init__(
-        self,
-        model: ModelType,
-        pretrained: Union[bool, str] = True,
-        device: Union[str, torch.device, None] = None,
-    ) -> None:
-        device = device or get_device()
-
-        if isinstance(model, BaseModel):
-            if isinstance(pretrained, str):
-                load_checkpoint(model, pretrained, map_location='cpu')
-            model = model.to(device)
-        else:
-            model = get_model(model, pretrained, device)
-
-        model.eval()
-
-        self.config = model.config
-        self.model = model
-        self.pipeline = self._init_pipeline(self.config)
-        self.collate_fn = default_collate
-        self.visualizer = None
+    visualize_kwargs: set = {
+        'resize', 'draw_score', 'show', 'show_dir', 'wait_time'
+    }
 
     def __call__(self,
-                 inputs: InputType,
+                 inputs: InputsType,
+                 return_datasamples: bool = False,
                  batch_size: int = 1,
                  **kwargs) -> dict:
         """Call the inferencer.
 
         Args:
-            inputs (str | array | list): The image path or array, or a list of
-                images.
+            inputs (tuple, List[tuple]): The input data tuples, every tuple
+                should include three items (left image, right image, text).
+                The image can be a path or numpy array.
+            return_datasamples (bool): Whether to return results as
+                :obj:`DataSample`. Defaults to False.
             batch_size (int): Batch size. Defaults to 1.
-            **kwargs: Other keyword arguments accepted by the `extract_feat`
-                method of the model.
+            resize (int, optional): Resize the short edge of the image to the
+                specified length before visualization. Defaults to None.
+            draw_score (bool): Whether to draw the prediction scores
+                of prediction categories. Defaults to True.
+            show (bool): Whether to display the visualization result in a
+                window. Defaults to False.
+            wait_time (float): The display time (s). Defaults to 0, which means
+                "forever".
+            show_dir (str, optional): If not None, save the visualization
+                results in the specified directory. Defaults to None.
 
         Returns:
-            tensor | Tuple[tensor]: The extracted features.
+            list: The inference results.
         """
-        ori_inputs = self._inputs_to_list(inputs)
-        inputs = self.preprocess(ori_inputs, batch_size=batch_size)
-        preds = []
-        for data in inputs:
-            preds.extend(self.forward(data, **kwargs))
-
-        return preds
-
-    @torch.no_grad()
-    def forward(self, inputs: Union[dict, tuple], **kwargs):
-        inputs = self.model.data_preprocessor(inputs, False)['inputs']
-        outputs = self.model.extract_feat(inputs, **kwargs)
-
-        def scatter(feats, index):
-            if isinstance(feats, torch.Tensor):
-                return feats[index]
-            else:
-                # Sequence of tensor
-                return type(feats)([scatter(item, index) for item in feats])
-
-        results = []
-        for i in range(inputs.shape[0]):
-            results.append(scatter(outputs, i))
-
-        return results
+        assert isinstance(inputs, (tuple, list))
+        if isinstance(inputs, tuple):
+            inputs = [inputs]
+        for input_ in inputs:
+            assert isinstance(input_, tuple)
+            assert len(input_) == 3
+
+        return super().__call__(
+            inputs,
+            return_datasamples=return_datasamples,
+            batch_size=batch_size,
+            **kwargs)
 
     def _init_pipeline(self, cfg: Config) -> Callable:
         test_pipeline_cfg = cfg.test_dataloader.dataset.pipeline
-        if test_pipeline_cfg[0]['type'] == 'LoadImageFromFile':
-            # Image loading is finished in `self.preprocess`.
-            test_pipeline_cfg = test_pipeline_cfg[1:]
+        assert test_pipeline_cfg[0]['type'] == 'ApplyToList'
+
+        list_pipeline = deepcopy(test_pipeline_cfg[0])
+        if list_pipeline.scatter_key == 'img_path':
+            # Remove `LoadImageFromFile`
+            list_pipeline.transforms.pop(0)
+            list_pipeline.scatter_key = 'img'
+
         test_pipeline = Compose(
-            [TRANSFORMS.build(t) for t in test_pipeline_cfg])
+            [TRANSFORMS.build(list_pipeline)] +
+            [TRANSFORMS.build(t) for t in test_pipeline_cfg[1:]])
         return test_pipeline
 
-    def preprocess(self, inputs: List[InputType], batch_size: int = 1):
+    def preprocess(self, inputs: InputsType, batch_size: int = 1):
 
         def load_image(input_):
-            img = imread(input_)
-            if img is None:
-                raise ValueError(f'Failed to read image {input_}.')
+            img1 = imread(input_[0])
+            img2 = imread(input_[1])
+            text = input_[2]
+            if img1 is None:
+                raise ValueError(f'Failed to read image {input_[0]}.')
+            if img2 is None:
+                raise ValueError(f'Failed to read image {input_[1]}.')
             return dict(
-                img=img,
-                img_shape=img.shape[:2],
-                ori_shape=img.shape[:2],
+                img=[img1, img2],
+                img_shape=[img1.shape[:2], img2.shape[:2]],
+                ori_shape=[img1.shape[:2], img2.shape[:2]],
+                text=text,
             )
 
         pipeline = Compose([load_image, self.pipeline])
 
         chunked_data = self._get_chunk_data(map(pipeline, inputs), batch_size)
-        yield from map(self.collate_fn, chunked_data)
+        yield from map(default_collate, chunked_data)
+
+    def postprocess(self,
+                    preds: List[DataSample],
+                    visualization: List[np.ndarray],
+                    return_datasamples=False) -> dict:
+        if return_datasamples:
+            return preds
 
-    def visualize(self):
-        raise NotImplementedError(
-            "The FeatureExtractor doesn't support visualization.")
-
-    def postprocess(self):
-        raise NotImplementedError(
-            "The FeatureExtractor doesn't need postprocessing.")
+        results = []
+        for data_sample in preds:
+            pred_scores = data_sample.pred_score
+            pred_score = float(torch.max(pred_scores).item())
+            pred_label = torch.argmax(pred_scores).item()
+            result = {
+                'pred_scores': pred_scores.detach().cpu().numpy(),
+                'pred_label': pred_label,
+                'pred_score': pred_score,
+            }
+            results.append(result)
+
+        return results
 
     @staticmethod
     def list_models(pattern: Optional[str] = None):
         """List all available model names.
 
         Args:
             pattern (str | None): A wildcard pattern to match model names.
 
         Returns:
             List[str]: a list of model names.
         """
-        return list_models(pattern=pattern)
+        return list_models(pattern=pattern, task='NLVR')
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/apis/image_classification.py` & `mmpretrain-1.0.0rc8/mmpretrain/apis/image_classification.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,40 +3,36 @@
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 from mmcv.image import imread
 from mmengine.config import Config
 from mmengine.dataset import Compose, default_collate
-from mmengine.device import get_device
-from mmengine.infer import BaseInferencer
-from mmengine.model import BaseModel
-from mmengine.runner import load_checkpoint
 
 from mmpretrain.registry import TRANSFORMS
 from mmpretrain.structures import DataSample
-from .model import get_model, list_models
-
-ModelType = Union[BaseModel, str, Config]
-InputType = Union[str, np.ndarray, list]
+from .base import BaseInferencer, InputType, ModelType
+from .model import list_models
 
 
 class ImageClassificationInferencer(BaseInferencer):
     """The inferencer for image classification.
 
     Args:
-        model (BaseModel | str | Config): A model name or a path to the confi
+        model (BaseModel | str | Config): A model name or a path to the config
             file, or a :obj:`BaseModel` object. The model name can be found
             by ``ImageClassificationInferencer.list_models()`` and you can also
             query it in :doc:`/modelzoo_statistics`.
-        weights (str, optional): Path to the checkpoint. If None, it will try
-            to find a pre-defined weight from the model you specified
+        pretrained (str, optional): Path to the checkpoint. If None, it will
+            try to find a pre-defined weight from the model you specified
             (only work if the ``model`` is a model name). Defaults to None.
-        device (str, optional): Device to run inference. If None, use CPU or
-            the device of the input model. Defaults to None.
+        device (str, optional): Device to run inference. If None, the available
+            device will be automatically used. Defaults to None.
+        **kwargs: Other keyword arguments to initialize the model (only work if
+            the ``model`` is a model name).
 
     Example:
         1. Use a pre-trained model in MMPreTrain to inference an image.
 
            >>> from mmpretrain import ImageClassificationInferencer
            >>> inferencer = ImageClassificationInferencer('resnet50_8xb32_in1k')
            >>> inferencer('demo/demo.JPEG')
@@ -47,52 +43,38 @@
 
         2. Use a config file and checkpoint to inference multiple images on GPU,
            and save the visualization results in a folder.
 
            >>> from mmpretrain import ImageClassificationInferencer
            >>> inferencer = ImageClassificationInferencer(
                    model='configs/resnet/resnet50_8xb32_in1k.py',
-                   weights='https://download.openmmlab.com/mmclassification/v0/resnet/resnet50_8xb32_in1k_20210831-ea4938fc.pth',
+                   pretrained='https://download.openmmlab.com/mmclassification/v0/resnet/resnet50_8xb32_in1k_20210831-ea4938fc.pth',
                    device='cuda')
            >>> inferencer(['demo/dog.jpg', 'demo/bird.JPEG'], show_dir="./visualize/")
     """  # noqa: E501
 
     visualize_kwargs: set = {
         'resize', 'rescale_factor', 'draw_score', 'show', 'show_dir',
         'wait_time'
     }
 
-    def __init__(
-        self,
-        model: ModelType,
-        pretrained: Union[bool, str] = True,
-        device: Union[str, torch.device, None] = None,
-        classes=None,
-    ) -> None:
-        device = device or get_device()
-
-        if isinstance(model, BaseModel):
-            if isinstance(pretrained, str):
-                load_checkpoint(model, pretrained, map_location='cpu')
-            model = model.to(device)
-        else:
-            model = get_model(model, pretrained, device)
-
-        model.eval()
-
-        self.config = model.config
-        self.model = model
-        self.pipeline = self._init_pipeline(self.config)
-        self.collate_fn = default_collate
-        self.visualizer = None
+    def __init__(self,
+                 model: ModelType,
+                 pretrained: Union[bool, str] = True,
+                 device: Union[str, torch.device, None] = None,
+                 classes=None,
+                 **kwargs) -> None:
+        super().__init__(
+            model=model, pretrained=pretrained, device=device, **kwargs)
 
         if classes is not None:
             self.classes = classes
         else:
-            self.classes = getattr(model, 'dataset_meta', {}).get('classes')
+            self.classes = getattr(self.model, '_dataset_meta',
+                                   {}).get('classes')
 
     def __call__(self,
                  inputs: InputType,
                  return_datasamples: bool = False,
                  batch_size: int = 1,
                  **kwargs) -> dict:
         """Call the inferencer.
@@ -116,16 +98,19 @@
                 "forever".
             show_dir (str, optional): If not None, save the visualization
                 results in the specified directory. Defaults to None.
 
         Returns:
             list: The inference results.
         """
-        return super().__call__(inputs, return_datasamples, batch_size,
-                                **kwargs)
+        return super().__call__(
+            inputs,
+            return_datasamples=return_datasamples,
+            batch_size=batch_size,
+            **kwargs)
 
     def _init_pipeline(self, cfg: Config) -> Callable:
         test_pipeline_cfg = cfg.test_dataloader.dataset.pipeline
         if test_pipeline_cfg[0]['type'] == 'LoadImageFromFile':
             # Image loading is finished in `self.preprocess`.
             test_pipeline_cfg = test_pipeline_cfg[1:]
         test_pipeline = Compose(
@@ -143,15 +128,15 @@
                 img_shape=img.shape[:2],
                 ori_shape=img.shape[:2],
             )
 
         pipeline = Compose([load_image, self.pipeline])
 
         chunked_data = self._get_chunk_data(map(pipeline, inputs), batch_size)
-        yield from map(self.collate_fn, chunked_data)
+        yield from map(default_collate, chunked_data)
 
     def visualize(self,
                   ori_inputs: List[InputType],
                   preds: List[DataSample],
                   show: bool = False,
                   wait_time: int = 0,
                   resize: Optional[int] = None,
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/apis/image_retrieval.py` & `mmpretrain-1.0.0rc8/mmpretrain/apis/image_retrieval.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,156 +3,145 @@
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import torch
 from mmcv.image import imread
 from mmengine.config import Config
 from mmengine.dataset import BaseDataset, Compose, default_collate
-from mmengine.device import get_device
-from mmengine.infer import BaseInferencer
-from mmengine.model import BaseModel
-from mmengine.runner import load_checkpoint
 
 from mmpretrain.registry import TRANSFORMS
 from mmpretrain.structures import DataSample
-from .model import get_model, list_models
-
-ModelType = Union[BaseModel, str, Config]
-InputType = Union[str, np.ndarray, list]
+from .base import BaseInferencer, InputType, ModelType
+from .model import list_models
 
 
 class ImageRetrievalInferencer(BaseInferencer):
     """The inferencer for image to image retrieval.
 
     Args:
-        model (BaseModel | str | Config): A model name or a path to the confi
+        model (BaseModel | str | Config): A model name or a path to the config
             file, or a :obj:`BaseModel` object. The model name can be found
-            by ``ImageClassificationInferencer.list_models()`` and you can also
+            by ``ImageRetrievalInferencer.list_models()`` and you can also
             query it in :doc:`/modelzoo_statistics`.
-        weights (str, optional): Path to the checkpoint. If None, it will try
-            to find a pre-defined weight from the model you specified
+        prototype (str | list | dict | DataLoader, BaseDataset): The images to
+            be retrieved. It can be the following types:
+
+            - str: The directory of the the images.
+            - list: A list of path of the images.
+            - dict: A config dict of the a prototype dataset.
+            - BaseDataset: A prototype dataset.
+            - DataLoader: A data loader to load the prototype data.
+
+        prototype_cache (str, optional): The path of the generated prototype
+            features. If exists, directly load the cache instead of re-generate
+            the prototype features. If not exists, save the generated features
+            to the path. Defaults to None.
+        pretrained (str, optional): Path to the checkpoint. If None, it will
+            try to find a pre-defined weight from the model you specified
             (only work if the ``model`` is a model name). Defaults to None.
-        device (str, optional): Device to run inference. If None, use CPU or
-            the device of the input model. Defaults to None.
+        device (str, optional): Device to run inference. If None, the available
+            device will be automatically used. Defaults to None.
+        **kwargs: Other keyword arguments to initialize the model (only work if
+            the ``model`` is a model name).
 
     Example:
-        1. Use a pre-trained model in MMPreTrain to inference an image.
-
-           >>> from mmpretrain import ImageClassificationInferencer
-           >>> inferencer = ImageClassificationInferencer('resnet50_8xb32_in1k')
-           >>> inferencer('demo/demo.JPEG')
-           [{'pred_score': array([...]),
-             'pred_label': 65,
-             'pred_score': 0.6649367809295654,
-             'pred_class': 'sea snake'}]
-
-        2. Use a config file and checkpoint to inference multiple images on GPU,
-           and save the visualization results in a folder.
-
-           >>> from mmpretrain import ImageClassificationInferencer
-           >>> inferencer = ImageClassificationInferencer(
-                   model='configs/resnet/resnet50_8xb32_in1k.py',
-                   weights='https://download.openmmlab.com/mmclassification/v0/resnet/resnet50_8xb32_in1k_20210831-ea4938fc.pth',
-                   device='cuda')
-           >>> inferencer(['demo/dog.jpg', 'demo/bird.JPEG'], show_dir="./visualize/")
+        >>> from mmpretrain import ImageRetrievalInferencer
+        >>> inferencer = ImageRetrievalInferencer(
+        ...     'resnet50-arcface_8xb32_inshop',
+        ...     prototype='./demo/',
+        ...     prototype_cache='img_retri.pth')
+        >>> inferencer('demo/cat-dog.png', topk=2)[0][1]
+        {'match_score': tensor(0.4088, device='cuda:0'),
+         'sample_idx': 3,
+         'sample': {'img_path': './demo/dog.jpg'}}
     """  # noqa: E501
 
     visualize_kwargs: set = {
-        'draw_score', 'resize', 'show_dir', 'show', 'wait_time'
+        'draw_score', 'resize', 'show_dir', 'show', 'wait_time', 'topk'
     }
     postprocess_kwargs: set = {'topk'}
 
     def __init__(
         self,
         model: ModelType,
         prototype,
-        prototype_vecs=None,
+        prototype_cache=None,
         prepare_batch_size=8,
         pretrained: Union[bool, str] = True,
         device: Union[str, torch.device, None] = None,
+        **kwargs,
     ) -> None:
-        device = device or get_device()
-
-        if isinstance(model, BaseModel):
-            if isinstance(pretrained, str):
-                load_checkpoint(model, pretrained, map_location='cpu')
-            model = model.to(device)
-        else:
-            model = get_model(model, pretrained, device)
-
-        model.eval()
-
-        self.config = model.config
-        self.model = model
-        self.pipeline = self._init_pipeline(self.config)
-        self.collate_fn = default_collate
-        self.visualizer = None
+        super().__init__(
+            model=model, pretrained=pretrained, device=device, **kwargs)
 
         self.prototype_dataset = self._prepare_prototype(
-            prototype, prototype_vecs, prepare_batch_size)
-
-        # An ugly hack to escape from the duplicated arguments check in the
-        # base class
-        self.visualize_kwargs.add('topk')
+            prototype, prototype_cache, prepare_batch_size)
 
-    def _prepare_prototype(self, prototype, prototype_vecs=None, batch_size=8):
+    def _prepare_prototype(self, prototype, cache=None, batch_size=8):
         from mmengine.dataset import DefaultSampler
         from torch.utils.data import DataLoader
 
         def build_dataloader(dataset):
             return DataLoader(
                 dataset,
                 batch_size=batch_size,
-                collate_fn=self.collate_fn,
+                collate_fn=default_collate,
                 sampler=DefaultSampler(dataset, shuffle=False),
                 persistent_workers=False,
             )
 
-        test_pipeline = self.config.test_dataloader.dataset.pipeline
-
         if isinstance(prototype, str):
             # A directory path of images
-            from mmpretrain.datasets import CustomDataset
-            dataset = CustomDataset(
-                data_root=prototype, pipeline=test_pipeline, with_label=False)
+            prototype = dict(
+                type='CustomDataset', with_label=False, data_root=prototype)
+
+        if isinstance(prototype, list):
+            test_pipeline = [dict(type='LoadImageFromFile'), self.pipeline]
+            dataset = BaseDataset(
+                lazy_init=True, serialize_data=False, pipeline=test_pipeline)
+            dataset.data_list = [{
+                'sample_idx': i,
+                'img_path': file
+            } for i, file in enumerate(prototype)]
+            dataset._fully_initialized = True
             dataloader = build_dataloader(dataset)
         elif isinstance(prototype, dict):
             # A config of dataset
             from mmpretrain.registry import DATASETS
-            prototype.setdefault('pipeline', test_pipeline)
+            test_pipeline = [dict(type='LoadImageFromFile'), self.pipeline]
             dataset = DATASETS.build(prototype)
             dataloader = build_dataloader(dataset)
         elif isinstance(prototype, DataLoader):
             dataset = prototype.dataset
             dataloader = prototype
         elif isinstance(prototype, BaseDataset):
             dataset = prototype
             dataloader = build_dataloader(dataset)
         else:
             raise TypeError(f'Unsupported prototype type {type(prototype)}.')
 
-        if prototype_vecs is not None and Path(prototype_vecs).exists():
-            self.model.prototype = prototype_vecs
+        if cache is not None and Path(cache).exists():
+            self.model.prototype = cache
         else:
             self.model.prototype = dataloader
         self.model.prepare_prototype()
 
         from mmengine.logging import MMLogger
         logger = MMLogger.get_current_instance()
-        if prototype_vecs is None:
+        if cache is None:
             logger.info('The prototype has been prepared, you can use '
-                        '`save_prototype_vecs` to dump it into a pickle '
+                        '`save_prototype` to dump it into a pickle '
                         'file for the future usage.')
-        elif not Path(prototype_vecs).exists():
-            self.save_prototype_vecs(prototype_vecs)
-            logger.info(f'The prototype has been saved at {prototype_vecs}.')
+        elif not Path(cache).exists():
+            self.save_prototype(cache)
+            logger.info(f'The prototype has been saved at {cache}.')
 
         return dataset
 
-    def save_prototype_vecs(self, path):
+    def save_prototype(self, path):
         self.model.dump_prototype(path)
 
     def __call__(self,
                  inputs: InputType,
                  return_datasamples: bool = False,
                  batch_size: int = 1,
                  **kwargs) -> dict:
@@ -201,15 +190,15 @@
                 img_shape=img.shape[:2],
                 ori_shape=img.shape[:2],
             )
 
         pipeline = Compose([load_image, self.pipeline])
 
         chunked_data = self._get_chunk_data(map(pipeline, inputs), batch_size)
-        yield from map(self.collate_fn, chunked_data)
+        yield from map(default_collate, chunked_data)
 
     def visualize(self,
                   ori_inputs: List[InputType],
                   preds: List[DataSample],
                   topk: int = 3,
                   resize: Optional[int] = 224,
                   show: bool = False,
@@ -290,53 +279,7 @@
         Args:
             pattern (str | None): A wildcard pattern to match model names.
 
         Returns:
             List[str]: a list of model names.
         """
         return list_models(pattern=pattern, task='Image Retrieval')
-
-    def _dispatch_kwargs(self, **kwargs):
-        """Dispatch kwargs to preprocess(), forward(), visualize() and
-        postprocess() according to the actual demands.
-
-        Override this method to allow same argument for different methods.
-
-        Returns:
-            Tuple[Dict, Dict, Dict, Dict]: kwargs passed to preprocess,
-            forward, visualize and postprocess respectively.
-        """
-        method_kwargs = set.union(
-            self.preprocess_kwargs,
-            self.forward_kwargs,
-            self.visualize_kwargs,
-            self.postprocess_kwargs,
-        )
-
-        union_kwargs = method_kwargs | set(kwargs.keys())
-        if union_kwargs != method_kwargs:
-            unknown_kwargs = union_kwargs - method_kwargs
-            raise ValueError(
-                f'unknown argument {unknown_kwargs} for `preprocess`, '
-                '`forward`, `visualize` and `postprocess`')
-
-        preprocess_kwargs = {}
-        forward_kwargs = {}
-        visualize_kwargs = {}
-        postprocess_kwargs = {}
-
-        for key, value in kwargs.items():
-            if key in self.preprocess_kwargs:
-                preprocess_kwargs[key] = value
-            if key in self.forward_kwargs:
-                forward_kwargs[key] = value
-            if key in self.visualize_kwargs:
-                visualize_kwargs[key] = value
-            if key in self.postprocess_kwargs:
-                postprocess_kwargs[key] = value
-
-        return (
-            preprocess_kwargs,
-            forward_kwargs,
-            visualize_kwargs,
-            postprocess_kwargs,
-        )
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/base_dataset.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/base_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         indices (int or Sequence[int], optional): Support using first few
             data in annotation file to facilitate training/testing on a smaller
             dataset. Defaults to None, which means using all ``data_infos``.
         serialize_data (bool): Whether to hold memory using serialized objects,
             when enabled, data loader workers can use shared RAM from master
             process instead of making a copy. Defaults to True.
         pipeline (Sequence): Processing pipeline. Defaults to an empty tuple.
-        test_mode (bool): ``test_mode=True`` means in test phase.
+        test_mode (bool, optional): ``test_mode=True`` means in test phase,
+            an error will be raised when getting an item fails, ``test_mode=False``
+            means in training phase, another item will be returned randomly.
             Defaults to False.
         lazy_init (bool): Whether to load annotation during instantiation.
             In some cases, such as visualization, only the meta information of
             the dataset is needed, which is not necessary to load annotation
             file. ``Basedataset`` can skip load annotations to save time by set
             ``lazy_init=False``. Defaults to False.
         max_refetch (int): If ``Basedataset.prepare_data`` get a None img.
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/builder.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/categories.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/categories.py`

 * *Files 22% similar despite different names*

```diff
@@ -1137,7 +1137,304 @@
     'stage/indoor', 'subway_station/platform', 'swimming_pool/outdoor',
     'television_studio', 'topiary_garden', 'tower', 'train_railway',
     'tree_farm', 'trench', 'temple/east_asia', 'temple/south_asia',
     'track/outdoor', 'train_station/platform', 'underwater/coral_reef',
     'valley', 'vegetable_garden', 'veranda', 'viaduct', 'volcano',
     'waiting_room', 'water_tower', 'watering_hole', 'wheat_field', 'wind_farm',
     'windmill', 'yard')
+
+OxfordIIITPet_CATEGORIES = (
+    'Abyssinian', 'american_bulldog', 'american_pit_bull_terrier',
+    'basset_hound', 'beagle', 'Bengal', 'Birman', 'Bombay', 'boxer',
+    'British_Shorthair', 'chihuahua', 'Egyptian_Mau', 'english_cocker_spaniel',
+    'english_setter', 'german_shorthaired', 'great_pyrenees', 'havanese',
+    'japanese_chin', 'keeshond', 'leonberger', 'Maine_Coon',
+    'miniature_pinscher', 'newfoundland', 'Persian', 'pomeranian', 'pug',
+    'Ragdoll', 'Russian_Blue', 'saint_bernard', 'samoyed', 'scottish_terrier',
+    'shiba_inu', 'Siamese', 'Sphynx', 'staffordshire_bull_terrier',
+    'wheaten_terrier', 'yorkshire_terrier')
+
+DTD_CATEGORIES = ('banded', 'blotchy', 'braided', 'bubbly', 'bumpy',
+                  'chequered', 'cobwebbed', 'cracked', 'crosshatched',
+                  'crystalline', 'dotted', 'fibrous', 'flecked', 'freckled',
+                  'frilly', 'gauzy', 'grid', 'grooved', 'honeycombed',
+                  'interlaced', 'knitted', 'lacelike', 'lined', 'marbled',
+                  'matted', 'meshed', 'paisley', 'perforated', 'pitted',
+                  'pleated', 'polka-dotted', 'porous', 'potholed', 'scaly',
+                  'smeared', 'spiralled', 'sprinkled', 'stained', 'stratified',
+                  'striped', 'studded', 'swirly', 'veined', 'waffled', 'woven',
+                  'wrinkled', 'zigzagged')
+
+FGVCAIRCRAFT_CATEGORIES = (
+    '707-320', '727-200', '737-200', '737-300', '737-400', '737-500',
+    '737-600', '737-700', '737-800', '737-900', '747-100', '747-200',
+    '747-300', '747-400', '757-200', '757-300', '767-200', '767-300',
+    '767-400', '777-200', '777-300', 'A300B4', 'A310', 'A318', 'A319', 'A320',
+    'A321', 'A330-200', 'A330-300', 'A340-200', 'A340-300', 'A340-500',
+    'A340-600', 'A380', 'ATR-42', 'ATR-72', 'An-12', 'BAE 146-200',
+    'BAE 146-300', 'BAE-125', 'Beechcraft 1900', 'Boeing 717', 'C-130', 'C-47',
+    'CRJ-200', 'CRJ-700', 'CRJ-900', 'Cessna 172', 'Cessna 208', 'Cessna 525',
+    'Cessna 560', 'Challenger 600', 'DC-10', 'DC-3', 'DC-6', 'DC-8', 'DC-9-30',
+    'DH-82', 'DHC-1', 'DHC-6', 'DHC-8-100', 'DHC-8-300', 'DR-400',
+    'Dornier 328', 'E-170', 'E-190', 'E-195', 'EMB-120', 'ERJ 135', 'ERJ 145',
+    'Embraer Legacy 600', 'Eurofighter Typhoon', 'F-16A/B', 'F/A-18',
+    'Falcon 2000', 'Falcon 900', 'Fokker 100', 'Fokker 50', 'Fokker 70',
+    'Global Express', 'Gulfstream IV', 'Gulfstream V', 'Hawk T1', 'Il-76',
+    'L-1011', 'MD-11', 'MD-80', 'MD-87', 'MD-90', 'Metroliner', 'Model B200',
+    'PA-28', 'SR-20', 'Saab 2000', 'Saab 340', 'Spitfire', 'Tornado', 'Tu-134',
+    'Tu-154', 'Yak-42')
+
+STANFORDCARS_CATEGORIES = (
+    'AM General Hummer SUV 2000', 'Acura RL Sedan 2012', 'Acura TL Sedan 2012',
+    'Acura TL Type-S 2008', 'Acura TSX Sedan 2012',
+    'Acura Integra Type R 2001', 'Acura ZDX Hatchback 2012',
+    'Aston Martin V8 Vantage Convertible 2012',
+    'Aston Martin V8 Vantage Coupe 2012',
+    'Aston Martin Virage Convertible 2012', 'Aston Martin Virage Coupe 2012',
+    'Audi RS 4 Convertible 2008', 'Audi A5 Coupe 2012', 'Audi TTS Coupe 2012',
+    'Audi R8 Coupe 2012', 'Audi V8 Sedan 1994', 'Audi 100 Sedan 1994',
+    'Audi 100 Wagon 1994', 'Audi TT Hatchback 2011', 'Audi S6 Sedan 2011',
+    'Audi S5 Convertible 2012', 'Audi S5 Coupe 2012', 'Audi S4 Sedan 2012',
+    'Audi S4 Sedan 2007', 'Audi TT RS Coupe 2012',
+    'BMW ActiveHybrid 5 Sedan 2012', 'BMW 1 Series Convertible 2012',
+    'BMW 1 Series Coupe 2012', 'BMW 3 Series Sedan 2012',
+    'BMW 3 Series Wagon 2012', 'BMW 6 Series Convertible 2007',
+    'BMW X5 SUV 2007', 'BMW X6 SUV 2012', 'BMW M3 Coupe 2012',
+    'BMW M5 Sedan 2010', 'BMW M6 Convertible 2010', 'BMW X3 SUV 2012',
+    'BMW Z4 Convertible 2012',
+    'Bentley Continental Supersports Conv. Convertible 2012',
+    'Bentley Arnage Sedan 2009', 'Bentley Mulsanne Sedan 2011',
+    'Bentley Continental GT Coupe 2012', 'Bentley Continental GT Coupe 2007',
+    'Bentley Continental Flying Spur Sedan 2007',
+    'Bugatti Veyron 16.4 Convertible 2009', 'Bugatti Veyron 16.4 Coupe 2009',
+    'Buick Regal GS 2012', 'Buick Rainier SUV 2007', 'Buick Verano Sedan 2012',
+    'Buick Enclave SUV 2012', 'Cadillac CTS-V Sedan 2012',
+    'Cadillac SRX SUV 2012', 'Cadillac Escalade EXT Crew Cab 2007',
+    'Chevrolet Silverado 1500 Hybrid Crew Cab 2012',
+    'Chevrolet Corvette Convertible 2012', 'Chevrolet Corvette ZR1 2012',
+    'Chevrolet Corvette Ron Fellows Edition Z06 2007',
+    'Chevrolet Traverse SUV 2012', 'Chevrolet Camaro Convertible 2012',
+    'Chevrolet HHR SS 2010', 'Chevrolet Impala Sedan 2007',
+    'Chevrolet Tahoe Hybrid SUV 2012', 'Chevrolet Sonic Sedan 2012',
+    'Chevrolet Express Cargo Van 2007', 'Chevrolet Avalanche Crew Cab 2012',
+    'Chevrolet Cobalt SS 2010', 'Chevrolet Malibu Hybrid Sedan 2010',
+    'Chevrolet TrailBlazer SS 2009',
+    'Chevrolet Silverado 2500HD Regular Cab 2012',
+    'Chevrolet Silverado 1500 Classic Extended Cab 2007',
+    'Chevrolet Express Van 2007', 'Chevrolet Monte Carlo Coupe 2007',
+    'Chevrolet Malibu Sedan 2007',
+    'Chevrolet Silverado 1500 Extended Cab 2012',
+    'Chevrolet Silverado 1500 Regular Cab 2012', 'Chrysler Aspen SUV 2009',
+    'Chrysler Sebring Convertible 2010',
+    'Chrysler Town and Country Minivan 2012', 'Chrysler 300 SRT-8 2010',
+    'Chrysler Crossfire Convertible 2008',
+    'Chrysler PT Cruiser Convertible 2008', 'Daewoo Nubira Wagon 2002',
+    'Dodge Caliber Wagon 2012', 'Dodge Caliber Wagon 2007',
+    'Dodge Caravan Minivan 1997', 'Dodge Ram Pickup 3500 Crew Cab 2010',
+    'Dodge Ram Pickup 3500 Quad Cab 2009', 'Dodge Sprinter Cargo Van 2009',
+    'Dodge Journey SUV 2012', 'Dodge Dakota Crew Cab 2010',
+    'Dodge Dakota Club Cab 2007', 'Dodge Magnum Wagon 2008',
+    'Dodge Challenger SRT8 2011', 'Dodge Durango SUV 2012',
+    'Dodge Durango SUV 2007', 'Dodge Charger Sedan 2012',
+    'Dodge Charger SRT-8 2009', 'Eagle Talon Hatchback 1998',
+    'FIAT 500 Abarth 2012', 'FIAT 500 Convertible 2012',
+    'Ferrari FF Coupe 2012', 'Ferrari California Convertible 2012',
+    'Ferrari 458 Italia Convertible 2012', 'Ferrari 458 Italia Coupe 2012',
+    'Fisker Karma Sedan 2012', 'Ford F-450 Super Duty Crew Cab 2012',
+    'Ford Mustang Convertible 2007', 'Ford Freestar Minivan 2007',
+    'Ford Expedition EL SUV 2009', 'Ford Edge SUV 2012',
+    'Ford Ranger SuperCab 2011', 'Ford GT Coupe 2006',
+    'Ford F-150 Regular Cab 2012', 'Ford F-150 Regular Cab 2007',
+    'Ford Focus Sedan 2007', 'Ford E-Series Wagon Van 2012',
+    'Ford Fiesta Sedan 2012', 'GMC Terrain SUV 2012', 'GMC Savana Van 2012',
+    'GMC Yukon Hybrid SUV 2012', 'GMC Acadia SUV 2012',
+    'GMC Canyon Extended Cab 2012', 'Geo Metro Convertible 1993',
+    'HUMMER H3T Crew Cab 2010', 'HUMMER H2 SUT Crew Cab 2009',
+    'Honda Odyssey Minivan 2012', 'Honda Odyssey Minivan 2007',
+    'Honda Accord Coupe 2012', 'Honda Accord Sedan 2012',
+    'Hyundai Veloster Hatchback 2012', 'Hyundai Santa Fe SUV 2012',
+    'Hyundai Tucson SUV 2012', 'Hyundai Veracruz SUV 2012',
+    'Hyundai Sonata Hybrid Sedan 2012', 'Hyundai Elantra Sedan 2007',
+    'Hyundai Accent Sedan 2012', 'Hyundai Genesis Sedan 2012',
+    'Hyundai Sonata Sedan 2012', 'Hyundai Elantra Touring Hatchback 2012',
+    'Hyundai Azera Sedan 2012', 'Infiniti G Coupe IPL 2012',
+    'Infiniti QX56 SUV 2011', 'Isuzu Ascender SUV 2008', 'Jaguar XK XKR 2012',
+    'Jeep Patriot SUV 2012', 'Jeep Wrangler SUV 2012', 'Jeep Liberty SUV 2012',
+    'Jeep Grand Cherokee SUV 2012', 'Jeep Compass SUV 2012',
+    'Lamborghini Reventon Coupe 2008', 'Lamborghini Aventador Coupe 2012',
+    'Lamborghini Gallardo LP 570-4 Superleggera 2012',
+    'Lamborghini Diablo Coupe 2001', 'Land Rover Range Rover SUV 2012',
+    'Land Rover LR2 SUV 2012', 'Lincoln Town Car Sedan 2011',
+    'MINI Cooper Roadster Convertible 2012',
+    'Maybach Landaulet Convertible 2012', 'Mazda Tribute SUV 2011',
+    'McLaren MP4-12C Coupe 2012', 'Mercedes-Benz 300-Class Convertible 1993',
+    'Mercedes-Benz C-Class Sedan 2012', 'Mercedes-Benz SL-Class Coupe 2009',
+    'Mercedes-Benz E-Class Sedan 2012', 'Mercedes-Benz S-Class Sedan 2012',
+    'Mercedes-Benz Sprinter Van 2012', 'Mitsubishi Lancer Sedan 2012',
+    'Nissan Leaf Hatchback 2012', 'Nissan NV Passenger Van 2012',
+    'Nissan Juke Hatchback 2012', 'Nissan 240SX Coupe 1998',
+    'Plymouth Neon Coupe 1999', 'Porsche Panamera Sedan 2012',
+    'Ram C/V Cargo Van Minivan 2012',
+    'Rolls-Royce Phantom Drophead Coupe Convertible 2012',
+    'Rolls-Royce Ghost Sedan 2012', 'Rolls-Royce Phantom Sedan 2012',
+    'Scion xD Hatchback 2012', 'Spyker C8 Convertible 2009',
+    'Spyker C8 Coupe 2009', 'Suzuki Aerio Sedan 2007',
+    'Suzuki Kizashi Sedan 2012', 'Suzuki SX4 Hatchback 2012',
+    'Suzuki SX4 Sedan 2012', 'Tesla Model S Sedan 2012',
+    'Toyota Sequoia SUV 2012', 'Toyota Camry Sedan 2012',
+    'Toyota Corolla Sedan 2012', 'Toyota 4Runner SUV 2012',
+    'Volkswagen Golf Hatchback 2012', 'Volkswagen Golf Hatchback 1991',
+    'Volkswagen Beetle Hatchback 2012', 'Volvo C30 Hatchback 2012',
+    'Volvo 240 Sedan 1993', 'Volvo XC90 SUV 2007',
+    'smart fortwo Convertible 2012')
+
+SUN397_CATEGORIES = (
+    'abbey', 'airplane_cabin', 'airport_terminal', 'alley', 'amphitheater',
+    'amusement_arcade', 'amusement_park', 'anechoic_chamber',
+    'apartment_building_outdoor', 'apse_indoor', 'aquarium', 'aqueduct',
+    'arch', 'archive', 'arrival_gate_outdoor', 'art_gallery', 'art_school',
+    'art_studio', 'assembly_line', 'athletic_field_outdoor', 'atrium_public',
+    'attic', 'auditorium', 'auto_factory', 'badlands',
+    'badminton_court_indoor', 'baggage_claim', 'bakery_shop',
+    'balcony_exterior', 'balcony_interior', 'ball_pit', 'ballroom',
+    'bamboo_forest', 'banquet_hall', 'bar', 'barn', 'barndoor',
+    'baseball_field', 'basement', 'basilica', 'basketball_court_outdoor',
+    'bathroom', 'batters_box', 'bayou', 'bazaar_indoor', 'bazaar_outdoor',
+    'beach', 'beauty_salon', 'bedroom', 'berth', 'biology_laboratory',
+    'bistro_indoor', 'boardwalk', 'boat_deck', 'boathouse', 'bookstore',
+    'booth_indoor', 'botanical_garden', 'bow_window_indoor',
+    'bow_window_outdoor', 'bowling_alley', 'boxing_ring', 'brewery_indoor',
+    'bridge', 'building_facade', 'bullring', 'burial_chamber', 'bus_interior',
+    'butchers_shop', 'butte', 'cabin_outdoor', 'cafeteria', 'campsite',
+    'campus', 'canal_natural', 'canal_urban', 'candy_store', 'canyon',
+    'car_interior_backseat', 'car_interior_frontseat', 'carrousel',
+    'casino_indoor', 'castle', 'catacomb', 'cathedral_indoor',
+    'cathedral_outdoor', 'cavern_indoor', 'cemetery', 'chalet',
+    'cheese_factory', 'chemistry_lab', 'chicken_coop_indoor',
+    'chicken_coop_outdoor', 'childs_room', 'church_indoor', 'church_outdoor',
+    'classroom', 'clean_room', 'cliff', 'cloister_indoor', 'closet',
+    'clothing_store', 'coast', 'cockpit', 'coffee_shop', 'computer_room',
+    'conference_center', 'conference_room', 'construction_site',
+    'control_room', 'control_tower_outdoor', 'corn_field', 'corral',
+    'corridor', 'cottage_garden', 'courthouse', 'courtroom', 'courtyard',
+    'covered_bridge_exterior', 'creek', 'crevasse', 'crosswalk',
+    'cubicle_office', 'dam', 'delicatessen', 'dentists_office', 'desert_sand',
+    'desert_vegetation', 'diner_indoor', 'diner_outdoor', 'dinette_home',
+    'dinette_vehicle', 'dining_car', 'dining_room', 'discotheque', 'dock',
+    'doorway_outdoor', 'dorm_room', 'driveway', 'driving_range_outdoor',
+    'drugstore', 'electrical_substation', 'elevator_door', 'elevator_interior',
+    'elevator_shaft', 'engine_room', 'escalator_indoor', 'excavation',
+    'factory_indoor', 'fairway', 'fastfood_restaurant', 'field_cultivated',
+    'field_wild', 'fire_escape', 'fire_station', 'firing_range_indoor',
+    'fishpond', 'florist_shop_indoor', 'food_court', 'forest_broadleaf',
+    'forest_needleleaf', 'forest_path', 'forest_road', 'formal_garden',
+    'fountain', 'galley', 'game_room', 'garage_indoor', 'garbage_dump',
+    'gas_station', 'gazebo_exterior', 'general_store_indoor',
+    'general_store_outdoor', 'gift_shop', 'golf_course', 'greenhouse_indoor',
+    'greenhouse_outdoor', 'gymnasium_indoor', 'hangar_indoor',
+    'hangar_outdoor', 'harbor', 'hayfield', 'heliport', 'herb_garden',
+    'highway', 'hill', 'home_office', 'hospital', 'hospital_room',
+    'hot_spring', 'hot_tub_outdoor', 'hotel_outdoor', 'hotel_room', 'house',
+    'hunting_lodge_outdoor', 'ice_cream_parlor', 'ice_floe', 'ice_shelf',
+    'ice_skating_rink_indoor', 'ice_skating_rink_outdoor', 'iceberg', 'igloo',
+    'industrial_area', 'inn_outdoor', 'islet', 'jacuzzi_indoor', 'jail_indoor',
+    'jail_cell', 'jewelry_shop', 'kasbah', 'kennel_indoor', 'kennel_outdoor',
+    'kindergarden_classroom', 'kitchen', 'kitchenette', 'labyrinth_outdoor',
+    'lake_natural', 'landfill', 'landing_deck', 'laundromat', 'lecture_room',
+    'library_indoor', 'library_outdoor', 'lido_deck_outdoor', 'lift_bridge',
+    'lighthouse', 'limousine_interior', 'living_room', 'lobby', 'lock_chamber',
+    'locker_room', 'mansion', 'manufactured_home', 'market_indoor',
+    'market_outdoor', 'marsh', 'martial_arts_gym', 'mausoleum', 'medina',
+    'moat_water', 'monastery_outdoor', 'mosque_indoor', 'mosque_outdoor',
+    'motel', 'mountain', 'mountain_snowy', 'movie_theater_indoor',
+    'museum_indoor', 'music_store', 'music_studio',
+    'nuclear_power_plant_outdoor', 'nursery', 'oast_house',
+    'observatory_outdoor', 'ocean', 'office', 'office_building',
+    'oil_refinery_outdoor', 'oilrig', 'operating_room', 'orchard',
+    'outhouse_outdoor', 'pagoda', 'palace', 'pantry', 'park',
+    'parking_garage_indoor', 'parking_garage_outdoor', 'parking_lot', 'parlor',
+    'pasture', 'patio', 'pavilion', 'pharmacy', 'phone_booth',
+    'physics_laboratory', 'picnic_area', 'pilothouse_indoor',
+    'planetarium_outdoor', 'playground', 'playroom', 'plaza', 'podium_indoor',
+    'podium_outdoor', 'pond', 'poolroom_establishment', 'poolroom_home',
+    'power_plant_outdoor', 'promenade_deck', 'pub_indoor', 'pulpit',
+    'putting_green', 'racecourse', 'raceway', 'raft', 'railroad_track',
+    'rainforest', 'reception', 'recreation_room', 'residential_neighborhood',
+    'restaurant', 'restaurant_kitchen', 'restaurant_patio', 'rice_paddy',
+    'riding_arena', 'river', 'rock_arch', 'rope_bridge', 'ruin', 'runway',
+    'sandbar', 'sandbox', 'sauna', 'schoolhouse', 'sea_cliff', 'server_room',
+    'shed', 'shoe_shop', 'shopfront', 'shopping_mall_indoor', 'shower',
+    'skatepark', 'ski_lodge', 'ski_resort', 'ski_slope', 'sky', 'skyscraper',
+    'slum', 'snowfield', 'squash_court', 'stable', 'stadium_baseball',
+    'stadium_football', 'stage_indoor', 'staircase', 'street',
+    'subway_interior', 'subway_station_platform', 'supermarket', 'sushi_bar',
+    'swamp', 'swimming_pool_indoor', 'swimming_pool_outdoor',
+    'synagogue_indoor', 'synagogue_outdoor', 'television_studio',
+    'temple_east_asia', 'temple_south_asia', 'tennis_court_indoor',
+    'tennis_court_outdoor', 'tent_outdoor', 'theater_indoor_procenium',
+    'theater_indoor_seats', 'thriftshop', 'throne_room', 'ticket_booth',
+    'toll_plaza', 'topiary_garden', 'tower', 'toyshop', 'track_outdoor',
+    'train_railway', 'train_station_platform', 'tree_farm', 'tree_house',
+    'trench', 'underwater_coral_reef', 'utility_room', 'valley',
+    'van_interior', 'vegetable_garden', 'veranda', 'veterinarians_office',
+    'viaduct', 'videostore', 'village', 'vineyard', 'volcano',
+    'volleyball_court_indoor', 'volleyball_court_outdoor', 'waiting_room',
+    'warehouse_indoor', 'water_tower', 'waterfall_block', 'waterfall_fan',
+    'waterfall_plunge', 'watering_hole', 'wave', 'wet_bar', 'wheat_field',
+    'wind_farm', 'windmill', 'wine_cellar_barrel_storage',
+    'wine_cellar_bottle_storage', 'wrestling_ring_indoor', 'yard',
+    'youth_hostel')
+
+CALTECH101_CATEGORIES = (
+    'BACKGROUND_Google', 'Faces', 'Faces_easy', 'Leopards', 'Motorbikes',
+    'accordion', 'airplanes', 'anchor', 'ant', 'barrel', 'bass', 'beaver',
+    'binocular', 'bonsai', 'brain', 'brontosaurus', 'buddha', 'butterfly',
+    'camera', 'cannon', 'car_side', 'ceiling_fan', 'cellphone', 'chair',
+    'chandelier', 'cougar_body', 'cougar_face', 'crab', 'crayfish',
+    'crocodile', 'crocodile_head', 'cup', 'dalmatian', 'dollar_bill',
+    'dolphin', 'dragonfly', 'electric_guitar', 'elephant', 'emu', 'euphonium',
+    'ewer', 'ferry', 'flamingo', 'flamingo_head', 'garfield', 'gerenuk',
+    'gramophone', 'grand_piano', 'hawksbill', 'headphone', 'hedgehog',
+    'helicopter', 'ibis', 'inline_skate', 'joshua_tree', 'kangaroo', 'ketch',
+    'lamp', 'laptop', 'llama', 'lobster', 'lotus', 'mandolin', 'mayfly',
+    'menorah', 'metronome', 'minaret', 'nautilus', 'octopus', 'okapi',
+    'pagoda', 'panda', 'pigeon', 'pizza', 'platypus', 'pyramid', 'revolver',
+    'rhino', 'rooster', 'saxophone', 'schooner', 'scissors', 'scorpion',
+    'sea_horse', 'snoopy', 'soccer_ball', 'stapler', 'starfish', 'stegosaurus',
+    'stop_sign', 'strawberry', 'sunflower', 'tick', 'trilobite', 'umbrella',
+    'watch', 'water_lilly', 'wheelchair', 'wild_cat', 'windsor_chair',
+    'wrench', 'yin_yang')
+
+FOOD101_CATEGORIES = (
+    'apple_pie', 'baby_back_ribs', 'baklava', 'beef_carpaccio', 'beef_tartare',
+    'beet_salad', 'beignets', 'bibimbap', 'bread_pudding', 'breakfast_burrito',
+    'bruschetta', 'caesar_salad', 'cannoli', 'caprese_salad', 'carrot_cake',
+    'ceviche', 'cheesecake', 'cheese_plate', 'chicken_curry',
+    'chicken_quesadilla', 'chicken_wings', 'chocolate_cake',
+    'chocolate_mousse', 'churros', 'clam_chowder', 'club_sandwich',
+    'crab_cakes', 'creme_brulee', 'croque_madame', 'cup_cakes', 'deviled_eggs',
+    'donuts', 'dumplings', 'edamame', 'eggs_benedict', 'escargots', 'falafel',
+    'filet_mignon', 'fish_and_chips', 'foie_gras', 'french_fries',
+    'french_onion_soup', 'french_toast', 'fried_calamari', 'fried_rice',
+    'frozen_yogurt', 'garlic_bread', 'gnocchi', 'greek_salad',
+    'grilled_cheese_sandwich', 'grilled_salmon', 'guacamole', 'gyoza',
+    'hamburger', 'hot_and_sour_soup', 'hot_dog', 'huevos_rancheros', 'hummus',
+    'ice_cream', 'lasagna', 'lobster_bisque', 'lobster_roll_sandwich',
+    'macaroni_and_cheese', 'macarons', 'miso_soup', 'mussels', 'nachos',
+    'omelette', 'onion_rings', 'oysters', 'pad_thai', 'paella', 'pancakes',
+    'panna_cotta', 'peking_duck', 'pho', 'pizza', 'pork_chop', 'poutine',
+    'prime_rib', 'pulled_pork_sandwich', 'ramen', 'ravioli', 'red_velvet_cake',
+    'risotto', 'samosa', 'sashimi', 'scallops', 'seaweed_salad',
+    'shrimp_and_grits', 'spaghetti_bolognese', 'spaghetti_carbonara',
+    'spring_rolls', 'steak', 'strawberry_shortcake', 'sushi', 'tacos',
+    'takoyaki', 'tiramisu', 'tuna_tartare', 'waffles')
+
+CIFAR100_CATEGORIES_CN = (
+    '苹果', '水族馆鱼', '婴儿', '熊', '河狸', '床', '蜜蜂', '甲虫', '自行车', '瓶子', '碗', '小男孩',
+    '桥', '公共汽车', '蝴蝶', '骆驼', '易拉罐', '城堡', '毛毛虫', '牛', '椅子', '猩猩', '钟', '白云',
+    '蟑螂', '沙发', '螃蟹', '鳄鱼', '杯子', '恐龙', '海豚', '大象', '比目鱼', '森林', '狐狸', '小女孩',
+    '仓鼠', '屋子', '袋鼠', '键盘', '台灯', '割草机', '猎豹', '狮子', '蜥蜴', '龙虾', '男人', '枫树',
+    '摩托车', '山', '老鼠', '蘑菇', '橡树', '橙子橘子', '兰花', '水獭', '棕榈树', '梨', '皮卡车', '松树',
+    '田野', '盘子', '罂粟', '豪猪', '负鼠', '兔子', '浣熊', '鳐鱼', '公路', '火箭', '玫瑰', '大海',
+    '海豹', '鲨鱼', '尖嘴小鼠', '臭鼬', '摩天大楼', '蜗牛', '蛇', '蜘蛛', '松鼠', '电车', '向日葵', '甜椒',
+    '桌子', '坦克', '电话', '电视', '老虎', '拖拉机', '火车', '鳟鱼', '郁金香', '乌龟', '衣柜', '鲸鱼',
+    '柳树', '狼', '女人', '蠕虫')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/cifar.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/cifar.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pickle
 from typing import List, Optional
 
 import mmengine.dist as dist
 import numpy as np
 from mmengine.fileio import (LocalBackend, exists, get, get_file_backend,
                              join_path)
+from mmengine.logging import MMLogger
 
 from mmpretrain.registry import DATASETS
 from .base_dataset import BaseDataset
 from .categories import CIFAR10_CATEGORIES, CIFAR100_CATEGORIES
 from .utils import check_md5, download_and_extract_archive
 
 
@@ -17,21 +18,19 @@
 class CIFAR10(BaseDataset):
     """`CIFAR10 <https://www.cs.toronto.edu/~kriz/cifar.html>`_ Dataset.
 
     This implementation is modified from
     https://github.com/pytorch/vision/blob/master/torchvision/datasets/cifar.py
 
     Args:
-        data_prefix (str): Prefix for data.
-        test_mode (bool): ``test_mode=True`` means in test phase.
-            It determines to use the training set or test set.
+        data_root (str): The root directory of the CIFAR Dataset.
+        split (str, optional): The dataset split, supports "train" and "test".
+            Default to "train".
         metainfo (dict, optional): Meta information for dataset, such as
             categories information. Defaults to None.
-        data_root (str): The root directory for ``data_prefix``.
-            Defaults to ''.
         download (bool): Whether to download the dataset if not exists.
             Defaults to True.
         **kwargs: Other keyword arguments in :class:`BaseDataset`.
     """  # noqa: E501
 
     base_folder = 'cifar-10-batches-py'
     url = 'https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz'
@@ -52,20 +51,37 @@
         'filename': 'batches.meta',
         'key': 'label_names',
         'md5': '5ff9c542aee3614f3951f8cda6e48888',
     }
     METAINFO = {'classes': CIFAR10_CATEGORIES}
 
     def __init__(self,
-                 data_prefix: str,
-                 test_mode: bool,
-                 metainfo: Optional[dict] = None,
                  data_root: str = '',
+                 split: str = 'train',
+                 metainfo: Optional[dict] = None,
                  download: bool = True,
+                 data_prefix: str = '',
+                 test_mode: bool = False,
                  **kwargs):
+
+        splits = ['train', 'test']
+        assert split in splits, \
+            f"The split must be one of {splits}, but get '{split}'"
+        self.split = split
+
+        # To handle the BC-breaking
+        if split == 'train' and test_mode:
+            logger = MMLogger.get_current_instance()
+            logger.warning('split="train" but test_mode=True. '
+                           'The training set will be used.')
+
+        if not data_root and not data_prefix:
+            raise RuntimeError('Please set ``data_root`` to'
+                               'specify the dataset path')
+
         self.download = download
         super().__init__(
             # The CIFAR dataset doesn't need specify annotation file
             ann_file='',
             metainfo=metainfo,
             data_root=data_root,
             data_prefix=dict(root=data_prefix),
@@ -92,15 +108,15 @@
                     '`download=True` to download automatically.')
 
         dist.barrier()
         assert self._check_integrity(), \
             'Download failed or shared storage is unavailable. Please ' \
             f'download the dataset manually through {self.url}.'
 
-        if not self.test_mode:
+        if self.split == 'train':
             downloaded_list = self.train_list
         else:
             downloaded_list = self.test_list
 
         imgs = []
         gt_labels = []
 
@@ -161,21 +177,19 @@
 
 
 @DATASETS.register_module()
 class CIFAR100(CIFAR10):
     """`CIFAR100 <https://www.cs.toronto.edu/~kriz/cifar.html>`_ Dataset.
 
     Args:
-        data_prefix (str): Prefix for data.
-        test_mode (bool): ``test_mode=True`` means in test phase.
-            It determines to use the training set or test set.
+        data_root (str): The root directory of the CIFAR Dataset.
+        split (str, optional): The dataset split, supports "train" and "test".
+            Default to "train".
         metainfo (dict, optional): Meta information for dataset, such as
             categories information. Defaults to None.
-        data_root (str): The root directory for ``data_prefix``.
-            Defaults to ''.
         download (bool): Whether to download the dataset if not exists.
             Defaults to True.
         **kwargs: Other keyword arguments in :class:`BaseDataset`.
     """
 
     base_folder = 'cifar-100-python'
     url = 'https://www.cs.toronto.edu/~kriz/cifar-100-python.tar.gz'
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/cub.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/cub.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from typing import List
 
 from mmengine import get_file_backend, list_from_file
+from mmengine.logging import MMLogger
 
 from mmpretrain.registry import DATASETS
 from .base_dataset import BaseDataset
 from .categories import CUB_CATEGORIES
 
 
 @DATASETS.register_module()
@@ -15,73 +16,75 @@
     Support the `CUB-200-2011 <http://www.vision.caltech.edu/visipedia/CUB-200-2011.html>`_ Dataset.
     Comparing with the `CUB-200 <http://www.vision.caltech.edu/visipedia/CUB-200.html>`_ Dataset,
     there are much more pictures in `CUB-200-2011`. After downloading and decompression, the dataset
     directory structure is as follows.
 
     CUB dataset directory: ::
 
-        CUB-200-2011 (data_root)/
-        ├── images (data_prefix)
+        CUB_200_2011
+        ├── images
         │   ├── class_x
         │   │   ├── xx1.jpg
         │   │   ├── xx2.jpg
         │   │   └── ...
         │   ├── class_y
         │   │   ├── yy1.jpg
         │   │   ├── yy2.jpg
         │   │   └── ...
         │   └── ...
-        ├── images.txt (ann_file)
-        ├── image_class_labels.txt (image_class_labels_file)
-        ├── train_test_split.txt (train_test_split_file)
+        ├── images.txt
+        ├── image_class_labels.txt
+        ├── train_test_split.txt
         └── ....
 
     Args:
         data_root (str): The root directory for CUB-200-2011 dataset.
-        test_mode (bool): ``test_mode=True`` means in test phase. It determines
-             to use the training set or test set.
-        ann_file (str, optional): Annotation file path, path relative to
-            ``data_root``. Defaults to 'images.txt'.
-        data_prefix (str): Prefix for iamges, path relative to
-            ``data_root``. Defaults to 'images'.
-        image_class_labels_file (str, optional): The label file, path
-            relative to ``data_root``. Defaults to 'image_class_labels.txt'.
-        train_test_split_file (str, optional): The split file  to split train
-            and test dataset, path relative to ``data_root``.
-            Defaults to 'train_test_split_file.txt'.
-
+        split (str, optional): The dataset split, supports "train" and "test".
+            Default to "train".
 
     Examples:
         >>> from mmpretrain.datasets import CUB
-        >>> cub_train_cfg = dict(data_root='data/CUB_200_2011', test_mode=True)
-        >>> cub_train = CUB(**cub_train_cfg)
-        >>> cub_train
+        >>> train_dataset = CUB(data_root='data/CUB_200_2011', split='train')
+        >>> train_dataset
         Dataset CUB
-        Number of samples:  5994
-        Number of categories:       200
-        Root of dataset:    data/CUB_200_2011
-        >>> cub_test_cfg = dict(data_root='data/CUB_200_2011', test_mode=True)
-        >>> cub_test = CUB(**cub_test_cfg)
-        >>> cub_test
+            Number of samples:  5994
+            Number of categories:       200
+            Root of dataset:    data/CUB_200_2011
+        >>> test_dataset = CUB(data_root='data/CUB_200_2011', split='test')
+        >>> test_dataset
         Dataset CUB
-        Number of samples:  5794
-        Number of categories:       200
-        Root of dataset:    data/CUB_200_2011
+            Number of samples:  5794
+            Number of categories:       200
+            Root of dataset:    data/CUB_200_2011
     """  # noqa: E501
 
     METAINFO = {'classes': CUB_CATEGORIES}
 
     def __init__(self,
                  data_root: str,
-                 test_mode: bool,
-                 ann_file: str = 'images.txt',
-                 data_prefix: str = 'images',
-                 image_class_labels_file: str = 'image_class_labels.txt',
-                 train_test_split_file: str = 'train_test_split.txt',
+                 split: str = 'train',
+                 test_mode: bool = False,
                  **kwargs):
+
+        splits = ['train', 'test']
+        assert split in splits, \
+            f"The split must be one of {splits}, but get '{split}'"
+        self.split = split
+
+        # To handle the BC-breaking
+        if split == 'train' and test_mode:
+            logger = MMLogger.get_current_instance()
+            logger.warning('split="train" but test_mode=True. '
+                           'The training set will be used.')
+
+        ann_file = 'images.txt'
+        data_prefix = 'images'
+        image_class_labels_file = 'image_class_labels.txt'
+        train_test_split_file = 'train_test_split.txt'
+
         self.backend = get_file_backend(data_root, enable_singleton=True)
         self.image_class_labels_file = self.backend.join_path(
             data_root, image_class_labels_file)
         self.train_test_split_file = self.backend.join_path(
             data_root, train_test_split_file)
         super(CUB, self).__init__(
             ann_file=ann_file,
@@ -112,19 +115,19 @@
 
         assert sample_dict.keys() == label_dict.keys() == split_dict.keys(),\
             f'sample_ids should be same in files {self.ann_file}, ' \
             f'{self.image_class_labels_file} and {self.train_test_split_file}'
 
         data_list = []
         for sample_id in sample_dict.keys():
-            if split_dict[sample_id] == '1' and self.test_mode:
-                # skip train samples when test_mode=True
+            if split_dict[sample_id] == '1' and self.split == 'test':
+                # skip train samples when split='test'
                 continue
-            elif split_dict[sample_id] == '0' and not self.test_mode:
-                # skip test samples when test_mode=False
+            elif split_dict[sample_id] == '0' and self.split == 'train':
+                # skip test samples when split='train'
                 continue
 
             img_path = self.backend.join_path(self.img_prefix,
                                               sample_dict[sample_id])
             gt_label = int(label_dict[sample_id]) - 1
             info = dict(img_path=img_path, gt_label=gt_label)
             data_list.append(info)
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/custom.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/dataset_wrappers.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/imagenet.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/imagenet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/inshop.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/inshop.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/mnist.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/multi_label.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/multi_label.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,35 +8,32 @@
 @DATASETS.register_module()
 class MultiLabelDataset(BaseDataset):
     """Multi-label Dataset.
 
     This dataset support annotation file in `OpenMMLab 2.0 style annotation
     format`.
 
-    .. _OpenMMLab 2.0 style annotation format:
-        https://github.com/open-mmlab/mmengine/blob/main/docs/zh_cn/tutorials/basedataset.md
-
     The annotation format is shown as follows.
 
     .. code-block:: none
 
         {
             "metainfo":
             {
               "classes":['A', 'B', 'C'....]
             },
             "data_list":
             [
               {
                 "img_path": "test_img1.jpg",
-                'img_label': [0, 1],
+                'gt_label': [0, 1],
               },
               {
                 "img_path": "test_img2.jpg",
-                'img_label': [2],
+                'gt_label': [2],
               },
             ]
             ....
         }
 
 
     Args:
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/multi_task.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/multi_task.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/places205.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/places205.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/samplers/repeat_aug.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/samplers/repeat_aug.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 
 from mmpretrain.registry import TRANSFORMS
 from .auto_augment import (AutoAugment, AutoContrast, BaseAugTransform,
                            Brightness, ColorTransform, Contrast, Cutout,
                            Equalize, GaussianBlur, Invert, Posterize,
                            RandAugment, Rotate, Sharpness, Shear, Solarize,
                            SolarizeAdd, Translate)
-from .formatting import (Collect, PackInputs, PackMultiTaskInputs, ToNumpy,
-                         ToPIL, Transpose)
-from .processing import (Albumentations, BEiTMaskGenerator, ColorJitter,
-                         EfficientNetCenterCrop, EfficientNetRandomCrop,
-                         Lighting, RandomCrop, RandomErasing,
-                         RandomResizedCrop, ResizeEdge, SimMIMMaskGenerator)
-from .wrappers import MultiView
+from .formatting import (Collect, NumpyToPIL, PackInputs, PackMultiTaskInputs,
+                         PILToNumpy, Transpose)
+from .processing import (Albumentations, BEiTMaskGenerator, CleanCaption,
+                         ColorJitter, EfficientNetCenterCrop,
+                         EfficientNetRandomCrop, Lighting, RandomCrop,
+                         RandomErasing, RandomResizedCrop, RandomTranslatePad,
+                         ResizeEdge, SimMIMMaskGenerator)
+from .wrappers import ApplyToList, MultiView
 
 for t in (CenterCrop, LoadImageFromFile, Normalize, RandomFlip,
           RandomGrayscale, RandomResize, Resize):
     TRANSFORMS.register_module(module=t)
 
 __all__ = [
-    'ToPIL', 'ToNumpy', 'Transpose', 'Collect', 'RandomCrop',
+    'NumpyToPIL', 'PILToNumpy', 'Transpose', 'Collect', 'RandomCrop',
     'RandomResizedCrop', 'Shear', 'Translate', 'Rotate', 'Invert',
     'ColorTransform', 'Solarize', 'Posterize', 'AutoContrast', 'Equalize',
     'Contrast', 'Brightness', 'Sharpness', 'AutoAugment', 'SolarizeAdd',
     'Cutout', 'RandAugment', 'Lighting', 'ColorJitter', 'RandomErasing',
     'PackInputs', 'Albumentations', 'EfficientNetRandomCrop',
     'EfficientNetCenterCrop', 'ResizeEdge', 'BaseAugTransform',
     'PackMultiTaskInputs', 'GaussianBlur', 'BEiTMaskGenerator',
     'SimMIMMaskGenerator', 'CenterCrop', 'LoadImageFromFile', 'Normalize',
-    'RandomFlip', 'RandomGrayscale', 'RandomResize', 'Resize', 'MultiView'
+    'RandomFlip', 'RandomGrayscale', 'RandomResize', 'Resize', 'MultiView',
+    'ApplyToList', 'CleanCaption', 'RandomTranslatePad'
 ]
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/auto_augment.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/auto_augment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1230,8 +1230,15 @@
         dict(type='Brightness', magnitude_range=(0, 0.9)),
         dict(type='Sharpness', magnitude_range=(0, 0.9)),
         dict(type='Shear', magnitude_range=(0, 0.3), direction='horizontal'),
         dict(type='Shear', magnitude_range=(0, 0.3), direction='vertical'),
         dict(type='Translate', magnitude_range=(0, 0.45), direction='horizontal'),
         dict(type='Translate', magnitude_range=(0, 0.45), direction='vertical'),
     ],
+    'simple_increasing': [
+        dict(type='AutoContrast'),
+        dict(type='Equalize'),
+        dict(type='Rotate', magnitude_range=(0, 30)),
+        dict(type='Shear', magnitude_range=(0, 0.3), direction='horizontal'),
+        dict(type='Shear', magnitude_range=(0, 0.3), direction='vertical'),
+    ],
 }
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/formatting.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/formatting.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from collections import defaultdict
 from collections.abc import Sequence
 
+import cv2
 import numpy as np
 import torch
 import torchvision.transforms.functional as F
 from mmcv.transforms import BaseTransform
 from mmengine.utils import is_str
 from PIL import Image
 
@@ -124,14 +125,15 @@
         elif not isinstance(input_, torch.Tensor):
             raise TypeError(f'Unsupported input type {type(input_)}.')
 
         return input_
 
     def transform(self, results: dict) -> dict:
         """Method to pack the input data."""
+
         packed_results = dict()
         if self.input_key in results:
             input_ = results[self.input_key]
             packed_results['inputs'] = self.format_input(input_)
 
         data_sample = DataSample()
 
@@ -252,63 +254,78 @@
         return results
 
     def __repr__(self):
         return self.__class__.__name__ + \
             f'(keys={self.keys}, order={self.order})'
 
 
-@TRANSFORMS.register_module()
-class ToPIL(BaseTransform):
+@TRANSFORMS.register_module(('NumpyToPIL', 'ToPIL'))
+class NumpyToPIL(BaseTransform):
     """Convert the image from OpenCV format to :obj:`PIL.Image.Image`.
 
     **Required Keys:**
 
-    - img
+    - ``img``
 
     **Modified Keys:**
 
-    - img
+    - ``img``
+
+    Args:
+        to_rgb (bool): Whether to convert img to rgb. Defaults to True.
     """
 
-    def transform(self, results):
+    def __init__(self, to_rgb: bool = False) -> None:
+        self.to_rgb = to_rgb
+
+    def transform(self, results: dict) -> dict:
         """Method to convert images to :obj:`PIL.Image.Image`."""
-        results['img'] = Image.fromarray(results['img'])
+        img = results['img']
+        img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB) if self.to_rgb else img
+
+        results['img'] = Image.fromarray(img)
         return results
 
+    def __repr__(self) -> str:
+        return self.__class__.__name__ + f'(to_rgb={self.to_rgb})'
+
 
-@TRANSFORMS.register_module()
-class ToNumpy(BaseTransform):
-    """Convert object to :obj:`numpy.ndarray`.
+@TRANSFORMS.register_module(('PILToNumpy', 'ToNumpy'))
+class PILToNumpy(BaseTransform):
+    """Convert img to :obj:`numpy.ndarray`.
 
     **Required Keys:**
 
-    - ``*keys**``
+    - ``img``
 
     **Modified Keys:**
 
-    - ``*keys**``
+    - ``img``
 
     Args:
+        to_bgr (bool): Whether to convert img to rgb. Defaults to True.
         dtype (str, optional): The dtype of the converted numpy array.
             Defaults to None.
     """
 
-    def __init__(self, keys, dtype=None):
-        self.keys = keys
+    def __init__(self, to_bgr: bool = False, dtype=None) -> None:
+        self.to_bgr = to_bgr
         self.dtype = dtype
 
-    def transform(self, results):
-        """Method to convert object to :obj:`numpy.ndarray`."""
-        for key in self.keys:
-            results[key] = np.array(results[key], dtype=self.dtype)
+    def transform(self, results: dict) -> dict:
+        """Method to convert img to :obj:`numpy.ndarray`."""
+        img = np.array(results['img'], dtype=self.dtype)
+        img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR) if self.to_bgr else img
+
+        results['img'] = img
         return results
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.__class__.__name__ + \
-            f'(keys={self.keys}, dtype={self.dtype})'
+            f'(to_bgr={self.to_bgr}, dtype={self.dtype})'
 
 
 @TRANSFORMS.register_module()
 class Collect(BaseTransform):
     """Collect and only reserve the specified fields.
 
     **Required Keys:**
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/transforms/processing.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/transforms/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,120 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import inspect
 import math
 import numbers
+import re
+import string
+import traceback
+from enum import EnumMeta
 from numbers import Number
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import mmcv
 import mmengine
 import numpy as np
+import torchvision
 from mmcv.transforms import BaseTransform
 from mmcv.transforms.utils import cache_randomness
+from torchvision.transforms.transforms import InterpolationMode
 
 from mmpretrain.registry import TRANSFORMS
 
 try:
     import albumentations
 except ImportError:
     albumentations = None
 
 
+def _str_to_torch_dtype(t: str):
+    """mapping str format dtype to torch.dtype."""
+    import torch  # noqa: F401,F403
+    return eval(f'torch.{t}')
+
+
+def _interpolation_modes_from_str(t: str):
+    """mapping str format to Interpolation."""
+    t = t.lower()
+    inverse_modes_mapping = {
+        'nearest': InterpolationMode.NEAREST,
+        'bilinear': InterpolationMode.BILINEAR,
+        'bicubic': InterpolationMode.BICUBIC,
+        'box': InterpolationMode.BOX,
+        'hammimg': InterpolationMode.HAMMING,
+        'lanczos': InterpolationMode.LANCZOS,
+    }
+    return inverse_modes_mapping[t]
+
+
+def _warpper_vision_transform_cls(vision_transform_cls, new_name):
+    """build a transform warpper class for specific torchvison.transform to
+    handle the different input type between torchvison.transforms with
+    mmcls.datasets.transforms."""
+
+    def new_init(self, *args, **kwargs):
+        if 'interpolation' in kwargs and isinstance(kwargs['interpolation'],
+                                                    str):
+            kwargs['interpolation'] = _interpolation_modes_from_str(
+                kwargs['interpolation'])
+        if 'dtype' in kwargs and isinstance(kwargs['dtype'], str):
+            kwargs['dtype'] = _str_to_torch_dtype(kwargs['dtype'])
+
+        try:
+            self.t = vision_transform_cls(*args, **kwargs)
+        except TypeError as e:
+            traceback.print_exc()
+            raise TypeError(
+                f'Error when init the {vision_transform_cls}, please '
+                f'check the argmemnts of {args} and {kwargs}. \n{e}')
+
+    def new_call(self, input):
+        try:
+            input['img'] = self.t(input['img'])
+        except Exception as e:
+            traceback.print_exc()
+            raise Exception('Error when processing of transform(`torhcvison/'
+                            f'{vision_transform_cls.__name__}`). \n{e}')
+        return input
+
+    def new_str(self):
+        return str(self.t)
+
+    new_transforms_cls = type(
+        new_name, (),
+        dict(__init__=new_init, __call__=new_call, __str__=new_str))
+    return new_transforms_cls
+
+
+def register_vision_transforms() -> List[str]:
+    """Register transforms in ``torchvision.transforms`` to the ``TRANSFORMS``
+    registry.
+
+    Returns:
+        List[str]: A list of registered transforms' name.
+    """
+    vision_transforms = []
+    for module_name in dir(torchvision.transforms):
+        if not re.match('[A-Z]', module_name):
+            # must startswith a capital letter
+            continue
+        _transform = getattr(torchvision.transforms, module_name)
+        if inspect.isclass(_transform) and callable(
+                _transform) and not isinstance(_transform, (EnumMeta)):
+            new_cls = _warpper_vision_transform_cls(
+                _transform, f'TorchVison{module_name}')
+            TRANSFORMS.register_module(
+                module=new_cls, name=f'torchvision/{module_name}')
+            vision_transforms.append(f'torchvision/{module_name}')
+    return vision_transforms
+
+
+# register all the transforms in torchvision by using a transform wrapper
+VISION_TRANSFORMS = register_vision_transforms()
+
+
 @TRANSFORMS.register_module()
 class RandomCrop(BaseTransform):
     """Crop the given Image at a random location.
 
     **Required Keys:**
 
     - img
@@ -1529,7 +1621,142 @@
         repr_str += f'(size={self.size}, '
         repr_str += f'second_size={self.second_size}, '
         repr_str += f'interpolation={self.interpolation}, '
         repr_str += f'second_interpolation={self.second_interpolation}, '
         repr_str += f'scale={self.scale}, '
         repr_str += f'ratio={self.ratio})'
         return repr_str
+
+
+@TRANSFORMS.register_module()
+class CleanCaption(BaseTransform):
+    """Clean caption text.
+
+    Remove some useless punctuation for the caption task.
+
+    **Required Keys:**
+
+    - ``*keys``
+
+    **Modified Keys:**
+
+    - ``*keys``
+
+    Args:
+        keys (Sequence[str], optional): The keys of text to be cleaned.
+            Defaults to 'gt_caption'.
+        remove_chars (str): The characters to be removed. Defaults to
+            :py:attr:`string.punctuation`.
+        lowercase (bool): Whether to convert the text to lowercase.
+            Defaults to True.
+        remove_dup_space (bool): Whether to remove duplicated whitespaces.
+            Defaults to True.
+        strip (bool): Whether to remove leading and trailing whitespaces.
+            Defaults to True.
+    """
+
+    def __init__(
+        self,
+        keys='gt_caption',
+        remove_chars=string.punctuation,
+        lowercase=True,
+        remove_dup_space=True,
+        strip=True,
+    ):
+        if isinstance(keys, str):
+            keys = [keys]
+        self.keys = keys
+        self.transtab = str.maketrans({ch: None for ch in remove_chars})
+        self.lowercase = lowercase
+        self.remove_dup_space = remove_dup_space
+        self.strip = strip
+
+    def _clean(self, text):
+        """Perform text cleaning before tokenizer."""
+
+        if self.strip:
+            text = text.strip()
+
+        text = text.translate(self.transtab)
+
+        if self.remove_dup_space:
+            text = re.sub(r'\s{2,}', ' ', text)
+
+        if self.lowercase:
+            text = text.lower()
+
+        return text
+
+    def clean(self, text):
+        """Perform text cleaning before tokenizer."""
+        if isinstance(text, (list, tuple)):
+            return [self._clean(item) for item in text]
+        elif isinstance(text, str):
+            return self._clean(text)
+        else:
+            raise TypeError('text must be a string or a list of strings')
+
+    def transform(self, results: dict) -> dict:
+        """Method to clean the input text data."""
+        for key in self.keys:
+            results[key] = self.clean(results[key])
+        return results
+
+
+@TRANSFORMS.register_module()
+class OFAAddObjects(BaseTransform):
+
+    def transform(self, results: dict) -> dict:
+        if 'objects' not in results:
+            raise ValueError(
+                'Some OFA fine-tuned models requires `objects` field in the '
+                'dataset, which is generated by VinVL. Or please use '
+                'zero-shot configs. See '
+                'https://github.com/OFA-Sys/OFA/issues/189')
+
+        if 'question' in results:
+            prompt = '{} object: {}'.format(
+                results['question'],
+                ' '.join(results['objects']),
+            )
+            results['decoder_prompt'] = prompt
+            results['question'] = prompt
+
+
+@TRANSFORMS.register_module()
+class RandomTranslatePad(BaseTransform):
+
+    def __init__(self, size=640, aug_translate=False):
+        self.size = size
+        self.aug_translate = aug_translate
+
+    @cache_randomness
+    def rand_translate_params(self, dh, dw):
+        top = np.random.randint(0, dh)
+        left = np.random.randint(0, dw)
+        return top, left
+
+    def transform(self, results: dict) -> dict:
+        img = results['img']
+        h, w = img.shape[:-1]
+        dw = self.size - w
+        dh = self.size - h
+        if self.aug_translate:
+            top, left = self.rand_translate_params(dh, dw)
+        else:
+            top = round(dh / 2.0 - 0.1)
+            left = round(dw / 2.0 - 0.1)
+
+        out_img = np.zeros((self.size, self.size, 3), dtype=np.float32)
+        out_img[top:top + h, left:left + w, :] = img
+        results['img'] = out_img
+        results['img_shape'] = (self.size, self.size)
+
+        # translate box
+        if 'gt_bboxes' in results.keys():
+            for i in range(len(results['gt_bboxes'])):
+                box = results['gt_bboxes'][i]
+                box[0], box[2] = box[0] + left, box[2] + left
+                box[1], box[3] = box[1] + top, box[3] + top
+                results['gt_bboxes'][i] = box
+
+        return results
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/utils.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/datasets/voc.py` & `mmpretrain-1.0.0rc8/mmpretrain/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .margin_head_hooks import SetAdaptiveMarginsHook
 from .precise_bn_hook import PreciseBNHook
 from .retriever_hooks import PrepareProtoBeforeValLoopHook
 from .simsiam_hook import SimSiamHook
 from .swav_hook import SwAVHook
 from .switch_recipe_hook import SwitchRecipeHook
 from .visualization_hook import VisualizationHook
+from .warmup_param_hook import WarmupParamHook
 
 __all__ = [
     'ClassNumCheckHook', 'PreciseBNHook', 'VisualizationHook',
     'SwitchRecipeHook', 'PrepareProtoBeforeValLoopHook',
     'SetAdaptiveMarginsHook', 'EMAHook', 'SimSiamHook', 'DenseCLHook',
-    'SwAVHook'
+    'SwAVHook', 'WarmupParamHook'
 ]
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/class_num_check_hook.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/class_num_check_hook.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/densecl_hook.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/densecl_hook.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/ema_hook.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/margin_head_hooks.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/margin_head_hooks.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/precise_bn_hook.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/precise_bn_hook.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/retriever_hooks.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/retriever_hooks.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/simsiam_hook.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/simsiam_hook.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/swav_hook.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/swav_hook.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/switch_recipe_hook.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/switch_recipe_hook.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/hooks/visualization_hook.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/hooks/visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/adan_t.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/adan_t.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/lamb.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/lamb.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/lars.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/engine/optimizers/layer_decay_optim_wrapper_constructor.py` & `mmpretrain-1.0.0rc8/mmpretrain/engine/optimizers/layer_decay_optim_wrapper_constructor.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/multi_label.py` & `mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/multi_label.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/multi_task.py` & `mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/multi_task.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/retrieval.py` & `mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/retrieval.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/single_label.py` & `mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/single_label.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/evaluation/metrics/voc_multi_label.py` & `mmpretrain-1.0.0rc8/mmpretrain/evaluation/metrics/voc_multi_label.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .backbones import *  # noqa: F401,F403
 from .builder import (BACKBONES, CLASSIFIERS, HEADS, LOSSES, NECKS,
                       build_backbone, build_classifier, build_head, build_loss,
                       build_neck)
 from .classifiers import *  # noqa: F401,F403
 from .heads import *  # noqa: F401,F403
 from .losses import *  # noqa: F401,F403
+from .multimodal import *  # noqa: F401,F403
 from .necks import *  # noqa: F401,F403
 from .retrievers import *  # noqa: F401,F403
 from .selfsup import *  # noqa: F401,F403
 from .tta import *  # noqa: F401,F403
 from .utils import *  # noqa: F401,F403
 
 __all__ = [
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 from .tinyvit import TinyViT
 from .tnt import TNT
 from .twins import PCPVT, SVT
 from .van import VAN
 from .vgg import VGG
 from .vig import PyramidVig, Vig
 from .vision_transformer import VisionTransformer
+from .vit_eva02 import ViTEVA02
+from .vit_sam import ViTSAM
 from .xcit import XCiT
 
 __all__ = [
     'LeNet5',
     'AlexNet',
     'VGG',
     'RegNet',
@@ -112,8 +114,10 @@
     'RevVisionTransformer',
     'MixMIMTransformer',
     'TinyViT',
     'LeViT',
     'Vig',
     'PyramidVig',
     'XCiT',
+    'ViTSAM',
+    'ViTEVA02',
 ]
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/alexnet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/alexnet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/base_backbone.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/base_backbone.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/beit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/conformer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/conformer.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/convmixer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/convmixer.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/convnext.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/convnext.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/cspnet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/cspnet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/davit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/davit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/deit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/deit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/deit3.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/deit3.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/densenet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/densenet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/edgenext.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/edgenext.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/efficientformer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/efficientformer.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/efficientnet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/efficientnet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/efficientnet_v2.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/hornet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/hornet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/hrnet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/inception_v3.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/inception_v3.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/lenet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/lenet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/levit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/levit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mixmim.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mixmim.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mlp_mixer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mlp_mixer.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mobilenet_v2.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mobilenet_v3.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mobileone.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mobileone.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mobilevit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mobilevit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/mvit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/mvit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/poolformer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/poolformer.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/regnet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/regnet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/replknet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/replknet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/repmlp.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/repmlp.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/repvgg.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/repvgg.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/res2net.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/res2net.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,30 +139,39 @@
             downsampling in the bottle2neck. Defaults to True.
         conv_cfg (dict): dictionary to construct and config conv layer.
             Default: None
         norm_cfg (dict): dictionary to construct and config norm layer.
             Default: dict(type='BN')
         scales (int): Scales used in Res2Net. Default: 4
         base_width (int): Basic width of each scale. Default: 26
+        drop_path_rate (float or np.ndarray): stochastic depth rate.
+            Default: 0.
     """
 
     def __init__(self,
                  block,
                  in_channels,
                  out_channels,
                  num_blocks,
                  stride=1,
                  avg_down=True,
                  conv_cfg=None,
                  norm_cfg=dict(type='BN'),
                  scales=4,
                  base_width=26,
+                 drop_path_rate=0.0,
                  **kwargs):
         self.block = block
 
+        if isinstance(drop_path_rate, float):
+            drop_path_rate = [drop_path_rate] * num_blocks
+
+        assert len(drop_path_rate
+                   ) == num_blocks, 'Please check the length of drop_path_rate'
+
         downsample = None
         if stride != 1 or in_channels != out_channels:
             if avg_down:
                 downsample = nn.Sequential(
                     nn.AvgPool2d(
                         kernel_size=stride,
                         stride=stride,
@@ -197,26 +206,28 @@
                 stride=stride,
                 downsample=downsample,
                 conv_cfg=conv_cfg,
                 norm_cfg=norm_cfg,
                 scales=scales,
                 base_width=base_width,
                 stage_type='stage',
+                drop_path_rate=drop_path_rate[0],
                 **kwargs))
         in_channels = out_channels
-        for _ in range(1, num_blocks):
+        for i in range(1, num_blocks):
             layers.append(
                 block(
                     in_channels=in_channels,
                     out_channels=out_channels,
                     stride=1,
                     conv_cfg=conv_cfg,
                     norm_cfg=norm_cfg,
                     scales=scales,
                     base_width=base_width,
+                    drop_path_rate=drop_path_rate[i],
                     **kwargs))
         super(Res2Layer, self).__init__(*layers)
 
 
 @MODELS.register_module()
 class Res2Net(ResNet):
     """Res2Net backbone.
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/resnest.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/resnet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/resnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-
+import torch
 import torch.nn as nn
 import torch.utils.checkpoint as cp
 from mmcv.cnn import (ConvModule, build_activation_layer, build_conv_layer,
                       build_norm_layer)
 from mmcv.cnn.bricks import DropPath
 from mmengine.model import BaseModule
 from mmengine.model.weight_init import constant_init
@@ -330,30 +330,39 @@
         stride (int): stride of the first block. Default: 1.
         avg_down (bool): Use AvgPool instead of stride conv when
             downsampling in the bottleneck. Default: False
         conv_cfg (dict, optional): dictionary to construct and config conv
             layer. Default: None
         norm_cfg (dict): dictionary to construct and config norm layer.
             Default: dict(type='BN')
+        drop_path_rate (float or list): stochastic depth rate.
+            Default: 0.
     """
 
     def __init__(self,
                  block,
                  num_blocks,
                  in_channels,
                  out_channels,
                  expansion=None,
                  stride=1,
                  avg_down=False,
                  conv_cfg=None,
                  norm_cfg=dict(type='BN'),
+                 drop_path_rate=0.0,
                  **kwargs):
         self.block = block
         self.expansion = get_expansion(block, expansion)
 
+        if isinstance(drop_path_rate, float):
+            drop_path_rate = [drop_path_rate] * num_blocks
+
+        assert len(drop_path_rate
+                   ) == num_blocks, 'Please check the length of drop_path_rate'
+
         downsample = None
         if stride != 1 or in_channels != out_channels:
             downsample = []
             conv_stride = stride
             if avg_down and stride != 1:
                 conv_stride = 1
                 downsample.append(
@@ -380,25 +389,27 @@
                 in_channels=in_channels,
                 out_channels=out_channels,
                 expansion=self.expansion,
                 stride=stride,
                 downsample=downsample,
                 conv_cfg=conv_cfg,
                 norm_cfg=norm_cfg,
+                drop_path_rate=drop_path_rate[0],
                 **kwargs))
         in_channels = out_channels
         for i in range(1, num_blocks):
             layers.append(
                 block(
                     in_channels=in_channels,
                     out_channels=out_channels,
                     expansion=self.expansion,
                     stride=1,
                     conv_cfg=conv_cfg,
                     norm_cfg=norm_cfg,
+                    drop_path_rate=drop_path_rate[i],
                     **kwargs))
         super(ResLayer, self).__init__(*layers)
 
 
 @MODELS.register_module()
 class ResNet(BaseBackbone):
     """ResNet backbone.
@@ -514,14 +525,21 @@
         self.expansion = get_expansion(self.block, expansion)
 
         self._make_stem_layer(in_channels, stem_channels)
 
         self.res_layers = []
         _in_channels = stem_channels
         _out_channels = base_channels * self.expansion
+
+        # stochastic depth decay rule
+        total_depth = sum(stage_blocks)
+        dpr = [
+            x.item() for x in torch.linspace(0, drop_path_rate, total_depth)
+        ]
+
         for i, num_blocks in enumerate(self.stage_blocks):
             stride = strides[i]
             dilation = dilations[i]
             res_layer = self.make_res_layer(
                 block=self.block,
                 num_blocks=num_blocks,
                 in_channels=_in_channels,
@@ -530,17 +548,18 @@
                 stride=stride,
                 dilation=dilation,
                 style=self.style,
                 avg_down=self.avg_down,
                 with_cp=with_cp,
                 conv_cfg=conv_cfg,
                 norm_cfg=norm_cfg,
-                drop_path_rate=drop_path_rate)
+                drop_path_rate=dpr[:num_blocks])
             _in_channels = _out_channels
             _out_channels *= 2
+            dpr = dpr[num_blocks:]
             layer_name = f'layer{i + 1}'
             self.add_module(layer_name, res_layer)
             self.res_layers.append(layer_name)
 
         self._freeze_stages()
 
         self.feat_dim = res_layer[-1].out_channels
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/resnet_cifar.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/resnext.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/revvit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/revvit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/riformer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/riformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         drop_rate (float): Dropout rate. Defaults to 0.
         drop_path_rate (float): Stochastic depth rate. Defaults to 0.
         out_indices (Sequence | int): Output from which network position.
             Index 0-6 respectively corresponds to
             [stage1, downsampling, stage2, downsampling, stage3, downsampling, stage4]
             Defaults to -1, means the last stage.
         frozen_stages (int): Stages to be frozen (all param fixed).
-            Defaults to 0, which means not freezing any parameters.
+            Defaults to -1, which means not freezing any parameters.
         deploy (bool): Whether to switch the model structure to
             deployment mode. Default: False.
         init_cfg (dict, optional): Initialization config dict
     """  # noqa: E501
 
     # --layers: [x,x,x,x], numbers of layers for the four stages
     # --embed_dims, --mlp_ratios:
@@ -255,15 +255,15 @@
                  in_pad=2,
                  down_patch_size=3,
                  down_stride=2,
                  down_pad=1,
                  drop_rate=0.,
                  drop_path_rate=0.,
                  out_indices=-1,
-                 frozen_stages=0,
+                 frozen_stages=-1,
                  init_cfg=None,
                  deploy=False):
 
         super().__init__(init_cfg=init_cfg)
 
         if isinstance(arch, str):
             assert arch in self.arch_settings, \
@@ -362,15 +362,15 @@
 
     def _freeze_stages(self):
         if self.frozen_stages >= 0:
             self.patch_embed.eval()
             for param in self.patch_embed.parameters():
                 param.requires_grad = False
 
-        for i in range(self.frozen_stages):
+        for i in range(0, self.frozen_stages + 1):
             # Include both block and downsample layer.
             module = self.network[i]
             module.eval()
             for param in module.parameters():
                 param.requires_grad = False
             if i in self.out_indices:
                 norm_layer = getattr(self, f'norm{i}')
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/seresnet.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/seresnet.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/seresnext.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/seresnext.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/shufflenet_v1.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/shufflenet_v1.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/shufflenet_v2.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/shufflenet_v2.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/swin_transformer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/swin_transformer_v2.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/swin_transformer_v2.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/t2t_vit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/t2t_vit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/timm_backbone.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/timm_backbone.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import warnings
 
 from mmengine.logging import MMLogger
 
 from mmpretrain.registry import MODELS
+from mmpretrain.utils import require
 from .base_backbone import BaseBackbone
 
 
 def print_timm_feature_info(feature_info):
     """Print feature_info of timm backbone to help development and debug.
 
     Args:
@@ -51,39 +52,41 @@
             not loading.
         in_channels (int): Number of input image channels. Defaults to 3.
         init_cfg (dict or list[dict], optional): Initialization config dict of
             OpenMMLab projects. Defaults to None.
         **kwargs: Other timm & model specific arguments.
     """
 
+    @require('timm')
     def __init__(self,
                  model_name,
                  features_only=False,
                  pretrained=False,
                  checkpoint_path='',
                  in_channels=3,
                  init_cfg=None,
                  **kwargs):
-        try:
-            import timm
-        except ImportError:
-            raise ImportError(
-                'Failed to import timm. Please run "pip install timm".')
+        import timm
 
         if not isinstance(pretrained, bool):
             raise TypeError('pretrained must be bool, not str for model path')
         if features_only and checkpoint_path:
             warnings.warn(
                 'Using both features_only and checkpoint_path will cause error'
                 ' in timm. See '
                 'https://github.com/rwightman/pytorch-image-models/issues/488')
 
         super(TIMMBackbone, self).__init__(init_cfg)
         if 'norm_layer' in kwargs:
-            kwargs['norm_layer'] = MODELS.get(kwargs['norm_layer'])
+            norm_class = MODELS.get(kwargs['norm_layer'])
+
+            def build_norm(*args, **kwargs):
+                return norm_class(*args, **kwargs)
+
+            kwargs['norm_layer'] = build_norm
         self.timm_model = timm.create_model(
             model_name=model_name,
             features_only=features_only,
             pretrained=pretrained,
             in_chans=in_channels,
             checkpoint_path=checkpoint_path,
             **kwargs)
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/tinyvit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/tinyvit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/tnt.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/tnt.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/twins.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/twins.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/van.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/van.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/vgg.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/vgg.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/vig.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/vig.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/vision_transformer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/vision_transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,51 +5,56 @@
 import torch
 import torch.nn as nn
 from mmcv.cnn.bricks.transformer import FFN, PatchEmbed
 from mmengine.model import BaseModule, ModuleList
 from mmengine.model.weight_init import trunc_normal_
 
 from mmpretrain.registry import MODELS
-from ..utils import (MultiheadAttention, build_norm_layer, resize_pos_embed,
-                     to_2tuple)
+from ..utils import (MultiheadAttention, SwiGLUFFNFused, build_norm_layer,
+                     resize_pos_embed, to_2tuple)
 from .base_backbone import BaseBackbone
 
 
 class TransformerEncoderLayer(BaseModule):
     """Implements one encoder layer in Vision Transformer.
 
     Args:
         embed_dims (int): The feature dimension
         num_heads (int): Parallel attention heads
         feedforward_channels (int): The hidden dimension for FFNs
+        layer_scale_init_value (float or torch.Tensor): Init value of layer
+            scale. Defaults to 0.
         drop_rate (float): Probability of an element to be zeroed
             after the feed forward layer. Defaults to 0.
         attn_drop_rate (float): The drop out rate for attention output weights.
             Defaults to 0.
         drop_path_rate (float): Stochastic depth rate. Defaults to 0.
         num_fcs (int): The number of fully-connected layers for FFNs.
             Defaults to 2.
         qkv_bias (bool): enable bias for qkv if True. Defaults to True.
+        ffn_type (str): Select the type of ffn layers. Defaults to 'origin'.
         act_cfg (dict): The activation config for FFNs.
             Defaluts to ``dict(type='GELU')``.
         norm_cfg (dict): Config dict for normalization layer.
             Defaults to ``dict(type='LN')``.
         init_cfg (dict, optional): Initialization config dict.
             Defaults to None.
     """
 
     def __init__(self,
                  embed_dims,
                  num_heads,
                  feedforward_channels,
+                 layer_scale_init_value=0.,
                  drop_rate=0.,
                  attn_drop_rate=0.,
                  drop_path_rate=0.,
                  num_fcs=2,
                  qkv_bias=True,
+                 ffn_type='origin',
                  act_cfg=dict(type='GELU'),
                  norm_cfg=dict(type='LN'),
                  init_cfg=None):
         super(TransformerEncoderLayer, self).__init__(init_cfg=init_cfg)
 
         self.embed_dims = embed_dims
 
@@ -57,25 +62,35 @@
 
         self.attn = MultiheadAttention(
             embed_dims=embed_dims,
             num_heads=num_heads,
             attn_drop=attn_drop_rate,
             proj_drop=drop_rate,
             dropout_layer=dict(type='DropPath', drop_prob=drop_path_rate),
-            qkv_bias=qkv_bias)
+            qkv_bias=qkv_bias,
+            layer_scale_init_value=layer_scale_init_value)
 
         self.ln2 = build_norm_layer(norm_cfg, self.embed_dims)
 
-        self.ffn = FFN(
-            embed_dims=embed_dims,
-            feedforward_channels=feedforward_channels,
-            num_fcs=num_fcs,
-            ffn_drop=drop_rate,
-            dropout_layer=dict(type='DropPath', drop_prob=drop_path_rate),
-            act_cfg=act_cfg)
+        if ffn_type == 'origin':
+            self.ffn = FFN(
+                embed_dims=embed_dims,
+                feedforward_channels=feedforward_channels,
+                num_fcs=num_fcs,
+                ffn_drop=drop_rate,
+                dropout_layer=dict(type='DropPath', drop_prob=drop_path_rate),
+                act_cfg=act_cfg,
+                layer_scale_init_value=layer_scale_init_value)
+        elif ffn_type == 'swiglu_fused':
+            self.ffn = SwiGLUFFNFused(
+                embed_dims=embed_dims,
+                feedforward_channels=feedforward_channels,
+                layer_scale_init_value=layer_scale_init_value)
+        else:
+            raise NotImplementedError
 
     @property
     def norm1(self):
         return self.ln1
 
     @property
     def norm2(self):
@@ -143,14 +158,16 @@
             Defaults to ``"cls_token"``.
         with_cls_token (bool): Whether concatenating class token into image
             tokens as transformer input. Defaults to True.
         frozen_stages (int): Stages to be frozen (stop grad and set eval mode).
             -1 means not freezing any parameters. Defaults to -1.
         interpolate_mode (str): Select the interpolate mode for position
             embeding vector resize. Defaults to "bicubic".
+        layer_scale_init_value (float or torch.Tensor): Init value of layer
+            scale. Defaults to 0.
         patch_cfg (dict): Configs of patch embeding. Defaults to an empty dict.
         layer_cfgs (Sequence | dict): Configs of each transformer layer in
             encoder. Defaults to an empty dict.
         init_cfg (dict, optional): Initialization config dict.
             Defaults to None.
     """
     arch_zoo = {
@@ -199,27 +216,34 @@
             ['deit-t', 'deit-tiny'], {
                 'embed_dims': 192,
                 'num_layers': 12,
                 'num_heads': 3,
                 'feedforward_channels': 192 * 4
             }),
         **dict.fromkeys(
-            ['deit-s', 'deit-small'], {
+            ['deit-s', 'deit-small', 'dinov2-s', 'dinov2-small'], {
                 'embed_dims': 384,
                 'num_layers': 12,
                 'num_heads': 6,
                 'feedforward_channels': 384 * 4
             }),
         **dict.fromkeys(
             ['deit-b', 'deit-base'], {
                 'embed_dims': 768,
                 'num_layers': 12,
                 'num_heads': 12,
                 'feedforward_channels': 768 * 4
             }),
+        **dict.fromkeys(
+            ['dinov2-g', 'dinov2-giant'], {
+                'embed_dims': 1536,
+                'num_layers': 40,
+                'num_heads': 24,
+                'feedforward_channels': 6144
+            }),
     }
     num_extra_tokens = 1  # class token
     OUT_TYPES = {'raw', 'cls_token', 'featmap', 'avg_featmap'}
 
     def __init__(self,
                  arch='base',
                  img_size=224,
@@ -231,14 +255,15 @@
                  qkv_bias=True,
                  norm_cfg=dict(type='LN', eps=1e-6),
                  final_norm=True,
                  out_type='cls_token',
                  with_cls_token=True,
                  frozen_stages=-1,
                  interpolate_mode='bicubic',
+                 layer_scale_init_value=0.,
                  patch_cfg=dict(),
                  layer_cfgs=dict(),
                  pre_norm=False,
                  init_cfg=None):
         super(VisionTransformer, self).__init__(init_cfg)
 
         if isinstance(arch, str):
@@ -318,14 +343,15 @@
             layer_cfgs = [layer_cfgs] * self.num_layers
         for i in range(self.num_layers):
             _layer_cfg = dict(
                 embed_dims=self.embed_dims,
                 num_heads=self.arch_settings['num_heads'],
                 feedforward_channels=self.
                 arch_settings['feedforward_channels'],
+                layer_scale_init_value=layer_scale_init_value,
                 drop_rate=drop_rate,
                 drop_path_rate=dpr[i],
                 qkv_bias=qkv_bias,
                 norm_cfg=norm_cfg)
             _layer_cfg.update(layer_cfgs[i])
             self.layers.append(TransformerEncoderLayer(**_layer_cfg))
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/backbones/xcit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/backbones/xcit.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/builder.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/builder.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/base.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/hugging_face.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/hugging_face.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from mmpretrain.registry import MODELS
 from mmpretrain.structures import DataSample
+from mmpretrain.utils import require
 from .base import BaseClassifier
 
 
 @MODELS.register_module()
 class HuggingFaceClassifier(BaseClassifier):
     """Image classifiers for HuggingFace model.
 
@@ -62,14 +63,15 @@
         >>> model = build_classifier(cfg)
         >>> inputs = torch.rand(1, 3, 224, 224)
         >>> out = model(inputs)
         >>> print(out.shape)
         torch.Size([1, 1000])
     """  # noqa: E501
 
+    @require('transformers')
     def __init__(self,
                  model_name,
                  pretrained=False,
                  *model_args,
                  loss=dict(type='CrossEntropyLoss', loss_weight=1.0),
                  train_cfg: Optional[dict] = None,
                  with_cp: bool = False,
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/image.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/image.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/classifiers/timm.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/classifiers/timm.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from mmpretrain.registry import MODELS
 from mmpretrain.structures import DataSample
+from mmpretrain.utils import require
 from .base import BaseClassifier
 
 
 @MODELS.register_module()
 class TimmClassifier(BaseClassifier):
     """Image classifiers for pytorch-image-models (timm) model.
 
@@ -55,14 +56,15 @@
         >>> model = build_classifier(cfg)
         >>> inputs = torch.rand(1, 3, 224, 224)
         >>> out = model(inputs)
         >>> print(out.shape)
         torch.Size([1, 1000])
     """  # noqa: E501
 
+    @require('timm')
     def __init__(self,
                  *args,
                  loss=dict(type='CrossEntropyLoss', loss_weight=1.0),
                  train_cfg: Optional[dict] = None,
                  with_cp: bool = False,
                  data_preprocessor: Optional[dict] = None,
                  init_cfg: Optional[dict] = None,
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,36 @@
 from .beitv2_head import BEiTV2Head
 from .cae_head import CAEHead
 from .cls_head import ClsHead
 from .conformer_head import ConformerHead
 from .contrastive_head import ContrastiveHead
 from .deit_head import DeiTClsHead
 from .efficientformer_head import EfficientFormerClsHead
+from .grounding_head import GroundingHead
+from .itc_head import ITCHead
+from .itm_head import ITMHead
 from .latent_heads import LatentCrossCorrelationHead, LatentPredictHead
 from .levit_head import LeViTClsHead
 from .linear_head import LinearClsHead
 from .mae_head import MAEPretrainHead
 from .margin_head import ArcFaceClsHead
 from .mim_head import MIMHead
 from .mixmim_head import MixMIMPretrainHead
 from .mocov3_head import MoCoV3Head
 from .multi_label_cls_head import MultiLabelClsHead
 from .multi_label_csra_head import CSRAClsHead
 from .multi_label_linear_head import MultiLabelLinearClsHead
 from .multi_task_head import MultiTaskHead
+from .seq_gen_head import SeqGenerationHead
 from .simmim_head import SimMIMHead
 from .stacked_head import StackedLinearClsHead
 from .swav_head import SwAVHead
 from .vig_head import VigClsHead
 from .vision_transformer_head import VisionTransformerClsHead
+from .vqa_head import VQAGenerationHead
 
 __all__ = [
     'ClsHead',
     'LinearClsHead',
     'StackedLinearClsHead',
     'MultiLabelClsHead',
     'MultiLabelLinearClsHead',
@@ -48,8 +53,13 @@
     'LatentPredictHead',
     'MAEPretrainHead',
     'MixMIMPretrainHead',
     'SwAVHead',
     'MoCoV3Head',
     'MIMHead',
     'SimMIMHead',
+    'SeqGenerationHead',
+    'VQAGenerationHead',
+    'ITCHead',
+    'ITMHead',
+    'GroundingHead',
 ]
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/beitv1_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/beitv1_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/beitv2_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/beitv2_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/cae_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/cae_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/cls_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/cls_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/conformer_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/conformer_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/contrastive_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/contrastive_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/deit_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/deit_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/efficientformer_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/efficientformer_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/latent_heads.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/latent_heads.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/levit_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/levit_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/linear_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/linear_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/mae_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/mae_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/margin_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/margin_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/mim_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/mim_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/mixmim_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/mixmim_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/mocov3_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/mocov3_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/multi_label_cls_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/multi_label_cls_head.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     def _get_loss(self, cls_score: torch.Tensor,
                   data_samples: List[DataSample], **kwargs):
         """Unpack data samples and compute loss."""
         num_classes = cls_score.size()[-1]
         # Unpack data samples and pack targets
         if 'gt_score' in data_samples[0]:
-            target = torch.stack([i.gt_score for i in data_samples])
+            target = torch.stack([i.gt_score.float() for i in data_samples])
         else:
             target = torch.stack([
                 label_to_onehot(i.gt_label, num_classes) for i in data_samples
             ]).float()
 
         # compute loss
         losses = dict()
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/multi_label_csra_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/multi_label_csra_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/multi_label_linear_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/multi_label_linear_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/multi_task_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/multi_task_head.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,18 @@
             assert isinstance(data_sample, MultiTaskDataSample)
             sample_mask = task_name in data_sample
             mask[i] = sample_mask
             if sample_mask:
                 task_data_samples.append(data_sample.get(task_name))
 
         if len(task_data_samples) == 0:
-            return {'loss': torch.tensor(0.), 'mask_size': torch.tensor(0.)}
+            # This makes it possible to perform loss.backward when a
+            # task does not have gt_labels within a batch.
+            loss = (inputs[0] * 0).sum()
+            return {'loss': loss, 'mask_size': torch.tensor(0.)}
 
         # Mask the inputs of the task
         def mask_inputs(inputs, mask):
             if isinstance(inputs, Sequence):
                 return type(inputs)(
                     [mask_inputs(input, mask) for input in inputs])
             elif isinstance(inputs, torch.Tensor):
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/simmim_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/simmim_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/stacked_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/stacked_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/swav_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/swav_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/vig_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/vig_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/heads/vision_transformer_head.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/heads/vision_transformer_head.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/asymmetric_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/asymmetric_loss.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/cae_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/cae_loss.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/cosine_similarity_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/cosine_similarity_loss.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/cross_correlation_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/cross_entropy_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/cross_entropy_loss.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     assert pred.dim() == label.dim()
 
     if class_weight is not None:
         N = pred.size()[0]
         class_weight = class_weight.repeat(N, 1)
     loss = F.binary_cross_entropy_with_logits(
         pred,
-        label,
+        label.float(),  # only accepts float type tensor
         weight=class_weight,
         pos_weight=pos_weight,
         reduction='none')
 
     # apply weights and do the reduction
     if weight is not None:
         assert weight.dim() == 1
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/focal_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/label_smooth_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/label_smooth_loss.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,17 @@
 
     def __init__(self,
                  label_smooth_val,
                  num_classes=None,
                  use_sigmoid=None,
                  mode='original',
                  reduction='mean',
-                 loss_weight=1.0):
+                 loss_weight=1.0,
+                 class_weight=None,
+                 pos_weight=None):
         super().__init__()
         self.num_classes = num_classes
         self.loss_weight = loss_weight
 
         assert (isinstance(label_smooth_val, float)
                 and 0 <= label_smooth_val < 1), \
             f'LabelSmoothLoss accepts a float label_smooth_val ' \
@@ -97,15 +99,19 @@
             self.smooth_label = self.multilabel_smooth_label
             use_sigmoid = True if use_sigmoid is None else use_sigmoid
         else:
             self.smooth_label = self.original_smooth_label
             use_sigmoid = False if use_sigmoid is None else use_sigmoid
 
         self.ce = CrossEntropyLoss(
-            use_sigmoid=use_sigmoid, use_soft=not use_sigmoid)
+            use_sigmoid=use_sigmoid,
+            use_soft=not use_sigmoid,
+            reduction=reduction,
+            class_weight=class_weight,
+            pos_weight=pos_weight)
 
     def generate_one_hot_like_label(self, label):
         """This function takes one-hot or index label vectors and computes one-
         hot like label vectors (float)"""
         # check if targets are inputted as class integers
         if label.dim() == 1 or (label.dim() == 2 and label.shape[1] == 1):
             label = convert_to_one_hot(label.view(-1, 1), self.num_classes)
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/reconstruction_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/reconstruction_loss.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/seesaw_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/seesaw_loss.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/swav_loss.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/swav_loss.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/losses/utils.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/beitv2_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/beitv2_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/cae_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/cae_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/densecl_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/densecl_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/gap.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/gap.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/gem.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/gem.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/hr_fuse.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/hr_fuse.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/linear_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/linear_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/mae_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/mae_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/milan_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/milan_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/mixmim_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/mixmim_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/mocov2_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/mocov2_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/nonlinear_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/nonlinear_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/simmim_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/simmim_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/necks/swav_neck.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/necks/swav_neck.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/retrievers/base.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/retrievers/image2image.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/retrievers/image2image.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/__init__.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/barlowtwins.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/barlowtwins.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/base.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/base.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/beit.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/beit.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                  patch_size: int = 16,
                  in_channels: int = 3,
                  out_indices: int = -1,
                  drop_rate: float = 0,
                  drop_path_rate: float = 0,
                  norm_cfg: dict = dict(type='LN', eps=1e-6),
                  final_norm: bool = True,
-                 out_type: str = 'avg_featmap',
+                 out_type: str = 'raw',
                  frozen_stages: int = -1,
                  use_abs_pos_emb: bool = False,
                  use_rel_pos_bias: bool = False,
                  use_shared_rel_pos_bias: bool = True,
                  layer_scale_init_value: int = 0.1,
                  interpolate_mode: str = 'bicubic',
                  patch_cfg: dict = dict(padding=0),
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/byol.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/byol.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/cae.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/cae.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
         in_channels: int = 3,
         out_indices: int = -1,
         drop_rate: float = 0,
         drop_path_rate: float = 0,
         bias: bool = 'qv_bias',
         norm_cfg: dict = dict(type='LN', eps=1e-6),
         final_norm: bool = True,
-        out_type: str = 'avg_featmap',
+        out_type: str = 'raw',
         frozen_stages: int = -1,
         use_abs_pos_emb: bool = True,
         use_rel_pos_bias: bool = False,
         use_shared_rel_pos_bias: bool = False,
         layer_scale_init_value: float = None,
         interpolate_mode: str = 'bicubic',
         patch_cfg: dict = dict(),
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/densecl.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/densecl.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/eva.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/eva.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/mae.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/mae.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                  img_size: int = 224,
                  patch_size: int = 16,
                  out_indices: Union[Sequence, int] = -1,
                  drop_rate: float = 0,
                  drop_path_rate: float = 0,
                  norm_cfg: dict = dict(type='LN', eps=1e-6),
                  final_norm: bool = True,
-                 out_type: str = 'avg_featmap',
+                 out_type: str = 'raw',
                  interpolate_mode: str = 'bicubic',
                  patch_cfg: dict = dict(),
                  layer_cfgs: dict = dict(),
                  mask_ratio: float = 0.75,
                  init_cfg: Optional[Union[List[dict], dict]] = None) -> None:
         super().__init__(
             arch=arch,
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/maskfeat.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/maskfeat.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                  img_size: int = 224,
                  patch_size: int = 16,
                  out_indices: Union[Sequence, int] = -1,
                  drop_rate: float = 0,
                  drop_path_rate: float = 0,
                  norm_cfg: dict = dict(type='LN', eps=1e-6),
                  final_norm: bool = True,
-                 out_type: str = 'avg_featmap',
+                 out_type: str = 'raw',
                  interpolate_mode: str = 'bicubic',
                  patch_cfg: dict = dict(),
                  layer_cfgs: dict = dict(),
                  init_cfg: Optional[Union[List[dict], dict]] = None) -> None:
         super().__init__(
             arch=arch,
             img_size=img_size,
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/milan.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/milan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 from typing import Dict, List, Optional, Tuple
 
 import torch
-from mmengine.model import BaseModule
+import torch.nn as nn
 from mmengine.runner.checkpoint import _load_checkpoint
 
 from mmpretrain.registry import MODELS
 from mmpretrain.structures import DataSample
 from ..utils import build_clip_model
 from .base import BaseSelfSupervisor
 from .mae import MAEViT
 
 
 @MODELS.register_module()
-class CLIPGenerator(BaseModule):
+class CLIPGenerator(nn.Module):
     """Get the features and attention from the last layer of CLIP.
 
     This module is used to generate target features in masked image modeling.
 
     Args:
         tokenizer_path (str): The path of the checkpoint of CLIP.
     """
 
     def __init__(self, tokenizer_path: str) -> None:
         super().__init__()
         self.tokenizer_path = tokenizer_path
-        self.tokenizer = None
-
-    def init_weights(self):
-        super().init_weights()
         self.tokenizer = build_clip_model(
             _load_checkpoint(self.tokenizer_path), False)
 
     @torch.no_grad()
     def forward(self, x: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         """Get the features and attention from the last layer of CLIP.
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/mixmim.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/mixmim.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/moco.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/moco.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/mocov3.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/mocov3.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/simclr.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/simclr.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/simmim.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/simmim.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/simsiam.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/simsiam.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/selfsup/swav.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/selfsup/swav.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/tta/score_tta.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/tta/score_tta.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/__init__.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+from mmpretrain.utils.dependency import WITH_MULTIMODAL
 from .attention import (BEiTAttention, ChannelMultiheadAttention,
                         CrossMultiheadAttention, LeAttention,
                         MultiheadAttention, PromptMultiheadAttention,
                         ShiftWindowMSA, WindowMSA, WindowMSAV2)
 from .batch_augments import CutMix, Mixup, RandomBatchAugment, ResizeMix
 from .batch_shuffle import batch_shuffle_ddp, batch_unshuffle_ddp
 from .channel_shuffle import channel_shuffle
-from .clip_generator_helper import build_clip_model
-from .data_preprocessor import (ClsDataPreprocessor, SelfSupDataPreprocessor,
+from .clip_generator_helper import QuickGELU, build_clip_model
+from .data_preprocessor import (ClsDataPreprocessor,
+                                MultiModalDataPreprocessor,
+                                SelfSupDataPreprocessor,
                                 TwoNormDataPreprocessor, VideoDataPreprocessor)
 from .ema import CosineEMA
 from .embed import (HybridEmbed, PatchEmbed, PatchMerging, resize_pos_embed,
                     resize_relative_position_bias_table)
 from .helpers import is_tracing, to_2tuple, to_3tuple, to_4tuple, to_ntuple
 from .inverted_residual import InvertedResidual
 from .layer_scale import LayerScale
 from .make_divisible import make_divisible
 from .norm import GRN, LayerNorm2d, build_norm_layer
 from .position_encoding import (ConditionalPositionEncoding,
-                                PositionEncodingFourier,
+                                PositionEncodingFourier, RotaryEmbeddingFast,
                                 build_2d_sincos_position_embedding)
 from .res_layer_extra_norm import ResLayerExtraNorm
 from .se_layer import SELayer
+from .swiglu_ffn import SwiGLUFFN, SwiGLUFFNFused
 from .vector_quantizer import NormEMAVectorQuantizer
 
 __all__ = [
     'channel_shuffle',
     'make_divisible',
     'InvertedResidual',
     'SELayer',
@@ -65,8 +69,24 @@
     'batch_shuffle_ddp',
     'batch_unshuffle_ddp',
     'SelfSupDataPreprocessor',
     'TwoNormDataPreprocessor',
     'VideoDataPreprocessor',
     'CosineEMA',
     'ResLayerExtraNorm',
+    'MultiModalDataPreprocessor',
+    'QuickGELU',
+    'SwiGLUFFN',
+    'SwiGLUFFNFused',
+    'RotaryEmbeddingFast',
 ]
+
+if WITH_MULTIMODAL:
+    from .huggingface import (no_load_hf_pretrained_model, register_hf_model,
+                              register_hf_tokenizer)
+    from .tokenizer import (Blip2Tokenizer, BlipTokenizer, FullTokenizer,
+                            OFATokenizer)
+
+    __all__.extend([
+        'BlipTokenizer', 'OFATokenizer', 'Blip2Tokenizer', 'register_hf_model',
+        'register_hf_tokenizer', 'no_load_hf_pretrained_model', 'FullTokenizer'
+    ])
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/attention.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 import itertools
+import warnings
 from functools import partial
 from typing import List, Optional, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
@@ -524,14 +525,17 @@
         qk_scale (float, optional): Override default qk scale of
             ``head_dim ** -0.5`` if set. Defaults to None.
         proj_bias (bool) If True, add a learnable bias to output projection.
             Defaults to True.
         v_shortcut (bool): Add a shortcut from value to output. It's usually
             used if ``input_dims`` is different from ``embed_dims``.
             Defaults to False.
+        use_layer_scale (bool): Whether to use layer scale. Defaults to False.
+        layer_scale_init_value (float or torch.Tensor): Init value of layer
+            scale. Defaults to 0.
         init_cfg (dict, optional): The Config for initialization.
             Defaults to None.
     """
 
     def __init__(self,
                  embed_dims,
                  num_heads,
@@ -540,14 +544,15 @@
                  proj_drop=0.,
                  dropout_layer=dict(type='Dropout', drop_prob=0.),
                  qkv_bias=True,
                  qk_scale=None,
                  proj_bias=True,
                  v_shortcut=False,
                  use_layer_scale=False,
+                 layer_scale_init_value=0.,
                  init_cfg=None):
         super(MultiheadAttention, self).__init__(init_cfg=init_cfg)
 
         self.input_dims = input_dims or embed_dims
         self.embed_dims = embed_dims
         self.num_heads = num_heads
         self.v_shortcut = v_shortcut
@@ -564,15 +569,22 @@
         self.attn_drop = attn_drop
         self.proj = nn.Linear(embed_dims, embed_dims, bias=proj_bias)
         self.proj_drop = nn.Dropout(proj_drop)
 
         self.out_drop = build_dropout(dropout_layer)
 
         if use_layer_scale:
-            self.gamma1 = LayerScale(embed_dims)
+            warnings.warn('The `use_layer_scale` in `MultiheadAttention` will '
+                          'be deprecated. Please use `layer_scale_init_value` '
+                          'to control whether using layer scale or not.')
+
+        if use_layer_scale or (layer_scale_init_value > 0):
+            layer_scale_init_value = layer_scale_init_value or 1e-5
+            self.gamma1 = LayerScale(
+                embed_dims, layer_scale_init_value=layer_scale_init_value)
         else:
             self.gamma1 = nn.Identity()
 
     def forward(self, x):
         B, N, _ = x.shape
         qkv = self.qkv(x).reshape(B, N, 3, self.num_heads,
                                   self.head_dims).permute(2, 0, 3, 1, 4)
@@ -1053,17 +1065,27 @@
                  dropout_layer: dict = dict(type='Dropout', drop_prob=0.),
                  qkv_bias: bool = True,
                  qk_scale: Optional[float] = None,
                  proj_bias: bool = True,
                  v_shortcut: bool = False,
                  use_layer_scale: bool = False,
                  init_cfg: Optional[Union[List[dict], dict]] = None) -> None:
-        super().__init__(embed_dims, num_heads, input_dims, attn_drop,
-                         proj_drop, dropout_layer, qkv_bias, qk_scale,
-                         proj_bias, v_shortcut, use_layer_scale, init_cfg)
+        super().__init__(
+            embed_dims=embed_dims,
+            num_heads=num_heads,
+            input_dims=input_dims,
+            attn_drop=attn_drop,
+            proj_drop=proj_drop,
+            dropout_layer=dropout_layer,
+            qkv_bias=qkv_bias,
+            qk_scale=qk_scale,
+            proj_bias=proj_bias,
+            v_shortcut=v_shortcut,
+            use_layer_scale=use_layer_scale,
+            init_cfg=init_cfg)
         # no longer need qkv
         del self.qkv
 
         # to project the mask tokens
         self.q = nn.Linear(embed_dims, embed_dims, bias=qkv_bias)
         # to project al the tokens
         self.kv = nn.Linear(embed_dims, embed_dims * 2, bias=qkv_bias)
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/cutmix.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/cutmix.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/mixup.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/mixup.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/resizemix.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/resizemix.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_augments/wrapper.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_augments/wrapper.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/batch_shuffle.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/batch_shuffle.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/channel_shuffle.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/channel_shuffle.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/clip_generator_helper.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/clip_generator_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import torch
 from mmengine.logging import MMLogger
 from torch import nn
 
+from mmpretrain.registry import MODELS
+
 
 class LayerNorm(nn.LayerNorm):
     """Subclass torch's LayerNorm to handle fp16."""
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """Forward function."""
         orig_type = x.dtype
         ret = super().forward(x.type(torch.float32))
         return ret.type(orig_type)
 
 
+@MODELS.register_module()
 class QuickGELU(nn.Module):
     """A faster version of GELU."""
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         """Forward function."""
         return x * torch.sigmoid(1.702 * x)
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/data_preprocessor.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/data_preprocessor.py`

 * *Files 13% similar despite different names*

```diff
@@ -511,7 +511,110 @@
             batch_inputs = batch_inputs.float()
 
             # normalization
             if self._enable_normalize:
                 batch_inputs = (batch_inputs - self.mean) / self.std
 
         return {'inputs': batch_inputs, 'data_samples': batch_data_samples}
+
+
+@MODELS.register_module()
+class MultiModalDataPreprocessor(BaseDataPreprocessor):
+    """Data pre-processor for image-text multimodality tasks.
+
+    It provides the data pre-processing as follows
+
+    - Collate and move data to the target device.
+    - Pad inputs to the maximum size of current batch with defined
+      ``pad_value``. The padding size can be divisible by a defined
+      ``pad_size_divisor``
+    - Stack inputs to batch_inputs.
+    - Convert inputs from bgr to rgb if the shape of input is (3, H, W).
+    - Normalize image with defined std and mean.
+
+    Args:
+        mean (Sequence[Number], optional): The pixel mean of R, G, B channels.
+            Defaults to None.
+        std (Sequence[Number], optional): The pixel standard deviation of
+            R, G, B channels. Defaults to None.
+        pad_size_divisor (int): The size of padded image should be
+            divisible by ``pad_size_divisor``. Defaults to 1.
+        pad_value (Number): The padded pixel value. Defaults to 0.
+        to_rgb (bool): whether to convert image from BGR to RGB.
+            Defaults to False.
+    """
+
+    def __init__(
+        self,
+        mean: Sequence[Number] = None,
+        std: Sequence[Number] = None,
+        pad_size_divisor: int = 1,
+        pad_value: Number = 0,
+        to_rgb: bool = False,
+    ):
+        super().__init__()
+        self.pad_size_divisor = pad_size_divisor
+        self.pad_value = pad_value
+        self.to_rgb = to_rgb
+
+        if mean is not None:
+            assert std is not None, 'To enable the normalization in ' \
+                'preprocessing, please specify both `mean` and `std`.'
+            # Enable the normalization in preprocessing.
+            self._enable_normalize = True
+            self.register_buffer('mean',
+                                 torch.tensor(mean).view(-1, 1, 1), False)
+            self.register_buffer('std',
+                                 torch.tensor(std).view(-1, 1, 1), False)
+        else:
+            self._enable_normalize = False
+
+    def forward(self, data: dict, training: bool = False) -> dict:
+        """Perform normalization, padding, bgr2rgb conversion and batch
+        augmentation based on ``BaseDataPreprocessor``.
+
+        Args:
+            data (dict): data sampled from dataloader.
+            training (bool): Whether to enable training time augmentation.
+
+        Returns:
+            dict: Data in the same format as the model input.
+        """
+        data = self.cast_data(data)
+
+        imgs = data.get('inputs', None)
+
+        def _process_img(img):
+            # ------ To RGB ------
+            if self.to_rgb and img.size(1) == 3:
+                img = img.flip(1)
+
+            # -- Normalization ---
+            img = img.float()
+            if self._enable_normalize:
+                img = (img - self.mean) / self.std
+
+            # ------ Padding -----
+            if self.pad_size_divisor > 1:
+                h, w = img.shape[-2:]
+
+                target_h = math.ceil(
+                    h / self.pad_size_divisor) * self.pad_size_divisor
+                target_w = math.ceil(
+                    w / self.pad_size_divisor) * self.pad_size_divisor
+                pad_h = target_h - h
+                pad_w = target_w - w
+                img = F.pad(img, (0, pad_w, 0, pad_h), 'constant',
+                            self.pad_value)
+            return img
+
+        if isinstance(imgs, torch.Tensor):
+            imgs = _process_img(imgs)
+        elif isinstance(imgs, Sequence):
+            # B, T, C, H, W
+            imgs = torch.stack([_process_img(img) for img in imgs], dim=1)
+        elif imgs is not None:
+            raise ValueError(f'{type(imgs)} is not supported for imgs inputs.')
+
+        data_samples = data.get('data_samples', None)
+
+        return {'images': imgs, 'data_samples': data_samples}
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/ema.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/ema.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/embed.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/embed.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/helpers.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/inverted_residual.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/layer_scale.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/layer_scale.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # Copyright (c) OpenMMLab. All rights reserved.
+from typing import Union
+
 import torch
 import torch.nn as nn
 
 
 class LayerScale(nn.Module):
     """LayerScale layer.
 
     Args:
         dim (int): Dimension of input features.
+        layer_scale_init_value (float or torch.Tensor): Init value of layer
+            scale. Defaults to 1e-5.
         inplace (bool): inplace: can optionally do the
             operation in-place. Defaults to False.
         data_format (str): The input data format, could be 'channels_last'
              or 'channels_first', representing (B, C, H, W) and
              (B, N, C) format data respectively. Defaults to 'channels_last'.
     """
 
     def __init__(self,
                  dim: int,
+                 layer_scale_init_value: Union[float, torch.Tensor] = 1e-5,
                  inplace: bool = False,
                  data_format: str = 'channels_last'):
         super().__init__()
         assert data_format in ('channels_last', 'channels_first'), \
             "'data_format' could only be channels_last or channels_first."
         self.inplace = inplace
         self.data_format = data_format
-        self.weight = nn.Parameter(torch.ones(dim) * 1e-5)
+        self.weight = nn.Parameter(torch.ones(dim) * layer_scale_init_value)
 
     def forward(self, x):
         if self.data_format == 'channels_first':
             if self.inplace:
                 return x.mul_(self.weight.view(-1, 1, 1))
             else:
                 return x * self.weight.view(-1, 1, 1)
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/make_divisible.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/norm.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/norm.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/res_layer_extra_norm.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/res_layer_extra_norm.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/se_layer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/models/utils/vector_quantizer.py` & `mmpretrain-1.0.0rc8/mmpretrain/models/utils/vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/registry.py` & `mmpretrain-1.0.0rc8/mmpretrain/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,19 @@
 )
 # Task-specific modules like anchor generators and box coders
 TASK_UTILS = Registry(
     'task util',
     parent=MMENGINE_TASK_UTILS,
     locations=['mmpretrain.models'],
 )
+# Tokenizer to encode sequence
+TOKENIZER = Registry(
+    'tokenizer',
+    locations=['mmpretrain.models'],
+)
 
 #######################################################################
 #                       mmpretrain.evaluation                         #
 #######################################################################
 
 # Metrics to evaluate the model prediction results.
 METRICS = Registry(
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/structures/data_sample.py` & `mmpretrain-1.0.0rc8/mmpretrain/structures/data_sample.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/structures/utils.py` & `mmpretrain-1.0.0rc8/mmpretrain/structures/utils.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/utils/analyze.py` & `mmpretrain-1.0.0rc8/mmpretrain/utils/analyze.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/utils/collect_env.py` & `mmpretrain-1.0.0rc8/mmpretrain/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/utils/setup_env.py` & `mmpretrain-1.0.0rc8/mmpretrain/utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/version.py` & `mmpretrain-1.0.0rc8/mmpretrain/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved
 
-__version__ = '1.0.0rc7'
+__version__ = '1.0.0rc8'
 
 
 def parse_version_info(version_str):
     """Parse a version string into a tuple.
 
     Args:
         version_str (str): The version string.
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain/visualization/utils.py` & `mmpretrain-1.0.0rc8/mmpretrain/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `mmpretrain-1.0.0rc7/mmpretrain.egg-info/PKG-INFO` & `mmpretrain-1.0.0rc8/mmpretrain.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmpretrain
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: OpenMMLab Model Pretraining Toolbox and Benchmark
 Home-page: https://github.com/open-mmlab/mmpretrain
 Author: MMPretrain Contributors
 Author-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
         
@@ -74,22 +74,36 @@
         MMPreTrain is an open source pre-training toolbox based on PyTorch. It is a part of the [OpenMMLab](https://openmmlab.com/) project.
         
         The `main` branch works with **PyTorch 1.8+**.
         
         ### Major features
         
         - Various backbones and pretrained models
-        - Rich training strategies(supervised learning, self-supervised learning, etc.)
+        - Rich training strategies (supervised learning, self-supervised learning, multi-modality learning etc.)
         - Bag of training tricks
         - Large-scale training configs
         - High efficiency and extensibility
         - Powerful toolkits for model analysis and experiments
+        - Various out-of-box inference tasks.
+          - Image Classification
+          - Image Caption
+          - Visual Question Answering
+          - Visual Grounding
+          - Retrieval (Image-To-Image, Text-To-Image, Image-To-Text)
+        
+        https://github.com/open-mmlab/mmpretrain/assets/26739999/e4dcd3a2-f895-4d1b-a351-fbc74a04e904
         
         ## What's new
         
+        🌟 v1.0.0rc8 was released in 22/05/2023
+        
+        - Support multiple **multi-modal** algorithms and inferencers. You can explore these features by the [gradio demo](https://github.com/open-mmlab/mmpretrain/tree/main/projects/gradio_demo)!
+        - Add EVA-02, Dino-V2, ViT-SAM and GLIP backbones.
+        - Register torchvision transforms into MMPretrain, you can now easily integrate torchvision's data augmentations in MMPretrain. See [the doc](https://mmpretrain.readthedocs.io/en/latest/api/data_process.html#torchvision-transforms)
+        
         🌟 v1.0.0rc7 was released in 07/04/2023
         
         - Integrated Self-supervised learning algorithms from **MMSelfSup**, such as **MAE**, **BEiT**, etc.
         - Support **RIFormer**, a simple but effective vision backbone by removing token mixer.
         - Add t-SNE visualization.
         - Refactor dataset pipeline visualization.
         
@@ -121,14 +135,20 @@
         git clone https://github.com/open-mmlab/mmpretrain.git
         cd mmpretrain
         mim install -e .
         ```
         
         Please refer to [installation documentation](https://mmpretrain.readthedocs.io/en/latest/get_started.html) for more detailed installation and dataset preparation.
         
+        For multi-modality models support, please install the extra dependencies by:
+        
+        ```shell
+        mim install -e ".[multimodal]"
+        ```
+        
         ## User Guides
         
         We provided a series of tutorials about the basic usage of MMPreTrain for new users:
         
         - [Learn about Configs](https://mmpretrain.readthedocs.io/en/latest/user_guides/config.html)
         - [Prepare Dataset](https://mmpretrain.readthedocs.io/en/latest/user_guides/dataset_prepare.html)
         - [Inference with existing models](https://mmpretrain.readthedocs.io/en/latest/user_guides/inference.html)
@@ -151,14 +171,17 @@
               <td>
                 <b>Supported Backbones</b>
               </td>
               <td>
                 <b>Self-supervised Learning</b>
               </td>
               <td>
+                <b>Multi-Modality Algorithms</b>
+              </td>
+              <td>
                 <b>Others</b>
               </td>
             </tr>
             <tr valign="top">
               <td>
                 <ul>
                 <li><a href="configs/vgg">VGG</a></li>
@@ -204,14 +227,15 @@
                 <li><a href="configs/efficientnet_v2">EfficientNet V2</a></li>
                 <li><a href="configs/revvit">RevViT</a></li>
                 <li><a href="configs/convnext_v2">ConvNeXt V2</a></li>
                 <li><a href="configs/vig">ViG</a></li>
                 <li><a href="configs/xcit">XCiT</a></li>
                 <li><a href="configs/levit">LeViT</a></li>
                 <li><a href="configs/riformer">RIFormer</a></li>
+                <li><a href="configs/glip">GLIP</a></li>
                 </ul>
               </td>
               <td>
                 <ul>
                 <li><a href="configs/mocov2">MoCo V1 (CVPR'2020)</a></li>
                 <li><a href="configs/simclr">SimCLR (ICML'2020)</a></li>
                 <li><a href="configs/mocov2">MoCo V2 (arXiv'2020)</a></li>
@@ -229,14 +253,23 @@
                 <li><a href="configs/milan">MILAN (arXiv'2022)</a></li>
                 <li><a href="configs/beitv2">BEiT V2 (arXiv'2022)</a></li>
                 <li><a href="configs/eva">EVA (CVPR'2023)</a></li>
                 <li><a href="configs/mixmim">MixMIM (arXiv'2022)</a></li>
                 </ul>
               </td>
               <td>
+                <ul>
+                <li><a href="configs/blip">BLIP (arxiv'2022)</a></li>
+                <li><a href="configs/blip2">BLIP-2 (arxiv'2023)</a></li>
+                <li><a href="configs/ofa">OFA (CoRR'2022)</a></li>
+                <li><a href="configs/flamingo">Flamingo (NeurIPS'2022)</a></li>
+                <li><a href="configs/chinese_clip">Chinese CLIP (arxiv'2022)</a></li>
+                </ul>
+              </td>
+              <td>
               Image Retrieval Task:
                 <ul>
                 <li><a href="configs/arcface">ArcFace (CVPR'2019)</a></li>
                 </ul>
               Training&Test Tips:
                 <ul>
                 <li><a href="https://arxiv.org/abs/1909.13719">RandAug</a></li>
@@ -293,17 +326,18 @@
         - [MMHuman3D](https://github.com/open-mmlab/mmhuman3d): OpenMMLab 3D human parametric model toolbox and benchmark.
         - [MMSelfSup](https://github.com/open-mmlab/mmselfsup): OpenMMLab self-supervised learning toolbox and benchmark.
         - [MMRazor](https://github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and benchmark.
         - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab fewshot learning toolbox and benchmark.
         - [MMAction2](https://github.com/open-mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and benchmark.
         - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab video perception toolbox and benchmark.
         - [MMFlow](https://github.com/open-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark.
-        - [MMEditing](https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing toolbox.
+        - [MMagic](https://github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and **I**ntelligent **C**reation toolbox.
         - [MMGeneration](https://github.com/open-mmlab/mmgeneration): OpenMMLab image and video generative models toolbox.
         - [MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+        - [Playground](https://github.com/open-mmlab/playground): A central hub for gathering and showcasing amazing projects built upon OpenMMLab.
         
 Keywords: computer vision,image classification,unsupervised learning,self-supervised learning
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -315,7 +349,8 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: tests
 Provides-Extra: optional
 Provides-Extra: mim
+Provides-Extra: multimodal
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmpretrain Version: 1.0.0rc7 Summary: OpenMMLab
+Metadata-Version: 2.1 Name: mmpretrain Version: 1.0.0rc8 Summary: OpenMMLab
 Model Pretraining Toolbox and Benchmark Home-page: https://github.com/open-
 mmlab/mmpretrain Author: MMPretrain Contributors Author-email:
 openmmlab@gmail.com License: Apache License 2.0 Description:
                            [resources/mmpt-logo.png]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
                                         
@@ -26,18 +26,29 @@
  Issues](https://github.com/open-mmlab/mmpretrain/issues/new/choose) [https://
  user-images.githubusercontent.com/36138628/230307505-4727ad0a-7d71-4069-939d-
          b499c7e272b7.png] English | [ç®ä½ä¸­æ](/README_zh-CN.md)
 
 ## Introduction MMPreTrain is an open source pre-training toolbox based on
 PyTorch. It is a part of the [OpenMMLab](https://openmmlab.com/) project. The
 `main` branch works with **PyTorch 1.8+**. ### Major features - Various
-backbones and pretrained models - Rich training strategies(supervised learning,
-self-supervised learning, etc.) - Bag of training tricks - Large-scale training
-configs - High efficiency and extensibility - Powerful toolkits for model
-analysis and experiments ## What's new ð v1.0.0rc7 was released in 07/04/
+backbones and pretrained models - Rich training strategies (supervised
+learning, self-supervised learning, multi-modality learning etc.) - Bag of
+training tricks - Large-scale training configs - High efficiency and
+extensibility - Powerful toolkits for model analysis and experiments - Various
+out-of-box inference tasks. - Image Classification - Image Caption - Visual
+Question Answering - Visual Grounding - Retrieval (Image-To-Image, Text-To-
+Image, Image-To-Text) https://github.com/open-mmlab/mmpretrain/assets/26739999/
+e4dcd3a2-f895-4d1b-a351-fbc74a04e904 ## What's new ð v1.0.0rc8 was released
+in 22/05/2023 - Support multiple **multi-modal** algorithms and inferencers.
+You can explore these features by the [gradio demo](https://github.com/open-
+mmlab/mmpretrain/tree/main/projects/gradio_demo)! - Add EVA-02, Dino-V2, ViT-
+SAM and GLIP backbones. - Register torchvision transforms into MMPretrain, you
+can now easily integrate torchvision's data augmentations in MMPretrain. See
+[the doc](https://mmpretrain.readthedocs.io/en/latest/api/
+data_process.html#torchvision-transforms) ð v1.0.0rc7 was released in 07/04/
 2023 - Integrated Self-supervised learning algorithms from **MMSelfSup**, such
 as **MAE**, **BEiT**, etc. - Support **RIFormer**, a simple but effective
 vision backbone by removing token mixer. - Add t-SNE visualization. - Refactor
 dataset pipeline visualization. Update of previous versions - Support
 **LeViT**, **XCiT**, **ViG**, **ConvNeXt-V2**, **EVA**, **RevViT**,
 **EfficientnetV2**, **CLIP**, **TinyViT** and **MixMIM** backbones. - Reproduce
 the training accuracy of **ConvNeXt** and **RepVGG**. - Support confusion
@@ -52,62 +63,68 @@
 mmpretrain.readthedocs.io/en/latest/notes/changelog.html) for more details and
 other release history. ## Installation Below are quick steps for installation:
 ```shell conda create -n open-mmlab python=3.8 pytorch==1.10.1
 torchvision==0.11.2 cudatoolkit=11.3 -c pytorch -y conda activate open-mmlab
 pip install openmim git clone https://github.com/open-mmlab/mmpretrain.git cd
 mmpretrain mim install -e . ``` Please refer to [installation documentation]
 (https://mmpretrain.readthedocs.io/en/latest/get_started.html) for more
-detailed installation and dataset preparation. ## User Guides We provided a
-series of tutorials about the basic usage of MMPreTrain for new users: - [Learn
-about Configs](https://mmpretrain.readthedocs.io/en/latest/user_guides/
-config.html) - [Prepare Dataset](https://mmpretrain.readthedocs.io/en/latest/
-user_guides/dataset_prepare.html) - [Inference with existing models](https://
+detailed installation and dataset preparation. For multi-modality models
+support, please install the extra dependencies by: ```shell mim install -e ".
+[multimodal]" ``` ## User Guides We provided a series of tutorials about the
+basic usage of MMPreTrain for new users: - [Learn about Configs](https://
+mmpretrain.readthedocs.io/en/latest/user_guides/config.html) - [Prepare
+Dataset](https://mmpretrain.readthedocs.io/en/latest/user_guides/
+dataset_prepare.html) - [Inference with existing models](https://
 mmpretrain.readthedocs.io/en/latest/user_guides/inference.html) - [Train]
 (https://mmpretrain.readthedocs.io/en/latest/user_guides/train.html) - [Test]
 (https://mmpretrain.readthedocs.io/en/latest/user_guides/test.html) -
 [Downstream tasks](https://mmpretrain.readthedocs.io/en/latest/user_guides/
 downstream.html) For more information, please refer to [our documentation]
 (https://mmpretrain.readthedocs.io/en/latest/). ## Model zoo Results and models
 are available in the [model zoo](https://mmpretrain.readthedocs.io/en/latest/
 modelzoo_statistics.html).
                                    Overview
-    Supported Backbones    Self-supervised Learning                Others
-    * VGG                     * MoCo_V1_(CVPR'2020)  Image Retrieval Task:
-    * ResNet                  * SimCLR_(ICML'2020)       * ArcFace_(CVPR'2019)
-    * ResNeXt                 * MoCo_V2_(arXiv'2020) Training&Test Tips:
-    * SE-ResNet               * BYOL_(NeurIPS'2020)      * RandAug
-    * SE-ResNeXt              * SwAV_(NeurIPS'2020)      * AutoAug
-    * RegNet                  * DenseCL_(CVPR'2021)      * RepeatAugSampler
-    * ShuffleNet_V1           * SimSiam_(CVPR'2021)      * TTA
-    * ShuffleNet_V2           * Barlow_Twins_            * ...
-    * MobileNet_V2              (ICML'2021)
-    * MobileNet_V3            * MoCo_V3_(ICCV'2021)
-    * Swin-Transformer        * BEiT_(ICLR'2022)
-    * Swin-Transformer_V2     * MAE_(CVPR'2022)
-    * RepVGG                  * SimMIM_(CVPR'2022)
-    * Vision-Transformer      * MaskFeat_(CVPR'2022)
-    * Transformer-in-         * CAE_(arXiv'2022)
-      Transformer             * MILAN_(arXiv'2022)
-    * Res2Net                 * BEiT_V2_(arXiv'2022)
-    * MLP-Mixer               * EVA_(CVPR'2023)
-    * DeiT                    * MixMIM_(arXiv'2022)
-    * DeiT-3
-    * Conformer
-    * T2T-ViT
-    * Twins
-    * EfficientNet
-    * EdgeNeXt
-    * ConvNeXt
-    * HRNet
-    * VAN
-    * ConvMixer
-    * CSPNet
-    * PoolFormer
-    * Inception_V3
-    * MobileOne
+                         Self-supervised       Multi-Modality
+ Supported Backbones         Learning            Algorithms                 Others
+    * VGG                 * MoCo_V1_           * BLIP_          Image Retrieval Task:
+    * ResNet                (CVPR'2020)          (arxiv'2022)       * ArcFace_
+    * ResNeXt             * SimCLR_            * BLIP-2_              (CVPR'2019)
+    * SE-ResNet             (ICML'2020)          (arxiv'2023)   Training&Test Tips:
+    * SE-ResNeXt          * MoCo_V2_           * OFA_               * RandAug
+    * RegNet                (arXiv'2020)         (CoRR'2022)        * AutoAug
+    * ShuffleNet_V1       * BYOL_              * Flamingo_          * RepeatAugSampler
+    * ShuffleNet_V2         (NeurIPS'2020)       (NeurIPS'2022)     * TTA
+    * MobileNet_V2        * SwAV_              * Chinese_CLIP_      * ...
+    * MobileNet_V3          (NeurIPS'2020)       (arxiv'2022)
+    * Swin-               * DenseCL_
+      Transformer           (CVPR'2021)
+    * Swin-               * SimSiam_
+      Transformer_V2        (CVPR'2021)
+    * RepVGG              * Barlow_Twins_
+    * Vision-               (ICML'2021)
+      Transformer         * MoCo_V3_
+    * Transformer-in-       (ICCV'2021)
+      Transformer         * BEiT_
+    * Res2Net               (ICLR'2022)
+    * MLP-Mixer           * MAE_
+    * DeiT                  (CVPR'2022)
+    * DeiT-3              * SimMIM_
+    * Conformer             (CVPR'2022)
+    * T2T-ViT             * MaskFeat_
+    * Twins                 (CVPR'2022)
+    * EfficientNet        * CAE_
+    * EdgeNeXt              (arXiv'2022)
+    * ConvNeXt            * MILAN_
+    * HRNet                 (arXiv'2022)
+    * VAN                 * BEiT_V2_
+    * ConvMixer             (arXiv'2022)
+    * CSPNet              * EVA_
+    * PoolFormer            (CVPR'2023)
+    * Inception_V3        * MixMIM_
+    * MobileOne             (arXiv'2022)
     * EfficientFormer
     * MViT
     * HorNet
     * MobileViT
     * DaViT
     * RepLKNet
     * BEiT
@@ -115,14 +132,15 @@
     * EfficientNet_V2
     * RevViT
     * ConvNeXt_V2
     * ViG
     * XCiT
     * LeViT
     * RIFormer
+    * GLIP
 ## Contributing We appreciate all contributions to improve MMPreTrain. Please
 refer to [CONTRUBUTING](https://mmpretrain.readthedocs.io/en/latest/notes/
 contribution_guide.html) for the contributing guideline. ## Acknowledgement
 MMPreTrain is an open source project that is contributed by researchers and
 engineers from various colleges and companies. We appreciate all the
 contributors who implement their methods or add new features, as well as users
 who give valuable feedbacks. We wish that the toolbox and benchmark could serve
@@ -155,23 +173,25 @@
 OpenMMLab self-supervised learning toolbox and benchmark. - [MMRazor](https://
 github.com/open-mmlab/mmrazor): OpenMMLab model compression toolbox and
 benchmark. - [MMFewShot](https://github.com/open-mmlab/mmfewshot): OpenMMLab
 fewshot learning toolbox and benchmark. - [MMAction2](https://github.com/open-
 mmlab/mmaction2): OpenMMLab's next-generation action understanding toolbox and
 benchmark. - [MMTracking](https://github.com/open-mmlab/mmtracking): OpenMMLab
 video perception toolbox and benchmark. - [MMFlow](https://github.com/open-
-mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMEditing]
-(https://github.com/open-mmlab/mmediting): OpenMMLab image and video editing
-toolbox. - [MMGeneration](https://github.com/open-mmlab/mmgeneration):
-OpenMMLab image and video generative models toolbox. - [MMDeploy](https://
-github.com/open-mmlab/mmdeploy): OpenMMLab model deployment framework.
+mmlab/mmflow): OpenMMLab optical flow toolbox and benchmark. - [MMagic](https:/
+/github.com/open-mmlab/mmagic): Open**MM**Lab **A**dvanced, **G**enerative and
+**I**ntelligent **C**reation toolbox. - [MMGeneration](https://github.com/open-
+mmlab/mmgeneration): OpenMMLab image and video generative models toolbox. -
+[MMDeploy](https://github.com/open-mmlab/mmdeploy): OpenMMLab model deployment
+framework. - [Playground](https://github.com/open-mmlab/playground): A central
+hub for gathering and showcasing amazing projects built upon OpenMMLab.
 Keywords: computer vision,image classification,unsupervised learning,self-
 supervised learning Platform: UNKNOWN Classifier: Development Status :: 4 -
 Beta Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7 Description-Content-Type: text/
 markdown Provides-Extra: all Provides-Extra: tests Provides-Extra: optional
-Provides-Extra: mim
+Provides-Extra: mim Provides-Extra: multimodal
```

### Comparing `mmpretrain-1.0.0rc7/mmpretrain.egg-info/SOURCES.txt` & `mmpretrain-1.0.0rc8/mmpretrain.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,31 @@
 mmpretrain.egg-info/not-zip-safe
 mmpretrain.egg-info/requires.txt
 mmpretrain.egg-info/top_level.txt
 mmpretrain/.mim/model-index.yml
 mmpretrain/.mim/configs/_base_/default_runtime.py
 mmpretrain/.mim/configs/_base_/datasets/cifar100_bs16.py
 mmpretrain/.mim/configs/_base_/datasets/cifar10_bs16.py
+mmpretrain/.mim/configs/_base_/datasets/coco_caption.py
+mmpretrain/.mim/configs/_base_/datasets/coco_retrieval.py
+mmpretrain/.mim/configs/_base_/datasets/coco_vg_vqa.py
+mmpretrain/.mim/configs/_base_/datasets/coco_vqa.py
 mmpretrain/.mim/configs/_base_/datasets/cub_bs8_384.py
 mmpretrain/.mim/configs/_base_/datasets/cub_bs8_448.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet21k_bs128.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_mbv3.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_medium_224.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_poolformer_small_224.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_revvit_224.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_medium_384.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_riformer_small_384.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs128_vig_224.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_196.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_336.py
+mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_448.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_eva_560.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs16_pil_bicubic_384.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_beitv2.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_davit_224.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_levit_224.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a12.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs256_rsb_a3.py
@@ -58,14 +63,16 @@
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_pil_resize_autoaug.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_224.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_256.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_swin_384.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs64_t2t_224.py
 mmpretrain/.mim/configs/_base_/datasets/imagenet_bs8_pil_bicubic_320.py
 mmpretrain/.mim/configs/_base_/datasets/inshop_bs32_448.py
+mmpretrain/.mim/configs/_base_/datasets/nlvr2.py
+mmpretrain/.mim/configs/_base_/datasets/refcoco.py
 mmpretrain/.mim/configs/_base_/datasets/voc_bs16.py
 mmpretrain/.mim/configs/_base_/datasets/pipelines/auto_aug.py
 mmpretrain/.mim/configs/_base_/datasets/pipelines/rand_aug.py
 mmpretrain/.mim/configs/_base_/models/efficientformer-l1.py
 mmpretrain/.mim/configs/_base_/models/efficientnet_b0.py
 mmpretrain/.mim/configs/_base_/models/efficientnet_b1.py
 mmpretrain/.mim/configs/_base_/models/efficientnet_b2.py
@@ -308,29 +315,45 @@
 mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py
 mmpretrain/.mim/configs/beit/benchmarks/beit-base-p16_8xb64_in1k.py
 mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-1600e_in1k.py
 mmpretrain/.mim/configs/beitv2/beitv2_beit-base-p16_8xb256-amp-coslr-300e_in1k.py
 mmpretrain/.mim/configs/beitv2/metafile.yml
 mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py
 mmpretrain/.mim/configs/beitv2/benchmarks/beit-base-p16_8xb64_in1k.py
+mmpretrain/.mim/configs/blip/blip-base_8xb16_refcoco.py
+mmpretrain/.mim/configs/blip/blip-base_8xb32_caption.py
+mmpretrain/.mim/configs/blip/blip-base_8xb32_nlvr.py
+mmpretrain/.mim/configs/blip/blip-base_8xb32_retrieval.py
+mmpretrain/.mim/configs/blip/blip-base_8xb32_vqa.py
+mmpretrain/.mim/configs/blip/metafile.yml
+mmpretrain/.mim/configs/blip2/blip2-opt2.7b_8xb16_vqa.py
+mmpretrain/.mim/configs/blip2/blip2-opt2.7b_8xb32_caption.py
+mmpretrain/.mim/configs/blip2/blip2_8xb32_retrieval.py
+mmpretrain/.mim/configs/blip2/metafile.yml
 mmpretrain/.mim/configs/byol/byol_resnet50_16xb256-coslr-200e_in1k.py
 mmpretrain/.mim/configs/byol/metafile.yml
 mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50-c4_ms-1x_coco.py
 mmpretrain/.mim/configs/byol/benchmarks/mask-rcnn_r50_fpn_ms-1x_coco.py
 mmpretrain/.mim/configs/byol/benchmarks/resnet50_8xb512-linear-coslr-90e_in1k.py
 mmpretrain/.mim/configs/cae/cae_beit-base-p16_8xb256-amp-coslr-300e_in1k.py
 mmpretrain/.mim/configs/cae/metafile.yml
 mmpretrain/.mim/configs/cae/benchmarks/beit-base-p16_8xb128-coslr-100e_in1k.py
+mmpretrain/.mim/configs/chinese_clip/cn-clip_resnet50_zeroshot-cls_cifar100.py
+mmpretrain/.mim/configs/chinese_clip/cn-clip_vit-base-p16_zeroshot-cls_cifar100.py
+mmpretrain/.mim/configs/chinese_clip/cn-clip_vit-huge-p14_zeroshot-cls_cifar100.py
+mmpretrain/.mim/configs/chinese_clip/cn-clip_vit-large-p14_zeroshot-cls_cifar100.py
+mmpretrain/.mim/configs/chinese_clip/metafile.yml
 mmpretrain/.mim/configs/clip/metafile.yml
 mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-384px.py
 mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k-448px.py
 mmpretrain/.mim/configs/clip/vit-base-p16_pt-64xb64_in1k.py
 mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-384px.py
 mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k-448px.py
 mmpretrain/.mim/configs/clip/vit-base-p32_pt-64xb64_in1k.py
+mmpretrain/.mim/configs/clip/vit-large-p14_headless.py
 mmpretrain/.mim/configs/conformer/conformer-base-p16_8xb128_in1k.py
 mmpretrain/.mim/configs/conformer/conformer-small-p16_8xb128_in1k.py
 mmpretrain/.mim/configs/conformer/conformer-small-p32_8xb128_in1k.py
 mmpretrain/.mim/configs/conformer/conformer-tiny-p16_8xb128_in1k.py
 mmpretrain/.mim/configs/conformer/metafile.yml
 mmpretrain/.mim/configs/convmixer/convmixer-1024-20_10xb64_in1k.py
 mmpretrain/.mim/configs/convmixer/convmixer-1536-20_10xb64_in1k.py
@@ -397,14 +420,19 @@
 mmpretrain/.mim/configs/densecl/metafile.yml
 mmpretrain/.mim/configs/densecl/benchmarks/resnet50_8xb32-linear-steplr-100e_in1k.py
 mmpretrain/.mim/configs/densenet/densenet121_4xb256_in1k.py
 mmpretrain/.mim/configs/densenet/densenet161_4xb256_in1k.py
 mmpretrain/.mim/configs/densenet/densenet169_4xb256_in1k.py
 mmpretrain/.mim/configs/densenet/densenet201_4xb256_in1k.py
 mmpretrain/.mim/configs/densenet/metafile.yml
+mmpretrain/.mim/configs/dinov2/metafile.yml
+mmpretrain/.mim/configs/dinov2/vit-base-p14_dinov2-pre_headless.py
+mmpretrain/.mim/configs/dinov2/vit-giant-p14_dinov2-pre_headless.py
+mmpretrain/.mim/configs/dinov2/vit-large-p14_dinov2-pre_headless.py
+mmpretrain/.mim/configs/dinov2/vit-small-p14_dinov2-pre_headless.py
 mmpretrain/.mim/configs/edgenext/edgenext-base_8xb256-usi_in1k.py
 mmpretrain/.mim/configs/edgenext/edgenext-base_8xb256_in1k.py
 mmpretrain/.mim/configs/edgenext/edgenext-small_8xb256-usi_in1k.py
 mmpretrain/.mim/configs/edgenext/edgenext-small_8xb256_in1k.py
 mmpretrain/.mim/configs/edgenext/edgenext-xsmall_8xb256_in1k.py
 mmpretrain/.mim/configs/edgenext/edgenext-xxsmall_8xb256_in1k.py
 mmpretrain/.mim/configs/edgenext/metafile.yml
@@ -455,14 +483,31 @@
 mmpretrain/.mim/configs/eva/eva-l-p14_8xb16_in1k-196px.py
 mmpretrain/.mim/configs/eva/eva-l-p14_8xb16_in1k-336px.py
 mmpretrain/.mim/configs/eva/eva-l-p14_headless.py
 mmpretrain/.mim/configs/eva/eva-mae-style_vit-base-p16_16xb256-coslr-400e_in1k.py
 mmpretrain/.mim/configs/eva/metafile.yml
 mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb128-coslr-100e_in1k.py
 mmpretrain/.mim/configs/eva/benchmarks/vit-base-p16_8xb2048-linear-coslr-100e_in1k.py
+mmpretrain/.mim/configs/eva02/eva02-base-p14_headless.py
+mmpretrain/.mim/configs/eva02/eva02-base-p14_in1k.py
+mmpretrain/.mim/configs/eva02/eva02-large-p14_headless.py
+mmpretrain/.mim/configs/eva02/eva02-large-p14_in1k.py
+mmpretrain/.mim/configs/eva02/eva02-small-p14_headless.py
+mmpretrain/.mim/configs/eva02/eva02-small-p14_in1k.py
+mmpretrain/.mim/configs/eva02/eva02-tiny-p14_headless.py
+mmpretrain/.mim/configs/eva02/eva02-tiny-p14_in1k.py
+mmpretrain/.mim/configs/eva02/metafile.yml
+mmpretrain/.mim/configs/flamingo/flamingo_fewshot_caption.py
+mmpretrain/.mim/configs/flamingo/flamingo_fewshot_vqa.py
+mmpretrain/.mim/configs/flamingo/flamingo_zeroshot_caption.py
+mmpretrain/.mim/configs/flamingo/flamingo_zeroshot_vqa.py
+mmpretrain/.mim/configs/flamingo/metafile.yml
+mmpretrain/.mim/configs/glip/glip-l_headless.py
+mmpretrain/.mim/configs/glip/glip-t_headless.py
+mmpretrain/.mim/configs/glip/metafile.yml
 mmpretrain/.mim/configs/hornet/hornet-base-gf_8xb64_in1k.py
 mmpretrain/.mim/configs/hornet/hornet-base_8xb64_in1k.py
 mmpretrain/.mim/configs/hornet/hornet-small-gf_8xb64_in1k.py
 mmpretrain/.mim/configs/hornet/hornet-small_8xb64_in1k.py
 mmpretrain/.mim/configs/hornet/hornet-tiny-gf_8xb128_in1k.py
 mmpretrain/.mim/configs/hornet/hornet-tiny_8xb128_in1k.py
 mmpretrain/.mim/configs/hornet/metafile.yml
@@ -557,14 +602,20 @@
 mmpretrain/.mim/configs/mocov3/benchmarks/vit-large-p16_8xb64-coslr-100e_in1k.py
 mmpretrain/.mim/configs/mocov3/benchmarks/vit-small-p16_8xb128-linear-coslr-90e_in1k.py
 mmpretrain/.mim/configs/mvit/metafile.yml
 mmpretrain/.mim/configs/mvit/mvitv2-base_8xb256_in1k.py
 mmpretrain/.mim/configs/mvit/mvitv2-large_8xb256_in1k.py
 mmpretrain/.mim/configs/mvit/mvitv2-small_8xb256_in1k.py
 mmpretrain/.mim/configs/mvit/mvitv2-tiny_8xb256_in1k.py
+mmpretrain/.mim/configs/ofa/metafile.yml
+mmpretrain/.mim/configs/ofa/ofa-base_finetuned_caption.py
+mmpretrain/.mim/configs/ofa/ofa-base_finetuned_refcoco.py
+mmpretrain/.mim/configs/ofa/ofa-base_finetuned_vqa.py
+mmpretrain/.mim/configs/ofa/ofa-base_zeroshot_vqa.py
+mmpretrain/.mim/configs/ofa/ofa-large_zeroshot_vqa.py
 mmpretrain/.mim/configs/poolformer/metafile.yml
 mmpretrain/.mim/configs/poolformer/poolformer-m36_32xb128_in1k.py
 mmpretrain/.mim/configs/poolformer/poolformer-m48_32xb128_in1k.py
 mmpretrain/.mim/configs/poolformer/poolformer-s12_32xb128_in1k.py
 mmpretrain/.mim/configs/poolformer/poolformer-s24_32xb128_in1k.py
 mmpretrain/.mim/configs/poolformer/poolformer-s36_32xb128_in1k.py
 mmpretrain/.mim/configs/regnet/metafile.yml
@@ -672,14 +723,18 @@
 mmpretrain/.mim/configs/riformer/deploy/riformer-m48-deploy_8xb64_in1k.py
 mmpretrain/.mim/configs/riformer/deploy/riformer-s12-deploy_8xb128_in1k-384px.py
 mmpretrain/.mim/configs/riformer/deploy/riformer-s12-deploy_8xb128_in1k.py
 mmpretrain/.mim/configs/riformer/deploy/riformer-s24-deploy_8xb128_in1k-384px.py
 mmpretrain/.mim/configs/riformer/deploy/riformer-s24-deploy_8xb128_in1k.py
 mmpretrain/.mim/configs/riformer/deploy/riformer-s36-deploy_8xb128_in1k.py
 mmpretrain/.mim/configs/riformer/deploy/riformer-s36-deploy_8xb64_in1k-384px.py
+mmpretrain/.mim/configs/sam/metafile.yml
+mmpretrain/.mim/configs/sam/vit-base-p16_sam_headless.py
+mmpretrain/.mim/configs/sam/vit-huge-p16_sam_headless.py
+mmpretrain/.mim/configs/sam/vit-large-p16_sam_headless.py
 mmpretrain/.mim/configs/seresnet/metafile.yml
 mmpretrain/.mim/configs/seresnet/seresnet101_8xb32_in1k.py
 mmpretrain/.mim/configs/seresnet/seresnet50_8xb32_in1k.py
 mmpretrain/.mim/configs/seresnet/seresnext101-32x4d_8xb32_in1k.py
 mmpretrain/.mim/configs/seresnet/seresnext50-32x4d_8xb32_in1k.py
 mmpretrain/.mim/configs/shufflenet_v1/metafile.yml
 mmpretrain/.mim/configs/shufflenet_v1/shufflenet-v1-1x_16xb64_in1k.py
@@ -844,20 +899,23 @@
 mmpretrain/.mim/tools/model_converters/clip_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/convnext_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/davit_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/deit3_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/edgenext_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/efficientnet_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/efficientnetv2_to_mmpretrain.py
+mmpretrain/.mim/tools/model_converters/eva02_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/eva_to_mmpretrain.py
+mmpretrain/.mim/tools/model_converters/glip_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/hornet2mmpretrain.py
 mmpretrain/.mim/tools/model_converters/levit2mmpretrain.py
 mmpretrain/.mim/tools/model_converters/mixmim_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/mlpmixer_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/mobilenetv2_to_mmpretrain.py
+mmpretrain/.mim/tools/model_converters/ofa.py
 mmpretrain/.mim/tools/model_converters/publish_model.py
 mmpretrain/.mim/tools/model_converters/reparameterize_model.py
 mmpretrain/.mim/tools/model_converters/replknet_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/repvgg_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/revvit_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/shufflenetv2_to_mmpretrain.py
 mmpretrain/.mim/tools/model_converters/tinyvit_to_mmpretrain.py
@@ -870,36 +928,61 @@
 mmpretrain/.mim/tools/torchserve/mmpretrain_handler.py
 mmpretrain/.mim/tools/torchserve/test_torchserver.py
 mmpretrain/.mim/tools/visualization/browse_dataset.py
 mmpretrain/.mim/tools/visualization/vis_cam.py
 mmpretrain/.mim/tools/visualization/vis_scheduler.py
 mmpretrain/.mim/tools/visualization/vis_tsne.py
 mmpretrain/apis/__init__.py
+mmpretrain/apis/base.py
 mmpretrain/apis/feature_extractor.py
+mmpretrain/apis/image_caption.py
 mmpretrain/apis/image_classification.py
 mmpretrain/apis/image_retrieval.py
 mmpretrain/apis/model.py
+mmpretrain/apis/multimodal_retrieval.py
+mmpretrain/apis/nlvr.py
+mmpretrain/apis/utils.py
+mmpretrain/apis/visual_grounding.py
+mmpretrain/apis/visual_question_answering.py
 mmpretrain/datasets/__init__.py
 mmpretrain/datasets/base_dataset.py
 mmpretrain/datasets/builder.py
+mmpretrain/datasets/caltech101.py
 mmpretrain/datasets/categories.py
 mmpretrain/datasets/cifar.py
+mmpretrain/datasets/coco_caption.py
+mmpretrain/datasets/coco_retrieval.py
+mmpretrain/datasets/coco_vqa.py
 mmpretrain/datasets/cub.py
 mmpretrain/datasets/custom.py
 mmpretrain/datasets/dataset_wrappers.py
+mmpretrain/datasets/dtd.py
+mmpretrain/datasets/fgvcaircraft.py
+mmpretrain/datasets/flamingo.py
+mmpretrain/datasets/flowers102.py
+mmpretrain/datasets/food101.py
 mmpretrain/datasets/imagenet.py
 mmpretrain/datasets/inshop.py
 mmpretrain/datasets/mnist.py
 mmpretrain/datasets/multi_label.py
 mmpretrain/datasets/multi_task.py
+mmpretrain/datasets/nlvr2.py
+mmpretrain/datasets/oxfordiiitpet.py
 mmpretrain/datasets/places205.py
+mmpretrain/datasets/refcoco.py
+mmpretrain/datasets/scienceqa.py
+mmpretrain/datasets/stanfordcars.py
+mmpretrain/datasets/sun397.py
 mmpretrain/datasets/utils.py
+mmpretrain/datasets/vg_vqa.py
+mmpretrain/datasets/visual_genome.py
 mmpretrain/datasets/voc.py
 mmpretrain/datasets/samplers/__init__.py
 mmpretrain/datasets/samplers/repeat_aug.py
+mmpretrain/datasets/samplers/sequential.py
 mmpretrain/datasets/transforms/__init__.py
 mmpretrain/datasets/transforms/auto_augment.py
 mmpretrain/datasets/transforms/formatting.py
 mmpretrain/datasets/transforms/processing.py
 mmpretrain/datasets/transforms/wrappers.py
 mmpretrain/engine/__init__.py
 mmpretrain/engine/hooks/__init__.py
@@ -909,27 +992,34 @@
 mmpretrain/engine/hooks/margin_head_hooks.py
 mmpretrain/engine/hooks/precise_bn_hook.py
 mmpretrain/engine/hooks/retriever_hooks.py
 mmpretrain/engine/hooks/simsiam_hook.py
 mmpretrain/engine/hooks/swav_hook.py
 mmpretrain/engine/hooks/switch_recipe_hook.py
 mmpretrain/engine/hooks/visualization_hook.py
+mmpretrain/engine/hooks/warmup_param_hook.py
 mmpretrain/engine/optimizers/__init__.py
 mmpretrain/engine/optimizers/adan_t.py
 mmpretrain/engine/optimizers/lamb.py
 mmpretrain/engine/optimizers/lars.py
 mmpretrain/engine/optimizers/layer_decay_optim_wrapper_constructor.py
+mmpretrain/engine/runners/__init__.py
+mmpretrain/engine/runners/retrieval_loop.py
 mmpretrain/evaluation/__init__.py
 mmpretrain/evaluation/functional/__init__.py
 mmpretrain/evaluation/metrics/__init__.py
+mmpretrain/evaluation/metrics/caption.py
 mmpretrain/evaluation/metrics/multi_label.py
 mmpretrain/evaluation/metrics/multi_task.py
 mmpretrain/evaluation/metrics/retrieval.py
+mmpretrain/evaluation/metrics/scienceqa.py
 mmpretrain/evaluation/metrics/single_label.py
+mmpretrain/evaluation/metrics/visual_grounding_eval.py
 mmpretrain/evaluation/metrics/voc_multi_label.py
+mmpretrain/evaluation/metrics/vqa.py
 mmpretrain/models/__init__.py
 mmpretrain/models/builder.py
 mmpretrain/models/backbones/__init__.py
 mmpretrain/models/backbones/alexnet.py
 mmpretrain/models/backbones/base_backbone.py
 mmpretrain/models/backbones/beit.py
 mmpretrain/models/backbones/conformer.py
@@ -979,14 +1069,16 @@
 mmpretrain/models/backbones/tinyvit.py
 mmpretrain/models/backbones/tnt.py
 mmpretrain/models/backbones/twins.py
 mmpretrain/models/backbones/van.py
 mmpretrain/models/backbones/vgg.py
 mmpretrain/models/backbones/vig.py
 mmpretrain/models/backbones/vision_transformer.py
+mmpretrain/models/backbones/vit_eva02.py
+mmpretrain/models/backbones/vit_sam.py
 mmpretrain/models/backbones/xcit.py
 mmpretrain/models/classifiers/__init__.py
 mmpretrain/models/classifiers/base.py
 mmpretrain/models/classifiers/hugging_face.py
 mmpretrain/models/classifiers/image.py
 mmpretrain/models/classifiers/timm.py
 mmpretrain/models/heads/__init__.py
@@ -994,43 +1086,74 @@
 mmpretrain/models/heads/beitv2_head.py
 mmpretrain/models/heads/cae_head.py
 mmpretrain/models/heads/cls_head.py
 mmpretrain/models/heads/conformer_head.py
 mmpretrain/models/heads/contrastive_head.py
 mmpretrain/models/heads/deit_head.py
 mmpretrain/models/heads/efficientformer_head.py
+mmpretrain/models/heads/grounding_head.py
+mmpretrain/models/heads/itc_head.py
+mmpretrain/models/heads/itm_head.py
 mmpretrain/models/heads/latent_heads.py
 mmpretrain/models/heads/levit_head.py
 mmpretrain/models/heads/linear_head.py
 mmpretrain/models/heads/mae_head.py
 mmpretrain/models/heads/margin_head.py
 mmpretrain/models/heads/mim_head.py
 mmpretrain/models/heads/mixmim_head.py
 mmpretrain/models/heads/mocov3_head.py
 mmpretrain/models/heads/multi_label_cls_head.py
 mmpretrain/models/heads/multi_label_csra_head.py
 mmpretrain/models/heads/multi_label_linear_head.py
 mmpretrain/models/heads/multi_task_head.py
+mmpretrain/models/heads/seq_gen_head.py
 mmpretrain/models/heads/simmim_head.py
 mmpretrain/models/heads/stacked_head.py
 mmpretrain/models/heads/swav_head.py
 mmpretrain/models/heads/vig_head.py
 mmpretrain/models/heads/vision_transformer_head.py
+mmpretrain/models/heads/vqa_head.py
 mmpretrain/models/losses/__init__.py
 mmpretrain/models/losses/asymmetric_loss.py
 mmpretrain/models/losses/cae_loss.py
 mmpretrain/models/losses/cosine_similarity_loss.py
 mmpretrain/models/losses/cross_correlation_loss.py
 mmpretrain/models/losses/cross_entropy_loss.py
 mmpretrain/models/losses/focal_loss.py
 mmpretrain/models/losses/label_smooth_loss.py
 mmpretrain/models/losses/reconstruction_loss.py
 mmpretrain/models/losses/seesaw_loss.py
 mmpretrain/models/losses/swav_loss.py
 mmpretrain/models/losses/utils.py
+mmpretrain/models/multimodal/__init__.py
+mmpretrain/models/multimodal/blip/__init__.py
+mmpretrain/models/multimodal/blip/blip_caption.py
+mmpretrain/models/multimodal/blip/blip_grounding.py
+mmpretrain/models/multimodal/blip/blip_nlvr.py
+mmpretrain/models/multimodal/blip/blip_retrieval.py
+mmpretrain/models/multimodal/blip/blip_vqa.py
+mmpretrain/models/multimodal/blip/language_model.py
+mmpretrain/models/multimodal/blip2/Qformer.py
+mmpretrain/models/multimodal/blip2/__init__.py
+mmpretrain/models/multimodal/blip2/blip2_caption.py
+mmpretrain/models/multimodal/blip2/blip2_opt_vqa.py
+mmpretrain/models/multimodal/blip2/blip2_retriever.py
+mmpretrain/models/multimodal/blip2/modeling_opt.py
+mmpretrain/models/multimodal/chinese_clip/__init__.py
+mmpretrain/models/multimodal/chinese_clip/bert.py
+mmpretrain/models/multimodal/chinese_clip/chinese_clip.py
+mmpretrain/models/multimodal/chinese_clip/utils.py
+mmpretrain/models/multimodal/flamingo/__init__.py
+mmpretrain/models/multimodal/flamingo/adapter.py
+mmpretrain/models/multimodal/flamingo/flamingo.py
+mmpretrain/models/multimodal/flamingo/modules.py
+mmpretrain/models/multimodal/flamingo/utils.py
+mmpretrain/models/multimodal/ofa/__init__.py
+mmpretrain/models/multimodal/ofa/ofa.py
+mmpretrain/models/multimodal/ofa/ofa_modules.py
 mmpretrain/models/necks/__init__.py
 mmpretrain/models/necks/beitv2_neck.py
 mmpretrain/models/necks/cae_neck.py
 mmpretrain/models/necks/densecl_neck.py
 mmpretrain/models/necks/gap.py
 mmpretrain/models/necks/gem.py
 mmpretrain/models/necks/hr_fuse.py
@@ -1064,45 +1187,51 @@
 mmpretrain/models/selfsup/simsiam.py
 mmpretrain/models/selfsup/swav.py
 mmpretrain/models/tta/__init__.py
 mmpretrain/models/tta/score_tta.py
 mmpretrain/models/utils/__init__.py
 mmpretrain/models/utils/attention.py
 mmpretrain/models/utils/batch_shuffle.py
+mmpretrain/models/utils/box_utils.py
 mmpretrain/models/utils/channel_shuffle.py
 mmpretrain/models/utils/clip_generator_helper.py
 mmpretrain/models/utils/data_preprocessor.py
 mmpretrain/models/utils/ema.py
 mmpretrain/models/utils/embed.py
 mmpretrain/models/utils/helpers.py
+mmpretrain/models/utils/huggingface.py
 mmpretrain/models/utils/inverted_residual.py
 mmpretrain/models/utils/layer_scale.py
 mmpretrain/models/utils/make_divisible.py
 mmpretrain/models/utils/norm.py
 mmpretrain/models/utils/position_encoding.py
 mmpretrain/models/utils/res_layer_extra_norm.py
 mmpretrain/models/utils/se_layer.py
+mmpretrain/models/utils/swiglu_ffn.py
+mmpretrain/models/utils/tokenizer.py
 mmpretrain/models/utils/vector_quantizer.py
 mmpretrain/models/utils/batch_augments/__init__.py
 mmpretrain/models/utils/batch_augments/cutmix.py
 mmpretrain/models/utils/batch_augments/mixup.py
 mmpretrain/models/utils/batch_augments/resizemix.py
 mmpretrain/models/utils/batch_augments/wrapper.py
 mmpretrain/structures/__init__.py
 mmpretrain/structures/data_sample.py
 mmpretrain/structures/multi_task_data_sample.py
 mmpretrain/structures/utils.py
 mmpretrain/utils/__init__.py
 mmpretrain/utils/analyze.py
 mmpretrain/utils/collect_env.py
+mmpretrain/utils/dependency.py
 mmpretrain/utils/misc.py
 mmpretrain/utils/progress.py
 mmpretrain/utils/setup_env.py
 mmpretrain/visualization/__init__.py
 mmpretrain/visualization/utils.py
 mmpretrain/visualization/visualizer.py
 requirements/docs.txt
 requirements/mminstall.txt
+requirements/multimodal.txt
 requirements/optional.txt
 requirements/readthedocs.txt
 requirements/runtime.txt
 requirements/tests.txt
```

### Comparing `mmpretrain-1.0.0rc7/setup.cfg` & `mmpretrain-1.0.0rc8/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -18,11 +18,16 @@
 default_section = THIRDPARTY
 
 [codespell]
 skip = *.ipynb
 quiet-level = 3
 ignore-words-list = patten,confectionary,nd,ty,formating,dows
 
+[flake8]
+extend-ignore = E251
+per-file-ignores = 
+	*/__init__.py: F401
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mmpretrain-1.0.0rc7/setup.py` & `mmpretrain-1.0.0rc8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -189,9 +189,10 @@
         license='Apache License 2.0',
         install_requires=parse_requirements('requirements/runtime.txt'),
         extras_require={
             'all': parse_requirements('requirements.txt'),
             'tests': parse_requirements('requirements/tests.txt'),
             'optional': parse_requirements('requirements/optional.txt'),
             'mim': parse_requirements('requirements/mminstall.txt'),
+            'multimodal': parse_requirements('requirements/multimodal.txt'),
         },
         zip_safe=False)
```

