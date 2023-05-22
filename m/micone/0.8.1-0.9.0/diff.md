# Comparing `tmp/micone-0.8.1.tar.gz` & `tmp/micone-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micone-0.8.1.tar", max compression
+gzip compressed data, was "micone-0.9.0.tar", max compression
```

## Comparing `micone-0.8.1.tar` & `micone-0.9.0.tar`

### file list

```diff
@@ -1,180 +1,201 @@
--rw-r--r--   0        0        0     1073 2020-12-17 21:32:29.671644 micone-0.8.1/LICENSE
--rw-r--r--   0        0        0     5116 2021-03-02 21:18:20.768048 micone-0.8.1/README.md
--rw-r--r--   0        0        0      211 2021-03-16 15:05:22.728177 micone-0.8.1/micone/__init__.py
--rw-r--r--   0        0        0     5000 2021-03-13 17:29:35.811533 micone-0.8.1/micone/cli.py
--rw-r--r--   0        0        0       98 2020-12-17 21:32:30.064978 micone-0.8.1/micone/config/__init__.py
--rw-r--r--   0        0        0     3205 2020-12-17 21:32:30.064978 micone-0.8.1/micone/config/config.py
--rw-r--r--   0        0        0     3054 2020-12-17 21:32:30.068311 micone-0.8.1/micone/config/datatypes.py
--rw-r--r--   0        0        0    12861 2021-03-02 15:49:42.944572 micone-0.8.1/micone/config/params.py
--rw-r--r--   0        0        0      128 2020-12-17 21:32:30.064978 micone-0.8.1/micone/conversion/__init__.py
--rw-r--r--   0        0        0      864 2020-12-17 21:32:30.064978 micone-0.8.1/micone/conversion/network_converter.py
--rw-r--r--   0        0        0        0 2020-12-17 21:32:30.064978 micone-0.8.1/micone/conversion/otu_converter.py
--rw-r--r--   0        0        0     2392 2021-01-25 21:42:09.462263 micone-0.8.1/micone/conversion/taxmetadata_converter.py
--rw-r--r--   0        0        0       24 2020-12-17 21:32:30.054977 micone-0.8.1/micone/logging/__init__.py
--rw-r--r--   0        0        0     2146 2021-01-01 16:11:29.961447 micone-0.8.1/micone/logging/logger.py
--rw-r--r--   0        0        0      119 2020-12-17 21:32:30.061644 micone-0.8.1/micone/main/__init__.py
--rw-r--r--   0        0        0     8789 2021-02-11 21:32:26.968329 micone-0.8.1/micone/main/lineage.py
--rw-r--r--   0        0        0    31005 2021-10-07 15:26:57.471219 micone-0.8.1/micone/main/network.py
--rw-r--r--   0        0        0    21335 2021-10-07 23:51:38.751436 micone-0.8.1/micone/main/network_group.py
--rw-r--r--   0        0        0    16629 2021-02-01 18:07:48.958428 micone-0.8.1/micone/main/otu.py
--rw-r--r--   0        0        0       24 2020-12-17 21:32:30.058311 micone-0.8.1/micone/micone.py
--rw-r--r--   0        0        0      142 2020-12-17 21:32:30.068311 micone-0.8.1/micone/pipelines/__init__.py
--rw-r--r--   0        0        0     7199 2020-12-17 21:32:30.068311 micone-0.8.1/micone/pipelines/command.py
--rw-r--r--   0        0        0     2133 2021-05-26 15:18:15.064568 micone-0.8.1/micone/pipelines/configs/denoise_cluster.config
--rw-r--r--   0        0        0     1938 2021-10-07 23:52:49.191436 micone-0.8.1/micone/pipelines/configs/network_inference.config
--rw-r--r--   0        0        0      668 2021-05-26 15:18:15.064568 micone-0.8.1/micone/pipelines/configs/otu_processing.config
--rw-r--r--   0        0        0     1516 2021-09-27 14:39:04.744584 micone-0.8.1/micone/pipelines/configs/process.config
--rw-r--r--   0        0        0      549 2021-09-28 14:34:22.297810 micone-0.8.1/micone/pipelines/configs/profiles.config
--rw-r--r--   0        0        0      726 2021-05-27 15:35:33.901107 micone-0.8.1/micone/pipelines/configs/tax_assignment.config
--rw-r--r--   0        0        0      329 2021-05-27 15:05:54.871120 micone-0.8.1/micone/pipelines/envs/micone-dada2/env.yml
--rw-r--r--   0        0        0      190 2021-02-16 23:22:23.388997 micone-0.8.1/micone/pipelines/envs/micone-flashweave/env.yml
--rw-r--r--   0        0        0      659 2021-10-09 14:31:55.347394 micone-0.8.1/micone/pipelines/envs/micone-flashweave/post_install.sh
--rw-r--r--   0        0        0      152 2021-01-29 20:22:23.384587 micone-0.8.1/micone/pipelines/envs/micone-mldm/env.yml
--rw-r--r--   0        0        0      389 2021-01-29 20:32:52.407925 micone-0.8.1/micone/pipelines/envs/micone-mldm/post_install.sh
--rw-r--r--   0        0        0      203 2021-02-10 15:55:24.037865 micone-0.8.1/micone/pipelines/envs/micone-netcomi/env.yml
--rw-r--r--   0        0        0      241 2021-02-10 16:08:51.394549 micone-0.8.1/micone/pipelines/envs/micone-netcomi/post_install.sh
--rw-r--r--   0        0        0      170 2021-02-09 21:38:14.925624 micone-0.8.1/micone/pipelines/envs/micone-propr/env.yml
--rw-r--r--   0        0        0      113 2021-02-09 21:38:37.268957 micone-0.8.1/micone/pipelines/envs/micone-propr/post_install.sh
--rw-r--r--   0        0        0      217 2021-05-27 14:56:49.747790 micone-0.8.1/micone/pipelines/envs/micone-qiime1/env.yml
--rw-r--r--   0        0        0      133 2021-01-29 14:16:04.747765 micone-0.8.1/micone/pipelines/envs/micone-qiime1/post_install.sh
--rw-r--r--   0        0        0     9474 2021-01-29 14:25:32.404435 micone-0.8.1/micone/pipelines/envs/micone-qiime2/env.yml
--rw-r--r--   0        0        0       82 2021-01-01 16:08:30.224776 micone-0.8.1/micone/pipelines/envs/micone-qiime2/post_install.sh
--rw-r--r--   0        0        0      202 2021-10-08 18:08:08.414113 micone-0.8.1/micone/pipelines/envs/micone-sparcc/env.yml
--rw-r--r--   0        0        0      175 2021-01-29 17:43:00.387854 micone-0.8.1/micone/pipelines/envs/micone-spieceasi/env.yml
--rw-r--r--   0        0        0      642 2021-10-06 18:44:26.850168 micone-0.8.1/micone/pipelines/functions/functions.nf
--rw-r--r--   0        0        0       74 2020-12-17 21:32:30.071644 micone-0.8.1/micone/pipelines/helpers.py
--rw-r--r--   0        0        0      941 2021-05-26 21:21:42.394411 micone-0.8.1/micone/pipelines/main.nf
--rw-r--r--   0        0        0      319 2021-05-16 14:43:37.786755 micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/create_seqtable.nf
--rw-r--r--   0        0        0      646 2021-09-30 12:23:08.671984 micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/export_files.nf
--rw-r--r--   0        0        0      338 2021-05-16 14:52:06.560092 micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/import_files.nf
--rw-r--r--   0        0        0      780 2021-09-29 14:38:55.131253 micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/remove_bimera.nf
--rw-r--r--   0        0        0      564 2021-05-26 15:38:56.817893 micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/remove_bimera_workflow.nf
--rw-r--r--   0        0        0      613 2021-09-29 14:39:20.534586 micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/uchime.nf
--rw-r--r--   0        0        0      529 2021-05-16 14:56:01.963427 micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/uchime_workflow.nf
--rw-r--r--   0        0        0     1898 2021-10-09 14:58:40.604019 micone-0.8.1/micone/pipelines/modules/denoise_cluster/denoise_cluster_workflow.nf
--rw-r--r--   0        0        0      972 2021-09-29 14:42:41.131254 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/closed_reference.nf
--rw-r--r--   0        0        0      548 2021-05-15 20:47:38.673579 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/closed_reference_workflow.nf
--rw-r--r--   0        0        0      667 2021-09-29 14:43:20.071254 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/dada2.nf
--rw-r--r--   0        0        0      522 2021-05-15 21:11:13.506922 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/dada2_workflow.nf
--rw-r--r--   0        0        0      798 2021-09-29 14:43:57.464588 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/de_novo.nf
--rw-r--r--   0        0        0      512 2021-05-15 20:57:53.523584 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/de_novo_workflow.nf
--rw-r--r--   0        0        0      793 2021-09-29 14:43:35.547921 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/deblur.nf
--rw-r--r--   0        0        0      432 2021-05-15 21:22:40.776928 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/deblur_workflow.nf
--rw-r--r--   0        0        0      308 2021-05-26 15:26:32.101231 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/fastq2fasta.nf
--rw-r--r--   0        0        0      653 2021-09-30 12:21:44.408650 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/hashing2.nf
--rw-r--r--   0        0        0      742 2021-09-30 12:36:56.598657 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/hashing3.nf
--rw-r--r--   0        0        0      333 2021-05-26 15:26:54.931231 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/make_biom_repseqs.nf
--rw-r--r--   0        0        0     1055 2021-09-29 14:44:32.284588 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/open_reference.nf
--rw-r--r--   0        0        0      540 2021-05-26 15:37:59.814560 micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/open_reference_workflow.nf
--rw-r--r--   0        0        0      944 2021-09-29 14:49:18.844590 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/demultiplexing_illumina.nf
--rw-r--r--   0        0        0      711 2021-05-26 15:44:43.691223 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/demultiplexing_illumina_workflow.nf
--rw-r--r--   0        0        0      703 2021-09-30 12:16:56.038648 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/export_sequences.nf
--rw-r--r--   0        0        0      474 2021-05-27 13:25:03.047829 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/export_visualization.nf
--rw-r--r--   0        0        0      340 2021-05-15 19:32:59.806882 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/import_sequences_py.nf
--rw-r--r--   0        0        0      358 2021-05-15 13:15:04.033382 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/import_sequences_sh.nf
--rw-r--r--   0        0        0      545 2021-05-25 12:57:52.374620 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/join_reads.nf
--rw-r--r--   0        0        0      660 2021-05-25 12:39:54.871278 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/quality_analysis.nf
--rw-r--r--   0        0        0      728 2021-10-09 14:58:32.770686 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/trim_filter_fixed_workflow.nf
--rw-r--r--   0        0        0      948 2021-09-30 12:18:59.648649 micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/trimming.nf
--rw-r--r--   0        0        0      431 2021-05-11 14:51:17.508373 micone-0.8.1/micone/pipelines/modules/network_inference/bootstrap/filter.nf
--rw-r--r--   0        0        0      898 2021-09-30 12:57:04.101999 micone-0.8.1/micone/pipelines/modules/network_inference/bootstrap/pvalue.nf
--rw-r--r--   0        0        0      546 2021-05-27 21:17:29.760959 micone-0.8.1/micone/pipelines/modules/network_inference/bootstrap/resample.nf
--rw-r--r--   0        0        0     1085 2021-09-30 12:57:07.391999 micone-0.8.1/micone/pipelines/modules/network_inference/correlation/pearson.nf
--rw-r--r--   0        0        0      624 2021-05-25 14:00:56.687981 micone-0.8.1/micone/pipelines/modules/network_inference/correlation/pearson_workflow.nf
--rw-r--r--   0        0        0     1073 2021-09-30 12:59:11.475333 micone-0.8.1/micone/pipelines/modules/network_inference/correlation/propr.nf
--rw-r--r--   0        0        0      614 2021-05-25 14:01:06.214647 micone-0.8.1/micone/pipelines/modules/network_inference/correlation/propr_workflow.nf
--rw-r--r--   0        0        0     1162 2021-09-30 13:00:01.455334 micone-0.8.1/micone/pipelines/modules/network_inference/correlation/sparcc.nf
--rw-r--r--   0        0        0      619 2021-05-25 14:01:15.834647 micone-0.8.1/micone/pipelines/modules/network_inference/correlation/sparcc_workflow.nf
--rw-r--r--   0        0        0     1090 2021-09-30 13:00:12.595334 micone-0.8.1/micone/pipelines/modules/network_inference/correlation/spearman.nf
--rw-r--r--   0        0        0      629 2021-05-25 14:01:25.091314 micone-0.8.1/micone/pipelines/modules/network_inference/correlation/spearman_workflow.nf
--rw-r--r--   0        0        0      787 2021-09-30 13:01:10.072001 micone-0.8.1/micone/pipelines/modules/network_inference/direct/export_gml.nf
--rw-r--r--   0        0        0     1301 2021-09-30 13:01:27.188667 micone-0.8.1/micone/pipelines/modules/network_inference/direct/flashweave.nf
--rw-r--r--   0        0        0      471 2021-05-22 14:29:12.051720 micone-0.8.1/micone/pipelines/modules/network_inference/direct/flashweave_workflow.nf
--rw-r--r--   0        0        0     1073 2021-09-30 13:01:37.655334 micone-0.8.1/micone/pipelines/modules/network_inference/direct/mldm.nf
--rw-r--r--   0        0        0      382 2021-05-22 14:26:18.595048 micone-0.8.1/micone/pipelines/modules/network_inference/direct/mldm_workflow.nf
--rw-r--r--   0        0        0     1328 2021-09-30 13:01:50.338668 micone-0.8.1/micone/pipelines/modules/network_inference/direct/spieceasi.nf
--rw-r--r--   0        0        0      407 2021-05-22 14:13:07.975023 micone-0.8.1/micone/pipelines/modules/network_inference/direct/spieceasi_workflow.nf
--rw-r--r--   0        0        0      837 2021-10-08 19:10:52.270793 micone-0.8.1/micone/pipelines/modules/network_inference/network/create_consensus.nf
--rw-r--r--   0        0        0     1090 2021-10-08 19:10:52.270793 micone-0.8.1/micone/pipelines/modules/network_inference/network/make_network_with_pvalue.nf
--rw-r--r--   0        0        0      975 2021-10-08 19:10:52.270793 micone-0.8.1/micone/pipelines/modules/network_inference/network/make_network_without_pvalue.nf
--rw-r--r--   0        0        0      464 2021-10-08 19:10:52.270793 micone-0.8.1/micone/pipelines/modules/network_inference/network/merge_pvalues.nf
--rw-r--r--   0        0        0     2381 2021-10-07 23:52:49.191436 micone-0.8.1/micone/pipelines/modules/network_inference/network_inference_workflow.nf
--rw-r--r--   0        0        0      844 2021-10-06 18:44:26.850168 micone-0.8.1/micone/pipelines/modules/otu_processing/export/biom2tsv.nf
--rw-r--r--   0        0        0      738 2021-05-17 14:24:32.103429 micone-0.8.1/micone/pipelines/modules/otu_processing/otu_processing_workflow.nf
--rw-r--r--   0        0        0      688 2021-09-30 12:54:51.155331 micone-0.8.1/micone/pipelines/modules/otu_processing/transform/group.nf
--rw-r--r--   0        0        0     1138 2021-09-30 12:47:55.471995 micone-0.8.1/micone/pipelines/modules/otu_processing/transform/normalize.nf
--rw-r--r--   0        0        0      731 2021-09-30 12:41:45.108659 micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/add_md2biom.nf
--rw-r--r--   0        0        0     1146 2021-09-29 14:47:37.687923 micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/blast.nf
--rw-r--r--   0        0        0      538 2021-05-16 19:19:16.056874 micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/blast_workflow.nf
--rw-r--r--   0        0        0      357 2021-05-16 19:17:47.280206 micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/import_reads.nf
--rw-r--r--   0        0        0      250 2021-05-11 13:46:44.384920 micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/import_references.nf
--rw-r--r--   0        0        0      895 2021-09-29 14:47:32.087923 micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/naive_bayes.nf
--rw-r--r--   0        0        0      574 2021-05-26 15:40:20.331225 micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/naive_bayes_workflow.nf
--rw-r--r--   0        0        0      375 2021-03-24 15:21:31.681298 micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/train_classifier.nf
--rw-r--r--   0        0        0      726 2021-05-26 15:39:49.777892 micone-0.8.1/micone/pipelines/modules/tax_assignment/tax_assignment_workflow.nf
--rw-r--r--   0        0        0     1482 2021-09-28 17:39:38.527889 micone-0.8.1/micone/pipelines/modules/utils/dc_data_ingestion.nf
--rw-r--r--   0        0        0     1298 2021-05-25 20:49:40.364823 micone-0.8.1/micone/pipelines/modules/utils/ni_data_ingestion.nf
--rw-r--r--   0        0        0      646 2021-05-25 20:43:40.384820 micone-0.8.1/micone/pipelines/modules/utils/op_data_ingestion.nf
--rw-r--r--   0        0        0     1482 2021-10-09 14:33:11.690725 micone-0.8.1/micone/pipelines/modules/utils/sp_data_ingesetion.nf
--rw-r--r--   0        0        0     1057 2021-05-25 20:46:51.708155 micone-0.8.1/micone/pipelines/modules/utils/ta_data_ingestion.nf
--rw-r--r--   0        0        0      520 2021-10-06 18:44:26.850168 micone-0.8.1/micone/pipelines/nextflow.config
--rw-r--r--   0        0        0    17476 2021-03-11 16:39:23.431557 micone-0.8.1/micone/pipelines/pipeline.py
--rw-r--r--   0        0        0    16880 2021-02-01 18:20:34.718444 micone-0.8.1/micone/pipelines/process.py
--rw-r--r--   0        0        0     5657 2020-12-17 21:32:30.074977 micone-0.8.1/micone/pipelines/template.py
--rw-r--r--   0        0        0      632 2021-03-19 20:15:23.718050 micone-0.8.1/micone/pipelines/templates/denoise_cluster/chimera_checking/create_seqtable.py
--rw-r--r--   0        0        0      360 2021-03-19 20:17:13.484717 micone-0.8.1/micone/pipelines/templates/denoise_cluster/chimera_checking/export_files.sh
--rw-r--r--   0        0        0      371 2021-05-16 14:52:39.070093 micone-0.8.1/micone/pipelines/templates/denoise_cluster/chimera_checking/import_files.sh
--rw-r--r--   0        0        0      801 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/denoise_cluster/chimera_checking/remove_chimeras.R
--rw-r--r--   0        0        0      478 2021-03-19 20:17:13.484717 micone-0.8.1/micone/pipelines/templates/denoise_cluster/chimera_checking/remove_chimeras.sh
--rw-r--r--   0        0        0     1131 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/dada2.R
--rw-r--r--   0        0        0      704 2021-05-15 21:22:40.776928 micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/deblur.sh
--rw-r--r--   0        0        0     1517 2021-05-15 20:51:49.433581 micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/fastq2fasta.py
--rw-r--r--   0        0        0     1600 2021-03-19 19:58:34.728043 micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/hashing2.py
--rw-r--r--   0        0        0     1499 2021-05-27 21:13:56.140961 micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/hashing3.py
--rw-r--r--   0        0        0      860 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/make_biom_repseqs.py
--rw-r--r--   0        0        0      392 2021-05-15 20:47:38.673579 micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/pick_closed_reference_otus.sh
--rw-r--r--   0        0        0      260 2021-05-15 20:59:56.890251 micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/pick_de_novo_otus.sh
--rw-r--r--   0        0        0      352 2021-05-15 20:54:16.086915 micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/pick_open_reference_otus.sh
--rw-r--r--   0        0        0      297 2021-05-26 21:21:11.041078 micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/demultiplex_illumina.sh
--rw-r--r--   0        0        0     1102 2021-05-26 15:08:48.807906 micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/export_sequences.py
--rw-r--r--   0        0        0      525 2021-05-27 13:19:04.367832 micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/export_visualization.py
--rw-r--r--   0        0        0      535 2021-05-15 19:34:44.150215 micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/import_sequences.py
--rw-r--r--   0        0        0      266 2021-05-15 13:13:52.863382 micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/import_sequences.sh
--rw-r--r--   0        0        0      138 2021-05-25 12:56:48.437953 micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/join_reads.sh
--rw-r--r--   0        0        0     4915 2021-05-27 13:43:39.987822 micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/quality_analysis.py
--rw-r--r--   0        0        0     1166 2021-05-15 19:57:43.250225 micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/trimming.R
--rw-r--r--   0        0        0      317 2021-05-18 20:47:20.916946 micone-0.8.1/micone/pipelines/templates/network_inference/bootstrap/calculate_pvalues.sh
--rw-r--r--   0        0        0      871 2021-03-19 21:14:28.514742 micone-0.8.1/micone/pipelines/templates/network_inference/bootstrap/filter.py
--rw-r--r--   0        0        0      243 2021-05-18 21:09:03.690289 micone-0.8.1/micone/pipelines/templates/network_inference/bootstrap/resample.sh
--rw-r--r--   0        0        0     1464 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/network_inference/correlation/pearson.py
--rw-r--r--   0        0        0      839 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/network_inference/correlation/propr.R
--rw-r--r--   0        0        0      499 2021-05-27 21:33:22.137620 micone-0.8.1/micone/pipelines/templates/network_inference/correlation/sparcc.sh
--rw-r--r--   0        0        0     1445 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/network_inference/correlation/spearman.py
--rw-r--r--   0        0        0      976 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/network_inference/direct/export_gml.py
--rw-r--r--   0        0        0      882 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/network_inference/direct/flashweave.jl
--rw-r--r--   0        0        0      835 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/network_inference/direct/mldm.R
--rw-r--r--   0        0        0     1592 2021-05-27 13:42:52.217822 micone-0.8.1/micone/pipelines/templates/network_inference/direct/spieceasi.R
--rw-r--r--   0        0        0     1328 2021-10-08 19:10:52.270793 micone-0.8.1/micone/pipelines/templates/network_inference/network/create_consensus.py
--rw-r--r--   0        0        0     1829 2021-10-07 13:11:52.521160 micone-0.8.1/micone/pipelines/templates/network_inference/network/make_network_with_pvalue.py
--rw-r--r--   0        0        0     1578 2021-10-07 13:11:52.521160 micone-0.8.1/micone/pipelines/templates/network_inference/network/make_network_without_pvalue.py
--rw-r--r--   0        0        0      780 2021-10-08 19:10:52.270793 micone-0.8.1/micone/pipelines/templates/network_inference/network/merge_pvalues.py
--rw-r--r--   0        0        0      298 2021-05-16 20:58:45.760248 micone-0.8.1/micone/pipelines/templates/otu_processing/export/biom2tsv.py
--rw-r--r--   0        0        0      803 2021-05-16 20:50:58.503578 micone-0.8.1/micone/pipelines/templates/otu_processing/transform/group.py
--rw-r--r--   0        0        0     1151 2021-05-16 20:31:56.436904 micone-0.8.1/micone/pipelines/templates/otu_processing/transform/normalize.py
--rw-r--r--   0        0        0     1758 2021-05-16 19:05:33.926868 micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/add_md2biom.py
--rw-r--r--   0        0        0      548 2021-05-16 19:28:38.260211 micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/assign_taxonomy_blast.sh
--rw-r--r--   0        0        0      578 2021-05-16 19:09:45.143536 micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/assign_taxonomy_naivebayes.sh
--rw-r--r--   0        0        0      150 2021-03-19 21:03:45.874738 micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/import_reads.sh
--rw-r--r--   0        0        0      429 2021-03-19 21:04:31.741405 micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/import_references.sh
--rw-r--r--   0        0        0      721 2021-03-19 21:05:07.628072 micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/train_classifier.sh
--rw-r--r--   0        0        0       39 2020-12-17 21:32:30.061644 micone-0.8.1/micone/setup/__init__.py
--rw-r--r--   0        0        0     3682 2021-10-06 19:10:16.436840 micone-0.8.1/micone/setup/environments.py
--rw-r--r--   0        0        0       29 2020-12-17 21:32:30.058311 micone-0.8.1/micone/utils/__init__.py
--rw-r--r--   0        0        0     1828 2021-01-21 14:19:56.758060 micone-0.8.1/micone/utils/spinner.py
--rw-r--r--   0        0        0      323 2020-12-17 21:32:30.114977 micone-0.8.1/micone/validation/__init__.py
--rw-r--r--   0        0        0     6495 2020-12-17 21:32:30.114977 micone-0.8.1/micone/validation/network_schema.py
--rw-r--r--   0        0        0     8041 2021-01-25 21:08:54.335553 micone-0.8.1/micone/validation/otu_schema.py
--rw-r--r--   0        0        0     7159 2020-12-17 21:32:30.114977 micone-0.8.1/micone/validation/otu_validator.py
--rw-r--r--   0        0        0     1504 2021-10-09 15:03:38.227344 micone-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     8649 2021-10-09 15:03:42.551901 micone-0.8.1/setup.py
--rw-r--r--   0        0        0     6412 2021-10-09 15:03:42.552284 micone-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2020-12-17 21:32:29.671644 micone-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5116 2021-03-02 21:18:20.768048 micone-0.9.0/README.md
+-rw-r--r--   0        0        0      211 2021-03-16 15:05:22.728177 micone-0.9.0/micone/__init__.py
+-rw-r--r--   0        0        0     5000 2021-03-13 17:29:35.811533 micone-0.9.0/micone/cli.py
+-rw-r--r--   0        0        0       98 2020-12-17 21:32:30.064978 micone-0.9.0/micone/config/__init__.py
+-rw-r--r--   0        0        0     3205 2020-12-17 21:32:30.064978 micone-0.9.0/micone/config/config.py
+-rw-r--r--   0        0        0     3054 2020-12-17 21:32:30.068311 micone-0.9.0/micone/config/datatypes.py
+-rw-r--r--   0        0        0    12861 2021-03-02 15:49:42.944572 micone-0.9.0/micone/config/params.py
+-rw-r--r--   0        0        0      128 2020-12-17 21:32:30.064978 micone-0.9.0/micone/conversion/__init__.py
+-rw-r--r--   0        0        0      864 2020-12-17 21:32:30.064978 micone-0.9.0/micone/conversion/network_converter.py
+-rw-r--r--   0        0        0        0 2020-12-17 21:32:30.064978 micone-0.9.0/micone/conversion/otu_converter.py
+-rw-r--r--   0        0        0     2392 2021-01-25 21:42:09.462263 micone-0.9.0/micone/conversion/taxmetadata_converter.py
+-rw-r--r--   0        0        0       24 2020-12-17 21:32:30.054977 micone-0.9.0/micone/logging/__init__.py
+-rw-r--r--   0        0        0     2146 2021-01-01 16:11:29.961447 micone-0.9.0/micone/logging/logger.py
+-rw-r--r--   0        0        0      119 2020-12-17 21:32:30.061644 micone-0.9.0/micone/main/__init__.py
+-rw-r--r--   0        0        0     8789 2021-02-11 21:32:26.968329 micone-0.9.0/micone/main/lineage.py
+-rw-r--r--   0        0        0    31005 2021-10-07 15:26:57.471219 micone-0.9.0/micone/main/network.py
+-rw-r--r--   0        0        0    21335 2021-10-18 14:05:15.931607 micone-0.9.0/micone/main/network_group.py
+-rw-r--r--   0        0        0    16629 2021-10-20 19:53:38.248966 micone-0.9.0/micone/main/otu.py
+-rw-r--r--   0        0        0       24 2020-12-17 21:32:30.058311 micone-0.9.0/micone/micone.py
+-rw-r--r--   0        0        0      142 2020-12-17 21:32:30.068311 micone-0.9.0/micone/pipelines/__init__.py
+-rw-r--r--   0        0        0     7199 2020-12-17 21:32:30.068311 micone-0.9.0/micone/pipelines/command.py
+-rw-r--r--   0        0        0     1553 2021-10-30 11:48:32.484272 micone-0.9.0/micone/pipelines/configs/denoise_cluster.config
+-rw-r--r--   0        0        0     1776 2021-10-23 11:47:25.301049 micone-0.9.0/micone/pipelines/configs/network_inference.config
+-rw-r--r--   0        0        0      757 2021-10-25 18:21:36.489465 micone-0.9.0/micone/pipelines/configs/otu_processing.config
+-rw-r--r--   0        0        0     1516 2021-09-27 14:39:04.744584 micone-0.9.0/micone/pipelines/configs/process.config
+-rw-r--r--   0        0        0      549 2021-09-28 14:34:22.297810 micone-0.9.0/micone/pipelines/configs/profiles.config
+-rw-r--r--   0        0        0     1066 2021-10-25 18:22:01.229466 micone-0.9.0/micone/pipelines/configs/sequence_processing.config
+-rw-r--r--   0        0        0      822 2021-10-30 13:50:39.737388 micone-0.9.0/micone/pipelines/configs/tax_assignment.config
+-rw-r--r--   0        0        0      329 2021-05-27 15:05:54.871120 micone-0.9.0/micone/pipelines/envs/micone-dada2/env.yml
+-rw-r--r--   0        0        0      190 2021-02-16 23:22:23.388997 micone-0.9.0/micone/pipelines/envs/micone-flashweave/env.yml
+-rw-r--r--   0        0        0      659 2021-10-09 14:31:55.347394 micone-0.9.0/micone/pipelines/envs/micone-flashweave/post_install.sh
+-rw-r--r--   0        0        0      152 2021-01-29 20:22:23.384587 micone-0.9.0/micone/pipelines/envs/micone-mldm/env.yml
+-rw-r--r--   0        0        0      389 2021-01-29 20:32:52.407925 micone-0.9.0/micone/pipelines/envs/micone-mldm/post_install.sh
+-rw-r--r--   0        0        0      203 2021-02-10 15:55:24.037865 micone-0.9.0/micone/pipelines/envs/micone-netcomi/env.yml
+-rw-r--r--   0        0        0      241 2021-02-10 16:08:51.394549 micone-0.9.0/micone/pipelines/envs/micone-netcomi/post_install.sh
+-rw-r--r--   0        0        0      170 2021-02-09 21:38:14.925624 micone-0.9.0/micone/pipelines/envs/micone-propr/env.yml
+-rw-r--r--   0        0        0      113 2021-02-09 21:38:37.268957 micone-0.9.0/micone/pipelines/envs/micone-propr/post_install.sh
+-rw-r--r--   0        0        0      217 2021-05-27 14:56:49.747790 micone-0.9.0/micone/pipelines/envs/micone-qiime1/env.yml
+-rw-r--r--   0        0        0      133 2021-01-29 14:16:04.747765 micone-0.9.0/micone/pipelines/envs/micone-qiime1/post_install.sh
+-rw-r--r--   0        0        0     9224 2021-10-21 15:21:08.112202 micone-0.9.0/micone/pipelines/envs/micone-qiime2/env.yml
+-rw-r--r--   0        0        0      117 2021-10-19 15:35:00.117281 micone-0.9.0/micone/pipelines/envs/micone-qiime2/post_install.sh
+-rw-r--r--   0        0        0      202 2021-10-08 18:08:08.414113 micone-0.9.0/micone/pipelines/envs/micone-sparcc/env.yml
+-rw-r--r--   0        0        0      175 2021-01-29 17:43:00.387854 micone-0.9.0/micone/pipelines/envs/micone-spieceasi/env.yml
+-rw-r--r--   0        0        0      687 2021-10-22 20:10:52.932918 micone-0.9.0/micone/pipelines/functions/functions.nf
+-rw-r--r--   0        0        0       74 2020-12-17 21:32:30.071644 micone-0.9.0/micone/pipelines/helpers.py
+-rw-r--r--   0        0        0     1535 2021-10-21 14:57:47.098838 micone-0.9.0/micone/pipelines/main.nf
+-rw-r--r--   0        0        0      375 2021-10-16 15:31:38.777587 micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/create_seqtable.nf
+-rw-r--r--   0        0        0      702 2021-10-16 15:31:48.454253 micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/export_files.nf
+-rw-r--r--   0        0        0      394 2021-10-16 15:32:02.850920 micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/import_files.nf
+-rw-r--r--   0        0        0      942 2021-10-30 13:38:32.390743 micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/remove_bimera.nf
+-rw-r--r--   0        0        0      592 2021-10-16 15:31:14.864254 micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/remove_bimera_workflow.nf
+-rw-r--r--   0        0        0      669 2021-10-16 15:32:29.317586 micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/uchime.nf
+-rw-r--r--   0        0        0      557 2021-10-16 15:31:24.157587 micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/uchime_workflow.nf
+-rw-r--r--   0        0        0     1379 2021-10-27 17:05:11.810068 micone-0.9.0/micone/pipelines/modules/denoise_cluster/denoise_cluster_workflow.nf
+-rw-r--r--   0        0        0     1195 2021-10-30 12:29:45.880865 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/closed_reference.nf
+-rw-r--r--   0        0        0     1181 2021-10-30 14:59:45.690598 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/closed_reference_workflow.nf
+-rw-r--r--   0        0        0      778 2021-10-27 17:05:11.810068 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/dada2_paired.nf
+-rw-r--r--   0        0        0      778 2021-10-27 17:05:11.810068 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/dada2_single.nf
+-rw-r--r--   0        0        0      953 2021-10-27 21:34:50.650125 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/dada2_workflow.nf
+-rw-r--r--   0        0        0      915 2021-10-30 12:29:43.904198 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/de_novo.nf
+-rw-r--r--   0        0        0     1016 2021-10-28 11:50:35.221211 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/de_novo_workflow.nf
+-rw-r--r--   0        0        0     1017 2021-10-30 12:29:42.707532 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/deblur.nf
+-rw-r--r--   0        0        0      896 2021-10-27 21:34:50.650125 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/deblur_workflow.nf
+-rw-r--r--   0        0        0      401 2021-10-27 17:05:11.810068 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/fastq2fasta.nf
+-rw-r--r--   0        0        0      767 2021-10-30 14:13:36.414014 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/hashing2.nf
+-rw-r--r--   0        0        0      911 2021-10-30 13:38:54.094075 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/hashing3.nf
+-rw-r--r--   0        0        0      800 2021-10-30 14:32:41.300646 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/join_reads.nf
+-rw-r--r--   0        0        0      547 2021-10-28 12:06:13.274574 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/make_biom_repseqs.nf
+-rw-r--r--   0        0        0     1179 2021-10-30 12:29:41.697532 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/open_reference.nf
+-rw-r--r--   0        0        0     1163 2021-10-28 12:33:16.511291 micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/open_reference_workflow.nf
+-rw-r--r--   0        0        0      431 2021-05-11 14:51:17.508373 micone-0.9.0/micone/pipelines/modules/network_inference/bootstrap/filter.nf
+-rw-r--r--   0        0        0      898 2021-09-30 12:57:04.101999 micone-0.9.0/micone/pipelines/modules/network_inference/bootstrap/pvalue.nf
+-rw-r--r--   0        0        0      546 2021-05-27 21:17:29.760959 micone-0.9.0/micone/pipelines/modules/network_inference/bootstrap/resample.nf
+-rw-r--r--   0        0        0     1085 2021-09-30 12:57:07.391999 micone-0.9.0/micone/pipelines/modules/network_inference/correlation/pearson.nf
+-rw-r--r--   0        0        0      624 2021-05-25 14:00:56.687981 micone-0.9.0/micone/pipelines/modules/network_inference/correlation/pearson_workflow.nf
+-rw-r--r--   0        0        0     1073 2021-09-30 12:59:11.475333 micone-0.9.0/micone/pipelines/modules/network_inference/correlation/propr.nf
+-rw-r--r--   0        0        0      614 2021-05-25 14:01:06.214647 micone-0.9.0/micone/pipelines/modules/network_inference/correlation/propr_workflow.nf
+-rw-r--r--   0        0        0     1162 2021-09-30 13:00:01.455334 micone-0.9.0/micone/pipelines/modules/network_inference/correlation/sparcc.nf
+-rw-r--r--   0        0        0      619 2021-05-25 14:01:15.834647 micone-0.9.0/micone/pipelines/modules/network_inference/correlation/sparcc_workflow.nf
+-rw-r--r--   0        0        0     1090 2021-09-30 13:00:12.595334 micone-0.9.0/micone/pipelines/modules/network_inference/correlation/spearman.nf
+-rw-r--r--   0        0        0      629 2021-05-25 14:01:25.091314 micone-0.9.0/micone/pipelines/modules/network_inference/correlation/spearman_workflow.nf
+-rw-r--r--   0        0        0      787 2021-09-30 13:01:10.072001 micone-0.9.0/micone/pipelines/modules/network_inference/direct/export_gml.nf
+-rw-r--r--   0        0        0     1301 2021-09-30 13:01:27.188667 micone-0.9.0/micone/pipelines/modules/network_inference/direct/flashweave.nf
+-rw-r--r--   0        0        0      471 2021-05-22 14:29:12.051720 micone-0.9.0/micone/pipelines/modules/network_inference/direct/flashweave_workflow.nf
+-rw-r--r--   0        0        0     1073 2021-09-30 13:01:37.655334 micone-0.9.0/micone/pipelines/modules/network_inference/direct/mldm.nf
+-rw-r--r--   0        0        0      382 2021-05-22 14:26:18.595048 micone-0.9.0/micone/pipelines/modules/network_inference/direct/mldm_workflow.nf
+-rw-r--r--   0        0        0     1328 2021-09-30 13:01:50.338668 micone-0.9.0/micone/pipelines/modules/network_inference/direct/spieceasi.nf
+-rw-r--r--   0        0        0      407 2021-05-22 14:13:07.975023 micone-0.9.0/micone/pipelines/modules/network_inference/direct/spieceasi_workflow.nf
+-rw-r--r--   0        0        0      837 2021-10-08 19:10:52.270793 micone-0.9.0/micone/pipelines/modules/network_inference/network/create_consensus.nf
+-rw-r--r--   0        0        0     1090 2021-10-22 14:49:02.629516 micone-0.9.0/micone/pipelines/modules/network_inference/network/make_network_with_pvalue.nf
+-rw-r--r--   0        0        0      975 2021-10-22 14:49:17.072849 micone-0.9.0/micone/pipelines/modules/network_inference/network/make_network_without_pvalue.nf
+-rw-r--r--   0        0        0      464 2021-10-08 19:10:52.270793 micone-0.9.0/micone/pipelines/modules/network_inference/network/merge_pvalues.nf
+-rw-r--r--   0        0        0     2381 2021-10-21 13:43:18.595409 micone-0.9.0/micone/pipelines/modules/network_inference/network_inference_workflow.nf
+-rw-r--r--   0        0        0      844 2021-10-06 18:44:26.850168 micone-0.9.0/micone/pipelines/modules/otu_processing/export/biom2tsv.nf
+-rw-r--r--   0        0        0     1068 2021-10-27 19:12:18.040095 micone-0.9.0/micone/pipelines/modules/otu_processing/otu_processing_workflow.nf
+-rw-r--r--   0        0        0      798 2021-10-22 14:27:22.422844 micone-0.9.0/micone/pipelines/modules/otu_processing/transform/fork.nf
+-rw-r--r--   0        0        0      688 2021-09-30 12:54:51.155331 micone-0.9.0/micone/pipelines/modules/otu_processing/transform/group.nf
+-rw-r--r--   0        0        0     1263 2021-10-21 13:37:36.782068 micone-0.9.0/micone/pipelines/modules/otu_processing/transform/normalize.nf
+-rw-r--r--   0        0        0     1084 2021-10-24 00:11:43.250728 micone-0.9.0/micone/pipelines/modules/sequence_processing/demultiplexing/demultiplexing_illumina_paired.nf
+-rw-r--r--   0        0        0     1084 2021-10-24 00:11:34.827395 micone-0.9.0/micone/pipelines/modules/sequence_processing/demultiplexing/demultiplexing_illumina_single.nf
+-rw-r--r--   0        0        0      770 2021-10-26 14:40:39.311460 micone-0.9.0/micone/pipelines/modules/sequence_processing/demultiplexing/demultiplexing_paired_workflow.nf
+-rw-r--r--   0        0        0      751 2021-10-26 14:40:27.391460 micone-0.9.0/micone/pipelines/modules/sequence_processing/demultiplexing/demultiplexing_single_workflow.nf
+-rw-r--r--   0        0        0      755 2021-10-26 14:39:42.594792 micone-0.9.0/micone/pipelines/modules/sequence_processing/demultiplexing/export_sequences.nf
+-rw-r--r--   0        0        0      402 2021-10-22 20:00:31.346249 micone-0.9.0/micone/pipelines/modules/sequence_processing/demultiplexing/import_sequences_paired.nf
+-rw-r--r--   0        0        0      382 2021-10-22 20:00:37.486249 micone-0.9.0/micone/pipelines/modules/sequence_processing/demultiplexing/import_sequences_single.nf
+-rw-r--r--   0        0        0     1149 2021-10-27 17:05:11.810068 micone-0.9.0/micone/pipelines/modules/sequence_processing/sequence_processing_paired_workflow.nf
+-rw-r--r--   0        0        0     1153 2021-10-27 17:05:11.810068 micone-0.9.0/micone/pipelines/modules/sequence_processing/sequence_processing_single_workflow.nf
+-rw-r--r--   0        0        0      533 2021-10-22 20:00:52.919583 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/export_visualization_paired.nf
+-rw-r--r--   0        0        0      486 2021-10-22 20:00:59.202916 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/export_visualization_single.nf
+-rw-r--r--   0        0        0      384 2021-10-26 14:41:38.841461 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/import_sequences_paired.nf
+-rw-r--r--   0        0        0      384 2021-10-26 14:41:24.798127 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/import_sequences_single.nf
+-rw-r--r--   0        0        0      719 2021-10-22 20:01:30.289583 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/quality_analysis_paired.nf
+-rw-r--r--   0        0        0      691 2021-10-22 20:01:44.612916 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/quality_analysis_single.nf
+-rw-r--r--   0        0        0     1030 2021-10-27 17:05:11.810068 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/trimming_paired.nf
+-rw-r--r--   0        0        0      878 2021-10-27 17:05:11.810068 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/trimming_paired_workflow.nf
+-rw-r--r--   0        0        0     1030 2021-10-27 17:05:11.810068 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/trimming_single.nf
+-rw-r--r--   0        0        0      878 2021-10-27 17:05:11.813401 micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/trimming_single_workflow.nf
+-rw-r--r--   0        0        0      783 2021-10-30 13:41:58.480737 micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/add_md2biom.nf
+-rw-r--r--   0        0        0     1242 2021-10-28 15:37:07.714965 micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/blast.nf
+-rw-r--r--   0        0        0      638 2021-10-28 15:26:31.498279 micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/blast_workflow.nf
+-rw-r--r--   0        0        0      357 2021-05-16 19:17:47.280206 micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/import_reads.nf
+-rw-r--r--   0        0        0      250 2021-05-11 13:46:44.384920 micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/import_references.nf
+-rw-r--r--   0        0        0      932 2021-10-28 12:40:04.637971 micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/naive_bayes.nf
+-rw-r--r--   0        0        0      661 2021-10-28 12:40:39.311305 micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/naive_bayes_workflow.nf
+-rw-r--r--   0        0        0      375 2021-03-24 15:21:31.681298 micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/train_classifier.nf
+-rw-r--r--   0        0        0      726 2021-05-26 15:39:49.777892 micone-0.9.0/micone/pipelines/modules/tax_assignment/tax_assignment_workflow.nf
+-rw-r--r--   0        0        0     1392 2021-10-27 19:41:20.153435 micone-0.9.0/micone/pipelines/modules/utils/dc_data_ingestion.nf
+-rw-r--r--   0        0        0     1298 2021-05-25 20:49:40.364823 micone-0.9.0/micone/pipelines/modules/utils/ni_data_ingestion.nf
+-rw-r--r--   0        0        0      646 2021-05-25 20:43:40.384820 micone-0.9.0/micone/pipelines/modules/utils/op_data_ingestion.nf
+-rw-r--r--   0        0        0     1753 2021-10-25 18:25:07.319466 micone-0.9.0/micone/pipelines/modules/utils/spp_data_ingestion.nf
+-rw-r--r--   0        0        0     1519 2021-10-22 20:33:09.189589 micone-0.9.0/micone/pipelines/modules/utils/sps_data_ingestion.nf
+-rw-r--r--   0        0        0     1057 2021-05-25 20:46:51.708155 micone-0.9.0/micone/pipelines/modules/utils/ta_data_ingestion.nf
+-rw-r--r--   0        0        0      605 2021-10-21 15:04:17.082180 micone-0.9.0/micone/pipelines/nextflow.config
+-rw-r--r--   0        0        0    17476 2021-03-11 16:39:23.431557 micone-0.9.0/micone/pipelines/pipeline.py
+-rw-r--r--   0        0        0    16880 2021-02-01 18:20:34.718444 micone-0.9.0/micone/pipelines/process.py
+-rw-r--r--   0        0        0     5657 2020-12-17 21:32:30.074977 micone-0.9.0/micone/pipelines/template.py
+-rw-r--r--   0        0        0      632 2021-03-19 20:15:23.718050 micone-0.9.0/micone/pipelines/templates/denoise_cluster/chimera_checking/create_seqtable.py
+-rw-r--r--   0        0        0      360 2021-03-19 20:17:13.484717 micone-0.9.0/micone/pipelines/templates/denoise_cluster/chimera_checking/export_files.sh
+-rw-r--r--   0        0        0      371 2021-05-16 14:52:39.070093 micone-0.9.0/micone/pipelines/templates/denoise_cluster/chimera_checking/import_files.sh
+-rw-r--r--   0        0        0      820 2021-10-27 20:25:06.156777 micone-0.9.0/micone/pipelines/templates/denoise_cluster/chimera_checking/remove_chimeras.R
+-rw-r--r--   0        0        0      478 2021-03-19 20:17:13.484717 micone-0.9.0/micone/pipelines/templates/denoise_cluster/chimera_checking/remove_chimeras.sh
+-rw-r--r--   0        0        0     1038 2021-10-27 20:07:01.766774 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/cluster_closed_reference.sh
+-rw-r--r--   0        0        0      908 2021-10-27 20:06:08.593440 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/cluster_de_novo.sh
+-rw-r--r--   0        0        0     1043 2021-10-27 20:06:36.886773 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/cluster_open_reference.sh
+-rw-r--r--   0        0        0     2270 2021-10-27 19:46:30.593436 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/dada2_paired.R
+-rw-r--r--   0        0        0     1279 2021-10-27 19:46:14.886769 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/dada2_single.R
+-rw-r--r--   0        0        0      860 2021-10-27 20:05:01.783440 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/deblur.sh
+-rw-r--r--   0        0        0     1522 2021-10-27 21:34:22.033459 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/fastq2fasta.py
+-rw-r--r--   0        0        0     2643 2021-10-21 20:43:04.932618 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/hashing2.py
+-rw-r--r--   0        0        0     2428 2021-10-21 20:43:36.942619 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/hashing3.py
+-rw-r--r--   0        0        0      516 2021-10-27 17:05:11.813401 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/join_reads.sh
+-rw-r--r--   0        0        0     1160 2021-10-27 20:08:45.713441 micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/make_biom_repseqs.py
+-rw-r--r--   0        0        0      317 2021-05-18 20:47:20.916946 micone-0.9.0/micone/pipelines/templates/network_inference/bootstrap/calculate_pvalues.sh
+-rw-r--r--   0        0        0      871 2021-03-19 21:14:28.514742 micone-0.9.0/micone/pipelines/templates/network_inference/bootstrap/filter.py
+-rw-r--r--   0        0        0      243 2021-05-18 21:09:03.690289 micone-0.9.0/micone/pipelines/templates/network_inference/bootstrap/resample.sh
+-rw-r--r--   0        0        0     1464 2021-05-27 13:42:52.217822 micone-0.9.0/micone/pipelines/templates/network_inference/correlation/pearson.py
+-rw-r--r--   0        0        0      839 2021-05-27 13:42:52.217822 micone-0.9.0/micone/pipelines/templates/network_inference/correlation/propr.R
+-rw-r--r--   0        0        0      499 2021-05-27 21:33:22.137620 micone-0.9.0/micone/pipelines/templates/network_inference/correlation/sparcc.sh
+-rw-r--r--   0        0        0     1445 2021-05-27 13:42:52.217822 micone-0.9.0/micone/pipelines/templates/network_inference/correlation/spearman.py
+-rw-r--r--   0        0        0      976 2021-05-27 13:42:52.217822 micone-0.9.0/micone/pipelines/templates/network_inference/direct/export_gml.py
+-rw-r--r--   0        0        0      882 2021-05-27 13:42:52.217822 micone-0.9.0/micone/pipelines/templates/network_inference/direct/flashweave.jl
+-rw-r--r--   0        0        0      835 2021-05-27 13:42:52.217822 micone-0.9.0/micone/pipelines/templates/network_inference/direct/mldm.R
+-rw-r--r--   0        0        0     1592 2021-05-27 13:42:52.217822 micone-0.9.0/micone/pipelines/templates/network_inference/direct/spieceasi.R
+-rw-r--r--   0        0        0     1336 2021-10-18 14:05:35.734940 micone-0.9.0/micone/pipelines/templates/network_inference/network/create_consensus.py
+-rw-r--r--   0        0        0     1997 2021-10-23 11:50:37.301047 micone-0.9.0/micone/pipelines/templates/network_inference/network/make_network_with_pvalue.py
+-rw-r--r--   0        0        0     1786 2021-10-23 11:51:43.461047 micone-0.9.0/micone/pipelines/templates/network_inference/network/make_network_without_pvalue.py
+-rw-r--r--   0        0        0      788 2021-10-18 13:54:24.868271 micone-0.9.0/micone/pipelines/templates/network_inference/network/merge_pvalues.py
+-rw-r--r--   0        0        0      298 2021-05-16 20:58:45.760248 micone-0.9.0/micone/pipelines/templates/otu_processing/export/biom2tsv.py
+-rw-r--r--   0        0        0     1201 2021-10-30 13:46:07.340729 micone-0.9.0/micone/pipelines/templates/otu_processing/transform/fork.py
+-rw-r--r--   0        0        0      803 2021-05-16 20:50:58.503578 micone-0.9.0/micone/pipelines/templates/otu_processing/transform/group.py
+-rw-r--r--   0        0        0     1176 2021-10-25 18:19:17.542798 micone-0.9.0/micone/pipelines/templates/otu_processing/transform/normalize.py
+-rw-r--r--   0        0        0      299 2021-10-25 18:24:34.002799 micone-0.9.0/micone/pipelines/templates/sequence_processing/demultiplexing/demultiplex_illumina_paired.sh
+-rw-r--r--   0        0        0      299 2021-10-25 18:24:34.002799 micone-0.9.0/micone/pipelines/templates/sequence_processing/demultiplexing/demultiplex_illumina_single.sh
+-rw-r--r--   0        0        0      110 2021-10-26 12:38:10.997969 micone-0.9.0/micone/pipelines/templates/sequence_processing/demultiplexing/export_sequences.sh
+-rw-r--r--   0        0        0      310 2021-10-09 16:08:27.340575 micone-0.9.0/micone/pipelines/templates/sequence_processing/demultiplexing/import_sequences_paired.sh
+-rw-r--r--   0        0        0      266 2021-05-15 13:13:52.863382 micone-0.9.0/micone/pipelines/templates/sequence_processing/demultiplexing/import_sequences_single.sh
+-rw-r--r--   0        0        0      525 2021-05-27 13:19:04.367832 micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/export_visualization.py
+-rw-r--r--   0        0        0      300 2021-10-26 14:41:56.084795 micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/import_sequences_paired.sh
+-rw-r--r--   0        0        0      291 2021-10-26 14:42:05.841462 micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/import_sequences_single.sh
+-rw-r--r--   0        0        0     4853 2021-10-11 13:53:15.845289 micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/quality_analysis_paired.py
+-rw-r--r--   0        0        0     4915 2021-05-27 13:43:39.987822 micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/quality_analysis_single.py
+-rw-r--r--   0        0        0     2041 2021-10-27 17:05:11.813401 micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/trimming_paired.R
+-rw-r--r--   0        0        0     1166 2021-10-27 16:56:37.710066 micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/trimming_single.R
+-rw-r--r--   0        0        0     1785 2021-10-27 21:16:52.260121 micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/add_md2biom.py
+-rw-r--r--   0        0        0      548 2021-05-16 19:28:38.260211 micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/assign_taxonomy_blast.sh
+-rw-r--r--   0        0        0      578 2021-05-16 19:09:45.143536 micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/assign_taxonomy_naivebayes.sh
+-rw-r--r--   0        0        0      150 2021-03-19 21:03:45.874738 micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/import_reads.sh
+-rw-r--r--   0        0        0      429 2021-03-19 21:04:31.741405 micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/import_references.sh
+-rw-r--r--   0        0        0      721 2021-03-19 21:05:07.628072 micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/train_classifier.sh
+-rw-r--r--   0        0        0       39 2020-12-17 21:32:30.061644 micone-0.9.0/micone/setup/__init__.py
+-rw-r--r--   0        0        0     3682 2021-10-06 19:10:16.436840 micone-0.9.0/micone/setup/environments.py
+-rw-r--r--   0        0        0       29 2020-12-17 21:32:30.058311 micone-0.9.0/micone/utils/__init__.py
+-rw-r--r--   0        0        0     1828 2021-01-21 14:19:56.758060 micone-0.9.0/micone/utils/spinner.py
+-rw-r--r--   0        0        0      323 2020-12-17 21:32:30.114977 micone-0.9.0/micone/validation/__init__.py
+-rw-r--r--   0        0        0     6495 2020-12-17 21:32:30.114977 micone-0.9.0/micone/validation/network_schema.py
+-rw-r--r--   0        0        0     8041 2021-01-25 21:08:54.335553 micone-0.9.0/micone/validation/otu_schema.py
+-rw-r--r--   0        0        0     7159 2020-12-17 21:32:30.114977 micone-0.9.0/micone/validation/otu_validator.py
+-rw-r--r--   0        0        0     1504 2021-10-30 15:08:40.333916 micone-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8832 2021-10-30 15:10:19.859134 micone-0.9.0/setup.py
+-rw-r--r--   0        0        0     6412 2021-10-30 15:10:19.859964 micone-0.9.0/PKG-INFO
```

### Comparing `micone-0.8.1/LICENSE` & `micone-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/README.md` & `micone-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/cli.py` & `micone-0.9.0/micone/cli.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/config/config.py` & `micone-0.9.0/micone/config/config.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/config/datatypes.py` & `micone-0.9.0/micone/config/datatypes.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/config/params.py` & `micone-0.9.0/micone/config/params.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/conversion/network_converter.py` & `micone-0.9.0/micone/conversion/network_converter.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/conversion/taxmetadata_converter.py` & `micone-0.9.0/micone/conversion/taxmetadata_converter.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/logging/logger.py` & `micone-0.9.0/micone/logging/logger.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/main/lineage.py` & `micone-0.9.0/micone/main/lineage.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/main/network.py` & `micone-0.9.0/micone/main/network.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/main/network_group.py` & `micone-0.9.0/micone/main/network_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
                         pvalue_filter=pvalue_filter,
                         interaction_filter=interaction_filter,
                     )
                 )
         else:
             for cid, network in enumerate(self._networks):
                 path = pathlib.Path(fpath)
