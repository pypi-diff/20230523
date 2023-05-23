# Comparing `tmp/pyglove-0.3.1.dev20230521.tar.gz` & `tmp/pyglove-0.3.1.dev20230522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230521.tar", last modified: Sun May 21 08:06:26 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230522.tar", last modified: Mon May 22 08:07:03 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230521.tar` & `pyglove-0.3.1.dev20230522.tar`

### file list

```diff
@@ -1,192 +1,194 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.239312 pyglove-0.3.1.dev20230521/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-21 08:06:26.239312 pyglove-0.3.1.dev20230521/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-21 08:06:24.000000 pyglove-0.3.1.dev20230521/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.223312 pyglove-0.3.1.dev20230521/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.223312 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.227312 pyglove-0.3.1.dev20230521/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.231312 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/compounding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/compounding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23864 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28989 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34356 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    77608 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.231312 pyglove-0.3.1.dev20230521/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.231312 pyglove-0.3.1.dev20230521/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    49302 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79366 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.235312 pyglove-0.3.1.dev20230521/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.235312 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.235312 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.235312 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.239312 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 08:06:26.219312 pyglove-0.3.1.dev20230521/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 08:06:26.000000 pyglove-0.3.1.dev20230521/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 08:06:26.239312 pyglove-0.3.1.dev20230521/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-21 08:06:10.000000 pyglove-0.3.1.dev20230521/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.056222 pyglove-0.3.1.dev20230522/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-22 08:07:03.056222 pyglove-0.3.1.dev20230522/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-22 08:06:58.000000 pyglove-0.3.1.dev20230522/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.024222 pyglove-0.3.1.dev20230522/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.024222 pyglove-0.3.1.dev20230522/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.028222 pyglove-0.3.1.dev20230522/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.032222 pyglove-0.3.1.dev20230522/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.036222 pyglove-0.3.1.dev20230522/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.044222 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.044222 pyglove-0.3.1.dev20230522/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.048222 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72533 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/compounding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/compounding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/contextual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/contextual_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33112 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58261 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23864 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28989 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27492 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52333 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34428 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80848 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.048222 pyglove-0.3.1.dev20230522/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49538 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79366 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.052222 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.056222 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:07:03.024222 pyglove-0.3.1.dev20230522/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 08:07:02.000000 pyglove-0.3.1.dev20230522/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:07:03.056222 pyglove-0.3.1.dev20230522/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-22 08:06:36.000000 pyglove-0.3.1.dev20230522/setup.py
```

### Comparing `pyglove-0.3.1.dev20230521/LICENSE` & `pyglove-0.3.1.dev20230522/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/PKG-INFO` & `pyglove-0.3.1.dev20230522/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230521
+Version: 0.3.1.dev20230522
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230521/README.md` & `pyglove-0.3.1.dev20230522/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,17 @@
 List = symbolic.List
 list = List   # pylint: disable=redefined-builtin
 
 Object = symbolic.Object
 ClassWrapper = symbolic.ClassWrapper
 Functor = symbolic.Functor
 
+# Contextual value marker.
+Contextual = symbolic.Contextual
+
 # Decorator for declaring symbolic. members for `pg.Object`.
 members = symbolic.members
 
 #
 # Methods for making symbolic types.
 #
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230522/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230522/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230522/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230522/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230522/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,17 @@
 from pyglove.core.symbolic.base import from_json
 from pyglove.core.symbolic.base import from_json_str
 from pyglove.core.symbolic.base import to_json
 from pyglove.core.symbolic.base import to_json_str
 from pyglove.core.symbolic.base import load
 from pyglove.core.symbolic.base import save
 
+# Marker for contextual values.
+from pyglove.core.symbolic.contextual import Contextual
+
 # Interfaces for pure symbolic objects.
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 
 # Symbolic helper classes.
 from pyglove.core.symbolic.base import FieldUpdate
 from pyglove.core.symbolic.base import DescendantQueryOption
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 import abc
 import copy
 import enum
 import inspect
 import json
 import re
 import sys
-from typing import Any, Callable, Dict, Iterator, List, Optional, Type, Union, Tuple
+import typing
+from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Type, Union
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import flags
+from pyglove.core.symbolic.contextual import Contextual
 from pyglove.core.symbolic.origin import Origin
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
 
 class WritePermissionError(Exception):
   """Exception raisen when write access to object fields is not allowed."""
