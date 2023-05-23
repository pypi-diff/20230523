# Comparing `tmp/deepchem-2.7.2.dev20230523160930.tar.gz` & `tmp/deepchem-2.7.2.dev20230523163554.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230523160930.tar", last modified: Tue May 23 16:09:30 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230523163554.tar", last modified: Tue May 23 16:35:55 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230523160930.tar` & `deepchem-2.7.2.dev20230523163554.tar`

### file list

```diff
@@ -1,294 +1,294 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.648714 deepchem-2.7.2.dev20230523160930/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 16:09:30.648714 deepchem-2.7.2.dev20230523160930/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.600713 deepchem-2.7.2.dev20230523160930/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.600713 deepchem-2.7.2.dev20230523160930/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67894 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.600713 deepchem-2.7.2.dev20230523160930/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.604713 deepchem-2.7.2.dev20230523160930/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.604713 deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.604713 deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.608713 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.608713 deepchem-2.7.2.dev20230523160930/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.608713 deepchem-2.7.2.dev20230523160930/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.608713 deepchem-2.7.2.dev20230523160930/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.608713 deepchem-2.7.2.dev20230523160930/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.612713 deepchem-2.7.2.dev20230523160930/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.612713 deepchem-2.7.2.dev20230523160930/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.612713 deepchem-2.7.2.dev20230523160930/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/dft/dftxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.612713 deepchem-2.7.2.dev20230523160930/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.616713 deepchem-2.7.2.dev20230523160930/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.616713 deepchem-2.7.2.dev20230523160930/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    55220 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.616713 deepchem-2.7.2.dev20230523160930/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.620713 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   110013 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.620713 deepchem-2.7.2.dev20230523160930/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.632713 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.632713 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.636714 deepchem-2.7.2.dev20230523160930/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.636714 deepchem-2.7.2.dev20230523160930/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.636714 deepchem-2.7.2.dev20230523160930/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.640714 deepchem-2.7.2.dev20230523160930/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.644714 deepchem-2.7.2.dev20230523160930/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.644714 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-23 16:09:13.000000 deepchem-2.7.2.dev20230523160930/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:09:30.600713 deepchem-2.7.2.dev20230523160930/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 16:09:30.000000 deepchem-2.7.2.dev20230523160930/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10589 2023-05-23 16:09:30.000000 deepchem-2.7.2.dev20230523160930/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:09:30.000000 deepchem-2.7.2.dev20230523160930/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-23 16:09:30.000000 deepchem-2.7.2.dev20230523160930/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 16:09:30.000000 deepchem-2.7.2.dev20230523160930/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-23 16:09:30.648714 deepchem-2.7.2.dev20230523160930/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-23 16:09:14.000000 deepchem-2.7.2.dev20230523160930/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.224949 deepchem-2.7.2.dev20230523163554/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 16:35:55.224949 deepchem-2.7.2.dev20230523163554/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.192949 deepchem-2.7.2.dev20230523163554/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.196949 deepchem-2.7.2.dev20230523163554/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67894 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.196949 deepchem-2.7.2.dev20230523163554/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.196949 deepchem-2.7.2.dev20230523163554/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.200949 deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21863 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.200949 deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.200949 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.200949 deepchem-2.7.2.dev20230523163554/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.200949 deepchem-2.7.2.dev20230523163554/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.204949 deepchem-2.7.2.dev20230523163554/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.204949 deepchem-2.7.2.dev20230523163554/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.204949 deepchem-2.7.2.dev20230523163554/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.208949 deepchem-2.7.2.dev20230523163554/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.208949 deepchem-2.7.2.dev20230523163554/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/dft/dftxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.208949 deepchem-2.7.2.dev20230523163554/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.208949 deepchem-2.7.2.dev20230523163554/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.208949 deepchem-2.7.2.dev20230523163554/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55220 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.208949 deepchem-2.7.2.dev20230523163554/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.212949 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115619 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.212949 deepchem-2.7.2.dev20230523163554/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.216949 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.216949 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.220949 deepchem-2.7.2.dev20230523163554/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.220949 deepchem-2.7.2.dev20230523163554/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.220949 deepchem-2.7.2.dev20230523163554/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.220949 deepchem-2.7.2.dev20230523163554/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.224949 deepchem-2.7.2.dev20230523163554/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.224949 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 16:35:55.196949 deepchem-2.7.2.dev20230523163554/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-23 16:35:55.000000 deepchem-2.7.2.dev20230523163554/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10589 2023-05-23 16:35:55.000000 deepchem-2.7.2.dev20230523163554/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 16:35:55.000000 deepchem-2.7.2.dev20230523163554/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-23 16:35:55.000000 deepchem-2.7.2.dev20230523163554/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 16:35:55.000000 deepchem-2.7.2.dev20230523163554/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-23 16:35:55.224949 deepchem-2.7.2.dev20230523163554/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-23 16:35:42.000000 deepchem-2.7.2.dev20230523163554/setup.py
```