-                fname = f"{path.parent}/{path.stem}_{cid}{path.suffix}"
+                fname = f"{path.parent}/{cid}_{path.stem}{path.suffix}"
                 network.write(
                     fname,
                     pvalue_filter=pvalue_filter,
                     interaction_filter=interaction_filter,
                 )
 
     @classmethod
```

### Comparing `micone-0.8.1/micone/main/otu.py` & `micone-0.9.0/micone/main/otu.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/command.py` & `micone-0.9.0/micone/pipelines/command.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/configs/denoise_cluster.config` & `micone-0.9.0/micone/pipelines/configs/denoise_cluster.config`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,37 @@
 // -*- mode: groovy -*-
 
 params {
     denoise_cluster {
-        sequence_processing {
-            // Demultiplexing illumina workflow
-            'demultiplexing_illumina' {
-                rev_comp_barcodes = "False"
-                rev_comp_mapping_barcodes = "False"
-            }
-            // 'join_reads' {}
-            // Trim filter fixed workflow
-            'export_visualization' {
-                seq_samplesize = 10000
-            }
-            'trimming' {
-                ncpus = 1
-                max_ee = 2
-                trunc_q = 2
-            }
-            // TODO: Demultiplexing 454 workflow
-        }
         otu_assignment {
             selection = [
                 "closed_reference",
                 "open_reference",
                 "de_novo",
                 "dada2",
                 "deblur"
             ]
             // Closed reference workflow
             'closed_reference' {
                 ncpus = 1
-                parameters = "nf_micone/data/qiime1_parameters.txt"
-                reference_sequences = "nf_micone/data/rep_set/97_otus.fasta"
+                percent_identity = 0.97
+                strand = "plus"
+                reference_sequences = ["${PWD}/nf_micone/data/databases/greengenes/gg_97/refseqs.qza"]
             }
             // Open reference workflow
             'open_reference' {
                 ncpus = 1
-                parameters = "nf_micone/data/qiime1_parameters.txt"
-                reference_sequences = "nf_micone/data/rep_set/97_otus.fasta"
-                picking_method = "uclust"
+                percent_identity = 0.97
+                strand = "plus"
+                reference_sequences = ["${PWD}/nf_micone/data/databases/greengenes/gg_97/refseqs.qza"]
             }
             // De novo workflow
             'de_novo' {
                 ncpus = 1
-                parameters = "nf_micone/data/qiime1_parameters.txt"
+                percent_identity = 0.97
             }
             // Dada2 workflow
             'dada2' {
                 ncpus = 1
                 big_data = "FALSE"
             }
             // Deblur workflow
```