@@ -345,23 +347,23 @@
       default: Any = object_utils.MISSING_VALUE) -> Any:
     """Returns a sub-node by path.
 
     NOTE: there is no `sym_set`, use `sym_rebind`.
 
     Args:
       path: A KeyPath object or equivalence.
-      default: Default value if path does not exists. If absent, `KeyError`
-        will be thrown.
+      default: Default value if path does not exists. If absent, `KeyError` will
+        be thrown.
 
     Returns:
       Value of symbolic attribute specified by path if found, otherwise the
       default value if it's specified.
 
     Raises:
-      KeyError if `path` does not exist and default value is `pg.MISSING_VALUE`.
+      KeyError if `path` does not exist and `default` is `pg.MISSING_VALUE`.
     """
     path = object_utils.KeyPath.from_value(path)
     if default == object_utils.MISSING_VALUE:
       return path.query(self)
     else:
       return path.get(self, default)
 
@@ -374,31 +376,110 @@
       key: Union[str, int],
       default: Any = object_utils.MISSING_VALUE) -> Any:
     """Gets a symbolic attribute.
 
     Args:
       key: Key of symbolic attribute.
       default: Default value if attribute does not exist. If absent,
-        `AttributeError` will be thrown.
 
     Returns:
       Value of symbolic attribute if found, otherwise the default value
       if it's specified.
 
     Raises:
-      AttributeError if `key` does not exist.
+      AttributeError if `key` does not exist and `default` is
+        ``pg.MISSING_VALUE``.
     """
     if not self.sym_hasattr(key):
       if default != object_utils.MISSING_VALUE:
         return default
       raise AttributeError(
           self._error_message(
               f'{self.__class__!r} object has no symbolic attribute {key!r}.'))
     return self._sym_getattr(key)
 