### Comparing `deepchem-2.7.2.dev20230523160930/LICENSE` & `deepchem-2.7.2.dev20230523163554/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/PKG-INFO` & `deepchem-2.7.2.dev20230523163554/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230523160930
+Version: 2.7.2.dev20230523163554
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230523160930/README.md` & `deepchem-2.7.2.dev20230523163554/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230523163554/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230523163554/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230523163554/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230523163554/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230523163554/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230523163554/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230523163554/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230523163554/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230523163554/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230523163554/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230523163554/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230523163554/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230523163554/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230523163554/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230523163554/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/dft/dftxc.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/models.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from deepchem.models.torch_models.infograph import InfoGraphStar, InfoGraphStarModel, InfoGraphEncoder, GINEncoder, InfoGraph, InfoGraphModel, InfoGraphEncoder
 from deepchem.models.torch_models.mpnn import MPNN, MPNNModel
 from deepchem.models.torch_models.lcnn import LCNN, LCNNModel
 from deepchem.models.torch_models.pagtn import Pagtn, PagtnModel
 from deepchem.models.torch_models.mat import MAT, MATModel
 from deepchem.models.torch_models.megnet import MEGNetModel
 from deepchem.models.torch_models.normalizing_flows_pytorch import NormalizingFlow
-from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList
+from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather
 from deepchem.models.torch_models.cnn import CNN
 from deepchem.models.torch_models.attention import ScaledDotProductAttention, SelfAttention
 from deepchem.models.torch_models.grover import GroverModel, GroverPretrain, GroverFinetune
 from deepchem.models.torch_models.readout import GroverReadout
 try:
     from deepchem.models.torch_models.dmpnn import DMPNN, DMPNNModel
     from deepchem.models.torch_models.gnn import GNN, GNNHead, GNNModular
