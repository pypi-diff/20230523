# Comparing `tmp/curated-tokenizers-0.0.6.tar.gz` & `tmp/curated-tokenizers-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-tokenizers-0.0.6.tar", last modified: Tue May 23 08:17:09 2023, max compression
+gzip compressed data, was "curated-tokenizers-0.0.7.tar", last modified: Tue May 23 09:43:43 2023, max compression
```

## Comparing `curated-tokenizers-0.0.6.tar` & `curated-tokenizers-0.0.7.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.683875 curated-tokenizers-0.0.6/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2642 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1880 2023-05-23 08:17:09.683875 curated-tokenizers-0.0.6/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      939 2023-05-23 08:15:40.000000 curated-tokenizers-0.0.6/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.668875 curated-tokenizers-0.0.6/curated_tokenizers/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      120 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      333 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/_bbpe.pxd
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5835 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/_bbpe.pyx
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2149 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/_spp.pxd
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7162 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/_spp.pyx
--rw-r--r--   0 daniel    (1000) daniel    (1000)      654 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/_wordpiece.pxd
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4395 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/_wordpiece.pyx
--rw-r--r--   0 daniel    (1000) daniel    (1000)      156 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/config.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2126 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/merges.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1190 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/merges.hh
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.669875 curated-tokenizers-0.0.6/curated_tokenizers/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/tests/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       19 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/tests/incorrect-merges.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6291 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/tests/robbert-merges-1000.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)    16815 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/tests/robbert-vocab-1000.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1865 2023-05-23 08:13:55.000000 curated-tokenizers-0.0.6/curated_tokenizers/tests/test_bbpe_processor.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4297 2023-05-23 08:13:55.000000 curated-tokenizers-0.0.6/curated_tokenizers/tests/test_sp.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2009 2023-05-23 08:13:55.000000 curated-tokenizers-0.0.6/curated_tokenizers/tests/test_word_piece_processor.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       31 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/tests/toy-word-pieces.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)   253270 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/tests/toy.model
--rw-r--r--   0 daniel    (1000) daniel    (1000)      333 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/util.hh
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1083 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/wordpiece.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1011 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/curated_tokenizers/wordpiece.hh
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.668875 curated-tokenizers-0.0.6/curated_tokenizers.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1880 2023-05-23 08:17:09.000000 curated-tokenizers-0.0.6/curated_tokenizers.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10412 2023-05-23 08:17:09.000000 curated-tokenizers-0.0.6/curated_tokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-23 08:17:09.000000 curated-tokenizers-0.0.6/curated_tokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       12 2023-05-23 08:17:09.000000 curated-tokenizers-0.0.6/curated_tokenizers.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       19 2023-05-23 08:17:09.000000 curated-tokenizers-0.0.6/curated_tokenizers.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-23 08:17:09.000000 curated-tokenizers-0.0.6/curated_tokenizers.egg-info/zip-safe
--rw-r--r--   0 daniel    (1000) daniel    (1000)      107 2023-05-23 08:10:50.000000 curated-tokenizers-0.0.6/pyproject.toml
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.666875 curated-tokenizers-0.0.6/sentencepiece/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.669875 curated-tokenizers-0.0.6/sentencepiece/python/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5858 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/python/once.h
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.676875 curated-tokenizers-0.0.6/sentencepiece/src/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6648 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/bpe_model.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1748 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/bpe_model.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     9294 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/bpe_model_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10322 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/bpe_model_trainer.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4416 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/bpe_model_trainer.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4850 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/bpe_model_trainer_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    18401 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/builder.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5102 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/builder.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7354 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/builder_test.cc
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.677875 curated-tokenizers-0.0.6/sentencepiece/src/builtin_pb/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    35154 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    40648 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/builtin_pb/sentencepiece.pb.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)   130839 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)   189303 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1304 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/char_model.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1061 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/char_model.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3525 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/char_model_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1782 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/char_model_trainer.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1265 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/char_model_trainer.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2506 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/char_model_trainer_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6007 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/common.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5713 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/compile_charsmap_main.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4167 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/error.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3563 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/filesystem.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1852 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/filesystem.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1577 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/filesystem_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2345 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/freelist.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1221 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/freelist_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1341 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/init.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5359 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/init_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1644 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/model_factory.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)      972 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/model_factory.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1743 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/model_factory_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6609 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/model_interface.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     9527 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/model_interface.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    15932 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/model_interface_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)  7198605 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/normalization_rule.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11633 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/normalizer.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5835 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/normalizer.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    16156 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/normalizer_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2024 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/pretokenizer_for_training.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2126 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/pretokenizer_for_training.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2654 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/pretokenizer_for_training_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    30990 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_processor.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    19673 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_processor.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    47605 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_processor_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     9966 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_trainer.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6527 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_trainer.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    13402 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_trainer_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10493 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/spec_parser.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3986 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/spm_decode_main.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6557 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/spm_encode_main.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2035 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/spm_export_vocab_main.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4163 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/spm_normalize_main.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12142 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/spm_train_main.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1026 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/test_main.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1899 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/testharness.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8718 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/testharness.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2103 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/trainer_factory.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1104 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/trainer_factory.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1656 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/trainer_factory_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    25917 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/trainer_interface.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5727 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/trainer_interface.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    19808 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/trainer_interface_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1239 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unicode_script.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2807 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unicode_script.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)   106446 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unicode_script_map.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1525 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unicode_script_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    31219 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unigram_model.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6912 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unigram_model.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    32258 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unigram_model_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    18625 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unigram_model_trainer.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3879 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unigram_model_trainer.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3321 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/unigram_model_trainer_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7746 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/util.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11414 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/util.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12866 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/util_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1124 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/word_model.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1045 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/word_model.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2639 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/word_model_test.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2101 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/word_model_trainer.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1372 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/word_model_trainer.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2464 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/src/word_model_trainer_test.cc
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.667875 curated-tokenizers-0.0.6/sentencepiece/third_party/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.666875 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.677875 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/container/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1001 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/container/flat_hash_map.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)      966 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/container/flat_hash_set.h
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.677875 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/flags/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5614 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/flags/flag.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1673 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/flags/flag.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)      799 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/flags/parse.h
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.677875 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/memory/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2592 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/memory/memory.h
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.678875 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1309 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/ascii.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1308 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/match.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1012 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/numbers.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1447 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_cat.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1088 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_format.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2413 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_join.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2127 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_replace.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2669 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_split.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7856 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/string_view.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20934 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/string_view.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)      991 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/strip.h
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.678875 curated-tokenizers-0.0.6/sentencepiece/third_party/darts_clone/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    51750 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/darts_clone/darts.h
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.680875 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    15726 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/arena.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8985 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/arenastring.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5975 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/bytestream.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    30847 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/coded_stream.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10999 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/common.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    82338 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/extension_set.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3573 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4441 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    30000 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.667875 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.682875 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6215 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    29756 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    18092 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    15918 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    96637 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    78585 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12437 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3993 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3266 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12532 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    31313 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10023 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3542 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7024 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.682875 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    69376 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5384 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10258 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12750 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    16950 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    48107 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    24921 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7104 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    31973 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    27172 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8270 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    32754 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2050 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20834 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4209 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
--rw-r--r--   0 daniel    (1000) daniel    (1000)   101600 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-23 08:17:09.683875 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11769 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    17098 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5733 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7283 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3911 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11971 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8915 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4903 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    31213 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6157 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2184 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5108 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    12765 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3949 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8558 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3293 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    17861 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3615 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    39629 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3356 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    14401 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)    83648 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2756 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6587 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/int128.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    13526 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/io_win32.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20751 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/message_lite.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    20703 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/parse_context.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5500 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/repeated_field.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4197 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/status.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2096 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/statusor.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     9193 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/stringpiece.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     6283 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/stringprintf.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    26415 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    88575 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/strutil.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10168 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/time.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    27892 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2392 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    11345 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)    13255 2023-05-23 08:11:04.000000 curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1196 2023-05-23 08:17:09.684875 curated-tokenizers-0.0.6/setup.cfg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     6023 2023-05-23 08:14:16.000000 curated-tokenizers-0.0.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.642227 curated-tokenizers-0.0.7/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2642 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)     1880 2023-05-23 09:43:43.642227 curated-tokenizers-0.0.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      939 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.610226 curated-tokenizers-0.0.7/curated_tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/_bbpe.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     5835 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/_bbpe.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     2149 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/_spp.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     7162 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/_spp.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      654 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/_wordpiece.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     4395 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/_wordpiece.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/config.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/merges.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1190 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/merges.hh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.610226 curated-tokenizers-0.0.7/curated_tokenizers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/tests/incorrect-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     6291 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/tests/robbert-merges-1000.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    16815 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/tests/robbert-vocab-1000.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     1865 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/tests/test_bbpe_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4297 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/tests/test_sp.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2009 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/tests/test_word_piece_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/tests/toy-word-pieces.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/tests/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/util.hh
+-rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/wordpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1011 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/curated_tokenizers/wordpiece.hh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.610226 curated-tokenizers-0.0.7/curated_tokenizers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1880 2023-05-23 09:43:43.000000 curated-tokenizers-0.0.7/curated_tokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    10412 2023-05-23 09:43:43.000000 curated-tokenizers-0.0.7/curated_tokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 09:43:43.000000 curated-tokenizers-0.0.7/curated_tokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-05-23 09:43:43.000000 curated-tokenizers-0.0.7/curated_tokenizers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-05-23 09:43:43.000000 curated-tokenizers-0.0.7/curated_tokenizers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-23 09:43:43.000000 curated-tokenizers-0.0.7/curated_tokenizers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.606226 curated-tokenizers-0.0.7/sentencepiece/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.610226 curated-tokenizers-0.0.7/sentencepiece/python/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5858 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/python/once.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.630226 curated-tokenizers-0.0.7/sentencepiece/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6648 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/bpe_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/bpe_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     9294 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/bpe_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10322 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/bpe_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4416 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/bpe_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/bpe_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    18401 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/builder.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5102 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/builder.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/builder_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.630226 curated-tokenizers-0.0.7/sentencepiece/src/builtin_pb/
+-rw-r--r--   0 vsts      (1001) docker     (122)    35154 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    40648 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/builtin_pb/sentencepiece.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   130839 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)   189303 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/char_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1061 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/char_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/char_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1782 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/char_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1265 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/char_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/char_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6007 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5713 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/compile_charsmap_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4167 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/error.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3563 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/filesystem.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1852 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/filesystem.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1577 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/filesystem_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2345 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/freelist.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1221 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/freelist_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1341 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/init.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5359 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/init_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/model_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/model_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1743 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/model_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6609 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/model_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9527 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/model_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15932 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/model_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)  7198605 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/normalization_rule.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    11633 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/normalizer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5835 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/normalizer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16156 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/normalizer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2024 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/pretokenizer_for_training.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/pretokenizer_for_training.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2654 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/pretokenizer_for_training_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30990 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_processor.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    19673 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_processor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    47605 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_processor_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9966 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6527 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    13402 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10493 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/spec_parser.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3986 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/spm_decode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6557 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/spm_encode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2035 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/spm_export_vocab_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4163 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/spm_normalize_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    12142 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/spm_train_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1026 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/test_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1899 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/testharness.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8718 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/testharness.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2103 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/trainer_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1104 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/trainer_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1656 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/trainer_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    25917 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/trainer_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/trainer_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    19808 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/trainer_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unicode_script.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unicode_script.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   106446 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unicode_script_map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1525 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unicode_script_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    31219 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unigram_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6912 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unigram_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    32258 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unigram_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    18625 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unigram_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3879 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unigram_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3321 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/unigram_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     7746 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/util.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    11414 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12866 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/util_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1124 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/word_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1045 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/word_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/word_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2101 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/word_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1372 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/word_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2464 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/src/word_model_trainer_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.606226 curated-tokenizers-0.0.7/sentencepiece/third_party/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.606226 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.630226 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/container/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1001 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/container/flat_hash_map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      966 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/container/flat_hash_set.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.630226 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/flags/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5614 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/flags/flag.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1673 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/flags/flag.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/flags/parse.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.630226 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/memory/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/memory/memory.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.630226 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/ascii.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/match.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1012 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/numbers.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1447 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_cat.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_format.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2413 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_join.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2127 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_replace.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2669 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_split.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7856 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/string_view.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20934 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/string_view.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      991 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/strip.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.630226 curated-tokenizers-0.0.7/sentencepiece/third_party/darts_clone/
+-rw-r--r--   0 vsts      (1001) docker     (122)    51750 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/darts_clone/darts.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.634226 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15726 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/arena.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8985 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/arenastring.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5975 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/bytestream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30847 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/coded_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10999 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/common.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    82338 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/extension_set.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3573 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4441 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30000 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.606226 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.638227 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6215 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    29756 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    18092 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15918 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    96637 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    78585 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12437 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3993 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3266 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12532 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31313 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    10023 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3542 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7024 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.638227 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
+-rw-r--r--   0 vsts      (1001) docker     (122)    69376 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5384 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    10258 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12750 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16950 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    48107 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    24921 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7104 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31973 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    27172 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8270 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    32754 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    20834 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4209 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
+-rw-r--r--   0 vsts      (1001) docker     (122)   101600 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-23 09:43:43.642227 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11769 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17098 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5733 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7283 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3911 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    11971 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8915 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4903 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31213 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6157 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2184 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5108 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12765 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3949 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8558 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3293 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17861 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3615 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    39629 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3356 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    14401 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    83648 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2756 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6587 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/int128.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13526 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/io_win32.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20751 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/message_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20703 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/parse_context.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5500 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/repeated_field.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4197 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/status.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2096 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/statusor.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9193 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/stringpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6283 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/stringprintf.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    26415 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    88575 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/strutil.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10168 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/time.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    27892 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2392 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    11345 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13255 2023-05-23 09:43:27.000000 curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1196 2023-05-23 09:43:43.642227 curated-tokenizers-0.0.7/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     6023 2023-05-23 09:43:24.000000 curated-tokenizers-0.0.7/setup.py
```

### Comparing `curated-tokenizers-0.0.6/LICENSE` & `curated-tokenizers-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/PKG-INFO` & `curated-tokenizers-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: curated-tokenizers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Lightweight piece tokenization library
-Home-page: https://github.com/explosion/curated_tokenizers
+Home-page: https://github.com/explosion/curated-tokenizers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `curated-tokenizers-0.0.6/README.md` & `curated-tokenizers-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/_bbpe.pyx` & `curated-tokenizers-0.0.7/curated_tokenizers/_bbpe.pyx`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/_spp.pxd` & `curated-tokenizers-0.0.7/curated_tokenizers/_spp.pxd`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/_spp.pyx` & `curated-tokenizers-0.0.7/curated_tokenizers/_spp.pyx`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/_wordpiece.pxd` & `curated-tokenizers-0.0.7/curated_tokenizers/_wordpiece.pxd`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/_wordpiece.pyx` & `curated-tokenizers-0.0.7/curated_tokenizers/_wordpiece.pyx`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/merges.cc` & `curated-tokenizers-0.0.7/curated_tokenizers/merges.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/merges.hh` & `curated-tokenizers-0.0.7/curated_tokenizers/merges.hh`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/tests/robbert-merges-1000.txt` & `curated-tokenizers-0.0.7/curated_tokenizers/tests/robbert-merges-1000.txt`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/tests/robbert-vocab-1000.json` & `curated-tokenizers-0.0.7/curated_tokenizers/tests/robbert-vocab-1000.json`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/tests/test_bbpe_processor.py` & `curated-tokenizers-0.0.7/curated_tokenizers/tests/test_bbpe_processor.py`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/tests/test_sp.py` & `curated-tokenizers-0.0.7/curated_tokenizers/tests/test_sp.py`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/tests/test_word_piece_processor.py` & `curated-tokenizers-0.0.7/curated_tokenizers/tests/test_word_piece_processor.py`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/tests/toy.model` & `curated-tokenizers-0.0.7/curated_tokenizers/tests/toy.model`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/wordpiece.cc` & `curated-tokenizers-0.0.7/curated_tokenizers/wordpiece.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers/wordpiece.hh` & `curated-tokenizers-0.0.7/curated_tokenizers/wordpiece.hh`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers.egg-info/PKG-INFO` & `curated-tokenizers-0.0.7/curated_tokenizers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: curated-tokenizers
-Version: 0.0.6
+Version: 0.0.7
 Summary: Lightweight piece tokenization library