+  def sym_contextual_hasattr(
+      self,
+      key: Union[str, int],
+      getter: Optional[Contextual] = None,
+      start: Union[
+          'Symbolic', object_utils.MissingValue
+      ] = pg_typing.MISSING_VALUE,
+  ) -> bool:
+    """Returns True if an attribute exists from current object's context.
+
+    Args:
+      key: Key of symbolic attribute.
+      getter: An optional ``Contextual`` object as the value retriever.
+      start: An object from current object to the root of the composition as the
+        starting point of context lookup (upward). If ``pg.MISSING_VALUE``, it
+        will start with current node.
+
+    Returns:
+      True if the attribute exists. Otherwise False.
+    """
+    v = self.sym_contextual_getattr(
+        key, default=(pg_typing.MISSING_VALUE,), getter=getter, start=start
+    )
+    return v != (pg_typing.MISSING_VALUE,)
+
+  def sym_contextual_getattr(
+      self,
+      key: Union[str, int],
+      default: Any = object_utils.MISSING_VALUE,
+      getter: Optional[Contextual] = None,
+      start: Union[
+          'Symbolic', object_utils.MissingValue
+      ] = pg_typing.MISSING_VALUE,
+  ) -> Any:
+    """Gets a key from current object's context (symbolic parent chain).
+
+    Args:
+      key: Key of symbolic attribute.
+      default: Default value if attribute does not exist. If absent,
+        `AttributeError` will be thrown.
+      getter: An optional ``Contextual`` object as the value retriever.
+      start: An object from current object to the root of the composition as the
+        starting point of context lookup (upward). If ``pg.MISSING_VALUE``, it
+        will start with current node.
+
+    Returns:
+      Value of symbolic attribute if found, otherwise the default value
+      if it's specified.
+
+    Raises:
+      AttributeError if `key` does not exist along the parent chain and
+        default value is not ``pg.MISSING_VALUE``.
+    """
+    getter = getter or Contextual()
+    if start == pg_typing.MISSING_VALUE:
+      current = self
+    else:
+      current = typing.cast(Symbolic, start)
+
+    while current is not None:
+      v = getter.value_from(key, current)
+      # NOTE(daiyip): when the contextual value from the parent returns
+      # another contextual object, we should follow the new return value's
+      # instruction instead of the original one.
+      if isinstance(v, Contextual):
+        getter = v
+      elif v != object_utils.MISSING_VALUE:
+        return v
+      current = current.sym_parent
+
+    if default != object_utils.MISSING_VALUE:
+      return default
+    raise AttributeError(
+        self._error_message(
+            f'`{key}` is not found under its context '
+            '(along its symbolic parent chain).'
+        )
+    )
+
   @abc.abstractmethod
   def sym_keys(self) -> Iterator[Union[str, int]]:
     """Iterates the keys of symbolic attributes."""
 
   @abc.abstractmethod
   def sym_values(self) -> Iterator[Any]:
     """Iterates the values of symbolic attributes."""
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/boilerplate.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/class_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/compounding.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/compounding.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/compounding_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/compounding_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import typing
 from typing import Any, Callable, Iterable, Iterator, List, Optional, Sequence, Set, Tuple, Union
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
+from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
 
 
 class Dict(dict, base.Symbolic, pg_typing.CustomTyping):
   """Symbolic dict.
 
   ``pg.Dict`` implements a dict type whose instances are symbolically
@@ -193,16 +194,18 @@
     # check in nested structures, which takes effect only when value_spec
     # is not None.
     pass_through = kwargs.pop('pass_through', False)
 
     # If True, the parent of dict items should be set to `self.sym_parent`,
     # This is useful when Dict is used as the field container of
     # pg.Object.
-    self._set_raw_attr('_pass_through_parent',
-                       kwargs.pop('pass_through_parent', False))
+    self._set_raw_attr(
+        '_as_object_attributes_container',
+        kwargs.pop('as_object_attributes_container', False),
+    )
 
     if dict_obj is not None:
       dict_obj = dict(dict_obj)
 
     # NOTE(daiyip): we call __init__ of superclasses explicitly instead of
     # calling super().__init__(...) since dict.__init__ does
     # not follow super(...).__init__ fashion, which will lead to
@@ -432,43 +435,43 @@
         for key in super().__iter__():
           if key not in traversed:
             yield key
 
   def sym_values(self) -> Iterator[Any]:
     """Iterates the values of symbolic attributes."""
     for k in self.sym_keys():
-      yield self[k]
+      yield self._sym_getattr(k)
 
   def sym_items(self) -> Iterator[
       Tuple[str, Any]]:
     """Iterates the (key, value) pairs of symbolic attributes."""
     for k in self.sym_keys():
-      yield k, self[k]
+      yield k, self._sym_getattr(k)
 
   def sym_setparent(self, parent: base.Symbolic):
     """Override set parent of Dict to handle the passing through scenario."""
     super().sym_setparent(parent)
-    # NOTE(daiyip): when flag `pass_through_parent` is on, it sets the parent
-    # of child symbolic values using its parent.
-    if self._pass_through_parent:
+    # NOTE(daiyip): when flag `as_object_attributes_container` is on, it sets
+    # the parent of child symbolic values using its parent.
+    if self._as_object_attributes_container:
       for v in self.values():
         if isinstance(v, base.Symbolic):
           v.sym_setparent(parent)
 
   def sym_hash(self) -> int:
     """Symbolic hashing."""
     return base.sym_hash(
         (self.__class__,
          tuple([base.sym_hash((k, v)) for k, v in self.sym_items()
                 if v != pg_typing.MISSING_VALUE])))
 
   def _sym_getattr(  # pytype: disable=signature-mismatch  # overriding-parameter-type-checks
       self, key: str) -> Any:
     """Gets symbolic attribute by key."""
-    return self[key]
+    return super().__getitem__(key)
 
   def _sym_clone(self, deep: bool, memo=None) -> 'Dict':
     """Override Symbolic._sym_clone."""
     source = dict()
     for k, v in self.items():
       if deep or isinstance(v, base.Symbolic):
         v = base.clone(v, deep, memo)
@@ -569,14 +572,28 @@
 
   def _on_change(self, field_updates: typing.Dict[object_utils.KeyPath,
                                                   base.FieldUpdate]):
     """On change event of Dict."""
     if self._onchange_callback:
       self._onchange_callback(field_updates)
 
+  def __getitem__(self, key: str) -> Any:
+    """Get item in this Dict."""
+    v = super().__getitem__(key)
+    if isinstance(v, contextual.Contextual):
+      start = self.sym_parent
+      # NOTE(daiyip): The parent of `pg.Object`'s attribute dict points to
+      # the `pg.Object` instance once it's set up. Here we let the ancester
+      # traversal to bypass `pg.Object` to avoid double entry, which causes
+      # dead loop.
+      if self._as_object_attributes_container and self.sym_parent:
+        start = start.sym_parent
+      v = self.sym_contextual_getattr(key, getter=v, start=start)
+    return v
+
   def __setitem__(self, key: str, value: Any) -> None:
     """Set item in this Dict.
 
     Args:
       key: String key. (Please be noted that key path is not supported.)
       value: Value to be inserted.
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/dict_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 from pyglove.core.symbolic import object as pg_object
+from pyglove.core.symbolic.contextual import Contextual
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
 
 MISSING_VALUE = object_utils.MISSING_VALUE