### Comparing `micone-0.8.1/micone/pipelines/configs/network_inference.config` & `micone-0.9.0/micone/pipelines/configs/network_inference.config`

 * *Files 14% similar despite different names*

```diff
@@ -47,20 +47,18 @@
                 max_iteration = 1500
             }
         }
         network {
             'make_network_with_pvalue' {
                 interaction_threshold = 0.3
                 pvalue_threshold = 0.05
-                // FIXME: This should ideally be passed through the sample_sheet
                 metadata_file = ""
             }
             'make_network_without_pvalue' {
                 interaction_threshold = 0.3
-                // FIXME: This should ideally be passed through the sample_sheet
                 metadata_file = ""
             }
             // 'merge_pvalues' {}
             'create_consensus' {
                 method = 'scaled_sum'
                 parameter = 0.3
                 pvalue_filter = "true"
```

### Comparing `micone-0.8.1/micone/pipelines/configs/otu_processing.config` & `micone-0.9.0/micone/pipelines/configs/otu_processing.config`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 params {
     otu_processing {
         // export {
         //     'biom2tsv' {}
         // }
         transform {
+            'fork' {
+                axis = "sample"
+                column = ""
+            }
             'group' {
                 tax_levels = ['Phylum', 'Class', 'Order', 'Family', 'Genus', 'Species']
             }
-            // NOTE: Set to "False" to disable filtering
+            // NOTE: Set to false to disable filtering
             // NOTE: Set axis to "None" to disable normalization
             'normalize' {
                 axis = "sample"
                 count_thres = 500
                 prevalence_thres = 0.05
                 abundance_thres = 0.01
-                rm_sparse_obs = "True"
-                rm_sparse_samples = "True"
+                rm_sparse_obs = true
+                rm_sparse_samples = true
             }
         }
     }
 }
