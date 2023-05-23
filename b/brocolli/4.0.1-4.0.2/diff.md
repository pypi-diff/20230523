# Comparing `tmp/brocolli-4.0.1.tar.gz` & `tmp/brocolli-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brocolli-4.0.1.tar", last modified: Sun May 14 09:53:51 2023, max compression
+gzip compressed data, was "brocolli-4.0.2.tar", last modified: Tue May 23 11:46:07 2023, max compression
```

## Comparing `brocolli-4.0.1.tar` & `brocolli-4.0.2.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.928557 brocolli-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-14 09:53:41.000000 brocolli-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-14 09:53:51.928557 brocolli-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-14 09:53:41.000000 brocolli-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.912557 brocolli-4.0.1/brocolli/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.912557 brocolli-4.0.1/brocolli/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.924557 brocolli-4.0.1/brocolli/converter/onnx_layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/abs_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/add_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/avgpool_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/avgpool_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/baddbmm_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/base_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/batchnorm_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/bnll_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/cast_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/celu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/chunk_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/clip_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/concat_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/conv_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/conv_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/conv_transpose_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/cosine_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/custom_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/div_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/dropout_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/elu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/elu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/embedding_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/exp_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/exp_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/flatten_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/flatten_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/gelu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/gemm_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/gemm_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/getattr_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/getitem_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/glu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/gru_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/hardsigmoid_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/hardsigmoid_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/hardswish_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/hardswish_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/identity_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/layernorm_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/leakyrelu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/leakyrelu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/linear_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/linear_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/log_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/log_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/lstm_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/matmul_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/max_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/mean_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/min_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/mul_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/neg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/normalize_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/output_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/pad_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/pad_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/permute_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/pooling_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/pooling_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/power_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/prelu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/prelu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/reduction_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/relu6_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/relu6_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/relu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/relu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/reshape_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15246 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/rnn_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/selu_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/selu_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sigmoid_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sigmoid_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sine_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/slice_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/softmax_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/softmax_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/softplus_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/softplus_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/split_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sqrt_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/squeeze_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/stack_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sub_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/sum_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/swish_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/tanh_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/tanh_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/tile_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/transpose_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/unbind_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/unsqueeze_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/upsample_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_layers/upsample_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/onnx_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    57317 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_caffe_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.924557 brocolli-4.0.1/brocolli/converter/pytorch_layer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/glu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/mha.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_layer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/converter/pytorch_onnx_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.924557 brocolli-4.0.1/brocolli/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/fuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/graph_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    13767 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/qconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.928557 brocolli-4.0.1/brocolli/quantization/quantization_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/relu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantization_layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-14 09:53:41.000000 brocolli-4.0.1/brocolli/quantization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 09:53:51.912557 brocolli-4.0.1/brocolli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 09:53:51.000000 brocolli-4.0.1/brocolli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-14 09:53:41.000000 brocolli-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 09:53:51.928557 brocolli-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-14 09:53:41.000000 brocolli-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:46:07.977510 brocolli-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-23 11:45:52.000000 brocolli-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-23 11:46:07.977510 brocolli-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-23 11:45:52.000000 brocolli-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:46:07.957510 brocolli-4.0.2/brocolli/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:46:07.957510 brocolli-4.0.2/brocolli/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/common_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:46:07.973510 brocolli-4.0.2/brocolli/converter/onnx_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/abs_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/add_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/avgpool_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/avgpool_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/baddbmm_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/base_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/batchnorm_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/bnll_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/cast_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/celu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/chunk_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/clip_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/concat_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/conv_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/conv_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/conv_transpose_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/cosine_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/custom_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/div_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/dropout_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/elu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/elu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/embedding_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/exp_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/exp_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/flatten_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/flatten_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/gelu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/gemm_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/gemm_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/getattr_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/getitem_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/glu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/gru_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/hardsigmoid_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/hardsigmoid_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/hardswish_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/hardswish_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/identity_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/layernorm_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/leakyrelu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/leakyrelu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/linear_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/linear_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/log_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/log_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/lstm_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/matmul_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/max_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/mean_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/min_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/mul_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/neg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/normalize_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/output_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/pad_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/pad_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/permute_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/pooling_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/pooling_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/power_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/prelu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/prelu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/reduction_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/relu6_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/relu6_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/relu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/relu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/reshape_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15246 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/rnn_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/selu_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/selu_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/sigmoid_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/sigmoid_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/sine_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/slice_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/softmax_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/softmax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/softplus_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/softplus_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/split_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/sqrt_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/squeeze_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/stack_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/sub_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/sum_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/swish_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/tanh_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/tanh_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/tile_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/transpose_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/unbind_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/unsqueeze_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/upsample_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_layers/upsample_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/onnx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57317 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/pytorch_caffe_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/pytorch_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:46:07.973510 brocolli-4.0.2/brocolli/converter/pytorch_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/pytorch_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/pytorch_layer/glu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/pytorch_layer/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/pytorch_layer/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/pytorch_layer/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/pytorch_layer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/converter/pytorch_onnx_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:46:07.977510 brocolli-4.0.2/brocolli/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/fuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/graph_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/qconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:46:07.977510 brocolli-4.0.2/brocolli/quantization/quantization_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/relu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantization_layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22751 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-23 11:45:52.000000 brocolli-4.0.2/brocolli/quantization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 11:46:07.957510 brocolli-4.0.2/brocolli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-23 11:46:07.000000 brocolli-4.0.2/brocolli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-05-23 11:46:07.000000 brocolli-4.0.2/brocolli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 11:46:07.000000 brocolli-4.0.2/brocolli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 11:46:07.000000 brocolli-4.0.2/brocolli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 11:46:07.000000 brocolli-4.0.2/brocolli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-23 11:45:52.000000 brocolli-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 11:46:07.977510 brocolli-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-23 11:45:52.000000 brocolli-4.0.2/setup.py
```

### Comparing `brocolli-4.0.1/LICENSE` & `brocolli-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/PKG-INFO` & `brocolli-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brocolli
-Version: 4.0.1
+Version: 4.0.2
 Summary: everything in pytorch
 Home-page: https://github.com/inisis/brocolli
 Author: desmond
 Author-email: desmond.yao@buaa.edu.cn
 Project-URL: Bug Tracker, https://github.com/inisis/brocolli/issues
 Keywords: machine-learning,pytorch,caffe,torchfx
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brocolli-4.0.1/README.md` & `brocolli-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/common_utils.py` & `brocolli-4.0.2/brocolli/converter/common_utils.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/__init__.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/add_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/add_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/avgpool_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/avgpool_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/avgpool_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/avgpool_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/baddbmm_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/baddbmm_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/base_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/base_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/batchnorm_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/batchnorm_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/bnll_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/bnll_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/cast_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/cast_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/celu_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/celu_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/chunk_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/chunk_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/clip_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/clip_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/concat_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/concat_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/conv_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/conv_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/conv_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/conv_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/conv_transpose_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/conv_transpose_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/cosine_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/cosine_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/custom_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/custom_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/div_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/div_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/dropout_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/dropout_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/elu_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/elu_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/elu_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/elu_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/embedding_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/embedding_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/exp_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/exp_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/flatten_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/flatten_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/flatten_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/flatten_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/gelu_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/gelu_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/gemm_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/gemm_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/gemm_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/gemm_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/getattr_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/getattr_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/getitem_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/getitem_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/glu_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/glu_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/gru_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/gru_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/hardsigmoid_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/hardsigmoid_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/hardsigmoid_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/hardsigmoid_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/hardswish_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/hardswish_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/hardswish_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/hardswish_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/identity_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/identity_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/input_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/input_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/layernorm_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/layernorm_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/leakyrelu_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/leakyrelu_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/leakyrelu_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/leakyrelu_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/linear_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/linear_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/linear_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/linear_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/log_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/log_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/lstm_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/lstm_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/matmul_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/matmul_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/max_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/max_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/mean_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/mean_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/mul_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/mul_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/neg_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/neg_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/normalize_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/normalize_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/output_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/output_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/pad_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/pad_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/pad_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/pad_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/permute_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/permute_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/pooling_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/pooling_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/pooling_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/pooling_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/power_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/power_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/prelu_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/prelu_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/prelu_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/prelu_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/reduction_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/reduction_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/relu6_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/relu6_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/relu6_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/relu6_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/reshape_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/reshape_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/rnn_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/rnn_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/selu_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/selu_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/sigmoid_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/sigmoid_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/sigmoid_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/sigmoid_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/sine_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/sine_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/slice_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/slice_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/softmax_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/softmax_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/softmax_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/softmax_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/softplus_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/softplus_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/softplus_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/softplus_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/split_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/split_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/sqrt_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/sqrt_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/squeeze_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/squeeze_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/stack_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/stack_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/sum_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/sum_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/swish_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/swish_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/template.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/template.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/tile_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/tile_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/transpose_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/transpose_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/unbind_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/unbind_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/unsqueeze_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/unsqueeze_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/upsample_func.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/upsample_func.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_layers/upsample_layer.py` & `brocolli-4.0.2/brocolli/converter/onnx_layers/upsample_layer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/onnx_utils.py` & `brocolli-4.0.2/brocolli/converter/onnx_utils.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/optimizer.py` & `brocolli-4.0.2/brocolli/converter/optimizer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/pytorch_caffe_parser.py` & `brocolli-4.0.2/brocolli/converter/pytorch_caffe_parser.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/pytorch_graph.py` & `brocolli-4.0.2/brocolli/converter/pytorch_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,10 +162,10 @@
 
     def trace_prune(self, graph_module):
         self.placeholder_prune(graph_module)
 
     def shape_inference(self):
         shape_runner = BrocolliShapeRunner(self.graph_module, self.dynamic_batch)
         if self.concrete_args is not None:
-            shape_runner.run(*self.inputs + tuple(self.concrete_args.values()))
+            shape_runner.run(*self.inputs, tuple(self.concrete_args.values()))
         else:
             shape_runner.run(*self.inputs)
```

### Comparing `brocolli-4.0.1/brocolli/converter/pytorch_layer/layernorm.py` & `brocolli-4.0.2/brocolli/converter/pytorch_layer/layernorm.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/pytorch_layer/mha.py` & `brocolli-4.0.2/brocolli/converter/pytorch_layer/mha.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/pytorch_layer/transformer.py` & `brocolli-4.0.2/brocolli/converter/pytorch_layer/transformer.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/pytorch_layer/utils.py` & `brocolli-4.0.2/brocolli/converter/pytorch_layer/utils.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/converter/pytorch_onnx_parser.py` & `brocolli-4.0.2/brocolli/converter/pytorch_onnx_parser.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/comparator.py` & `brocolli-4.0.2/brocolli/quantization/comparator.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/fuser.py` & `brocolli-4.0.2/brocolli/quantization/fuser.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/graph_modules.py` & `brocolli-4.0.2/brocolli/quantization/graph_modules.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/observer.py` & `brocolli-4.0.2/brocolli/quantization/observer.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,21 @@
         self.min_val.copy_(min_val)
         self.max_val.copy_(max_val)
         return x_orig
 
     @torch.jit.export
     def calculate_qparams(self):
         r"""Calculates the quantization parameters."""