-Home-page: https://github.com/explosion/curated_tokenizers
+Home-page: https://github.com/explosion/curated-tokenizers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `curated-tokenizers-0.0.6/curated_tokenizers.egg-info/SOURCES.txt` & `curated-tokenizers-0.0.7/curated_tokenizers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/python/once.h` & `curated-tokenizers-0.0.7/sentencepiece/python/once.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/bpe_model.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/bpe_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/bpe_model.h` & `curated-tokenizers-0.0.7/sentencepiece/src/bpe_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/bpe_model_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/bpe_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/bpe_model_trainer.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/bpe_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/bpe_model_trainer.h` & `curated-tokenizers-0.0.7/sentencepiece/src/bpe_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/bpe_model_trainer_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/bpe_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/builder.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/builder.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/builder.h` & `curated-tokenizers-0.0.7/sentencepiece/src/builder.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/builder_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/builder_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/builtin_pb/sentencepiece.pb.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/builtin_pb/sentencepiece.pb.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/builtin_pb/sentencepiece.pb.h` & `curated-tokenizers-0.0.7/sentencepiece/src/builtin_pb/sentencepiece.pb.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h` & `curated-tokenizers-0.0.7/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/char_model.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/char_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/char_model.h` & `curated-tokenizers-0.0.7/sentencepiece/src/char_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/char_model_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/char_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/char_model_trainer.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/char_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/char_model_trainer.h` & `curated-tokenizers-0.0.7/sentencepiece/src/char_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/char_model_trainer_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/char_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/common.h` & `curated-tokenizers-0.0.7/sentencepiece/src/common.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/compile_charsmap_main.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/compile_charsmap_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/error.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/error.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/filesystem.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/filesystem.h` & `curated-tokenizers-0.0.7/sentencepiece/src/filesystem.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/filesystem_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/filesystem_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/freelist.h` & `curated-tokenizers-0.0.7/sentencepiece/src/freelist.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/freelist_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/freelist_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/init.h` & `curated-tokenizers-0.0.7/sentencepiece/src/init.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/init_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/init_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/model_factory.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/model_factory.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/model_factory.h` & `curated-tokenizers-0.0.7/sentencepiece/src/model_factory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/model_factory_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/model_factory_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/model_interface.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/model_interface.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/model_interface.h` & `curated-tokenizers-0.0.7/sentencepiece/src/model_interface.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/model_interface_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/model_interface_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/normalization_rule.h` & `curated-tokenizers-0.0.7/sentencepiece/src/normalization_rule.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/normalizer.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/normalizer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/normalizer.h` & `curated-tokenizers-0.0.7/sentencepiece/src/normalizer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/normalizer_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/normalizer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/pretokenizer_for_training.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/pretokenizer_for_training.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/pretokenizer_for_training.h` & `curated-tokenizers-0.0.7/sentencepiece/src/pretokenizer_for_training.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/pretokenizer_for_training_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/pretokenizer_for_training_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_processor.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_processor.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_processor.h` & `curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_processor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_processor_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_processor_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_trainer.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_trainer.h` & `curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/sentencepiece_trainer_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/sentencepiece_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/spec_parser.h` & `curated-tokenizers-0.0.7/sentencepiece/src/spec_parser.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/spm_decode_main.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/spm_decode_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/spm_encode_main.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/spm_encode_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/spm_export_vocab_main.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/spm_export_vocab_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/spm_normalize_main.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/spm_normalize_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/spm_train_main.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/spm_train_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/test_main.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/test_main.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/testharness.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/testharness.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/testharness.h` & `curated-tokenizers-0.0.7/sentencepiece/src/testharness.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/trainer_factory.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/trainer_factory.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/trainer_factory.h` & `curated-tokenizers-0.0.7/sentencepiece/src/trainer_factory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/trainer_factory_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/trainer_factory_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/trainer_interface.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/trainer_interface.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/trainer_interface.h` & `curated-tokenizers-0.0.7/sentencepiece/src/trainer_interface.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/trainer_interface_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/trainer_interface_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unicode_script.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/unicode_script.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unicode_script.h` & `curated-tokenizers-0.0.7/sentencepiece/src/unicode_script.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unicode_script_map.h` & `curated-tokenizers-0.0.7/sentencepiece/src/unicode_script_map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unicode_script_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/unicode_script_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unigram_model.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/unigram_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unigram_model.h` & `curated-tokenizers-0.0.7/sentencepiece/src/unigram_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unigram_model_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/unigram_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unigram_model_trainer.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/unigram_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unigram_model_trainer.h` & `curated-tokenizers-0.0.7/sentencepiece/src/unigram_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/unigram_model_trainer_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/unigram_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/util.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/util.h` & `curated-tokenizers-0.0.7/sentencepiece/src/util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/util_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/util_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/word_model.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/word_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/word_model.h` & `curated-tokenizers-0.0.7/sentencepiece/src/word_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/word_model_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/word_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/word_model_trainer.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/word_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/word_model_trainer.h` & `curated-tokenizers-0.0.7/sentencepiece/src/word_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/src/word_model_trainer_test.cc` & `curated-tokenizers-0.0.7/sentencepiece/src/word_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/container/flat_hash_map.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/container/flat_hash_map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/container/flat_hash_set.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/container/flat_hash_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/flags/flag.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/flags/flag.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/flags/flag.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/flags/flag.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/flags/parse.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/flags/parse.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/memory/memory.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/memory/memory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/ascii.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/ascii.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/match.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/match.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/numbers.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/numbers.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_cat.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_cat.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_format.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_format.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_join.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_join.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_replace.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_replace.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/str_split.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/str_split.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/string_view.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/string_view.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/string_view.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/string_view.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/absl/strings/strip.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/absl/strings/strip.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/darts_clone/darts.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/darts_clone/darts.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/arena.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/arena.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/arenastring.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/arenastring.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/bytestream.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/bytestream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/coded_stream.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/coded_stream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/common.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/common.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/extension_set.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/extension_set.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/generated_message_util.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/generated_message_util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/int128.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/int128.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/io_win32.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/io_win32.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/message_lite.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/message_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/parse_context.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/parse_context.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/repeated_field.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/repeated_field.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/status.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/status.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/statusor.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/statusor.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/stringpiece.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/stringprintf.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/stringprintf.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/structurally_valid.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/structurally_valid.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/strutil.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/strutil.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/time.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/time.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc` & `curated-tokenizers-0.0.7/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.6/setup.cfg` & `curated-tokenizers-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 description = Lightweight piece tokenization library
-version = 0.0.6
-url = https://github.com/explosion/curated_tokenizers
+version = 0.0.7
+url = https://github.com/explosion/curated-tokenizers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `curated-tokenizers-0.0.6/setup.py` & `curated-tokenizers-0.0.7/setup.py`

 * *Files identical despite different names*