```

### Comparing `micone-0.8.1/micone/pipelines/configs/process.config` & `micone-0.9.0/micone/pipelines/configs/process.config`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/configs/profiles.config` & `micone-0.9.0/micone/pipelines/configs/profiles.config`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/configs/tax_assignment.config` & `micone-0.9.0/micone/pipelines/configs/tax_assignment.config`

 * *Files 25% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 params {
     tax_assignment {
         assign {
             selection = ['naive_bayes', 'blast']
             // NOTE: The classifiers for naive_bayes are .qza files
             'naive_bayes' {
-                classifier = "${PWD}/nf_micone/data/classifiers/gg-13-8-99-515-806-nb-classifier.qza"
+                classifier = ["${PWD}/nf_micone/data/classifiers/gg_13_8_99_515_806.qza"]
                 confidence = 0.7
                 ncpus = 1
             }
-            // NOTE: The references and tax_map for blast are .qza files
+            // NOTE: 1. The references and tax_map for blast are .qza files
+            //       2. The references must be a folder containing "refseqs.qza" and "taxonomy.qza"
             'blast' {
-                reference_sequences = ""
-                tax_map = ""
+                references = ["${PWD}/nf_micone/data/databases/ncbi/ncbi"]
                 max_accepts = 10
                 perc_identity = 0.8
                 evalue = 0.001
                 min_consensus = 0.51
             }
         }
     }
```

### Comparing `micone-0.8.1/micone/pipelines/envs/micone-flashweave/post_install.sh` & `micone-0.9.0/micone/pipelines/envs/micone-flashweave/post_install.sh`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/envs/micone-qiime2/env.yml` & `micone-0.9.0/micone/pipelines/envs/micone-qiime2/env.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,432 +1,430 @@
 channels:
-  - qiime2/label/r2020.11
+  - qiime2/label/r2021.8
   - conda-forge
   - bioconda
   - defaults
 dependencies:
   - _libgcc_mutex=0.1
   - _openmp_mutex=4.5
   - _r-mutex=1.0.1
   - alsa-lib=1.2.3
-  - arb-bio-tools=6.0.6
+  - argcomplete=1.12.3
   - argon2-cffi=20.1.0
   - async_generator=1.10
-  - attrs=20.3.0
+  - attrs=21.2.0
   - backcall=0.2.0
   - backports=1.0
-  - backports.functools_lru_cache=1.6.1
+  - backports.functools_lru_cache=1.6.4
   - bibtexparser=1.1.0
-  - binutils_impl_linux-64=2.35.1
-  - binutils_linux-64=2.35
+  - binutils_impl_linux-64=2.36.1
+  - binutils_linux-64=2.36
   - bioconductor-biobase=2.50.0
   - bioconductor-biocgenerics=0.36.0
-  - bioconductor-biocparallel=1.24.0
+  - bioconductor-biocparallel=1.24.1
   - bioconductor-biostrings=2.58.0
   - bioconductor-dada2=1.18.0
-  - bioconductor-delayedarray=0.16.0
-  - bioconductor-genomeinfodb=1.26.0
+  - bioconductor-delayedarray=0.16.3
+  - bioconductor-genomeinfodb=1.26.4
   - bioconductor-genomeinfodbdata=1.2.4
   - bioconductor-genomicalignments=1.26.0
   - bioconductor-genomicranges=1.42.0
-  - bioconductor-iranges=2.24.0
-  - bioconductor-matrixgenerics=1.2.0
+  - bioconductor-iranges=2.24.1
+  - bioconductor-matrixgenerics=1.2.1
   - bioconductor-rhtslib=1.22.0
   - bioconductor-rsamtools=2.6.0
-  - bioconductor-s4vectors=0.28.0
+  - bioconductor-s4vectors=0.28.1
   - bioconductor-shortread=1.48.0
   - bioconductor-summarizedexperiment=1.20.0
   - bioconductor-xvector=0.30.0
   - bioconductor-zlibbioc=1.36.0
   - biom-format=2.1.10
-  - blas=2.17
-  - blast=2.10.1
-  - bleach=3.2.1
-  - bokeh=2.2.3
-  - boost-cpp=1.70.0
+  - blast=2.12.0
+  - bleach=4.1.0
+  - bokeh=2.3.3
   - bowtie2=2.4.2
   - brotlipy=0.7.0
   - bwidget=1.9.14
   - bzip2=1.0.8
-  - c-ares=1.17.1
-  - ca-certificates=2020.12.5
+  - c-ares=1.17.2
+  - ca-certificates=2021.5.30
   - cachecontrol=0.12.6
+  - cached-property=1.5.2
+  - cached_property=1.5.2
   - cairo=1.16.0
-  - certifi=2020.12.5
-  - cffi=1.14.4
-  - chardet=3.0.4
+  - certifi=2021.5.30
+  - cffi=1.14.6
+  - chardet=4.0.0
   - click=7.1.2
-  - cryptography=3.3.1
-  - curl=7.71.1
-  - cutadapt=3.1
+  - cryptography=3.4.7
+  - curl=7.78.0
+  - cutadapt=3.4
   - cycler=0.10.0
-  - cython=0.29.21
+  - cython=0.29.24
+  - dbus=1.13.6
   - deblur=1.1.0
+  - debugpy=1.4.1
   - decorator=4.4.2
-  - defusedxml=0.6.0
-  - dendropy=4.5.1
-  - dnaio=0.4.4
-  - emperor=1.0.1
-  - entrez-direct=13.9
+  - defusedxml=0.7.1
+  - dendropy=4.5.2
+  - dill=0.3.4
+  - dnaio=0.5.2
+  - emperor=1.0.3
+  - entrez-direct=15.6
   - entrypoints=0.3
-  - expat=2.2.9
+  - expat=2.4.1
   - fastcluster=1.1.26
   - fasttree=2.1.10
+  - font-ttf-dejavu-sans-mono=2.37
+  - font-ttf-inconsolata=3.000
+  - font-ttf-source-code-pro=2.038
+  - font-ttf-ubuntu=0.83
   - fontconfig=2.13.1
+  - fonts-conda-ecosystem=1
+  - fonts-conda-forge=1
   - freetype=2.10.4
   - fribidi=1.0.10
   - future=0.18.2
-  - gcc_impl_linux-64=7.5.0
-  - gcc_linux-64=7.5.0
+  - gcc_impl_linux-64=9.4.0
+  - gcc_linux-64=9.4.0
   - gettext=0.19.8.1
-  - gfortran_impl_linux-64=7.5.0
-  - gfortran_linux-64=7.5.0
+  - gfortran_impl_linux-64=9.4.0
+  - gfortran_linux-64=9.4.0
   - giflib=5.2.1
-  - glib=2.66.3
+  - glib=2.68.4
+  - glib-tools=2.68.4
   - gneiss=0.4.6
   - graphite2=1.3.13
-  - gsl=2.6
-  - gxx_impl_linux-64=7.5.0
-  - gxx_linux-64=7.5.0
-  - h5py=2.10.0
-  - harfbuzz=2.7.2
-  - hdf5=1.10.5
-  - hdmedians=0.14.1
+  - gsl=2.7
+  - gst-plugins-base=1.18.5
+  - gstreamer=1.18.5
+  - gxx_impl_linux-64=9.4.0
+  - gxx_linux-64=9.4.0
+  - h5py=3.3.0
+  - harfbuzz=2.9.1
+  - hdf5=1.10.6
+  - hdmedians=0.14.2
   - hmmer=3.1b2
-  - htslib=1.11
-  - icu=67.1
+  - htslib=1.13
+  - icu=68.1
   - idna=2.10
   - ijson=3.1.3
-  - importlib-metadata=3.1.1
-  - importlib_metadata=3.1.1
+  - importlib-metadata=4.8.1
+  - importlib_metadata=4.8.1
   - iniconfig=1.1.1
-  - ipykernel=5.3.4
-  - ipython=7.16.1
+  - ipykernel=6.4.0
+  - ipython=7.27.0
   - ipython_genutils=0.2.0
-  - ipywidgets=7.5.1
-  - iqtree=2.0.3
+  - ipywidgets=7.6.4
+  - iqtree=2.1.4_beta
   - isa-l=2.30.0
-  - jedi=0.17.2
-  - jinja2=2.11.2
-  - joblib=0.17.0
+  - jbig=2.1
+  - jedi=0.18.0
+  - jinja2=3.0.1
+  - joblib=1.0.1
   - jpeg=9d
+  - jq=1.6
   - jsonschema=3.2.0
-  - jupyter_client=6.1.7
-  - jupyter_core=4.7.0
+  - jupyter_client=7.0.2
+  - jupyter_core=4.7.1
   - jupyterlab_pygments=0.1.2
+  - jupyterlab_widgets=1.0.1
   - kernel-headers_linux-64=2.6.32
-  - kiwisolver=1.3.1
-  - krb5=1.17.2
-  - lcms2=2.11
-  - ld_impl_linux-64=2.35.1
-  - libarbdb=6.0.6
-  - libblas=3.8.0
-  - libcblas=3.8.0
-  - libcurl=7.71.1
-  - libdeflate=1.6
+  - kiwisolver=1.3.2
+  - krb5=1.19.2
+  - lcms2=2.12
+  - ld_impl_linux-64=2.36.1
+  - lerc=2.2.1
+  - libblas=3.9.0
+  - libcblas=3.9.0
+  - libclang=11.1.0
+  - libcurl=7.78.0
+  - libdeflate=1.7
   - libedit=3.1.20191231
   - libev=4.33
+  - libevent=2.1.10
   - libffi=3.3
   - libgcc=7.2.0
-  - libgcc-ng=9.3.0
-  - libgfortran-ng=7.5.0
-  - libgfortran4=7.5.0
-  - libglib=2.66.3
-  - libgomp=9.3.0
+  - libgcc-devel_linux-64=9.4.0
+  - libgcc-ng=11.1.0
+  - libgfortran-ng=11.1.0
+  - libgfortran5=11.1.0
+  - libglib=2.68.4
+  - libgomp=11.1.0
   - libiconv=1.16
-  - liblapack=3.8.0
-  - liblapacke=3.8.0
-  - libnghttp2=1.41.0
-  - libopenblas=0.3.10
+  - liblapack=3.9.0
+  - libllvm11=11.1.0
+  - libnghttp2=1.43.0
+  - libogg=1.3.4
+  - libopenblas=0.3.17
+  - libopus=1.3.1
   - libpng=1.6.37
+  - libpq=13.3
+  - libsanitizer=9.4.0
   - libsodium=1.0.18
-  - libssh2=1.9.0
-  - libstdcxx-ng=9.3.0
-  - libtiff=4.1.0
+  - libssh2=1.10.0
+  - libstdcxx-devel_linux-64=9.4.0
+  - libstdcxx-ng=11.1.0
+  - libtiff=4.3.0
   - libuuid=2.32.1
-  - libwebp-base=1.1.0
+  - libuv=1.42.0
+  - libvorbis=1.3.7
+  - libwebp-base=1.2.1
   - libxcb=1.13
-  - libxml2=2.9.10
-  - llvm-openmp=11.0.0
+  - libxkbcommon=1.0.3
+  - libxml2=2.9.12
+  - libxslt=1.1.33
   - lockfile=0.12.2
-  - lz4=3.1.1
-  - lz4-c=1.9.2
-  - mafft=7.475
+  - lxml=4.6.3
+  - lz4=3.1.3
+  - lz4-c=1.9.3
+  - mafft=7.487
   - make=4.3
-  - markupsafe=1.1.1
-  - matplotlib=3.2.2
-  - matplotlib-base=3.2.2
+  - markupsafe=2.0.1
+  - matplotlib=3.4.3
+  - matplotlib-base=3.4.3
+  - matplotlib-inline=0.1.3
   - mistune=0.8.4
-  - more-itertools=8.6.0
-  - msgpack-python=1.0.0
-  - natsort=7.1.0
-  - nbclient=0.5.1
-  - nbconvert=6.0.7
-  - nbformat=5.0.8
+  - more-itertools=8.9.0
+  - msgpack-python=1.0.2
+  - mysql-common=8.0.25
+  - mysql-libs=8.0.25
+  - natsort=7.1.1
+  - nbclient=0.5.4
+  - nbconvert=6.1.0
+  - nbformat=5.1.3
   - ncurses=6.2
-  - nest-asyncio=1.4.3
-  - networkx=2.5
+  - nest-asyncio=1.5.1
+  - networkx=2.6.2
+  - nodejs=16.6.1
   - nose=1.3.7
-  - notebook=6.1.5
-  - numpy=1.19.4
+  - notebook=6.4.3
+  - nspr=4.30
+  - nss=3.69
+  - numpy=1.21.2
   - olefile=0.46
-  - openjdk=11.0.8
-  - openssl=1.1.1h
-  - packaging=20.7
-  - pandas=1.1.5
-  - pandoc=2.11.2
+  - oniguruma=6.9.7.1
+  - openjdk=11.0.9.1
+  - openjpeg=2.4.0
+  - openssl=1.1.1l
+  - packaging=21.0
+  - pandas=1.2.5
+  - pandoc=2.14.2
   - pandocfilters=1.4.2
-  - pango=1.42.4
-  - parso=0.7.1
+  - pango=1.48.9
+  - parso=0.8.2
   - patsy=0.5.1
-  - pcre=8.44
-  - pcre2=10.35
+  - pcre=8.45
+  - pcre2=10.37
   - perl=5.26.2
-  - perl-app-cpanminus=1.7044
   - perl-archive-tar=2.32
-  - perl-base=2.23
-  - perl-business-isbn=3.004
-  - perl-business-isbn-data=20140910.003
   - perl-carp=1.38
   - perl-common-sense=3.74
   - perl-compress-raw-bzip2=2.087
   - perl-compress-raw-zlib=2.087
-  - perl-constant=1.33
-  - perl-data-dumper=2.173
-  - perl-digest-hmac=1.03
-  - perl-digest-md5=2.55
-  - perl-encode=2.88
-  - perl-encode-locale=1.05
   - perl-exporter=5.72
   - perl-exporter-tiny=1.002001
   - perl-extutils-makemaker=7.36
-  - perl-file-listing=6.04
-  - perl-file-path=2.16
-  - perl-file-temp=0.2304
-  - perl-html-parser=3.72
-  - perl-html-tagset=3.20
-  - perl-html-tree=5.07
-  - perl-http-cookies=6.04
-  - perl-http-daemon=6.01
-  - perl-http-date=6.02
-  - perl-http-message=6.18
-  - perl-http-negotiate=6.01
   - perl-io-compress=2.087