```

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/chemberta.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/hf_models.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6869,8 +6869,359 @@
 0001ad40: 2020 2020 2020 2020 2020 6f75 745f 7465            out_te
 0001ad50: 6e73 6f72 203d 2077 202a 2069 6e5f 7465  nsor = w * in_te
 0001ad60: 6e73 6f72 0a20 2020 2020 2020 2020 2020  nsor.           
 0001ad70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
 0001ad80: 2020 2020 2020 206f 7574 5f74 656e 736f         out_tenso
 0001ad90: 7220 2b3d 2077 202a 2069 6e5f 7465 6e73  r += w * in_tens
 0001ada0: 6f72 0a20 2020 2020 2020 2072 6574 7572  or.        retur
-0001adb0: 6e20 6f75 745f 7465 6e73 6f72 0a         n out_tensor.
+0001adb0: 6e20 6f75 745f 7465 6e73 6f72 0a0a 0a63  n out_tensor...c
+0001adc0: 6c61 7373 2053 6574 4761 7468 6572 286e  lass SetGather(n
+0001add0: 6e2e 4d6f 6475 6c65 293a 0a20 2020 2022  n.Module):.    "
+0001ade0: 2222 7365 7432 7365 7420 6761 7468 6572  ""set2set gather
+0001adf0: 206c 6179 6572 2066 6f72 2067 7261 7068   layer for graph
+0001ae00: 2d62 6173 6564 206d 6f64 656c 0a0a 2020  -based model..  
+0001ae10: 2020 4d6f 6465 6c73 2075 7369 6e67 2074    Models using t
+0001ae20: 6869 7320 6c61 7965 7220 6d75 7374 2073  his layer must s
+0001ae30: 6574 2060 7061 645f 6261 7463 6865 733d  et `pad_batches=
+0001ae40: 5472 7565 600a 0a20 2020 2054 6f72 6368  True`..    Torch
+0001ae50: 2045 7175 6976 616c 656e 7420 6f66 204b   Equivalent of K
+0001ae60: 6572 6173 2053 6574 4761 7468 6572 206c  eras SetGather l
+0001ae70: 6179 6572 0a0a 2020 2020 5061 7261 6d65  ayer..    Parame
+0001ae80: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+0001ae90: 2d2d 2d0a 2020 2020 4d3a 2069 6e74 0a20  ---.    M: int. 
+0001aea0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+0001aeb0: 204c 5354 4d20 7374 6570 730a 2020 2020   LSTM steps.    
+0001aec0: 6261 7463 685f 7369 7a65 3a20 696e 740a  batch_size: int.
+0001aed0: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+0001aee0: 6620 7361 6d70 6c65 7320 696e 2061 2062  f samples in a b
+0001aef0: 6174 6368 2861 6c6c 2062 6174 6368 6573  atch(all batches
+0001af00: 206d 7573 7420 6861 7665 2073 616d 6520   must have same 
+0001af10: 7369 7a65 290a 2020 2020 6e5f 6869 6464  size).    n_hidd
+0001af20: 656e 3a20 696e 742c 206f 7074 696f 6e61  en: int, optiona
+0001af30: 6c0a 2020 2020 2020 2020 6e75 6d62 6572  l.        number
+0001af40: 206f 6620 6869 6464 656e 2075 6e69 7473   of hidden units
+0001af50: 2069 6e20 7468 6520 7061 7373 696e 6720   in the passing 
+0001af60: 7068 6173 650a 0a20 2020 2045 7861 6d70  phase..    Examp
+0001af70: 6c65 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  les.    --------
+0001af80: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
+0001af90: 6465 6570 6368 656d 2061 7320 6463 0a20  deepchem as dc. 
+0001afa0: 2020 203e 3e3e 2069 6d70 6f72 7420 6e75     >>> import nu
+0001afb0: 6d70 7920 6173 206e 700a 2020 2020 3e3e  mpy as np.    >>
+0001afc0: 3e20 6672 6f6d 2064 6565 7063 6865 6d2e  > from deepchem.
+0001afd0: 6d6f 6465 6c73 2e74 6f72 6368 5f6d 6f64  models.torch_mod
+0001afe0: 656c 7320 696d 706f 7274 206c 6179 6572  els import layer
+0001aff0: 730a 2020 2020 3e3e 3e20 746f 7461 6c5f  s.    >>> total_
+0001b000: 6e5f 6174 6f6d 7320 3d20 340a 2020 2020  n_atoms = 4.    
+0001b010: 3e3e 3e20 6e5f 6174 6f6d 5f66 6561 7420  >>> n_atom_feat 
+0001b020: 3d20 340a 2020 2020 3e3e 3e20 6174 6f6d  = 4.    >>> atom
+0001b030: 5f66 6561 7420 3d20 6e70 2e72 616e 646f  _feat = np.rando
+0001b040: 6d2e 7261 6e64 2874 6f74 616c 5f6e 5f61  m.rand(total_n_a
+0001b050: 746f 6d73 2c20 6e5f 6174 6f6d 5f66 6561  toms, n_atom_fea
+0001b060: 7429 0a20 2020 203e 3e3e 2061 746f 6d5f  t).    >>> atom_
+0001b070: 7370 6c69 7420 3d20 6e70 2e61 7272 6179  split = np.array
+0001b080: 285b 302c 2030 2c20 312c 2031 5d2c 2064  ([0, 0, 1, 1], d
+0001b090: 7479 7065 3d6e 702e 696e 7433 3229 0a20  type=np.int32). 
+0001b0a0: 2020 203e 3e3e 2067 6174 6865 7220 3d20     >>> gather = 
+0001b0b0: 6c61 7965 7273 2e53 6574 4761 7468 6572  layers.SetGather
+0001b0c0: 2832 2c20 322c 206e 5f68 6964 6465 6e3d  (2, 2, n_hidden=
+0001b0d0: 3429 0a20 2020 203e 3e3e 206f 7574 7075  4).    >>> outpu
+0001b0e0: 745f 6d6f 6c65 6375 6c65 7320 3d20 6761  t_molecules = ga
+0001b0f0: 7468 6572 285b 6174 6f6d 5f66 6561 742c  ther([atom_feat,
+0001b100: 2061 746f 6d5f 7370 6c69 745d 290a 2020   atom_split]).  
+0001b110: 2020 3e3e 3e20 7072 696e 7428 6f75 7470    >>> print(outp
+0001b120: 7574 5f6d 6f6c 6563 756c 6573 2e73 6861  ut_molecules.sha
+0001b130: 7065 290a 2020 2020 746f 7263 682e 5369  pe).    torch.Si
+0001b140: 7a65 285b 322c 2038 5d29 0a0a 2020 2020  ze([2, 8])..    
+0001b150: 2222 220a 0a20 2020 2064 6566 205f 5f69  """..    def __i
+0001b160: 6e69 745f 5f28 7365 6c66 2c0a 2020 2020  nit__(self,.    
+0001b170: 2020 2020 2020 2020 2020 2020 204d 3a20               M: 
+0001b180: 696e 742c 0a20 2020 2020 2020 2020 2020  int,.           
+0001b190: 2020 2020 2020 6261 7463 685f 7369 7a65        batch_size
+0001b1a0: 3a20 696e 742c 0a20 2020 2020 2020 2020  : int,.         
+0001b1b0: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
+0001b1c0: 3a20 696e 7420 3d20 3130 302c 0a20 2020  : int = 100,.   
+0001b1d0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0001b1e0: 6974 3d27 6f72 7468 6f67 6f6e 616c 272c  it='orthogonal',
+0001b1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b200: 2020 2a2a 6b77 6172 6773 293a 0a0a 2020    **kwargs):..  
+0001b210: 2020 2020 2020 7375 7065 7228 5365 7447        super(SetG
+0001b220: 6174 6865 722c 2073 656c 6629 2e5f 5f69  ather, self).__i
+0001b230: 6e69 745f 5f28 2a2a 6b77 6172 6773 290a  nit__(**kwargs).
+0001b240: 2020 2020 2020 2020 7365 6c66 2e4d 203d          self.M =
+0001b250: 204d 0a20 2020 2020 2020 2073 656c 662e   M.        self.
+0001b260: 6261 7463 685f 7369 7a65 203d 2062 6174  batch_size = bat
+0001b270: 6368 5f73 697a 650a 2020 2020 2020 2020  ch_size.        
+0001b280: 7365 6c66 2e6e 5f68 6964 6465 6e20 3d20  self.n_hidden = 
+0001b290: 6e5f 6869 6464 656e 0a20 2020 2020 2020  n_hidden.       
+0001b2a0: 2073 656c 662e 696e 6974 203d 2069 6e69   self.init = ini
+0001b2b0: 740a 0a20 2020 2020 2020 2073 656c 662e  t..        self.
+0001b2c0: 5520 3d20 6e6e 2e50 6172 616d 6574 6572  U = nn.Parameter
+0001b2d0: 280a 2020 2020 2020 2020 2020 2020 746f  (.            to
+0001b2e0: 7263 682e 5465 6e73 6f72 2832 202a 2073  rch.Tensor(2 * s
+0001b2f0: 656c 662e 6e5f 6869 6464 656e 2c20 3420  elf.n_hidden, 4 
+0001b300: 2a20 7365 6c66 2e6e 5f68 6964 6465 6e29  * self.n_hidden)
+0001b310: 2e6e 6f72 6d61 6c5f 286d 6561 6e3d 302e  .normal_(mean=0.
+0001b320: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+0001b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b360: 2020 2020 2020 2020 2020 7374 643d 302e            std=0.
+0001b370: 3129 290a 2020 2020 2020 2020 7365 6c66  1)).        self
+0001b380: 2e62 203d 206e 6e2e 5061 7261 6d65 7465  .b = nn.Paramete
+0001b390: 7228 0a20 2020 2020 2020 2020 2020 2074  r(.            t
+0001b3a0: 6f72 6368 2e63 6174 2828 746f 7263 682e  orch.cat((torch.
+0001b3b0: 7a65 726f 7328 7365 6c66 2e6e 5f68 6964  zeros(self.n_hid
+0001b3c0: 6465 6e29 2c20 746f 7263 682e 6f6e 6573  den), torch.ones
+0001b3d0: 2873 656c 662e 6e5f 6869 6464 656e 292c  (self.n_hidden),
+0001b3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b3f0: 2020 2020 2020 2020 746f 7263 682e 7a65          torch.ze
+0001b400: 726f 7328 7365 6c66 2e6e 5f68 6964 6465  ros(self.n_hidde
+0001b410: 6e29 2c20 746f 7263 682e 7a65 726f 7328  n), torch.zeros(
+0001b420: 7365 6c66 2e6e 5f68 6964 6465 6e29 2929  self.n_hidden)))
+0001b430: 290a 2020 2020 2020 2020 7365 6c66 2e62  ).        self.b
+0001b440: 7569 6c74 203d 2054 7275 650a 0a20 2020  uilt = True..   
+0001b450: 2064 6566 205f 5f72 6570 725f 5f28 7365   def __repr__(se
+0001b460: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+0001b470: 2020 2020 7265 7475 726e 2028 0a20 2020      return (.   
+0001b480: 2020 2020 2020 2020 2066 277b 7365 6c66           f'{self
+0001b490: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+0001b4a0: 655f 5f7d 284d 3d7b 7365 6c66 2e4d 7d2c  e__}(M={self.M},
+0001b4b0: 2062 6174 6368 5f73 697a 653d 7b73 656c   batch_size={sel
+0001b4c0: 662e 6261 7463 685f 7369 7a65 7d2c 206e  f.batch_size}, n
+0001b4d0: 5f68 6964 6465 6e3d 7b73 656c 662e 6e5f  _hidden={self.n_
+0001b4e0: 6869 6464 656e 7d2c 2069 6e69 743d 7b73  hidden}, init={s
+0001b4f0: 656c 662e 696e 6974 7d29 270a 2020 2020  elf.init})'.    
+0001b500: 2020 2020 290a 0a20 2020 2064 6566 2066      )..    def f
+0001b510: 6f72 7761 7264 2873 656c 662c 2069 6e70  orward(self, inp
+0001b520: 7574 733a 204c 6973 7429 202d 3e20 746f  uts: List) -> to
+0001b530: 7263 682e 5465 6e73 6f72 3a0a 2020 2020  rch.Tensor:.    
+0001b540: 2020 2020 2222 2250 6572 666f 726d 204d      """Perform M
+0001b550: 2073 7465 7073 206f 6620 7365 7432 7365   steps of set2se
+0001b560: 7420 6761 7468 6572 2c0a 0a20 2020 2020  t gather,..     
+0001b570: 2020 2044 6574 6169 6c65 6420 6465 7363     Detailed desc
+0001b580: 7269 7074 696f 6e73 2069 6e3a 2068 7474  riptions in: htt
+0001b590: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+0001b5a0: 6273 2f31 3531 312e 3036 3339 310a 0a20  bs/1511.06391.. 
+0001b5b0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+0001b5c0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0001b5d0: 2d2d 2d2d 0a20 2020 2020 2020 2069 6e70  ----.        inp
+0001b5e0: 7574 733a 204c 6973 740a 2020 2020 2020  uts: List.      
+0001b5f0: 2020 2020 2020 5468 6973 2063 6f6e 7461        This conta
+0001b600: 696e 7320 7477 6f20 656c 656d 656e 7473  ins two elements
+0001b610: 2e0a 2020 2020 2020 2020 2020 2020 6174  ..            at
+0001b620: 6f6d 5f66 6561 7475 7265 733a 206e 702e  om_features: np.
+0001b630: 6e64 6172 7261 790a 2020 2020 2020 2020  ndarray.        
+0001b640: 2020 2020 6174 6f6d 5f73 706c 6974 3a20      atom_split: 
+0001b650: 6e70 2e6e 6461 7272 6179 0a0a 2020 2020  np.ndarray..    
+0001b660: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+0001b670: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0001b680: 2020 2020 715f 7374 6172 3a20 746f 7263      q_star: torc
+0001b690: 682e 5465 6e73 6f72 0a20 2020 2020 2020  h.Tensor.       
+0001b6a0: 2020 2020 2046 696e 616c 2073 7461 7465       Final state
+0001b6b0: 206f 6620 7468 6520 6d6f 6465 6c20 6166   of the model af
+0001b6c0: 7465 7220 616c 6c20 4d20 7374 6570 732e  ter all M steps.
+0001b6d0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0001b6e0: 2020 2020 2020 6174 6f6d 5f66 6561 7475        atom_featu
+0001b6f0: 7265 732c 2061 746f 6d5f 7370 6c69 7420  res, atom_split 
+0001b700: 3d20 696e 7075 7473 0a20 2020 2020 2020  = inputs.       
+0001b710: 2063 203d 2074 6f72 6368 2e7a 6572 6f73   c = torch.zeros
+0001b720: 2828 7365 6c66 2e62 6174 6368 5f73 697a  ((self.batch_siz
+0001b730: 652c 2073 656c 662e 6e5f 6869 6464 656e  e, self.n_hidden
+0001b740: 2929 0a20 2020 2020 2020 2068 203d 2074  )).        h = t
+0001b750: 6f72 6368 2e7a 6572 6f73 2828 7365 6c66  orch.zeros((self
+0001b760: 2e62 6174 6368 5f73 697a 652c 2073 656c  .batch_size, sel
+0001b770: 662e 6e5f 6869 6464 656e 2929 0a0a 2020  f.n_hidden))..  
+0001b780: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0001b790: 616e 6765 2873 656c 662e 4d29 3a0a 2020  ange(self.M):.  
+0001b7a0: 2020 2020 2020 2020 2020 715f 6578 7061            q_expa
+0001b7b0: 6e64 6564 203d 2068 5b61 746f 6d5f 7370  nded = h[atom_sp
+0001b7c0: 6c69 745d 0a20 2020 2020 2020 2020 2020  lit].           
+0001b7d0: 2065 203d 2028 746f 7263 682e 6672 6f6d   e = (torch.from
+0001b7e0: 5f6e 756d 7079 2861 746f 6d5f 6665 6174  _numpy(atom_feat
+0001b7f0: 7572 6573 2920 2a20 715f 6578 7061 6e64  ures) * q_expand
+0001b800: 6564 292e 7375 6d28 6469 6d3d 2d31 290a  ed).sum(dim=-1).
+0001b810: 2020 2020 2020 2020 2020 2020 655f 6d6f              e_mo
+0001b820: 6c73 203d 2073 656c 662e 5f64 796e 616d  ls = self._dynam
+0001b830: 6963 5f70 6172 7469 7469 6f6e 2865 2c20  ic_partition(e, 
+0001b840: 6174 6f6d 5f73 706c 6974 2c20 7365 6c66  atom_split, self
+0001b850: 2e62 6174 6368 5f73 697a 6529 0a0a 2020  .batch_size)..  
+0001b860: 2020 2020 2020 2020 2020 2320 4164 6420            # Add 
+0001b870: 616e 6f74 6865 7220 7661 6c75 6528 7e2d  another value(~-
+0001b880: 496e 6629 2074 6f20 7072 6576 656e 7420  Inf) to prevent 
+0001b890: 6572 726f 7220 696e 2073 6f66 746d 6178  error in softmax
+0001b8a0: 0a20 2020 2020 2020 2020 2020 2065 5f6d  .            e_m
+0001b8b0: 6f6c 7320 3d20 5b0a 2020 2020 2020 2020  ols = [.        
+0001b8c0: 2020 2020 2020 2020 746f 7263 682e 6361          torch.ca
+0001b8d0: 7428 5b65 5f6d 6f6c 2c20 746f 7263 682e  t([e_mol, torch.
+0001b8e0: 7465 6e73 6f72 285b 2d31 3030 302e 5d29  tensor([-1000.])
+0001b8f0: 5d2c 2064 696d 3d30 290a 2020 2020 2020  ], dim=0).      
+0001b900: 2020 2020 2020 2020 2020 666f 7220 655f            for e_
+0001b910: 6d6f 6c20 696e 2065 5f6d 6f6c 730a 2020  mol in e_mols.  
+0001b920: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+0001b930: 2020 2020 2020 2020 6120 3d20 746f 7263          a = torc
+0001b940: 682e 6361 7428 5b0a 2020 2020 2020 2020  h.cat([.        
+0001b950: 2020 2020 2020 2020 746f 7263 682e 6e6e          torch.nn
+0001b960: 2e66 756e 6374 696f 6e61 6c2e 736f 6674  .functional.soft
+0001b970: 6d61 7828 655f 6d6f 6c5b 3a2d 315d 2c20  max(e_mol[:-1], 
+0001b980: 6469 6d3d 3029 0a20 2020 2020 2020 2020  dim=0).         
+0001b990: 2020 2020 2020 2066 6f72 2065 5f6d 6f6c         for e_mol
+0001b9a0: 2069 6e20 655f 6d6f 6c73 0a20 2020 2020   in e_mols.     
+0001b9b0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+0001b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9d0: 2020 2020 6469 6d3d 3029 0a0a 2020 2020      dim=0)..    
+0001b9e0: 2020 2020 2020 2020 7220 3d20 7363 6174          r = scat
+0001b9f0: 7465 7228 746f 7263 682e 7265 7368 6170  ter(torch.reshap
+0001ba00: 6528 612c 205b 2d31 2c20 315d 2920 2a20  e(a, [-1, 1]) * 
+0001ba10: 6174 6f6d 5f66 6561 7475 7265 732c 0a20  atom_features,. 
+0001ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba30: 2020 2020 2020 2074 6f72 6368 2e66 726f         torch.fro
+0001ba40: 6d5f 6e75 6d70 7928 6174 6f6d 5f73 706c  m_numpy(atom_spl
+0001ba50: 6974 292e 6c6f 6e67 2829 2c0a 2020 2020  it).long(),.    
+0001ba60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ba70: 2020 2020 6469 6d3d 3029 0a20 2020 2020      dim=0).     
+0001ba80: 2020 2020 2020 2023 204d 6f64 656c 2075         # Model u
+0001ba90: 7369 6e67 2074 6869 7320 6c61 7965 7220  sing this layer 
+0001baa0: 6d75 7374 2073 6574 2060 7061 645f 6261  must set `pad_ba
+0001bab0: 7463 6865 733d 5472 7565 600a 2020 2020  tches=True`.    
+0001bac0: 2020 2020 2020 2020 715f 7374 6172 203d          q_star =
+0001bad0: 2074 6f72 6368 2e63 6174 285b 682c 2072   torch.cat([h, r
+0001bae0: 5d2c 2064 696d 3d31 290a 2020 2020 2020  ], dim=1).      
+0001baf0: 2020 2020 2020 682c 2063 203d 2073 656c        h, c = sel
+0001bb00: 662e 5f4c 5354 4d53 7465 7028 715f 7374  f._LSTMStep(q_st
+0001bb10: 6172 2c20 6329 0a20 2020 2020 2020 2072  ar, c).        r
+0001bb20: 6574 7572 6e20 715f 7374 6172 0a0a 2020  eturn q_star..  
+0001bb30: 2020 6465 6620 5f4c 5354 4d53 7465 7028    def _LSTMStep(
+0001bb40: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+0001bb50: 2020 2020 2020 2020 683a 2074 6f72 6368          h: torch
+0001bb60: 2e54 656e 736f 722c 0a20 2020 2020 2020  .Tensor,.       
+0001bb70: 2020 2020 2020 2020 2020 2063 3a20 746f             c: to
+0001bb80: 7263 682e 5465 6e73 6f72 2c0a 2020 2020  rch.Tensor,.    
+0001bb90: 2020 2020 2020 2020 2020 2020 2020 783d                x=
+0001bba0: 4e6f 6e65 2920 2d3e 2054 7570 6c65 5b74  None) -> Tuple[t
+0001bbb0: 6f72 6368 2e54 656e 736f 722c 2074 6f72  orch.Tensor, tor
+0001bbc0: 6368 2e54 656e 736f 725d 3a0a 2020 2020  ch.Tensor]:.    
+0001bbd0: 2020 2020 2222 2254 6869 7320 6d65 7468      """This meth
+0001bbe0: 6f72 6420 7065 7266 6f72 6d73 2061 2073  ord performs a s
+0001bbf0: 696e 676c 6520 7374 6570 206f 6620 6120  ingle step of a 
+0001bc00: 4c6f 6e67 2053 686f 7274 2d54 6572 6d20  Long Short-Term 
+0001bc10: 4d65 6d6f 7279 2028 4c53 544d 2920 6365  Memory (LSTM) ce
+0001bc20: 6c6c 2c0a 0a20 2020 2020 2020 2050 6172  ll,..        Par
+0001bc30: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0001bc40: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0001bc50: 2020 2068 3a20 746f 7263 682e 5465 6e73     h: torch.Tens
+0001bc60: 6f72 0a20 2020 2020 2020 2020 2020 2054  or.            T
+0001bc70: 6865 2068 6964 6465 6e20 7374 6174 6520  he hidden state 
+0001bc80: 6f66 2074 6865 204c 5354 4d20 6365 6c6c  of the LSTM cell
+0001bc90: 2e0a 2020 2020 2020 2020 633a 2074 6f72  ..        c: tor
+0001bca0: 6368 2e54 656e 736f 720a 2020 2020 2020  ch.Tensor.      
+0001bcb0: 2020 2020 2020 5468 6520 6365 6c6c 2073        The cell s
+0001bcc0: 7461 7465 206f 6620 7468 6520 4c53 544d  tate of the LSTM
+0001bcd0: 2063 656c 6c2e 0a0a 2020 2020 2020 2020   cell...        
+0001bce0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0001bcf0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0001bd00: 685f 6f75 743a 2074 6f72 6368 2e54 656e  h_out: torch.Ten
+0001bd10: 736f 720a 2020 2020 2020 2020 2020 2020  sor.            
+0001bd20: 5468 6520 7570 6461 7465 6420 6869 6464  The updated hidd
+0001bd30: 656e 2073 7461 7465 206f 6620 7468 6520  en state of the 
+0001bd40: 4c53 544d 2063 656c 6c2e 0a20 2020 2020  LSTM cell..     
+0001bd50: 2020 2063 5f6f 7574 3a20 746f 7263 682e     c_out: torch.
+0001bd60: 5465 6e73 6f72 0a20 2020 2020 2020 2020  Tensor.         
+0001bd70: 2020 2054 6865 2075 7064 6174 6564 2063     The updated c
+0001bd80: 656c 6c20 7374 6174 6520 6f66 2074 6865  ell state of the
+0001bd90: 204c 5354 4d20 6365 6c6c 2e0a 0a20 2020   LSTM cell...   
+0001bda0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001bdb0: 2023 207a 203d 2074 6f72 6368 2e6d 6d28   # z = torch.mm(
+0001bdc0: 682c 2073 656c 662e 5529 202b 2073 656c  h, self.U) + sel
+0001bdd0: 662e 620a 2020 2020 2020 2020 7a20 3d20  f.b.        z = 
+0001bde0: 462e 6c69 6e65 6172 2868 2e66 6c6f 6174  F.linear(h.float
+0001bdf0: 2829 2e64 6574 6163 6828 292c 0a20 2020  ().detach(),.   
+0001be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be10: 2020 7365 6c66 2e55 2e66 6c6f 6174 2829    self.U.float()
+0001be20: 2e54 2e64 6574 6163 6828 292c 2073 656c  .T.detach(), sel
+0001be30: 662e 622e 6465 7461 6368 2829 290a 2020  f.b.detach()).  
+0001be40: 2020 2020 2020 6920 3d20 746f 7263 682e        i = torch.
+0001be50: 7369 676d 6f69 6428 7a5b 3a2c 203a 7365  sigmoid(z[:, :se
+0001be60: 6c66 2e6e 5f68 6964 6465 6e5d 290a 2020  lf.n_hidden]).  
+0001be70: 2020 2020 2020 6620 3d20 746f 7263 682e        f = torch.
+0001be80: 7369 676d 6f69 6428 7a5b 3a2c 2073 656c  sigmoid(z[:, sel
+0001be90: 662e 6e5f 6869 6464 656e 3a32 202a 2073  f.n_hidden:2 * s
+0001bea0: 656c 662e 6e5f 6869 6464 656e 5d29 0a20  elf.n_hidden]). 
+0001beb0: 2020 2020 2020 206f 203d 2074 6f72 6368         o = torch
+0001bec0: 2e73 6967 6d6f 6964 287a 5b3a 2c20 3220  .sigmoid(z[:, 2 
+0001bed0: 2a20 7365 6c66 2e6e 5f68 6964 6465 6e3a  * self.n_hidden:
+0001bee0: 3320 2a20 7365 6c66 2e6e 5f68 6964 6465  3 * self.n_hidde
+0001bef0: 6e5d 290a 2020 2020 2020 2020 7a33 203d  n]).        z3 =
+0001bf00: 207a 5b3a 2c20 3320 2a20 7365 6c66 2e6e   z[:, 3 * self.n
+0001bf10: 5f68 6964 6465 6e3a 5d0a 2020 2020 2020  _hidden:].      
+0001bf20: 2020 635f 6f75 7420 3d20 6620 2a20 6320    c_out = f * c 
+0001bf30: 2b20 6920 2a20 746f 7263 682e 7461 6e68  + i * torch.tanh
+0001bf40: 287a 3329 0a20 2020 2020 2020 2068 5f6f  (z3).        h_o
+0001bf50: 7574 203d 206f 202a 2074 6f72 6368 2e74  ut = o * torch.t
+0001bf60: 616e 6828 635f 6f75 7429 0a20 2020 2020  anh(c_out).     
+0001bf70: 2020 2072 6574 7572 6e20 685f 6f75 742c     return h_out,
+0001bf80: 2063 5f6f 7574 0a0a 2020 2020 6465 6620   c_out..    def 
+0001bf90: 5f64 796e 616d 6963 5f70 6172 7469 7469  _dynamic_partiti
+0001bfa0: 6f6e 2873 656c 662c 2069 6e70 7574 5f74  on(self, input_t
+0001bfb0: 656e 736f 723a 2074 6f72 6368 2e54 656e  ensor: torch.Ten
+0001bfc0: 736f 722c 0a20 2020 2020 2020 2020 2020  sor,.           
+0001bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bfe0: 7061 7274 6974 696f 6e5f 7465 6e73 6f72  partition_tensor
+0001bff0: 3a20 6e70 2e6e 6461 7272 6179 2c0a 2020  : np.ndarray,.  
+0001c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c010: 2020 2020 2020 2020 206e 756d 5f70 6172           num_par
+0001c020: 7469 7469 6f6e 733a 2069 6e74 2920 2d3e  titions: int) ->
+0001c030: 204c 6973 745b 746f 7263 682e 5465 6e73   List[torch.Tens
+0001c040: 6f72 5d3a 0a20 2020 2020 2020 2022 2222  or]:.        """
+0001c050: 5061 7274 6974 696f 6e73 2060 6461 7461  Partitions `data
+0001c060: 6020 696e 746f 2060 6e75 6d5f 7061 7274  ` into `num_part
+0001c070: 6974 696f 6e73 6020 7465 6e73 6f72 7320  itions` tensors 
+0001c080: 7573 696e 6720 696e 6469 6365 7320 6672  using indices fr
+0001c090: 6f6d 2060 7061 7274 6974 696f 6e73 602e  om `partitions`.
+0001c0a0: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+0001c0b0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+0001c0c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0001c0d0: 696e 7075 745f 7465 6e73 6f72 3a20 746f  input_tensor: to
+0001c0e0: 7263 682e 5465 6e73 6f72 0a20 2020 2020  rch.Tensor.     
+0001c0f0: 2020 2020 2020 2054 6865 2074 656e 736f         The tenso
+0001c100: 7220 746f 2062 6520 7061 7274 6974 696f  r to be partitio
+0001c110: 6e65 642e 0a20 2020 2020 2020 2070 6172  ned..        par
+0001c120: 7469 7469 6f6e 5f74 656e 736f 723a 206e  tition_tensor: n
+0001c130: 702e 6e64 6172 7261 790a 2020 2020 2020  p.ndarray.      
+0001c140: 2020 2020 2020 4120 312d 4420 7465 6e73        A 1-D tens
+0001c150: 6f72 2077 686f 7365 2073 697a 6520 6973  or whose size is
+0001c160: 2065 7175 616c 2074 6f20 7468 6520 6669   equal to the fi
+0001c170: 7273 7420 6469 6d65 6e73 696f 6e20 6f66  rst dimension of
+0001c180: 2060 696e 7075 745f 7465 6e73 6f72 602e   `input_tensor`.
+0001c190: 0a20 2020 2020 2020 206e 756d 5f70 6172  .        num_par
+0001c1a0: 7469 7469 6f6e 733a 2069 6e74 0a20 2020  titions: int.   
+0001c1b0: 2020 2020 2020 2020 2054 6865 206e 756d           The num
+0001c1c0: 6265 7220 6f66 2070 6172 7469 7469 6f6e  ber of partition
+0001c1d0: 7320 746f 206f 7574 7075 742e 0a0a 2020  s to output...  
+0001c1e0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+0001c1f0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+0001c200: 2020 2020 2020 7061 7274 6974 696f 6e73        partitions
+0001c210: 3a20 4c69 7374 5b74 6f72 6368 2e54 656e  : List[torch.Ten
+0001c220: 736f 725d 0a20 2020 2020 2020 2020 2020  sor].           
+0001c230: 2041 206c 6973 7420 6f66 2060 6e75 6d5f   A list of `num_
+0001c240: 7061 7274 6974 696f 6e73 6020 6054 656e  partitions` `Ten
+0001c250: 736f 7260 206f 626a 6563 7473 2077 6974  sor` objects wit
+0001c260: 6820 7468 6520 7361 6d65 2074 7970 6520  h the same type 
+0001c270: 6173 2060 6461 7461 602e 0a0a 2020 2020  as `data`...    
+0001c280: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0001c290: 2320 6372 6561 7465 2061 2062 6f6f 6c65  # create a boole
+0001c2a0: 616e 206d 6173 6b20 666f 7220 6561 6368  an mask for each
+0001c2b0: 2070 6172 7469 7469 6f6e 0a20 2020 2020   partition.     
+0001c2c0: 2020 2070 6172 7469 7469 6f6e 5f6d 6173     partition_mas
+0001c2d0: 6b73 203d 205b 7061 7274 6974 696f 6e5f  ks = [partition_
+0001c2e0: 7465 6e73 6f72 203d 3d20 6920 666f 7220  tensor == i for 
+0001c2f0: 6920 696e 2072 616e 6765 286e 756d 5f70  i in range(num_p
+0001c300: 6172 7469 7469 6f6e 7329 5d0a 0a20 2020  artitions)]..   
+0001c310: 2020 2020 2023 2070 6172 7469 7469 6f6e       # partition
+0001c320: 2074 6865 2069 6e70 7574 2074 656e 736f   the input tenso
+0001c330: 7220 7573 696e 6720 7468 6520 6d61 736b  r using the mask
+0001c340: 730a 2020 2020 2020 2020 7061 7274 6974  s.        partit
+0001c350: 696f 6e73 203d 205b 696e 7075 745f 7465  ions = [input_te
+0001c360: 6e73 6f72 5b6d 6173 6b5d 2066 6f72 206d  nsor[mask] for m
+0001c370: 6173 6b20 696e 2070 6172 7469 7469 6f6e  ask in partition
+0001c380: 5f6d 6173 6b73 5d0a 0a20 2020 2020 2020  _masks]..       
+0001c390: 2072 6574 7572 6e20 7061 7274 6974 696f   return partitio
+0001c3a0: 6e73 0a                                  ns.
```

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230523163554/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230523163554/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230523163554/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230523163554/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230523163554/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230523163554/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230523163554/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230523163554/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230523163554/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230523163554/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/graph_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230523163554/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230523163554/deepchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230523160930
+Version: 2.7.2.dev20230523163554
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230523160930/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230523163554/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/setup.cfg` & `deepchem-2.7.2.dev20230523163554/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230523160930/setup.py` & `deepchem-2.7.2.dev20230523163554/setup.py`

 * *Files identical despite different names*