-        return self._calculate_qparams(self.min_val, self.max_val)
+        quant_min, quant_max = self._calculate_qmin_qmax()
+        if self.min_val >= 0:
+            quant_min, quant_max = 0, 255
+
+        max_val_pos = torch.max(self.min_val, self.max_val)
+        scale = max_val_pos / quant_max
+        return scale
 
     @torch.jit.export
     def extra_repr(self):
         return "min_val={}, max_val={}".format(self.min_val, self.max_val)
 
 
 @register_observer
@@ -385,15 +391,14 @@
             )
         else:
             self.s = torch.nn.Parameter(
                 x.detach().abs().mean() * 2 / (self.thd_pos**0.5)
             )
 
     def forward(self, x):
-        print(self.s)
         if self.per_channel:
             s_grad_scale = 1.0 / ((self.thd_pos * x.numel()) ** 0.5)
         else:
             s_grad_scale = 1.0 / ((self.thd_pos * x.numel()) ** 0.5)
         s_scale = grad_scale(self.s, s_grad_scale)
 
         x = x / s_scale
```

### Comparing `brocolli-4.0.1/brocolli/quantization/profiler.py` & `brocolli-4.0.2/brocolli/quantization/profiler.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/qconfig.py` & `brocolli-4.0.2/brocolli/quantization/qconfig.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/quantization_layers/arithmetic.py` & `brocolli-4.0.2/brocolli/quantization/quantization_layers/arithmetic.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/quantization_layers/conv.py` & `brocolli-4.0.2/brocolli/quantization/quantization_layers/conv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
+from loguru import logger
+
 from .base import BaseOperator
 from .utils import _pair, _quantize_weight, _quantize_bias
 from .registry import register_quant_op
 
 _SUPPORTED_PADDING = {"zeros", "reflect"}
 
 
