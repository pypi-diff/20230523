# Comparing `tmp/shaperone-0.41.3.tar.gz` & `tmp/shaperone-0.41.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaperone-0.41.3.tar", max compression
+gzip compressed data, was "shaperone-0.41.4.tar", max compression
```

## Comparing `shaperone-0.41.3.tar` & `shaperone-0.41.4.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     1081 2023-05-19 12:16:20.410505 shaperone-0.41.3/LICENSE
--rw-r--r--   0        0        0      606 2023-05-23 11:44:08.075958 shaperone-0.41.3/README.md
--rw-r--r--   0        0        0      977 2023-05-23 11:46:17.750369 shaperone-0.41.3/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-19 12:16:22.675245 shaperone-0.41.3/shaperone/.pylintrc2
--rw-r--r--   0        0        0     3259 2023-05-23 11:45:55.264489 shaperone-0.41.3/shaperone/__init__.py
--rw-r--r--   0        0        0    32344 2023-05-23 11:20:06.489661 shaperone-0.41.3/shaperone/_explanation.py
--rw-r--r--   0        0        0     8707 2023-05-23 11:20:06.404107 shaperone-0.41.3/shaperone/_serializable.py
--rw-r--r--   0        0        0       27 2023-05-19 12:16:22.676670 shaperone-0.41.3/shaperone/actions/__init__.py
--rw-r--r--   0        0        0      210 2023-05-19 12:16:22.676909 shaperone-0.41.3/shaperone/actions/_action.py
--rw-r--r--   0        0        0     3636 2023-05-19 12:16:22.677174 shaperone-0.41.3/shaperone/actions/_optimizer.py
--rw-r--r--   0        0        0      214 2023-05-19 12:16:22.677428 shaperone-0.41.3/shaperone/benchmark/__init__.py
--rw-r--r--   0        0        0      289 2023-05-19 12:16:22.677588 shaperone-0.41.3/shaperone/benchmark/_compute.py
--rw-r--r--   0        0        0     8099 2023-05-23 11:20:06.198786 shaperone-0.41.3/shaperone/benchmark/_explanation_error.py
--rw-r--r--   0        0        0     1074 2023-05-19 12:16:22.678044 shaperone-0.41.3/shaperone/benchmark/_result.py
--rw-r--r--   0        0        0    13399 2023-05-23 11:20:06.379830 shaperone-0.41.3/shaperone/benchmark/_sequential.py
--rw-r--r--   0        0        0    14182 2023-05-23 11:20:06.525273 shaperone-0.41.3/shaperone/benchmark/experiments.py
--rw-r--r--   0        0        0     4243 2023-05-23 11:20:06.147074 shaperone-0.41.3/shaperone/benchmark/framework.py
--rw-r--r--   0        0        0    18601 2023-05-19 12:16:22.678958 shaperone-0.41.3/shaperone/benchmark/measures.py
--rw-r--r--   0        0        0     4287 2023-05-19 12:16:22.679149 shaperone-0.41.3/shaperone/benchmark/methods.py
--rw-r--r--   0        0        0    31376 2023-05-19 12:30:35.021854 shaperone-0.41.3/shaperone/benchmark/metrics.py
--rw-r--r--   0        0        0     6513 2023-05-19 12:16:22.679646 shaperone-0.41.3/shaperone/benchmark/models.py
--rw-r--r--   0        0        0    23812 2023-05-23 11:20:06.545890 shaperone-0.41.3/shaperone/benchmark/plots.py
--rw-r--r--   0        0        0    25873 2023-05-19 12:16:22.680237 shaperone-0.41.3/shaperone/cext/_cext.cc
--rw-r--r--   0        0        0     8085 2023-05-19 12:16:22.680403 shaperone-0.41.3/shaperone/cext/_cext_gpu.cc
--rw-r--r--   0        0        0    14595 2023-05-19 12:16:22.680578 shaperone-0.41.3/shaperone/cext/_cext_gpu.cu
--rw-r--r--   0        0        0    62762 2023-05-19 12:16:22.680977 shaperone-0.41.3/shaperone/cext/gpu_treeshap.h
--rw-r--r--   0        0        0    58256 2023-05-19 12:16:22.681320 shaperone-0.41.3/shaperone/cext/tree_shap.h
--rw-r--r--   0        0        0     9612 2023-05-23 11:20:06.172429 shaperone-0.41.3/shaperone/datasets.py
--rw-r--r--   0        0        0      268 2023-05-19 12:16:22.681691 shaperone-0.41.3/shaperone/explainers/__init__.py
--rw-r--r--   0        0        0     8939 2023-05-23 11:20:06.650366 shaperone-0.41.3/shaperone/explainers/_additive.py
--rw-r--r--   0        0        0     6730 2023-05-23 11:20:06.431032 shaperone-0.41.3/shaperone/explainers/_deep/__init__.py
--rw-r--r--   0        0        0    16170 2023-05-19 12:16:22.682286 shaperone-0.41.3/shaperone/explainers/_deep/deep_pytorch.py
--rw-r--r--   0        0        0    35006 2023-05-19 12:27:39.295775 shaperone-0.41.3/shaperone/explainers/_deep/deep_tf.py
--rw-r--r--   0        0        0    16264 2023-05-23 11:20:06.531908 shaperone-0.41.3/shaperone/explainers/_exact.py
--rw-r--r--   0        0        0    23234 2023-05-23 11:20:06.209921 shaperone-0.41.3/shaperone/explainers/_explainer.py
--rw-r--r--   0        0        0     9330 2023-05-19 12:16:22.683710 shaperone-0.41.3/shaperone/explainers/_gpu_tree.py
--rw-r--r--   0        0        0    27238 2023-05-23 11:20:06.613415 shaperone-0.41.3/shaperone/explainers/_gradient.py
--rw-r--r--   0        0        0    31017 2023-05-23 11:20:06.387085 shaperone-0.41.3/shaperone/explainers/_kernel.py
--rw-r--r--   0        0        0    19121 2023-05-23 11:20:06.550266 shaperone-0.41.3/shaperone/explainers/_linear.py
--rw-r--r--   0        0        0    31746 2023-05-23 11:20:06.371080 shaperone-0.41.3/shaperone/explainers/_partition.py
--rw-r--r--   0        0        0    10941 2023-05-23 11:20:06.440928 shaperone-0.41.3/shaperone/explainers/_permutation.py
--rw-r--r--   0        0        0     9255 2023-05-23 11:20:06.408027 shaperone-0.41.3/shaperone/explainers/_sampling.py
--rw-r--r--   0        0        0    93670 2023-05-23 11:20:06.346964 shaperone-0.41.3/shaperone/explainers/_tree.py
--rw-r--r--   0        0        0     5009 2023-05-23 11:20:06.218057 shaperone-0.41.3/shaperone/explainers/mimic.py
--rw-r--r--   0        0        0      163 2023-05-19 12:16:22.686920 shaperone-0.41.3/shaperone/explainers/other/__init__.py
--rw-r--r--   0        0        0      512 2023-05-19 12:16:22.687102 shaperone-0.41.3/shaperone/explainers/other/_coefficent.py
--rw-r--r--   0        0        0     2528 2023-05-23 11:20:06.229050 shaperone-0.41.3/shaperone/explainers/other/_lime.py
--rw-r--r--   0        0        0    11413 2023-05-19 12:16:22.687538 shaperone-0.41.3/shaperone/explainers/other/_maple.py
--rw-r--r--   0        0        0     3344 2023-05-23 11:20:06.541222 shaperone-0.41.3/shaperone/explainers/other/_random.py
--rw-r--r--   0        0        0     1283 2023-05-19 12:16:22.687898 shaperone-0.41.3/shaperone/explainers/other/_treegain.py
--rw-r--r--   0        0        0    20310 2023-05-23 11:20:06.591261 shaperone-0.41.3/shaperone/explainers/pytree.py
--rw-r--r--   0        0        0     2774 2023-05-19 12:16:22.688361 shaperone-0.41.3/shaperone/explainers/tf_utils.py
--rw-r--r--   0        0        0      443 2023-05-19 12:16:22.688609 shaperone-0.41.3/shaperone/links.py
--rw-r--r--   0        0        0      283 2023-05-19 12:16:22.688804 shaperone-0.41.3/shaperone/maskers/__init__.py
--rw-r--r--   0        0        0     5213 2023-05-19 12:16:22.688969 shaperone-0.41.3/shaperone/maskers/_composite.py
--rw-r--r--   0        0        0     1008 2023-05-19 12:16:22.689086 shaperone-0.41.3/shaperone/maskers/_fixed.py
--rw-r--r--   0        0        0     2416 2023-05-23 11:20:06.310200 shaperone-0.41.3/shaperone/maskers/_fixed_composite.py
--rw-r--r--   0        0        0     9543 2023-05-23 11:20:06.506190 shaperone-0.41.3/shaperone/maskers/_image.py
--rw-r--r--   0        0        0      753 2023-05-19 12:27:39.449782 shaperone-0.41.3/shaperone/maskers/_masker.py
--rw-r--r--   0        0        0     2692 2023-05-23 11:20:06.419680 shaperone-0.41.3/shaperone/maskers/_output_composite.py
--rw-r--r--   0        0        0    14131 2023-05-23 11:20:06.204183 shaperone-0.41.3/shaperone/maskers/_tabular.py
--rw-r--r--   0        0        0    21556 2023-05-23 11:20:06.400876 shaperone-0.41.3/shaperone/maskers/_text.py
--rw-r--r--   0        0        0      202 2023-05-19 12:16:22.690658 shaperone-0.41.3/shaperone/models/__init__.py
--rw-r--r--   0        0        0     1498 2023-05-23 11:20:06.485053 shaperone-0.41.3/shaperone/models/_model.py
--rw-r--r--   0        0        0    18717 2023-05-23 11:20:06.423374 shaperone-0.41.3/shaperone/models/_teacher_forcing.py
--rw-r--r--   0        0        0     9978 2023-05-23 11:20:06.537864 shaperone-0.41.3/shaperone/models/_text_generation.py
--rw-r--r--   0        0        0    10116 2023-05-23 11:20:06.266358 shaperone-0.41.3/shaperone/models/_topk_lm.py
--rw-r--r--   0        0        0     1623 2023-05-23 11:20:06.163448 shaperone-0.41.3/shaperone/models/_transformers_pipeline.py
--rw-r--r--   0        0        0      685 2023-05-19 12:16:22.692042 shaperone-0.41.3/shaperone/plots/__init__.py
--rw-r--r--   0        0        0    17309 2023-05-23 11:20:06.167759 shaperone-0.41.3/shaperone/plots/_bar.py
--rw-r--r--   0        0        0    41107 2023-05-23 11:20:06.582131 shaperone-0.41.3/shaperone/plots/_beeswarm.py
--rw-r--r--   0        0        0     9455 2023-05-19 12:16:22.693063 shaperone-0.41.3/shaperone/plots/_benchmark.py
--rw-r--r--   0        0        0    26022 2023-05-23 11:20:06.461304 shaperone-0.41.3/shaperone/plots/_decision.py
--rw-r--r--   0        0        0     2813 2023-05-19 12:16:22.693473 shaperone-0.41.3/shaperone/plots/_embedding.py
--rw-r--r--   0        0        0    19463 2023-05-23 11:20:06.137439 shaperone-0.41.3/shaperone/plots/_force.py
--rw-r--r--   0        0        0    14797 2023-05-23 11:20:06.496409 shaperone-0.41.3/shaperone/plots/_force_matplotlib.py
--rw-r--r--   0        0        0     3121 2023-05-19 12:27:39.370797 shaperone-0.41.3/shaperone/plots/_group_difference.py
--rw-r--r--   0        0        0     6502 2023-05-23 11:20:06.244976 shaperone-0.41.3/shaperone/plots/_heatmap.py
--rw-r--r--   0        0        0    25135 2023-05-23 11:20:06.364945 shaperone-0.41.3/shaperone/plots/_image.py
--rw-r--r--   0        0        0      608 2023-05-19 12:16:22.694518 shaperone-0.41.3/shaperone/plots/_labels.py
--rw-r--r--   0        0        0     2825 2023-05-19 12:16:22.694625 shaperone-0.41.3/shaperone/plots/_monitoring.py
--rw-r--r--   0        0        0     9521 2023-05-19 12:16:22.694768 shaperone-0.41.3/shaperone/plots/_partial_dependence.py
--rw-r--r--   0        0        0    33020 2023-05-23 11:20:06.153574 shaperone-0.41.3/shaperone/plots/_scatter.py
--rw-r--r--   0        0        0    59166 2023-05-23 11:20:06.501966 shaperone-0.41.3/shaperone/plots/_text.py
--rw-r--r--   0        0        0     7616 2023-05-19 12:16:22.695662 shaperone-0.41.3/shaperone/plots/_utils.py
--rw-r--r--   0        0        0    23943 2023-05-23 11:20:06.326960 shaperone-0.41.3/shaperone/plots/_violin.py
--rw-r--r--   0        0        0    26592 2023-05-23 11:20:06.468981 shaperone-0.41.3/shaperone/plots/_waterfall.py
--rw-r--r--   0        0        0      262 2023-05-19 12:16:22.696525 shaperone-0.41.3/shaperone/plots/colors/__init__.py
--rw-r--r--   0        0        0    36754 2023-05-19 12:27:39.309034 shaperone-0.41.3/shaperone/plots/colors/_colorconv.py
--rw-r--r--   0        0        0     5096 2023-05-19 12:16:22.696928 shaperone-0.41.3/shaperone/plots/colors/_colors.py
--rw-r--r--   0        0        0   370829 2023-05-19 12:16:22.704487 shaperone-0.41.3/shaperone/plots/resources/bundle.js
--rw-r--r--   0        0        0      570 2023-05-19 12:16:22.704694 shaperone-0.41.3/shaperone/plots/resources/logoSmallGray.png
--rw-r--r--   0        0        0       31 2023-05-19 12:16:22.704846 shaperone-0.41.3/shaperone/setup.cfg
--rw-r--r--   0        0        0      449 2023-05-19 12:16:22.705057 shaperone-0.41.3/shaperone/utils/__init__.py
--rw-r--r--   0        0        0     8513 2023-05-23 11:20:06.176709 shaperone-0.41.3/shaperone/utils/_clustering.py
--rw-r--r--   0        0        0      591 2023-05-19 12:16:22.705349 shaperone-0.41.3/shaperone/utils/_exceptions.py
--rw-r--r--   0        0        0    10645 2023-05-23 11:20:06.186826 shaperone-0.41.3/shaperone/utils/_general.py
--rw-r--r--   0        0        0     2576 2023-05-19 12:16:22.705705 shaperone-0.41.3/shaperone/utils/_keras.py
--rw-r--r--   0        0        0     7329 2023-05-19 12:16:22.705884 shaperone-0.41.3/shaperone/utils/_legacy.py
--rw-r--r--   0        0        0    21361 2023-05-19 12:32:42.478522 shaperone-0.41.3/shaperone/utils/_masked_model.py
--rw-r--r--   0        0        0     1227 2023-05-19 12:16:22.706555 shaperone-0.41.3/shaperone/utils/_show_progress.py
--rw-r--r--   0        0        0     5562 2023-05-23 11:20:06.428023 shaperone-0.41.3/shaperone/utils/image.py
--rw-r--r--   0        0        0     6494 2023-05-19 12:16:22.706900 shaperone-0.41.3/shaperone/utils/transformers.py
--rw-r--r--   0        0        0     1886 1970-01-01 00:00:00.000000 shaperone-0.41.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-19 12:16:20.410505 shaperone-0.41.4/LICENSE
+-rw-r--r--   0        0        0      631 2023-05-23 11:51:38.933952 shaperone-0.41.4/README.md
+-rw-r--r--   0        0        0      977 2023-05-23 11:53:23.639536 shaperone-0.41.4/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-05-19 12:16:22.675245 shaperone-0.41.4/shaperone/.pylintrc2
+-rw-r--r--   0        0        0     3259 2023-05-23 11:53:16.428283 shaperone-0.41.4/shaperone/__init__.py
+-rw-r--r--   0        0        0    32344 2023-05-23 11:20:06.489661 shaperone-0.41.4/shaperone/_explanation.py
+-rw-r--r--   0        0        0     8707 2023-05-23 11:20:06.404107 shaperone-0.41.4/shaperone/_serializable.py
+-rw-r--r--   0        0        0       27 2023-05-19 12:16:22.676670 shaperone-0.41.4/shaperone/actions/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-19 12:16:22.676909 shaperone-0.41.4/shaperone/actions/_action.py
+-rw-r--r--   0        0        0     3636 2023-05-19 12:16:22.677174 shaperone-0.41.4/shaperone/actions/_optimizer.py
+-rw-r--r--   0        0        0      214 2023-05-19 12:16:22.677428 shaperone-0.41.4/shaperone/benchmark/__init__.py
+-rw-r--r--   0        0        0      289 2023-05-19 12:16:22.677588 shaperone-0.41.4/shaperone/benchmark/_compute.py
+-rw-r--r--   0        0        0     8099 2023-05-23 11:20:06.198786 shaperone-0.41.4/shaperone/benchmark/_explanation_error.py
+-rw-r--r--   0        0        0     1074 2023-05-19 12:16:22.678044 shaperone-0.41.4/shaperone/benchmark/_result.py
+-rw-r--r--   0        0        0    13399 2023-05-23 11:20:06.379830 shaperone-0.41.4/shaperone/benchmark/_sequential.py
+-rw-r--r--   0        0        0    14182 2023-05-23 11:20:06.525273 shaperone-0.41.4/shaperone/benchmark/experiments.py
+-rw-r--r--   0        0        0     4243 2023-05-23 11:20:06.147074 shaperone-0.41.4/shaperone/benchmark/framework.py
+-rw-r--r--   0        0        0    18601 2023-05-19 12:16:22.678958 shaperone-0.41.4/shaperone/benchmark/measures.py
+-rw-r--r--   0        0        0     4287 2023-05-19 12:16:22.679149 shaperone-0.41.4/shaperone/benchmark/methods.py
+-rw-r--r--   0        0        0    31376 2023-05-19 12:30:35.021854 shaperone-0.41.4/shaperone/benchmark/metrics.py
+-rw-r--r--   0        0        0     6513 2023-05-19 12:16:22.679646 shaperone-0.41.4/shaperone/benchmark/models.py
+-rw-r--r--   0        0        0    23812 2023-05-23 11:20:06.545890 shaperone-0.41.4/shaperone/benchmark/plots.py
+-rw-r--r--   0        0        0    25873 2023-05-19 12:16:22.680237 shaperone-0.41.4/shaperone/cext/_cext.cc
+-rw-r--r--   0        0        0     8085 2023-05-19 12:16:22.680403 shaperone-0.41.4/shaperone/cext/_cext_gpu.cc
+-rw-r--r--   0        0        0    14595 2023-05-19 12:16:22.680578 shaperone-0.41.4/shaperone/cext/_cext_gpu.cu
+-rw-r--r--   0        0        0    62762 2023-05-19 12:16:22.680977 shaperone-0.41.4/shaperone/cext/gpu_treeshap.h
+-rw-r--r--   0        0        0    58256 2023-05-19 12:16:22.681320 shaperone-0.41.4/shaperone/cext/tree_shap.h
+-rw-r--r--   0        0        0     9612 2023-05-23 11:20:06.172429 shaperone-0.41.4/shaperone/datasets.py
+-rw-r--r--   0        0        0      268 2023-05-19 12:16:22.681691 shaperone-0.41.4/shaperone/explainers/__init__.py
+-rw-r--r--   0        0        0     8939 2023-05-23 11:20:06.650366 shaperone-0.41.4/shaperone/explainers/_additive.py
+-rw-r--r--   0        0        0     6730 2023-05-23 11:20:06.431032 shaperone-0.41.4/shaperone/explainers/_deep/__init__.py
+-rw-r--r--   0        0        0    16170 2023-05-19 12:16:22.682286 shaperone-0.41.4/shaperone/explainers/_deep/deep_pytorch.py
+-rw-r--r--   0        0        0    35006 2023-05-19 12:27:39.295775 shaperone-0.41.4/shaperone/explainers/_deep/deep_tf.py
+-rw-r--r--   0        0        0    16264 2023-05-23 11:20:06.531908 shaperone-0.41.4/shaperone/explainers/_exact.py
+-rw-r--r--   0        0        0    23234 2023-05-23 11:20:06.209921 shaperone-0.41.4/shaperone/explainers/_explainer.py
+-rw-r--r--   0        0        0     9330 2023-05-19 12:16:22.683710 shaperone-0.41.4/shaperone/explainers/_gpu_tree.py
+-rw-r--r--   0        0        0    27238 2023-05-23 11:20:06.613415 shaperone-0.41.4/shaperone/explainers/_gradient.py
+-rw-r--r--   0        0        0    31017 2023-05-23 11:20:06.387085 shaperone-0.41.4/shaperone/explainers/_kernel.py
+-rw-r--r--   0        0        0    19121 2023-05-23 11:20:06.550266 shaperone-0.41.4/shaperone/explainers/_linear.py
+-rw-r--r--   0        0        0    31746 2023-05-23 11:20:06.371080 shaperone-0.41.4/shaperone/explainers/_partition.py
+-rw-r--r--   0        0        0    10941 2023-05-23 11:20:06.440928 shaperone-0.41.4/shaperone/explainers/_permutation.py
+-rw-r--r--   0        0        0     9255 2023-05-23 11:20:06.408027 shaperone-0.41.4/shaperone/explainers/_sampling.py
+-rw-r--r--   0        0        0    93670 2023-05-23 11:20:06.346964 shaperone-0.41.4/shaperone/explainers/_tree.py
+-rw-r--r--   0        0        0     5009 2023-05-23 11:20:06.218057 shaperone-0.41.4/shaperone/explainers/mimic.py
+-rw-r--r--   0        0        0      163 2023-05-19 12:16:22.686920 shaperone-0.41.4/shaperone/explainers/other/__init__.py
+-rw-r--r--   0        0        0      512 2023-05-19 12:16:22.687102 shaperone-0.41.4/shaperone/explainers/other/_coefficent.py
+-rw-r--r--   0        0        0     2528 2023-05-23 11:20:06.229050 shaperone-0.41.4/shaperone/explainers/other/_lime.py
+-rw-r--r--   0        0        0    11413 2023-05-19 12:16:22.687538 shaperone-0.41.4/shaperone/explainers/other/_maple.py
+-rw-r--r--   0        0        0     3344 2023-05-23 11:20:06.541222 shaperone-0.41.4/shaperone/explainers/other/_random.py
+-rw-r--r--   0        0        0     1283 2023-05-19 12:16:22.687898 shaperone-0.41.4/shaperone/explainers/other/_treegain.py
+-rw-r--r--   0        0        0    20310 2023-05-23 11:20:06.591261 shaperone-0.41.4/shaperone/explainers/pytree.py
+-rw-r--r--   0        0        0     2774 2023-05-19 12:16:22.688361 shaperone-0.41.4/shaperone/explainers/tf_utils.py
+-rw-r--r--   0        0        0      443 2023-05-19 12:16:22.688609 shaperone-0.41.4/shaperone/links.py
+-rw-r--r--   0        0        0      283 2023-05-19 12:16:22.688804 shaperone-0.41.4/shaperone/maskers/__init__.py
+-rw-r--r--   0        0        0     5213 2023-05-19 12:16:22.688969 shaperone-0.41.4/shaperone/maskers/_composite.py
+-rw-r--r--   0        0        0     1008 2023-05-19 12:16:22.689086 shaperone-0.41.4/shaperone/maskers/_fixed.py
+-rw-r--r--   0        0        0     2416 2023-05-23 11:20:06.310200 shaperone-0.41.4/shaperone/maskers/_fixed_composite.py
+-rw-r--r--   0        0        0     9543 2023-05-23 11:20:06.506190 shaperone-0.41.4/shaperone/maskers/_image.py
+-rw-r--r--   0        0        0      753 2023-05-19 12:27:39.449782 shaperone-0.41.4/shaperone/maskers/_masker.py
+-rw-r--r--   0        0        0     2692 2023-05-23 11:20:06.419680 shaperone-0.41.4/shaperone/maskers/_output_composite.py
+-rw-r--r--   0        0        0    14131 2023-05-23 11:20:06.204183 shaperone-0.41.4/shaperone/maskers/_tabular.py
+-rw-r--r--   0        0        0    21556 2023-05-23 11:20:06.400876 shaperone-0.41.4/shaperone/maskers/_text.py
+-rw-r--r--   0        0        0      202 2023-05-19 12:16:22.690658 shaperone-0.41.4/shaperone/models/__init__.py
+-rw-r--r--   0        0        0     1498 2023-05-23 11:20:06.485053 shaperone-0.41.4/shaperone/models/_model.py
+-rw-r--r--   0        0        0    18717 2023-05-23 11:20:06.423374 shaperone-0.41.4/shaperone/models/_teacher_forcing.py
+-rw-r--r--   0        0        0     9978 2023-05-23 11:20:06.537864 shaperone-0.41.4/shaperone/models/_text_generation.py
+-rw-r--r--   0        0        0    10116 2023-05-23 11:20:06.266358 shaperone-0.41.4/shaperone/models/_topk_lm.py
+-rw-r--r--   0        0        0     1623 2023-05-23 11:20:06.163448 shaperone-0.41.4/shaperone/models/_transformers_pipeline.py
+-rw-r--r--   0        0        0      685 2023-05-19 12:16:22.692042 shaperone-0.41.4/shaperone/plots/__init__.py
+-rw-r--r--   0        0        0    17309 2023-05-23 11:20:06.167759 shaperone-0.41.4/shaperone/plots/_bar.py
+-rw-r--r--   0        0        0    41107 2023-05-23 11:20:06.582131 shaperone-0.41.4/shaperone/plots/_beeswarm.py
+-rw-r--r--   0        0        0     9455 2023-05-19 12:16:22.693063 shaperone-0.41.4/shaperone/plots/_benchmark.py
+-rw-r--r--   0        0        0    26022 2023-05-23 11:20:06.461304 shaperone-0.41.4/shaperone/plots/_decision.py
+-rw-r--r--   0        0        0     2813 2023-05-19 12:16:22.693473 shaperone-0.41.4/shaperone/plots/_embedding.py
+-rw-r--r--   0        0        0    19463 2023-05-23 11:20:06.137439 shaperone-0.41.4/shaperone/plots/_force.py
+-rw-r--r--   0        0        0    14797 2023-05-23 11:20:06.496409 shaperone-0.41.4/shaperone/plots/_force_matplotlib.py
+-rw-r--r--   0        0        0     3121 2023-05-19 12:27:39.370797 shaperone-0.41.4/shaperone/plots/_group_difference.py
+-rw-r--r--   0        0        0     6502 2023-05-23 11:20:06.244976 shaperone-0.41.4/shaperone/plots/_heatmap.py
+-rw-r--r--   0        0        0    25135 2023-05-23 11:20:06.364945 shaperone-0.41.4/shaperone/plots/_image.py
+-rw-r--r--   0        0        0      608 2023-05-19 12:16:22.694518 shaperone-0.41.4/shaperone/plots/_labels.py
+-rw-r--r--   0        0        0     2825 2023-05-19 12:16:22.694625 shaperone-0.41.4/shaperone/plots/_monitoring.py
+-rw-r--r--   0        0        0     9521 2023-05-19 12:16:22.694768 shaperone-0.41.4/shaperone/plots/_partial_dependence.py
+-rw-r--r--   0        0        0    33020 2023-05-23 11:20:06.153574 shaperone-0.41.4/shaperone/plots/_scatter.py
+-rw-r--r--   0        0        0    59166 2023-05-23 11:20:06.501966 shaperone-0.41.4/shaperone/plots/_text.py
+-rw-r--r--   0        0        0     7616 2023-05-19 12:16:22.695662 shaperone-0.41.4/shaperone/plots/_utils.py
+-rw-r--r--   0        0        0    23943 2023-05-23 11:20:06.326960 shaperone-0.41.4/shaperone/plots/_violin.py
+-rw-r--r--   0        0        0    26592 2023-05-23 11:20:06.468981 shaperone-0.41.4/shaperone/plots/_waterfall.py
+-rw-r--r--   0        0        0      262 2023-05-19 12:16:22.696525 shaperone-0.41.4/shaperone/plots/colors/__init__.py
+-rw-r--r--   0        0        0    36754 2023-05-19 12:27:39.309034 shaperone-0.41.4/shaperone/plots/colors/_colorconv.py
+-rw-r--r--   0        0        0     5096 2023-05-19 12:16:22.696928 shaperone-0.41.4/shaperone/plots/colors/_colors.py
+-rw-r--r--   0        0        0   370829 2023-05-19 12:16:22.704487 shaperone-0.41.4/shaperone/plots/resources/bundle.js
+-rw-r--r--   0        0        0      570 2023-05-19 12:16:22.704694 shaperone-0.41.4/shaperone/plots/resources/logoSmallGray.png
+-rw-r--r--   0        0        0       31 2023-05-19 12:16:22.704846 shaperone-0.41.4/shaperone/setup.cfg
+-rw-r--r--   0        0        0      449 2023-05-19 12:16:22.705057 shaperone-0.41.4/shaperone/utils/__init__.py
+-rw-r--r--   0        0        0     8513 2023-05-23 11:20:06.176709 shaperone-0.41.4/shaperone/utils/_clustering.py
+-rw-r--r--   0        0        0      591 2023-05-19 12:16:22.705349 shaperone-0.41.4/shaperone/utils/_exceptions.py
+-rw-r--r--   0        0        0    10645 2023-05-23 11:20:06.186826 shaperone-0.41.4/shaperone/utils/_general.py
+-rw-r--r--   0        0        0     2576 2023-05-19 12:16:22.705705 shaperone-0.41.4/shaperone/utils/_keras.py
+-rw-r--r--   0        0        0     7329 2023-05-19 12:16:22.705884 shaperone-0.41.4/shaperone/utils/_legacy.py
+-rw-r--r--   0        0        0    21361 2023-05-19 12:32:42.478522 shaperone-0.41.4/shaperone/utils/_masked_model.py
+-rw-r--r--   0        0        0     1227 2023-05-19 12:16:22.706555 shaperone-0.41.4/shaperone/utils/_show_progress.py
+-rw-r--r--   0        0        0     5562 2023-05-23 11:20:06.428023 shaperone-0.41.4/shaperone/utils/image.py
+-rw-r--r--   0        0        0     6494 2023-05-19 12:16:22.706900 shaperone-0.41.4/shaperone/utils/transformers.py
+-rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 shaperone-0.41.4/PKG-INFO
```

### Comparing `shaperone-0.41.3/LICENSE` & `shaperone-0.41.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/pyproject.toml` & `shaperone-0.41.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shaperone"
-version = "0.41.3"
+version = "0.41.4"
 description = "A patched version of the Shap library aimed to contribute the health and safety of Shap."
 authors = ["Thijs van den Berg <thijs@sitmo.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
 "Operating System :: MacOS",
 "Operating System :: Microsoft :: Windows",
```

### Comparing `shaperone-0.41.3/shaperone/__init__.py` & `shaperone-0.41.4/shaperone/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # flake8: noqa
 
 import warnings
 import sys
 
-__version__ = '0.41.3'
+__version__ = '0.41.4'
 
 # check python version
 if (sys.version_info < (3, 0)):
     warnings.warn("As of version 0.29.0 shaperone only supports Python 3 (not 2)!")
 
 from ._explanation import Explanation, Cohorts
```

### Comparing `shaperone-0.41.3/shaperone/_explanation.py` & `shaperone-0.41.4/shaperone/_explanation.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/_serializable.py` & `shaperone-0.41.4/shaperone/_serializable.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/actions/_optimizer.py` & `shaperone-0.41.4/shaperone/actions/_optimizer.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/_explanation_error.py` & `shaperone-0.41.4/shaperone/benchmark/_explanation_error.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/_result.py` & `shaperone-0.41.4/shaperone/benchmark/_result.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/_sequential.py` & `shaperone-0.41.4/shaperone/benchmark/_sequential.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/experiments.py` & `shaperone-0.41.4/shaperone/benchmark/experiments.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/framework.py` & `shaperone-0.41.4/shaperone/benchmark/framework.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/measures.py` & `shaperone-0.41.4/shaperone/benchmark/measures.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/methods.py` & `shaperone-0.41.4/shaperone/benchmark/methods.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/metrics.py` & `shaperone-0.41.4/shaperone/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/models.py` & `shaperone-0.41.4/shaperone/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/benchmark/plots.py` & `shaperone-0.41.4/shaperone/benchmark/plots.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/cext/_cext.cc` & `shaperone-0.41.4/shaperone/cext/_cext.cc`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/cext/_cext_gpu.cc` & `shaperone-0.41.4/shaperone/cext/_cext_gpu.cc`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/cext/_cext_gpu.cu` & `shaperone-0.41.4/shaperone/cext/_cext_gpu.cu`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/cext/gpu_treeshap.h` & `shaperone-0.41.4/shaperone/cext/gpu_treeshap.h`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/cext/tree_shap.h` & `shaperone-0.41.4/shaperone/cext/tree_shap.h`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/datasets.py` & `shaperone-0.41.4/shaperone/datasets.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_additive.py` & `shaperone-0.41.4/shaperone/explainers/_additive.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_deep/__init__.py` & `shaperone-0.41.4/shaperone/explainers/_deep/__init__.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_deep/deep_pytorch.py` & `shaperone-0.41.4/shaperone/explainers/_deep/deep_pytorch.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_deep/deep_tf.py` & `shaperone-0.41.4/shaperone/explainers/_deep/deep_tf.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_exact.py` & `shaperone-0.41.4/shaperone/explainers/_exact.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_explainer.py` & `shaperone-0.41.4/shaperone/explainers/_explainer.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_gpu_tree.py` & `shaperone-0.41.4/shaperone/explainers/_gpu_tree.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_gradient.py` & `shaperone-0.41.4/shaperone/explainers/_gradient.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_kernel.py` & `shaperone-0.41.4/shaperone/explainers/_kernel.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_linear.py` & `shaperone-0.41.4/shaperone/explainers/_linear.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_partition.py` & `shaperone-0.41.4/shaperone/explainers/_partition.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_permutation.py` & `shaperone-0.41.4/shaperone/explainers/_permutation.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_sampling.py` & `shaperone-0.41.4/shaperone/explainers/_sampling.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/_tree.py` & `shaperone-0.41.4/shaperone/explainers/_tree.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/mimic.py` & `shaperone-0.41.4/shaperone/explainers/mimic.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/other/_coefficent.py` & `shaperone-0.41.4/shaperone/explainers/other/_coefficent.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/other/_lime.py` & `shaperone-0.41.4/shaperone/explainers/other/_lime.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/other/_maple.py` & `shaperone-0.41.4/shaperone/explainers/other/_maple.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/other/_random.py` & `shaperone-0.41.4/shaperone/explainers/other/_random.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/other/_treegain.py` & `shaperone-0.41.4/shaperone/explainers/other/_treegain.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/pytree.py` & `shaperone-0.41.4/shaperone/explainers/pytree.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/explainers/tf_utils.py` & `shaperone-0.41.4/shaperone/explainers/tf_utils.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/maskers/_composite.py` & `shaperone-0.41.4/shaperone/maskers/_composite.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/maskers/_fixed.py` & `shaperone-0.41.4/shaperone/maskers/_fixed.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/maskers/_fixed_composite.py` & `shaperone-0.41.4/shaperone/maskers/_fixed_composite.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/maskers/_image.py` & `shaperone-0.41.4/shaperone/maskers/_image.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/maskers/_masker.py` & `shaperone-0.41.4/shaperone/maskers/_masker.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/maskers/_output_composite.py` & `shaperone-0.41.4/shaperone/maskers/_output_composite.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/maskers/_tabular.py` & `shaperone-0.41.4/shaperone/maskers/_tabular.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/maskers/_text.py` & `shaperone-0.41.4/shaperone/maskers/_text.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/models/_model.py` & `shaperone-0.41.4/shaperone/models/_model.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/models/_teacher_forcing.py` & `shaperone-0.41.4/shaperone/models/_teacher_forcing.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/models/_text_generation.py` & `shaperone-0.41.4/shaperone/models/_text_generation.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/models/_topk_lm.py` & `shaperone-0.41.4/shaperone/models/_topk_lm.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/models/_transformers_pipeline.py` & `shaperone-0.41.4/shaperone/models/_transformers_pipeline.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/__init__.py` & `shaperone-0.41.4/shaperone/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_bar.py` & `shaperone-0.41.4/shaperone/plots/_bar.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_beeswarm.py` & `shaperone-0.41.4/shaperone/plots/_beeswarm.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_benchmark.py` & `shaperone-0.41.4/shaperone/plots/_benchmark.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_decision.py` & `shaperone-0.41.4/shaperone/plots/_decision.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_embedding.py` & `shaperone-0.41.4/shaperone/plots/_embedding.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_force.py` & `shaperone-0.41.4/shaperone/plots/_force.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_force_matplotlib.py` & `shaperone-0.41.4/shaperone/plots/_force_matplotlib.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_group_difference.py` & `shaperone-0.41.4/shaperone/plots/_group_difference.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_heatmap.py` & `shaperone-0.41.4/shaperone/plots/_heatmap.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_image.py` & `shaperone-0.41.4/shaperone/plots/_image.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_labels.py` & `shaperone-0.41.4/shaperone/plots/_labels.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_monitoring.py` & `shaperone-0.41.4/shaperone/plots/_monitoring.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_partial_dependence.py` & `shaperone-0.41.4/shaperone/plots/_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_scatter.py` & `shaperone-0.41.4/shaperone/plots/_scatter.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_text.py` & `shaperone-0.41.4/shaperone/plots/_text.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_utils.py` & `shaperone-0.41.4/shaperone/plots/_utils.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_violin.py` & `shaperone-0.41.4/shaperone/plots/_violin.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/_waterfall.py` & `shaperone-0.41.4/shaperone/plots/_waterfall.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/colors/_colorconv.py` & `shaperone-0.41.4/shaperone/plots/colors/_colorconv.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/colors/_colors.py` & `shaperone-0.41.4/shaperone/plots/colors/_colors.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/resources/bundle.js` & `shaperone-0.41.4/shaperone/plots/resources/bundle.js`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/plots/resources/logoSmallGray.png` & `shaperone-0.41.4/shaperone/plots/resources/logoSmallGray.png`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/utils/_clustering.py` & `shaperone-0.41.4/shaperone/utils/_clustering.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/utils/_exceptions.py` & `shaperone-0.41.4/shaperone/utils/_exceptions.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/utils/_general.py` & `shaperone-0.41.4/shaperone/utils/_general.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/utils/_keras.py` & `shaperone-0.41.4/shaperone/utils/_keras.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/utils/_legacy.py` & `shaperone-0.41.4/shaperone/utils/_legacy.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/utils/_masked_model.py` & `shaperone-0.41.4/shaperone/utils/_masked_model.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/utils/_show_progress.py` & `shaperone-0.41.4/shaperone/utils/_show_progress.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/utils/image.py` & `shaperone-0.41.4/shaperone/utils/image.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/shaperone/utils/transformers.py` & `shaperone-0.41.4/shaperone/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.3/PKG-INFO` & `shaperone-0.41.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaperone
-Version: 0.41.3
+Version: 0.41.4
 Summary: A patched version of the Shap library aimed to contribute the health and safety of Shap.
 License: MIT
 Author: Thijs van den Berg
 Author-email: thijs@sitmo.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
@@ -32,20 +32,20 @@
 Description-Content-Type: text/markdown
 
 
 SHAPerone is a patched fork of [SHAP](https://pypi.org/project/shap)
 
 Current patches:
 
-* patched an [issue](https://github.com/slundberg/shap/issues/2721) with `beeswarmplot` that 
+* patched [issue 2721](https://github.com/slundberg/shap/issues/2721), [pull 2697](https://github.com/slundberg/shap/pull/2697) with `beeswarmplot` that 
 broke compatibility with `matplotlib>3.5.3`
-* removed usage of np.int, bp.bool and np.float [see pull](https://github.com/slundberg/shap/pull/1890). 
-The use of np.int has been depreciated since numpy 1.20.0 and removed in `numpy>=1.24.0`.
+* removed usage of np.int, np.bool and np.float [pull 1890](https://github.com/slundberg/shap/pull/1890). 
+The use of np.int, np.bool and np.float has been depreciated since numpy 1.20.0 and removed in `numpy>=1.24.0`.
 
 ## Install
 
-SHAP can be installed from either [PyPI](https://pypi.org/project/shaperone) or [conda-forge](https://anaconda.org/conda-forge/shap):
+SHAPerone can be installed from [PyPI](https://pypi.org/project/shaperone):
 
 <pre>
 pip install shaperone
 </pre>
```

