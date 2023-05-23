# Comparing `tmp/dialogy-2.0.6.tar.gz` & `tmp/dialogy-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-2.0.6.tar", max compression
+gzip compressed data, was "dialogy-2.0.7.tar", max compression
```

## Comparing `dialogy-2.0.6.tar` & `dialogy-2.0.7.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1069 2023-05-10 14:37:20.344091 dialogy-2.0.6/LICENSE.md
--rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9777 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15679 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     5017 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     2011 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/registry.py
--rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     4001 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8874 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3796 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11811 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1185 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    16771 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7682 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    38996 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20340 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12306 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      743 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1804 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14129 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11529 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4705 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4253 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4154 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7361 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2281 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4432 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      975 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-10 14:37:20.344091 dialogy-2.0.6/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/__init__.py
--rw-r--r--   0        0        0    10469 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/config.py
--rw-r--r--   0        0        0     2180 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2687 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     6917 2023-05-10 14:37:20.348091 dialogy-2.0.6/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1471 2023-05-10 14:37:36.824187 dialogy-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     1651 1970-01-01 00:00:00.000000 dialogy-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-23 03:34:05.535176 dialogy-2.0.7/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-05-23 03:34:05.535176 dialogy-2.0.7/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-23 03:34:05.535176 dialogy-2.0.7/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-23 03:34:05.535176 dialogy-2.0.7/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9777 2023-05-23 03:34:05.535176 dialogy-2.0.7/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15685 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     5017 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     2011 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/registry.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     4001 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8880 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3802 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11811 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1185 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    16717 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7682 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    38996 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20340 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12306 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1804 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14135 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11529 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4711 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     3013 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4259 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4154 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7361 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2281 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4432 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      975 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0    10660 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/config.py
+-rw-r--r--   0        0        0     2180 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2880 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     7069 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1536 2023-05-23 03:34:25.671321 dialogy-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 dialogy-2.0.7/PKG-INFO
```

### Comparing `dialogy-2.0.6/LICENSE.md` & `dialogy-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/base/entity_extractor/__init__.py` & `dialogy-2.0.7/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/base/input/__init__.py` & `dialogy-2.0.7/dialogy/base/input/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/base/output/__init__.py` & `dialogy-2.0.7/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/base/plugin/__init__.py` & `dialogy-2.0.7/dialogy/base/plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,15 @@
 
     def train(self, _: Any) -> Any:
         """
         Train a plugin.
         """
         return None
 
-    def transform(self, training_data: Any) -> Any:
+    async def transform(self, training_data: Any) -> Any:
         """
         Transform data for a plugin in the workflow.
         """
         if not self.use_transform:
             return training_data
         return training_data
```

### Comparing `dialogy-2.0.6/dialogy/cli/__init__.py` & `dialogy-2.0.7/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/cli/project.py` & `dialogy-2.0.7/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/cli/workflow.py` & `dialogy-2.0.7/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/constants/__init__.py` & `dialogy-2.0.7/dialogy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/registry.py` & `dialogy-2.0.7/dialogy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/address_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-2.0.7/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/address_parser/maps.py` & `dialogy-2.0.7/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/calibration/xgb.py` & `dialogy-2.0.7/dialogy/plugins/text/calibration/xgb.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             prediction = self.predict(utterance)
             for alternative, wer in zip(utterance, prediction):
                 if wer < self.threshold:
                     filtered_alternatives.append(alternative)
             filtered_utterances.append(filtered_alternatives)
         return filtered_utterances
 
-    def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
+    async def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         # filters df alternatives and feeds into merge_asr_output,
         # doesn't change training_data schema
         training_data["use"] = True
         logger.debug("Transforming training data.")
         for i, row in training_data.iterrows():
             asr_output = None
             try:
```

### Comparing `dialogy-2.0.6/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         return canonicalized_transcripts
 
     async def utility(self, input: Input, output: Output) -> Any:
         entities = output.entities
         transcripts = input.transcripts
         return self.mask_transcript(entities, transcripts)
 
-    def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
+    async def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         if not self.use_transform:
             return training_data
 
         logger.debug(f"Transforming dataset via {self.__class__.__name__}")
 
         for i, row in tqdm(training_data.iterrows(), total=len(training_data)):
             try:
```

### Comparing `dialogy-2.0.6/dialogy/plugins/text/classification/mlp.py` & `dialogy-2.0.7/dialogy/plugins/text/classification/mlp.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-2.0.7/dialogy/plugins/text/classification/retain_intent.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/classification/xlmr.py` & `dialogy-2.0.7/dialogy/plugins/text/classification/xlmr.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,20 +119,18 @@
             self.labelencoder_file_path = os.path.join(
                 self.model_dir, const.LABELENCODER_FILE
             )
 
             self.kwargs = kwargs or {}
 
             # TODO: check if this can be avoided