@@ -69,21 +71,21 @@
         else:
             weight_shape = [out_channels, in_channels // self.groups]
         qweight = torch._empty_affine_quantized(
             weight_shape + list(kernel_size),
             scale=1,
             zero_point=0,
             dtype=torch.qint8,
-            **{k: v for k, v in factory_kwargs.items() if k != "dtype"}
+            **{k: v for k, v in factory_kwargs.items() if k != "dtype"},
         )
         bias_float = (
             torch.zeros(
                 out_channels,
                 dtype=torch.float,
-                **{k: v for k, v in factory_kwargs.items() if k != "dtype"}
+                **{k: v for k, v in factory_kwargs.items() if k != "dtype"},
             )
             if bias
             else None
         )
 
         self.weight = qweight
         self.bias = bias_float
@@ -126,42 +128,47 @@
     ):
         r"""Creates a qconv object and returns it."""
         if weight_post_process is None:
             weight_post_process = mod.qconfig.weight()
 
         weight_post_process(mod.weight)
         qweight, wt_scale = _quantize_weight(mod.weight.float(), weight_post_process)
+
         act_scale = activation_pre_process.calculate_qparams()
-        qbias = (
-            _quantize_bias(mod.bias.float(), wt_scale * act_scale)
-            if mod.bias is not None
-            else None
+        logger.debug(
+            f"activation scale: {act_scale}, max_val: {activation_pre_process.max_val}, min_val: {activation_pre_process.min_val}"
         )
         output_scale = activation_post_process.calculate_qparams()
+        logger.debug(
+            f"output scale: {output_scale}, max_val: {activation_post_process.max_val}, min_val: {activation_post_process.min_val}"
+        )
+        qbias = mod.bias.float() if mod.bias is not None else None
 
         assert (
             weight_post_process.dtype == torch.qint8
         ), "Weight observer must have a dtype of qint8"
 
         qconv = cls(
             mod.in_channels,
             mod.out_channels,
-            mod.kernel_size,  # type: ignore[call-arg]
+            mod.kernel_size,
             mod.stride,
             mod.padding,
             mod.dilation,
             mod.groups,
-            mod.bias is not None,
+            None,
             mod.padding_mode,
         )
 
         qconv.qbit = mod.activation_pre_process.qbit
         qconv.weight = torch.nn.Parameter(qweight, requires_grad=False)
         if mod.bias is not None:
-            qconv.bias = torch.nn.Parameter(qbias, requires_grad=False)
+            qconv.bias = torch.nn.Parameter(
+                qbias.reshape(1, -1, 1, 1), requires_grad=False
+            )
         qconv.act_scale = torch.Tensor(act_scale).to(qweight.device)
         qconv.wt_scale = torch.Tensor(wt_scale).reshape(1, -1, 1, 1).to(qweight.device)
         qconv.output_scale = torch.Tensor(output_scale).to(qweight.device)
         qconv.output_min_value = activation_post_process.min_val
         qconv.output_max_value = activation_post_process.max_val
 
         return qconv
@@ -218,34 +225,39 @@
             padding,
             dilation,
             False,
             _pair(0),
             groups,
             bias,
             padding_mode,
-            **factory_kwargs
+            **factory_kwargs,
         )
 
     def _get_name(self):
         return "QuantizedConv2d"
 
     def forward(self, input):
         if len(input.shape) != 4:
             raise ValueError("Input shape must be `(N, C, H, W)`!")
 
         out = F.conv2d(
             input.to(torch.double),
             self.weight.to(torch.double),
-            self.bias.to(torch.double) if self.bias is not None else None,
+            None,
             self.stride,
             self.padding,
             self.dilation,
             self.groups,
         )