-  - perl-io-html=1.001
-  - perl-io-socket-ssl=2.066
   - perl-io-zlib=1.10
   - perl-json=4.02
   - perl-json-xs=2.34
-  - perl-libwww-perl=6.39
   - perl-list-moreutils=0.428
   - perl-list-moreutils-xs=0.428
-  - perl-lwp-mediatypes=6.04
-  - perl-lwp-protocol-https=6.07
-  - perl-mime-base64=3.15
-  - perl-mozilla-ca=20180117
-  - perl-net-http=6.19
-  - perl-net-ssleay=1.88
-  - perl-ntlm=1.09
-  - perl-parent=0.236
   - perl-pathtools=3.75
   - perl-scalar-list-utils=1.52
-  - perl-socket=2.027
-  - perl-storable=3.15
-  - perl-test-requiresinternet=0.05
-  - perl-time-local=1.28
-  - perl-try-tiny=0.30
   - perl-types-serialiser=1.0
-  - perl-uri=1.76
-  - perl-www-robotrules=6.02
-  - perl-xml-namespacesupport=1.12
-  - perl-xml-parser=2.44_01
-  - perl-xml-sax=1.02
-  - perl-xml-sax-base=1.09
-  - perl-xml-sax-expat=0.51
-  - perl-xml-simple=2.25
   - perl-xsloader=0.24
   - pexpect=4.8.0
   - pickleshare=0.7.5
-  - pigz=2.3.4
-  - pillow=8.0.1
-  - pip=20.3.1
+  - pigz=2.6
+  - pillow=8.3.2
+  - pip=21.2.4
   - pixman=0.40.0
   - pluggy=0.13.1
-  - prometheus_client=0.9.0
-  - prompt-toolkit=3.0.8
-  - psutil=5.7.3
+  - prometheus_client=0.11.0
+  - prompt-toolkit=3.0.20
+  - psutil=5.8.0
   - pthread-stubs=0.4
-  - ptyprocess=0.6.0
-  - py=1.9.0
+  - ptyprocess=0.7.0
+  - py=1.10.0
   - pycparser=2.20
-  - pygments=2.7.3
-  - pyopenssl=20.0.0
+  - pygments=2.10.0
+  - pyopenssl=20.0.1
   - pyparsing=2.4.7
+  - pyqt=5.12.3
+  - pyqt-impl=5.12.3
+  - pyqt5-sip=4.19.18
+  - pyqtchart=5.12
+  - pyqtwebengine=5.12.1
   - pyrsistent=0.17.3
   - pysocks=1.7.1
-  - pytest=6.1.2
-  - python=3.6.12
-  - python-dateutil=2.8.1
-  - python_abi=3.6
-  - pytz=2020.4
-  - pyyaml=5.3.1
-  - pyzmq=20.0.0
-  - q2-alignment=2020.11.1
-  - q2-composition=2020.11.1
-  - q2-cutadapt=2020.11.1
-  - q2-dada2=2020.11.1
-  - q2-deblur=2020.11.1
-  - q2-demux=2020.11.1
-  - q2-diversity=2020.11.1
-  - q2-diversity-lib=2020.11.1
-  - q2-emperor=2020.11.1
-  - q2-feature-classifier=2020.11.1
-  - q2-feature-table=2020.11.1
-  - q2-fragment-insertion=2020.11.1
-  - q2-gneiss=2020.11.1
-  - q2-longitudinal=2020.11.1
-  - q2-metadata=2020.11.1
-  - q2-phylogeny=2020.11.1
-  - q2-quality-control=2020.11.1
-  - q2-quality-filter=2020.11.1
-  - q2-sample-classifier=2020.11.1
-  - q2-taxa=2020.11.1
-  - q2-types=2020.11.1
-  - q2-vsearch=2020.11.1
-  - q2cli=2020.11.1
-  - q2templates=2020.11.1
-  - qiime2=2020.11.1
+  - pytest=6.2.5
+  - python=3.8.10
+  - python-dateutil=2.8.2
+  - python-isal=0.11.1
+  - python_abi=3.8
+  - pytz=2021.1
+  - pyyaml=5.4.1
+  - pyzmq=22.2.1
+  - q2-alignment=2021.8.0
+  - q2-composition=2021.8.0
+  - q2-cutadapt=2021.8.0
+  - q2-dada2=2021.8.0
+  - q2-deblur=2021.8.0
+  - q2-demux=2021.8.0
+  - q2-diversity=2021.8.0
+  - q2-diversity-lib=2021.8.0
+  - q2-emperor=2021.8.0
+  - q2-feature-classifier=2021.8.0
+  - q2-feature-table=2021.8.0
+  - q2-fragment-insertion=2021.8.0
+  - q2-gneiss=2021.8.0
+  - q2-longitudinal=2021.8.0
+  - q2-metadata=2021.8.0
+  - q2-mystery-stew=2021.8.0
+  - q2-phylogeny=2021.8.0
+  - q2-quality-control=2021.8.0
+  - q2-quality-filter=2021.8.0
+  - q2-sample-classifier=2021.8.0
+  - q2-taxa=2021.8.0
+  - q2-types=2021.8.0
+  - q2-vsearch=2021.8.0
+  - q2cli=2021.8.0
+  - q2galaxy=2021.8.0
+  - q2templates=2021.8.0
+  - qiime2=2021.8.0
+  - qt=5.12.9
   - r-assertthat=0.2.1
   - r-backports=1.2.1
-  - r-base=4.0.2
-  - r-bh=1.72.0_3
-  - r-bitops=1.0_6
-  - r-brio=1.1.0
-  - r-callr=3.5.1
-  - r-cli=2.2.0
-  - r-cluster=2.1.0
-  - r-colorspace=2.0_0
-  - r-crayon=1.3.4
-  - r-desc=1.2.0
-  - r-diffobj=0.3.2
+  - r-base=4.0.5
+  - r-bh=1.75.0_0
+  - r-bitops=1.0_7
+  - r-brio=1.1.2
+  - r-callr=3.7.0
+  - r-cli=3.0.1
+  - r-cluster=2.1.2
+  - r-colorspace=2.0_2
+  - r-crayon=1.4.1
+  - r-desc=1.3.0
+  - r-diffobj=0.3.4
   - r-digest=0.6.27
-  - r-ellipsis=0.3.1
+  - r-ellipsis=0.3.2
   - r-evaluate=0.14
-  - r-fansi=0.4.1
-  - r-farver=2.0.3
-  - r-formatr=1.7
+  - r-fansi=0.5.0
+  - r-farver=2.1.0
+  - r-formatr=1.11
   - r-futile.logger=1.4.3
   - r-futile.options=1.0.1
-  - r-ggplot2=3.3.2
+  - r-ggplot2=3.3.5
   - r-glue=1.4.2
   - r-gtable=0.3.0
   - r-hwriter=1.3.2
-  - r-isoband=0.2.3
+  - r-isoband=0.2.5
   - r-jpeg=0.1_8.1
   - r-jsonlite=1.7.2
   - r-labeling=0.4.2
   - r-lambda.r=1.2.4
-  - r-lattice=0.20_41
+  - r-lattice=0.20_44
   - r-latticeextra=0.6_29
-  - r-lifecycle=0.2.0
+  - r-lifecycle=1.0.0
   - r-magrittr=2.0.1
-  - r-mass=7.3_53
-  - r-matrix=1.2_18
-  - r-matrixstats=0.57.0
-  - r-mgcv=1.8_33
+  - r-mass=7.3_54
+  - r-matrix=1.3_2
+  - r-matrixstats=0.60.1
+  - r-mgcv=1.8_36
   - r-munsell=0.5.0
-  - r-nlme=3.1_150
+  - r-nlme=3.1_153
   - r-permute=0.9_5
-  - r-pillar=1.4.7
-  - r-pkgbuild=1.1.0
+  - r-pillar=1.6.2
   - r-pkgconfig=2.0.3
-  - r-pkgload=1.1.0
+  - r-pkgload=1.2.1
   - r-plyr=1.8.6
   - r-png=0.1_7
   - r-praise=1.0.0
-  - r-prettyunits=1.1.1
-  - r-processx=3.4.5
-  - r-ps=1.5.0
-  - r-r6=2.5.0
+  - r-processx=3.5.2
+  - r-ps=1.6.0
+  - r-r6=2.5.1
   - r-rcolorbrewer=1.1_2
-  - r-rcpp=1.0.5
-  - r-rcppparallel=5.0.2
-  - r-rcurl=1.98_1.2
+  - r-rcpp=1.0.7
+  - r-rcppparallel=5.1.4
+  - r-rcurl=1.98_1.4
   - r-rematch2=2.1.2
   - r-reshape2=1.4.4
-  - r-rlang=0.4.9
+  - r-rlang=0.4.11
   - r-rprojroot=2.0.2
   - r-rstudioapi=0.13
   - r-scales=1.1.1
   - r-snow=0.4_3
-  - r-stringi=1.5.3
+  - r-stringi=1.7.4
   - r-stringr=1.4.0
-  - r-testthat=3.0.0
-  - r-tibble=3.0.4
-  - r-utf8=1.1.4
-  - r-vctrs=0.3.5
-  - r-vegan=2.5_6
-  - r-viridislite=0.3.0
-  - r-waldo=0.2.3
-  - r-withr=2.3.0
-  - r-zeallot=0.1.0
+  - r-testthat=3.0.4
+  - r-tibble=3.1.4
+  - r-utf8=1.2.2
+  - r-vctrs=0.3.8
+  - r-vegan=2.5_7
+  - r-viridislite=0.4.0
+  - r-waldo=0.3.0
+  - r-withr=2.4.2
   - raxml=8.2.12
-  - readline=8.0
-  - requests=2.25.0
-  - samtools=1.11
+  - readline=8.1
+  - requests=2.25.1
+  - samtools=1.13
   - scikit-bio=0.5.6
-  - scikit-learn=0.23.1
-  - scipy=1.5.3
-  - seaborn=0.11.0
-  - seaborn-base=0.11.0
+  - scikit-learn=0.24.1
+  - scipy=1.7.1
+  - seaborn=0.11.2
+  - seaborn-base=0.11.2
   - sed=4.8
-  - send2trash=1.5.0
+  - send2trash=1.8.0
   - sepp=4.3.10
-  - setuptools=49.6.0
-  - sina=1.7.1
-  - six=1.15.0
+  - setuptools=58.0.4
+  - six=1.16.0
   - sortmerna=2.0
-  - sqlite=3.34.0
-  - statsmodels=0.12.1
+  - sqlite=3.36.0
+  - statsmodels=0.12.2
   - sysroot_linux-64=2.12
   - tbb=2020.2
-  - terminado=0.9.1
-  - testpath=0.4.4
-  - threadpoolctl=2.1.0
-  - tk=8.6.10
+  - terminado=0.12.1
+  - testpath=0.5.0
+  - threadpoolctl=2.2.0
+  - tk=8.6.11
   - tktable=2.10
   - toml=0.10.2
   - tornado=6.1
-  - traitlets=4.3.3
-  - typing_extensions=3.7.4.3
+  - traitlets=5.1.0
+  - typing_extensions=3.10.0.0
   - tzlocal=2.1
-  - unifrac=0.20.1
-  - urllib3=1.25.11
+  - unifrac=0.20.2
+  - urllib3=1.26.6
   - vsearch=2.7.0
   - wcwidth=0.2.5
   - webencodings=0.5.1
-  - wheel=0.36.1
+  - wheel=0.37.0
   - widgetsnbextension=3.5.1
-  - xopen=1.0.1
+  - xmltodict=0.12.0
+  - xopen=1.1.0
   - xorg-fixesproto=5.0
   - xorg-inputproto=2.3.2
   - xorg-kbproto=1.0.7
   - xorg-libice=1.0.10
   - xorg-libsm=1.2.3
-  - xorg-libx11=1.6.12
+  - xorg-libx11=1.7.2
   - xorg-libxau=1.0.9
   - xorg-libxdmcp=1.1.3
   - xorg-libxext=1.3.4
   - xorg-libxfixes=5.0.3
   - xorg-libxi=1.7.10
   - xorg-libxrender=0.9.10
+  - xorg-libxt=1.2.1
   - xorg-libxtst=1.2.3
   - xorg-recordproto=1.14.2
   - xorg-renderproto=0.11.1
   - xorg-xextproto=7.3.0
   - xorg-xproto=7.0.31
   - xz=5.2.5
   - yaml=0.2.5
-  - zeromq=4.3.3
-  - zipp=3.4.0
+  - yq=2.12.2
+  - zeromq=4.3.4
+  - zipp=3.5.0
   - zlib=1.2.11
-  - zstd=1.4.5
+  - zstd=1.5.0
```

### Comparing `micone-0.8.1/micone/pipelines/functions/functions.nf` & `micone-0.9.0/micone/pipelines/functions/functions.nf`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 def updateMeta(Map args) {
     def Map meta = [:]
     meta.id                = args.id ?: ''
+    meta.run                = args.run ?: ''
     meta.single_end        = args.single_end ?: ''
     meta.strandedness      = args.strandedness ?: ''
     meta.denoise_cluster   = args.denoise_cluster ?: ''
     meta.chimera_checking  = args.chimera_checking ?: ''
     meta.tax_assignment    = args.tax_assignment ?: ''
     meta.tax_level         = args.tax_level ?: ''
     meta.network_inference = args.network_inference ?: ''
```

### Comparing `micone-0.8.1/micone/pipelines/main.nf` & `micone-0.9.0/micone/pipelines/main.nf`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 // -*- mode:groovy -*-
 // vim:ft=groovy
 
 nextflow.enable.dsl=2
 
 // Include workflows
+include { sequence_processing_single_workflow } from './nf_micone/modules/sequence_processing/sequence_processing_single_workflow.nf'
+include { sequence_processing_paired_workflow } from './nf_micone/modules/sequence_processing/sequence_processing_paired_workflow.nf'
 include { denoise_cluster_workflow } from './nf_micone/modules/denoise_cluster/denoise_cluster_workflow.nf'
 include { tax_assignment_workflow } from './nf_micone/modules/tax_assignment/tax_assignment_workflow.nf'
 include { otu_processing_workflow } from './nf_micone/modules/otu_processing/otu_processing_workflow.nf'
 include { network_inference_workflow } from './nf_micone/modules/network_inference/network_inference_workflow.nf'
 
 // Include data ingestion functions
