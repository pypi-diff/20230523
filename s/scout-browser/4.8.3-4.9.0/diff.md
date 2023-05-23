# Comparing `tmp/scout-browser-4.8.3.tar.gz` & `tmp/scout-browser-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scout-browser-4.8.3.tar", last modified: Wed Nov 13 13:47:24 2019, max compression
+gzip compressed data, was "dist/scout-browser-4.9.0.tar", last modified: Wed Nov 27 07:45:41 2019, max compression
```

## Comparing `scout-browser-4.8.3.tar` & `scout-browser-4.9.0.tar`

### file list

```diff
@@ -1,660 +1,760 @@
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    19561 2019-11-13 13:46:21.000000 scout-browser-4.8.3/CHANGELOG.md
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1485 2018-06-15 11:15:21.000000 scout-browser-4.8.3/LICENSE
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      636 2018-06-15 11:15:21.000000 scout-browser-4.8.3/MANIFEST.in
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     9363 2019-11-13 13:47:24.000000 scout-browser-4.8.3/PKG-INFO
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7182 2019-10-23 12:24:42.000000 scout-browser-4.8.3/README.md
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      239 2019-11-13 13:45:51.000000 scout-browser-4.8.3/requirements-dev.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      574 2019-11-13 13:45:51.000000 scout-browser-4.8.3/requirements.txt
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      124 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/__init__.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)      372 2019-10-16 07:34:29.000000 scout-browser-4.8.3/scout/__main__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       22 2019-11-13 13:46:21.000000 scout-browser-4.8.3/scout/__version__.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/adapter/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       85 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/adapter/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1563 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/adapter/client.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/adapter/mongo/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       30 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/adapter/mongo/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3399 2019-10-07 07:11:42.000000 scout-browser-4.8.3/scout/adapter/mongo/acmg.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)     3336 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/adapter/mongo/base.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    31584 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/adapter/mongo/case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    19764 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/adapter/mongo/case_events.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    14641 2019-08-20 07:16:43.000000 scout-browser-4.8.3/scout/adapter/mongo/clinvar.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    12403 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/adapter/mongo/event.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4370 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/adapter/mongo/filter.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    14409 2019-10-24 09:20:44.000000 scout-browser-4.8.3/scout/adapter/mongo/hgnc.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5314 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/adapter/mongo/hpo.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2747 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/adapter/mongo/index.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6024 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/adapter/mongo/institute.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3091 2019-09-26 07:27:49.000000 scout-browser-4.8.3/scout/adapter/mongo/matchmaker.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    15679 2019-10-29 11:17:17.000000 scout-browser-4.8.3/scout/adapter/mongo/panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    23928 2019-10-25 13:13:21.000000 scout-browser-4.8.3/scout/adapter/mongo/query.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7389 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/adapter/mongo/transcript.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2896 2019-11-06 12:40:59.000000 scout-browser-4.8.3/scout/adapter/mongo/user.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    24897 2019-11-05 16:39:07.000000 scout-browser-4.8.3/scout/adapter/mongo/variant.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    25159 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/adapter/mongo/variant_events.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    24224 2019-10-29 07:28:17.000000 scout-browser-4.8.3/scout/adapter/mongo/variant_loader.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1550 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/adapter/utils.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/build/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      511 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/build/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1656 2019-10-07 07:11:42.000000 scout-browser-4.8.3/scout/build/acmg.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8234 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/build/case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2631 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/build/disease.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/build/genes/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)        1 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/build/genes/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2345 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/build/genes/exon.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4804 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/build/genes/hgnc_gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2228 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/build/genes/transcript.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1124 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/build/hpo.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3411 2019-08-20 07:16:43.000000 scout-browser-4.8.3/scout/build/individual.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      918 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/build/institute.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4674 2019-09-26 07:27:49.000000 scout-browser-4.8.3/scout/build/panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      359 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/build/phenotype.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      861 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/build/user.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/build/variant/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      172 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/build/variant/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      734 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/build/variant/clnsig.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      848 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/build/variant/compound.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3594 2019-11-04 10:01:16.000000 scout-browser-4.8.3/scout/build/variant/gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      720 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/build/variant/genotype.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2582 2019-09-09 13:20:04.000000 scout-browser-4.8.3/scout/build/variant/transcript.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    14076 2019-10-29 11:17:25.000000 scout-browser-4.8.3/scout/build/variant/variant.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/commands/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       22 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/commands/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3612 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/commands/base.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1059 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/convert.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/commands/delete/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       34 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/commands/delete/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5217 2019-09-26 07:27:49.000000 scout-browser-4.8.3/scout/commands/delete/delete_command.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/commands/export/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       34 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/commands/export/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2139 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/export/case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      679 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/export/exon.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)      896 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/export/export_command.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1267 2019-10-26 04:09:12.000000 scout-browser-4.8.3/scout/commands/export/gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      713 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/export/hpo.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3337 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/export/mitochondrial_report.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1553 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/export/panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      988 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/export/transcript.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      266 2019-08-20 07:16:43.000000 scout-browser-4.8.3/scout/commands/export/utils.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5859 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/export/variant.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      749 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/index_command.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/commands/load/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       23 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/commands/load/__init__.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)      925 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/load/base.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3052 2019-09-02 09:39:15.000000 scout-browser-4.8.3/scout/commands/load/case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1868 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/load/exons.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1105 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/load/institute.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2829 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/load/panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      844 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/load/region.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      810 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/load/report.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4145 2019-09-02 09:39:15.000000 scout-browser-4.8.3/scout/commands/load/research.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)     1452 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/commands/load/user.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4872 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/commands/load/variants.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2054 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/serve.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/commands/setup/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       30 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/commands/setup/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4457 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/commands/setup/setup_scout.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/commands/update/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       25 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/commands/update/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1060 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/update/base.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5383 2019-06-14 10:28:22.000000 scout-browser-4.8.3/scout/commands/update/case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      752 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/update/compounds.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)     1397 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/update/disease.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)     3419 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/commands/update/genes.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      816 2019-09-26 07:27:49.000000 scout-browser-4.8.3/scout/commands/update/hpo.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1517 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/update/institute.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1395 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/update/omim.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1575 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/update/panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1974 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/update/phenotype_groups.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2694 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/update/user.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      312 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/commands/utils.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/commands/view/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       23 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/commands/view/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2035 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/view/aliases.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1110 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/view/base.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2954 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/view/case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      454 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/view/collections.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      703 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/view/diseases.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1283 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/view/exons.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1396 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/view/hgnc.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1442 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/view/hpo.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      760 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/view/index.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1775 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/view/individuals.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1379 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/view/institutes.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1393 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/view/intervals.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      933 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/view/panels.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1221 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/view/transcripts.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      799 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/commands/view/users.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      509 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/view/whitelist.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)      997 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/commands/wipe_database.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/constants/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3639 2019-11-05 13:28:01.000000 scout-browser-4.8.3/scout/constants/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7861 2019-10-08 10:56:44.000000 scout-browser-4.8.3/scout/constants/acmg.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2204 2019-11-04 10:24:49.000000 scout-browser-4.8.3/scout/constants/case_tags.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3274 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/constants/clinvar.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1126 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/constants/clnsig.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      723 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/constants/file_types.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      667 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/constants/gene_tags.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3873 2019-03-25 14:01:02.000000 scout-browser-4.8.3/scout/constants/indexes.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1578 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/constants/phenotype.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1178 2019-10-25 13:13:20.000000 scout-browser-4.8.3/scout/constants/query_terms.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3110 2019-10-08 10:56:44.000000 scout-browser-4.8.3/scout/constants/so_terms.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6187 2019-10-26 04:09:12.000000 scout-browser-4.8.3/scout/constants/variant_tags.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1251 2019-03-25 14:01:02.000000 scout-browser-4.8.3/scout/constants/variants_export.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/demo/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11927 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.clinical.SV.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1284 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.clinical.SV.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1941 2019-10-29 11:17:25.000000 scout-browser-4.8.3/scout/demo/643594.clinical.str.annotated.limits.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1698 2019-10-29 11:17:25.000000 scout-browser-4.8.3/scout/demo/643594.clinical.str.annotated.limits.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1744 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.clinical.str.annotated.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1700 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.clinical.str.annotated.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1631 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.clinical.str.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1695 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.clinical.str.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   408608 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.clinical.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7711 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.clinical.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1808 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/demo/643594.config.yaml
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      154 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/643594.ped
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      445 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/643594.ped_check.csv
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      421 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/643594.peddy.ped
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11927 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.research.SV.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1284 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.research.SV.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   440072 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.research.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7702 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/643594.research.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      239 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/643594.sex_check.csv
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   409369 2019-10-07 07:11:42.000000 scout-browser-4.8.3/scout/demo/643595.clinical.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7733 2019-10-07 07:11:42.000000 scout-browser-4.8.3/scout/demo/643595.clinical.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1435 2019-10-07 07:11:42.000000 scout-browser-4.8.3/scout/demo/643595.config.yaml
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       30 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/ADM1059A1.dummy.cgh
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       30 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/ADM1059A2.dummy.cgh
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       30 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/ADM1059A3.dummy.cgh
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1414 2019-10-29 11:17:25.000000 scout-browser-4.8.3/scout/demo/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      830 2019-05-03 10:43:18.000000 scout-browser-4.8.3/scout/demo/cancer.load_config.yaml
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       36 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/cancer_test.ped
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    33942 2019-10-03 08:25:03.000000 scout-browser-4.8.3/scout/demo/cancer_test.vcf
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     9854 2019-10-07 07:23:29.000000 scout-browser-4.8.3/scout/demo/cancer_test.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1055 2019-10-07 07:23:29.000000 scout-browser-4.8.3/scout/demo/cancer_test.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   997982 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/chanjo4_demo.sql
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   225269 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/delivery_report.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3813 2019-03-25 14:01:02.000000 scout-browser-4.8.3/scout/demo/empty.clinical.SV.vcf.gz
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       72 2019-03-25 14:01:02.000000 scout-browser-4.8.3/scout/demo/empty.clinical.SV.vcf.gz.tbi
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1636 2019-03-01 12:08:50.000000 scout-browser-4.8.3/scout/demo/empty_vcf.config.yaml
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5187 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/madeline.xml
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8903 2018-10-30 12:02:09.000000 scout-browser-4.8.3/scout/demo/panel_1.bed
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6075 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/demo/panel_1.csv
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6145 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/panel_1.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   492247 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/reduced_mt.bam
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      808 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/reduced_mt.bam.bai
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/demo/resources/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   321814 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_diseases_to_genes_to_phenotypes_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   214557 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_genes_to_phenotype_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   888123 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_phenotype_to_genes_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2566 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/demo/resources/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3536 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/chanjo4_structure.sql
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)  1609018 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/demo/resources/ensembl_exons_37_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)  1609018 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/demo/resources/ensembl_exons_38_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    12736 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/ensembl_genes_37_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    12731 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/ensembl_genes_38_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   150542 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/ensembl_transcripts_37_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   253991 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/ensembl_transcripts_38_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    64800 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/forweb_cleaned_exac_r03_march16_z_data_pLI_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    54452 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/genemap2_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   122488 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/hgnc_reduced_set.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    80883 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/hpo_terms.csv
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    10588 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/mim2gene_reduced.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)  1152237 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/demo/resources/reduced.hpo.obo
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/exceptions/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      219 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/exceptions/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       38 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/exceptions/config.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1104 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/exceptions/database.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       40 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/exceptions/pedigree.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       35 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/exceptions/vcf.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/export/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)        0 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/export/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2714 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/export/exon.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      270 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/export/gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5198 2019-09-02 09:39:15.000000 scout-browser-4.8.3/scout/export/panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      411 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/export/transcript.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6332 2019-10-07 07:11:42.000000 scout-browser-4.8.3/scout/export/variant.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/load/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      230 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/load/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4268 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/load/all.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1066 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/load/case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2153 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/load/exon.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5255 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/load/hgnc_gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5218 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/load/hpo.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      697 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/load/institute.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4283 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/load/panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1615 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/load/report.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6482 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/load/setup.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4526 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/load/transcript.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/log/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       63 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/log/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1332 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/log/handlers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1684 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/log/log.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/models/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      131 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/models/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      687 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/models/acmg_evaluation.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/models/case/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      110 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/models/case/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3010 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/models/case/case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1984 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/models/event.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4386 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/models/hgnc_map.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1265 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/models/institute.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      664 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/models/panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2421 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/models/phenotype_term.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1031 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/models/user.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/models/variant/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       42 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/models/variant/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      790 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/models/variant/gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1617 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/models/variant/transcript.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3840 2019-03-25 14:01:02.000000 scout-browser-4.8.3/scout/models/variant/variant.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      376 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/models/whitelist.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/parse/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)        0 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/parse/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    15158 2019-11-12 17:23:36.000000 scout-browser-4.8.3/scout/parse/case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6895 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/parse/clinvar.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1871 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/parse/cytoband.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     9192 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/parse/ensembl.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1465 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/parse/exac.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3277 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/parse/hgnc.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    10682 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/parse/hpo.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8433 2019-05-03 10:43:18.000000 scout-browser-4.8.3/scout/parse/matchmaker.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    14740 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/parse/omim.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    13553 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/parse/panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5557 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/parse/peddy.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/parse/variant/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       34 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/parse/variant/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1365 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/parse/variant/callers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3873 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/parse/variant/clnsig.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)     1534 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/parse/variant/compound.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1666 2019-03-25 14:01:02.000000 scout-browser-4.8.3/scout/parse/variant/conservation.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4962 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/parse/variant/coordinates.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      564 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/parse/variant/deleteriousness.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6209 2019-09-09 13:20:04.000000 scout-browser-4.8.3/scout/parse/variant/frequency.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)     4266 2019-08-29 07:04:29.000000 scout-browser-4.8.3/scout/parse/variant/gene.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)     6954 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/parse/variant/genotype.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1589 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/parse/variant/headers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2678 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/parse/variant/ids.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      508 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/parse/variant/models.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      508 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/parse/variant/rank_score.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7607 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/parse/variant/transcript.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    10290 2019-10-29 11:17:25.000000 scout-browser-4.8.3/scout/parse/variant/variant.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/resources/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      214 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/resources/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6264 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/resources/cytoBand.txt.gz
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       24 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7167 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/app.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      206 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/auto.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       24 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/__init__.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/alignviewers/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       59 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/server/blueprints/alignviewers/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1956 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/server/blueprints/alignviewers/partial.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/alignviewers/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/alignviewers/templates/alignviewers/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3371 2019-09-27 06:34:29.000000 scout-browser-4.8.3/scout/server/blueprints/alignviewers/templates/alignviewers/igv_viewer.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4082 2019-10-07 09:25:32.000000 scout-browser-4.8.3/scout/server/blueprints/alignviewers/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/api/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       26 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/api/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      898 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/api/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/cases/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       52 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/cases/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    35217 2019-11-12 17:23:36.000000 scout-browser-4.8.3/scout/server/blueprints/cases/controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1207 2019-08-29 07:04:29.000000 scout-browser-4.8.3/scout/server/blueprints/cases/forms.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/cases/static/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1175 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/cases/static/madeline.js
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5187 2019-11-12 14:25:33.000000 scout-browser-4.8.3/scout/server/blueprints/cases/static/madeline.svg
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    47320 2019-11-05 13:28:01.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/case.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    14111 2019-11-06 07:56:32.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/case_ideograms.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    43242 2019-11-12 17:23:36.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/case_report.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    14387 2019-11-05 16:39:07.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/cases.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5697 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/causatives.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    14168 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/clinvar_submissions.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    18031 2019-11-12 17:23:36.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/collapsible_actionbar.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1681 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/diseases.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7227 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/gene_variants.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      887 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/index.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11254 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/matchmaker.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    40369 2019-11-05 16:39:07.000000 scout-browser-4.8.3/scout/server/blueprints/cases/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/dashboard/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       69 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/dashboard/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    10485 2019-05-03 10:43:18.000000 scout-browser-4.8.3/scout/server/blueprints/dashboard/controllers.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/dashboard/static/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5768 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/dashboard/static/charts.js
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/dashboard/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/dashboard/templates/dashboard/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8382 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/dashboard/templates/dashboard/dashboard_general.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2848 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/dashboard/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/genes/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       52 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/genes/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2156 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/server/blueprints/genes/controllers.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/genes/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/genes/templates/genes/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7293 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/genes/templates/genes/gene.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      880 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/genes/templates/genes/genes.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1100 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/genes/templates/genes/layout.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1591 2019-09-26 07:27:50.000000 scout-browser-4.8.3/scout/server/blueprints/genes/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/institutes/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       65 2019-03-13 11:41:36.000000 scout-browser-4.8.3/scout/server/blueprints/institutes/__init__.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/institutes/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/institutes/templates/overview/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1547 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/institutes/templates/overview/institutes.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1491 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/institutes/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/login/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       52 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/login/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1034 2019-03-25 14:01:02.000000 scout-browser-4.8.3/scout/server/blueprints/login/controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      689 2019-11-12 17:23:36.000000 scout-browser-4.8.3/scout/server/blueprints/login/models.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/login/static/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   195476 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/login/static/commander.svg
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)   415421 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/login/static/commissioner.svg
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2022 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/login/static/constable.svg
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    29283 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/login/static/inspector.svg
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3007 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/login/static/sergeant.svg
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    99307 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/login/static/superintendent.svg
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/login/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/login/templates/login/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1709 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/login/templates/login/users.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5013 2019-11-12 17:23:36.000000 scout-browser-4.8.3/scout/server/blueprints/login/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/panels/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       53 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/panels/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5108 2019-09-13 11:44:52.000000 scout-browser-4.8.3/scout/server/blueprints/panels/controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      631 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/panels/forms.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/panels/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/panels/templates/panels/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3354 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/panels/templates/panels/gene-edit.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     9873 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/panels/templates/panels/panel.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2538 2019-03-13 11:41:37.000000 scout-browser-4.8.3/scout/server/blueprints/panels/templates/panels/panel_pdf_simple.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7267 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/panels/templates/panels/panels.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8189 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/panels/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/blueprints/phenotypes/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       50 2019-03-13 11:41:37.000000 scout-browser-4.8.3/scout/server/blueprints/phenotypes/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      381 2019-11-06 07:56:32.000000 scout-browser-4.8.3/scout/server/blueprints/phenotypes/controllers.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/phenotypes/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/blueprints/phenotypes/templates/phenotypes/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1829 2019-11-06 07:56:32.000000 scout-browser-4.8.3/scout/server/blueprints/phenotypes/templates/phenotypes/hpo_terms.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      524 2019-11-06 07:56:32.000000 scout-browser-4.8.3/scout/server/blueprints/phenotypes/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/blueprints/public/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       53 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/public/__init__.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/blueprints/public/static/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    21794 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/public/static/logo-karolinska.png
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    19202 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/public/static/logo-scilifelab.png
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3784 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/public/static/scout-logo.png
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    41358 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/public/static/swedac.png
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/public/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/blueprints/public/templates/public/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2513 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/public/templates/public/index.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      785 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/blueprints/public/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/blueprints/variant/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       54 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/blueprints/variant/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    12743 2019-11-13 13:45:51.000000 scout-browser-4.8.3/scout/server/blueprints/variant/controllers.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/variant/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4525 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/acmg.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    47744 2019-11-05 13:28:01.000000 scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/clinvar.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    27711 2019-11-13 13:45:51.000000 scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/sv-variant.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1401 2019-11-07 14:49:58.000000 scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/utils.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    52626 2019-11-07 14:51:35.000000 scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/variant.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    16427 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/blueprints/variant/utils.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     9140 2019-11-13 13:45:51.000000 scout-browser-4.8.3/scout/server/blueprints/variant/verification_controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11185 2019-11-13 13:45:51.000000 scout-browser-4.8.3/scout/server/blueprints/variant/views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/blueprints/variants/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       55 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/blueprints/variants/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    19198 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/server/blueprints/variants/controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4682 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/server/blueprints/variants/forms.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/blueprints/variants/templates/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6358 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/cancer-variants.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3154 2019-11-04 10:01:16.000000 scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/components.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6701 2019-10-29 11:17:25.000000 scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/str-variants.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7839 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/sv-variants.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    19363 2019-11-12 17:23:36.000000 scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/utils.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    10198 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/variants.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1345 2019-10-29 07:47:13.000000 scout-browser-4.8.3/scout/server/blueprints/variants/utils.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    16435 2019-11-04 09:34:48.000000 scout-browser-4.8.3/scout/server/blueprints/variants/views.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1334 2019-11-13 13:45:51.000000 scout-browser-4.8.3/scout/server/config.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1942 2019-11-13 13:45:51.000000 scout-browser-4.8.3/scout/server/extensions.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11405 2019-11-12 17:23:36.000000 scout-browser-4.8.3/scout/server/links.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/static/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5561 2019-11-07 09:08:38.000000 scout-browser-4.8.3/scout/server/static/bs4_styles.css
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1469 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/static/favicon.ico
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      259 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/static/humans.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      106 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/static/robots.txt
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/templates/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1218 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/templates/bootstrap4.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3652 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/server/templates/layout_bs4.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      838 2019-03-05 14:41:11.000000 scout-browser-4.8.3/scout/server/templates/report_base.html
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4672 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/templates/utils.html
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/translations/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout/server/translations/sv/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/server/translations/sv/LC_MESSAGES/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4452 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4531 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/translations/sv/LC_MESSAGES/messages.po
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1282 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/server/userpanel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4936 2019-10-27 12:21:15.000000 scout-browser-4.8.3/scout/server/utils.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/update/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)        0 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/update/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1455 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/update/panel.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout/utils/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       24 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/utils/__init__.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6856 2019-10-08 10:56:44.000000 scout-browser-4.8.3/scout/utils/acmg.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      823 2019-06-12 08:58:45.000000 scout-browser-4.8.3/scout/utils/algorithms.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      701 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/utils/convert.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1183 2019-09-02 09:39:15.000000 scout-browser-4.8.3/scout/utils/coordinates.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1377 2019-03-13 11:41:37.000000 scout-browser-4.8.3/scout/utils/date.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8762 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/utils/ensembl_rest_clients.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      581 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/utils/gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      330 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/utils/handle.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7801 2019-10-23 12:24:42.000000 scout-browser-4.8.3/scout/utils/link.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2458 2019-05-03 10:43:18.000000 scout-browser-4.8.3/scout/utils/matchmaker.py
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)      636 2018-06-15 11:15:21.000000 scout-browser-4.8.3/scout/utils/md5.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    10260 2019-09-12 09:53:57.000000 scout-browser-4.8.3/scout/utils/requests.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/scout_browser.egg-info/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     9363 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout_browser.egg-info/PKG-INFO
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    20513 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout_browser.egg-info/SOURCES.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)        1 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout_browser.egg-info/dependency_links.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)       46 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout_browser.egg-info/entry_points.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)        1 2017-01-23 11:48:46.000000 scout-browser-4.8.3/scout_browser.egg-info/not-zip-safe
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      469 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout_browser.egg-info/requires.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)        6 2019-11-13 13:47:23.000000 scout-browser-4.8.3/scout_browser.egg-info/top_level.txt
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      129 2019-11-13 13:47:24.000000 scout-browser-4.8.3/setup.cfg
--rwxr-xr-x   0 mansmagnusson  (3001) staff       (20)     3911 2019-09-13 11:48:24.000000 scout-browser-4.8.3/setup.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/adapter/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2189 2019-11-04 09:34:48.000000 scout-browser-4.8.3/tests/adapter/conftest.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/adapter/mongo/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2516 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/adapter/mongo/test_adapter_variant_caseid.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    19887 2019-11-05 16:39:07.000000 scout-browser-4.8.3/tests/adapter/mongo/test_case_handling.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8013 2019-08-20 07:16:43.000000 scout-browser-4.8.3/tests/adapter/mongo/test_clinvar_handler.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6984 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/adapter/mongo/test_comment_handling.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1208 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/adapter/mongo/test_connect.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5929 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/adapter/mongo/test_evaluated_variants.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    19887 2019-11-04 09:34:48.000000 scout-browser-4.8.3/tests/adapter/mongo/test_event_handling.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    12795 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/adapter/mongo/test_gene_handler.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     9603 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/adapter/mongo/test_hpo_handler.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1440 2018-10-09 07:36:29.000000 scout-browser-4.8.3/tests/adapter/mongo/test_index_handling.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5834 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/adapter/mongo/test_institute_handler.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1510 2019-03-25 14:01:02.000000 scout-browser-4.8.3/tests/adapter/mongo/test_load_adapter_case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1782 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/adapter/mongo/test_matchmaker.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    10448 2019-10-29 11:17:17.000000 scout-browser-4.8.3/tests/adapter/mongo/test_panel_handler.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    25093 2019-10-25 13:13:21.000000 scout-browser-4.8.3/tests/adapter/mongo/test_query.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     6181 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/adapter/mongo/test_sanger_validation.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     9562 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/adapter/mongo/test_transcript_handler.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)        0 2019-03-13 11:41:37.000000 scout-browser-4.8.3/tests/adapter/mongo/test_update_synopsis
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4461 2019-11-06 12:40:59.000000 scout-browser-4.8.3/tests/adapter/mongo/test_user_handling.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11004 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/adapter/mongo/test_variant_events.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7787 2019-10-23 12:23:24.000000 scout-browser-4.8.3/tests/adapter/mongo/test_variant_handling.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1194 2019-10-29 07:28:17.000000 scout-browser-4.8.3/tests/adapter/mongo/test_variant_loader.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/build/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1128 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/build/conftest.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4289 2019-11-04 09:34:48.000000 scout-browser-4.8.3/tests/build/test_build_case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1350 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/build/test_build_clnsig.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      951 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/build/test_build_disease.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      638 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/build/test_build_exon.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3617 2019-08-29 07:04:29.000000 scout-browser-4.8.3/tests/build/test_build_gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1520 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/build/test_build_hgnc_gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      449 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/build/test_build_hgnc_transcript.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      529 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/build/test_build_hpo.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8306 2019-08-29 07:04:29.000000 scout-browser-4.8.3/tests/build/test_build_individual.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      868 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/build/test_build_institute.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3724 2019-09-12 09:27:32.000000 scout-browser-4.8.3/tests/build/test_build_panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      454 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/build/test_build_user.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5891 2019-09-09 13:20:04.000000 scout-browser-4.8.3/tests/build/test_build_variant.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/commands/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      878 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/commands/conftest.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/commands/delete/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11929 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/commands/delete/test_delete_cmd.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/commands/export/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4603 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/export/test_export_cases_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2113 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/export/test_export_gene.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1407 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/export/test_export_hpo_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1468 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/export/test_export_mt_report_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2456 2019-08-20 07:16:43.000000 scout-browser-4.8.3/tests/commands/export/test_export_panel_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1744 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/export/test_export_transcripts_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     5153 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/export/test_export_variant_cmd.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/commands/load/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2475 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/load/test_load_case_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      641 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/load/test_load_delivery_report_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      429 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/load/test_load_exons_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      951 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/load/test_load_institute_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      742 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/load/test_load_panel_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      770 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/load/test_load_region_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      813 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/load/test_load_research_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      937 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/load/test_load_user_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4507 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/commands/load/test_load_variants_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1056 2019-08-20 07:16:43.000000 scout-browser-4.8.3/tests/commands/test_base_command.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1019 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/test_convert_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1480 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/commands/test_delete_case_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      895 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/test_index_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      367 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/test_serve_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1070 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/commands/test_setup_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      499 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/test_wipe_database.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/commands/update/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8117 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/update/test_update_case_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      951 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/update/test_update_compounds_cli.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      809 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/update/test_update_disease_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      488 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/commands/update/test_update_genes_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3147 2019-09-02 09:39:15.000000 scout-browser-4.8.3/tests/commands/update/test_update_groups_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1165 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/commands/update/test_update_hpo_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3004 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/update/test_update_institute_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      832 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/update/test_update_omim_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1144 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/update/test_update_panel_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2076 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/update/test_update_user_cmd.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/commands/view/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      842 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/view/test_panels_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1299 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/view/test_view_aliases_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4152 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/view/test_view_cases.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2562 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/view/test_view_cases_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      496 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/view/test_view_collections_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      993 2019-09-02 09:39:15.000000 scout-browser-4.8.3/tests/commands/view/test_view_diseases_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      898 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/view/test_view_hgnc.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1731 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/view/test_view_hpo_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      830 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/view/test_view_index_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2439 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/view/test_view_individuals_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1450 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/view/test_view_institutes_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      966 2019-06-12 08:58:45.000000 scout-browser-4.8.3/tests/commands/view/test_view_intervals_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2319 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/view/test_view_transcripts_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      419 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/commands/view/test_view_users_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      740 2019-09-02 09:39:15.000000 scout-browser-4.8.3/tests/commands/view/test_view_whitelist_cmd.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    42040 2019-10-29 11:17:25.000000 scout-browser-4.8.3/tests/conftest.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/export/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3696 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/export/test_export_variants.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/tests/fixtures/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/fixtures/peds/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      157 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/fixtures/peds/clinvar.ped
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/fixtures/vcfs/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    72169 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/fixtures/vcfs/clinvar.vcf
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    72169 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/fixtures/vcfs/no_clinvar.vcf
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/load/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      839 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/load/test_load_case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      966 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/load/test_load_exons.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3384 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/load/test_load_hgnc_genes.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2382 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/load/test_load_hpo.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      666 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/load/test_load_institute.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      709 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/load/test_load_panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2160 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/load/test_load_report.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      713 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/load/test_load_transcripts.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11403 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/load/test_load_variant.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      441 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/load/test_setup_scout.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/parse/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      444 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/parse/conftest.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4001 2019-09-09 13:20:04.000000 scout-browser-4.8.3/tests/parse/test_frequency.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2179 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_ids.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4133 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_callers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11233 2019-11-07 09:08:38.000000 scout-browser-4.8.3/tests/parse/test_parse_case.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2267 2019-11-04 09:34:48.000000 scout-browser-4.8.3/tests/parse/test_parse_clinvar_form.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8167 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/parse/test_parse_clnsig.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1653 2019-03-13 11:41:37.000000 scout-browser-4.8.3/tests/parse/test_parse_compounds.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1387 2019-03-25 14:01:02.000000 scout-browser-4.8.3/tests/parse/test_parse_conservation.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7279 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_coordinates.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     7884 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/parse/test_parse_ensembl_exons.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2262 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/parse/test_parse_ensembl_transcripts.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      517 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_exac_genes.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2887 2019-03-13 11:41:37.000000 scout-browser-4.8.3/tests/parse/test_parse_genes.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2310 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_genotype.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1451 2019-03-13 11:41:37.000000 scout-browser-4.8.3/tests/parse/test_parse_headers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      569 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_hgnc.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3006 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_hpo_disease.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      503 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_hpo_genes.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2574 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_hpo_terms.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1287 2019-05-03 10:43:18.000000 scout-browser-4.8.3/tests/parse/test_parse_match_matchmaker.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4215 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_omim.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     9161 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/test_parse_panel.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1286 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/parse/test_parse_rank_score.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8458 2019-09-09 13:20:04.000000 scout-browser-4.8.3/tests/parse/test_parse_transcripts.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3068 2019-10-29 11:17:25.000000 scout-browser-4.8.3/tests/parse/test_parse_variant.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/parse/vcfs/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    21658 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/parse/vcfs/one_cnvnator.vcf
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:23.000000 scout-browser-4.8.3/tests/server/blueprints/
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/cases/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3491 2019-11-05 13:28:01.000000 scout-browser-4.8.3/tests/server/blueprints/cases/test_cases_controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    15574 2019-10-02 09:01:23.000000 scout-browser-4.8.3/tests/server/blueprints/cases/test_cases_views.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      610 2019-05-03 10:43:18.000000 scout-browser-4.8.3/tests/server/blueprints/cases/test_cases_views_gene_variants.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8359 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/server/blueprints/cases/test_matchmaker_controllers.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/dashboard/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3794 2019-03-25 14:01:02.000000 scout-browser-4.8.3/tests/server/blueprints/dashboard/test_dashboard_controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      970 2019-05-03 10:43:18.000000 scout-browser-4.8.3/tests/server/blueprints/dashboard/test_dashboard_views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/genes/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1689 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/server/blueprints/genes/test_genes_views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/institutes/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      524 2019-05-03 10:43:18.000000 scout-browser-4.8.3/tests/server/blueprints/institutes/test_institutes_views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/login/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      278 2019-11-12 17:23:36.000000 scout-browser-4.8.3/tests/server/blueprints/login/test_models.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2097 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/server/blueprints/login/test_views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/panels/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4231 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/server/blueprints/panels/test_panels_views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/phenotypes/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      578 2019-11-06 07:56:32.000000 scout-browser-4.8.3/tests/server/blueprints/phenotypes/test_phenotypes_controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1385 2019-05-03 10:43:18.000000 scout-browser-4.8.3/tests/server/blueprints/phenotypes/test_phenotypes_views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/public/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      369 2019-05-03 10:43:18.000000 scout-browser-4.8.3/tests/server/blueprints/public/test_public_views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/variant/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     8792 2019-11-05 16:39:07.000000 scout-browser-4.8.3/tests/server/blueprints/variant/test_variant_controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    22533 2019-10-27 12:21:15.000000 scout-browser-4.8.3/tests/server/blueprints/variant/test_variant_utils.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2485 2019-10-27 12:21:15.000000 scout-browser-4.8.3/tests/server/blueprints/variant/test_variant_verification_controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3715 2019-11-04 09:34:48.000000 scout-browser-4.8.3/tests/server/blueprints/variant/test_variant_views.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/server/blueprints/variants/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)        0 2019-10-27 12:21:15.000000 scout-browser-4.8.3/tests/server/blueprints/variants/conftest.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1480 2019-10-27 12:21:15.000000 scout-browser-4.8.3/tests/server/blueprints/variants/test_variants_controllers.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1186 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/server/blueprints/variants/test_variants_utils.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4420 2019-11-04 09:34:48.000000 scout-browser-4.8.3/tests/server/blueprints/variants/test_variants_views.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    23784 2019-11-13 13:45:51.000000 scout-browser-4.8.3/tests/server/conftest.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      822 2019-11-12 17:23:36.000000 scout-browser-4.8.3/tests/server/test_links.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      342 2019-10-27 12:21:15.000000 scout-browser-4.8.3/tests/server/test_server_utils.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/update/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3452 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/update/test_update_compounds.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      666 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/update/test_update_institute.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4206 2019-09-26 07:27:50.000000 scout-browser-4.8.3/tests/update/test_update_panel.py
-drwxr-xr-x   0 mansmagnusson  (3001) staff       (20)        0 2019-11-13 13:47:24.000000 scout-browser-4.8.3/tests/utils/
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)    11244 2019-10-07 07:11:42.000000 scout-browser-4.8.3/tests/utils/test_acmg.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1933 2019-06-14 10:29:35.000000 scout-browser-4.8.3/tests/utils/test_algorithms.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     3661 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/utils/test_convert.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)      844 2018-06-15 11:15:21.000000 scout-browser-4.8.3/tests/utils/test_date.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     4624 2019-09-12 09:53:57.000000 scout-browser-4.8.3/tests/utils/test_ensembl_rest_clients.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     2841 2019-10-23 12:24:42.000000 scout-browser-4.8.3/tests/utils/test_link_genes.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1300 2019-09-02 09:39:15.000000 scout-browser-4.8.3/tests/utils/test_par.py
--rw-r--r--   0 mansmagnusson  (3001) staff       (20)     1480 2019-09-09 13:20:39.000000 scout-browser-4.8.3/tests/utils/test_requests.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/
+-rw-r--r--   0 dannil     (501) staff       (20)    10399 2019-11-27 07:45:41.000000 scout-browser-4.9.0/PKG-INFO
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout_browser.egg-info/
+-rw-r--r--   0 dannil     (501) staff       (20)    10399 2019-11-27 07:45:40.000000 scout-browser-4.9.0/scout_browser.egg-info/PKG-INFO
+-rw-r--r--   0 dannil     (501) staff       (20)        1 2019-10-07 09:23:56.000000 scout-browser-4.9.0/scout_browser.egg-info/not-zip-safe
+-rw-r--r--   0 dannil     (501) staff       (20)    24768 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout_browser.egg-info/SOURCES.txt
+-rw-r--r--   0 dannil     (501) staff       (20)       46 2019-11-27 07:45:40.000000 scout-browser-4.9.0/scout_browser.egg-info/entry_points.txt
+-rw-r--r--   0 dannil     (501) staff       (20)      469 2019-11-27 07:45:40.000000 scout-browser-4.9.0/scout_browser.egg-info/requires.txt
+-rw-r--r--   0 dannil     (501) staff       (20)        6 2019-11-27 07:45:40.000000 scout-browser-4.9.0/scout_browser.egg-info/top_level.txt
+-rw-r--r--   0 dannil     (501) staff       (20)        1 2019-11-27 07:45:40.000000 scout-browser-4.9.0/scout_browser.egg-info/dependency_links.txt
+-rw-r--r--   0 dannil     (501) staff       (20)     1485 2019-10-07 06:32:17.000000 scout-browser-4.9.0/LICENSE
+-rw-r--r--   0 dannil     (501) staff       (20)      574 2019-11-20 12:53:08.000000 scout-browser-4.9.0/requirements.txt
+-rw-r--r--   0 dannil     (501) staff       (20)    20402 2019-11-27 07:44:37.000000 scout-browser-4.9.0/CHANGELOG.md
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/
+-rw-r--r--   0 dannil     (501) staff       (20)    42040 2019-11-22 10:10:32.000000 scout-browser-4.9.0/tests/conftest.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/update/
+-rw-r--r--   0 dannil     (501) staff       (20)     4206 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/update/test_update_panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)      666 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/update/test_update_institute.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3452 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/update/test_update_compounds.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/parse/
+-rw-r--r--   0 dannil     (501) staff       (20)      444 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/conftest.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8458 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_transcripts.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/parse/vcfs/
+-rw-r--r--   0 dannil     (501) staff       (20)    21658 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/vcfs/one_cnvnator.vcf
+-rw-r--r--   0 dannil     (501) staff       (20)      517 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_exac_genes.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2887 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_genes.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1287 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_match_matchmaker.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2574 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_hpo_terms.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2262 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_ensembl_transcripts.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1653 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_compounds.py
+-rw-r--r--   0 dannil     (501) staff       (20)     9161 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2267 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/parse/test_parse_clinvar_form.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4133 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_callers.py
+-rw-r--r--   0 dannil     (501) staff       (20)    11233 2019-11-20 13:10:43.000000 scout-browser-4.9.0/tests/parse/test_parse_case.py
+-rw-r--r--   0 dannil     (501) staff       (20)     7884 2019-10-25 12:59:17.000000 scout-browser-4.9.0/tests/parse/test_parse_ensembl_exons.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1286 2019-10-25 12:59:17.000000 scout-browser-4.9.0/tests/parse/test_parse_rank_score.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2179 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_ids.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4001 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_frequency.py
+-rw-r--r--   0 dannil     (501) staff       (20)      569 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_hgnc.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2310 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_genotype.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8167 2019-10-11 12:26:50.000000 scout-browser-4.9.0/tests/parse/test_parse_clnsig.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1387 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_conservation.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3068 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/parse/test_parse_variant.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3006 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_hpo_disease.py
+-rw-r--r--   0 dannil     (501) staff       (20)     7279 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_coordinates.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1451 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_headers.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4215 2019-11-27 07:44:37.000000 scout-browser-4.9.0/tests/parse/test_parse_omim.py
+-rw-r--r--   0 dannil     (501) staff       (20)      503 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/parse/test_parse_hpo_genes.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/
+-rw-r--r--   0 dannil     (501) staff       (20)    23784 2019-11-20 13:42:32.000000 scout-browser-4.9.0/tests/server/conftest.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/variants/
+-rw-r--r--   0 dannil     (501) staff       (20)     1796 2019-11-22 10:10:32.000000 scout-browser-4.9.0/tests/server/blueprints/variants/test_variants_utils.py
+-rw-r--r--   0 dannil     (501) staff       (20)        0 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/server/blueprints/variants/conftest.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1480 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/server/blueprints/variants/test_variants_controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)     6002 2019-11-22 10:10:32.000000 scout-browser-4.9.0/tests/server/blueprints/variants/test_variants_views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/phenotypes/
+-rw-r--r--   0 dannil     (501) staff       (20)     1385 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/server/blueprints/phenotypes/test_phenotypes_views.py
+-rw-r--r--   0 dannil     (501) staff       (20)      578 2019-11-20 13:10:43.000000 scout-browser-4.9.0/tests/server/blueprints/phenotypes/test_phenotypes_controllers.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/panels/
+-rw-r--r--   0 dannil     (501) staff       (20)     4915 2019-11-22 10:10:32.000000 scout-browser-4.9.0/tests/server/blueprints/panels/test_panels_views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/cases/
+-rw-r--r--   0 dannil     (501) staff       (20)      610 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/server/blueprints/cases/test_cases_views_gene_variants.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8359 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/server/blueprints/cases/test_matchmaker_controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)    17993 2019-11-20 13:35:09.000000 scout-browser-4.9.0/tests/server/blueprints/cases/test_cases_views.py.suggestion
+-rw-r--r--   0 dannil     (501) staff       (20)     4455 2019-11-27 07:43:41.000000 scout-browser-4.9.0/tests/server/blueprints/cases/test_cases_controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)    15574 2019-11-20 13:42:32.000000 scout-browser-4.9.0/tests/server/blueprints/cases/test_cases_views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/institutes/
+-rw-r--r--   0 dannil     (501) staff       (20)      524 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/server/blueprints/institutes/test_institutes_views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/dashboard/
+-rw-r--r--   0 dannil     (501) staff       (20)      970 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/server/blueprints/dashboard/test_dashboard_views.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3794 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/server/blueprints/dashboard/test_dashboard_controllers.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/public/
+-rw-r--r--   0 dannil     (501) staff       (20)      369 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/server/blueprints/public/test_public_views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/variant/
+-rw-r--r--   0 dannil     (501) staff       (20)    22533 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/server/blueprints/variant/test_variant_utils.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2485 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/server/blueprints/variant/test_variant_verification_controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3715 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/server/blueprints/variant/test_variant_views.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8792 2019-11-20 13:10:43.000000 scout-browser-4.9.0/tests/server/blueprints/variant/test_variant_controllers.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/genes/
+-rw-r--r--   0 dannil     (501) staff       (20)     1689 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/server/blueprints/genes/test_genes_views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/server/blueprints/login/
+-rw-r--r--   0 dannil     (501) staff       (20)     2544 2019-11-22 10:10:32.000000 scout-browser-4.9.0/tests/server/blueprints/login/test_views.py
+-rw-r--r--   0 dannil     (501) staff       (20)      278 2019-11-20 13:10:43.000000 scout-browser-4.9.0/tests/server/blueprints/login/test_models.py
+-rw-r--r--   0 dannil     (501) staff       (20)      342 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/server/test_server_utils.py
+-rw-r--r--   0 dannil     (501) staff       (20)      822 2019-11-22 10:10:32.000000 scout-browser-4.9.0/tests/server/test_links.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/utils/
+-rw-r--r--   0 dannil     (501) staff       (20)    11244 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/utils/test_acmg.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2841 2019-10-25 12:59:17.000000 scout-browser-4.9.0/tests/utils/test_link_genes.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3661 2019-10-12 12:57:32.000000 scout-browser-4.9.0/tests/utils/test_convert.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4624 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/utils/test_ensembl_rest_clients.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1300 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/utils/test_par.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1480 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/utils/test_requests.py
+-rw-r--r--   0 dannil     (501) staff       (20)      844 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/utils/test_date.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1933 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/utils/test_algorithms.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/adapter/
+-rw-r--r--   0 dannil     (501) staff       (20)     2189 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/adapter/conftest.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/adapter/mongo/
+-rw-r--r--   0 dannil     (501) staff       (20)    21319 2019-11-22 10:10:32.000000 scout-browser-4.9.0/tests/adapter/mongo/test_case_handling.py
+-rw-r--r--   0 dannil     (501) staff       (20)     9603 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_hpo_handler.py
+-rw-r--r--   0 dannil     (501) staff       (20)     6984 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_comment_handling.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1208 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_connect.py
+-rw-r--r--   0 dannil     (501) staff       (20)        0 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_update_synopsis
+-rw-r--r--   0 dannil     (501) staff       (20)     1440 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_index_handling.py
+-rw-r--r--   0 dannil     (501) staff       (20)    10448 2019-10-14 11:01:32.000000 scout-browser-4.9.0/tests/adapter/mongo/test_panel_handler.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1194 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/adapter/mongo/test_variant_loader.py
+-rw-r--r--   0 dannil     (501) staff       (20)     9562 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_transcript_handler.py
+-rw-r--r--   0 dannil     (501) staff       (20)     7787 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_variant_handling.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5834 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_institute_handler.py
+-rw-r--r--   0 dannil     (501) staff       (20)    12795 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_gene_handler.py
+-rw-r--r--   0 dannil     (501) staff       (20)    11004 2019-11-27 07:43:41.000000 scout-browser-4.9.0/tests/adapter/mongo/test_variant_events.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2516 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_adapter_variant_caseid.py
+-rw-r--r--   0 dannil     (501) staff       (20)     6181 2019-10-11 12:26:50.000000 scout-browser-4.9.0/tests/adapter/mongo/test_sanger_validation.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8013 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_clinvar_handler.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1782 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_matchmaker.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4461 2019-11-20 13:10:43.000000 scout-browser-4.9.0/tests/adapter/mongo/test_user_handling.py
+-rw-r--r--   0 dannil     (501) staff       (20)    19887 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/adapter/mongo/test_event_handling.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5929 2019-11-27 07:43:41.000000 scout-browser-4.9.0/tests/adapter/mongo/test_evaluated_variants.py
+-rw-r--r--   0 dannil     (501) staff       (20)    25093 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/adapter/mongo/test_query.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1510 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/adapter/mongo/test_load_adapter_case.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/load/
+-rw-r--r--   0 dannil     (501) staff       (20)     2382 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/load/test_load_hpo.py
+-rw-r--r--   0 dannil     (501) staff       (20)      713 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/load/test_load_transcripts.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2160 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/load/test_load_report.py
+-rw-r--r--   0 dannil     (501) staff       (20)      966 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/load/test_load_exons.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3384 2019-10-25 12:59:17.000000 scout-browser-4.9.0/tests/load/test_load_hgnc_genes.py
+-rw-r--r--   0 dannil     (501) staff       (20)      839 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/load/test_load_case.py
+-rw-r--r--   0 dannil     (501) staff       (20)    11403 2019-10-11 12:26:50.000000 scout-browser-4.9.0/tests/load/test_load_variant.py
+-rw-r--r--   0 dannil     (501) staff       (20)      441 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/load/test_setup_scout.py
+-rw-r--r--   0 dannil     (501) staff       (20)      709 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/load/test_load_panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)      666 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/load/test_load_institute.py
+-rw-r--r--   0 dannil     (501) staff       (20)    16374 2019-10-31 10:00:04.000000 scout-browser-4.9.0/tests/test_protocol.md
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/fixtures/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/fixtures/vcfs/
+-rw-r--r--   0 dannil     (501) staff       (20)    72169 2019-10-11 12:26:50.000000 scout-browser-4.9.0/tests/fixtures/vcfs/no_clinvar.vcf
+-rw-r--r--   0 dannil     (501) staff       (20)    72169 2019-10-11 12:26:50.000000 scout-browser-4.9.0/tests/fixtures/vcfs/clinvar.vcf
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/fixtures/peds/
+-rw-r--r--   0 dannil     (501) staff       (20)      157 2019-10-11 12:26:50.000000 scout-browser-4.9.0/tests/fixtures/peds/clinvar.ped
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/commands/
+-rw-r--r--   0 dannil     (501) staff       (20)     1019 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/test_convert_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      878 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/conftest.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1480 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/test_delete_case_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      367 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/test_serve_cmd.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/commands/update/
+-rw-r--r--   0 dannil     (501) staff       (20)      488 2019-10-25 12:59:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_genes_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2076 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_user_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8117 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_case_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3147 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_groups_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3004 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_institute_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      809 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_disease_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      832 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_omim_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      951 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_compounds_cli.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1165 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_hpo_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1144 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/update/test_update_panel_cmd.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/commands/delete/
+-rw-r--r--   0 dannil     (501) staff       (20)    11929 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/delete/test_delete_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      895 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/test_index_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1056 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/test_base_command.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/commands/load/
+-rw-r--r--   0 dannil     (501) staff       (20)     4507 2019-10-11 12:26:50.000000 scout-browser-4.9.0/tests/commands/load/test_load_variants_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      937 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/load/test_load_user_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2475 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/load/test_load_case_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      429 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/load/test_load_exons_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      975 2019-11-22 10:10:32.000000 scout-browser-4.9.0/tests/commands/load/test_load_institute_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      742 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/load/test_load_panel_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      813 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/load/test_load_research_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      770 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/load/test_load_region_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      641 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/load/test_load_delivery_report_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1070 2019-10-25 12:59:17.000000 scout-browser-4.9.0/tests/commands/test_setup_cmd.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/commands/view/
+-rw-r--r--   0 dannil     (501) staff       (20)      966 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_intervals_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      898 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_hgnc.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4152 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_cases.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1450 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_institutes_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2562 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_cases_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2319 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_transcripts_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      740 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_whitelist_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      842 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_panels_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1731 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_hpo_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2439 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_individuals_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1299 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_aliases_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      496 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_collections_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      419 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_users_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      830 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_index_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      993 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/view/test_view_diseases_cmd.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/commands/export/
+-rw-r--r--   0 dannil     (501) staff       (20)     5153 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/export/test_export_variant_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1407 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/export/test_export_hpo_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2113 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/export/test_export_gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1468 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/export/test_export_mt_report_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2456 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/export/test_export_panel_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4603 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/export/test_export_cases_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1744 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/export/test_export_transcripts_cmd.py
+-rw-r--r--   0 dannil     (501) staff       (20)      499 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/commands/test_wipe_database.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/build/
+-rw-r--r--   0 dannil     (501) staff       (20)     1128 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/conftest.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3617 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)      868 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_institute.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4289 2019-11-01 16:59:46.000000 scout-browser-4.9.0/tests/build/test_build_case.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1520 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_hgnc_gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8306 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_individual.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5891 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_variant.py
+-rw-r--r--   0 dannil     (501) staff       (20)      529 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_hpo.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3724 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)      638 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_exon.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1350 2019-10-11 12:26:50.000000 scout-browser-4.9.0/tests/build/test_build_clnsig.py
+-rw-r--r--   0 dannil     (501) staff       (20)      449 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_hgnc_transcript.py
+-rw-r--r--   0 dannil     (501) staff       (20)      951 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_disease.py
+-rw-r--r--   0 dannil     (501) staff       (20)      454 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/build/test_build_user.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/tests/export/
+-rw-r--r--   0 dannil     (501) staff       (20)     3696 2019-10-07 06:32:17.000000 scout-browser-4.9.0/tests/export/test_export_variants.py
+-rw-r--r--   0 dannil     (501) staff       (20)      636 2019-10-07 06:32:17.000000 scout-browser-4.9.0/MANIFEST.in
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/demo/
+-rw-r--r--   0 dannil     (501) staff       (20)     9854 2019-10-07 07:27:40.000000 scout-browser-4.9.0/scout/demo/cancer_test.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)   440072 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.research.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)     1700 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.clinical.str.annotated.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)     1808 2019-11-27 06:51:54.000000 scout-browser-4.9.0/scout/demo/643594.config.yaml
+-rw-r--r--   0 dannil     (501) staff       (20)     1695 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.clinical.str.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)       72 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/empty.clinical.SV.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)   409369 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643595.clinical.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)      421 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.peddy.ped
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/demo/images/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/demo/images/roh_images/
+-rw-r--r--   0 dannil     (501) staff       (20)     5545 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr20.png
+-rw-r--r--   0 dannil     (501) staff       (20)     3565 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr21.png
+-rw-r--r--   0 dannil     (501) staff       (20)     4026 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr22.png
+-rw-r--r--   0 dannil     (501) staff       (20)     5627 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr19.png
+-rw-r--r--   0 dannil     (501) staff       (20)     6170 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr18.png
+-rw-r--r--   0 dannil     (501) staff       (20)      707 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chrM.png
+-rw-r--r--   0 dannil     (501) staff       (20)    10679 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr8.png
+-rw-r--r--   0 dannil     (501) staff       (20)     1729 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chrY.png
+-rw-r--r--   0 dannil     (501) staff       (20)    11245 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chrX.png
+-rw-r--r--   0 dannil     (501) staff       (20)    10252 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr9.png
+-rw-r--r--   0 dannil     (501) staff       (20)    16701 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr2.png
+-rw-r--r--   0 dannil     (501) staff       (20)    13367 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr3.png
+-rw-r--r--   0 dannil     (501) staff       (20)    16839 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr1.png
+-rw-r--r--   0 dannil     (501) staff       (20)    12688 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr4.png
+-rw-r--r--   0 dannil     (501) staff       (20)    12397 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr5.png
+-rw-r--r--   0 dannil     (501) staff       (20)    11976 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr7.png
+-rw-r--r--   0 dannil     (501) staff       (20)    12150 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr6.png
+-rw-r--r--   0 dannil     (501) staff       (20)     7217 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr15.png
+-rw-r--r--   0 dannil     (501) staff       (20)     7120 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr14.png
+-rw-r--r--   0 dannil     (501) staff       (20)     7235 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr16.png
+-rw-r--r--   0 dannil     (501) staff       (20)     1873 2019-08-08 11:01:36.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr17.png
+-rw-r--r--   0 dannil     (501) staff       (20)     7287 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr13.png
+-rw-r--r--   0 dannil     (501) staff       (20)     7729 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr17 bak.png
+-rw-r--r--   0 dannil     (501) staff       (20)    10016 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr12.png
+-rw-r--r--   0 dannil     (501) staff       (20)    10706 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr10.png
+-rw-r--r--   0 dannil     (501) staff       (20)    10604 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/roh_images/roh_chr11.png
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/demo/images/upd_images/
+-rw-r--r--   0 dannil     (501) staff       (20)      473 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr21.png
+-rw-r--r--   0 dannil     (501) staff       (20)      530 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr20.png
+-rw-r--r--   0 dannil     (501) staff       (20)      526 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr22.png
+-rw-r--r--   0 dannil     (501) staff       (20)    14528 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chrcombined.png
+-rw-r--r--   0 dannil     (501) staff       (20)      593 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr9.png
+-rw-r--r--   0 dannil     (501) staff       (20)      569 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chrX.png
+-rw-r--r--   0 dannil     (501) staff       (20)      624 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr8.png
+-rw-r--r--   0 dannil     (501) staff       (20)      534 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr18.png
+-rw-r--r--   0 dannil     (501) staff       (20)   212037 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/test_upd.sites.bed.gz
+-rw-r--r--   0 dannil     (501) staff       (20)      564 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr19.png
+-rw-r--r--   0 dannil     (501) staff       (20)   972363 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/test_upd.sites.bed
+-rw-r--r--   0 dannil     (501) staff       (20)      558 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr14.png
+-rw-r--r--   0 dannil     (501) staff       (20)      674 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr6.png
+-rw-r--r--   0 dannil     (501) staff       (20)      668 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr7.png
+-rw-r--r--   0 dannil     (501) staff       (20)      567 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr15.png
+-rw-r--r--   0 dannil     (501) staff       (20)      555 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr17.png
+-rw-r--r--   0 dannil     (501) staff       (20)      649 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr5.png
+-rw-r--r--   0 dannil     (501) staff       (20)      663 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr4.png
+-rw-r--r--   0 dannil     (501) staff       (20)      547 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr16.png
+-rw-r--r--   0 dannil     (501) staff       (20)      624 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr12.png
+-rw-r--r--   0 dannil     (501) staff       (20)      760 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr1.png
+-rw-r--r--   0 dannil     (501) staff       (20)      517 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr13.png
+-rw-r--r--   0 dannil     (501) staff       (20)      624 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr11.png
+-rw-r--r--   0 dannil     (501) staff       (20)      705 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr3.png
+-rw-r--r--   0 dannil     (501) staff       (20)      734 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr2.png
+-rw-r--r--   0 dannil     (501) staff       (20)      614 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/upd_images/upd_chr10.png
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/demo/images/chr_images/
+-rw-r--r--   0 dannil     (501) staff       (20)      467 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr19.png
+-rw-r--r--   0 dannil     (501) staff       (20)      494 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr18.png
+-rw-r--r--   0 dannil     (501) staff       (20)      470 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr22.png
+-rw-r--r--   0 dannil     (501) staff       (20)      477 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr20.png
+-rw-r--r--   0 dannil     (501) staff       (20)      472 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr21.png
+-rw-r--r--   0 dannil     (501) staff       (20)      560 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr9.png
+-rw-r--r--   0 dannil     (501) staff       (20)      550 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chrX.png
+-rw-r--r--   0 dannil     (501) staff       (20)      447 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chrY.png
+-rw-r--r--   0 dannil     (501) staff       (20)      551 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr8.png
+-rw-r--r--   0 dannil     (501) staff       (20)      602 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr1.png
+-rw-r--r--   0 dannil     (501) staff       (20)      600 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr3.png
+-rw-r--r--   0 dannil     (501) staff       (20)      594 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr2.png
+-rw-r--r--   0 dannil     (501) staff       (20)      565 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr6.png
+-rw-r--r--   0 dannil     (501) staff       (20)      554 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr7.png
+-rw-r--r--   0 dannil     (501) staff       (20)      561 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr5.png
+-rw-r--r--   0 dannil     (501) staff       (20)      571 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr4.png
+-rw-r--r--   0 dannil     (501) staff       (20)      547 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr10.png
+-rw-r--r--   0 dannil     (501) staff       (20)      544 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr11.png
+-rw-r--r--   0 dannil     (501) staff       (20)      539 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr13.png
+-rw-r--r--   0 dannil     (501) staff       (20)      549 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr12.png
+-rw-r--r--   0 dannil     (501) staff       (20)      502 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr16.png
+-rw-r--r--   0 dannil     (501) staff       (20)      500 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr17.png
+-rw-r--r--   0 dannil     (501) staff       (20)      519 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr15.png
+-rw-r--r--   0 dannil     (501) staff       (20)      535 2019-08-02 12:17:00.000000 scout-browser-4.9.0/scout/demo/images/chr_images/cytoBand.txt.chr14.png
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/
+-rw-r--r--   0 dannil     (501) staff       (20)      233 2019-08-08 11:01:36.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/._roh_chr17.png
+-rw-r--r--   0 dannil     (501) staff       (20)      120 2019-08-08 11:06:07.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/._.DS_Store
+-rw-r--r--   0 dannil     (501) staff       (20)      233 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/._roh_chr12.png
+-rw-r--r--   0 dannil     (501) staff       (20)      233 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/._roh_chr2.png
+-rw-r--r--   0 dannil     (501) staff       (20)      233 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/._roh_chr1.png
+-rw-r--r--   0 dannil     (501) staff       (20)      177 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/._roh_chr6.png
+-rw-r--r--   0 dannil     (501) staff       (20)      233 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/._roh_chr17 bak.png
+-rw-r--r--   0 dannil     (501) staff       (20)      233 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/._roh_chr21.png
+-rw-r--r--   0 dannil     (501) staff       (20)      233 2019-08-05 06:37:00.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/roh_images/._roh_chr19.png
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/upd_images/
+-rw-r--r--   0 dannil     (501) staff       (20)      233 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/upd_images/._upd_chr1.png
+-rw-r--r--   0 dannil     (501) staff       (20)      824 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/upd_images/._test_upd.sites.bed.gz
+-rw-r--r--   0 dannil     (501) staff       (20)      174 2019-08-05 06:36:52.000000 scout-browser-4.9.0/scout/demo/images/__MACOSX/upd_images/._test_upd.sites.bed
+-rw-r--r--   0 dannil     (501) staff       (20)     1055 2019-10-07 07:27:40.000000 scout-browser-4.9.0/scout/demo/cancer_test.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)     1744 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.clinical.str.annotated.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)     1284 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.research.SV.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)    44596 2019-11-25 11:46:45.000000 scout-browser-4.9.0/scout/demo/test.bw
+-rw-r--r--   0 dannil     (501) staff       (20)      239 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.sex_check.csv
+-rw-r--r--   0 dannil     (501) staff       (20)     3813 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/empty.clinical.SV.vcf.gz
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/demo/resources/
+-rw-r--r--   0 dannil     (501) staff       (20)    10588 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/mim2gene_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)    54452 2019-11-27 07:44:37.000000 scout-browser-4.9.0/scout/demo/resources/genemap2_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)   321814 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_diseases_to_genes_to_phenotypes_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)   122488 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/hgnc_reduced_set.txt
+-rw-r--r--   0 dannil     (501) staff       (20)    80883 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/hpo_terms.csv
+-rw-r--r--   0 dannil     (501) staff       (20)     2566 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)  1152237 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/reduced.hpo.obo
+-rw-r--r--   0 dannil     (501) staff       (20)   888123 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_phenotype_to_genes_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)    12731 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/ensembl_genes_38_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)    64800 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/forweb_cleaned_exac_r03_march16_z_data_pLI_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)  1609018 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/ensembl_exons_37_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)   214557 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_genes_to_phenotype_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)   253991 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/ensembl_transcripts_38_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)     3536 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/chanjo4_structure.sql
+-rw-r--r--   0 dannil     (501) staff       (20)    12736 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/ensembl_genes_37_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)   150542 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/ensembl_transcripts_37_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)  1609018 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/resources/ensembl_exons_38_reduced.txt
+-rw-r--r--   0 dannil     (501) staff       (20)   408608 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.clinical.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)   997982 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/chanjo4_demo.sql
+-rw-r--r--   0 dannil     (501) staff       (20)    44596 2019-11-26 07:50:40.000000 scout-browser-4.9.0/scout/demo/test1.bw
+-rw-r--r--   0 dannil     (501) staff       (20)     7711 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.clinical.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)     7702 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.research.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)     1414 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/demo/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     7733 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643595.clinical.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)    11927 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.clinical.SV.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)      808 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/reduced_mt.bam.bai
+-rw-r--r--   0 dannil     (501) staff       (20)       36 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/cancer_test.ped
+-rw-r--r--   0 dannil     (501) staff       (20)   492247 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/reduced_mt.bam
+-rw-r--r--   0 dannil     (501) staff       (20)      154 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.ped
+-rw-r--r--   0 dannil     (501) staff       (20)  3273656 2019-11-25 15:57:10.000000 scout-browser-4.9.0/scout/demo/output.chrn.wig
+-rw-r--r--   0 dannil     (501) staff       (20)     6075 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/panel_1.csv
+-rw-r--r--   0 dannil     (501) staff       (20)       30 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/ADM1059A1.dummy.cgh
+-rw-r--r--   0 dannil     (501) staff       (20)      830 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/cancer.load_config.yaml
+-rw-r--r--   0 dannil     (501) staff       (20)    11927 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.research.SV.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)     5187 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/madeline.xml
+-rw-r--r--   0 dannil     (501) staff       (20)      445 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.ped_check.csv
+-rw-r--r--   0 dannil     (501) staff       (20)   225269 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/delivery_report.html
+-rw-r--r--   0 dannil     (501) staff       (20)  3273845 2019-11-26 11:33:33.000000 scout-browser-4.9.0/scout/demo/output.wig
+-rw-r--r--   0 dannil     (501) staff       (20)     1435 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643595.config.yaml
+-rw-r--r--   0 dannil     (501) staff       (20)     1284 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.clinical.SV.vcf.gz.tbi
+-rw-r--r--   0 dannil     (501) staff       (20)  3273575 2019-11-26 11:25:01.000000 scout-browser-4.9.0/scout/demo/output.wig.orig
+-rw-r--r--   0 dannil     (501) staff       (20)       30 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/ADM1059A2.dummy.cgh
+-rw-r--r--   0 dannil     (501) staff       (20)    44596 2019-11-26 07:50:42.000000 scout-browser-4.9.0/scout/demo/test2.bw
+-rw-r--r--   0 dannil     (501) staff       (20)   698187 2019-10-11 12:17:17.000000 scout-browser-4.9.0/scout/demo/ideo_upd_roh.zip
+-rw-r--r--   0 dannil     (501) staff       (20)     6145 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/panel_1.txt
+-rw-r--r--   0 dannil     (501) staff       (20)  2716069 2019-11-20 10:37:27.000000 scout-browser-4.9.0/scout/demo/643594.clinical.vcf
+-rw-r--r--   0 dannil     (501) staff       (20)     1941 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/demo/643594.clinical.str.annotated.limits.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)     1631 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/643594.clinical.str.vcf.gz
+-rw-r--r--   0 dannil     (501) staff       (20)       30 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/demo/ADM1059A3.dummy.cgh
+-rw-r--r--   0 dannil     (501) staff       (20)     1698 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/demo/643594.clinical.str.annotated.limits.vcf.gz.tbi
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/update/
+-rw-r--r--   0 dannil     (501) staff       (20)        0 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/update/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1455 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/update/panel.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/constants/
+-rw-r--r--   0 dannil     (501) staff       (20)     3274 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/constants/clinvar.py
+-rw-r--r--   0 dannil     (501) staff       (20)      723 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/constants/file_types.py
+-rw-r--r--   0 dannil     (501) staff       (20)      667 2019-10-14 11:01:31.000000 scout-browser-4.9.0/scout/constants/gene_tags.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3639 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/constants/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1251 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/constants/variants_export.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1178 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/constants/query_terms.py
+-rw-r--r--   0 dannil     (501) staff       (20)     7861 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/constants/acmg.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1126 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/constants/clnsig.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3873 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/constants/indexes.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3110 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/constants/so_terms.py
+-rw-r--r--   0 dannil     (501) staff       (20)     6187 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/constants/variant_tags.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2204 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/constants/case_tags.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1578 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/constants/phenotype.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/resources/
+-rw-r--r--   0 dannil     (501) staff       (20)     6264 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/resources/cytoBand.txt.gz
+-rw-r--r--   0 dannil     (501) staff       (20)      214 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/resources/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/parse/
+-rw-r--r--   0 dannil     (501) staff       (20)     5557 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/peddy.py
+-rw-r--r--   0 dannil     (501) staff       (20)     6895 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/clinvar.py
+-rw-r--r--   0 dannil     (501) staff       (20)    14740 2019-11-27 07:44:37.000000 scout-browser-4.9.0/scout/parse/omim.py
+-rw-r--r--   0 dannil     (501) staff       (20)        0 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3277 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/hgnc.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1465 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/exac.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8433 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/matchmaker.py
+-rw-r--r--   0 dannil     (501) staff       (20)     9192 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/parse/ensembl.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1871 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/cytoband.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/parse/variant/
+-rw-r--r--   0 dannil     (501) staff       (20)     6209 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/frequency.py
+-rw-r--r--   0 dannil     (501) staff       (20)      508 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/models.py
+-rw-r--r--   0 dannil     (501) staff       (20)     7607 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/parse/variant/transcript.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1365 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/callers.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)     6954 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/parse/variant/genotype.py
+-rw-r--r--   0 dannil     (501) staff       (20)      508 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/rank_score.py
+-rw-r--r--   0 dannil     (501) staff       (20)       34 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3873 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/parse/variant/clnsig.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1666 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/conservation.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)     1534 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/compound.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)     4266 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2678 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/ids.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1589 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/variant/headers.py
+-rw-r--r--   0 dannil     (501) staff       (20)      564 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/parse/variant/deleteriousness.py
+-rw-r--r--   0 dannil     (501) staff       (20)    10290 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/parse/variant/variant.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4962 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/parse/variant/coordinates.py
+-rw-r--r--   0 dannil     (501) staff       (20)    15158 2019-11-27 06:51:54.000000 scout-browser-4.9.0/scout/parse/case.py
+-rw-r--r--   0 dannil     (501) staff       (20)    13553 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)    10682 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/parse/hpo.py
+-rw-r--r--   0 dannil     (501) staff       (20)      124 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/variants/
+-rw-r--r--   0 dannil     (501) staff       (20)    19215 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/server/blueprints/variants/controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)       55 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/variants/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4764 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/server/blueprints/variants/forms.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/variants/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/
+-rw-r--r--   0 dannil     (501) staff       (20)    10328 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/variants.html
+-rw-r--r--   0 dannil     (501) staff       (20)     3154 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/components.html
+-rw-r--r--   0 dannil     (501) staff       (20)     6699 2019-11-27 06:51:54.000000 scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/str-variants.html
+-rw-r--r--   0 dannil     (501) staff       (20)    19478 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/utils.html
+-rw-r--r--   0 dannil     (501) staff       (20)     7997 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/sv-variants.html
+-rw-r--r--   0 dannil     (501) staff       (20)     6358 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/cancer-variants.html
+-rw-r--r--   0 dannil     (501) staff       (20)    16689 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/server/blueprints/variants/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/alignviewers/
+-rw-r--r--   0 dannil     (501) staff       (20)       59 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/alignviewers/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/alignviewers/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/alignviewers/templates/alignviewers/
+-rw-r--r--   0 dannil     (501) staff       (20)     3371 2019-11-27 06:51:54.000000 scout-browser-4.9.0/scout/server/blueprints/alignviewers/templates/alignviewers/igv_viewer.html
+-rw-r--r--   0 dannil     (501) staff       (20)     1956 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/alignviewers/partial.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4082 2019-11-27 06:51:54.000000 scout-browser-4.9.0/scout/server/blueprints/alignviewers/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/phenotypes/
+-rw-r--r--   0 dannil     (501) staff       (20)      381 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/server/blueprints/phenotypes/controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)       50 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/phenotypes/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/phenotypes/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/phenotypes/templates/phenotypes/
+-rw-r--r--   0 dannil     (501) staff       (20)     1829 2019-11-27 07:44:37.000000 scout-browser-4.9.0/scout/server/blueprints/phenotypes/templates/phenotypes/hpo_terms.html
+-rw-r--r--   0 dannil     (501) staff       (20)      524 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/server/blueprints/phenotypes/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/panels/
+-rw-r--r--   0 dannil     (501) staff       (20)     5108 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/panels/controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)       53 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/panels/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)      631 2019-10-14 11:01:31.000000 scout-browser-4.9.0/scout/server/blueprints/panels/forms.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/panels/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/panels/templates/panels/
+-rw-r--r--   0 dannil     (501) staff       (20)     2538 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/panels/templates/panels/panel_pdf_simple.html
+-rw-r--r--   0 dannil     (501) staff       (20)     3354 2019-10-14 11:01:31.000000 scout-browser-4.9.0/scout/server/blueprints/panels/templates/panels/gene-edit.html
+-rw-r--r--   0 dannil     (501) staff       (20)     7267 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/server/blueprints/panels/templates/panels/panels.html
+-rw-r--r--   0 dannil     (501) staff       (20)     9873 2019-10-30 10:27:03.000000 scout-browser-4.9.0/scout/server/blueprints/panels/templates/panels/panel.html
+-rw-r--r--   0 dannil     (501) staff       (20)     8189 2019-10-14 11:01:31.000000 scout-browser-4.9.0/scout/server/blueprints/panels/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/cases/
+-rw-r--r--   0 dannil     (501) staff       (20)    36044 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/server/blueprints/cases/controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)       52 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/cases/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1207 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/cases/forms.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/cases/static/
+-rw-r--r--   0 dannil     (501) staff       (20)     1175 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/cases/static/madeline.js
+-rw-r--r--   0 dannil     (501) staff       (20)     5187 2019-11-23 10:48:26.000000 scout-browser-4.9.0/scout/server/blueprints/cases/static/madeline.svg
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/
+-rw-r--r--   0 dannil     (501) staff       (20)    47531 2019-11-27 07:44:37.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/case.html
+-rw-r--r--   0 dannil     (501) staff       (20)      887 2019-10-30 10:27:03.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/index.html
+-rw-r--r--   0 dannil     (501) staff       (20)    14387 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/cases.html
+-rw-r--r--   0 dannil     (501) staff       (20)    14111 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/case_ideograms.html
+-rw-r--r--   0 dannil     (501) staff       (20)    14168 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/clinvar_submissions.html
+-rw-r--r--   0 dannil     (501) staff       (20)     1681 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/diseases.html
+-rw-r--r--   0 dannil     (501) staff       (20)    18189 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/collapsible_actionbar.html
+-rw-r--r--   0 dannil     (501) staff       (20)    43242 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/case_report.html
+-rw-r--r--   0 dannil     (501) staff       (20)     7227 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/gene_variants.html
+-rw-r--r--   0 dannil     (501) staff       (20)    11953 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/matchmaker.html
+-rw-r--r--   0 dannil     (501) staff       (20)     5697 2019-11-27 07:44:37.000000 scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/causatives.html
+-rw-r--r--   0 dannil     (501) staff       (20)    40885 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/server/blueprints/cases/views.py
+-rw-r--r--   0 dannil     (501) staff       (20)       24 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/institutes/
+-rw-r--r--   0 dannil     (501) staff       (20)       65 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/institutes/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/institutes/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/institutes/templates/overview/
+-rw-r--r--   0 dannil     (501) staff       (20)     1547 2019-10-30 10:27:03.000000 scout-browser-4.9.0/scout/server/blueprints/institutes/templates/overview/institutes.html
+-rw-r--r--   0 dannil     (501) staff       (20)     1491 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/server/blueprints/institutes/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/dashboard/
+-rw-r--r--   0 dannil     (501) staff       (20)    10485 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/dashboard/controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)       69 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/dashboard/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/dashboard/static/
+-rw-r--r--   0 dannil     (501) staff       (20)     5768 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/server/blueprints/dashboard/static/charts.js
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/dashboard/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/dashboard/templates/dashboard/
+-rw-r--r--   0 dannil     (501) staff       (20)     8382 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/server/blueprints/dashboard/templates/dashboard/dashboard_general.html
+-rw-r--r--   0 dannil     (501) staff       (20)     2848 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/server/blueprints/dashboard/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/public/
+-rw-r--r--   0 dannil     (501) staff       (20)       53 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/public/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/public/static/
+-rw-r--r--   0 dannil     (501) staff       (20)    19202 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/public/static/logo-scilifelab.png
+-rw-r--r--   0 dannil     (501) staff       (20)     1469 2019-11-26 09:05:05.000000 scout-browser-4.9.0/scout/server/blueprints/public/static/favicon.ico
+-rw-r--r--   0 dannil     (501) staff       (20)    41358 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/public/static/swedac.png
+-rw-r--r--   0 dannil     (501) staff       (20)    21794 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/public/static/logo-karolinska.png
+-rw-r--r--   0 dannil     (501) staff       (20)     3784 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/public/static/scout-logo.png
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/public/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/public/templates/public/
+-rw-r--r--   0 dannil     (501) staff       (20)     2513 2019-10-25 12:59:17.000000 scout-browser-4.9.0/scout/server/blueprints/public/templates/public/index.html
+-rw-r--r--   0 dannil     (501) staff       (20)      785 2019-10-25 12:59:17.000000 scout-browser-4.9.0/scout/server/blueprints/public/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/api/
+-rw-r--r--   0 dannil     (501) staff       (20)       26 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/api/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)      898 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/api/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/variant/
+-rw-r--r--   0 dannil     (501) staff       (20)    12743 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/server/blueprints/variant/controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)       54 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/server/blueprints/variant/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     9140 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/server/blueprints/variant/verification_controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)    16427 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/server/blueprints/variant/utils.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/variant/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/variant/templates/variant/
+-rw-r--r--   0 dannil     (501) staff       (20)    52737 2019-11-27 07:44:37.000000 scout-browser-4.9.0/scout/server/blueprints/variant/templates/variant/variant.html
+-rw-r--r--   0 dannil     (501) staff       (20)    27725 2019-11-27 07:44:37.000000 scout-browser-4.9.0/scout/server/blueprints/variant/templates/variant/sv-variant.html
+-rw-r--r--   0 dannil     (501) staff       (20)    47744 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/server/blueprints/variant/templates/variant/clinvar.html
+-rw-r--r--   0 dannil     (501) staff       (20)     4805 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/server/blueprints/variant/templates/variant/acmg.html
+-rw-r--r--   0 dannil     (501) staff       (20)    11382 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/server/blueprints/variant/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/genes/
+-rw-r--r--   0 dannil     (501) staff       (20)     2156 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/genes/controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)       52 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/genes/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/genes/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/genes/templates/genes/
+-rw-r--r--   0 dannil     (501) staff       (20)     1100 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/server/blueprints/genes/templates/genes/layout.html
+-rw-r--r--   0 dannil     (501) staff       (20)     7501 2019-11-27 07:44:37.000000 scout-browser-4.9.0/scout/server/blueprints/genes/templates/genes/gene.html
+-rw-r--r--   0 dannil     (501) staff       (20)      880 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/server/blueprints/genes/templates/genes/genes.html
+-rw-r--r--   0 dannil     (501) staff       (20)     1591 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/genes/views.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/login/
+-rw-r--r--   0 dannil     (501) staff       (20)      689 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/server/blueprints/login/models.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1034 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/login/controllers.py
+-rw-r--r--   0 dannil     (501) staff       (20)       52 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/login/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/login/static/
+-rw-r--r--   0 dannil     (501) staff       (20)    29283 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/login/static/inspector.svg
+-rw-r--r--   0 dannil     (501) staff       (20)   415421 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/login/static/commissioner.svg
+-rw-r--r--   0 dannil     (501) staff       (20)     2022 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/login/static/constable.svg
+-rw-r--r--   0 dannil     (501) staff       (20)    99307 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/login/static/superintendent.svg
+-rw-r--r--   0 dannil     (501) staff       (20)     3007 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/login/static/sergeant.svg
+-rw-r--r--   0 dannil     (501) staff       (20)   195476 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/blueprints/login/static/commander.svg
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/login/templates/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/blueprints/login/templates/login/
+-rw-r--r--   0 dannil     (501) staff       (20)     1709 2019-10-30 10:27:03.000000 scout-browser-4.9.0/scout/server/blueprints/login/templates/login/users.html
+-rw-r--r--   0 dannil     (501) staff       (20)     5013 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/server/blueprints/login/views.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1334 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/server/config.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1282 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/userpanel.py
+-rw-r--r--   0 dannil     (501) staff       (20)       24 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)    11629 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/server/links.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1942 2019-11-20 12:53:08.000000 scout-browser-4.9.0/scout/server/extensions.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4887 2019-11-27 06:51:54.000000 scout-browser-4.9.0/scout/server/utils.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/static/
+-rw-r--r--   0 dannil     (501) staff       (20)     1469 2019-10-19 12:15:54.000000 scout-browser-4.9.0/scout/server/static/favicon.ico
+-rw-r--r--   0 dannil     (501) staff       (20)      259 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/static/humans.txt
+-rw-r--r--   0 dannil     (501) staff       (20)     5601 2019-11-27 07:44:37.000000 scout-browser-4.9.0/scout/server/static/bs4_styles.css
+-rw-r--r--   0 dannil     (501) staff       (20)      106 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/static/robots.txt
+-rw-r--r--   0 dannil     (501) staff       (20)     7167 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/server/app.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/templates/
+-rw-r--r--   0 dannil     (501) staff       (20)      838 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/templates/report_base.html
+-rw-r--r--   0 dannil     (501) staff       (20)     4672 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/server/templates/utils.html
+-rw-r--r--   0 dannil     (501) staff       (20)     1218 2019-10-25 12:59:17.000000 scout-browser-4.9.0/scout/server/templates/bootstrap4.html
+-rw-r--r--   0 dannil     (501) staff       (20)     3652 2019-10-25 12:59:17.000000 scout-browser-4.9.0/scout/server/templates/layout_bs4.html
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/translations/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/translations/sv/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/server/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 dannil     (501) staff       (20)     4531 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/translations/sv/LC_MESSAGES/messages.po
+-rw-r--r--   0 dannil     (501) staff       (20)     4452 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dannil     (501) staff       (20)      206 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/server/auto.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/utils/
+-rw-r--r--   0 dannil     (501) staff       (20)     7801 2019-10-25 12:59:17.000000 scout-browser-4.9.0/scout/utils/link.py
+-rw-r--r--   0 dannil     (501) staff       (20)      823 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/algorithms.py
+-rw-r--r--   0 dannil     (501) staff       (20)      330 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/handle.py
+-rw-r--r--   0 dannil     (501) staff       (20)      701 2019-10-14 11:01:31.000000 scout-browser-4.9.0/scout/utils/convert.py
+-rw-r--r--   0 dannil     (501) staff       (20)       24 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     6856 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/acmg.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2458 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/matchmaker.py
+-rw-r--r--   0 dannil     (501) staff       (20)      581 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)    10260 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/requests.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8762 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/ensembl_rest_clients.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1377 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/date.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1183 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/coordinates.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)      636 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/utils/md5.py
+-rw-r--r--   0 dannil     (501) staff       (20)       22 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/__version__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/models/
+-rw-r--r--   0 dannil     (501) staff       (20)     1031 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/models/user.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1984 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/event.py
+-rw-r--r--   0 dannil     (501) staff       (20)      376 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/whitelist.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4386 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/hgnc_map.py
+-rw-r--r--   0 dannil     (501) staff       (20)      131 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/models/variant/
+-rw-r--r--   0 dannil     (501) staff       (20)     1617 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/variant/transcript.py
+-rw-r--r--   0 dannil     (501) staff       (20)       42 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/variant/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)      790 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/variant/gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3840 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/variant/variant.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/models/case/
+-rw-r--r--   0 dannil     (501) staff       (20)      110 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/case/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3010 2019-11-27 06:51:54.000000 scout-browser-4.9.0/scout/models/case/case.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2421 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/phenotype_term.py
+-rw-r--r--   0 dannil     (501) staff       (20)      687 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/acmg_evaluation.py
+-rw-r--r--   0 dannil     (501) staff       (20)      664 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1265 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/models/institute.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/adapter/
+-rw-r--r--   0 dannil     (501) staff       (20)     1563 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/client.py
+-rw-r--r--   0 dannil     (501) staff       (20)       85 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1550 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/utils.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/adapter/mongo/
+-rw-r--r--   0 dannil     (501) staff       (20)     2896 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/adapter/mongo/user.py
+-rw-r--r--   0 dannil     (501) staff       (20)    12403 2019-11-16 19:09:15.000000 scout-browser-4.9.0/scout/adapter/mongo/event.py
+-rw-r--r--   0 dannil     (501) staff       (20)    14641 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/mongo/clinvar.py
+-rw-r--r--   0 dannil     (501) staff       (20)    23928 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/adapter/mongo/query.py
+-rw-r--r--   0 dannil     (501) staff       (20)     7389 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/mongo/transcript.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2747 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/mongo/index.py
+-rw-r--r--   0 dannil     (501) staff       (20)    25159 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/adapter/mongo/variant_events.py
+-rw-r--r--   0 dannil     (501) staff       (20)    19764 2019-10-30 10:27:03.000000 scout-browser-4.9.0/scout/adapter/mongo/case_events.py
+-rw-r--r--   0 dannil     (501) staff       (20)       30 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/mongo/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)    14409 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/adapter/mongo/hgnc.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3399 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/mongo/acmg.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3091 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/mongo/matchmaker.py
+-rw-r--r--   0 dannil     (501) staff       (20)    24224 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/adapter/mongo/variant_loader.py
+-rw-r--r--   0 dannil     (501) staff       (20)    32266 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/adapter/mongo/case.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4370 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/adapter/mongo/filter.py
+-rw-r--r--   0 dannil     (501) staff       (20)    15679 2019-10-14 11:01:31.000000 scout-browser-4.9.0/scout/adapter/mongo/panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)    25039 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/adapter/mongo/variant.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)     3336 2019-11-01 16:59:46.000000 scout-browser-4.9.0/scout/adapter/mongo/base.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5978 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/adapter/mongo/institute.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5314 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/adapter/mongo/hpo.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/exceptions/
+-rw-r--r--   0 dannil     (501) staff       (20)       35 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/exceptions/vcf.py
+-rw-r--r--   0 dannil     (501) staff       (20)       38 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/exceptions/config.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1104 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/exceptions/database.py
+-rw-r--r--   0 dannil     (501) staff       (20)       40 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/exceptions/pedigree.py
+-rw-r--r--   0 dannil     (501) staff       (20)      219 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/exceptions/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/load/
+-rw-r--r--   0 dannil     (501) staff       (20)     2153 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/load/exon.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4526 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/load/transcript.py
+-rw-r--r--   0 dannil     (501) staff       (20)      230 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/load/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4268 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/load/all.py
+-rw-r--r--   0 dannil     (501) staff       (20)     6482 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/load/setup.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1066 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/load/case.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5255 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/load/hgnc_gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4283 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/load/panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1615 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/load/report.py
+-rw-r--r--   0 dannil     (501) staff       (20)      571 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/load/institute.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5218 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/load/hpo.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/log/
+-rw-r--r--   0 dannil     (501) staff       (20)     1684 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/log/log.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1332 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/log/handlers.py
+-rw-r--r--   0 dannil     (501) staff       (20)       63 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/log/__init__.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/commands/
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/commands/update/
+-rw-r--r--   0 dannil     (501) staff       (20)     2694 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/user.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1395 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/omim.py
+-rw-r--r--   0 dannil     (501) staff       (20)       25 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1974 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/phenotype_groups.py
+-rw-r--r--   0 dannil     (501) staff       (20)      752 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/compounds.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)     1397 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/disease.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)     3419 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/commands/update/genes.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5383 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/commands/update/case.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1575 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1060 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/base.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1517 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/institute.py
+-rw-r--r--   0 dannil     (501) staff       (20)      816 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/update/hpo.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/commands/delete/
+-rw-r--r--   0 dannil     (501) staff       (20)     5217 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/delete/delete_command.py
+-rw-r--r--   0 dannil     (501) staff       (20)       34 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/delete/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1059 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/convert.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/commands/setup/
+-rw-r--r--   0 dannil     (501) staff       (20)     4457 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/commands/setup/setup_scout.py
+-rw-r--r--   0 dannil     (501) staff       (20)       30 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/setup/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)       22 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2054 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/serve.py
+-rw-r--r--   0 dannil     (501) staff       (20)      749 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/index_command.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/commands/load/
+-rwxr-xr-x   0 dannil     (501) staff       (20)     1452 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/commands/load/user.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4872 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/commands/load/variants.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4145 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/load/research.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1868 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/load/exons.py
+-rw-r--r--   0 dannil     (501) staff       (20)      844 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/load/region.py
+-rw-r--r--   0 dannil     (501) staff       (20)       23 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/load/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3052 2019-11-11 08:51:50.000000 scout-browser-4.9.0/scout/commands/load/case.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2829 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/load/panel.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)      925 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/load/base.py
+-rw-r--r--   0 dannil     (501) staff       (20)      810 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/load/report.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1105 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/load/institute.py
+-rw-r--r--   0 dannil     (501) staff       (20)      312 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/utils.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/commands/view/
+-rw-r--r--   0 dannil     (501) staff       (20)     1221 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/transcripts.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1379 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/institutes.py
+-rw-r--r--   0 dannil     (501) staff       (20)      760 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/index.py
+-rw-r--r--   0 dannil     (501) staff       (20)      799 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/users.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1775 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/individuals.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1283 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/exons.py
+-rw-r--r--   0 dannil     (501) staff       (20)      509 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/whitelist.py
+-rw-r--r--   0 dannil     (501) staff       (20)       23 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1393 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/intervals.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1396 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/hgnc.py
+-rw-r--r--   0 dannil     (501) staff       (20)      703 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/diseases.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2035 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/aliases.py
+-rw-r--r--   0 dannil     (501) staff       (20)      454 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/collections.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2954 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/case.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1110 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/base.py
+-rw-r--r--   0 dannil     (501) staff       (20)      933 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/panels.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1442 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/view/hpo.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/commands/export/
+-rw-r--r--   0 dannil     (501) staff       (20)      679 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/exon.py
+-rw-r--r--   0 dannil     (501) staff       (20)      988 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/transcript.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3337 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/mitochondrial_report.py
+-rw-r--r--   0 dannil     (501) staff       (20)       34 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)      266 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/utils.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)      896 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/export_command.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2139 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/case.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1267 2019-10-26 11:59:05.000000 scout-browser-4.9.0/scout/commands/export/gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1553 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5859 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/variant.py
+-rw-r--r--   0 dannil     (501) staff       (20)      713 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/export/hpo.py
+-rwxr-xr-x   0 dannil     (501) staff       (20)      997 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/commands/wipe_database.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3612 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/commands/base.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/build/
+-rw-r--r--   0 dannil     (501) staff       (20)      861 2019-10-25 12:59:16.000000 scout-browser-4.9.0/scout/build/user.py
+-rw-r--r--   0 dannil     (501) staff       (20)      511 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1656 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/acmg.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2631 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/disease.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3411 2019-11-27 06:51:54.000000 scout-browser-4.9.0/scout/build/individual.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/build/variant/
+-rw-r--r--   0 dannil     (501) staff       (20)     2582 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/variant/transcript.py
+-rw-r--r--   0 dannil     (501) staff       (20)      720 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/variant/genotype.py
+-rw-r--r--   0 dannil     (501) staff       (20)      172 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/variant/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)      734 2019-10-11 12:26:50.000000 scout-browser-4.9.0/scout/build/variant/clnsig.py
+-rw-r--r--   0 dannil     (501) staff       (20)      848 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/variant/compound.py
+-rw-r--r--   0 dannil     (501) staff       (20)     3594 2019-11-20 13:10:43.000000 scout-browser-4.9.0/scout/build/variant/gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)    14076 2019-11-27 07:43:41.000000 scout-browser-4.9.0/scout/build/variant/variant.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8234 2019-11-22 10:10:32.000000 scout-browser-4.9.0/scout/build/case.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/build/genes/
+-rw-r--r--   0 dannil     (501) staff       (20)     2345 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/genes/exon.py
+-rw-r--r--   0 dannil     (501) staff       (20)     2228 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/genes/transcript.py
+-rw-r--r--   0 dannil     (501) staff       (20)        1 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/genes/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4804 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/genes/hgnc_gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)     4674 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)      918 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/institute.py
+-rw-r--r--   0 dannil     (501) staff       (20)     1124 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/hpo.py
+-rw-r--r--   0 dannil     (501) staff       (20)      359 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/build/phenotype.py
+drwxr-xr-x   0 dannil     (501) staff       (20)        0 2019-11-27 07:45:41.000000 scout-browser-4.9.0/scout/export/
+-rw-r--r--   0 dannil     (501) staff       (20)     2714 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/export/exon.py
+-rw-r--r--   0 dannil     (501) staff       (20)      411 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/export/transcript.py
+-rw-r--r--   0 dannil     (501) staff       (20)        0 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/export/__init__.py
+-rw-r--r--   0 dannil     (501) staff       (20)      270 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/export/gene.py
+-rw-r--r--   0 dannil     (501) staff       (20)     5198 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/export/panel.py
+-rw-r--r--   0 dannil     (501) staff       (20)     6332 2019-10-07 06:32:17.000000 scout-browser-4.9.0/scout/export/variant.py
+-rw-r--r--   0 dannil     (501) staff       (20)     8138 2019-11-22 10:10:32.000000 scout-browser-4.9.0/README.md
+-rwxr-xr-x   0 dannil     (501) staff       (20)     3911 2019-10-07 06:32:17.000000 scout-browser-4.9.0/setup.py
+-rw-r--r--   0 dannil     (501) staff       (20)      239 2019-11-20 12:53:08.000000 scout-browser-4.9.0/requirements-dev.txt
+-rw-r--r--   0 dannil     (501) staff       (20)      129 2019-11-27 07:45:41.000000 scout-browser-4.9.0/setup.cfg
```

### Comparing `scout-browser-4.8.3/CHANGELOG.md` & `scout-browser-4.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,62 @@
 # Change Log
 All notable changes to this project will be documented in this file.
 This project adheres to [Semantic Versioning](http://semver.org/).
 
 About changelog [here](https://keepachangelog.com/en/1.0.0/)
 
-## [4.8.3]
+## [x.x.x]
+
+### Added
+
+
+### Fixed
+
+
+
+## [4.9.0]
+
+### Added
+- Improved MatchMaker pages, including visible patient contacts email address
+- New badges for the github repo
+- Links to [GENEMANIA](genemania.org)
+- Sort gene panel list on case view.
+- More automatic tests
 
 ### Fixed
+- Fix error when a gene is added to an empty dynamic gene panel
+- Fix crash when attempting to add genes on incorrect format to dynamic gene panel
+- Manual rank variant tags could be saved in a "Select a tag"-state, a problem in the variants view.
+- Same case evaluations are no longer shown as gray previous evaluations on the variants page
+- Stay on research pages, even if reset, next first buttons are pressed..
+- Overlapping variants will now be visible on variant page again
+- Fix missing classification comments and links in evaluations page
+
+
+## [4.8.3]
+
+### Added
 
+### Fixed
 - Bug when ordering sanger
 
+
 ## [4.8.2]
 
 ### Added
 
 ### Fixed
-
 - Avoid opening extra tab for coverage report
 - Fixed a problem when rank model version was saved as floats and not strings
 - Fixed a problem with displaying dismiss variant reasons on the general report
 - Disable load and delete filter buttons if there are no saved filters
 - Fix problem with missing verifications
 - Remove duplicate users and merge their data and activity
 
+
 ## [4.8.1]
 
 ### Added
 
 ### Fixed
 - Prevent login fail for users with id defined by ObjectId and not email
 - Prevent the app from crashing with `AttributeError: 'NoneType' object has no attribute 'message'`
```

### Comparing `scout-browser-4.8.3/LICENSE` & `scout-browser-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/MANIFEST.in` & `scout-browser-4.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/PKG-INFO` & `scout-browser-4.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scout-browser
-Version: 4.8.3
+Version: 4.9.0
 Summary: Clinical DNA variant visualizer and browser.
 Home-page: https://github.com/Clinical-Genomics/scout
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.se
 License: UNKNOWN
 Description: 
         <p align="center">
@@ -13,14 +13,18 @@
         	</a>
         	<h3 align="center">Analyze VCFs and collaborate on solving rare diseases quicker</h3>
         </p>
         
         [![Build Status][travis-img]][travis-url]
         [![PyPI Version][pypi-img]][pypi-url]
         [![Coverage Status](https://coveralls.io/repos/github/Clinical-Genomics/scout/badge.svg?branch=master)](https://coveralls.io/github/Clinical-Genomics/scout?branch=master)
+        [![GitHub issues-closed][closed-issues-img]][closed-issues-url]
+        [![Average time to resolve an issue][ismaintained-resolve-img]][ismaintained-resolve-url]
+        [![Percentage of issues still open][ismaintained-open-rate-img]][ismaintained-open-rate-url]
+        [![GitHub commits](https://img.shields.io/github/commits-since/Clinical-Genomics/scout/v4.8.0.svg)](https://GitHub.com/Clinical-Genomics/scout/commit/)
         
         ## What is Scout?
         
         - **Simple** - Analyze variants in a simple to use web interface.
         - **Aggregation** - Combine results from multiple analyses and VCFs into a centralized database.
         - **Collaboration** - Write comments and share cases between users and institutes.
         
@@ -182,14 +186,20 @@
         
         
         [chanjo]: https://github.com/Clinical-Genomics/chanjo
         [travis-img]: https://img.shields.io/travis/Clinical-Genomics/scout/develop.svg?style=flat-square
         [travis-url]: https://travis-ci.org/Clinical-Genomics/scout
         [pypi-img]: https://img.shields.io/pypi/v/scout-browser.svg?style=flat-square
         [pypi-url]: https://pypi.python.org/pypi/scout-browser/
+        [ismaintained-resolve-img]: http://isitmaintained.com/badge/resolution/Clinical-Genomics/scout.svg
+        [ismaintained-resolve-url]: http://isitmaintained.com/project/Clinical-Genomics/scout
+        [ismaintained-open-rate-img]: http://isitmaintained.com/badge/open/Clinical-Genomics/scout.svg
+        [ismaintained-open-rate-url]: http://isitmaintained.com/project/Clinical-Genomics/scout
+        [closed-issues-img]: https://img.shields.io/github/issues-closed/Clinical-Genomics/scout.svg
+        [closed-issues-url]: https://GitHub.com/Clinical-Genomics/scout/issues?q=is%3Aissue+is%3Aclosed
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,63 +1,69 @@
-Metadata-Version: 2.1 Name: scout-browser Version: 4.8.3 Summary: Clinical DNA
+Metadata-Version: 2.1 Name: scout-browser Version: 4.9.0 Summary: Clinical DNA
 variant visualizer and browser. Home-page: https://github.com/Clinical-
 Genomics/scout Author: MÃ¥ns Magnusson Author-email:
 mans.magnusson@scilifelab.se License: UNKNOWN Description:
                           [artwork/logo-display.png]
     **** Analyze VCFs and collaborate on solving rare diseases quicker ****
 [![Build Status][travis-img]][travis-url] [![PyPI Version][pypi-img]][pypi-url]
 [![Coverage Status](https://coveralls.io/repos/github/Clinical-Genomics/scout/
 badge.svg?branch=master)](https://coveralls.io/github/Clinical-Genomics/
-scout?branch=master) ## What is Scout? - **Simple** - Analyze variants in a
-simple to use web interface. - **Aggregation** - Combine results from multiple
-analyses and VCFs into a centralized database. - **Collaboration** - Write
-comments and share cases between users and institutes. ## Documentation This
-README only gives a brief overview of Scout, for a more complete reference,
-please check out our docs: [www.clinicalgenomics.se/scout](http://
-www.clinicalgenomics.se/scout/). ## Installation  ```bash git clone https://
-github.com/Clinical-Genomics/scout cd scout pip install --requirement
-requirements.txt --editable . ``` Scout PDF reports are created using [Flask-
-WeasyPrint](https://pythonhosted.org/Flask-WeasyPrint/). This library requires
-external dependencies which need be installed separately (namely Cairo and
-Pango). See platform-specific instructions for Linux, macOS and Windows
-available on the WeasyPrint installation [pages](https://
-weasyprint.readthedocs.io/en/stable/install.html#). You also need to have an
-instance of MongoDB running. I've found that it's easiest to do using the
-official Docker image: ```bash docker run --name mongo -p 27017:27017 mongo ```
-## Usage ### Demo Once installed, you can setup Scout by running a few commands
-using the included command line interface. Given you have a MongoDB server
-listening on the default port (27017), this is how you would setup a fully
-working Scout demo: ```bash scout setup demo ``` This will setup an instance of
-scout with a database called `scout-demo`. Now run ```bash scout --demo serve
-``` And play around with the interface. A user has been created with email
-clark.kent@mail.com so use that adress to get access ### Initialize scout To
-initialize a working instance with all genes, diseases etc run ```bash scout
-setup database ``` for more info, run `scout --help` > If you intent to use
-authentication, make sure you are using a Google email! The previous command
-setup the database with a curated collection of gene definitions with links to
-OMIM along with HPO phenotype terms. Now we will load some example data. Scout
-expects the analysis to be accomplished using various gene panels so let's load
-one and then our first analysis case: ```bash scout load panel scout/demo/
-panel_1.txt scout load case scout/demo/643594.config.yaml ``` ## Integration
-with chanjo for coverage report visualization Scout may be configured to
-visualize coverage reports produced by [Chanjo][chanjo]. Instructions on how to
-enable this feature can be found in the document [chanjo_coverage_integration]
-(docs/admin-guide/chanjo_coverage_integration.md). ## Server setup Scout needs
-a server config to know which databases to connect to etc. Depending on which
-information you provide you activate different parts of the interface
-automatically, including user authentication, coverage, and local observations.
-This is an example of the config file: ```python # scoutconfig.py # list of
-email addresses to send errors to in production ADMINS =
-['paul.anderson@magnolia.com'] MONGO_HOST = 'localhost' MONGO_PORT = 27017
-MONGO_DBNAME = 'scoutTest' MONGO_USERNAME = 'testUser' MONGO_PASSWORD =
-'testPass' # enable user authentication using Google OAuth GOOGLE = dict
-( consumer_key='CLIENT_ID', consumer_secret='CLIENT_SECRET', base_url='https://
-www.googleapis.com/oauth2/v1/', authorize_url='https://accounts.google.com/o/
-oauth2/auth', request_token_url=None, request_token_params={ 'scope': ("https:/
-/www.googleapis.com/auth/userinfo.profile " "https://www.googleapis.com/auth/
+scout?branch=master) [![GitHub issues-closed][closed-issues-img]][closed-
+issues-url] [![Average time to resolve an issue][ismaintained-resolve-img]]
+[ismaintained-resolve-url] [![Percentage of issues still open][ismaintained-
+open-rate-img]][ismaintained-open-rate-url] [![GitHub commits](https://
+img.shields.io/github/commits-since/Clinical-Genomics/scout/v4.8.0.svg)](https:
+//GitHub.com/Clinical-Genomics/scout/commit/) ## What is Scout? - **Simple** -
+Analyze variants in a simple to use web interface. - **Aggregation** - Combine
+results from multiple analyses and VCFs into a centralized database. -
+**Collaboration** - Write comments and share cases between users and
+institutes. ## Documentation This README only gives a brief overview of Scout,
+for a more complete reference, please check out our docs:
+[www.clinicalgenomics.se/scout](http://www.clinicalgenomics.se/scout/). ##
+Installation  ```bash git clone https://github.com/Clinical-Genomics/scout cd
+scout pip install --requirement requirements.txt --editable . ``` Scout PDF
+reports are created using [Flask-WeasyPrint](https://pythonhosted.org/Flask-
+WeasyPrint/). This library requires external dependencies which need be
+installed separately (namely Cairo and Pango). See platform-specific
+instructions for Linux, macOS and Windows available on the WeasyPrint
+installation [pages](https://weasyprint.readthedocs.io/en/stable/
+install.html#). You also need to have an instance of MongoDB running. I've
+found that it's easiest to do using the official Docker image: ```bash docker
+run --name mongo -p 27017:27017 mongo ``` ## Usage ### Demo Once installed, you
+can setup Scout by running a few commands using the included command line
+interface. Given you have a MongoDB server listening on the default port
+(27017), this is how you would setup a fully working Scout demo: ```bash scout
+setup demo ``` This will setup an instance of scout with a database called
+`scout-demo`. Now run ```bash scout --demo serve ``` And play around with the
+interface. A user has been created with email clark.kent@mail.com so use that
+adress to get access ### Initialize scout To initialize a working instance with
+all genes, diseases etc run ```bash scout setup database ``` for more info, run
+`scout --help` > If you intent to use authentication, make sure you are using a
+Google email! The previous command setup the database with a curated collection
+of gene definitions with links to OMIM along with HPO phenotype terms. Now we
+will load some example data. Scout expects the analysis to be accomplished
+using various gene panels so let's load one and then our first analysis case:
+```bash scout load panel scout/demo/panel_1.txt scout load case scout/demo/
+643594.config.yaml ``` ## Integration with chanjo for coverage report
+visualization Scout may be configured to visualize coverage reports produced by
+[Chanjo][chanjo]. Instructions on how to enable this feature can be found in
+the document [chanjo_coverage_integration](docs/admin-guide/
+chanjo_coverage_integration.md). ## Server setup Scout needs a server config to
+know which databases to connect to etc. Depending on which information you
+provide you activate different parts of the interface automatically, including
+user authentication, coverage, and local observations. This is an example of
+the config file: ```python # scoutconfig.py # list of email addresses to send
+errors to in production ADMINS = ['paul.anderson@magnolia.com'] MONGO_HOST =
+'localhost' MONGO_PORT = 27017 MONGO_DBNAME = 'scoutTest' MONGO_USERNAME =
+'testUser' MONGO_PASSWORD = 'testPass' # enable user authentication using
+Google OAuth GOOGLE = dict( consumer_key='CLIENT_ID',
+consumer_secret='CLIENT_SECRET', base_url='https://www.googleapis.com/oauth2/
+v1/', authorize_url='https://accounts.google.com/o/oauth2/auth',
+request_token_url=None, request_token_params={ 'scope': ("https://
+www.googleapis.com/auth/userinfo.profile " "https://www.googleapis.com/auth/
 userinfo.email"), }, access_token_url='https://accounts.google.com/o/oauth2/
 token', access_token_method='POST' ) # enable Phenomizer gene predictions from
 phenotype terms PHENOMIZER_USERNAME = '???' PHENOMIZER_PASSWORD = '???' #
 enable Chanjo coverage integration SQLALCHEMY_DATABASE_URI = '???'
 REPORT_LANGUAGE = 'en' # or 'sv' # other interesting settings
 SQLALCHEMY_TRACK_MODIFICATIONS = False # this is essential in production
 TEMPLATES_AUTO_RELOAD = False # consider turning off in production SECRET_KEY =
@@ -87,14 +93,22 @@
 regardless of the amount of code provided or your skills as a programmer. More
 info on how to contribute to the project and a description of the Scout
 branching workflow can be found [here](CONTRIBUTING.md). [chanjo]: https://
 github.com/Clinical-Genomics/chanjo [travis-img]: https://img.shields.io/
 travis/Clinical-Genomics/scout/develop.svg?style=flat-square [travis-url]:
 https://travis-ci.org/Clinical-Genomics/scout [pypi-img]: https://
 img.shields.io/pypi/v/scout-browser.svg?style=flat-square [pypi-url]: https://
-pypi.python.org/pypi/scout-browser/ Platform: UNKNOWN Classifier: Environment
-:: Web Environment Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: BSD License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Topic ::
-Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
-Development :: Libraries Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown Provides-Extra: coverage
+pypi.python.org/pypi/scout-browser/ [ismaintained-resolve-img]: http://
+isitmaintained.com/badge/resolution/Clinical-Genomics/scout.svg [ismaintained-
+resolve-url]: http://isitmaintained.com/project/Clinical-Genomics/scout
+[ismaintained-open-rate-img]: http://isitmaintained.com/badge/open/Clinical-
+Genomics/scout.svg [ismaintained-open-rate-url]: http://isitmaintained.com/
+project/Clinical-Genomics/scout [closed-issues-img]: https://img.shields.io/
+github/issues-closed/Clinical-Genomics/scout.svg [closed-issues-url]: https://
+GitHub.com/Clinical-Genomics/scout/issues?q=is%3Aissue+is%3Aclosed Platform:
+UNKNOWN Classifier: Environment :: Web Environment Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries Classifier: Programming
+Language :: Python :: 3.6 Description-Content-Type: text/markdown Provides-
+Extra: coverage
```

### Comparing `scout-browser-4.8.3/README.md` & `scout-browser-4.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 	</a>
 	<h3 align="center">Analyze VCFs and collaborate on solving rare diseases quicker</h3>
 </p>
 
 [![Build Status][travis-img]][travis-url]
 [![PyPI Version][pypi-img]][pypi-url]
 [![Coverage Status](https://coveralls.io/repos/github/Clinical-Genomics/scout/badge.svg?branch=master)](https://coveralls.io/github/Clinical-Genomics/scout?branch=master)
+[![GitHub issues-closed][closed-issues-img]][closed-issues-url]
+[![Average time to resolve an issue][ismaintained-resolve-img]][ismaintained-resolve-url]
+[![Percentage of issues still open][ismaintained-open-rate-img]][ismaintained-open-rate-url]
+[![GitHub commits](https://img.shields.io/github/commits-since/Clinical-Genomics/scout/v4.8.0.svg)](https://GitHub.com/Clinical-Genomics/scout/commit/)
 
 ## What is Scout?
 
 - **Simple** - Analyze variants in a simple to use web interface.
 - **Aggregation** - Combine results from multiple analyses and VCFs into a centralized database.
 - **Collaboration** - Write comments and share cases between users and institutes.
 
@@ -173,7 +177,13 @@
 
 
 [chanjo]: https://github.com/Clinical-Genomics/chanjo
 [travis-img]: https://img.shields.io/travis/Clinical-Genomics/scout/develop.svg?style=flat-square
 [travis-url]: https://travis-ci.org/Clinical-Genomics/scout
 [pypi-img]: https://img.shields.io/pypi/v/scout-browser.svg?style=flat-square
 [pypi-url]: https://pypi.python.org/pypi/scout-browser/
+[ismaintained-resolve-img]: http://isitmaintained.com/badge/resolution/Clinical-Genomics/scout.svg
+[ismaintained-resolve-url]: http://isitmaintained.com/project/Clinical-Genomics/scout
+[ismaintained-open-rate-img]: http://isitmaintained.com/badge/open/Clinical-Genomics/scout.svg
+[ismaintained-open-rate-url]: http://isitmaintained.com/project/Clinical-Genomics/scout
+[closed-issues-img]: https://img.shields.io/github/issues-closed/Clinical-Genomics/scout.svg
+[closed-issues-url]: https://GitHub.com/Clinical-Genomics/scout/issues?q=is%3Aissue+is%3Aclosed
```

#### html2text {}

```diff
@@ -1,59 +1,65 @@
                           [artwork/logo-display.png]
     **** Analyze VCFs and collaborate on solving rare diseases quicker ****
 [![Build Status][travis-img]][travis-url] [![PyPI Version][pypi-img]][pypi-url]
 [![Coverage Status](https://coveralls.io/repos/github/Clinical-Genomics/scout/
 badge.svg?branch=master)](https://coveralls.io/github/Clinical-Genomics/
-scout?branch=master) ## What is Scout? - **Simple** - Analyze variants in a
-simple to use web interface. - **Aggregation** - Combine results from multiple
-analyses and VCFs into a centralized database. - **Collaboration** - Write
-comments and share cases between users and institutes. ## Documentation This
-README only gives a brief overview of Scout, for a more complete reference,
-please check out our docs: [www.clinicalgenomics.se/scout](http://
-www.clinicalgenomics.se/scout/). ## Installation  ```bash git clone https://
-github.com/Clinical-Genomics/scout cd scout pip install --requirement
-requirements.txt --editable . ``` Scout PDF reports are created using [Flask-
-WeasyPrint](https://pythonhosted.org/Flask-WeasyPrint/). This library requires
-external dependencies which need be installed separately (namely Cairo and
-Pango). See platform-specific instructions for Linux, macOS and Windows
-available on the WeasyPrint installation [pages](https://
-weasyprint.readthedocs.io/en/stable/install.html#). You also need to have an
-instance of MongoDB running. I've found that it's easiest to do using the
-official Docker image: ```bash docker run --name mongo -p 27017:27017 mongo ```
-## Usage ### Demo Once installed, you can setup Scout by running a few commands
-using the included command line interface. Given you have a MongoDB server
-listening on the default port (27017), this is how you would setup a fully
-working Scout demo: ```bash scout setup demo ``` This will setup an instance of
-scout with a database called `scout-demo`. Now run ```bash scout --demo serve
-``` And play around with the interface. A user has been created with email
-clark.kent@mail.com so use that adress to get access ### Initialize scout To
-initialize a working instance with all genes, diseases etc run ```bash scout
-setup database ``` for more info, run `scout --help` > If you intent to use
-authentication, make sure you are using a Google email! The previous command
-setup the database with a curated collection of gene definitions with links to
-OMIM along with HPO phenotype terms. Now we will load some example data. Scout
-expects the analysis to be accomplished using various gene panels so let's load
-one and then our first analysis case: ```bash scout load panel scout/demo/
-panel_1.txt scout load case scout/demo/643594.config.yaml ``` ## Integration
-with chanjo for coverage report visualization Scout may be configured to
-visualize coverage reports produced by [Chanjo][chanjo]. Instructions on how to
-enable this feature can be found in the document [chanjo_coverage_integration]
-(docs/admin-guide/chanjo_coverage_integration.md). ## Server setup Scout needs
-a server config to know which databases to connect to etc. Depending on which
-information you provide you activate different parts of the interface
-automatically, including user authentication, coverage, and local observations.
-This is an example of the config file: ```python # scoutconfig.py # list of
-email addresses to send errors to in production ADMINS =
-['paul.anderson@magnolia.com'] MONGO_HOST = 'localhost' MONGO_PORT = 27017
-MONGO_DBNAME = 'scoutTest' MONGO_USERNAME = 'testUser' MONGO_PASSWORD =
-'testPass' # enable user authentication using Google OAuth GOOGLE = dict
-( consumer_key='CLIENT_ID', consumer_secret='CLIENT_SECRET', base_url='https://
-www.googleapis.com/oauth2/v1/', authorize_url='https://accounts.google.com/o/
-oauth2/auth', request_token_url=None, request_token_params={ 'scope': ("https:/
-/www.googleapis.com/auth/userinfo.profile " "https://www.googleapis.com/auth/
+scout?branch=master) [![GitHub issues-closed][closed-issues-img]][closed-
+issues-url] [![Average time to resolve an issue][ismaintained-resolve-img]]
+[ismaintained-resolve-url] [![Percentage of issues still open][ismaintained-
+open-rate-img]][ismaintained-open-rate-url] [![GitHub commits](https://
+img.shields.io/github/commits-since/Clinical-Genomics/scout/v4.8.0.svg)](https:
+//GitHub.com/Clinical-Genomics/scout/commit/) ## What is Scout? - **Simple** -
+Analyze variants in a simple to use web interface. - **Aggregation** - Combine
+results from multiple analyses and VCFs into a centralized database. -
+**Collaboration** - Write comments and share cases between users and
+institutes. ## Documentation This README only gives a brief overview of Scout,
+for a more complete reference, please check out our docs:
+[www.clinicalgenomics.se/scout](http://www.clinicalgenomics.se/scout/). ##
+Installation  ```bash git clone https://github.com/Clinical-Genomics/scout cd
+scout pip install --requirement requirements.txt --editable . ``` Scout PDF
+reports are created using [Flask-WeasyPrint](https://pythonhosted.org/Flask-
+WeasyPrint/). This library requires external dependencies which need be
+installed separately (namely Cairo and Pango). See platform-specific
+instructions for Linux, macOS and Windows available on the WeasyPrint
+installation [pages](https://weasyprint.readthedocs.io/en/stable/
+install.html#). You also need to have an instance of MongoDB running. I've
+found that it's easiest to do using the official Docker image: ```bash docker
+run --name mongo -p 27017:27017 mongo ``` ## Usage ### Demo Once installed, you
+can setup Scout by running a few commands using the included command line
+interface. Given you have a MongoDB server listening on the default port
+(27017), this is how you would setup a fully working Scout demo: ```bash scout
+setup demo ``` This will setup an instance of scout with a database called
+`scout-demo`. Now run ```bash scout --demo serve ``` And play around with the
+interface. A user has been created with email clark.kent@mail.com so use that
+adress to get access ### Initialize scout To initialize a working instance with
+all genes, diseases etc run ```bash scout setup database ``` for more info, run
+`scout --help` > If you intent to use authentication, make sure you are using a
+Google email! The previous command setup the database with a curated collection
+of gene definitions with links to OMIM along with HPO phenotype terms. Now we
+will load some example data. Scout expects the analysis to be accomplished
+using various gene panels so let's load one and then our first analysis case:
+```bash scout load panel scout/demo/panel_1.txt scout load case scout/demo/
+643594.config.yaml ``` ## Integration with chanjo for coverage report
+visualization Scout may be configured to visualize coverage reports produced by
+[Chanjo][chanjo]. Instructions on how to enable this feature can be found in
+the document [chanjo_coverage_integration](docs/admin-guide/
+chanjo_coverage_integration.md). ## Server setup Scout needs a server config to
+know which databases to connect to etc. Depending on which information you
+provide you activate different parts of the interface automatically, including
+user authentication, coverage, and local observations. This is an example of
+the config file: ```python # scoutconfig.py # list of email addresses to send
+errors to in production ADMINS = ['paul.anderson@magnolia.com'] MONGO_HOST =
+'localhost' MONGO_PORT = 27017 MONGO_DBNAME = 'scoutTest' MONGO_USERNAME =
+'testUser' MONGO_PASSWORD = 'testPass' # enable user authentication using
+Google OAuth GOOGLE = dict( consumer_key='CLIENT_ID',
+consumer_secret='CLIENT_SECRET', base_url='https://www.googleapis.com/oauth2/
+v1/', authorize_url='https://accounts.google.com/o/oauth2/auth',
+request_token_url=None, request_token_params={ 'scope': ("https://
+www.googleapis.com/auth/userinfo.profile " "https://www.googleapis.com/auth/
 userinfo.email"), }, access_token_url='https://accounts.google.com/o/oauth2/
 token', access_token_method='POST' ) # enable Phenomizer gene predictions from
 phenotype terms PHENOMIZER_USERNAME = '???' PHENOMIZER_PASSWORD = '???' #
 enable Chanjo coverage integration SQLALCHEMY_DATABASE_URI = '???'
 REPORT_LANGUAGE = 'en' # or 'sv' # other interesting settings
 SQLALCHEMY_TRACK_MODIFICATIONS = False # this is essential in production
 TEMPLATES_AUTO_RELOAD = False # consider turning off in production SECRET_KEY =
@@ -83,8 +89,15 @@
 regardless of the amount of code provided or your skills as a programmer. More
 info on how to contribute to the project and a description of the Scout
 branching workflow can be found [here](CONTRIBUTING.md). [chanjo]: https://
 github.com/Clinical-Genomics/chanjo [travis-img]: https://img.shields.io/
 travis/Clinical-Genomics/scout/develop.svg?style=flat-square [travis-url]:
 https://travis-ci.org/Clinical-Genomics/scout [pypi-img]: https://
 img.shields.io/pypi/v/scout-browser.svg?style=flat-square [pypi-url]: https://
-pypi.python.org/pypi/scout-browser/
+pypi.python.org/pypi/scout-browser/ [ismaintained-resolve-img]: http://
+isitmaintained.com/badge/resolution/Clinical-Genomics/scout.svg [ismaintained-
+resolve-url]: http://isitmaintained.com/project/Clinical-Genomics/scout
+[ismaintained-open-rate-img]: http://isitmaintained.com/badge/open/Clinical-
+Genomics/scout.svg [ismaintained-open-rate-url]: http://isitmaintained.com/
+project/Clinical-Genomics/scout [closed-issues-img]: https://img.shields.io/
+github/issues-closed/Clinical-Genomics/scout.svg [closed-issues-url]: https://
+GitHub.com/Clinical-Genomics/scout/issues?q=is%3Aissue+is%3Aclosed
```

### Comparing `scout-browser-4.8.3/requirements.txt` & `scout-browser-4.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/client.py` & `scout-browser-4.9.0/scout/adapter/client.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/acmg.py` & `scout-browser-4.9.0/scout/adapter/mongo/acmg.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/base.py` & `scout-browser-4.9.0/scout/adapter/mongo/base.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/case.py` & `scout-browser-4.9.0/scout/adapter/mongo/case.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,14 +242,30 @@
 
         LOG.info("Get cases with query {0}".format(query))
         if(order):
             return self.case_collection.find(query)
         else:
             return self.case_collection.find(query).sort('updated_at', -1)
 
+    def prioritized_cases(self, institute_id=None):
+        """Fetches any prioritized cases from the backend.
+
+        Args:
+            collaborator(str): If collaborator should be considered
+        """
+        query = {}
+
+        if institute_id:
+            LOG.debug("Use collaborator {0}".format(institute_id))
+            query['collaborators'] = institute_id
+
+        query['status'] = 'prioritized'
+
+        return self.case_collection.find(query).sort('updated_at', -1)
+
     def nr_cases(self, institute_id=None):
         """Return the number of cases
 
         This function will change when we migrate to 3.7.1
 
         Args:
             collaborator(str): Institute id
@@ -280,22 +296,25 @@
             description: str
         }
 
         Arguments:
             case (dict): The case that should be updated
             hgnc_symbols (iterable): A list of hgnc_symbols
             hgnc_ids (iterable): A list of hgnc_ids
+            phenotype_id(list): optionally add phenotype_ids used to generate list
+            add_only(bool): set by eg ADDGENE to add genes, and NOT reset previous dynamic_gene_list
 
         Returns:
             updated_case(dict)
         """
         dynamic_gene_list = []
         if add_only:
-            dynamic_gene_list  = self.case_collection.find_one({ '_id': case['_id'] },
-                { 'dynamic_gene_list': 1, '_id': 0 })['dynamic_gene_list']
+            dynamic_gene_list  = list( self.case_collection.find_one({ '_id': case['_id'] },
+                { 'dynamic_gene_list': 1, '_id': 0 }).get('dynamic_gene_list', []))
+
             LOG.debug("Add selected: current dynamic gene list: {}".format(dynamic_gene_list))
 
         res = []
         if hgnc_ids:
             LOG.info("Fetching genes by hgnc id: {}".format(hgnc_ids))
             res = self.hgnc_collection.find({'hgnc_id': {'$in': hgnc_ids}, 'build': build})
         elif hgnc_symbols:
```

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/case_events.py` & `scout-browser-4.9.0/scout/adapter/mongo/case_events.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/clinvar.py` & `scout-browser-4.9.0/scout/adapter/mongo/clinvar.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/event.py` & `scout-browser-4.9.0/scout/adapter/mongo/event.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/filter.py` & `scout-browser-4.9.0/scout/adapter/mongo/filter.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/hgnc.py` & `scout-browser-4.9.0/scout/adapter/mongo/hgnc.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/hpo.py` & `scout-browser-4.9.0/scout/adapter/mongo/hpo.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/index.py` & `scout-browser-4.9.0/scout/adapter/mongo/index.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/institute.py` & `scout-browser-4.9.0/scout/adapter/mongo/institute.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,23 @@
     def add_institute(self, institute_obj):
         """Add a institute to the database
 
             Args:
                 institute_obj(Institute)
         """
         internal_id = institute_obj['internal_id']
-        display_name = institute_obj['internal_id']
+        display_name = institute_obj['display_name']
 
         # Check if institute already exists
         if self.institute(institute_id=internal_id):
             raise IntegrityError("Institute {0} already exists in database"
                                  .format(display_name))
 
         LOG.info("Adding institute with internal_id: {0} and "
-                    "display_name: {1}".format(internal_id,
-                                               display_name))
+                    "display_name: {1}".format(internal_id, display_name))
 
         insert_info = self.institute_collection.insert_one(institute_obj)
         ##TODO check if insert info was ok
         LOG.info("Institute saved")
 
     def update_institute(self, internal_id, sanger_recipient=None, coverage_cutoff=None,
                          frequency_cutoff=None, display_name=None, remove_sanger=None,
```

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/matchmaker.py` & `scout-browser-4.9.0/scout/adapter/mongo/matchmaker.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/panel.py` & `scout-browser-4.9.0/scout/adapter/mongo/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/query.py` & `scout-browser-4.9.0/scout/adapter/mongo/query.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/transcript.py` & `scout-browser-4.9.0/scout/adapter/mongo/transcript.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/user.py` & `scout-browser-4.9.0/scout/adapter/mongo/user.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/variant.py` & `scout-browser-4.9.0/scout/adapter/mongo/variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,23 +493,25 @@
             variant_obj(dict)
 
         Returns:
             variants(iterable(dict))
         """
         #This is the category of the variants that we want to collect
         category = 'snv' if variant_obj['category'] == 'sv' else 'sv'
+        variant_type = variant_obj.get('variant_type', 'clinical')
+        hgnc_ids = variant_obj['hgnc_ids']
 
         query = {
             '$and': [
                 {'case_id': variant_obj['case_id']},
                 {'category': category},
-                {'hgnc_ids' : { '$in' : variant_obj['hgnc_ids']}}
+                {'variant_type': variant_type},
+                {'hgnc_ids' : { '$in' : hgnc_ids}}
             ]
         }
-
         sort_key = [('rank_score', pymongo.DESCENDING)]
         # We collect the 30 most severe overlapping variants
         variants = self.variant_collection.find(query).sort(sort_key).limit(30)
 
         return variants
 
     def evaluated_variants(self, case_id):
```

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/variant_events.py` & `scout-browser-4.9.0/scout/adapter/mongo/variant_events.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/mongo/variant_loader.py` & `scout-browser-4.9.0/scout/adapter/mongo/variant_loader.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/adapter/utils.py` & `scout-browser-4.9.0/scout/adapter/utils.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/acmg.py` & `scout-browser-4.9.0/scout/build/acmg.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/case.py` & `scout-browser-4.9.0/scout/build/case.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             panel['is_default'] = True
         else:
             panel['is_default'] = False
         panels.append(panel)
 
     case_obj['panels'] = panels
 
-    case_obj['dynamic_gene_list'] = {}
+    case_obj['dynamic_gene_list'] = []
 
     # Meta data
     genome_build = case_data.get('genome_build', '37')
     if not genome_build in ['37', '38']:
         pass
         ##TODO raise exception if invalid genome build was used
```

### Comparing `scout-browser-4.8.3/scout/build/disease.py` & `scout-browser-4.9.0/scout/build/disease.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/genes/exon.py` & `scout-browser-4.9.0/scout/build/genes/exon.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/genes/hgnc_gene.py` & `scout-browser-4.9.0/scout/build/genes/hgnc_gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/genes/transcript.py` & `scout-browser-4.9.0/scout/build/genes/transcript.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/hpo.py` & `scout-browser-4.9.0/scout/build/hpo.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/individual.py` & `scout-browser-4.9.0/scout/build/individual.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/institute.py` & `scout-browser-4.9.0/scout/build/institute.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/panel.py` & `scout-browser-4.9.0/scout/build/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/user.py` & `scout-browser-4.9.0/scout/build/user.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/variant/clnsig.py` & `scout-browser-4.9.0/scout/build/variant/clnsig.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/variant/compound.py` & `scout-browser-4.9.0/scout/build/variant/compound.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/variant/gene.py` & `scout-browser-4.9.0/scout/build/variant/gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/variant/genotype.py` & `scout-browser-4.9.0/scout/build/variant/genotype.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/variant/transcript.py` & `scout-browser-4.9.0/scout/build/variant/transcript.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/build/variant/variant.py` & `scout-browser-4.9.0/scout/build/variant/variant.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/base.py` & `scout-browser-4.9.0/scout/commands/base.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/convert.py` & `scout-browser-4.9.0/scout/commands/convert.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/delete/delete_command.py` & `scout-browser-4.9.0/scout/commands/delete/delete_command.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/export/case.py` & `scout-browser-4.9.0/scout/commands/export/case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/export/exon.py` & `scout-browser-4.9.0/scout/commands/export/exon.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/export/export_command.py` & `scout-browser-4.9.0/scout/commands/export/export_command.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/export/gene.py` & `scout-browser-4.9.0/scout/commands/export/gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/export/hpo.py` & `scout-browser-4.9.0/scout/commands/export/hpo.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/export/mitochondrial_report.py` & `scout-browser-4.9.0/scout/commands/export/mitochondrial_report.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/export/panel.py` & `scout-browser-4.9.0/scout/commands/export/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/export/transcript.py` & `scout-browser-4.9.0/scout/commands/export/transcript.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/export/variant.py` & `scout-browser-4.9.0/scout/commands/export/variant.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/index_command.py` & `scout-browser-4.9.0/scout/commands/index_command.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/base.py` & `scout-browser-4.9.0/scout/commands/load/base.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/case.py` & `scout-browser-4.9.0/scout/commands/load/case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/exons.py` & `scout-browser-4.9.0/scout/commands/load/exons.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/institute.py` & `scout-browser-4.9.0/scout/commands/load/institute.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/panel.py` & `scout-browser-4.9.0/scout/commands/load/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/region.py` & `scout-browser-4.9.0/scout/commands/load/region.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/report.py` & `scout-browser-4.9.0/scout/commands/load/report.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/research.py` & `scout-browser-4.9.0/scout/commands/load/research.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/user.py` & `scout-browser-4.9.0/scout/commands/load/user.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/load/variants.py` & `scout-browser-4.9.0/scout/commands/load/variants.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/serve.py` & `scout-browser-4.9.0/scout/commands/serve.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/setup/setup_scout.py` & `scout-browser-4.9.0/scout/commands/setup/setup_scout.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/base.py` & `scout-browser-4.9.0/scout/commands/update/base.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/case.py` & `scout-browser-4.9.0/scout/commands/update/case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/compounds.py` & `scout-browser-4.9.0/scout/commands/update/compounds.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/disease.py` & `scout-browser-4.9.0/scout/commands/update/disease.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/genes.py` & `scout-browser-4.9.0/scout/commands/update/genes.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/hpo.py` & `scout-browser-4.9.0/scout/commands/update/hpo.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/institute.py` & `scout-browser-4.9.0/scout/commands/update/institute.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/omim.py` & `scout-browser-4.9.0/scout/commands/update/omim.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/panel.py` & `scout-browser-4.9.0/scout/commands/update/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/phenotype_groups.py` & `scout-browser-4.9.0/scout/commands/update/phenotype_groups.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/update/user.py` & `scout-browser-4.9.0/scout/commands/update/user.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/aliases.py` & `scout-browser-4.9.0/scout/commands/view/aliases.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/base.py` & `scout-browser-4.9.0/scout/commands/view/base.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/case.py` & `scout-browser-4.9.0/scout/commands/view/case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/diseases.py` & `scout-browser-4.9.0/scout/commands/view/diseases.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/exons.py` & `scout-browser-4.9.0/scout/commands/view/exons.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/hgnc.py` & `scout-browser-4.9.0/scout/commands/view/hgnc.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/hpo.py` & `scout-browser-4.9.0/scout/commands/view/hpo.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/index.py` & `scout-browser-4.9.0/scout/commands/view/index.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/individuals.py` & `scout-browser-4.9.0/scout/commands/view/individuals.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/institutes.py` & `scout-browser-4.9.0/scout/commands/view/institutes.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/intervals.py` & `scout-browser-4.9.0/scout/commands/view/intervals.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/panels.py` & `scout-browser-4.9.0/scout/commands/view/panels.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/transcripts.py` & `scout-browser-4.9.0/scout/commands/view/transcripts.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/view/users.py` & `scout-browser-4.9.0/scout/commands/view/users.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/commands/wipe_database.py` & `scout-browser-4.9.0/scout/commands/wipe_database.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/__init__.py` & `scout-browser-4.9.0/scout/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/acmg.py` & `scout-browser-4.9.0/scout/constants/acmg.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/case_tags.py` & `scout-browser-4.9.0/scout/constants/case_tags.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/clinvar.py` & `scout-browser-4.9.0/scout/constants/clinvar.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/clnsig.py` & `scout-browser-4.9.0/scout/constants/clnsig.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/file_types.py` & `scout-browser-4.9.0/scout/constants/file_types.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/gene_tags.py` & `scout-browser-4.9.0/scout/constants/gene_tags.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/indexes.py` & `scout-browser-4.9.0/scout/constants/indexes.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/phenotype.py` & `scout-browser-4.9.0/scout/constants/phenotype.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/query_terms.py` & `scout-browser-4.9.0/scout/constants/query_terms.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/so_terms.py` & `scout-browser-4.9.0/scout/constants/so_terms.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/constants/variant_tags.py` & `scout-browser-4.9.0/scout/constants/variant_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,49 +83,49 @@
     'low',
     'medium',
     'high'
 )
 
 MANUAL_RANK_OPTIONS = {
     8: {
-        'label': 'known pathogenic',
+        'label': 'Known pathogenic',
         'description': 'Previously known pathogenic in Clinvar Hgmd literature etc',
     },
     7: {
-        'label': 'pathogenic',
+        'label': 'Pathogenic',
         'description': ("Novel mutation but overlapping phenotype with known pathogenic, "
                         "no further experimental validation needed"),
     },
     6: {
-        'label': 'novel validated pathogenic',
+        'label': 'Novel validated pathogenic',
         'description': 'Novel mutation and validated experimentally',
     },
     5: {
-        'label': 'pathogenic partial phenotype',
+        'label': 'Pathogenic partial phenotype',
         'description': ("Pathogenic variant explains part of patients phenotype, but "
                         "not all symptoms"),
     },
     4: {
-        'label': 'likely pathogenic',
+        'label': 'Likely pathogenic',
         'description': 'Experimental validation required to prove causality',
     },
     3: {
-        'label': 'possibly pathogenic',
+        'label': 'Possibly pathogenic',
         'description': 'Uncertain significance, but cannot disregard yet',
     },
     2: {
-        'label': 'likely benign',
+        'label': 'Likely benign',
         'description': 'Uncertain significance, but can discard',
     },
     1: {
-        'label': 'benign',
+        'label': 'Benign',
         'description': 'Does not cause phenotype',
     },
     0: {
-        'label': 'other',
+        'label': 'Other',
         'description': 'Phenotype not related to disease',
     },
 }
 
 DISMISS_VARIANT_OPTIONS = {
     2: {
         'label': 'Common public',
```

### Comparing `scout-browser-4.8.3/scout/constants/variants_export.py` & `scout-browser-4.9.0/scout/constants/variants_export.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.SV.vcf.gz` & `scout-browser-4.9.0/scout/demo/643594.clinical.SV.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.SV.vcf.gz.tbi` & `scout-browser-4.9.0/scout/demo/643594.clinical.SV.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.str.annotated.limits.vcf.gz` & `scout-browser-4.9.0/scout/demo/643594.clinical.str.annotated.limits.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.str.annotated.limits.vcf.gz.tbi` & `scout-browser-4.9.0/scout/demo/643594.clinical.str.annotated.limits.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.str.annotated.vcf.gz` & `scout-browser-4.9.0/scout/demo/643594.clinical.str.annotated.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.str.annotated.vcf.gz.tbi` & `scout-browser-4.9.0/scout/demo/643594.clinical.str.annotated.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.str.vcf.gz` & `scout-browser-4.9.0/scout/demo/643594.clinical.str.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.str.vcf.gz.tbi` & `scout-browser-4.9.0/scout/demo/643594.clinical.str.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.vcf.gz` & `scout-browser-4.9.0/scout/demo/643594.clinical.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.clinical.vcf.gz.tbi` & `scout-browser-4.9.0/scout/demo/643594.clinical.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.config.yaml` & `scout-browser-4.9.0/scout/demo/643594.config.yaml`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.research.SV.vcf.gz` & `scout-browser-4.9.0/scout/demo/643594.research.SV.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.research.SV.vcf.gz.tbi` & `scout-browser-4.9.0/scout/demo/643594.research.SV.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.research.vcf.gz` & `scout-browser-4.9.0/scout/demo/643594.research.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643594.research.vcf.gz.tbi` & `scout-browser-4.9.0/scout/demo/643594.research.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643595.clinical.vcf.gz` & `scout-browser-4.9.0/scout/demo/643595.clinical.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643595.clinical.vcf.gz.tbi` & `scout-browser-4.9.0/scout/demo/643595.clinical.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/643595.config.yaml` & `scout-browser-4.9.0/scout/demo/643595.config.yaml`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/__init__.py` & `scout-browser-4.9.0/scout/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/cancer.load_config.yaml` & `scout-browser-4.9.0/scout/demo/cancer.load_config.yaml`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/cancer_test.vcf.gz` & `scout-browser-4.9.0/scout/demo/cancer_test.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/cancer_test.vcf.gz.tbi` & `scout-browser-4.9.0/scout/demo/cancer_test.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/chanjo4_demo.sql` & `scout-browser-4.9.0/scout/demo/chanjo4_demo.sql`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/delivery_report.html` & `scout-browser-4.9.0/scout/demo/delivery_report.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/empty.clinical.SV.vcf.gz` & `scout-browser-4.9.0/scout/demo/empty.clinical.SV.vcf.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/madeline.xml` & `scout-browser-4.9.0/scout/demo/madeline.xml`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/panel_1.csv` & `scout-browser-4.9.0/scout/demo/panel_1.csv`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/panel_1.txt` & `scout-browser-4.9.0/scout/demo/panel_1.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/reduced_mt.bam` & `scout-browser-4.9.0/scout/demo/reduced_mt.bam`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/reduced_mt.bam.bai` & `scout-browser-4.9.0/scout/demo/reduced_mt.bam.bai`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_diseases_to_genes_to_phenotypes_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_diseases_to_genes_to_phenotypes_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_genes_to_phenotype_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_genes_to_phenotype_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_phenotype_to_genes_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_phenotype_to_genes_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/__init__.py` & `scout-browser-4.9.0/scout/demo/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/chanjo4_structure.sql` & `scout-browser-4.9.0/scout/demo/resources/chanjo4_structure.sql`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/ensembl_exons_37_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/ensembl_exons_37_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/ensembl_exons_38_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/ensembl_exons_38_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/ensembl_genes_37_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/ensembl_genes_37_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/ensembl_genes_38_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/ensembl_genes_38_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/ensembl_transcripts_37_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/ensembl_transcripts_37_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/ensembl_transcripts_38_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/ensembl_transcripts_38_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/forweb_cleaned_exac_r03_march16_z_data_pLI_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/forweb_cleaned_exac_r03_march16_z_data_pLI_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/genemap2_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/genemap2_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/hgnc_reduced_set.txt` & `scout-browser-4.9.0/scout/demo/resources/hgnc_reduced_set.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/hpo_terms.csv` & `scout-browser-4.9.0/scout/demo/resources/hpo_terms.csv`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/mim2gene_reduced.txt` & `scout-browser-4.9.0/scout/demo/resources/mim2gene_reduced.txt`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/demo/resources/reduced.hpo.obo` & `scout-browser-4.9.0/scout/demo/resources/reduced.hpo.obo`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/exceptions/database.py` & `scout-browser-4.9.0/scout/exceptions/database.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/export/exon.py` & `scout-browser-4.9.0/scout/export/exon.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/export/panel.py` & `scout-browser-4.9.0/scout/export/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/export/variant.py` & `scout-browser-4.9.0/scout/export/variant.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/load/all.py` & `scout-browser-4.9.0/scout/load/all.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/load/case.py` & `scout-browser-4.9.0/scout/load/case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/load/exon.py` & `scout-browser-4.9.0/scout/load/exon.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/load/hgnc_gene.py` & `scout-browser-4.9.0/scout/load/hgnc_gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/load/hpo.py` & `scout-browser-4.9.0/scout/load/hpo.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/load/institute.py` & `scout-browser-4.9.0/tests/build/test_build_institute.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-import logging
+import pytest
 from scout.build import build_institute
 
-log = logging.getLogger(__name__)
-
-
-def load_institute(adapter, internal_id, display_name, sanger_recipients=None):
-    """Load a institute into the database
-
-        Args:
-            adapter(MongoAdapter)
-            internal_id(str)
-            display_name(str)
-            sanger_recipients(list(email))
-    """
-
-    institute_obj = build_institute(
-        internal_id=internal_id,
-        display_name=display_name,
-        sanger_recipients=sanger_recipients
+def test_build_institute(parsed_institute):
+    ins = build_institute(
+        internal_id = parsed_institute['institute_id'],
+        display_name = parsed_institute['display_name'],
+        sanger_recipients = parsed_institute['sanger_recipients'],
+    )
+    
+    assert ins['internal_id'] == ins['_id'] == parsed_institute['institute_id']
+    assert isinstance(ins['sanger_recipients'], list)
+
+def test_build_institute_no_sanger():
+    ## GIVEN a institute without sanger recipients
+    institute_info = dict(
+            internal_id = 'cust000',
+            display_name = 'test'
+    )
+    ## WHEN building the institute
+    ins = build_institute(
+        internal_id = institute_info['internal_id'],
+        display_name = institute_info['display_name']
     )
-    log.info("Loading institute {0} with display name {1}" \
-             " into database".format(internal_id, display_name))
+    
+    assert 'sanger_recipients' not in ins
 
-    adapter.add_institute(institute_obj)
```

### Comparing `scout-browser-4.8.3/scout/load/panel.py` & `scout-browser-4.9.0/scout/load/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/load/report.py` & `scout-browser-4.9.0/scout/load/report.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/load/setup.py` & `scout-browser-4.9.0/scout/load/setup.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/load/transcript.py` & `scout-browser-4.9.0/scout/load/transcript.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/log/handlers.py` & `scout-browser-4.9.0/scout/log/handlers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/log/log.py` & `scout-browser-4.9.0/scout/log/log.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/acmg_evaluation.py` & `scout-browser-4.9.0/scout/models/acmg_evaluation.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/case/case.py` & `scout-browser-4.9.0/scout/models/case/case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/event.py` & `scout-browser-4.9.0/scout/models/event.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/hgnc_map.py` & `scout-browser-4.9.0/scout/models/hgnc_map.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/institute.py` & `scout-browser-4.9.0/scout/models/institute.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/panel.py` & `scout-browser-4.9.0/scout/models/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/phenotype_term.py` & `scout-browser-4.9.0/scout/models/phenotype_term.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/user.py` & `scout-browser-4.9.0/scout/models/user.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/variant/gene.py` & `scout-browser-4.9.0/scout/models/variant/gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/variant/transcript.py` & `scout-browser-4.9.0/scout/models/variant/transcript.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/models/variant/variant.py` & `scout-browser-4.9.0/scout/models/variant/variant.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/case.py` & `scout-browser-4.9.0/scout/parse/case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/clinvar.py` & `scout-browser-4.9.0/scout/parse/clinvar.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/cytoband.py` & `scout-browser-4.9.0/scout/parse/cytoband.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/ensembl.py` & `scout-browser-4.9.0/scout/parse/ensembl.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/exac.py` & `scout-browser-4.9.0/scout/parse/exac.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/hgnc.py` & `scout-browser-4.9.0/scout/parse/hgnc.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/hpo.py` & `scout-browser-4.9.0/scout/parse/hpo.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/matchmaker.py` & `scout-browser-4.9.0/scout/parse/matchmaker.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/omim.py` & `scout-browser-4.9.0/scout/parse/omim.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/panel.py` & `scout-browser-4.9.0/scout/parse/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/peddy.py` & `scout-browser-4.9.0/scout/parse/peddy.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/callers.py` & `scout-browser-4.9.0/scout/parse/variant/callers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/clnsig.py` & `scout-browser-4.9.0/scout/parse/variant/clnsig.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/compound.py` & `scout-browser-4.9.0/scout/parse/variant/compound.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/conservation.py` & `scout-browser-4.9.0/scout/parse/variant/conservation.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/coordinates.py` & `scout-browser-4.9.0/scout/parse/variant/coordinates.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/deleteriousness.py` & `scout-browser-4.9.0/scout/parse/variant/deleteriousness.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/frequency.py` & `scout-browser-4.9.0/scout/parse/variant/frequency.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/gene.py` & `scout-browser-4.9.0/scout/parse/variant/gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/genotype.py` & `scout-browser-4.9.0/scout/parse/variant/genotype.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/headers.py` & `scout-browser-4.9.0/scout/parse/variant/headers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/ids.py` & `scout-browser-4.9.0/scout/parse/variant/ids.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/transcript.py` & `scout-browser-4.9.0/scout/parse/variant/transcript.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/parse/variant/variant.py` & `scout-browser-4.9.0/scout/parse/variant/variant.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/resources/cytoBand.txt.gz` & `scout-browser-4.9.0/scout/resources/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/app.py` & `scout-browser-4.9.0/scout/server/app.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/alignviewers/partial.py` & `scout-browser-4.9.0/scout/server/blueprints/alignviewers/partial.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/alignviewers/templates/alignviewers/igv_viewer.html` & `scout-browser-4.9.0/scout/server/blueprints/alignviewers/templates/alignviewers/igv_viewer.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/alignviewers/views.py` & `scout-browser-4.9.0/scout/server/blueprints/alignviewers/views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/api/views.py` & `scout-browser-4.9.0/scout/server/blueprints/api/views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/controllers.py` & `scout-browser-4.9.0/scout/server/blueprints/cases/controllers.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,46 +30,64 @@
 STATUS_MAP = {'solved': 'bg-success', 'archived': 'bg-warning'}
 
 TRACKS = {
     'rare': 'Rare Disease',
     'cancer': 'Cancer',
 }
 
-def cases(store, case_query, limit=100):
+def cases(store, case_query, prioritized_cases_query=None, limit=100):
     """Preprocess case objects.
 
     Add the necessary information to display the 'cases' view
 
     Args:
         store(adapter.MongoAdapter)
         case_query(pymongo.Cursor)
+        prioritized_cases_query(pymongo.Cursor)
         limit(int): Maximum number of cases to display
 
     Returns:
         data(dict): includes the cases, how many there are and the limit.
     """
-
     case_groups = {status: [] for status in CASE_STATUSES}
     nr_cases = 0
-    for nr_cases, case_obj in enumerate(case_query.limit(limit),1):
 
+    # local function to add info to case obj
+    def populate_case_obj(case_obj):
         analysis_types = set(ind['analysis_type'] for ind in case_obj['individuals'])
         LOG.debug("Analysis types found in %s: %s", case_obj['_id'], ','.join(analysis_types))
         if len(analysis_types) > 1:
             LOG.debug("Set analysis types to {'mixed'}")
             analysis_types = set(['mixed'])
 
         case_obj['analysis_types'] = list(analysis_types)
         case_obj['assignees'] = [store.user(user_email) for user_email in
-                                 case_obj.get('assignees', [])]
+                                     case_obj.get('assignees', [])]
         case_obj['is_rerun'] = len(case_obj.get('analyses', [])) > 0
         case_obj['clinvar_variants'] = store.case_to_clinVars(case_obj['_id'])
         case_obj['display_track'] = TRACKS[case_obj.get('track', 'rare')]
+        return case_obj
+
+    for nr_cases, case_obj in enumerate(case_query.limit(limit),1):
+        case_obj = populate_case_obj(case_obj)
         case_groups[case_obj['status']].append(case_obj)
 
+    if prioritized_cases_query:
+        extra_prioritized = 0
+        for case_obj in prioritized_cases_query:
+            if any(group_obj.get('display_name') == case_obj.get('display_name')
+                for group_obj in case_groups[case_obj['status']]):
+                    continue
+            else:
+                extra_prioritized += 1
+                case_obj = populate_case_obj(case_obj)
+                case_groups[case_obj['status']].append(case_obj)
+        # extra prioritized cases are potentially shown in addition to the case query limit
+        nr_cases += extra_prioritized
+
     data = {
         'cases': [(status, case_groups[status]) for status in CASE_STATUSES],
         'found_cases': nr_cases,
         'limit': limit,
     }
     return data
 
@@ -140,26 +158,26 @@
                                 .format(hpo_term['phenotype_id']))
 
     rank_model_link_prefix = current_app.config.get('RANK_MODEL_LINK_PREFIX')
     if case_obj.get('rank_model_version'):
         rank_model_link_postfix = current_app.config.get('RANK_MODEL_LINK_POSTFIX','')
         case_obj['rank_model_link'] = ''.join(
             [
-                rank_model_link_prefix, 
-                str(case_obj['rank_model_version']), 
+                rank_model_link_prefix,
+                str(case_obj['rank_model_version']),
                 rank_model_link_postfix
             ]
         )
     sv_rank_model_link_prefix = current_app.config.get('SV_RANK_MODEL_LINK_PREFIX','')
     if case_obj.get('sv_rank_model_version'):
         sv_rank_model_link_postfix = current_app.config.get('SV_RANK_MODEL_LINK_POSTFIX','')
         case_obj['sv_rank_model_link'] = ''.join(
             [
-                sv_rank_model_link_prefix, 
-                str(case_obj['sv_rank_model_version']), 
+                sv_rank_model_link_prefix,
+                str(case_obj['sv_rank_model_version']),
                 sv_rank_model_link_postfix
             ]
         )
     # other collaborators than the owner of the case
     o_collaborators = []
     for collab_id in case_obj.get('collaborators',[]):
         if collab_id != case_obj['owner'] and store.institute(collab_id):
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/forms.py` & `scout-browser-4.9.0/scout/server/blueprints/cases/forms.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/static/madeline.js` & `scout-browser-4.9.0/scout/server/blueprints/cases/static/madeline.js`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/static/madeline.svg` & `scout-browser-4.9.0/scout/server/blueprints/cases/static/madeline.svg`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/case.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/case.html`

 * *Files 0% similar despite different names*

```diff
@@ -653,15 +653,15 @@
                 </button>
                 <ul class="dropdown-menu">
                   <li><a href="{{ url_for('cases.matchmaker_match', institute_id=institute._id, case_name=case.display_name, target='internal') }}">Scout patients in MatchMaker</a></li>
                   {% if mme_nodes|length >1 %}
                     <li><a href="{{ url_for('cases.matchmaker_match', institute_id=institute._id, case_name=case.display_name, target='external') }}">All external nodes</a></li>
                   {% endif %}
                   {% for node in mme_nodes %}
-                    <li><a href="{{ url_for('cases.matchmaker_match', institute_id=institute._id, case_name=case.display_name, target=node.id) }}">External node-> {{node.description}}</a></li>
+                    <li><a href="{{ url_for('cases.matchmaker_match', institute_id=institute._id, case_name=case.display_name, target=node.id) }}">{{node.description}}</a></li>
                   {% endfor %}
                 </ul>
               </div>
               <a class="btn btn-outline-secondary" href="#mme_form" data-toggle="collapse">Modify submission</a>
             </div>
           </div>
         </p>
@@ -873,15 +873,15 @@
       <div class="panel-heading panel-heading-secondary"  data-toggle='tooltip' title="Manually add a gene to the dynamic (HPO) panel.
       To remove, use the HPO panel button to regenerate a list without them.">
           Add gene to the dynamic panel
       </div>
       <div class="card-body">
         <div class="form-inline">
           <div class="form-group col-8">
-            <input name="genes" class="typeahead_gene form-control" data-provide="typeahead" autocomplete="off" placeholder="Search...">
+            <input name="genes" pattern="^[0-9]+\s*\|\s*.*" class="typeahead_gene form-control" data-provide="typeahead" autocomplete="off" placeholder="Search...">
           </div>
           <div class="form-group col-4">
             <button class="btn btn-secondary form-control" type="submit" name="action" value="ADDGENE">Add gene</button>
           </div>
         </div>
       </div>
   </div>
@@ -968,15 +968,15 @@
   </div>
 {% endmacro %}
 
 {% macro genepanels_table() %}
   <div class="card panel-default">
     <div class="panel-heading">Gene panels</div>
     <div class="table-responsive fixed-panel">
-      <table id="panel-table" class="table">
+      <table id="panel-table" class="table tablesorter">
         <thead>
           <tr>
             <th>Panel</th>
             <th>Version</th>
             <th>Genes</th>
           </tr>
         </thead>
@@ -1026,14 +1026,22 @@
 
 {% block scripts %}
 {{ super() }}
 <script src="{{ url_for('cases.static', filename='madeline.js') }}"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/sticky-table-headers/0.1.19/js/jquery.stickytableheaders.min.js"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-3-typeahead/4.0.2/bootstrap3-typeahead.min.js"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-multiselect/0.9.13/js/bootstrap-multiselect.min.js"></script>
+<script src="https://mottie.github.io/tablesorter/js/jquery.tablesorter.js"></script>
+
+<script>
+    $(function() {
+    $("#panel-table").tablesorter({ sortList: [[0,0]]})
+  })
+</script>
+
 <script>
 $(function () {
       function getTerms(query, process) {
         $.get("{{ url_for('cases.hpoterms') }}", {query: query}, function(data) {
           process(data)
         });
       }
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/case_ideograms.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/case_ideograms.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/case_report.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/case_report.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/cases.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/cases.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/causatives.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/causatives.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/clinvar_submissions.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/clinvar_submissions.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/collapsible_actionbar.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/collapsible_actionbar.html`

 * *Files 0% similar despite different names*

```diff
@@ -289,16 +289,18 @@
 {% macro research_modal(institute, case) %}
   <form action="{{ url_for('cases.research', institute_id=institute._id,
                            case_name=case.display_name) }}" method="POST">
     <div class="modal fade" id="research-modal">
       <div class="modal-dialog">
         <div class="modal-content">
           <div class="modal-header">
-            <button type="button" class="close" data-dismiss="modal">&times;</button>
             <h4 class="modal-title">Request research list</h4>
+            <button type="button" class="close" data-dismiss="modal" aria-label="Close">
+              <span aria-hidden="true">&times;</span>
+            </button>
           </div>
           <div class="modal-body">
             <p>Please confirm that you want to <strong>upload research variants for {{ case.display_name }}</strong>.</p>
             <p>You also confirm that you have the <strong>relevant consent</strong>.</p>
           </div>
           <div class="modal-footer">
             <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
@@ -313,16 +315,18 @@
 {% macro rerun_modal(institute, case) %}
   <form action="{{ url_for('cases.rerun', institute_id=institute._id,
                            case_name=case.display_name) }}" method="POST">
     <div id="rerun-modal" class="modal fade">
       <div class="modal-dialog">
         <div class="modal-content">
           <div class="modal-header">
-            <button type="button" class="close" data-dismiss="modal">&times;</button>
             <h4 class="modal-title">Request rerun</h4>
+            <button type="button" class="close" data-dismiss="modal" aria-label="Close">
+              <span aria-hidden="true">&times;</span>
+            </button>
           </div>
           <div class="modal-body">
             <p>Please confirm that you want to <strong>rerun {{ case.display_name }}</strong>. This will <strong>replace current variants</strong> with updated information.</p>
           </div>
           <div class="modal-footer">
             <button type="button" class="btn btn-default" data-dismiss="modal">Close</button>
             <button type="submit" class="btn btn-primary">Confirm</button>
```

#### html2text {}

```diff
@@ -65,23 +65,23 @@
 {% endif %}
 {% endmacro %} {% macro check_decipher(case, institute) %}
 div class="d-flex w-100 justify-content-start align-items-center">  Decipher
 check
 
   Decipher Checked
 {% endmacro %} {% macro research_modal(institute, case) %}
-×
 *** Request research list ***
+ ×
 Please confirm that you want to upload research variants for {
 { case.display_name }}.
 You also confirm that you have the relevant consent.
 Close Confirm
 {% endmacro %} {% macro rerun_modal(institute, case) %}
-×
 *** Request rerun ***
+ ×
 Please confirm that you want to rerun {{ case.display_name }}. This will
 replace current variants with updated information.
 Close Confirm
 {% endmacro %} {% macro confirm_inactivate(institute, case) %}
 ** Confirm inactivate case **
  ×
 You are the last user working on this case, do you wish to inactivate it?
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/diseases.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/diseases.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/gene_variants.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/gene_variants.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/index.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/index.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/templates/cases/matchmaker.html` & `scout-browser-4.9.0/scout/server/blueprints/cases/templates/cases/matchmaker.html`

 * *Files 10% similar despite different names*

```diff
@@ -23,27 +23,26 @@
     <span class="navbar-text">MatchMaker</span>
   </li>
 {% endblock %}
 
 {% block content_main %}
 {% set panel = panel|int %}
 <div class="container-float">
-  <div class="card mt-3">
+  <div class="card">
     <div class="card-body">
       <nav aria-label="breadcrumb">
         <ol class="breadcrumb">
           <li class="breadcrumb-item">Submitted: <strong>{{case.mme_submission.created_at.strftime('%Y-%m-%d %H:%M')}}</strong></li>
           <li class="breadcrumb-item">Last updated: <strong>{{case.mme_submission.updated_at.strftime('%Y-%m-%d %H:%M')}}</strong></li>
         </ol>
       </nav>
-      <br>
       <ul class="nav nav-tabs" id="myTab" role="tablist">
-        <li class="nav-item"><a href="#" class="nav-link {% if panel == 1 %}active{% endif %}" data-toggle="tab" onclick="hide_div(1)"><h4>Patient Overview</h4></a></li>
-        <li class="nav-item"><a href="#" class="nav-link {% if panel == 2 %}active{% endif %}" data-toggle="tab" onclick="hide_div(2)"><h4>External Matches</h4></a></li>
-        <li class="nav-item"><a href="#" class="nav-link {% if panel == 3 %}active{% endif %}" data-toggle="tab" onclick="hide_div(3)"><h4>Internal Matches</h4></a></li>
+        <li class="nav-item"><a href="#" class="nav-link {% if panel == 1 %}active{% endif %}" data-toggle="tab" onclick="hide_div(1)"><h4>Patient Overview <i class="fa fa-id-card-o" aria-hidden="true"></i></h4></a></li>
+        <li class="nav-item"><a href="#" class="nav-link {% if panel == 2 %}active{% endif %}" data-toggle="tab" onclick="hide_div(2)"><h4>Global matches <i class="fa fa-globe" aria-hidden="true"></i></h4></a></li>
+        <li class="nav-item"><a href="#" class="nav-link {% if panel == 3 %}active{% endif %}" data-toggle="tab" onclick="hide_div(3)"><h4>Local matches <i class="fa fa-hospital-o" aria-hidden="true"></i></h4></a></li>
       </ul>
       <div class="tab-content" id="tabs">
         <div class="tab-pane" id="1">
           {{ patient_data() }}
         </div>
         <div class="tab-pane" id="2">
           {{ show_matches('external') }}
@@ -53,75 +52,86 @@
         </div>
       </div>
     </div>
   </div>
 </div>
 {% endblock %}
 
-
 {% macro patient_data() %}
-<br>
-<div class="ml-3">
-  <p>Features (HPO terms):
-    {% for hpo in case.mme_submission.features %}
-      <span class="badge badge-primary">{{hpo.id}}</span>
-    {% endfor %}
-  </p>
-  <p>Disorders (OMIM terms):
-    {% for omim in case.mme_submission.disorders %}
-      <span class="badge badge-info">{{omim.id}}</span>
-    {% endfor %}
-  </p>
-  <p>Submitted patients:
+<div class="ml-3 mt-3">
+  <div class="row">
+    <div class="col">
+      <h5>Patients</h5>
+      {% for patient in case.mme_submission.patients %}
+        <ul class="list-group">
+          <li class="list-group-item">Patient id: <strong>{{patient.id}}</strong></li>
+          <li class="list-group-item">Patient label: <strong>{{patient.label}}</strong></li>
+          <li class="list-group-item">Sex: <strong>{{patient.sex}}</strong></li>
+        </ul>
+      {% endfor %}
+    </div>
+    <div class="col">
+      <h5>Phenotype features (HPO terms)</h5>
+        {% for hpo in case.mme_submission.features %}
+          <a class="text-white" target="_blank" href="http://hpo.jax.org/app/browse/term/{{hpo.id}}">
+            <span class="badge badge-sm badge-info">{{hpo.id}}</span>
+          </a>
+        {% endfor %}
+    </div>
+    <div class="col">
+      <h5>Diagnoses (OMIM terms)</h5>
+      {% for omim in case.mme_submission.disorders %}
+        <a class="text-white" target="_blank" href="http://omim.org/entry/{{omim.id[4:]}}">
+          <span class="badge badge-sm badge-secondary">{{omim.id}}</span>
+        </a>
+      {% endfor %}
+    </div>
+  </div>
+  <br>
+  <div>
+    <h5>Candidate genes/variants</h5>
     {% for patient in case.mme_submission.patients %}
-      <ul class="list-group list-group-flush">
-        <li class="list-group-item">Patient id: <strong>{{patient.id}}</strong></li>
-        <li class="list-group-item">Patient label: <strong>{{patient.label}}</strong></li>
-        <li class="list-group-item">Sex: <strong>{{patient.sex}}</strong></li>
-        <div class="list-group-item">genomic features:<br>
-            <div class="row">
-            {% for g_feat in patient.genomicFeatures %}
-              <div class="card">
-                  <div class="card-body">
-                    {% for key, value in g_feat.items() %}
-                      {% if key == 'gene' %}
-                        {{key}}:&nbsp;<span class="badge badge-secondary">{{value.id}}</span>
-                        <hr>
-                      {% elif key == 'variant' %}
-                        {% for ikey, item in value.items() %}
-                          {{ikey}}:<strong>{{item}}</strong><br>
-                        {% endfor %}
-                      {% elif key == 'type' %} <!-- this will be variant effect -->
-                        {{key}}:<strong>{{value.label}}</strong>
-                        <br>
-                      {% else %} <!-- this will be zygosity -->
-                        {{key}}:<strong>{{value}}</strong>
-                        {% if value == 1 %}
-                          (heteroz. or hemiz. if on X in males)
-                        {% elif value == 2 %}
-                          (homozygous)
-                        {% endif %}
-                      {% endif %}
+      <div class="row">
+        {% for g_feat in patient.genomicFeatures %}
+          <div class="col">
+            <ul class="list-group">
+              {% for key, value in g_feat.items() %}
+                <li class="list-group-item py-2">
+                  {% if key == 'gene' %}
+                    <span class="badge badge-secondary">{{value.id}}</span>
+                  {% elif key == 'variant' %}
+                    {% for ikey, item in value.items() %}
+                      {{ikey}}:<strong>{{item}}</strong><br>
                     {% endfor %}
-                  </div>
-              </div>
-            {% endfor %}
-            </div>
-        </div>
-      </ul>
+                  {% elif key == 'type' %} <!-- this will be variant effect -->
+                    {{key}}:<strong>{{value.label}}</strong>
+                    <br>
+                  {% else %} <!-- this will be zygosity -->
+                    {{key}}:<strong>{{value}}</strong>
+                    {% if value == 1 %}
+                      (heteroz. or hemiz. if on X in males)
+                    {% elif value == 2 %}
+                      (homozygous)
+                    {% endif %}
+                  {% endif %}
+                </li>
+              {% endfor %}
+            </ul>
+          </div>
+      {% endfor %}
+      </div>
     {% endfor %}
-  </p>
+  </div>
 </div>
 {% endmacro %}
 
 {% macro show_matches(type) %}
 <!-- show matches of the selected type from the most recent -->
-<br>
 {% set matching_patients = [] %}
-  <div class="m-3">
+  <div class="m-3 mt-3">
   {% for patient, match_objs in matches.items() %}
     <div class="panel-group">
     {% set p_name = patient.split('.') %}
     <h4> Showing {{type}} matches for patient {{ p_name[1] }}:</h4>
     {% for match_obj in match_objs %}
       {% if match_obj.match_type == type %}
         {% do matching_patients.append(match_obj.patient_id) %}
@@ -132,102 +142,95 @@
                 <button class="btn btn-link collapsed" type="button" data-toggle="collapse" data-target="#div_{{match_obj.match_oid}}" aria-expanded="false" aria-controls="collapseTwo">
                   Match {{match_obj.match_date.strftime('%Y-%m-%d %H:%M')}}
                 </button>
               </h2>
             </div>
             <div id="div_{{match_obj.match_oid}}" class="collapse" aria-labelledby="heading_{{match_obj.match_oid}}" data-parent="#accordionExample">
               <div class="card-body">
-                {% for match_result in match_obj.patients %}
-                   <table class="table table-condensed">
-                     <thead>
-                       <tr>
-                         <th scope="col">Score</th>
-                         <th scope="col">Patient ID</th>
-                         <th scope="col">MME node</th>
-                         <th scope="col">Contact</th>
-                       </tr>
-                     </thead>
-                     <tbody>
-                       <tr>
-                         <td><span class="badge badge-primary badge-pill">{{match_result.score.patient|round(4)}}</badge></td>
-                         <td><strong>{{match_result.patient_id}}</strong></td>
-                         <td>{{match_result.node.label}}</td>
-                         <td>{{match_result.patient.contact.name}}
+                <table class="table table-sm table-borderless">
+                  <thead>
+                    <tr>
+                      <th scope="col" style="width: 5%">Score</th>
+                      <th scope="col" style="width: 10%">Node</th>
+                      <th scope="col" style="width: 15%">ID</th>
+                      <th scope="col" style="width: 20%">Contact</th>
+                      <th scope="col" style="width: 35%">Phenotypes</th>
+                      <th scope="col" style="width: 15%">Diagnoses</th>
+                      <th></th>
+                    </tr>
+                  </thead>
+                  <tbody>
+                    {% for match_result in match_obj.patients %}
+                       <tr class="{{ loop.cycle('odd', 'even') }}">
+                         <td style="width: 5%"><span class="badge badge-primary badge-pill">{{match_result.score.patient|round(4)}}</badge></td>
+                         <td style="width: 10%">{{match_result.node.label}}</td>
+                         <td style="width: 15%">
+                           {% if "http" in match_result.patient_id %}
+                            <a href="{{match_result.patient_id}}" target="_blank">link</a>
+                           {% else %}
+                            <strong>{{match_result.patient_id}}</strong></td>
+                           {% endif %}
+                         <td style="width: 20%">
+                           {{match_result.patient.contact.name}}<br>
+                           {% if "http" in match_result.patient.contact.href %}
+                            <a href="{{match_result.patient.contact.href}}" target="_blank">contact link</a>
+                           {% else %}
+                            {{match_result.patient.contact.href}}
+                           {% endif %}
                            {% if match_result.patient.contact.institution %}
                              <br>{{match_result.patient.contact.institution}}
                            {% endif %}
-                           <br>{{match_result.patient.contact.href}}
-                         </td>
-                       </tr>
-                     </tbody>
-                   </table>
-                   <table class="table table-condensed">
-                     <thead>
-                       <tr>
-                         <th style="width: 30%">Diagnoses</th>
-                         <th style="width: 30%">Features</th>
-                         <th style="width: 40%">Genomic Features</th>
-                       </tr>
-                     </thead>
-                     <tbody>
-                       <tr>
-                         <td>
-                           {% for omim in match_result.patient.disorders %}
-                             <span data-toggle="tooltip" title="{{omim.label or 'description not available'}}" class="badge badge-info">{{omim.id}}</span>
-                           {% endfor %}
+                           {% if match_result.patient.contact.email %}
+                             <br>{{match_result.patient.contact.email|replace("mailto:","")}}
+                           {% endif %}
                          </td>
-                         <td>
+                         <td style="width: 35%">
                            {% for feature in match_result.patient.features %}
-                             <span data-toggle="tooltip" title="{{feature.label or 'description not available'}}" class="badge badge-primary">{{feature.label}}({{feature.id}})</span>
+                             <span data-toggle="tooltip" title="{{feature.label or 'description not available'}}" class="badge badge-info">{{feature.label}}({{feature.id}})</span>
+                           {% else %}
+                            -
                            {% endfor %}
                          </td>
-                         <td>
-                           <div class="card-columns">
-                           {% for g_feat in match_result.patient.genomicFeatures %}
-                            {% if g_feat %}
-
-                                <div class="card w-100">
-                                  <div class="card-body">
-                                    {% for key, value in g_feat.items() %}
-                                      {% if key == 'gene' %} <!-- genomic feature gene-->
-                                        {{key}}:&nbsp;<span class="badge badge-secondary">{{value.id}}</span>
-                                        <hr>
-                                      {% elif key == 'variant' %} <!-- genomic feature variant-->
-                                        {% for ikey, item in value.items() %}
-                                          {% if not ikey == 'shareVariantLevelData' %}
-                                            {{ikey}}:<strong>{{item}}</strong><br>
-                                          {% endif %}
-                                        {% endfor %}
-                                      {% elif key == 'zygosity' %} <!-- genomic feature zygosity-->
-                                        {{key}}:<strong>{{value}}</strong>
-                                        {% if value == 1 %}
-                                          (heteroz. or hemiz. if on X in males)
-                                        {% elif value == 2 %}
-                                          (homozygous)
-                                        {% endif %}
-                                      {% else %} <!-- genomic feature type-->
-                                        {{key}}:<strong>{{value.label}}</strong>
-                                        <br>
-                                      {% endif %}
-                                    {% endfor %}
-                                  </div>
-                                </div>
-
-                            {% endif %}
+                         <td style="width: 15%">
+                           {% for omim in match_result.patient.disorders %}
+                             <a class="text-white" target="_blank" href="http://omim.org/entry/{{omim.id[4:]}}">
+                               <span class="badge badge-sm badge-secondary">{{omim.id}}</span>
+                             </a>
+                           {% else %}
+                            -
                            {% endfor %}
-                           </div>
-                          </div> <!--end of card body -->
                          </td>
                        </tr>
-                     </tbody>
-                   </table>
-                   <br>
-                   <br>
-                   <hr>
-                {% endfor %} <!-- end of for patient in match_obj.patients -->
+                       <!-- Display candidate genes for matches -->
+                       {% if match_result.patient.genomicFeatures%}
+                         <tr class="{{ loop.cycle('odd', 'even') }}">
+                           <td style="width: 20%"><strong>Gene/Variants:</strong></td>
+                           <td colspan="5">
+                              {% for g_feat in match_result.patient.genomicFeatures %}
+                                <div class="row">
+                                  <div>{{loop.index}}</div>
+                                  <div class="col"><!--gene info-->
+                                    <strong>{{ g_feat.gene._geneName}}</strong>
+                                    <a class="text-white" target="_blank" href="https://grch37.ensembl.org/Homo_sapiens/Gene/Summary?db=core;g={{g_feat.gene.id}}">
+                                      <span class="badge badge-sm badge-secondary">{{g_feat.gene.id}}</span>
+                                    </a>,
+                                    <strong>Variant:</strong>{{g_feat.variant|replace("'", "") or '-'}},
+                                    <strong>Type:</strong>{{g_feat.type|replace("'", "") or '-'}},
+                                    <strong>zygosity:</strong>{{g_feat.zygosity or '-'}}
+                                  </div>
+                                </div>
+                              {% endfor %}
+                            </div>
+                         </tr>
+                        {% else %}
+                          No gene/variant info available
+                        {% endif %}
+                    {% endfor %} <!-- end of for patient in match_obj.patients -->
+                  </tbody>
+                </table>
               </div>
             </div>
           </div>
         </div>
         <br>
       {% endif %} <!-- end of if match_obj.match_type == type -->
     {% endfor %} <!-- end of for match_obj in match_objs -->
```

#### html2text {}

```diff
@@ -5,76 +5,72 @@
 {{_institute.display_name_}}
 {{_case.display_name_}}
 MatchMaker
 {% endblock %} {% block content_main %} {% set panel = panel|int %}
    1. Submitted: {{case.mme_submission.created_at.strftime('%Y-%m-%d %H:%M')}}
    2. Last updated: {{case.mme_submission.updated_at.strftime('%Y-%m-%d %H:
       %M')}}
-
-    * ***_Patient_Overview_***
-    * ***_External_Matches_***
-    * ***_Internal_Matches_***
+    * Patient_Overview
+    * Global_matches
+    * Local_matches
 {{ patient_data() }}
 {{ show_matches('external') }}
 {{ show_matches('internal') }}
 {% endblock %} {% macro patient_data() %}
-Features (HPO terms): {% for hpo in case.mme_submission.features %} {{hpo.id}}
-{% endfor %}
-Disorders (OMIM terms): {% for omim in case.mme_submission.disorders %} {
-{omim.id}} {% endfor %}
-Submitted patients: {% for patient in case.mme_submission.patients %}
+** Patients **
+{% for patient in case.mme_submission.patients %}
     * Patient id: {{patient.id}}
     * Patient label: {{patient.label}}
     * Sex: {{patient.sex}}
-      genomic features:
-      {% for g_feat in patient.genomicFeatures %}
-      {% for key, value in g_feat.items() %} {% if key == 'gene' %} {{key}}: {
-      {value.id}}
-      =========================================================================
-      {% elif key == 'variant' %} {% for ikey, item in value.items() %} {
-      {ikey}}:{{item}}
+{% endfor %}
+** Phenotype features (HPO terms) **
+{% for hpo in case.mme_submission.features %} {{hpo.id}} {% endfor %}
+** Diagnoses (OMIM terms) **
+{% for omim in case.mme_submission.disorders %} {{omim.id}} {% endfor %}
+
+** Candidate genes/variants **
+{% for patient in case.mme_submission.patients %}
+{% for g_feat in patient.genomicFeatures %}
+    * {% for key, value in g_feat.items() %}
+    * {% if key == 'gene' %} {{value.id}} {% elif key == 'variant' %} {% for
+      ikey, item in value.items() %} {{ikey}}:{{item}}
       {% endfor %} {% elif key == 'type' %}  {{key}}:{{value.label}}
       {% else %}  {{key}}:{{value}} {% if value == 1 %} (heteroz. or hemiz. if
       on X in males) {% elif value == 2 %} (homozygous) {% endif %} {% endif %}
-      {% endfor %}
-      {% endfor %}
+    * {% endfor %}
 {% endfor %}
-{% endmacro %} {% macro show_matches(type) %}
-{% set matching_patients = [] %}
+{% endfor %}
+{% endmacro %} {% macro show_matches(type) %}  {% set matching_patients = [] %}
 {% for patient, match_objs in matches.items() %}
 {% set p_name = patient.split('.') %}
 *** Showing {{type}} matches for patient {{ p_name[1] }}: ***
 {% for match_obj in match_objs %} {% if match_obj.match_type == type %} {% do
 matching_patients.append(match_obj.patient_id) %}
 *****  Match {{match_obj.match_date.strftime('%Y-%m-%d %H:%M')}}  *****
-{% for match_result in match_obj.patients %}
-Score                             Patient ID                 MME node                   Contact
-                                                                                        {{match_result.patient.contact.name}} {% if
-                                                                                        match_result.patient.contact.institution %}
-{                                 {                          {
-{match_result.score.patient|round {match_result.patient_id}} {match_result.node.label}} {
-(4)}}                                                                                   {match_result.patient.contact.institution}}
-                                                                                        {% endif %}
-                                                                                        {{match_result.patient.contact.href}}
-Diagnoses                      Features                      Genomic Features
-                                                             {% for g_feat in match_result.patient.genomicFeatures %} {% if g_feat %}
-                                                             {% for key, value in g_feat.items() %} {% if key == 'gene' %}  {{key}}: {
-                                                             {value.id}}
-                               {% for feature in             ==========================================================================
-{% for omim in                 match_result.patient.features {% elif key == 'variant' %}  {% for ikey, item in value.items() %} {% if
-match_result.patient.disorders %} {{feature.label}}({        not ikey == 'shareVariantLevelData' %} {{ikey}}:{{item}}
-%} {{omim.id}} {% endfor %}    {feature.id}}) {% endfor %}   {% endif %} {% endfor %} {% elif key == 'zygosity' %}  {{key}}:{{value}}
-                                                             {% if value == 1 %} (heteroz. or hemiz. if on X in males) {% elif value ==
-                                                             2 %} (homozygous) {% endif %} {% else %}  {{key}}:{{value.label}}
-                                                             {% endif %} {% endfor %}
-                                                             {% endif %} {% endfor %}
-
-
-===============================================================================
-{% endfor %}
+Score                             Node                       ID                         Contact                                     Phenotypes                    Diagnoses
+                                                                                        {{match_result.patient.contact.name}}
+                                                                                        {% if "http" in
+                                                                                        match_result.patient.contact.href %}
+                                                                                        contact_link {% else %} {
+                                                                                        {match_result.patient.contact.href}} {%
+                                                             {% if "http" in            endif %} {% if                              {% for feature in             {% for omim in
+{                                 {                          match_result.patient_id %} match_result.patient.contact.institution %} match_result.patient.features match_result.patient.disorders
+{match_result.score.patient|round {match_result.node.label}} link {% else %} {                                                      %} {{feature.label}}({        %} {{omim.id}} {% else %} - {%
+(4)}}                                                        {match_result.patient_id}} {                                           {feature.id}}) {% else %} -   endfor %}
+                                                                                        {match_result.patient.contact.institution}} {% endfor %}
+                                                                                        {% endif %} {% if
+                                                                                        match_result.patient.contact.email %}
+                                                                                        {
+                                                                                        {match_result.patient.contact.email|replace
+                                                                                        ("mailto:","")}} {% endif %}
+                                  {% for g_feat in match_result.patient.genomicFeatures %}
+                                  {{loop.index}}
+Gene/Variants:                    {{ g_feat.gene._geneName}} {{g_feat.gene.id}}, Variant:{{g_feat.variant|replace("'", "") or '-'}}, Type:{{g_feat.type|replace("'", "") or '-'}}, zygosity:{
+                                  {g_feat.zygosity or '-'}}
+                                  {% endfor %}
 
 {% endif %}  {% endfor %}  {% if not matching_patients %}
 
 No matches available for this patient. {% endif %}
 {% endfor %}
 {% endmacro %} {% block scripts %} {{ super() }}
  {% endblock %}
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/cases/views.py` & `scout-browser-4.9.0/scout/server/blueprints/cases/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,18 @@
             all_cases.sort('analysis_date', pymongo_sort)
         elif sort_by == 'track':
             all_cases.sort('track', pymongo_sort)
         elif sort_by == 'status':
             all_cases.sort('status', pymongo_sort)
 
     LOG.debug("Prepare all cases")
-    data = controllers.cases(store, all_cases, limit)
+
+    prioritized_cases = store.prioritized_cases(institute_id=institute_id)
+
+    data = controllers.cases(store, all_cases, prioritized_cases, limit)
     data['sort_order'] = sort_order
     data['sort_by'] = sort_by
     data['nr_cases'] = store.nr_cases(institute_id=institute_id)
 
     sanger_unevaluated = controllers.get_sanger_unevaluated(store, institute_id, current_user.email)
     if len(sanger_unevaluated)> 0:
         data['sanger_unevaluated'] = sanger_unevaluated
@@ -575,27 +578,35 @@
     elif action == 'ADDGENE':
         hgnc_symbol = None
         for raw_symbol in request.form.getlist('genes'):
             LOG.debug("raw gene: {}".format(raw_symbol))
             # avoid empty lists
             if raw_symbol:
                 # take the first nubmer before |, and remove any space.
-                hgnc_symbol_split = raw_symbol.split('|', 1)[0]
-                hgnc_symbol = int(hgnc_symbol_split.replace(' ', ''))
+                try:
+                    hgnc_symbol_split = raw_symbol.split('|', 1)[0]
+                    hgnc_symbol = int(hgnc_symbol_split.replace(' ', ''))
+                except ValueError:
+                    flash("Provided gene info could not be parsed! "
+                          "Please allow autocompletion to finish.", 'warning')
             LOG.debug("Parsed HGNC symbol {}".format(hgnc_symbol))
             store.update_dynamic_gene_list(case_obj, hgnc_ids=[hgnc_symbol], add_only=True)
 
     elif action == 'GENES':
         hgnc_symbols = set()
         for raw_symbols in request.form.getlist('genes'):
             LOG.debug("raw gene list: {}".format(raw_symbols))
             # avoid empty lists
             if raw_symbols:
-                hgnc_symbols.update(raw_symbol.split(' ', 1)[0] for raw_symbol in
+                try:
+                    hgnc_symbols.update(raw_symbol.split(' ', 1)[0] for raw_symbol in
                                     raw_symbols.split('|'))
+                except ValueError:
+                    flash("Provided gene info could not be parsed! "
+                          "Please allow autocompletion to finish.", 'warning')
             LOG.debug("HGNC symbols {}".format(hgnc_symbols))
         store.update_dynamic_gene_list(case_obj, hgnc_symbols=hgnc_symbols)
 
     elif action == 'GENERATE':
         if len(hpo_ids) == 0:
             hpo_ids = [term['phenotype_id'] for term in case_obj.get('phenotype_terms', [])]
         results = store.generate_hpo_gene_list(*hpo_ids)
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/dashboard/controllers.py` & `scout-browser-4.9.0/scout/server/blueprints/dashboard/controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/dashboard/static/charts.js` & `scout-browser-4.9.0/scout/server/blueprints/dashboard/static/charts.js`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/dashboard/templates/dashboard/dashboard_general.html` & `scout-browser-4.9.0/scout/server/blueprints/dashboard/templates/dashboard/dashboard_general.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/dashboard/views.py` & `scout-browser-4.9.0/scout/server/blueprints/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/genes/controllers.py` & `scout-browser-4.9.0/scout/server/blueprints/genes/controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/genes/templates/genes/gene.html` & `scout-browser-4.9.0/scout/server/blueprints/genes/templates/genes/gene.html`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,20 @@
     <li class="list-group-item">
       String
       <span class="float-right">
         <a target="_blank" href={{ gene.string_link }} target="_blank"> {{ gene.ensembl_id }}</a>
       </span>
     </li>
     <li class="list-group-item">
+      GENEMANIA
+      <span class="float-right">
+        <a target="_blank" href={{ gene.genemania_link }} target="_blank"> {{ gene.hgnc_symbol }}</a>
+      </span>
+    </li>
+    <li class="list-group-item">
       Vega Database
       <span class="float-right">
         <a target="_blank" href={{ gene.vega_link }} target="_blank"> {{ gene.vega_id }}</a>
       </span>
     </li>
     <li class="list-group-item">
       UCSC gene browser ({{ gene.build }})
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/genes/templates/genes/genes.html` & `scout-browser-4.9.0/scout/server/blueprints/genes/templates/genes/genes.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/genes/templates/genes/layout.html` & `scout-browser-4.9.0/scout/server/blueprints/genes/templates/genes/layout.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/genes/views.py` & `scout-browser-4.9.0/scout/server/blueprints/genes/views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/institutes/templates/overview/institutes.html` & `scout-browser-4.9.0/scout/server/blueprints/institutes/templates/overview/institutes.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/institutes/views.py` & `scout-browser-4.9.0/scout/server/blueprints/institutes/views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/controllers.py` & `scout-browser-4.9.0/scout/server/blueprints/login/controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/models.py` & `scout-browser-4.9.0/scout/server/blueprints/login/models.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/static/commander.svg` & `scout-browser-4.9.0/scout/server/blueprints/login/static/commander.svg`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/static/commissioner.svg` & `scout-browser-4.9.0/scout/server/blueprints/login/static/commissioner.svg`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/static/constable.svg` & `scout-browser-4.9.0/scout/server/blueprints/login/static/constable.svg`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/static/inspector.svg` & `scout-browser-4.9.0/scout/server/blueprints/login/static/inspector.svg`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/static/sergeant.svg` & `scout-browser-4.9.0/scout/server/blueprints/login/static/sergeant.svg`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/static/superintendent.svg` & `scout-browser-4.9.0/scout/server/blueprints/login/static/superintendent.svg`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/templates/login/users.html` & `scout-browser-4.9.0/scout/server/blueprints/login/templates/login/users.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/login/views.py` & `scout-browser-4.9.0/scout/server/blueprints/login/views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/panels/controllers.py` & `scout-browser-4.9.0/scout/server/blueprints/panels/controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/panels/forms.py` & `scout-browser-4.9.0/scout/server/blueprints/panels/forms.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/panels/templates/panels/gene-edit.html` & `scout-browser-4.9.0/scout/server/blueprints/panels/templates/panels/gene-edit.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/panels/templates/panels/panel.html` & `scout-browser-4.9.0/scout/server/blueprints/panels/templates/panels/panel.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/panels/templates/panels/panel_pdf_simple.html` & `scout-browser-4.9.0/scout/server/blueprints/panels/templates/panels/panel_pdf_simple.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/panels/templates/panels/panels.html` & `scout-browser-4.9.0/scout/server/blueprints/panels/templates/panels/panels.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/panels/views.py` & `scout-browser-4.9.0/scout/server/blueprints/panels/views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/phenotypes/templates/phenotypes/hpo_terms.html` & `scout-browser-4.9.0/scout/server/blueprints/phenotypes/templates/phenotypes/hpo_terms.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/phenotypes/views.py` & `scout-browser-4.9.0/scout/server/blueprints/phenotypes/views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/public/static/logo-karolinska.png` & `scout-browser-4.9.0/scout/server/blueprints/public/static/logo-karolinska.png`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/public/static/logo-scilifelab.png` & `scout-browser-4.9.0/scout/server/blueprints/public/static/logo-scilifelab.png`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/public/static/scout-logo.png` & `scout-browser-4.9.0/scout/server/blueprints/public/static/scout-logo.png`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/public/static/swedac.png` & `scout-browser-4.9.0/scout/server/blueprints/public/static/swedac.png`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/public/templates/public/index.html` & `scout-browser-4.9.0/scout/server/blueprints/public/templates/public/index.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/public/views.py` & `scout-browser-4.9.0/scout/server/blueprints/public/views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variant/controllers.py` & `scout-browser-4.9.0/scout/server/blueprints/variant/controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/acmg.html` & `scout-browser-4.9.0/scout/server/blueprints/variant/templates/variant/acmg.html`

 * *Files 18% similar despite different names*

```diff
@@ -31,35 +31,44 @@
         </div>
       </div>
 
       <div class="d-flex justify-content-between mt-3">
         {% for category, criteria_group in CRITERIA.items() %}
           <div class="flex-1 {{ 'mr-3' if not loop.last }}">
             <h4>Evidence of {{ category }}</h4>
-
             {% for evidence, criteria in criteria_group.items() %}
               <ul class="list-group mt-3">
                 <li class="list-group-item">{{ evidence }}</li>
                 {% for criterion_code, criterion in criteria.items() %}
+
+                  {% if evaluation and evaluation.criteria.get(criterion_code).comment %}
+                    {% set comment = evaluation.criteria.get(criterion_code).comment %}
+                  {% endif %}
+                  {% if evaluation and evaluation.criteria.get(criterion_code).links %}
+                    {% set link = evaluation.criteria.get(criterion_code).links[0] %}
+                  {% endif %}
+
                   <div class="list-group-item">
                     <div class="d-flex justify-content-between">
                       <div data-toggle="tooltip" data-placement="top" title="{{ criterion.description }}">
                         <span class="badge badge-info mr-1">{{ criterion_code }}</span>
                         {{ criterion.short }}
                       </div>
                       <div>
                         <input type="checkbox" class="ios8-switch" id="checkbox-{{ criterion_code }}" name="criteria" value="{{ criterion_code }}" {{ 'checked' if evaluation and criterion_code in evaluation.criteria }} {{ 'disabled' if evaluation }}>
                         <label for="checkbox-{{ criterion_code }}"></label>
                       </div>
                     </div>
-                    <div id="comment-{{ criterion_code }}" class="collapse {{ 'in' if evaluation and evaluation.criteria.get(criterion_code).comment }} mt-2">
+                    <div id="comment-{{ criterion_code }}" class="{{ 'collapse' if not (comment or link) }} mt-2">
                       <div class="form-group">
-                        <textarea class="form-control" name="comment-{{ criterion_code }}" rows="3" placeholder="Comment (optional)">{{ evaluation.criteria.get(criterion_code).comment if evaluation and evaluation.criteria.get(criterion_code).comment }}</textarea>
+                        <textarea {{ 'disabled' if comment }} class="form-control"
+                          name="comment-{{ criterion_code }}" rows="3" placeholder="Comment (optional)">{{ comment }}</textarea>
                       </div>
-                      <input type="url" class="form-control" name="link-{{ criterion_code }}" placeholder="Supporting link (optional)" value="{{ evaluation.criteria.get(criterion_code).link if evaluation and evaluation.criteria.get(criterion_code).link }}">
+                      <input type="url" {{ 'disabled' if link or comment }} class="form-control" name="link-{{ criterion_code }}"
+                        placeholder="{{ link or 'Supporting link (optional)' }}" value="">
                     </div>
                   </div>
                 {% endfor %}
                 </li>
               </ul>
             {% endfor %}
           </div>
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/clinvar.html` & `scout-browser-4.9.0/scout/server/blueprints/variant/templates/variant/clinvar.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/sv-variant.html` & `scout-browser-4.9.0/scout/server/blueprints/variant/templates/variant/sv-variant.html`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             <div class="list-group mt-3">
               <div>
                 <form action="{{ url_for('variant.variant_update', institute_id=institute._id, case_name=case.display_name, variant_id=variant._id) }}" method="POST">
                   <label class="ml-3">Variant tag</label>
                   <div class="row">
                     <div class="col-8">
                       <select name="manual_rank" class="form-control ml-3">
-                        <option>Select a tag</option>
+                        <option value="-1">Select a tag...</option>
                         {% for rank, data in manual_rank_options.items() %}
                           <option {% if rank == variant.manual_rank %} selected {% endif %} value="{{ rank }}">
                             {{ data.label }}
                           </option>
                         {% endfor %}
                       </select>
                     </div>
@@ -226,15 +226,15 @@
     {% if has_pedigree %}
       <div class="col-xs-12 col-md-3">{{ pedigree_panel(case) }}</div>
     {% endif %}
   </div>
 
   <div class="row">
     <div class="col-md-12">
-      {{ overlapping(overlapping_snvs, variant.rank_score) }}
+      {{ overlapping(overlapping_vars, variant.rank_score) }}
     </div>
   </div>
 
   <div class="row">
     <div class="col-12">
       <div class="card">
         <nav>
```

#### html2text {}

```diff
@@ -74,15 +74,15 @@
 {{ gt_calls(variant.samples) }}
 {{ comments_panel(institute, case, current_user, variant.comments,
 variant_id=variant._id) }}
 {% set has_pedigree = case.madeline_info and case.individuals|length > 1 %} {%
 if has_pedigree %}
 {{ pedigree_panel(case) }}
 {% endif %}
-{{ overlapping(overlapping_snvs, variant.rank_score) }}
+{{ overlapping(overlapping_vars, variant.rank_score) }}
 Genes Transcripts
 {{ genes_panel(variant) }}
 {{ transcripts_panel() }}
 {{ ext_links(variant) }}
 {% if config['MAIL_USERNAME'] %} {# Email setting must be setup #} {
 { verify_modal() }} {% endif %} {% if config['MAIL_USERNAME'] %} {# Email
 setting must be setup #} {{ modal_cancel_verify() }} {% endif %} {
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variant/templates/variant/variant.html` & `scout-browser-4.9.0/scout/server/blueprints/variant/templates/variant/variant.html`

 * *Files 0% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
             <th>Rank score</th>
             <th>Length</th>
             <th>Region</th>
             <th>Function</th>
           </tr>
         </thead>
         <tbody>
-          {% for sv_variant in overlapping_svs %}
+          {% for sv_variant in overlapping_vars %}
             <tr>
               <td>
                 <a href="{{url_for('variant.sv_variant', institute_id=institute._id,
                                    case_name=case.display_name, variant_id=sv_variant._id)}}">
                   {{ sv_variant.display_name|truncate(20, True) }}
                 </a>
               </td>
@@ -1240,14 +1240,15 @@
         External links: {{ gene.common.hgnc_symbol if gene.common else gene.hgnc_id }}
       </div>
       <div class="panel-body">
         <div class="btn-group">
           <a href="{{ gene.ensembl_link }}" class="btn btn-outline-secondary" target="_blank">Ensembl</a>
           <a href="{{ gene.hpa_link }}" class="btn btn-outline-secondary" target="_blank">HPA</a>
           <a href="{{ gene.string_link }}" class="btn btn-outline-secondary" target="_blank">STRING</a>
+          <a href="{{ gene.genemania_link }}" class="btn btn-outline-secondary" target="_blank">GENEMANIA</a>
           <a href="{{ variant.ucsc_link }}" class="btn btn-outline-secondary" target="_blank">UCSC</a>
           {% if gene.entrez_link %}
             <a href="{{ gene.entrez_link }}" class="btn btn-outline-secondary" target="_blank">Entrez</a>
           {% endif %}
           <a href="http://tools.genes.toronto.edu/" class="btn btn-outline-secondary" target="_blank">SPANR</a>
           <a href="{{ gene.reactome_link }}" class="btn btn-outline-secondary" target="_blank">Reactome</a>
           <a href="{{ gene.expression_atlas_link }}" class="btn btn-outline-secondary" target="_blank">Expr. Atlas</a>
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variant/utils.py` & `scout-browser-4.9.0/scout/server/blueprints/variant/utils.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variant/verification_controllers.py` & `scout-browser-4.9.0/scout/server/blueprints/variant/verification_controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variant/views.py` & `scout-browser-4.9.0/scout/server/blueprints/variant/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,21 @@
     institute_obj, case_obj = institute_and_case(store, institute_id, case_name)
     variant_obj = store.variant(variant_id)
     user_obj = store.user(current_user.email)
     link = request.referrer
 
     manual_rank = request.form.get('manual_rank')
     if manual_rank:
-        new_manual_rank = int(manual_rank) if manual_rank != '-1' else None
+        try:
+            new_manual_rank = int(manual_rank) if manual_rank != '-1' else None
+        except:
+            LOG.warning("Attempt to update manual rank with invalid value {}".format(manual_rank))
+            manual_rank = '-1'
+            new_manual_rank = -1
+
         store.update_manual_rank(institute_obj, case_obj, user_obj, link, variant_obj,
                                  new_manual_rank)
         if new_manual_rank:
             flash("updated variant tag: {}".format(new_manual_rank), 'info')
         else:
             flash("reset variant tag: {}".format(variant_obj.get('manual_rank', 'NA')), 'info')
     elif request.form.get('acmg_classification'):
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variants/controllers.py` & `scout-browser-4.9.0/scout/server/blueprints/variants/controllers.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,18 @@
         variant_obj['overlapping'] = overlapping_svs or None
 
         # Get all previous ACMG evalautions of the variant
         evaluations = []
         for evaluation_obj in store.get_evaluations(variant_obj):
             classification = evaluation_obj['classification']
             # Only show pathogenic/likely pathogenic from other cases on variants page
-            if evaluation_obj['case_id'] != case_obj['_id']:
-                if not classification in ['pathogenic', 'likely_pathogenic']:
-                    continue
+            if evaluation_obj['case_id'] == case_obj['_id']:
+                continue
+            if not classification in ['pathogenic', 'likely_pathogenic']:
+                continue
             # Convert the classification int to readable string
             evaluation_obj['classification'] = ACMG_COMPLETE_MAP.get(classification)
             evaluations.append(evaluation_obj)
         variant_obj['evaluations'] = evaluations
 
         variants.append(parse_variant(store, institute_obj, case_obj, variant_obj,
                         update=True, genome_build=genome_build))
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variants/forms.py` & `scout-browser-4.9.0/scout/server/blueprints/variants/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,14 +46,15 @@
                 self.data = decimal.Decimal(raw_decimal)
             except (decimal.InvalidOperation, ValueError):
                 self.data = None
                 raise ValueError(self.gettext('Not a valid decimal value'))
 
 class VariantFiltersForm(FlaskForm):
     variant_type = HiddenField(default='clinical')
+    
     gene_panels = SelectMultipleField(choices=[])
     hgnc_symbols = TagListField('HGNC Symbols/Ids (case sensitive)')
 
     region_annotations = SelectMultipleField(choices=REGION_ANNOTATIONS)
     functional_annotations = SelectMultipleField(choices=FUNC_ANNOTATIONS)
     genetic_models = SelectMultipleField(choices=GENETIC_MODELS)
 
@@ -96,20 +97,24 @@
     """Placeholder filters form for CancerFiltersForm (**unused**)"""
     variant_type = HiddenField(default='clinical')
 
     chrom = TextField('Chromosome')
     gene_panels = SelectMultipleField(choices=[])
     repids = TagListField()
 
-class SvFiltersForm(FiltersForm):
+class SvFiltersForm(VariantFiltersForm):
     """Extends FiltersForm for structural variants"""
-    variant_type = HiddenField(default='clinical')
     size = TextField('Length')
     size_shorter = BooleanField('Length shorter than')
     svtype = SelectMultipleField('SVType', choices=SV_TYPE_CHOICES)
+
     decipher = BooleanField('Decipher')
+    clingen_ngi = IntegerField('ClinGen NGI obs')
+    swegen = IntegerField('SweGen obs')
+
     chrom = TextField('Chromosome', [validators.Optional()])
     start = IntegerField('Start position', [validators.Optional(), IntegerField])
     end = IntegerField('End position', [validators.Optional(), IntegerField])
-    clingen_ngi = IntegerField('ClinGen NGI obs')
-    swegen = IntegerField('SweGen obs')
+
+    filter_variants = SubmitField(label='Filter variants')
+    clinical_filter = SubmitField(label='Clinical filter')
     export = SubmitField(label='Filter and export')
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/cancer-variants.html` & `scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/cancer-variants.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/components.html` & `scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/components.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/str-variants.html` & `scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/str-variants.html`

 * *Files 2% similar despite different names*

```diff
@@ -133,27 +133,27 @@
 
 {% macro footer() %}
   <div class="container-fluid">
     <div class="form-group text-center">
       {% if more_variants %}
         <div class="row">
             <div class="col-6">
-              <a class="btn btn-outline-secondary mx-auto d-block" href="{{ url_for('variants.str_variants', institute_id=institute._id, case_name=case.display_name, page=1, **form.data) }}">	
+              <a class="btn btn-outline-secondary mx-auto d-block" href="{{ url_for('variants.str_variants', institute_id=institute._id, case_name=case.display_name, page=1, **form.data) }}">
                   First page
               </a>
               </div>
               <div class="col-6">
                 <a class="btn btn-outline-secondary mx-auto d-block" href="{{ url_for('variants.str_variants', institute_id=institute._id, case_name=case.display_name, page=(page + 1), **form.data) }}">
                   Next page
                 </a>
               </div>
         </div>
       {% else %}
         <i class="text-muted">No more variants to display</i>
-        <a class="btn btn-outline-secondary mx-auto d-block" href="{{ url_for('variants.str_variants', institute_id=institute._id, case_name=case.display_name, page=1, **form.data) }}">	
+        <a class="btn btn-outline-secondary mx-auto d-block" href="{{ url_for('variants.str_variants', institute_id=institute._id, case_name=case.display_name, page=1, **form.data) }}">
       First page
         </a>
       {% endif %}
     </div>
   </div>
 {% endmacro %}
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/sv-variants.html` & `scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/sv-variants.html`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   </li>
   <li class="nav-item">
     <a class="nav-link text-nowrap" href="{{ url_for('cases.case', institute_id=institute._id, case_name=case.display_name) }}">
       {{ case.display_name }}
     </a>
   </li>
   <li class="nav-item active">
-    <span class="navbar-text">{{ variant_type|capitalize }}  Structural variants</span>
+    <span class="navbar-text">{{ form.variant_type.data|capitalize }}  Structural variants</span>
   </li>
 {% endblock %}
 
 {% block top_nav_right %}
   <li class="nav-item text-nowrap"><p class="navbar-text">Panels: {{ (form.gene_panels.data or ['All'])|join(',') }}</p></li>
   {{ super() }}
 {% endblock %}
@@ -81,22 +81,22 @@
   <div class="container-fluid">
     {{ pagination() }}
   </div>
 </form>
 {% endblock %}
 
 {% macro cell_rank(variant) %}
-  <a class="variants-row-item flex-small layout"
+  <a
      href="{{ url_for('variant.sv_variant', institute_id=institute._id,
                       case_name=case.display_name, variant_id=variant._id) }}">
     {{ variant.variant_rank }}
   </a>
   {% set comment_count = variant.comments.count() %}
   {% if variant.manual_rank %}
-    <span class="badge float-right" title="Manual rank">{{ variant.manual_rank }}</span>
+    <span class="badge badge-primary" data-toggle="tooltip" data-placement="right" title="Manual rank: {{ manual_rank_options[variant.manual_rank].description }}">{{  manual_rank_options[variant.manual_rank]['label'] }}</span>
   {% endif %}
 
   {% if comment_count > 0 %}
     {% set comments_content = comments_table(institute, case, variant.comments, variant._id) %}
     <a href="#"
       class="badge badge-secondary"
       style="color:white;"
@@ -119,23 +119,23 @@
 
 {% macro variant_row(variant) %}
   {% if variant.dismiss_variant %}
   <tr class="dismiss">
   {% else %}
   <tr>
   {% endif %}
-    <td>
+    <td class="text-left">
       {{ cell_rank(variant) }}
     </td>
-    <td>{{ variant.rank_score|int }}</td>
+    <td class="text-right">{{ variant.rank_score|int }}</td>
     <td>{{ variant.sub_category|upper }}</td>
     <td>{{ variant.chromosome if variant.chromosome == variant.end_chrom else variant.chromosome+'-'+variant.end_chrom }}</td>
     <td>{{ variant.position }}</td>
     <td>{{ 'inf' if variant.end == 100000000000 else variant.end }}</td>
-    <td>{{ variant.length }}</td>
+    <td class="text-right">{{ variant.length }}</td>
     <td>
       {% if 'region_annotations' in variant %}
         {% for annotation in variant.region_annotations[:3] %}
           <div>{{ annotation }}</div>
         {% endfor %}
       {% endif %}
     </td>
@@ -173,15 +173,15 @@
     {% if more_variants %}
     <div class="d-flex justify-content-around">
         <div>
             <button name="page" type="submit" class="btn btn-outline-secondary mx-auto d-block" value=1>First page</button>
         </div>
        <div>
           <button name="page" type="submit" class="btn btn-outline-secondary mx-auto d-block" value={{ page + 1 }}>Next page</button>
-         </div>
+       </div>
     </div>
     {% else %}
       <i class="text-muted">No more variants to display</i>
       <button name="page" type="submit" class="btn btn-outline-secondary mx-auto d-block" value=1>First page</button>
     {% endif %}
   </div>
 {% endmacro %}
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/utils.html` & `scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/utils.html`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
         </form>
     </div>
   </div>
 </div>
 {% endmacro %}
 
 {% macro snv_filters(form, institute, case)%}
+<input type="hidden" name="variant_type" value="{{ form.variant_type.data }}">
 <div class="form-group">
   <div class="row">
     <div class="col-4">
       {{ form.gene_panels.label}}
       {{ form.gene_panels(class="selectpicker") }}
     </div>
     <div class="col-2">
@@ -246,15 +247,15 @@
       </div>
   </div>
 </div>
 <div class="form-group">
   <div class="row justify-content-between" style="margin-top:20px;">
     <div class="col-6 text-left">
       <a href="{{ url_for('variants.variants', institute_id=institute._id, case_name=case.display_name,
-        variant_type='clinical', gene_panels=case.panels|selectattr('is_default')|map(attribute='panel_name')|list) }}"
+        variant_type=form.variant_type.data, gene_panels=case.panels|selectattr('is_default')|map(attribute='panel_name')|list) }}"
         class="btn btn-secondary" style="color: #ffffff !important;">
         Reset&nbsp;filters
       </a>
     </div>
     <div class="col-6">
       {{ stash_filter_buttons(form, institute, case) }}
     </div>
@@ -354,15 +355,15 @@
     <div class="col-4">
       {{ form.export(class="btn btn-warning form-control") }}
     </div>
   </div>
   <div class="row justify-content-between" style="margin-top:20px;">
     <div class="col-1">
       <a href="{{ url_for('variants.sv_variants', institute_id=institute._id,
-        case_name=case.display_name, variant_type='clinical',
+        case_name=case.display_name, variant_type=form.variant_type.data,
         gene_panels=case.panels|selectattr('is_default')|map(attribute='panel_name')|list) }}"
         class="btn btn-secondary" style="color: #ffffff !important;">
         Reset&nbsp;filters
       </a>
     </div>
     <div class="col-6">
       {{ stash_filter_buttons(form, institute, case) }}
@@ -443,15 +444,15 @@
     <div class="form-group">
       <div class="row">
         <div class="col-3">
           <button class="btn btn-primary form-control">Filter variants</button>
         </div>
         <div class="col-1 align-self-start">
           <a href="{{ url_for('variants.cancer_variants', institute_id=institute._id,
-            case_name=case.display_name, variant_type='clinical',
+            case_name=case.display_name, variant_type=form.variant_type.data,
             gene_panels=case.panels|selectattr('is_default')|map(attribute='panel_name')|list) }}"
             class="btn btn-secondary" style="color: #ffffff !important;">
             Reset&nbsp;filters
           </a>
         </div>
         <div class="col-2">
         </div>
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variants/templates/variants/variants.html` & `scout-browser-4.9.0/scout/server/blueprints/variants/templates/variants/variants.html`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,17 @@
 
   {% if variant.acmg_classification %}
     <span class="badge badge-primary" data-toggle="tooltip" data-placement="right" title="ACMG: {{ variant.acmg_classification.label }}">
       {{ variant.acmg_classification.short }}
     </span>
   {% endif %}
   {% if variant.manual_rank %}
-    <span class="badge badge-primary" data-toggle="tooltip" title="Manual rank">{{ variant.manual_rank }}</span>
+    <span class="badge badge-primary" data-toggle="tooltip" data-placement="right"
+        title="Manual rank: {{ manual_rank_options[variant.manual_rank].description }}">
+        {{ manual_rank_options[variant.manual_rank].label }}</span>
   {% endif %}
   {% if variant.evaluations %}
     {% for evaluation in (variant.evaluations or []) %}
       <span class="badge badge-secondary" style="margin-left:1px" data-toggle="tooltip" data-placement="right"
       title="Previously classified as {{ evaluation.classification.label }}">
       {{ evaluation.classification.short }}
       </span>
@@ -196,18 +198,18 @@
 
 {% macro footer() %}
   <div class="container-fluid">
       {% if more_variants %}
         <div class="d-flex justify-content-around">
 	         <div>
             <button name="page" type="submit" class="btn btn-outline-secondary mx-auto d-block" value=1>First page</button>
-        </div>
-        <div>
+          </div>
+          <div>
             <button name="page" type="submit" class="btn btn-outline-secondary mx-auto d-block" value={{ page + 1 }}>Next page</button>
-           </div>
+          </div>
 	     </div>
       {% else %}
         <i class="text-muted">No more variants to display</i>
         <button name="page" type="submit" class="btn btn-outline-secondary mx-auto d-block" value=1>First page</button>
       {% endif %}
   </div>
 {% endmacro %}
```

#### html2text {}

```diff
@@ -21,17 +21,18 @@
 (variant) }}                     }}                 (variant) (variant) }}   (variant) {{ annotation }}           {{ annotation }}               (variant)   (variant) }}
 }}                                                  }}                       }}        {% endfor %}               {% endfor %}                   }}
 No matching variants
  {{ footer() }}
 {% endblock %} {% macro cell_rank(variant) %} {{_variant.variant_rank_}}  {%
 set comment_count = variant.comments.count() %} {% if
 variant.acmg_classification %}  {{ variant.acmg_classification.short }}  {%
-endif %} {% if variant.manual_rank %} {{ variant.manual_rank }} {% endif %} {%
-if variant.evaluations %} {% for evaluation in (variant.evaluations or []) %}
-{{ evaluation.classification.short }}  {% endfor %} {% endif %} {% if
+endif %} {% if variant.manual_rank %}  {{ manual_rank_options
+[variant.manual_rank].label }} {% endif %} {% if variant.evaluations %} {% for
+evaluation in (variant.evaluations or []) %}  {
+{ evaluation.classification.short }}  {% endfor %} {% endif %} {% if
 comment_count > 0 %} {% set comments_content = comments_table(institute, case,
 variant.comments, variant._id) %}
 {{_comment_count_}}__{%_if_'GLOBAL'_in_comments_content_%}__{%_endif_%}
  {% endif %} {% if variant._id in case.suspects %}  {% endif %} {% endmacro %}
 {% macro cell_cadd(variant) %}
 {{ variant.cadd_score }}
 {% endmacro %} {% macro cell_models(variant) %} {% for model in
```

### Comparing `scout-browser-4.8.3/scout/server/blueprints/variants/views.py` & `scout-browser-4.9.0/scout/server/blueprints/variants/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pathlib
 
 from flask import (Blueprint, request, redirect, abort, flash, current_app, url_for, Response,
                    send_file)
 from werkzeug.datastructures import (Headers, MultiDict)
 from flask_login import current_user
 
-from scout.constants import SEVERE_SO_TERMS
+from scout.constants import SEVERE_SO_TERMS, MANUAL_RANK_OPTIONS
 from scout.server.extensions import store
 from scout.server.utils import (templated, institute_and_case)
 from . import controllers
 from .forms import FiltersForm, SvFiltersForm, StrFiltersForm, CancerFiltersForm
 
 LOG = logging.getLogger(__name__)
 variants_bp = Blueprint('variants', __name__, static_folder='static', template_folder='templates')
@@ -38,14 +38,16 @@
 
     if(request.method == "POST"):
         # If special filter buttons were selected:
         form = controllers.populate_filters_form(store, institute_obj, case_obj,
                                                  user_obj, category, request.form)
     else:
         form = FiltersForm(request.args)
+        # set form variant data type the first time around
+        form.variant_type.data = variant_type
 
     # populate filters dropdown
     available_filters = store.filters(institute_id, category)
     form.filters.choices = [(filter.get('_id'), filter.get('display_name'))
         for filter in available_filters]
 
     # populate available panel choices
@@ -146,16 +148,15 @@
         headers.add('Content-Disposition','attachment', filename=str(case_obj['display_name'])+'-filtered_variants.csv')
 
         # return a csv with the exported variants
         return Response(generate(",".join(document_header), export_lines), mimetype='text/csv',
                         headers=headers)
 
     data = controllers.variants(store, institute_obj, case_obj, variants_query, page)
-
-    return dict(institute=institute_obj, case=case_obj, form=form,
+    return dict(institute=institute_obj, case=case_obj, form=form, manual_rank_options=MANUAL_RANK_OPTIONS,
                     severe_so_terms=SEVERE_SO_TERMS, page=page, **data)
 
 @variants_bp.route('/<institute_id>/<case_name>/str/variants')
 @templated('variants/str-variants.html')
 def str_variants(institute_id, case_name):
     """Display a list of STR variants."""
     page = int(request.args.get('page', 1))
@@ -192,22 +193,23 @@
 
     user_obj = store.user(current_user.email)
     if(request.method == "POST"):
         form = controllers.populate_filters_form(store, institute_obj, case_obj,
                                                  user_obj, category, request.form)
     else:
         form = SvFiltersForm(request.args)
+        # set form variant data type the first time around
+        form.variant_type.data = variant_type
+
 
     # populate filters dropdown
     available_filters = store.filters(institute_id, category)
     form.filters.choices = [(filter.get('_id'), filter.get('display_name'))
         for filter in available_filters]
 
-    # redundant?
-    form.variant_type.data = variant_type
 
     # update status of case if visited for the first time
     if case_obj['status'] == 'inactive' and not current_user.is_admin:
         flash('You just activated this case!', 'info')
         user_obj = store.user(current_user.email)
         case_link = url_for('cases.case', institute_id=institute_obj['_id'],
                             case_name=case_obj['display_name'])
@@ -283,15 +285,15 @@
         headers.add('Content-Disposition','attachment', filename=str(case_obj['display_name'])+'-filtered_sv-variants.csv')
         return Response(generate(",".join(document_header), export_lines), mimetype='text/csv', headers=headers) # return a csv with the exported variants
 
     data = controllers.sv_variants(store, institute_obj, case_obj,
                                        variants_query, page)
 
     return dict(institute=institute_obj, case=case_obj, variant_type=variant_type,
-                form=form, severe_so_terms=SEVERE_SO_TERMS, page=page, **data)
+                form=form, severe_so_terms=SEVERE_SO_TERMS, manual_rank_options=MANUAL_RANK_OPTIONS, page=page, **data)
 
 @variants_bp.route('/<institute_id>/<case_name>/cancer/variants', methods=['GET','POST'])
 @templated('variants/cancer-variants.html')
 def cancer_variants(institute_id, case_name):
     """Show cancer variants overview."""
     category = 'cancer'
```

### Comparing `scout-browser-4.8.3/scout/server/config.py` & `scout-browser-4.9.0/scout/server/config.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/extensions.py` & `scout-browser-4.9.0/scout/server/extensions.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/links.py` & `scout-browser-4.9.0/scout/server/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,21 @@
     gene_obj['omim_link'] = omim(gene_obj.get('omim_id'))
     # Add links that use hgnc_symbol
     gene_obj['ppaint_link'] = ppaint(hgnc_symbol)
     # Add links that use vega_id
     gene_obj['vega_link'] = vega(gene_obj.get('vega_id'))
     # Add links that use ucsc link
     gene_obj['ucsc_link'] = ucsc(gene_obj.get('ucsc_id'))
+    gene_obj['genemania_link'] = genemania(hgnc_symbol)
+
+def genemania(hgnc_symbol):
+    link = "https://genemania.org/search/homo-sapiens/{}/"
+    if not hgnc_symbol:
+        return None
+    return link.format(hgnc_symbol)
 
 def genenames(hgnc_id):
     link = "https://www.genenames.org/cgi-bin/gene_symbol_report?hgnc_id=HGNC:{}"
     if not hgnc_id:
         return None
     return link.format(hgnc_id)
```

### Comparing `scout-browser-4.8.3/scout/server/static/bs4_styles.css` & `scout-browser-4.9.0/scout/server/static/bs4_styles.css`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,18 @@
 }
 
 a:visited {
 	/* purple */
 	color: #551A8B;
 }
 
+.odd {
+   background-color: #f2f2f2;
+}
+
 /* Introduce small space in between list elements */
 body {
 	background-color: var(--bg-color);
 	font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
 }
 
 .bg-success {
```

### Comparing `scout-browser-4.8.3/scout/server/static/favicon.ico` & `scout-browser-4.9.0/scout/server/blueprints/public/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/templates/bootstrap4.html` & `scout-browser-4.9.0/scout/server/templates/bootstrap4.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/templates/layout_bs4.html` & `scout-browser-4.9.0/scout/server/templates/layout_bs4.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/templates/report_base.html` & `scout-browser-4.9.0/scout/server/templates/report_base.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/templates/utils.html` & `scout-browser-4.9.0/scout/server/templates/utils.html`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/translations/sv/LC_MESSAGES/messages.mo` & `scout-browser-4.9.0/scout/server/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/translations/sv/LC_MESSAGES/messages.po` & `scout-browser-4.9.0/scout/server/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/userpanel.py` & `scout-browser-4.9.0/scout/server/userpanel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/server/utils.py` & `scout-browser-4.9.0/scout/server/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,21 +36,22 @@
 def institute_and_case(store, institute_id, case_name=None):
     """Fetch insitiute and case objects."""
     institute_obj = store.institute(institute_id)
     if institute_obj is None:
         flash("Can't find institute: {}".format(institute_id), 'warning')
         return abort(404)
 
+
     if case_name:
-        if case_name:
-            case_obj = store.case(institute_id=institute_id, display_name=case_name)
-            if case_obj is None:
-                return abort(404)
+        case_obj = store.case(institute_id=institute_id, display_name=case_name)
+        if case_obj is None:
+            return abort(404)
 
     # validate that user has access to the institute
+
     if not current_user.is_admin:
         if institute_id not in current_user.institutes:
             if not case_name or not any(inst_id in case_obj['collaborators'] for inst_id in
                                         current_user.institutes):
                 # you don't have access!!
                 flash("You don't have acccess to: {}".format(institute_id),'danger')
                 return abort(403)
@@ -91,44 +92,44 @@
         for gene in variant_obj.get('genes', []):
             chrom = gene['common']['chromosome']
             starts.append(gene['common']['start'])
             ends.append(gene['common']['end'])
 
         if (crom and starts and ends):
             vcf_path = store.get_region_vcf(
-                case_obj, 
-                chrom=chrom, 
-                start=min(starts), 
+                case_obj,
+                chrom=chrom,
+                start=min(starts),
                 end=max(ends)
             )
 
             # Create a reduced VCF with variants in the region
             case_obj['region_vcf_file'] = vcf_path
     except (SyntaxError, Exception):
         LOG.warning("skip VCF region for alignment view")
 
 def case_append_bam(case_obj):
     """Deconvolute information about files to case_obj.
 
-    This function prepares the bam files in a certain way so that they are easily accessed in the 
+    This function prepares the bam files in a certain way so that they are easily accessed in the
     templates.
 
     Loops over the the individuals and gather bam files, indexes and sample display names in lists
 
     Args:
         case_obj(scout.models.Case)
     """
     case_obj['bam_files'] = []
     case_obj['mt_bams'] = []
     case_obj['bai_files'] = []
     case_obj['mt_bais'] = []
     case_obj['sample_names'] = []
 
     bam_files = [
-        ('bam_file','bam_files', 'bai_files'), 
+        ('bam_file','bam_files', 'bai_files'),
         ('mt_bam', 'mt_bams', 'mt_bais')
     ]
 
     for individual in case_obj['individuals']:
         case_obj['sample_names'].append(individual.get('display_name'))
         for bam in bam_files:
             bam_path = individual.get(bam[0])
@@ -136,20 +137,20 @@
                 LOG.debug("%s: no bam file found", individual['individual_id'])
                 continue
             case_obj[bam[1]].append(bam_path) # either bam_files or mt_bams
             case_obj[bam[2]].append(find_bai_file(bam_path)) # either bai_files or mt_bais
 
 def find_bai_file(bam_file):
     """Find out BAI file by extension given the BAM file.
-    
+
     Index files wither ends with filename.bam.bai or filename.bai
-    
+
     Args:
         bam_file(str): The path to a bam file
-    
+
     Returns:
         bai_file(str): Path to index file
     """
     bai_file = bam_file.replace('.bam', '.bai')
     if not os.path.exists(bai_file):
         # try the other convention
         bai_file = "{}.bai".format(bam_file)
```

### Comparing `scout-browser-4.8.3/scout/update/panel.py` & `scout-browser-4.9.0/scout/update/panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/acmg.py` & `scout-browser-4.9.0/scout/utils/acmg.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/algorithms.py` & `scout-browser-4.9.0/scout/utils/algorithms.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/convert.py` & `scout-browser-4.9.0/scout/utils/convert.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/coordinates.py` & `scout-browser-4.9.0/scout/utils/coordinates.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/date.py` & `scout-browser-4.9.0/scout/utils/date.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/ensembl_rest_clients.py` & `scout-browser-4.9.0/scout/utils/ensembl_rest_clients.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/gene.py` & `scout-browser-4.9.0/scout/utils/gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/link.py` & `scout-browser-4.9.0/scout/utils/link.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/matchmaker.py` & `scout-browser-4.9.0/scout/utils/matchmaker.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/md5.py` & `scout-browser-4.9.0/scout/utils/md5.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout/utils/requests.py` & `scout-browser-4.9.0/scout/utils/requests.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/scout_browser.egg-info/PKG-INFO` & `scout-browser-4.9.0/scout_browser.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scout-browser
-Version: 4.8.3
+Version: 4.9.0
 Summary: Clinical DNA variant visualizer and browser.
 Home-page: https://github.com/Clinical-Genomics/scout
 Author: Måns Magnusson
 Author-email: mans.magnusson@scilifelab.se
 License: UNKNOWN
 Description: 
         <p align="center">
@@ -13,14 +13,18 @@
         	</a>
         	<h3 align="center">Analyze VCFs and collaborate on solving rare diseases quicker</h3>
         </p>
         
         [![Build Status][travis-img]][travis-url]
         [![PyPI Version][pypi-img]][pypi-url]
         [![Coverage Status](https://coveralls.io/repos/github/Clinical-Genomics/scout/badge.svg?branch=master)](https://coveralls.io/github/Clinical-Genomics/scout?branch=master)
+        [![GitHub issues-closed][closed-issues-img]][closed-issues-url]
+        [![Average time to resolve an issue][ismaintained-resolve-img]][ismaintained-resolve-url]
+        [![Percentage of issues still open][ismaintained-open-rate-img]][ismaintained-open-rate-url]
+        [![GitHub commits](https://img.shields.io/github/commits-since/Clinical-Genomics/scout/v4.8.0.svg)](https://GitHub.com/Clinical-Genomics/scout/commit/)
         
         ## What is Scout?
         
         - **Simple** - Analyze variants in a simple to use web interface.
         - **Aggregation** - Combine results from multiple analyses and VCFs into a centralized database.
         - **Collaboration** - Write comments and share cases between users and institutes.
         
@@ -182,14 +186,20 @@
         
         
         [chanjo]: https://github.com/Clinical-Genomics/chanjo
         [travis-img]: https://img.shields.io/travis/Clinical-Genomics/scout/develop.svg?style=flat-square
         [travis-url]: https://travis-ci.org/Clinical-Genomics/scout
         [pypi-img]: https://img.shields.io/pypi/v/scout-browser.svg?style=flat-square
         [pypi-url]: https://pypi.python.org/pypi/scout-browser/
+        [ismaintained-resolve-img]: http://isitmaintained.com/badge/resolution/Clinical-Genomics/scout.svg
+        [ismaintained-resolve-url]: http://isitmaintained.com/project/Clinical-Genomics/scout
+        [ismaintained-open-rate-img]: http://isitmaintained.com/badge/open/Clinical-Genomics/scout.svg
+        [ismaintained-open-rate-url]: http://isitmaintained.com/project/Clinical-Genomics/scout
+        [closed-issues-img]: https://img.shields.io/github/issues-closed/Clinical-Genomics/scout.svg
+        [closed-issues-url]: https://GitHub.com/Clinical-Genomics/scout/issues?q=is%3Aissue+is%3Aclosed
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,63 +1,69 @@
-Metadata-Version: 2.1 Name: scout-browser Version: 4.8.3 Summary: Clinical DNA
+Metadata-Version: 2.1 Name: scout-browser Version: 4.9.0 Summary: Clinical DNA
 variant visualizer and browser. Home-page: https://github.com/Clinical-
 Genomics/scout Author: MÃ¥ns Magnusson Author-email:
 mans.magnusson@scilifelab.se License: UNKNOWN Description:
                           [artwork/logo-display.png]
     **** Analyze VCFs and collaborate on solving rare diseases quicker ****
 [![Build Status][travis-img]][travis-url] [![PyPI Version][pypi-img]][pypi-url]
 [![Coverage Status](https://coveralls.io/repos/github/Clinical-Genomics/scout/
 badge.svg?branch=master)](https://coveralls.io/github/Clinical-Genomics/
-scout?branch=master) ## What is Scout? - **Simple** - Analyze variants in a
-simple to use web interface. - **Aggregation** - Combine results from multiple
-analyses and VCFs into a centralized database. - **Collaboration** - Write
-comments and share cases between users and institutes. ## Documentation This
-README only gives a brief overview of Scout, for a more complete reference,
-please check out our docs: [www.clinicalgenomics.se/scout](http://
-www.clinicalgenomics.se/scout/). ## Installation  ```bash git clone https://
-github.com/Clinical-Genomics/scout cd scout pip install --requirement
-requirements.txt --editable . ``` Scout PDF reports are created using [Flask-
-WeasyPrint](https://pythonhosted.org/Flask-WeasyPrint/). This library requires
-external dependencies which need be installed separately (namely Cairo and
-Pango). See platform-specific instructions for Linux, macOS and Windows
-available on the WeasyPrint installation [pages](https://
-weasyprint.readthedocs.io/en/stable/install.html#). You also need to have an
-instance of MongoDB running. I've found that it's easiest to do using the
-official Docker image: ```bash docker run --name mongo -p 27017:27017 mongo ```
-## Usage ### Demo Once installed, you can setup Scout by running a few commands
-using the included command line interface. Given you have a MongoDB server
-listening on the default port (27017), this is how you would setup a fully
-working Scout demo: ```bash scout setup demo ``` This will setup an instance of
-scout with a database called `scout-demo`. Now run ```bash scout --demo serve
-``` And play around with the interface. A user has been created with email
-clark.kent@mail.com so use that adress to get access ### Initialize scout To
-initialize a working instance with all genes, diseases etc run ```bash scout
-setup database ``` for more info, run `scout --help` > If you intent to use
-authentication, make sure you are using a Google email! The previous command
-setup the database with a curated collection of gene definitions with links to
-OMIM along with HPO phenotype terms. Now we will load some example data. Scout
-expects the analysis to be accomplished using various gene panels so let's load
-one and then our first analysis case: ```bash scout load panel scout/demo/
-panel_1.txt scout load case scout/demo/643594.config.yaml ``` ## Integration
-with chanjo for coverage report visualization Scout may be configured to
-visualize coverage reports produced by [Chanjo][chanjo]. Instructions on how to
-enable this feature can be found in the document [chanjo_coverage_integration]
-(docs/admin-guide/chanjo_coverage_integration.md). ## Server setup Scout needs
-a server config to know which databases to connect to etc. Depending on which
-information you provide you activate different parts of the interface
-automatically, including user authentication, coverage, and local observations.
-This is an example of the config file: ```python # scoutconfig.py # list of
-email addresses to send errors to in production ADMINS =
-['paul.anderson@magnolia.com'] MONGO_HOST = 'localhost' MONGO_PORT = 27017
-MONGO_DBNAME = 'scoutTest' MONGO_USERNAME = 'testUser' MONGO_PASSWORD =
-'testPass' # enable user authentication using Google OAuth GOOGLE = dict
-( consumer_key='CLIENT_ID', consumer_secret='CLIENT_SECRET', base_url='https://
-www.googleapis.com/oauth2/v1/', authorize_url='https://accounts.google.com/o/
-oauth2/auth', request_token_url=None, request_token_params={ 'scope': ("https:/
-/www.googleapis.com/auth/userinfo.profile " "https://www.googleapis.com/auth/
+scout?branch=master) [![GitHub issues-closed][closed-issues-img]][closed-
+issues-url] [![Average time to resolve an issue][ismaintained-resolve-img]]
+[ismaintained-resolve-url] [![Percentage of issues still open][ismaintained-
+open-rate-img]][ismaintained-open-rate-url] [![GitHub commits](https://
+img.shields.io/github/commits-since/Clinical-Genomics/scout/v4.8.0.svg)](https:
+//GitHub.com/Clinical-Genomics/scout/commit/) ## What is Scout? - **Simple** -
+Analyze variants in a simple to use web interface. - **Aggregation** - Combine
+results from multiple analyses and VCFs into a centralized database. -
+**Collaboration** - Write comments and share cases between users and
+institutes. ## Documentation This README only gives a brief overview of Scout,
+for a more complete reference, please check out our docs:
+[www.clinicalgenomics.se/scout](http://www.clinicalgenomics.se/scout/). ##
+Installation  ```bash git clone https://github.com/Clinical-Genomics/scout cd
+scout pip install --requirement requirements.txt --editable . ``` Scout PDF
+reports are created using [Flask-WeasyPrint](https://pythonhosted.org/Flask-
+WeasyPrint/). This library requires external dependencies which need be
+installed separately (namely Cairo and Pango). See platform-specific
+instructions for Linux, macOS and Windows available on the WeasyPrint
+installation [pages](https://weasyprint.readthedocs.io/en/stable/
+install.html#). You also need to have an instance of MongoDB running. I've
+found that it's easiest to do using the official Docker image: ```bash docker
+run --name mongo -p 27017:27017 mongo ``` ## Usage ### Demo Once installed, you
+can setup Scout by running a few commands using the included command line
+interface. Given you have a MongoDB server listening on the default port
+(27017), this is how you would setup a fully working Scout demo: ```bash scout
+setup demo ``` This will setup an instance of scout with a database called
+`scout-demo`. Now run ```bash scout --demo serve ``` And play around with the
+interface. A user has been created with email clark.kent@mail.com so use that
+adress to get access ### Initialize scout To initialize a working instance with
+all genes, diseases etc run ```bash scout setup database ``` for more info, run
+`scout --help` > If you intent to use authentication, make sure you are using a
+Google email! The previous command setup the database with a curated collection
+of gene definitions with links to OMIM along with HPO phenotype terms. Now we
+will load some example data. Scout expects the analysis to be accomplished
+using various gene panels so let's load one and then our first analysis case:
+```bash scout load panel scout/demo/panel_1.txt scout load case scout/demo/
+643594.config.yaml ``` ## Integration with chanjo for coverage report
+visualization Scout may be configured to visualize coverage reports produced by
+[Chanjo][chanjo]. Instructions on how to enable this feature can be found in
+the document [chanjo_coverage_integration](docs/admin-guide/
+chanjo_coverage_integration.md). ## Server setup Scout needs a server config to
+know which databases to connect to etc. Depending on which information you
+provide you activate different parts of the interface automatically, including
+user authentication, coverage, and local observations. This is an example of
+the config file: ```python # scoutconfig.py # list of email addresses to send
+errors to in production ADMINS = ['paul.anderson@magnolia.com'] MONGO_HOST =
+'localhost' MONGO_PORT = 27017 MONGO_DBNAME = 'scoutTest' MONGO_USERNAME =
+'testUser' MONGO_PASSWORD = 'testPass' # enable user authentication using
+Google OAuth GOOGLE = dict( consumer_key='CLIENT_ID',
+consumer_secret='CLIENT_SECRET', base_url='https://www.googleapis.com/oauth2/
+v1/', authorize_url='https://accounts.google.com/o/oauth2/auth',
+request_token_url=None, request_token_params={ 'scope': ("https://
+www.googleapis.com/auth/userinfo.profile " "https://www.googleapis.com/auth/
 userinfo.email"), }, access_token_url='https://accounts.google.com/o/oauth2/
 token', access_token_method='POST' ) # enable Phenomizer gene predictions from
 phenotype terms PHENOMIZER_USERNAME = '???' PHENOMIZER_PASSWORD = '???' #
 enable Chanjo coverage integration SQLALCHEMY_DATABASE_URI = '???'
 REPORT_LANGUAGE = 'en' # or 'sv' # other interesting settings
 SQLALCHEMY_TRACK_MODIFICATIONS = False # this is essential in production
 TEMPLATES_AUTO_RELOAD = False # consider turning off in production SECRET_KEY =
@@ -87,14 +93,22 @@
 regardless of the amount of code provided or your skills as a programmer. More
 info on how to contribute to the project and a description of the Scout
 branching workflow can be found [here](CONTRIBUTING.md). [chanjo]: https://
 github.com/Clinical-Genomics/chanjo [travis-img]: https://img.shields.io/
 travis/Clinical-Genomics/scout/develop.svg?style=flat-square [travis-url]:
 https://travis-ci.org/Clinical-Genomics/scout [pypi-img]: https://
 img.shields.io/pypi/v/scout-browser.svg?style=flat-square [pypi-url]: https://
-pypi.python.org/pypi/scout-browser/ Platform: UNKNOWN Classifier: Environment
-:: Web Environment Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: BSD License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Topic ::
-Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
-Development :: Libraries Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown Provides-Extra: coverage
+pypi.python.org/pypi/scout-browser/ [ismaintained-resolve-img]: http://
+isitmaintained.com/badge/resolution/Clinical-Genomics/scout.svg [ismaintained-
+resolve-url]: http://isitmaintained.com/project/Clinical-Genomics/scout
+[ismaintained-open-rate-img]: http://isitmaintained.com/badge/open/Clinical-
+Genomics/scout.svg [ismaintained-open-rate-url]: http://isitmaintained.com/
+project/Clinical-Genomics/scout [closed-issues-img]: https://img.shields.io/
+github/issues-closed/Clinical-Genomics/scout.svg [closed-issues-url]: https://
+GitHub.com/Clinical-Genomics/scout/issues?q=is%3Aissue+is%3Aclosed Platform:
+UNKNOWN Classifier: Environment :: Web Environment Classifier: Intended
+Audience :: Developers Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Classifier: Topic :: Software Development :: Libraries Classifier: Programming
+Language :: Python :: 3.6 Description-Content-Type: text/markdown Provides-
+Extra: coverage
```

### Comparing `scout-browser-4.8.3/scout_browser.egg-info/SOURCES.txt` & `scout-browser-4.9.0/scout_browser.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 MANIFEST.in
 README.md
 requirements-dev.txt
 requirements.txt
 setup.cfg
 setup.py
 scout/__init__.py
-scout/__main__.py
 scout/__version__.py
 scout/adapter/__init__.py
 scout/adapter/client.py
 scout/adapter/utils.py
 scout/adapter/mongo/__init__.py
 scout/adapter/mongo/acmg.py
 scout/adapter/mongo/base.py
@@ -132,14 +131,15 @@
 scout/demo/643594.clinical.SV.vcf.gz.tbi
 scout/demo/643594.clinical.str.annotated.limits.vcf.gz
 scout/demo/643594.clinical.str.annotated.limits.vcf.gz.tbi
 scout/demo/643594.clinical.str.annotated.vcf.gz
 scout/demo/643594.clinical.str.annotated.vcf.gz.tbi
 scout/demo/643594.clinical.str.vcf.gz
 scout/demo/643594.clinical.str.vcf.gz.tbi
+scout/demo/643594.clinical.vcf
 scout/demo/643594.clinical.vcf.gz
 scout/demo/643594.clinical.vcf.gz.tbi
 scout/demo/643594.config.yaml
 scout/demo/643594.ped
 scout/demo/643594.ped_check.csv
 scout/demo/643594.peddy.ped
 scout/demo/643594.research.SV.vcf.gz
@@ -152,28 +152,120 @@
 scout/demo/643595.config.yaml
 scout/demo/ADM1059A1.dummy.cgh
 scout/demo/ADM1059A2.dummy.cgh
 scout/demo/ADM1059A3.dummy.cgh
 scout/demo/__init__.py
 scout/demo/cancer.load_config.yaml
 scout/demo/cancer_test.ped
-scout/demo/cancer_test.vcf
 scout/demo/cancer_test.vcf.gz
 scout/demo/cancer_test.vcf.gz.tbi
 scout/demo/chanjo4_demo.sql
 scout/demo/delivery_report.html
 scout/demo/empty.clinical.SV.vcf.gz
 scout/demo/empty.clinical.SV.vcf.gz.tbi
-scout/demo/empty_vcf.config.yaml
+scout/demo/ideo_upd_roh.zip
 scout/demo/madeline.xml
-scout/demo/panel_1.bed
+scout/demo/output.chrn.wig
+scout/demo/output.wig
+scout/demo/output.wig.orig
 scout/demo/panel_1.csv
 scout/demo/panel_1.txt
 scout/demo/reduced_mt.bam
 scout/demo/reduced_mt.bam.bai
+scout/demo/test.bw
+scout/demo/test1.bw
+scout/demo/test2.bw
+scout/demo/images/__MACOSX/roh_images/._.DS_Store
+scout/demo/images/__MACOSX/roh_images/._roh_chr1.png
+scout/demo/images/__MACOSX/roh_images/._roh_chr12.png
+scout/demo/images/__MACOSX/roh_images/._roh_chr17 bak.png
+scout/demo/images/__MACOSX/roh_images/._roh_chr17.png
+scout/demo/images/__MACOSX/roh_images/._roh_chr19.png
+scout/demo/images/__MACOSX/roh_images/._roh_chr2.png
+scout/demo/images/__MACOSX/roh_images/._roh_chr21.png
+scout/demo/images/__MACOSX/roh_images/._roh_chr6.png
+scout/demo/images/__MACOSX/upd_images/._test_upd.sites.bed
+scout/demo/images/__MACOSX/upd_images/._test_upd.sites.bed.gz
+scout/demo/images/__MACOSX/upd_images/._upd_chr1.png
+scout/demo/images/chr_images/cytoBand.txt.chr1.png
+scout/demo/images/chr_images/cytoBand.txt.chr10.png
+scout/demo/images/chr_images/cytoBand.txt.chr11.png
+scout/demo/images/chr_images/cytoBand.txt.chr12.png
+scout/demo/images/chr_images/cytoBand.txt.chr13.png
+scout/demo/images/chr_images/cytoBand.txt.chr14.png
+scout/demo/images/chr_images/cytoBand.txt.chr15.png
+scout/demo/images/chr_images/cytoBand.txt.chr16.png
+scout/demo/images/chr_images/cytoBand.txt.chr17.png
+scout/demo/images/chr_images/cytoBand.txt.chr18.png
+scout/demo/images/chr_images/cytoBand.txt.chr19.png
+scout/demo/images/chr_images/cytoBand.txt.chr2.png
+scout/demo/images/chr_images/cytoBand.txt.chr20.png
+scout/demo/images/chr_images/cytoBand.txt.chr21.png
+scout/demo/images/chr_images/cytoBand.txt.chr22.png
+scout/demo/images/chr_images/cytoBand.txt.chr3.png
+scout/demo/images/chr_images/cytoBand.txt.chr4.png
+scout/demo/images/chr_images/cytoBand.txt.chr5.png
+scout/demo/images/chr_images/cytoBand.txt.chr6.png
+scout/demo/images/chr_images/cytoBand.txt.chr7.png
+scout/demo/images/chr_images/cytoBand.txt.chr8.png
+scout/demo/images/chr_images/cytoBand.txt.chr9.png
+scout/demo/images/chr_images/cytoBand.txt.chrX.png
+scout/demo/images/chr_images/cytoBand.txt.chrY.png
+scout/demo/images/roh_images/roh_chr1.png
+scout/demo/images/roh_images/roh_chr10.png
+scout/demo/images/roh_images/roh_chr11.png
+scout/demo/images/roh_images/roh_chr12.png
+scout/demo/images/roh_images/roh_chr13.png
+scout/demo/images/roh_images/roh_chr14.png
+scout/demo/images/roh_images/roh_chr15.png
+scout/demo/images/roh_images/roh_chr16.png
+scout/demo/images/roh_images/roh_chr17 bak.png
+scout/demo/images/roh_images/roh_chr17.png
+scout/demo/images/roh_images/roh_chr18.png
+scout/demo/images/roh_images/roh_chr19.png
+scout/demo/images/roh_images/roh_chr2.png
+scout/demo/images/roh_images/roh_chr20.png
+scout/demo/images/roh_images/roh_chr21.png
+scout/demo/images/roh_images/roh_chr22.png
+scout/demo/images/roh_images/roh_chr3.png
+scout/demo/images/roh_images/roh_chr4.png
+scout/demo/images/roh_images/roh_chr5.png
+scout/demo/images/roh_images/roh_chr6.png
+scout/demo/images/roh_images/roh_chr7.png
+scout/demo/images/roh_images/roh_chr8.png
+scout/demo/images/roh_images/roh_chr9.png
+scout/demo/images/roh_images/roh_chrM.png
+scout/demo/images/roh_images/roh_chrX.png
+scout/demo/images/roh_images/roh_chrY.png
+scout/demo/images/upd_images/test_upd.sites.bed
+scout/demo/images/upd_images/test_upd.sites.bed.gz
+scout/demo/images/upd_images/upd_chr1.png
+scout/demo/images/upd_images/upd_chr10.png
+scout/demo/images/upd_images/upd_chr11.png
+scout/demo/images/upd_images/upd_chr12.png
+scout/demo/images/upd_images/upd_chr13.png
+scout/demo/images/upd_images/upd_chr14.png
+scout/demo/images/upd_images/upd_chr15.png
+scout/demo/images/upd_images/upd_chr16.png
+scout/demo/images/upd_images/upd_chr17.png
+scout/demo/images/upd_images/upd_chr18.png
+scout/demo/images/upd_images/upd_chr19.png
+scout/demo/images/upd_images/upd_chr2.png
+scout/demo/images/upd_images/upd_chr20.png
+scout/demo/images/upd_images/upd_chr21.png
+scout/demo/images/upd_images/upd_chr22.png
+scout/demo/images/upd_images/upd_chr3.png
+scout/demo/images/upd_images/upd_chr4.png
+scout/demo/images/upd_images/upd_chr5.png
+scout/demo/images/upd_images/upd_chr6.png
+scout/demo/images/upd_images/upd_chr7.png
+scout/demo/images/upd_images/upd_chr8.png
+scout/demo/images/upd_images/upd_chr9.png
+scout/demo/images/upd_images/upd_chrX.png
+scout/demo/images/upd_images/upd_chrcombined.png
 scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_diseases_to_genes_to_phenotypes_reduced.txt
 scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_genes_to_phenotype_reduced.txt
 scout/demo/resources/ALL_SOURCES_ALL_FREQUENCIES_phenotype_to_genes_reduced.txt
 scout/demo/resources/__init__.py
 scout/demo/resources/chanjo4_structure.sql
 scout/demo/resources/ensembl_exons_37_reduced.txt
 scout/demo/resources/ensembl_exons_38_reduced.txt
@@ -324,33 +416,32 @@
 scout/server/blueprints/panels/templates/panels/panels.html
 scout/server/blueprints/phenotypes/__init__.py
 scout/server/blueprints/phenotypes/controllers.py
 scout/server/blueprints/phenotypes/views.py
 scout/server/blueprints/phenotypes/templates/phenotypes/hpo_terms.html
 scout/server/blueprints/public/__init__.py
 scout/server/blueprints/public/views.py
+scout/server/blueprints/public/static/favicon.ico
 scout/server/blueprints/public/static/logo-karolinska.png
 scout/server/blueprints/public/static/logo-scilifelab.png
 scout/server/blueprints/public/static/scout-logo.png
 scout/server/blueprints/public/static/swedac.png
 scout/server/blueprints/public/templates/public/index.html
 scout/server/blueprints/variant/__init__.py
 scout/server/blueprints/variant/controllers.py
 scout/server/blueprints/variant/utils.py
 scout/server/blueprints/variant/verification_controllers.py
 scout/server/blueprints/variant/views.py
 scout/server/blueprints/variant/templates/variant/acmg.html
 scout/server/blueprints/variant/templates/variant/clinvar.html
 scout/server/blueprints/variant/templates/variant/sv-variant.html
-scout/server/blueprints/variant/templates/variant/utils.html
 scout/server/blueprints/variant/templates/variant/variant.html
 scout/server/blueprints/variants/__init__.py
 scout/server/blueprints/variants/controllers.py
 scout/server/blueprints/variants/forms.py
-scout/server/blueprints/variants/utils.py
 scout/server/blueprints/variants/views.py
 scout/server/blueprints/variants/templates/variants/cancer-variants.html
 scout/server/blueprints/variants/templates/variants/components.html
 scout/server/blueprints/variants/templates/variants/str-variants.html
 scout/server/blueprints/variants/templates/variants/sv-variants.html
 scout/server/blueprints/variants/templates/variants/utils.html
 scout/server/blueprints/variants/templates/variants/variants.html
@@ -383,14 +474,15 @@
 scout_browser.egg-info/SOURCES.txt
 scout_browser.egg-info/dependency_links.txt
 scout_browser.egg-info/entry_points.txt
 scout_browser.egg-info/not-zip-safe
 scout_browser.egg-info/requires.txt
 scout_browser.egg-info/top_level.txt
 tests/conftest.py
+tests/test_protocol.md
 tests/adapter/conftest.py
 tests/adapter/mongo/test_adapter_variant_caseid.py
 tests/adapter/mongo/test_case_handling.py
 tests/adapter/mongo/test_clinvar_handler.py
 tests/adapter/mongo/test_comment_handling.py
 tests/adapter/mongo/test_connect.py
 tests/adapter/mongo/test_evaluated_variants.py
@@ -516,14 +608,15 @@
 tests/parse/test_parse_variant.py
 tests/parse/vcfs/one_cnvnator.vcf
 tests/server/conftest.py
 tests/server/test_links.py
 tests/server/test_server_utils.py
 tests/server/blueprints/cases/test_cases_controllers.py
 tests/server/blueprints/cases/test_cases_views.py
+tests/server/blueprints/cases/test_cases_views.py.suggestion
 tests/server/blueprints/cases/test_cases_views_gene_variants.py
 tests/server/blueprints/cases/test_matchmaker_controllers.py
 tests/server/blueprints/dashboard/test_dashboard_controllers.py
 tests/server/blueprints/dashboard/test_dashboard_views.py
 tests/server/blueprints/genes/test_genes_views.py
 tests/server/blueprints/institutes/test_institutes_views.py
 tests/server/blueprints/login/test_models.py
```

### Comparing `scout-browser-4.8.3/setup.py` & `scout-browser-4.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/conftest.py` & `scout-browser-4.9.0/tests/adapter/conftest.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_adapter_variant_caseid.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_adapter_variant_caseid.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_case_handling.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_case_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,26 @@
     assert adapter.case_collection.find_one() is None
     adapter.case_collection.insert_one(case_obj)
     ## WHEN retreiving an existing case from the database
     result = adapter.cases()
     ## THEN we should get the correct case
     assert sum(1 for i in result) == 1
 
+def test_get_prioritized_cases(adapter, case_obj, institute_obj):
+    ## GIVEN an empty database (no cases)
+    assert adapter.case_collection.find_one() is None
+    # WHEN inserting a prioritized case
+    case_obj['status']='prioritized'
+    adapter.case_collection.insert_one(case_obj)
+
+    # WHEN retrieving prioritized casese for the institute
+    result = adapter.prioritized_cases(institute_id=institute_obj['_id'])
+
+    # THEN one prioritized case is returned
+    assert sum(1 for i in result) == 1
 
 def test_nr_cases(adapter, case_obj):
     ## GIVEN an empty database (no cases)
     ## WHEN adding one case to the case collection
     adapter.case_collection.insert_one(case_obj)
     ## THEN the function nr_cases should return number of cases = 1
     result = adapter.nr_cases(institute_id=case_obj['owner'])
@@ -381,14 +393,37 @@
     assert hgnc_symbol
 
     # WHEN updating dynamic gene list with gene
     adapter.update_dynamic_gene_list(case_obj, hgnc_symbols=[hgnc_symbol])
     # THEN a the gene list will contain a gene
     assert len(adapter.case(case_obj['_id'])['dynamic_gene_list']) == 1
 
+def test_update_dynamic_gene_list_with_bad_dict_entry(gene_database, case_obj):
+
+    # GIVEN an populated gene database,
+    adapter = gene_database
+
+    # GIVEN an **incorrectly** assigned dict instead of list as dynamic panel
+    case_obj['dynamic_gene_list'] = {}
+
+    # GIVEN a case with an empty dynamic_gene_list
+    adapter.case_collection.insert_one(case_obj)
+    assert adapter.case_collection.find_one()
+    assert len(adapter.case(case_obj['_id'])['dynamic_gene_list']) == 0
+
+    # GIVEN a gene with a gene symobl
+    gene_obj = gene_database.hgnc_collection.find_one({'build': '37'})
+    assert gene_obj
+    hgnc_symbol = gene_obj.get('hgnc_symbol')
+    assert hgnc_symbol
+
+    # WHEN updating dynamic gene list with gene
+    adapter.update_dynamic_gene_list(case_obj, hgnc_symbols=[hgnc_symbol])
+    # THEN a the gene list will contain a gene
+    assert len(adapter.case(case_obj['_id'])['dynamic_gene_list']) == 1
 
 def test_update_case_individuals(adapter, case_obj):
     # GIVEN an empty database (no cases)
     assert adapter.case_collection.find_one() is None
     adapter.case_collection.insert_one(case_obj)
     assert adapter.case_collection.find_one()
     logger.info("Testing to update case")
@@ -430,16 +465,14 @@
     adapter.update_status(institute_obj, res, user_obj, 'active', 'blank')
     res = adapter.case(case_obj['_id'])
     # case becomes active
     assert res['status'] == 'active'
     # and user becomes assignee
     assert user_obj['email'] in res['assignees']
 
-
-
 def test_update_case_rerun_status(adapter, case_obj, institute_obj, user_obj, ):
 
     # GIVEN an empty database (no cases)
     assert sum(1 for i in adapter.cases()) == 0
     adapter.case_collection.insert_one(case_obj)
     assert sum(1 for i in adapter.cases()) == 1
```

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_clinvar_handler.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_clinvar_handler.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_comment_handling.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_comment_handling.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_connect.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_connect.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_evaluated_variants.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_evaluated_variants.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_event_handling.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_event_handling.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_gene_handler.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_gene_handler.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_hpo_handler.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_hpo_handler.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_index_handling.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_index_handling.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_institute_handler.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_institute_handler.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_load_adapter_case.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_load_adapter_case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_matchmaker.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_matchmaker.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_panel_handler.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_panel_handler.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_query.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_query.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_sanger_validation.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_sanger_validation.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_transcript_handler.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_transcript_handler.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_user_handling.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_user_handling.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_variant_events.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_variant_events.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_variant_handling.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_variant_handling.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/adapter/mongo/test_variant_loader.py` & `scout-browser-4.9.0/tests/adapter/mongo/test_variant_loader.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/conftest.py` & `scout-browser-4.9.0/tests/build/conftest.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_case.py` & `scout-browser-4.9.0/tests/build/test_build_case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_clnsig.py` & `scout-browser-4.9.0/tests/build/test_build_clnsig.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_disease.py` & `scout-browser-4.9.0/tests/build/test_build_disease.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_exon.py` & `scout-browser-4.9.0/tests/build/test_build_exon.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_gene.py` & `scout-browser-4.9.0/tests/build/test_build_gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_hgnc_gene.py` & `scout-browser-4.9.0/tests/build/test_build_hgnc_gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_hpo.py` & `scout-browser-4.9.0/tests/build/test_build_hpo.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_individual.py` & `scout-browser-4.9.0/tests/build/test_build_individual.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_panel.py` & `scout-browser-4.9.0/tests/build/test_build_panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/build/test_build_variant.py` & `scout-browser-4.9.0/tests/build/test_build_variant.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/conftest.py` & `scout-browser-4.9.0/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/delete/test_delete_cmd.py` & `scout-browser-4.9.0/tests/commands/delete/test_delete_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/export/test_export_cases_cmd.py` & `scout-browser-4.9.0/tests/commands/export/test_export_cases_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/export/test_export_gene.py` & `scout-browser-4.9.0/tests/commands/export/test_export_gene.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/export/test_export_hpo_cmd.py` & `scout-browser-4.9.0/tests/commands/export/test_export_hpo_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/export/test_export_mt_report_cmd.py` & `scout-browser-4.9.0/tests/commands/export/test_export_mt_report_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/export/test_export_panel_cmd.py` & `scout-browser-4.9.0/tests/commands/export/test_export_panel_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/export/test_export_transcripts_cmd.py` & `scout-browser-4.9.0/tests/commands/export/test_export_transcripts_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/export/test_export_variant_cmd.py` & `scout-browser-4.9.0/tests/commands/export/test_export_variant_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/load/test_load_case_cmd.py` & `scout-browser-4.9.0/tests/commands/load/test_load_case_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/load/test_load_delivery_report_cmd.py` & `scout-browser-4.9.0/tests/commands/load/test_load_delivery_report_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/load/test_load_institute_cmd.py` & `scout-browser-4.9.0/tests/commands/load/test_load_institute_cmd.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # -*- coding: utf-8 -*-
 
 from scout.commands import cli
 from scout.server.extensions import store
 
-def test_load_institute(mock_app, institute_obj):
+def test_load_institute(empty_mock_app):
     """Testing the load institute cli command"""
 
+    ## GIVEN an empty database and some institute information
+    mock_app = empty_mock_app
     runner = mock_app.test_cli_runner()
     assert runner
+    ins_id = "cust000"
+    display_name = "A special name"
 
-    # One institute is preloaded into populated database
-    assert sum(1 for i in store.institute_collection.find()) == 1
+    assert sum(1 for i in store.institute_collection.find()) == 0
 
-    # remove it
-    store.institute_collection.find_one_and_delete({'_id':institute_obj['_id']})
-    assert store.institute_collection.find_one() is None
-
-    # and re-load it using the CLI command:
-    result =  runner.invoke(cli, ['load', 'institute',
-        '-i', institute_obj['_id'], '-d', institute_obj['display_name'],
-        '-s', institute_obj['sanger_recipients']])
+    ## WHEN loading the institute into the database
+    result =  runner.invoke(cli, ['load', 'institute', '-i', ins_id, '-d', display_name])
 
-    # CLI command should be exit with no errors
+    ## THEN assert command exits without errors
     assert result.exit_code == 0
-
-    # and institute should be in database
+    
+    ## THEN assert logging is correct
+    assert 'Adding institute with internal_id: {0} and display_name: {1}'.format(
+            ins_id,display_name) in result.output
+    
+    ## THEN assert institute is added
     assert sum(1 for i in store.institute_collection.find()) == 1
```

### Comparing `scout-browser-4.8.3/tests/commands/load/test_load_panel_cmd.py` & `scout-browser-4.9.0/tests/commands/load/test_load_panel_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/load/test_load_region_cmd.py` & `scout-browser-4.9.0/tests/commands/load/test_load_region_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/load/test_load_research_cmd.py` & `scout-browser-4.9.0/tests/commands/load/test_load_research_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/load/test_load_user_cmd.py` & `scout-browser-4.9.0/tests/commands/load/test_load_user_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/load/test_load_variants_cmd.py` & `scout-browser-4.9.0/tests/commands/load/test_load_variants_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/test_base_command.py` & `scout-browser-4.9.0/tests/commands/test_base_command.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/test_convert_cmd.py` & `scout-browser-4.9.0/tests/commands/test_convert_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/test_delete_case_cmd.py` & `scout-browser-4.9.0/tests/commands/test_delete_case_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/test_index_cmd.py` & `scout-browser-4.9.0/tests/commands/test_index_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/test_setup_cmd.py` & `scout-browser-4.9.0/tests/commands/test_setup_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/update/test_update_case_cmd.py` & `scout-browser-4.9.0/tests/commands/update/test_update_case_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/update/test_update_compounds_cli.py` & `scout-browser-4.9.0/tests/commands/update/test_update_compounds_cli.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/update/test_update_disease_cmd.py` & `scout-browser-4.9.0/tests/commands/update/test_update_disease_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/update/test_update_groups_cmd.py` & `scout-browser-4.9.0/tests/commands/update/test_update_groups_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/update/test_update_hpo_cmd.py` & `scout-browser-4.9.0/tests/commands/update/test_update_hpo_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/update/test_update_institute_cmd.py` & `scout-browser-4.9.0/tests/commands/update/test_update_institute_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/update/test_update_omim_cmd.py` & `scout-browser-4.9.0/tests/commands/update/test_update_omim_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/update/test_update_panel_cmd.py` & `scout-browser-4.9.0/tests/commands/update/test_update_panel_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/update/test_update_user_cmd.py` & `scout-browser-4.9.0/tests/commands/update/test_update_user_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_panels_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_panels_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_aliases_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_aliases_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_cases.py` & `scout-browser-4.9.0/tests/commands/view/test_view_cases.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_cases_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_cases_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_diseases_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_diseases_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_hgnc.py` & `scout-browser-4.9.0/tests/commands/view/test_view_hgnc.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_hpo_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_hpo_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_index_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_index_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_individuals_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_individuals_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_institutes_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_institutes_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_intervals_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_intervals_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_transcripts_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_transcripts_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/commands/view/test_view_whitelist_cmd.py` & `scout-browser-4.9.0/tests/commands/view/test_view_whitelist_cmd.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/conftest.py` & `scout-browser-4.9.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 def case_obj(request, parsed_case):
 
     LOG.info("Create a case obj")
     case = parsed_case
     case['_id'] = parsed_case['case_id']
     case['owner'] = parsed_case['owner']
     case['created_at'] = parsed_case['analysis_date']
-    case['dynamic_gene_list'] = {}
+    case['dynamic_gene_list'] = []
     case['genome_version'] = None
     case['has_svvariants'] = True
 
     case['individuals'][0]['sex'] = '1'
     case['individuals'][1]['sex'] = '1'
     case['individuals'][2]['sex'] = '2'
```

### Comparing `scout-browser-4.8.3/tests/export/test_export_variants.py` & `scout-browser-4.9.0/tests/export/test_export_variants.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/fixtures/vcfs/clinvar.vcf` & `scout-browser-4.9.0/tests/fixtures/vcfs/clinvar.vcf`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/fixtures/vcfs/no_clinvar.vcf` & `scout-browser-4.9.0/tests/fixtures/vcfs/no_clinvar.vcf`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/load/test_load_case.py` & `scout-browser-4.9.0/tests/load/test_load_case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/load/test_load_exons.py` & `scout-browser-4.9.0/tests/load/test_load_exons.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/load/test_load_hgnc_genes.py` & `scout-browser-4.9.0/tests/load/test_load_hgnc_genes.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/load/test_load_hpo.py` & `scout-browser-4.9.0/tests/load/test_load_hpo.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/load/test_load_institute.py` & `scout-browser-4.9.0/tests/update/test_update_institute.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/load/test_load_panel.py` & `scout-browser-4.9.0/tests/load/test_load_panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/load/test_load_report.py` & `scout-browser-4.9.0/tests/load/test_load_report.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/load/test_load_transcripts.py` & `scout-browser-4.9.0/tests/load/test_load_transcripts.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/load/test_load_variant.py` & `scout-browser-4.9.0/tests/load/test_load_variant.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_frequency.py` & `scout-browser-4.9.0/tests/parse/test_frequency.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_ids.py` & `scout-browser-4.9.0/tests/parse/test_ids.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_callers.py` & `scout-browser-4.9.0/tests/parse/test_parse_callers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_case.py` & `scout-browser-4.9.0/tests/parse/test_parse_case.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_clinvar_form.py` & `scout-browser-4.9.0/tests/parse/test_parse_clinvar_form.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_clnsig.py` & `scout-browser-4.9.0/tests/parse/test_parse_clnsig.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_compounds.py` & `scout-browser-4.9.0/tests/parse/test_parse_compounds.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_conservation.py` & `scout-browser-4.9.0/tests/parse/test_parse_conservation.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_coordinates.py` & `scout-browser-4.9.0/tests/parse/test_parse_coordinates.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_ensembl_exons.py` & `scout-browser-4.9.0/tests/parse/test_parse_ensembl_exons.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_ensembl_transcripts.py` & `scout-browser-4.9.0/tests/parse/test_parse_ensembl_transcripts.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_exac_genes.py` & `scout-browser-4.9.0/tests/parse/test_parse_exac_genes.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_genes.py` & `scout-browser-4.9.0/tests/parse/test_parse_genes.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_genotype.py` & `scout-browser-4.9.0/tests/parse/test_parse_genotype.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_headers.py` & `scout-browser-4.9.0/tests/parse/test_parse_headers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_hgnc.py` & `scout-browser-4.9.0/tests/parse/test_parse_hgnc.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_hpo_disease.py` & `scout-browser-4.9.0/tests/parse/test_parse_hpo_disease.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_hpo_terms.py` & `scout-browser-4.9.0/tests/parse/test_parse_hpo_terms.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_match_matchmaker.py` & `scout-browser-4.9.0/tests/parse/test_parse_match_matchmaker.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_omim.py` & `scout-browser-4.9.0/tests/parse/test_parse_omim.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_panel.py` & `scout-browser-4.9.0/tests/parse/test_parse_panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_rank_score.py` & `scout-browser-4.9.0/tests/parse/test_parse_rank_score.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_transcripts.py` & `scout-browser-4.9.0/tests/parse/test_parse_transcripts.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/test_parse_variant.py` & `scout-browser-4.9.0/tests/parse/test_parse_variant.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/parse/vcfs/one_cnvnator.vcf` & `scout-browser-4.9.0/tests/parse/vcfs/one_cnvnator.vcf`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/cases/test_cases_views.py` & `scout-browser-4.9.0/tests/server/blueprints/cases/test_cases_views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/cases/test_cases_views_gene_variants.py` & `scout-browser-4.9.0/tests/server/blueprints/cases/test_cases_views_gene_variants.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/cases/test_matchmaker_controllers.py` & `scout-browser-4.9.0/tests/server/blueprints/cases/test_matchmaker_controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/dashboard/test_dashboard_controllers.py` & `scout-browser-4.9.0/tests/server/blueprints/dashboard/test_dashboard_controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/dashboard/test_dashboard_views.py` & `scout-browser-4.9.0/tests/server/blueprints/dashboard/test_dashboard_views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/genes/test_genes_views.py` & `scout-browser-4.9.0/tests/server/blueprints/genes/test_genes_views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/institutes/test_institutes_views.py` & `scout-browser-4.9.0/tests/server/blueprints/institutes/test_institutes_views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/login/test_views.py` & `scout-browser-4.9.0/tests/server/blueprints/login/test_views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 # -*- coding: utf-8 -*-
 from flask import url_for
 from flask_login import current_user
 from scout.server.extensions import store
 from flask_ldap3_login.forms import LDAPLoginForm
 
 
-def test_unathorized_login(app):
+def test_unathorized_login(app, institute_obj, case_obj):
     """Test failed authentication against scout database"""
 
     # GIVEN an initialized app
     # WHEN trying tp access scout with the email of an non-existing user
     with app.test_client() as client:
         resp = client.get(url_for('login.login', email='fakey_user@email.com'))
 
         # THEN response should redirect to user authentication form (index page)
         assert resp.status_code == 302
         # And current user should NOT be authenticated
         assert current_user.is_authenticated is False
 
+        # And also WHEN requesting a (known) case page
+        attribute_error = False
+        try:
+            resp = client.get(url_for('cases.case',
+                              institute_id=institute_obj['internal_id'],
+                              case_name=case_obj['display_name']))
+        except AttributeError:
+            attribute_error=True
+        # THEN an error is raised
+        assert attribute_error
+
 
 def test_authorized_login(app, user_obj):
     """Test successful authentication against scout database"""
 
     # GIVEN an initialized app
     # WHEN trying to access scout with the email of an existing user
     with app.test_client() as client:
```

### Comparing `scout-browser-4.8.3/tests/server/blueprints/panels/test_panels_views.py` & `scout-browser-4.9.0/tests/server/blueprints/panels/test_panels_views.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,14 +66,33 @@
         content_type="application/x-www-form-urlencoded"
     )
     # THEN the pending actions of panel should be updated:
     panel_obj = adapter.gene_panels()[0]
     assert panel_obj['pending'][0]['action'] == 'delete'
     assert panel_obj['pending'][0]['hgnc_id'] == a_gene['hgnc_id']
 
+    # WHEN removing that gene using the client
+    new_version = panel_obj['version'] + 1
+    data = urlencode({
+        'action' : 'submit',
+        'version': new_version})
+
+    resp = client.post(url_for('panels.panel_update', panel_id=panel_obj['_id']),
+        data=data,
+        content_type="application/x-www-form-urlencoded"
+    )
+
+    # THEN the new panel object should have the correct new version
+    new_panel_obj = adapter.gene_panel(panel_obj['panel_name'])
+    assert new_panel_obj['version'] == new_version
+
+    # needs a real app context due to user check. Repeat with app?
+    #resp = client.get(url_for('panels.panels'))
+    #assert new_version in str(resp.data)
+
     # remove gene from panel object using adapter:
     panel_obj['genes'] = panel_obj['genes'][1:]
     updated_panel = adapter.update_panel(panel_obj)
 
     # WHEN posting an add gene request to panel page
     data = urlencode({
         'action' : 'add',
```

### Comparing `scout-browser-4.8.3/tests/server/blueprints/phenotypes/test_phenotypes_controllers.py` & `scout-browser-4.9.0/tests/server/blueprints/phenotypes/test_phenotypes_controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/phenotypes/test_phenotypes_views.py` & `scout-browser-4.9.0/tests/server/blueprints/phenotypes/test_phenotypes_views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/variant/test_variant_controllers.py` & `scout-browser-4.9.0/tests/server/blueprints/variant/test_variant_controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/variant/test_variant_utils.py` & `scout-browser-4.9.0/tests/server/blueprints/variant/test_variant_utils.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/variant/test_variant_verification_controllers.py` & `scout-browser-4.9.0/tests/server/blueprints/variant/test_variant_verification_controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/variant/test_variant_views.py` & `scout-browser-4.9.0/tests/server/blueprints/variant/test_variant_views.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/variants/test_variants_controllers.py` & `scout-browser-4.9.0/tests/server/blueprints/variants/test_variants_controllers.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/blueprints/variants/test_variants_utils.py` & `scout-browser-4.9.0/tests/server/blueprints/variants/test_variants_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 from flask import get_template_attribute
+from scout.server.blueprints.variants.forms import FiltersForm
 
 def test_modal_causative(app, case_obj, institute_obj, variant_obj):
 
     # GIVEN an initialized app
     with app.test_client() as client:
 
         # WHILE collection a specific jinja macro
@@ -22,7 +23,20 @@
         }
         # and/or OMIM diagnoses
         case_obj['diagnosis_phenotypes'] = [ 616833 ]
 
         # THEN the macro should allow to assign partial causatives
         html = macro(case_obj, institute_obj, variant_obj)
         assert 'Assign at least an OMIM diagnosis or a HPO phenotype term' not in html
+
+
+def test_modal_prompt_filter_name(app):
+    # GIVEN an initialized app
+    with app.test_client() as client:
+        # WHILE collection a specific jinja macro
+        macro = get_template_attribute('variants/utils.html', 'modal_prompt_filter_name')
+        # and passing to it the required parameters
+        # Including a case without HPO phenotype or diagnosis (OMIM terms) assigned
+        form = FiltersForm()
+        html = macro(form)
+        # THEN a string from the modal can be found in the output
+        assert('Please name' in html)
```

### Comparing `scout-browser-4.8.3/tests/server/blueprints/variants/test_variants_views.py` & `scout-browser-4.9.0/tests/server/blueprints/variants/test_variants_views.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,33 @@
         # WHEN accessing the variants page
         resp = client.get(url_for('variants.variants',
                                   institute_id=institute_obj['internal_id'],
                                   case_name=case_obj['display_name']))
         # THEN it should return a page
         assert resp.status_code == 200
 
+def test_variants_research(app, institute_obj, case_obj):
+    # GIVEN an initialized app
+    # GIVEN a valid user and institute
+
+    with app.test_client() as client:
+        # GIVEN that the user could be logged in
+        resp = client.get(url_for('auto_login'))
+        assert resp.status_code == 200
+
+        # WHEN accessing the variants page
+        resp = client.get(url_for('variants.variants',
+                                  institute_id=institute_obj['internal_id'],
+                                  case_name=case_obj['display_name'],
+                                  variant_type='research'))
+        # THEN it should return a page
+        assert resp.status_code == 200
+        # THEN a reset filters link with variant type should have been made
+        assert "variant_type=research" in str(resp.data)
+
 def test_variants_post_data(app, institute_obj, case_obj):
     # GIVEN an initialized app
     # GIVEN a valid user and institute
 
     with app.test_client() as client:
         # GIVEN that the user could be logged in
         resp = client.get(url_for('auto_login'))
@@ -56,14 +75,30 @@
         # WHEN accessing the sv-variants page
         resp = client.get(url_for('variants.sv_variants',
                                   institute_id=institute_obj['internal_id'],
                                   case_name=case_obj['display_name']))
         # THEN it should return a page
         assert resp.status_code == 200
 
+def test_sv_variants_research(app, institute_obj, case_obj):
+    with app.test_client() as client:
+        # GIVEN that the user could be logged in
+        resp = client.get(url_for('auto_login'))
+        assert resp.status_code == 200
+
+        # WHEN accessing the sv-variants page
+        resp = client.get(url_for('variants.sv_variants',
+                                  institute_id=institute_obj['internal_id'],
+                                  case_name=case_obj['display_name'],
+                                  variant_type="research"))
+        # THEN it should return a page
+        assert resp.status_code == 200
+        # THEN a reset filters link with variant type should have been made
+        assert "variant_type=research" in str(resp.data)
+
 def test_sv_variants_post_data(app, institute_obj, case_obj):
     # GIVEN an initialized app
     # GIVEN a valid user and institute
 
     with app.test_client() as client:
         # GIVEN that the user could be logged in
         resp = client.get(url_for('auto_login'))
```

### Comparing `scout-browser-4.8.3/tests/server/conftest.py` & `scout-browser-4.9.0/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/server/test_links.py` & `scout-browser-4.9.0/tests/server/test_links.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/update/test_update_compounds.py` & `scout-browser-4.9.0/tests/update/test_update_compounds.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/update/test_update_institute.py` & `scout-browser-4.9.0/tests/load/test_load_institute.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/update/test_update_panel.py` & `scout-browser-4.9.0/tests/update/test_update_panel.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/utils/test_acmg.py` & `scout-browser-4.9.0/tests/utils/test_acmg.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/utils/test_algorithms.py` & `scout-browser-4.9.0/tests/utils/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/utils/test_convert.py` & `scout-browser-4.9.0/tests/utils/test_convert.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/utils/test_date.py` & `scout-browser-4.9.0/tests/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/utils/test_ensembl_rest_clients.py` & `scout-browser-4.9.0/tests/utils/test_ensembl_rest_clients.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/utils/test_link_genes.py` & `scout-browser-4.9.0/tests/utils/test_link_genes.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/utils/test_par.py` & `scout-browser-4.9.0/tests/utils/test_par.py`

 * *Files identical despite different names*

### Comparing `scout-browser-4.8.3/tests/utils/test_requests.py` & `scout-browser-4.9.0/tests/utils/test_requests.py`

 * *Files identical despite different names*