-        out = out * self.act_scale * self.wt_scale / self.output_scale
+
+        if self.bias is not None:
+            out = (out * self.act_scale * self.wt_scale + self.bias) / self.output_scale
+        else:
+            out = out * self.act_scale * self.wt_scale / self.output_scale
+
         out = self.clamp(out)
 
         return out
 
     @classmethod
     def from_float(cls, mod):
         r"""Creates a quantized module from a float module or qparams_dict.
```

### Comparing `brocolli-4.0.1/brocolli/quantization/quantization_layers/input.py` & `brocolli-4.0.2/brocolli/quantization/quantization_layers/input.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/quantization_layers/linear.py` & `brocolli-4.0.2/brocolli/quantization/quantization_layers/linear.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/quantization_layers/output.py` & `brocolli-4.0.2/brocolli/quantization/quantization_layers/output.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/quantization_layers/pooling.py` & `brocolli-4.0.2/brocolli/quantization/quantization_layers/pooling.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/quantization_layers/relu.py` & `brocolli-4.0.2/brocolli/quantization/quantization_layers/relu.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/quantization_layers/utils.py` & `brocolli-4.0.2/brocolli/quantization/quantization_layers/utils.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli/quantization/quantizer.py` & `brocolli-4.0.2/brocolli/quantization/quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,41 +46,41 @@
 
         return m.__module__.startswith("torch.nn") and not isinstance(
             m, torch.nn.Sequential
         )
 
 
 class PytorchQuantizer:
-    def __init__(self, model, input_shape, concrete_args=None, level=1):
+    def __init__(self, model, input_shape, concrete_args=None, log_level=1):
         super(PytorchQuantizer, self).__init__()
         self.model = model.eval()
         self.device = next(self.model.parameters()).device
         self.input_shape = input_shape
         if isinstance(input_shape, (tuple, list)) and all(
             isinstance(element, int) for element in input_shape
         ):
             self.input_shape = [input_shape]
         self.concrete_args = concrete_args
         self.qconfig = None
         self.qconfig_dict = {"": self.qconfig}
-        self.init_logging(level)
+        self.init_logging(log_level)
         self.graph_module = self.get_graph_module(self.model, self.concrete_args, False)
         self.modules = dict(self.graph_module.named_modules())
         self.print_tabular(self.graph_module)
         self.quant_ops = get_default_quant_ops()
 
-    def init_logging(self, level):
+    def init_logging(self, log_level):
         logger.remove()
-        if level == 0:
+        if log_level == 0:
             logger.add(sys.stderr, level="DEBUG")
-        elif level == 1:
+        elif log_level == 1:
             logger.add(sys.stderr, level="INFO")
-        elif level == 2:
+        elif log_level == 2:
             logger.add(sys.stderr, level="WARNING")
-        elif level == 3:
+        elif log_level == 3:
             logger.add(sys.stderr, level="ERROR")
         else:
             raise Exception("level must be 0, 1, 2 or 3")
 
     def get_graph_module(self, model, concrete_args, inplace=True):
         if not inplace:
             model = copy.deepcopy(model)
@@ -275,16 +275,14 @@
                     new_node = graph_module.graph.call_module(
                         node.name + "_observer", (node,), type_expr="observer"
                     )
                 for user in users:
                     user.replace_input_with(node, new_node)
 
         self.observed_model = torch.fx.GraphModule(graph_module, graph_module.graph)
-        # self.observed_model.graph.print_tabular()
-        # raise
 
     def finetune(self, train_func):
         for name, param in self.observed_model.named_parameters():
             if not "observer" in name:
                 param.requires_grad_(False)
 
         train_func(self.observed_model)
@@ -449,15 +447,15 @@
             torch.save(mdl.state_dict(), "tmp.pt")
             print("%.2f MB" % (os.path.getsize("tmp.pt") / 1e6))
             os.remove("tmp.pt")
 
         print_model_size(self.graph_module)
         print_model_size(self.quanted_model)
 
-    def compare(self):
+    def compare(self, interrested_node=None):
         logger.info("float runs")
         if hasattr(self, "fused_model"):
             float_model = self.fused_model
         else:
             float_model = self.graph_module
 
         prof_float = FXComparator(float_model)
@@ -472,14 +470,17 @@
         quant_node_dict = _node_dict(quanted_model)
 
         def compare(float_node_dict, quant_node_dict, float_model, quanted_model):
             quanted_modules = dict(quanted_model.named_modules())
             node_compare_specs = []
             for quanted_name in self.op_maps.keys():
                 float_name = self.op_maps[quanted_name]
+                logger.debug(
+                    f"compare float op : {float_name} and quanted op: {quanted_name}"
+                )
                 float_node = float_node_dict[float_name]
                 quant_node = quant_node_dict[quanted_name]
 
                 with torch.no_grad():
                     if quant_node.op == "call_module":
                         module = quanted_modules[quant_node.target]
                         float_data = float_node.meta["tensor_meta"]["tensor"].flatten()
@@ -491,18 +492,66 @@
                         mre = (
                             torch.abs(quant_data - float_data).sum()
                             * 100.0
                             / torch.abs(float_data).sum()
                         )
                         if float_node.op == "placeholder":
                             quanted_name = float_node.name
-                        node_compare_specs.append([quanted_name, cos_sim, mre])
+
+                        re = (
+                            torch.abs(quant_data - float_data)
+                            * 100.0
+                            / torch.abs(float_data)
+                        )
+                        re = torch.nan_to_num(re)
+                        total = len(float_data.flatten())
+                        section_0_1 = (re < 1).sum() * 100.0 / total
+                        section_1_10 = ((1 <= re) * (re < 10)).sum() * 100.0 / total
+                        section_10_50 = ((10 <= re) * (re < 50)).sum() * 100.0 / total
+                        section_50_100 = ((50 <= re) * (re < 100)).sum() * 100.0 / total
+                        section_100 = (100 <= re).sum() * 100.0 / total
+
+                        node_compare_specs.append(
+                            [
+                                quanted_name,
+                                cos_sim,
+                                mre,
+                                section_0_1,
+                                section_1_10,
+                                section_10_50,
+                                section_50_100,
+                                section_100,
+                            ]
+                        )
+                        if (
+                            interrested_node is not None
+                            and quanted_name in interrested_node
+                        ):
+                            import plotext as plt
+
+                            plt.theme("matrix")
+                            plt.subplots(1, 2)
+                            plt.subplot(1, 1)
+                            plt.hist(float_data.numpy(), bins=256)
+                            plt.subplot(1, 2)
+                            plt.hist(quant_data.numpy(), bins=256)
+                            plt.show()
+                            plt.savefig("plot.txt")
 
             logger.info(
                 tabulate(
                     node_compare_specs,
-                    headers=["\nname", "\ncos_sim", "\nmre"],
+                    headers=[
+                        "\nname",
+                        "\ncos_sim",
+                        "\nmre",
+                        "\nrelative error[0-1)",
+                        "\nrelative error[1-10)",
+                        "\nrelative error[10-50)",
+                        "\nrelative error[50-100)",
+                        "\nrelative error[100-inf)",
+                    ],
                     floatfmt=".4f",
                 )
             )
 
         compare(float_node_dict, quant_node_dict, float_model, quanted_model)
```

### Comparing `brocolli-4.0.1/brocolli/quantization/utils.py` & `brocolli-4.0.2/brocolli/quantization/utils.py`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/brocolli.egg-info/PKG-INFO` & `brocolli-4.0.2/brocolli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brocolli
-Version: 4.0.1
+Version: 4.0.2
 Summary: everything in pytorch
 Home-page: https://github.com/inisis/brocolli
 Author: desmond
 Author-email: desmond.yao@buaa.edu.cn
 Project-URL: Bug Tracker, https://github.com/inisis/brocolli/issues
 Keywords: machine-learning,pytorch,caffe,torchfx
 Classifier: Programming Language :: Python :: 3
```

### Comparing `brocolli-4.0.1/brocolli.egg-info/SOURCES.txt` & `brocolli-4.0.2/brocolli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brocolli-4.0.1/setup.py` & `brocolli-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="brocolli",
-    version="4.0.1",
+    version="4.0.2",
     author="desmond",
     author_email="desmond.yao@buaa.edu.cn",
     description="everything in pytorch",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/inisis/brocolli",
     install_requires=["loguru", "onnx==1.9.0", "onnxruntime==1.8.0", "tabulate"],
```