-            if "name" in self.kwargs:
-                del self.kwargs["name"]
-            if "imported" in self.kwargs:
-                del self.kwargs["imported"]
-            if "purpose" in self.kwargs:
-                del self.kwargs["purpose"]
+            avoiding_keys = ["name", "imported", "purpose", "project_name"]
+            for key in avoiding_keys:
+                if key in self.kwargs:
+                    del self.kwargs[key]
 
             try:
                 if os.path.exists(self.labelencoder_file_path):
                     logger.debug(f"initializing label encoder file from {self.labelencoder_file_path}")
                     self.init_model()
             except EOFError:
                 logger.error(
```

### Comparing `dialogy-2.0.6/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-2.0.7/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
                         )
                         entity_tokens.append(
                             (matches.group(), entity_type, entity_value, matches.span())
                         )
         logger.debug(entity_tokens)
         return entity_tokens
 
-    def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
+    async def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         """
         Transform training data.
 
         :param training_data: Training data.
         :type training_data: pd.DataFrame
         :return: Transformed training data.
         :rtype: pd.DataFrame
```

### Comparing `dialogy-2.0.6/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-2.0.7/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             debug=debug,
             **kwargs
         )
 
     async def utility(self, input: Input, _: Output) -> Any:
         return merge_asr_output(input.utterances)
 
-    def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
+    async def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         if not self.use_transform:
             return training_data
 
         training_data["use"] = True
         logger.debug(f"Transforming dataset via {self.__class__.__name__}")
         for i, row in tqdm(training_data.iterrows(), total=len(training_data)):
             asr_output = None
```

### Comparing `dialogy-2.0.6/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         training_data["use"] = training_data["conflicting_intents"].isna()
 
         return training_data
 
     async def utility(self, input: Input, _: Output) -> Any:
         return
 
-    def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
+    async def transform(self, training_data: pd.DataFrame) -> pd.DataFrame:
         if not self.use_transform:
             return training_data
 
         training_data["use"] = True
         logger.debug(f"Transforming dataset via {self.__class__.__name__}")
 
         if self.drop_conflicting_labels:
```

### Comparing `dialogy-2.0.6/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-2.0.7/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-2.0.7/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/__init__.py` & `dialogy-2.0.7/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/address/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/base_entity/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/base_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/deserialize/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/duration/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/keyword/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/numerical/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/people/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/pincode/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/time/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/entity/time_interval/__init__.py` & `dialogy-2.0.7/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/intent/__init__.py` & `dialogy-2.0.7/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/types/slots/__init__.py` & `dialogy-2.0.7/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/utils/__init__.py` & `dialogy-2.0.7/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/utils/config.py` & `dialogy-2.0.7/dialogy/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         return os.path.join(
             self.project_artifacts_root_path,
             self._get_data_dir(task_name),
             const.METRICS,
         )
 
     def get_dataset_dir(self, task_name: str) -> str:
-        return os.path.join(self._get_data_dir(task_name), const.DATASETS)
+        return os.path.join(self.project_artifacts_root_path, self._get_data_dir(task_name), const.DATASETS)
 
     def get_skip_list(self, task_name: str) -> Set[str]:
         if task_name == const.CLASSIFICATION:
             return set(self.model_config.tasks.classification.skip)
         raise NotImplementedError(f"Model for {task_name} is not defined!")
 
     def get_dataset(self, task_name: str, file_name: str) -> Any:
@@ -232,15 +232,15 @@
     return config
 
 
 def get_project_artifacts_path_by_name(project_name: str, project_artifacts_root: str) -> str:
     return os.path.join(project_artifacts_root, project_name, "configs")
 
 
-def fetch_project_config(project: str, all_project_artifacts_root: str) -> Config:
+def fetch_project_config(project: str, all_project_artifacts_root: str) -> Optional[Config]:
     project_config_path = get_project_artifacts_path_by_name(
         project, all_project_artifacts_root
     )
     pipeline_config, core_plugins_config, model_config, misc_config = None, None, {}, {}
     for file in glob.glob(os.path.join(project_config_path, "*.yaml")):
         with open(file, "r", encoding="utf8") as handle:
             yaml_contents = yaml.safe_load(handle)
@@ -248,14 +248,16 @@
             pipeline_config = yaml_contents
         elif const.CORE_PLUGINS_CONFIG_FILE in file:
             core_plugins_config = yaml_contents
         elif const.MODEL_CONFIG_FILE in file:
             model_config = yaml_contents
         else:
             misc_config.update(yaml_contents)
+    if pipeline_config is None or core_plugins_config is None or not model_config:
+        return None
     # TODO: raise exception for both kind of configs not found
     config = Config(
         **{ # type: ignore
             "project_artifacts_root_path": os.path.join(
                 all_project_artifacts_root, project
             ),
             "pipeline_config": pipeline_config,
@@ -278,10 +280,12 @@
         # hidden files from editors / OS like .idea
         if project.startswith("."):
             continue
         if filter_list and project not in filter_list:
             continue
         print(project)
         config = fetch_project_config(project, project_artifacts_root)
+        if not config:
+            continue
         all_project_configs.update({project: config})
 
     return all_project_configs
```

### Comparing `dialogy-2.0.6/dialogy/utils/datetime.py` & `dialogy-2.0.7/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/utils/file_handler.py` & `dialogy-2.0.7/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/utils/logger.py` & `dialogy-2.0.7/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/utils/misc.py` & `dialogy-2.0.7/dialogy/utils/misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Import functions:
     - dict_traversal
     - validate_type
 """
 from functools import reduce
 from typing import Any, Dict, List, Tuple, Union
