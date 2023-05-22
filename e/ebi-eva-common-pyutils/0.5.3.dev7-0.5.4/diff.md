# Comparing `tmp/ebi_eva_common_pyutils-0.5.3.dev7.tar.gz` & `tmp/ebi_eva_common_pyutils-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.5.3.dev7.tar", last modified: Fri Apr 28 16:50:33 2023, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.5.4.tar", last modified: Mon May 22 22:02:46 2023, max compression
```

## Comparing `ebi_eva_common_pyutils-0.5.3.dev7.tar` & `ebi_eva_common_pyutils-0.5.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1492 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/CHANGELOG.md
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    11357 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/LICENSE
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       28 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/MANIFEST.in
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/PKG-INFO
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1434 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/README.md
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4984 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/archive_directory.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/assembly/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       66 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/assembly/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1570 2023-04-28 09:52:41.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/assembly/assembly.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2151 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/command_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1192 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/common_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2242 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/config.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     8356 2023-04-28 16:29:30.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/config_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/contig_alias/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3056 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1452 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/ena_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1375 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/file_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4990 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/logger.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    14953 2023-04-28 09:52:41.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/metadata_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3589 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongo_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongodb/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       72 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongodb/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     9676 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongodb/mongo_database.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4859 2023-04-28 16:47:03.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/ncbi_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2285 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/network_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/nextflow/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      120 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/nextflow/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    10114 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     4398 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/pg_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      134 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    12162 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/assembly.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3911 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/sequence.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)    14310 2023-04-28 16:32:46.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/spring_properties.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/taxonomy/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     2259 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/__init__.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     3515 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/assembly_utils.py
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     5230 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-28 16:50:33.659999 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 nkumar2   (9636) eva       (1254)     1699 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)        1 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       81 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)       23 2023-04-28 16:50:33.000000 ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/top_level.txt
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      225 2023-04-28 16:50:33.663999 ebi_eva_common_pyutils-0.5.3.dev7/setup.cfg
--rw-r--r--   0 nkumar2   (9636) eva       (1254)      912 2023-04-28 11:34:28.000000 ebi_eva_common_pyutils-0.5.3.dev7/setup.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1706 2023-05-22 22:00:57.000000 ebi_eva_common_pyutils-0.5.4/CHANGELOG.md
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    11357 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/LICENSE
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       28 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/MANIFEST.in
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      512 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/PKG-INFO
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1434 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/README.md
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4984 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/archive_directory.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/assembly/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       66 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1570 2023-04-28 09:52:41.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2151 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/command_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1192 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/common_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2242 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/config.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     8356 2023-05-07 09:15:50.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/config_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/contig_alias/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3056 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1452 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/ena_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1375 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/file_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4990 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/logger.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    14953 2023-04-28 09:52:41.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/metadata_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3589 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongo_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongodb/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       72 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongodb/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     9676 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongodb/mongo_database.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4859 2023-05-07 09:16:05.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2285 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/network_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/nextflow/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      120 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/nextflow/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    10114 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4398 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/pg_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      134 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    12162 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/assembly.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3911 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/sequence.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    14347 2023-05-22 11:31:10.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/spring_properties.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/taxonomy/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2259 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3515 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/assembly_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     5230 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-05-22 22:02:46.156029 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      512 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1699 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        1 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       81 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       23 2023-05-22 22:02:46.000000 ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      225 2023-05-22 22:02:46.160029 ebi_eva_common_pyutils-0.5.4/setup.cfg
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      907 2023-05-22 22:00:57.000000 ebi_eva_common_pyutils-0.5.4/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/CHANGELOG.md` & `ebi_eva_common_pyutils-0.5.4/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 
 Changelog for ebi_eva_common_pyutils
 ===========================
 
+0.5.4 (2023-05-22)
+----------------
+
+- Add job tracker properties to accession import job
+
+0.5.3 (2023-05-07)
+----------------
+
+- Add spring properties generation option for variant load and accession import jobs
+
 0.5.2 (2023-03-03)
 ----------------
 
 - Add new spring properties generation options
 
 0.5.1 (2022-12-21)
 ----------------
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/LICENSE` & `ebi_eva_common_pyutils-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/PKG-INFO` & `ebi_eva_common_pyutils-0.5.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi_eva_common_pyutils
-Version: 0.5.3.dev7
+Version: 0.5.4
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/README.md` & `ebi_eva_common_pyutils-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/spring_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
             'spring.datasource.tomcat.max-active': 3,
             'spring.jpa.generate-ddl': 'true',
 
             'mongodb.read-preference': read_preference,
 
             'spring.main.web-application-type': 'none',
             'spring.main.allow-bean-definition-overriding': 'true',