-include { dc_data_ingestion } from './nf_micone/modules/utils/dc_data_ingestion.nf'
+include { spp_data_ingestion } from './nf_micone/modules/utils/spp_data_ingestion.nf'
+include { sps_data_ingestion } from './nf_micone/modules/utils/sps_data_ingestion.nf'
 
 // Channels for samplesheets
 Channel
     .fromPath(params.input)
     .set { input_channel }
 
 workflow {
+    ingestion = params.paired_end ? spp_data_ingestion : sps_data_ingestion
+    sequence_processing_workflow = params.paired_end ? sequence_processing_paired_workflow : sequence_processing_single_workflow
     input_channel \
-        | dc_data_ingestion \
+        | ingestion \
+        | sequence_processing_workflow \
         | denoise_cluster_workflow \
         | tax_assignment_workflow \
         | otu_processing_workflow \
         | network_inference_workflow
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/export_files.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/export_files.nf`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 process export_files {
     label 'qiime2'
     tag "${meta.id}"
     publishDir "${params.output_dir}/${f[0]}/${f[1]}/filtered_output/${meta.denoise_cluster}/${meta.id}",
         mode: 'copy',
         overwrite: true
     input:
-        tuple val(meta), file(otutable_nonchimeric), file(repseqs_nonchimeric)
+        tuple val(meta), file(otutable_nonchimeric), file(repseqs_nonchimeric), file(samplemetadata_files)
     output:
-        tuple val(meta), file("otu_table.biom"), file("rep_seqs.fasta")
+        tuple val(meta), file("otu_table.biom"), file("rep_seqs.fasta"), file(samplemetadata_files)
     script:
         String task_process = "${task.process}"
         f = getHierarchy(task_process)
         template 'denoise_cluster/chimera_checking/export_files.sh'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/remove_bimera.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/remove_bimera.nf`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 include { updateMeta } from '../../../functions/functions.nf'
 
 // Remove chimeras using removeBimeraDenovo
 process remove_bimera {
     label 'dada2'
     tag "${new_meta.id}"
     input:
-        tuple val(meta), file(seqtable_file)
+        tuple val(meta), file(seqtable_file), file(samplemetadata_files)
     when:
         "remove_bimera" in params.denoise_cluster.chimera_checking['selection']
     output:
-        tuple val(new_meta), file("unhashed_otu_table.biom"), file("unhashed_rep_seqs.fasta")
+        val(new_meta), emit: meta_channel
+        path('unhashed_otu_table.biom'), emit: otu_channel
+        path('unhashed_rep_seqs.fasta'), emit: repseq_channel
+        path(samplemetadata_files), emit: samplemetadata_channel
     script:
         new_meta = updateMeta(meta)
         new_meta.chimera_checking = 'remove_bimera'
         ncpus = params.denoise_cluster.chimera_checking['remove_bimera']['ncpus']
         chimera_method = params.denoise_cluster.chimera_checking['remove_bimera']['chimera_method']
         template 'denoise_cluster/chimera_checking/remove_chimeras.R'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/remove_bimera_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/remove_bimera_workflow.nf`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 include { create_seqtable } from './create_seqtable.nf'
 include { remove_bimera } from './remove_bimera.nf'
 include { hashing3 } from './../otu_assignment/hashing3.nf'
 
 
 workflow remove_bimera_workflow {
     take:
-        // tuple val(id), file(otutable_file), file(repseqs_file)
+        // tuple val(id), file(otutable_file), file(repseqs_file), file(samplemetadata_files)
         input_channel
     main:
         input_channel \
             | create_seqtable \
             | remove_bimera \
             | hashing3
     emit:
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/uchime.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/uchime.nf`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 include { updateMeta } from '../../../functions/functions.nf'
 
 // Remove chimeras using vserach uchime-denovo
 process uchime {
     label 'qiime2'
     tag "${new_meta.id}"
     input:
-        tuple val(meta), file(otutable_artifact), file(repseqs_artifact)
+        tuple val(meta), file(otutable_artifact), file(repseqs_artifact), file(samplemetadata_files)
     when:
         "uchime" in params.denoise_cluster.chimera_checking['selection']
     output:
-        tuple val(new_meta), file("otu_table_nonchimeric.qza"), file("rep_seqs_nonchimeric.qza")
+        tuple val(new_meta), file("otu_table_nonchimeric.qza"), file("rep_seqs_nonchimeric.qza"), file(samplemetadata_files)
     script:
         new_meta = updateMeta(meta)
         new_meta.chimera_checking = 'uchime'
         template 'denoise_cluster/chimera_checking/remove_chimeras.sh'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/chimera_checking/uchime_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/chimera_checking/uchime_workflow.nf`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 include { import_files } from './import_files.nf'
 include { uchime } from './uchime.nf'
 include { export_files } from './export_files.nf'
 
 
 workflow uchime_workflow {
     take:
-        // tuple val(id), file(otutable_file), file(repseqs_file)
+        // tuple val(id), file(otutable_file), file(repseqs_file), file(samplemetadata_files)
         input_channel
     main:
         input_channel \
             | import_files \
             | uchime \
             | export_files
     emit:
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/denoise_cluster_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/denoise_cluster_workflow.nf`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 // Main variables to be defined
 // NOTE: These should be defined before any include statements
 
-
-// Sequencing processing imports
-include { demultiplexing_illumina_workflow } from './sequence_processing/demultiplexing_illumina_workflow.nf'
-include { trim_filter_workflow } from './sequence_processing/trim_filter_workflow.nf'
-
 // Denoising clustering imports
 include { closed_reference_workflow } from './otu_assignment/closed_reference_workflow.nf'
 include { dada2_workflow } from './otu_assignment/dada2_workflow.nf'
 include { deblur_workflow } from './otu_assignment/deblur_workflow.nf'
 include { de_novo_workflow } from './otu_assignment/de_novo_workflow.nf'
 include { open_reference_workflow } from './otu_assignment/open_reference_workflow.nf'
 
@@ -17,26 +12,19 @@
 include { uchime_workflow } from './chimera_checking/uchime_workflow.nf'
 include { remove_bimera_workflow } from './chimera_checking/remove_bimera_workflow.nf'
 
 
 // Main workflow
 workflow denoise_cluster_workflow {
     take:
-        // tuple val(meta), file(sequence_files), file(barcode_files), file(mapping_files)
+        // tuple val(meta), file('trimmed/*.fastq.gz'), file('trimmed/MANIFEST'), file(sequence_metadata), file(samplemetadata_files)
         input_channel
-        // tuple val(meta), file(samplemetadata_files)
-        samplemetadata_channel
     main:
         input_channel \
-            | demultiplexing_illumina_workflow \
-            | trim_filter_workflow \
             | (dada2_workflow & deblur_workflow & open_reference_workflow & de_novo_workflow & closed_reference_workflow) \
             | mix \
             | (uchime_workflow & remove_bimera_workflow)
         output_channel = uchime_workflow.out.mix(remove_bimera_workflow.out)
-        crossed_channel = samplemetadata_channel
-            .cross(output_channel) { it -> it[0].id }
-            .map { it -> [it[1], it[0][1]].flatten() }
     emit:
         // tuple val(meta), file('otu_table.biom'), file('rep_seqs.fasta'), file(samplemetadata_files)
-        crossed_channel
+        output_channel
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/closed_reference.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/closed_reference.nf`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 include { updateMeta } from '../../../functions/functions.nf'
 
 // Step2: Closed reference OTU picking
 process closed_reference {
-    label 'qiime1'
-    tag "${new_meta.id}"
+    label 'qiime2'
+    tag "${new_meta.id}-${new_meta.run}:${ref_seq_id}"
     input:
-        tuple val(meta), file(fasta_file)
+        tuple val(meta), file(fasta_file), file(samplemetadata_files)
+        each reference_sequences
     output:
-        tuple val(new_meta), file('unhashed_otu_table.biom'), file('unhashed_rep_seqs.fasta'), file('log*.txt')
+        val(new_meta), emit: meta_channel
+        path('*_unhashed_otu_table.biom'), emit: otu_channel
+        path('*_unhashed_rep_seqs.fasta'), emit: repseq_channel
+        path('*_sample_metadata.tsv'), emit: samplemetadata_channel
     when:
         "closed_reference" in params.denoise_cluster.otu_assignment['selection']
     script:
         new_meta = updateMeta(meta)
-        new_meta.denoise_cluster = 'closed_reference'
+        ref_seq_id = "${file(reference_sequences).parent.simpleName}"
+        new_meta.denoise_cluster = "closed_reference(${ref_seq_id})"
+        percent_identity = params.denoise_cluster.otu_assignment['closed_reference']['percent_identity']
         ncpus = params.denoise_cluster.otu_assignment['closed_reference']['ncpus']
-        parameters = params.denoise_cluster.otu_assignment['closed_reference']['parameters']
-        reference_sequences = params.denoise_cluster.otu_assignment['closed_reference']['reference_sequences']
-        parallel_option = ncpus > 1 ? "-a -O ${ncpus}" : ''
-        template 'denoise_cluster/otu_assignment/pick_closed_reference_otus.sh'
+        strand = params.denoise_cluster.otu_assignment['closed_reference']['strand']
+        template 'denoise_cluster/otu_assignment/cluster_closed_reference.sh'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/dada2.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/dada2_single.nf`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 include { updateMeta } from '../../../functions/functions.nf'
 
 // Denoise using dada2
-process dada2 {
+process dada2_single {
     label 'dada2'
-    tag "${new_meta.id}"
+    tag "${new_meta.id}-${new_meta.run}"
     input:
-        tuple val(meta), file(sequence_files), file(manifest_file)
+        tuple val(meta), file(sequence_files), file(manifest_file), file(sequence_metadata), file(samplemetadata_files)
     output:
-        tuple val(new_meta), file("seq_table.tsv")
+        tuple val(new_meta), file("seq_table.tsv"), file(samplemetadata_files)
     when:
         "dada2" in params.denoise_cluster.otu_assignment['selection']
     script:
         new_meta = updateMeta(meta)
         new_meta.denoise_cluster = 'dada2'
         ncpus = params.denoise_cluster.otu_assignment['dada2']['ncpus']
         big_data = params.denoise_cluster.otu_assignment['dada2']['big_data']
-        template 'denoise_cluster/otu_assignment/dada2.R'
+        template 'denoise_cluster/otu_assignment/dada2_single.R'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/de_novo.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/de_novo.nf`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 include { updateMeta } from '../../../functions/functions.nf'
 
 // Step2: de_novo OTU picking
 process de_novo {
-    label 'qiime1'
-    tag "${new_meta.id}"
+    label 'qiime2'
+    tag "${new_meta.id}-${new_meta.run}"
     input:
-        tuple val(meta), file(fasta_file)
+        tuple val(meta), file(fasta_file), file(samplemetadata_files)
     output:
-        tuple val(new_meta), file('unhashed_otu_table.biom'), file('unhashed_rep_seqs.fasta'), file('log*.txt')
+        val(new_meta), emit: meta_channel
+        path('*_unhashed_otu_table.biom'), emit: otu_channel
+        path('*_unhashed_rep_seqs.fasta'), emit: repseq_channel
+        path('*_sample_metadata.tsv'), emit: samplemetadata_channel
     when:
         "de_novo" in params.denoise_cluster.otu_assignment['selection']
     script:
         new_meta = updateMeta(meta)
         new_meta.denoise_cluster = 'de_novo'
+        percent_identity = params.denoise_cluster.otu_assignment['de_novo']['percent_identity']
         ncpus = params.denoise_cluster.otu_assignment['de_novo']['ncpus']
-        parameters = params.denoise_cluster.otu_assignment['de_novo']['parameters']
-        parallel_option = ncpus > 1 ? "-a -O ${ncpus}" : ''
-        template 'denoise_cluster/otu_assignment/pick_de_novo_otus.sh'
+        template 'denoise_cluster/otu_assignment/cluster_de_novo.sh'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/deblur.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/deblur.nf`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 include { updateMeta } from '../../../functions/functions.nf'
 
 // Step1: Denoise using deblur
 process deblur {
     label 'qiime2'
-    tag "${new_meta.id}"
+    tag "${new_meta.id}-${new_meta.run}"
     input:
-        tuple val(meta), file(sequence_files), file(manifest_file)
+        tuple val(meta), file(sequence_files), file(manifest_file), file(sequence_metadata), file(samplemetadata_files)
     output:
-        tuple val(new_meta), file('*_otu_table.biom'), file('*_rep_seqs.fasta')
+        val(new_meta), emit: meta_channel
+        path('*_unhashed_otu_table.biom'), emit: otu_channel
+        path('*_unhashed_rep_seqs.fasta'), emit: repseq_channel
+        path('*_sample_metadata.tsv'), emit: samplemetadata_channel
     when:
         "deblur" in params.denoise_cluster.otu_assignment['selection']
     script:
         new_meta = updateMeta(meta)
         new_meta.denoise_cluster = 'deblur'
         ncpus = params.denoise_cluster.otu_assignment['deblur']['ncpus']
         min_reads = params.denoise_cluster.otu_assignment['deblur']['min_reads']
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/hashing2.nf` & `micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/quality_analysis_single.nf`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 include { getHierarchy } from '../../../functions/functions.nf'
 
-// Step3: Replace the ids with the hashes of the sequences
-process hashing2 {
-    label 'qiime1'
-    tag "${meta.id}"
-    publishDir "${params.output_dir}/${f[0]}/${f[1]}/hashed_output/${meta.id}",
+// Identify positions on the front and the tail that need to be trimmed based on
+// a. quality and b. sequence retainment
+process quality_analysis_single {
+    label 'qiime2'
+    tag "${meta.id}-${meta.run}"
+    publishDir "${params.output_dir}/${f[0]}/${f[1]}/${f[2]}/${meta.id}-${meta.run}",
         mode: 'copy',
         overwrite: true
     input:
-        tuple val(meta), file(unhashed_otu_table), file(unhashed_rep_seqs), file(log)
+        tuple val(meta), file(qual_summary)
     output:
-        tuple val(meta), file('otu_table.biom'), file('rep_seqs.fasta')
+        tuple val(meta), file('trim.txt')
     script:
         String task_process = "${task.process}"
         f = getHierarchy(task_process)
-        template 'denoise_cluster/otu_assignment/hashing2.py'
+        template 'sequence_processing/trimming/quality_analysis_single.py'
 }
+
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/otu_assignment/hashing3.nf` & `micone-0.9.0/micone/pipelines/modules/denoise_cluster/otu_assignment/hashing3.nf`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 include { getHierarchy } from '../../../functions/functions.nf'
 
 // Step3: Replace the ids with hashes of the sequences
 process hashing3 {
     label 'dada2'
     tag "${meta.id}"
-    publishDir "${params.output_dir}/${f[0]}/${f[1]}/${directory}/${meta.id}",
+    publishDir "${params.output_dir}/${f[0]}/${module_dir}/${directory}/${meta.id}",
         mode: 'copy',
         overwrite: true
     input:
-        tuple val(meta), file(unhashed_otu_table), file(unhashed_rep_seqs)
+        val(meta)
+        path(unhashed_otu_table)
+        path(unhashed_rep_seqs)
+        path(samplemetadata_files)
     output:
-        tuple val(meta), file('otu_table.biom'), file('rep_seqs.fasta')
+        tuple val(meta), file('otu_table.biom'), file('rep_seqs.fasta'), file('sample_metadata.tsv')
     script:
         String task_process = "${task.process}"
         f = getHierarchy(task_process)
+        module_dir = f[1] == 'remove_bimera' ? 'remove_bimera' : "${meta.denoise_cluster}"
         directory = f[1] == 'remove_bimera' ? "filtered_output/${meta.denoise_cluster}" : 'hashed_output'
         template 'denoise_cluster/otu_assignment/hashing3.py'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/demultiplexing_illumina_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/sequence_processing/demultiplexing/demultiplexing_paired_workflow.nf`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-include { import_sequences } from './import_sequences_sh.nf'
-include { demultiplexing_illumina } from './demultiplexing_illumina.nf'
+include { import_sequences_paired } from './import_sequences_paired.nf'
+include { demultiplexing_illumina_paired } from './demultiplexing_illumina_paired.nf'
 include { export_sequences } from './export_sequences.nf'
 
 
-workflow demultiplexing_illumina_workflow {
+workflow demultiplexing_paired_workflow {
     take:
-        // tuple val(meta), file(sequence_file), file(barcode_file), file(mapping_file)
+        // tuple val(meta), file(forward_file), file(reverse_file), file(barcode_file), file(mapping_file)
         input_channel
     main:
         input_channel \
-            | import_sequences \
-            | demultiplexing_illumina \
-            // | join_reads \
+            | import_sequences_paired \
+            | demultiplexing_illumina_paired \
             | export_sequences
     emit:
         // export_sequences and join_reads has publishDir
-        // tuple val(meta), file('demux_seqs/*.fastq.gz'), file('demux_seqs/MANIFEST')
+        // tuple val(meta), file('demux_seqs/*.fastq.gz'), file('demux_seqs/MANIFEST'), file('demux_seqs/metadata.yml')
         export_sequences.out
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/export_sequences.nf` & `micone-0.9.0/micone/pipelines/modules/sequence_processing/demultiplexing/export_sequences.nf`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 include { getHierarchy } from '../../../functions/functions.nf'
 
 // Export the sequences and fix the manifest file
 process export_sequences {
     label 'qiime2'
-    tag "${meta.id}"
-    publishDir "${params.output_dir}/${f[0]}/${f[1]}/demultiplexed_sequences/${meta.id}",
+    tag "${meta.id}-${meta.run}"
+    publishDir "${params.output_dir}/${f[0]}/${f[1]}/demultiplexed_sequences/${meta.id}-${meta.run}",
         saveAs: { filename -> filename.split("/")[1] },
         mode: 'copy',
         overwrite: true
     input:
         tuple val(meta), file(demux_artifact)
     output:
-        tuple val(meta), file('demux_seqs/*.fastq.gz'), file('demux_seqs/MANIFEST')
+    tuple val(meta), file('demux_seqs/*.fastq.gz'), file('demux_seqs/MANIFEST'), file('demux_seqs/metadata.yml')
     script:
         String task_process = "${task.process}"
         f = getHierarchy(task_process)
-        template 'denoise_cluster/sequence_processing/export_sequences.py'
+        template 'sequence_processing/demultiplexing/export_sequences.sh'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/join_reads.nf` & `micone-0.9.0/micone/pipelines/modules/otu_processing/transform/fork.nf`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 include { getHierarchy } from '../../../functions/functions.nf'
 
-// Join reads
-process join_reads {
-    label 'qiime2'
+process fork {
+    label 'micone'
     tag "${meta.id}"
-    publishDir "${params.output_dir}/${f[0]}/${f[1]}/${f[2]}/${meta.id}",
+    publishDir "${params.output_dir}/${f[0]}/transform/${f[1]}/${directory}/${meta.id}",
+        saveAs: { filename -> filename.split("/")[1] },
         mode: 'copy',
         overwrite: true
     input:
-        tuple val(meta), file(demux_artifact)
+        tuple val(meta), file(otu_file)
     output:
-        tuple val(meta), file('*_joined.qza')
+        tuple val(meta), file("split/**.biom")
     script:
         String task_process = "${task.process}"
         f = getHierarchy(task_process)
-        template 'denoise_cluster/sequence_processing/join_reads.sh'
+        directory = "${meta.denoise_cluster}-${meta.chimera_checking}-${meta.tax_assignment}"
+        axis = params.otu_processing.transform['fork']['axis']
+        column = params.otu_processing.transform['fork']['column']
+        template 'otu_processing/transform/fork.py'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/denoise_cluster/sequence_processing/quality_analysis.nf` & `micone-0.9.0/micone/pipelines/modules/sequence_processing/trimming/quality_analysis_paired.nf`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 include { getHierarchy } from '../../../functions/functions.nf'
 
 // Identify positions on the front and the tail that need to be trimmed based on
 // a. quality and b. sequence retainment
-process quality_analysis {
+process quality_analysis_paired {
     label 'qiime2'
-    tag "${meta.id}"
-    publishDir "${params.output_dir}/${f[0]}/${f[1]}/${f[2]}/${meta.id}",
+    tag "${meta.id}-${meta.run}"
+    publishDir "${params.output_dir}/${f[0]}/${f[1]}/${f[2]}/${meta.id}-${meta.run}",
         mode: 'copy',
         overwrite: true
     input:
-        tuple val(meta), file(qual_summary)
+        tuple val(meta), file(forward_summary), file(reverse_summary)
     output:
-        tuple val(meta), file('trim.txt')
+        tuple val(meta), file('*_trim.txt')
     script:
         String task_process = "${task.process}"
         f = getHierarchy(task_process)
-        template 'denoise_cluster/sequence_processing/quality_analysis.py'
+        template 'sequence_processing/trimming/quality_analysis_paired.py'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/bootstrap/pvalue.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/bootstrap/pvalue.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/bootstrap/resample.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/bootstrap/resample.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/correlation/pearson.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/correlation/pearson.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/correlation/pearson_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/correlation/pearson_workflow.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/correlation/propr.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/correlation/propr.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/correlation/propr_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/correlation/propr_workflow.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/correlation/sparcc.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/correlation/sparcc.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/correlation/sparcc_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/correlation/sparcc_workflow.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/correlation/spearman.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/correlation/spearman.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/correlation/spearman_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/correlation/spearman_workflow.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/direct/export_gml.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/direct/export_gml.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/direct/flashweave.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/direct/flashweave.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/direct/mldm.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/direct/mldm.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/direct/spieceasi.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/direct/spieceasi.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/network/create_consensus.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/network/create_consensus.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/network/make_network_with_pvalue.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/network/make_network_with_pvalue.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/network/make_network_without_pvalue.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/network/make_network_without_pvalue.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/network_inference/network_inference_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/network_inference/network_inference_workflow.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/otu_processing/export/biom2tsv.nf` & `micone-0.9.0/micone/pipelines/modules/otu_processing/export/biom2tsv.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/otu_processing/transform/group.nf` & `micone-0.9.0/micone/pipelines/modules/otu_processing/transform/group.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/otu_processing/transform/normalize.nf` & `micone-0.9.0/micone/pipelines/modules/otu_processing/transform/normalize.nf`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-include { getHierarchy } from '../../../functions/functions.nf'
+include { getHierarchy; updateMeta } from '../../../functions/functions.nf'
 
 process normalize {
     label 'micone'
-    tag "${meta.id}"
-    publishDir "${params.output_dir}/${f[0]}/transform/${f[1]}/${directory}/${meta.id}",
+    tag "${new_meta.id}"
+    publishDir "${params.output_dir}/${f[0]}/transform/${f[1]}/${directory}/${new_meta.id}",
         mode: 'copy',
         overwrite: true
     input:
         tuple val(meta), file(otu_file)
     output:
-        tuple val(meta), file("*_normalized.biom")
+        tuple val(new_meta), file("*_normalized.biom")
     script:
+        new_meta = updateMeta(meta)
+        new_meta.id = "${otu_file.baseName}"  // "meta.id_label"
         String task_process = "${task.process}"
         f = getHierarchy(task_process)
         directory = "${meta.denoise_cluster}-${meta.chimera_checking}-${meta.tax_assignment}"
         axis = params.otu_processing.transform['normalize']['axis']
         count_thres = params.otu_processing.transform['normalize']['count_thres']
         prevalence_thres = params.otu_processing.transform['normalize']['prevalence_thres']
         abundance_thres = params.otu_processing.transform['normalize']['abundance_thres']
```

### Comparing `micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/add_md2biom.nf` & `micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/add_md2biom.nf`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 include { getHierarchy } from '../../../functions/functions.nf'
 
 // Attach the observation and sample metadata to the OTU table
 process add_md2biom {
     label 'qiime2'
     tag "${meta.id}"
-    publishDir "${params.output_dir}/${f[0]}/${f[1]}/taxonomy_tables/${directory}/${meta.id}",
+    publishDir "${params.output_dir}/${f[0]}/${module_dir}/taxonomy_tables/${directory}/${meta.id}",
         mode: 'copy',
         overwrite: true
     input:
         tuple val(meta), file(otu_table_file), file(tax_assignment), file(sample_metadata_file)
     output:
         tuple val(meta), file("otu_table_wtax.biom")
     script:
         String task_process = "${task.process}"
         f = getHierarchy(task_process)
+        module_dir = "${meta.tax_assignment}"
         directory = "${meta.denoise_cluster}-${meta.chimera_checking}"
         template 'tax_assignment/assign/add_md2biom.py'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/naive_bayes.nf` & `micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/naive_bayes.nf`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 include { updateMeta } from '../../../functions/functions.nf'
 
 // Assign taxonomy using the naive bayes classifier
 process naive_bayes {
     label 'qiime2'
-    tag "${new_meta.id}"
+    tag "${new_meta.id}:${classifier_id}"
     input:
         tuple val(meta), file(otu_table), file(rep_seqs), file(sample_metadata)
+        each classifier
     when:
         'naive_bayes' in params.tax_assignment.assign['selection']
     output:
         tuple val(new_meta), file(otu_table), file('taxonomy.tsv'), file(sample_metadata)
     script:
         new_meta = updateMeta(meta)
-        new_meta.tax_assignment = 'naive_bayes'
-        classifier = params.tax_assignment.assign['naive_bayes']['classifier']
+        classifier_id = "${file(classifier).simpleName}"
+        new_meta.tax_assignment = "naive_bayes(${classifier_id})"
         new_meta.taxonomy_database = classifier
         confidence = params.tax_assignment.assign['naive_bayes']['confidence']
         ncpus = params.tax_assignment.assign['naive_bayes']['ncpus']
         template 'tax_assignment/assign/assign_taxonomy_naivebayes.sh'
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/tax_assignment/assign/naive_bayes_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/tax_assignment/assign/blast_workflow.nf`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-include { naive_bayes } from './naive_bayes.nf'
+include { import_reads } from './import_reads.nf'
+include { blast } from './blast.nf'
 include { add_md2biom } from './add_md2biom.nf'
 
-// NOTE: We try to simplify the workflow by requiring the user to pre-train the classifier
 
-workflow naive_bayes_workflow {
+workflow blast_workflow {
     take:
         // tuple val(meta), file('otu_table.biom'), file('rep_seqs.fasta'), file(samplemetadata_files)
         input_channel
     main:
         input_channel \
-            | naive_bayes \
-            | add_md2biom
+            | import_reads
+        blast(
+            import_reads.out,
+            params.tax_assignment.assign['blast']['references']
+        )
+        add_md2biom(blast.out)
     emit:
         // add_md2biom has publishDir
         // tuple val(meta), file("otu_table_wtax.biom")
         add_md2biom.out
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/tax_assignment/tax_assignment_workflow.nf` & `micone-0.9.0/micone/pipelines/modules/tax_assignment/tax_assignment_workflow.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/utils/dc_data_ingestion.nf` & `micone-0.9.0/micone/pipelines/modules/utils/spp_data_ingestion.nf`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 // input:
 // samplesheet
-// id,sequences,barcodes,mapping,sample_metadata
+// id,run,forward,reverse,barcodes,mapping,sample_metadata
 // output1:
-// tuple val(meta), file(sequence_files), file(barcode_files), file(mapping_files)
+// tuple val(meta), file(forward_files), file(reverse_files), file(barcode_files), file(mapping_files)
 // output2:
 // tuple val(meta), file(sample_metadata_files)
 
-workflow dc_data_ingestion {
+workflow spp_data_ingestion {
     take:
     samplesheet
 
     main:
     samplesheet
         .splitCsv(header: true, sep: ',')
-        .map { create_dc_channels(it) }
-        .multiMap { it ->
-            reads: tuple(it[0], it[1], it[2], it[3])
-            sample_md: tuple(it[0], it[4])
+        .map { create_spp_channels(it) }
+        .multiMap { row ->
+            reads: tuple(row[0], row[1], row[2], row[3], row[4])
+            sample_md: tuple(row[0], row[5])
         }
         .set { result }
 
     emit:
     reads = result.reads
     sample_md = result.sample_md
 }
 
 
-def create_dc_channels(LinkedHashMap row) {
+def create_spp_channels(LinkedHashMap row) {
     def meta = [:]
     meta.id = row.id
+    meta.run = row.run
     def array = []
-    if (!file(row.sequences).exists()) {
-        exit 1, "ERROR: Please check input samplesheet -> Sequences file does not exist!\n${row.sequences}"
+    if (!file(row.forward).exists()) {
+        exit 1, "ERROR: Please check input samplesheet -> Forward sequences file does not exist!\n${row.forward_sequences}"
+    }
+    if (!file(row.reverse).exists()) {
+        exit 1, "ERROR: Please check input samplesheet -> Reverse sequences file does not exist!\n${row.reverse_sequences}"
     }
     if (!file(row.barcodes).exists()) {
         exit 1, "ERROR: Please check input samplesheet -> Barcodes file does not exist!\n${row.barcodes}"
     }
     if (!file(row.mapping).exists()) {
         exit 1, "ERROR: Please check input samplesheet -> Mapping file does not exist!\n${row.mapping}"
     }
     if (!file(row.sample_metadata).exists()) {
         exit 1, "ERROR: Please check input samplesheet -> Sample_Metadata file does not exist!\n${row.sample_metadata}"
     }
-    array = [ meta, file(row.sequences), file(row.barcodes), file(row.mapping), file(row.sample_metadata) ]
+    array = [ meta, file(row.forward), file(row.reverse), file(row.barcodes), file(row.mapping), file(row.sample_metadata) ]
     return array
 }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/utils/ni_data_ingestion.nf` & `micone-0.9.0/micone/pipelines/modules/utils/ni_data_ingestion.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/utils/op_data_ingestion.nf` & `micone-0.9.0/micone/pipelines/modules/utils/op_data_ingestion.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/modules/utils/sp_data_ingesetion.nf` & `micone-0.9.0/micone/pipelines/modules/utils/sps_data_ingestion.nf`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 // input:
 // samplesheet
-// id,sequences,barcodes,mapping,sample_metadata
+// id,run,sequences,barcodes,mapping,sample_metadata
 // output1:
 // tuple val(meta), file(sequence_files), file(barcode_files), file(mapping_files)
 // output2:
 // tuple val(meta), file(sample_metadata_files)
 
-workflow sp_data_ingestion {
+workflow sps_data_ingestion {
     take:
     samplesheet
 
     main:
     samplesheet
         .splitCsv(header: true, sep: ',')
-        .map { create_sp_channels(it) }
-        .multiMap { it ->
-            reads: tuple(it[0], it[1], it[2], it[3])
-            sample_md: tuple(it[0], it[4])
+        .map { create_sps_channels(it) }
+        .multiMap { row ->
+            reads: tuple(row[0], row[1], row[2], row[3])
+            sample_md: tuple(row[0], row[4])
         }
         .set { result }
 
     emit:
     reads = result.reads
     sample_md = result.sample_md
 }
 
 
-def create_sp_channels(LinkedHashMap row) {
+def create_sps_channels(LinkedHashMap row) {
     def meta = [:]
     meta.id = row.id
+    meta.run = row.run
     def array = []
     if (!file(row.sequences).exists()) {
         exit 1, "ERROR: Please check input samplesheet -> Sequences file does not exist!\n${row.sequences}"
     }
     if (!file(row.barcodes).exists()) {
         exit 1, "ERROR: Please check input samplesheet -> Barcodes file does not exist!\n${row.barcodes}"
     }
```

### Comparing `micone-0.8.1/micone/pipelines/modules/utils/ta_data_ingestion.nf` & `micone-0.9.0/micone/pipelines/modules/utils/ta_data_ingestion.nf`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/nextflow.config` & `micone-0.9.0/micone/pipelines/nextflow.config`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 // vim:ft=groovy
 
 // Process specific configuration
 includeConfig './nf_micone/configs/process.config'
 includeConfig './nf_micone/configs/profiles.config'
 
 // Module specific configuration
+includeConfig './nf_micone/configs/sequence_processing.config'
 includeConfig './nf_micone/configs/denoise_cluster.config'
 includeConfig './nf_micone/configs/tax_assignment.config'
 includeConfig './nf_micone/configs/otu_processing.config'
 includeConfig './nf_micone/configs/network_inference.config'
 
 // User configuration
 // Refer: documentation for details
 
 params {
-
+    paired_end = false
 }
```

### Comparing `micone-0.8.1/micone/pipelines/pipeline.py` & `micone-0.9.0/micone/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/process.py` & `micone-0.9.0/micone/pipelines/process.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/template.py` & `micone-0.9.0/micone/pipelines/template.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/denoise_cluster/chimera_checking/create_seqtable.py` & `micone-0.9.0/micone/pipelines/templates/denoise_cluster/chimera_checking/create_seqtable.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/denoise_cluster/chimera_checking/remove_chimeras.R` & `micone-0.9.0/micone/pipelines/templates/denoise_cluster/chimera_checking/remove_chimeras.R`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 suppressWarnings(library(dada2))
 
 chimera.method <- "${chimera_method}"
 multithread <- ${ncpus}
 
 # load table and convert to matrix
 seq.table.file <- "${seqtable_file}"
-seq.table <- read.csv(seq.table.file, sep="\\t")
+seq.table <- read.csv(seq.table.file, sep="\\t", check.names=FALSE)
 rownames(seq.table) <- seq.table[,1]
 seq.table <- seq.table[ -c(1) ]
 seq.mat <- data.matrix(seq.table)
 mode(seq.mat) <- "integer"
 
 # chimera removal
 seq.table.nochim <- removeBimeraDenovo(t(seq.mat), method=chimera.method, multithread=multithread, verbose=TRUE)
```

### Comparing `micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/deblur.sh` & `micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/deblur.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env bash
 
 set -e
 
 mkdir sequence_folder
 mv ${sequence_files} sequence_folder
 mv ${manifest_file} sequence_folder
+mv ${sequence_metadata} sequence_folder
 
 deblur workflow \
     --seqs-fp  sequence_folder \
     --output-dir deblur_output \
     -t -1 \
     --left-trim-length 0 \
     --min-reads ${min_reads} \
@@ -20,9 +21,10 @@
 mkdir otu_table
 deblur build-biom-table \
     --min-reads ${min_reads} \
     --file_type .trim.derep.no_artifacts.msa.deblur \
     deblur_output/deblur_working_dir \
     otu_table
 
-mv otu_table/all.biom unhashed_otu_table.biom
-mv otu_table/all.seq.fa unhashed_rep_seqs.fasta
+mv otu_table/all.biom ${meta.id}-${meta.run}_unhashed_otu_table.biom
+mv otu_table/all.seq.fa ${meta.id}-${meta.run}_unhashed_rep_seqs.fasta
+mv ${samplemetadata_files} ${meta.id}-${meta.run}_sample_metadata.tsv
```

### Comparing `micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/fastq2fasta.py` & `micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/fastq2fasta.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-#!/usr/bin/env python2
+#!/usr/bin/env python3
 
+import pathlib
 import os
 import subprocess
 
 
 def convert(data):
     sample_name, file_name = data
     fasta_file = "fasta/" + sample_name + ".fasta"
@@ -13,15 +14,15 @@
     return fasta_file
 
 
 def merge(fasta_files, output_file):
     with open(output_file, "w") as wid:
         for fasta_file in fasta_files:
             with open(fasta_file) as rid:
-                sample_name = fasta_file.split("/")[-1].split(".")[0]
+                sample_name = pathlib.Path(fasta_file).stem
                 count = 0
                 for line in rid:
                     if line.startswith(">"):
                         wid.write(
                             ">{0}_{1} {2}".format(sample_name, str(count), line[1:])
                         )
                     else:
```

### Comparing `micone-0.8.1/micone/pipelines/templates/denoise_cluster/otu_assignment/hashing3.py` & `micone-0.9.0/micone/pipelines/templates/denoise_cluster/otu_assignment/hashing3.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,71 @@
 #!/usr/bin/env python3
 
 import hashlib
+import pathlib
 
 from biom import load_table, Table
 from biom.util import biom_open
 from Bio import SeqIO
 from Bio.SeqIO import FastaIO
+import pandas as pd
 
 
 def hash_function(seq):
     return hashlib.md5(seq.encode("utf-8")).hexdigest()
 
 
-def hash_otu_table(unhashed_otu_table, output_file):
+def hash_otu_table(unhashed_otu_table):
     table = load_table(unhashed_otu_table)
     df = table.to_dataframe(dense=True)
     seq_ids = list(map(hash_function, df.index))
     df.index = seq_ids
-    new_table = Table(df.values, list(df.index), list(df.columns))
-    with biom_open(output_file, "w") as fid:
-        new_table.to_hdf5(fid, "Constructed by micone in dada2 pipeline")
-    return seq_ids
+    return df
 
 
-def hash_rep_seqs(unhashed_rep_seqs, output_file):
-    seqs = list(SeqIO.parse(unhashed_rep_seqs, "fasta"))
-    seq_ids = []
-    for seq in seqs:
+def hash_rep_seqs(unhashed_rep_seqs, rep_seq_ids):
+    seqs_all = list(SeqIO.parse(unhashed_rep_seqs, "fasta"))
+    seqs = []
+    for seq in seqs_all:
         seq.id = hash_function(str(seq.seq))
-        seq_ids.append(seq.id)
-        seq.description = ""
-        seq.name = ""
-    with open(output_file, "w") as fid:
+        if seq.id not in rep_seq_ids:
+            rep_seq_ids.add(seq.id)
+            seq.description = ""
+            seq.name = ""
+            seqs.append(seq)
+    return seqs
+
+
+def hashing(unhashed_otu_table_list, unhashed_rep_seqs_list, sample_metadata_list):
+    otu_df_list = []
+    rep_seq_ids = set()
+    seqs = []
+    # Create OTU table
+    for unhashed_otu_table in unhashed_otu_table_list:
+        otu_df_list.append(hash_otu_table(unhashed_otu_table))
+    otu_df = pd.concat(otu_df_list, join="outer", axis=1)
+    otu_df.fillna(0.0, inplace=True)
+    otu_table = Table(otu_df.values, list(otu_df.index), list(otu_df.columns))
+    # Create rep seqs
+    for unhashed_rep_seqs in unhashed_rep_seqs_list:
+        seqs.extend(hash_rep_seqs(unhashed_rep_seqs, rep_seq_ids))
+    otu_table_ids = set(otu_df.index)
+    assert otu_table_ids == rep_seq_ids
+    assert len(otu_df.index) == len(rep_seq_ids)
+    # Merge sample metadata
+    sample_metadata = pd.concat(
+        [pd.read_csv(s, sep="\\t") for s in sample_metadata_list]
+    )
+    # Write files
+    sample_metadata.to_csv("sample_metadata.tsv", sep="\\t", index=False)
+    with biom_open("otu_table.biom", "w") as fid:
+        otu_table.to_hdf5(fid, "Constructed by micone in dada2/deblur pipeline")
+    with open("rep_seqs.fasta", "w") as fid:
         fasta_writer = FastaIO.FastaWriter(fid, wrap=None)
         fasta_writer.write_file(seqs)
-    return seq_ids
-
-
-def hashing(unhashed_otu_table, unhashed_rep_seqs):
-    otu_table_ids = hash_otu_table(unhashed_otu_table, "otu_table.biom")
-    rep_seq_ids = hash_rep_seqs(unhashed_rep_seqs, "rep_seqs.fasta")
-    assert otu_table_ids == rep_seq_ids
 
 
 if __name__ == "__main__":
-    UNHASHED_OTU_TABLE = "${unhashed_otu_table}"
-    UNHASHED_REP_SEQS = "${unhashed_rep_seqs}"
-    hashing(UNHASHED_OTU_TABLE, UNHASHED_REP_SEQS)
+    UNHASHED_OTU_TABLE_LIST = pathlib.Path().glob("*unhashed_otu_table.biom")
+    UNHASHED_REP_SEQS_LIST = pathlib.Path().glob("*unhashed_rep_seqs.fasta")
+    SAMPLE_METADATA_LIST = pathlib.Path().glob("*sample_metadata.tsv")
+    hashing(UNHASHED_OTU_TABLE_LIST, UNHASHED_REP_SEQS_LIST, SAMPLE_METADATA_LIST)
```

### Comparing `micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/export_visualization.py` & `micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/export_visualization.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/quality_analysis.py` & `micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/quality_analysis_single.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/denoise_cluster/sequence_processing/trimming.R` & `micone-0.9.0/micone/pipelines/templates/sequence_processing/trimming/trimming_single.R`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/bootstrap/filter.py` & `micone-0.9.0/micone/pipelines/templates/network_inference/bootstrap/filter.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/correlation/pearson.py` & `micone-0.9.0/micone/pipelines/templates/network_inference/correlation/pearson.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/correlation/propr.R` & `micone-0.9.0/micone/pipelines/templates/network_inference/correlation/propr.R`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/correlation/spearman.py` & `micone-0.9.0/micone/pipelines/templates/network_inference/correlation/spearman.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/direct/export_gml.py` & `micone-0.9.0/micone/pipelines/templates/network_inference/direct/export_gml.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/direct/flashweave.jl` & `micone-0.9.0/micone/pipelines/templates/network_inference/direct/flashweave.jl`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/direct/mldm.R` & `micone-0.9.0/micone/pipelines/templates/network_inference/direct/mldm.R`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/direct/spieceasi.R` & `micone-0.9.0/micone/pipelines/templates/network_inference/direct/spieceasi.R`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/network/create_consensus.py` & `micone-0.9.0/micone/pipelines/templates/network_inference/network/create_consensus.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,9 +31,9 @@
 
 if __name__ == "__main__":
     BASE_NAME = "consensus"
     METHOD = "${method}"
     PARAMETER = float("${parameter}")
     PVALUE_FILTER = True if "${pvalue_filter}" == "true" else False
     INTERACTION_FILTER = True if "${interaction_filter}" == "true" else False
-    NETWORK_FILES = list(pathlib.Path().glob("*.json"))
+    NETWORK_FILES = list(pathlib.Path().glob("*_network.json"))
     main(BASE_NAME, NETWORK_FILES, METHOD, PARAMETER, PVALUE_FILTER, INTERACTION_FILTER)
```

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/network/make_network_with_pvalue.py` & `micone-0.9.0/micone/pipelines/templates/network_inference/network/make_network_with_pvalue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 import json
 
-from micone import Network, NetworkGroup
+from micone import Network
 
 
 def main(
     base_name: str,
     corr_file: str,
     meta_file: str,
     cmeta_file: str,
@@ -23,17 +23,17 @@
         obsmeta_file=obsmeta_file,
         pvalue_file=pvalue_file,
         children_file=children_file,
         interaction_threshold=interaction_threshold,
         pvalue_threshold=pvalue_threshold,
     )
     network.write(base_name + "_network.json")
-    network.write(
-        base_name + "_thres_network.json", pvalue_filter=True, interaction_filter=True
-    )
+    # network.write(
+    #     base_name + "_network_thres.json", pvalue_filter=True, interaction_filter=True
+    # )
 
 
 def create_cmetadata():
     cmetadata = {
         "denoise_cluster": "${meta.denoise_cluster}",
         "chimera_checking": "${meta.chimera_checking}",
         "taxonomy_assignment": "${meta.taxonomy_assignment}",
@@ -45,18 +45,22 @@
 
 
 if __name__ == "__main__":
     BASE_NAME = "${meta.id}"
     CORR_FILE = "${corr_file}"
     PVALUE_FILE = "${pvalue_file}"
     META_FILE = "${metadata_file}"
+    if not META_FILE:
+        raise ValueError(
+            "The metadata file needs to be supplied via network.config in make_network_with_pvalue"
+        )
     OBSMETA_FILE = "${obs_metadata}"
     CHILDREN_FILE = "${children_map}"
-    INTERACTION_THRESHOLD = ${interaction_threshold}
-    PVALUE_THRESHOLD = ${pvalue_threshold}
+    INTERACTION_THRESHOLD = float("${interaction_threshold}")
+    PVALUE_THRESHOLD = float("${pvalue_threshold}")
     create_cmetadata()
     CMETA_FILE = "cmetadata.json"
     main(
         BASE_NAME,
         CORR_FILE,
         META_FILE,
         CMETA_FILE,
```

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/network/make_network_without_pvalue.py` & `micone-0.9.0/micone/pipelines/templates/network_inference/network/make_network_without_pvalue.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,19 +17,20 @@
     network = Network.load_data(
         interaction_file=corr_file,
         meta_file=meta_file,
         cmeta_file=cmeta_file,
         obsmeta_file=obsmeta_file,
         children_file=children_file,
         interaction_threshold=interaction_threshold,
+        pvalue_correction=None,
     )
     network.write(base_name + "_network.json")
-    network.write(
-        base_name + "_thres_network.json", pvalue_filter=False, interaction_filter=True
-    )
+    # network.write(
+    #     base_name + "_network_thres.json", pvalue_filter=False, interaction_filter=True
+    # )
 
 
 def create_cmetadata():
     cmetadata = {
         "denoise_cluster": "${meta.denoise_cluster}",
         "chimera_checking": "${meta.chimera_checking}",
         "taxonomy_assignment": "${meta.taxonomy_assignment}",
@@ -40,17 +41,21 @@
         json.dump(cmetadata, fid)
 
 
 if __name__ == "__main__":
     BASE_NAME = "${meta.id}"
     CORR_FILE = "${corr_file}"
     META_FILE = "${metadata_file}"
+    if not META_FILE:
+        raise ValueError(
+            "The metadata file needs to be supplied via network.config in make_network_without_pvalue"
+        )
     OBSMETA_FILE = "${obs_metadata}"
     CHILDREN_FILE = "${children_map}"
-    INTERACTION_THRESHOLD = ${interaction_threshold}
+    INTERACTION_THRESHOLD = float("${interaction_threshold}")
     create_cmetadata()
     CMETA_FILE = "cmetadata.json"
     main(
         BASE_NAME,
         CORR_FILE,
         META_FILE,
         CMETA_FILE,
```

### Comparing `micone-0.8.1/micone/pipelines/templates/network_inference/network/merge_pvalues.py` & `micone-0.9.0/micone/pipelines/templates/network_inference/network/merge_pvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     merged_network_group.write(
         "merged/" + base_name + "_network.json", split_files=True
     )
 
 
 if __name__ == "__main__":
     BASE_NAME = "merged"
-    NETWORK_FILES = list(pathlib.Path().glob("*.json"))
+    NETWORK_FILES = list(pathlib.Path().glob("*_network.json"))
     main(BASE_NAME, NETWORK_FILES)
```

### Comparing `micone-0.8.1/micone/pipelines/templates/otu_processing/transform/group.py` & `micone-0.9.0/micone/pipelines/templates/otu_processing/transform/group.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/otu_processing/transform/normalize.py` & `micone-0.9.0/micone/pipelines/templates/otu_processing/transform/normalize.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,35 +9,35 @@
     rm_sparse_obs: str,
     axis: str,
     count_thres: int,
     prevalence_thres: float,
     abundance_thres: float,
 ) -> Otu:
     otu = Otu.load_data(otu_file)
-    if rm_sparse_samples == "True":
+    if rm_sparse_samples == "true":
         otu = otu.rm_sparse_samples(count_thres=count_thres)
-    if rm_sparse_obs == "True":
+    if rm_sparse_obs == "true":
         otu = otu.rm_sparse_obs(
             prevalence_thres=prevalence_thres, abundance_thres=abundance_thres
         )
     if axis != "None":
         otu_norm = otu.normalize(axis=axis)
     else:
         otu_norm = otu
     return otu_norm
 
 
 if __name__ == "__main__":
     OTU_FILE = "${otu_file}"
     AXIS = "${axis}"
     RM_SPARSE_SAMPLES = "${rm_sparse_samples}"
-    COUNT_THRES = ${count_thres}
+    COUNT_THRES = int("${count_thres}")
     RM_SPARSE_OBS = "${rm_sparse_obs}"
-    PREVALENCE_THRES = ${prevalence_thres}
-    ABUNDANCE_THRES = ${abundance_thres}
+    PREVALENCE_THRES = float("${prevalence_thres}")
+    ABUNDANCE_THRES = float("${abundance_thres}")
     norm_otu = main(
         OTU_FILE,
         RM_SPARSE_SAMPLES,
         RM_SPARSE_OBS,
         AXIS,
         COUNT_THRES,
         PREVALENCE_THRES,
```

### Comparing `micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/add_md2biom.py` & `micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/add_md2biom.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,28 +19,28 @@
     tax_list.extend([""] * (len(HEADERS) - len(tax_list)))
     return pd.Series(data=tax_list, index=HEADERS)
 
 
 def main(otu_table_file, tax_assignment_file, sample_metadata_file):
     otu_table = load_table(otu_table_file)
     if os.path.splitext(sample_metadata_file)[1] == "csv":
-        sample_metadata = pd.read_csv(sample_metadata_file, index_col=0)
+        sample_metadata = pd.read_csv(sample_metadata_file, index_col=0, comment="#")
     else:
-        sample_metadata = pd.read_table(sample_metadata_file, index_col=0)
+        sample_metadata = pd.read_table(sample_metadata_file, index_col=0, comment="#")
     tax_assignment = pd.read_table(tax_assignment_file, index_col=0)
     obs_metadata = tax_assignment[["Taxon"]].apply(tax_splitter, axis=1)
     for index in otu_table.ids("observation"):
         if index not in obs_metadata.index:
             obs_metadata.loc[index] = [""] * len(HEADERS)
     otu_table.del_metadata(axis="observation")
     otu_table.add_metadata(obs_metadata.to_dict(orient="index"), axis="observation")
     otu_table.del_metadata(axis="sample")
     otu_table.add_metadata(sample_metadata.to_dict(orient="index"), axis="sample")
     with biom_open("otu_table_wtax.biom", "w") as fid:
-        otu_table.to_hdf5(fid, "Constructed using the blast pipeline")
+        otu_table.to_hdf5(fid, "Constructed using the micone pipeline")
 
 
 if __name__ == "__main__":
     OTU_TABLE = "${otu_table_file}"
     TAX_ASSIGNMENT = "${tax_assignment}"
     SAMPLE_METADATA = "${sample_metadata_file}"
     main(OTU_TABLE, TAX_ASSIGNMENT, SAMPLE_METADATA)
```

### Comparing `micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/assign_taxonomy_blast.sh` & `micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/assign_taxonomy_blast.sh`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/assign_taxonomy_naivebayes.sh` & `micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/assign_taxonomy_naivebayes.sh`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/pipelines/templates/tax_assignment/assign/train_classifier.sh` & `micone-0.9.0/micone/pipelines/templates/tax_assignment/assign/train_classifier.sh`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/setup/environments.py` & `micone-0.9.0/micone/setup/environments.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/utils/spinner.py` & `micone-0.9.0/micone/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/validation/network_schema.py` & `micone-0.9.0/micone/validation/network_schema.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/validation/otu_schema.py` & `micone-0.9.0/micone/validation/otu_schema.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/micone/validation/otu_validator.py` & `micone-0.9.0/micone/validation/otu_validator.py`

 * *Files identical despite different names*

### Comparing `micone-0.8.1/pyproject.toml` & `micone-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "micone"
-version = "0.8.1"
+version = "0.9.0"
 description = "The Microbial Co-occurrence Network Explorer"
 authors = ["Dileep Kishore <dkishore@bu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/segrelab/MiCoNE"
 documentation = "https://micone.readthedocs.io/en/latest"
```

### Comparing `micone-0.8.1/setup.py` & `micone-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
  'micone.config',
  'micone.conversion',
  'micone.logging',
  'micone.main',
  'micone.pipelines',
  'micone.pipelines.templates.denoise_cluster.chimera_checking',
  'micone.pipelines.templates.denoise_cluster.otu_assignment',
- 'micone.pipelines.templates.denoise_cluster.sequence_processing',
  'micone.pipelines.templates.network_inference.bootstrap',
  'micone.pipelines.templates.network_inference.correlation',
  'micone.pipelines.templates.network_inference.direct',
  'micone.pipelines.templates.network_inference.network',
  'micone.pipelines.templates.otu_processing.export',
  'micone.pipelines.templates.otu_processing.transform',
+ 'micone.pipelines.templates.sequence_processing.trimming',
  'micone.pipelines.templates.tax_assignment.assign',
  'micone.setup',
  'micone.utils',
  'micone.validation']
 
 package_data = \
 {'': ['*'],
@@ -34,26 +34,29 @@
                       'envs/micone-qiime2/*',
                       'envs/micone-sparcc/*',
                       'envs/micone-spieceasi/*',
                       'functions/*',
                       'modules/denoise_cluster/*',
                       'modules/denoise_cluster/chimera_checking/*',
                       'modules/denoise_cluster/otu_assignment/*',
-                      'modules/denoise_cluster/sequence_processing/*',
                       'modules/network_inference/*',
                       'modules/network_inference/bootstrap/*',
                       'modules/network_inference/correlation/*',
                       'modules/network_inference/direct/*',
                       'modules/network_inference/network/*',
                       'modules/otu_processing/*',
                       'modules/otu_processing/export/*',
                       'modules/otu_processing/transform/*',
+                      'modules/sequence_processing/*',
+                      'modules/sequence_processing/demultiplexing/*',
+                      'modules/sequence_processing/trimming/*',
                       'modules/tax_assignment/*',
                       'modules/tax_assignment/assign/*',
-                      'modules/utils/*']}
+                      'modules/utils/*',
+                      'templates/sequence_processing/demultiplexing/*']}
 
 install_requires = \
 ['Jinja2>=2.11.2,<3.0.0',
  'biom-format>=2.1.10,<3.0.0',
  'click>=7.1.2,<8.0.0',
  'ete3>=3.1.2,<4.0.0',
  'h5py>=3.1.0,<4.0.0',
@@ -73,15 +76,15 @@
 {'docs': ['Sphinx>=3.4.2,<4.0.0', 'sphinx-rtd-theme>=0.5.1,<0.6.0']}
 
 entry_points = \
 {'console_scripts': ['micone = micone.cli:main']}
 
 setup_kwargs = {
     'name': 'micone',
-    'version': '0.8.1',
+    'version': '0.9.0',
     'description': 'The Microbial Co-occurrence Network Explorer',
     'long_description': '# MiCoNE - Microbial Co-occurrence Network Explorer\n\n![Build Status](https://github.com/segrelab/MiCoNE/workflows/build/badge.svg)\n[![Documentation Status](https://readthedocs.org/projects/micone/badge/?version=latest)](https://micone.readthedocs.io/en/latest/?badge=latest)\n[![codecov](https://codecov.io/gh/segrelab/MiCoNE/branch/master/graph/badge.svg?token=2tKiI0lUJb)](https://codecov.io/gh/segrelab/MiCoNE)\n[![CodeFactor](https://www.codefactor.io/repository/github/segrelab/micone/badge)](https://www.codefactor.io/repository/github/segrelab/micone)\n[![Updates](https://pyup.io/repos/github/segrelab/MiCoNE/shield.svg)](https://pyup.io/repos/github/segrelab/MiCoNE/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n\n`MiCoNE`, is a flexible and modular pipeline for 16S data analysis.\nIt incorporates various popular, publicly available tools as well as custom Python modules and scripts to facilitate inference of co-occurrence networks from 16S data.\n\n<div align="center">\n⚠️ <p><strong>The package is under active development and breaking changes are possible</strong></p>\n</div>\n\n-   Free software: MIT license\n-   Documentation: <https://micone.readthedocs.io/>\n\nManuscript can be found on [bioRxiv](https://www.biorxiv.org/content/10.1101/2020.09.23.309781v2)\n\n## Features\n\n-   Plug and play architecture: allows easy additions and removal of new tools\n-   Flexible and portable: allows running the pipeline on local machine, compute cluster or the cloud with minimal configuration change. Uses the [nextflow](www.nextflow.io) under the hood\n-   Parallelization: automatic parallelization both within and across samples (needs to be enabled in the `config` file)\n-   Ease of use: available as a minimal `Python` library (without the pipeline) or the full `conda` package\n\n## Installation\n\nInstalling the minimal `Python` library:\n\n```sh\npip install micone\n```\n\nInstalling the `conda` package:\n\n```sh\ngit clone https://github.com/segrelab/MiCoNE.git\ncd MiCoNE\nconda env create -n micone -f env.yml\npip install .\n```\n\n> NOTE:\n> The `conda` package is currently being updated and will be available soon.\n\n## Workflow\n\n![pipeline](assets/pipeline.png)\n\nIt supports the conversion of raw 16S sequence data or counts matrices into co-occurrence networks through multiple methods. Each process in the pipeline supports alternate tools for performing the same task, users can use the configuration file to change these values.\n\n## Usage\n\nThe `MiCoNE` pipelines comes with an easy to use CLI. To get a list of subcommands you can type:\n\n```bash\nmicone --help\n```\n\nSupported subcommands:\n\n1. `init` - Creates `conda` environments for various pipeline processes\n2. `run` - The main subcommand that runs the pipeline\n3. `clean` - Cleans temporary data, log files and other extraneous files\n\nTo run the pipeline:\n\n```bash\nmicone run -p local -c run.toml -m 4\n```\n\nThis runs the pipeline in the `local` machine using `run.toml` for the pipeline configuration and with a maximum of 4 processes in parallel at a time.\n\n## Configuration\n\nThe configuration of the pipeline can be done using a `.toml` file.\nThe details can be found in the relevant section in the docs.\nHere is an example `config` file that performs:\n\n1. grouping of OTUs by taxonomy level\n2. correlation of the taxa using `fastspar`\n3. calculates p-values\n4. constructs the networks\n\n```toml\ntitle = "A example pipeline for testing"\n\norder = """\n  otu_processing.filter.group\n  otu_processing.export.biom2tsv\n  network_inference.bootstrap.resample\n  network_inference.correlation.sparcc\n  network_inference.bootstrap.pvalue\n  network_inference.network.make_network_with_pvalue\n"""\n\noutput_location = "/home/dileep/Documents/results/sparcc_network"\n\n[otu_processing.filter.group]\n  [[otu_processing.filter.group.input]]\n    datatype = "otu_table"\n    format = ["biom"]\n    location = "correlations/good/deblur/deblur.biom"\n  [[otu_processing.filter.group.parameters]]\n    process = "group"\n    tax_levels = "[\'Family\', \'Genus\', \'Species\']"\n\n[otu_processing.export.biom2tsv]\n\n[network_inference.bootstrap.resample]\n  [[network_inference.bootstrap.resample.parameters]]\n    process = "resample"\n    bootstraps = 10\n\n[network_inference.correlation.sparcc]\n  [[network_inference.correlation.sparcc.parameters]]\n    process = "sparcc"\n    iterations = 5\n\n[network_inference.bootstrap.pvalue]\n\n[network_inference.network.make_network_with_pvalue]\n  [[network_inference.network.make_network_with_pvalue.input]]\n    datatype = "metadata"\n    format = ["json"]\n    location = "correlations/good/deblur/deblur_metadata.json"\n  [[network_inference.network.make_network_with_pvalue.input]]\n    datatype = "computational_metadata"\n    format = ["json"]\n    location = "correlations/good/deblur/deblur_cmetadata.json"\n```\n\nOther example `config` files can be found at `tests/data/pipelines`\n\n## Credits\n\nThis package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.\n',
     'author': 'Dileep Kishore',
     'author_email': 'dkishore@bu.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/segrelab/MiCoNE',
```

### Comparing `micone-0.8.1/PKG-INFO` & `micone-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micone
-Version: 0.8.1
+Version: 0.9.0
 Summary: The Microbial Co-occurrence Network Explorer
 Home-page: https://github.com/segrelab/MiCoNE
 License: MIT
 Author: Dileep Kishore
 Author-email: dkishore@bu.edu
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
```