+from asyncio import Task
 
 
 def traverse_dict(obj: Dict[Any, Any], properties: List[str]) -> Any:
     """
     Traverse a dictionary for a given list of properties.
 
     This is useful for traversing a deeply nested dictionary.
@@ -74,7 +75,13 @@
         :type obj_type: (Union[type, Tuple[type]])
         :return:
         :rtype:
         :raises TypeError: If the type `obj_type` doesn't match the type of `obj`.
     """
     if not isinstance(obj, obj_type):
         raise TypeError(f"{obj} should be a {obj_type}")
+
+
+def _to_task(future: Any, as_task: bool, loop: Any) -> Any:
+    if not as_task or isinstance(future, Task):
+        return future
+    return loop.create_task(future)
```

### Comparing `dialogy-2.0.6/dialogy/utils/naive_lang_detect.py` & `dialogy-2.0.7/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/utils/normalize_utterance.py` & `dialogy-2.0.7/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/utils/temperature_scaling.py` & `dialogy-2.0.7/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.6/dialogy/workflow/workflow.py` & `dialogy-2.0.7/dialogy/workflow/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,21 +118,22 @@
 from typing import List
 
 import attr
 import pandas as pd
 
 from threading import Lock
 from pprint import pformat
+import asyncio, nest_asyncio
 
 from dialogy import constants as const
 from dialogy.base.input import Input
 from dialogy.base.output import Output
 from dialogy.base.plugin import Plugin
 from dialogy.utils.logger import logger
-from dialogy.utils import normalize, get_best_transcript
+from dialogy.utils.misc import _to_task
 
 
 @attr.s
 class Workflow:
     """
     SLU API blackbox.
 
@@ -234,11 +235,14 @@
         (in case the data isn't suitable for them) and saving/loading artifacts.
 
         :param training_data: [description]
         :type training_data: pd.DataFrame
         """
         for plugin in self.plugins:
             plugin.train(training_data)
-            transformed_data = plugin.transform(training_data)
+            loop = asyncio.get_event_loop()
+            nest_asyncio.apply(loop)
+            coroutine = plugin.transform(training_data)
+            transformed_data = loop.run_until_complete(coroutine)
             if transformed_data is not None:
                 training_data = transformed_data
         return self
```

### Comparing `dialogy-2.0.6/pyproject.toml` & `dialogy-2.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "dialogy"
-version = "2.0.6"
+version = "2.0.7"
 description = "Dialogy is a library for building and managing SLU applications."
-authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>"]
+authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>", "Daksh Varshneya <dakshvar22@gmail.com"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 attrs = "21.3.0"
 requests = "^2.25.1"
@@ -30,14 +30,15 @@
 types-requests = "^2.27.11"
 types-setuptools = "^57.4.10"
 black = "^22.8.0"
 googlemaps = "^4.6.0"
 torch = "1.12.1"
 pydantic = "^1.10.2"
 aiohttp = "^3.8.4"
+nest-asyncio = "^1.5.6"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^2.10.1"
 copier = "^6.0.0"
 mypy = "^0.982"
```

### Comparing `dialogy-2.0.6/PKG-INFO` & `dialogy-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 2.0.6
+Version: 2.0.7
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Requires-Dist: attrs (==21.3.0)
 Requires-Dist: black (>=22.8.0,<23.0.0)
 Requires-Dist: copier (>=6.0.0,<7.0.0)
 Requires-Dist: googlemaps (>=4.6.0,<5.0.0)
 Requires-Dist: jiwer (>=2.2.0,<3.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
+Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: numpy (>=1.20.2,<2.0.0)
 Requires-Dist: pandas (>=1.3.2,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pydash (>=4.9.3,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pytz (>=2020.4,<2021.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
```