-            'spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation': True,
-            'spring.jpa.properties.hibernate.temp.use_jdbc_metadata_defaults': False,
+            'spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation': 'true',
+            'spring.jpa.properties.hibernate.temp.use_jdbc_metadata_defaults': 'false',
             'spring.jpa.database-platform': 'org.hibernate.dialect.PostgreSQL9Dialect',
             'parameters.chunkSize': chunk_size,
         }
         merge = {**self._mongo_properties(), **self._count_stats_properties(), **props}
         return merge
 
     def _common_accessioning_properties(self, assembly_accession, read_preference, chunk_size):
@@ -219,56 +219,55 @@
                 'parameters.assemblyReportUrl': self._format_str('file:{0}', assembly_report),
                 'parameters.outputFolder': output_folder,
                 'parameters.accessionedVcf': accessioned_vcf,
                 'logging.level.uk.ac.ebi.eva.accession.release': 'INFO'
             })
 
     def _common_eva_pipeline_properties(self, opencga_path, read_preference='secondaryPreferred'):
+        files_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.files']
+        annotation_metadata_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotation-metadata']
+        annotation_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotations']
         variants_collection = get_properties_from_xml_file(
             self.maven_profile, self.private_settings_file)['eva.mongo.collections.variants']
+        job_tracker_properties = self._variant_load_job_tracker_properties()
         props = {
             'spring.profiles.active': 'production,mongo',
             'spring.profiles.include': 'variant-writer-mongo,variant-annotation-mongo',
 
             'spring.data.mongodb.authentication-mechanism': 'SCRAM-SHA-1',
             'job.repository.driverClassName': 'org.postgresql.Driver',
 
             'db.collections.variants.name': variants_collection,
+            'db.collections.files.name': files_collection,
+            'db.collections.annotation-metadata.name': annotation_metadata_collection,
+            'db.collections.annotations.name': annotation_collection,
 
             'app.opencga.path': opencga_path,
             'config.restartability.allow': 'false',
             'config.db.read-preference': read_preference,
 
             'logging.level.embl.ebi.variation.eva': 'DEBUG',
             'logging.level.org.opencb.opencga': 'DEBUG',
             'logging.level.org.springframework': 'INFO',
         }
 
-        merge = {**self._common_properties(read_preference=read_preference, chunk_size=100), **props}
+        merge = {**self._common_properties(read_preference=read_preference, chunk_size=100), **props, **job_tracker_properties}
         return merge
 
     def get_accession_import_properties(self, opencga_path, read_preference='secondaryPreferred'):
         return self._format(self._common_eva_pipeline_properties(opencga_path, read_preference))
 
     def get_variant_load_properties(self, project_accession, study_name, output_dir, annotation_dir, stats_dir,
                                     vep_cache_path, opencga_path, read_preference='secondaryPreferred'):
-        files_collection = get_properties_from_xml_file(
-            self.maven_profile, self.private_settings_file)['eva.mongo.collections.files']
-        annotation_metadata_collection = get_properties_from_xml_file(
-            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotation-metadata']
-        annotation_collection = get_properties_from_xml_file(
-            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotations']
         return self._format(
             self._common_eva_pipeline_properties(opencga_path, read_preference),
-            self._variant_load_job_tracker_properties(),
             {
-                'db.collections.files.name': files_collection,
-                'db.collections.annotation-metadata.name': annotation_metadata_collection,
-                'db.collections.annotations.name': annotation_collection,
-
                 'annotation.overwrite': False,
                 'app.vep.cache.path': vep_cache_path,
                 'app.vep.num-forks': 4,
                 'app.vep.timeout': 500,
                 'config.chunk.size': 200,
 
                 'input.study.id': project_accession,
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/assembly_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/PKG-INFO` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebi-eva-common-pyutils
-Version: 0.5.3.dev7
+Version: 0.5.4
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.5.4/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.3.dev7/setup.py` & `ebi_eva_common_pyutils-0.5.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_common_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.5.3-dev7',
+    version='0.5.4',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['psycopg2-binary', 'requests', 'pymongo', 'lxml', 'pyyaml', 'cached-property', 'retry',
                       'networkx<=2.5'],
     classifiers=[
```