@@ -1347,14 +1348,25 @@
     sd = Dict(a=Dict())
     self.assertFalse(sd.is_sealed)
     self.assertFalse(sd.a.is_sealed)
     sd.seal()
     self.assertTrue(sd.is_sealed)
     self.assertTrue(sd.a.is_sealed)
 
+  def test_contextual(self):
+    sd = Dict(x=Contextual())
+    with self.assertRaisesRegex(
+        AttributeError, '`x` is not found under its context'
+    ):
+      _ = sd.x
+
+    p = Dict(x=Dict(p='foo'), y=Dict(z=sd))
+    self.assertEqual(sd.x, Dict(p='foo'))
+    self.assertIs(p.x, sd.x)
+
 
 class RebindTest(unittest.TestCase):
   """Dedicated tests for `pg.Dict.rebind`."""
 
   def test_rebind_on_schemaless_dicts(self):
     sd = Dict(a=Dict(b=1, c=2), d=3)
     sd.rebind({
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/functor.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/functor_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Symbolic list."""
 
 import dataclasses
 import math
 import typing
-
 from typing import Any, Callable, Dict, Iterable, Iterator, Optional, Tuple, Union
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
+from pyglove.core.symbolic import contextual
 from pyglove.core.symbolic import flags
 
 
 class List(list, base.Symbolic, pg_typing.CustomTyping):
   """Symbolic list.
 
   ``pg.List`` implements a list type whose instances are symbolically
@@ -457,15 +457,22 @@
     for idx, item in enumerate(self):
       if isinstance(item, base.Symbolic) and item.sym_path.key != idx:
         item.sym_setpath(object_utils.KeyPath(idx, self.sym_path))
 
     if self._onchange_callback is not None:
       self._onchange_callback(field_updates)
 
-  def __setitem__(self, index: int, value: Any) -> None:
+  def __getitem__(self, index) -> Any:
+    """Gets the item at a given position."""
+    v = super().__getitem__(index)
+    if isinstance(v, contextual.Contextual):
+      v = self.sym_contextual_getattr(index, getter=v, start=self.sym_parent)
+    return v
+
+  def __setitem__(self, index, value: Any) -> None:
     """Set item in this List."""
     if base.treats_as_sealed(self):
       raise base.WritePermissionError(
           self._error_message('Cannot set item for a sealed List.'))
 
     if not base.writtable_via_accessors(self):
       raise base.WritePermissionError(
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/list_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import unittest
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 from pyglove.core.symbolic import object as pg_object
+from pyglove.core.symbolic.contextual import Contextual
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.list import Insertion
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
 from pyglove.core.symbolic.pure_symbolic import PureSymbolic
 
 
@@ -1148,14 +1149,28 @@
     sl = List([[]])
     self.assertFalse(sl.is_sealed)
     self.assertFalse(sl[0].is_sealed)
     sl.seal()
     self.assertTrue(sl.is_sealed)
     self.assertTrue(sl[0].is_sealed)
 
+  def test_contextual(self):
+    # Test contextual access for schemaless list.
+    # Okay: sl[1] is contextual.
+    sl = List([0, Contextual(lambda i, x: x.a)])
+
+    self.assertEqual(sl[0], 0)
+    with self.assertRaisesRegex(
+        AttributeError, '`1` is not found under its context'
+    ):
+      _ = sl[1]
+
+    sd = Dict(x=sl, a=Dict(y=2))
+    self.assertIs(sl[1], sd.a)
+
 
 class RebindTest(unittest.TestCase):
   """Dedicated tests for `pg.List.rebind`."""
 
   def test_rebind_on_schemaless_lists(self):
     sl = List(['foo', 2, {}, []])
     sl.rebind({
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,22 +542,26 @@
       if missing_args:
         arg_phrase = object_utils.auto_plural(len(missing_args), 'argument')
         keys_str = object_utils.comma_delimited_str(missing_args)
         raise TypeError(
             f'{self.__class__.__name__}.__init__() missing {len(missing_args)} '
             f'required {arg_phrase}: {keys_str}.')
 
-    self._set_raw_attr('_sym_attributes', pg_dict.Dict(
-        field_args,
-        value_spec=self.__class__.sym_fields,
-        allow_partial=allow_partial,
-        sealed=sealed,
-        accessor_writable=self.__class__.allow_symbolic_assignment,
-        root_path=root_path,
-        pass_through_parent=True))
+    self._set_raw_attr(
+        '_sym_attributes',
+        pg_dict.Dict(
+            field_args,
+            value_spec=self.__class__.sym_fields,
+            allow_partial=allow_partial,
+            sealed=sealed,
+            accessor_writable=self.__class__.allow_symbolic_assignment,
+            root_path=root_path,
+            as_object_attributes_container=True,
+        ),
+    )
     self._sym_attributes.sym_setparent(self)
     self._on_init()
     self.seal(sealed)
 
   #
   # Events that subclasses can override.
   #
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/object_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 from pyglove.core.symbolic.base import query as pg_query
 from pyglove.core.symbolic.base import traverse as pg_traverse
+from pyglove.core.symbolic.contextual import Contextual
 from pyglove.core.symbolic.dict import Dict
 from pyglove.core.symbolic.functor import functor as pg_functor
 from pyglove.core.symbolic.list import List
 from pyglove.core.symbolic.object import members as pg_members
 from pyglove.core.symbolic.object import Object
 from pyglove.core.symbolic.origin import Origin
 from pyglove.core.symbolic.pure_symbolic import NonDeterministic
@@ -711,14 +712,80 @@
 
     self.assertEqual(b.sym_getattr('x1'), 1)
     self.assertEqual(b.sym_getattr('x2'), 2)
     with self.assertRaisesRegex(
         AttributeError, 'has no symbolic attribute \'y\''):
       _ = b.sym_getattr('y')
 
+  def test_sym_contextual_hasattr(self):
+    class A(Object):
+      x: int
+      y: int = 1
+      z: int = Contextual()
+
+    a = A(0)
+    _ = Dict(p=Dict(a=a, b=3), z=2)
+    self.assertTrue(a.sym_contextual_hasattr('x'))
+    self.assertTrue(a.sym_contextual_hasattr('y'))
+    self.assertTrue(a.sym_contextual_hasattr('z'))
+
+    # Custom start.
+    self.assertFalse(a.sym_contextual_hasattr('x', start=a.sym_parent))
+    self.assertFalse(a.sym_contextual_hasattr('y', start=a.sym_parent))
+    self.assertTrue(a.sym_contextual_hasattr('z', start=a.sym_parent))
+
+    # Custom getter.
+    getter = Contextual(lambda k, p: getattr(p, 'b'))
+    self.assertTrue(a.sym_contextual_hasattr('x', getter, start=a.sym_parent))
+    self.assertTrue(a.sym_contextual_hasattr('y', getter, start=a.sym_parent))
+    self.assertTrue(a.sym_contextual_hasattr('z', getter, start=a.sym_parent))
+
+  def test_sym_contextual_getattr(self):
+    class A(Object):
+      x: int
+      y: int = 1
+      z: int = Contextual()
+
+    a = A(0)
+
+    with self.assertRaises(AttributeError):
+      _ = a.z
+
+    _ = Dict(p=Dict(a=a, b=3), z=2)
+    self.assertEqual(a.z, 2)
+
+    self.assertEqual(a.sym_contextual_getattr('x'), 0)
+    self.assertEqual(a.sym_contextual_getattr('y'), 1)
+    self.assertEqual(a.sym_contextual_getattr('z'), 2)
+
+    # Custom start.
+    with self.assertRaisesRegex(
+        AttributeError, '`x` is not found under its context'
+    ):
+      a.sym_contextual_getattr('x', start=a.sym_parent)
+
+    with self.assertRaisesRegex(
+        AttributeError, '`y` is not found under its context'
+    ):
+      a.sym_contextual_getattr('y', start=a.sym_parent)
+
+    self.assertEqual(a.sym_contextual_getattr('z', start=a.sym_parent), 2)
+
+    # Custom getter.
+    getter = Contextual(lambda k, p: getattr(p, 'b'))
+    self.assertEqual(
+        a.sym_contextual_getattr('x', getter=getter, start=a.sym_parent), 3
+    )
+    self.assertEqual(
+        a.sym_contextual_getattr('y', getter=getter, start=a.sym_parent), 3
+    )
+    self.assertEqual(
+        a.sym_contextual_getattr('z', getter=getter, start=a.sym_parent), 3
+    )
+
   def test_sym_field(self):
 
     @pg_members([
         ('x', pg_typing.Any())
     ])
     class A(Object):
       pass
@@ -1780,14 +1847,61 @@
         'Variable positional argument .* should be declared with '
         '`pg.typing.List.*`'):
 
       @pg_members([], init_arg_list=['*y'])
       class E(B):  # pylint: disable=unused-variable
         pass
 
+  def test_contextual(self):
+    class A(Object):
+      x: int
+      y: str = Contextual()
+
+    # Okay: `A.y` is contextual.
+    a = A(1)
+
+    # Not okay: `A.y` is not yet available in its context.
+    with self.assertRaisesRegex(
+        AttributeError, '`y` is not found under its context'
+    ):
+      _ = a.y
+
+    sd = Dict(x=a, y=Dict(z=1))
+    self.assertIs(a.y, sd.y)
+
+    # Clear context by reset a's parent.
+    a.sym_setparent(None)
+    with self.assertRaisesRegex(
+        AttributeError, '`y` is not found under its context'
+    ):
+      _ = a.y
+
+    # Test parent contextual value with custom getter.
+    sd = Dict(
+        a='bar',
+        b=Dict(
+            x=a,
+            y=Contextual(lambda k, p: getattr(p, 'a'))))
+
+    # a.y is redirected to sd.a.
+    self.assertEqual(a.y, 'bar')
+
+    class B(Object):
+      x: int = Contextual(lambda k, p: p.sym_getattr(k))
+
+    b = B()
+    sd = Dict(
+        a='bar',
+        b=Dict(
+            b=b,
+            x=Contextual(lambda k, p: getattr(p, 'a'))))
+
+    # a.y is redirected to sd.a.
+    self.assertEqual(b.x, 'bar')
+
 
 class RebindTest(unittest.TestCase):
   """Dedicated tests for `pg.Dict.rebind`."""
 
   def test_rebind_with_kwargs(self):
 
     @pg_members([
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230522/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230522/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230522/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230522/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230522/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_signature.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/callable_signature_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1099,18 +1099,23 @@
         # or partial.
         if object_utils.MISSING_VALUE == value:
           value = copy.deepcopy(field.default_value)
 
         child_path = object_utils.KeyPath(key, root_path)
         new_value = field.apply(
             value, allow_partial, child_transform, child_path)
-        # NOTE(daiyip): minimize call to __setitem__ when possible.
-        # Custom like symbolic dict may trigger additional logic
-        # when __setitem__ is called.
-        if key not in dict_obj or dict_obj[key] is not new_value:
+
+        # NOTE(daiyip): `pg.Dict.__getitem__`` has special logics in handling
+        # `pg.Contextual`` values. Therefore, we user `dict.__getitem__()`` to
+        # avoid triggering side effect.
+        if (key not in dict_obj
+            or dict.__getitem__(dict_obj, key) is not new_value):
+          # NOTE(daiyip): minimize call to __setitem__ when possible.
+          # Custom like symbolic dict may trigger additional logic
+          # when __setitem__ is called.
           dict_obj[key] = new_value
     return dict_obj
 
   def validate(self,
                dict_obj: Dict[str, Any],
                allow_partial: bool = False,
                root_path: Optional[object_utils.KeyPath] = None) -> None:
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/class_schema_utils_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/class_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/value_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230522/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230522/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230521/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230522/pyglove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230521
+Version: 0.3.1.dev20230522
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230521/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230522/pyglove.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 pyglove/core/symbolic/base_test.py
 pyglove/core/symbolic/boilerplate.py
 pyglove/core/symbolic/boilerplate_test.py
 pyglove/core/symbolic/class_wrapper.py
 pyglove/core/symbolic/class_wrapper_test.py
 pyglove/core/symbolic/compounding.py
 pyglove/core/symbolic/compounding_test.py
+pyglove/core/symbolic/contextual.py
+pyglove/core/symbolic/contextual_test.py
 pyglove/core/symbolic/dict.py
 pyglove/core/symbolic/dict_test.py
 pyglove/core/symbolic/diff.py
 pyglove/core/symbolic/diff_test.py
 pyglove/core/symbolic/flags.py
 pyglove/core/symbolic/flags_test.py
 pyglove/core/symbolic/functor.py
```

### Comparing `pyglove-0.3.1.dev20230521/setup.py` & `pyglove-0.3.1.dev20230522/setup.py`

 * *Files identical despite different names*

