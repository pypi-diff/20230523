# Comparing `tmp/cazy_webscraper-2.2.8.tar.gz` & `tmp/cazy_webscraper-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cazy_webscraper-2.2.8.tar", last modified: Wed Apr 26 13:33:02 2023, max compression
+gzip compressed data, was "cazy_webscraper-2.3.0.tar", last modified: Tue May 23 14:28:36 2023, max compression
```

## Comparing `cazy_webscraper-2.2.8.tar` & `cazy_webscraper-2.3.0.tar`

### file list

```diff
@@ -1,130 +1,139 @@
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.252468 cazy_webscraper-2.2.8/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1169 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/LICENSE
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    60950 2023-04-26 13:33:02.252468 cazy_webscraper-2.2.8/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    59902 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/README.md
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    10307 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/api/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1450 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/api/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    22929 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/api/cw_query_database.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/cazy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    18900 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/cazy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    13681 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/cazy_scraper.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/crawler/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4585 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/crawler/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    20748 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/crawler/get_validation_data.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper/expand/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2391 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1657 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11472 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/extract_db_seqs.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1495 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1533 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    24982 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/entrez.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    24100 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/get_genome_accs.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1508 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    25103 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/get_genbank_sequences.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1538 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    30711 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/get_ncbi_taxs.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8409 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     9413 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/get_gtdb_tax.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.228468 cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1655 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6715 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/get_pdb_structures.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/expand/uniprot/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1574 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/uniprot/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    24313 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/expand/uniprot/get_uniprot_data.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2554 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/gene_names/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    10668 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/gene_names/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/genomes/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8789 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/genomes/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/sequences/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    12894 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/sequences/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1486 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    21970 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/lineage.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    12045 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/multiple_taxa.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/sql/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1462 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.232468 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8480 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.236468 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1532 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    14773 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_cazyme_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4676 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_genbank_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7642 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_genome_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5492 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_gtdb_tax.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7599 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_ncbi_tax_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    18748 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_uniprot_data.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.236468 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1535 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    16230 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_api_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6989 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_assemblies.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4774 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_records.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    13821 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_selected_gbks.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3942 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_selected_pdbs.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    15484 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_table_dicts.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    13770 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_taxonomies.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    17953 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_orm.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.240468 cazy_webscraper-2.2.8/cazy_webscraper/utilities/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2319 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.240468 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    21390 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3907 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/cazy_class_synonym_dict.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.240468 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1493 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7011 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/api_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8612 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/cazy_webscraper_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8408 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/extract_seq_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7991 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/gbk_seq_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7903 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/get_genomes_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7891 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/get_gtdb_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8017 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/pdb_strctre_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7724 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/tax_ncbi_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     9968 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/uniprot_parser.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.224468 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    60950 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4088 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/SOURCES.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/dependency_links.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)      672 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/entry_points.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)      127 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/requires.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       16 2023-04-26 13:33:02.000000 cazy_webscraper-2.2.8/cazy_webscraper.egg-info/top_level.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-04-26 13:33:02.252468 cazy_webscraper-2.2.8/setup.cfg
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4337 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/setup.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:33:02.252468 cazy_webscraper-2.2.8/tests/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5480 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_add_cazymes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    19877 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_api.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11219 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_cazy_init.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2944 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_crawler.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6180 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_cw_init.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1834 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_expand.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3540 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_extract_seqs.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    21513 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_get_ncbi_tax.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    13574 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_gtdb.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3460 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_ncbi.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11718 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_ncbi_genomes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5398 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_orm.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7541 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_parse_config.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4412 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_parsers.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5970 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_pdb.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3398 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_ad_genbank.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5648 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_ad_genomes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5298 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_ad_gtdb.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5723 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_ad_ncbi_tax.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3406 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_interf_gd_get_records.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11054 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_interf_gd_get_tax.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5698 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_interface.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)        0 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_sql_queries.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4526 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_table_dicts.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6093 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_taxonomy.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6982 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_uniprot.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1827 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_utilities.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    18609 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_validation_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    23129 2023-04-26 13:32:20.000000 cazy_webscraper-2.2.8/tests/test_webscraper.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.612437 cazy_webscraper-2.3.0/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1169 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/LICENSE
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    66981 2023-05-23 14:28:36.612437 cazy_webscraper-2.3.0/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    65933 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/README.md
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.588437 cazy_webscraper-2.3.0/cazy_webscraper/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11118 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.588437 cazy_webscraper-2.3.0/cazy_webscraper/api/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1450 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/api/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    22929 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/api/cw_query_database.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.592437 cazy_webscraper-2.3.0/cazy_webscraper/cache/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1479 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/cache/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2562 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/cache/cazy.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4550 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/cache/ncbi.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4407 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/cache/uniprot.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.592437 cazy_webscraper-2.3.0/cazy_webscraper/cazy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    20079 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/cazy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    14793 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/cazy_scraper.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.592437 cazy_webscraper-2.3.0/cazy_webscraper/crawler/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4585 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/crawler/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    20748 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/crawler/get_validation_data.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.592437 cazy_webscraper-2.3.0/cazy_webscraper/expand/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2391 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.592437 cazy_webscraper-2.3.0/cazy_webscraper/expand/extract_seqs/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1657 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/extract_seqs/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11472 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/extract_seqs/extract_db_seqs.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.592437 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1495 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.592437 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/genomes/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1533 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/genomes/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    24982 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/genomes/entrez.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    24100 2023-04-26 14:09:30.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/genomes/get_genome_accs.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.592437 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/sequences/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1508 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/sequences/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    22217 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/sequences/get_genbank_sequences.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.592437 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/taxonomy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1538 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/taxonomy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    30711 2023-04-26 14:09:48.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/taxonomy/get_ncbi_taxs.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.596437 cazy_webscraper-2.3.0/cazy_webscraper/expand/gtdb/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8409 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/gtdb/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     9413 2023-04-26 14:09:30.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/gtdb/get_gtdb_tax.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.596437 cazy_webscraper-2.3.0/cazy_webscraper/expand/pdb/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1655 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/pdb/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6715 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/pdb/get_pdb_structures.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.596437 cazy_webscraper-2.3.0/cazy_webscraper/expand/uniprot/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1574 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/uniprot/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    25925 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/expand/uniprot/get_uniprot_data.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.596437 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2554 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.596437 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/gene_names/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    10663 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/gene_names/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.596437 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/genomes/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8789 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/genomes/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.596437 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/sequences/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    12894 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/sequences/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.596437 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/taxonomy/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1486 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/taxonomy/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    21970 2023-04-26 14:09:48.000000 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/taxonomy/lineage.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    12732 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/ncbi/taxonomy/multiple_taxa.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.600437 cazy_webscraper-2.3.0/cazy_webscraper/sql/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1462 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2580 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/get_schema.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.600437 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8480 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.600437 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1532 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    14884 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_cazyme_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4676 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_genbank_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7642 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_genome_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5492 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_gtdb_tax.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7599 2023-04-26 14:09:48.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_ncbi_tax_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    20162 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_uniprot_data.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.600437 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/delete_data/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7330 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/delete_data/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.604437 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1535 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    16230 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_api_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6989 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_assemblies.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4774 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_records.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    13821 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_selected_gbks.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3942 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_selected_pdbs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    16277 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_table_dicts.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    13770 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_taxonomies.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    18829 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_orm.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.604437 cazy_webscraper-2.3.0/cazy_webscraper/utilities/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2319 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/__init__.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.604437 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parse_configuration/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    21390 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parse_configuration/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3907 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parse_configuration/cazy_class_synonym_dict.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.604437 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1493 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/__init__.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7011 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/api_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     9230 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/cazy_webscraper_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8408 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/extract_seq_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7991 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/gbk_seq_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7903 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/get_genomes_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7891 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/get_gtdb_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2980 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/get_schema_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     8017 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/pdb_strctre_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7724 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/tax_ncbi_parser.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    10914 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/uniprot_parser.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.588437 cazy_webscraper-2.3.0/cazy_webscraper.egg-info/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    66981 2023-05-23 14:28:36.000000 cazy_webscraper-2.3.0/cazy_webscraper.egg-info/PKG-INFO
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4362 2023-05-23 14:28:36.000000 cazy_webscraper-2.3.0/cazy_webscraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-05-23 14:28:36.000000 cazy_webscraper-2.3.0/cazy_webscraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)      727 2023-05-23 14:28:36.000000 cazy_webscraper-2.3.0/cazy_webscraper.egg-info/entry_points.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)      123 2023-05-23 14:28:36.000000 cazy_webscraper-2.3.0/cazy_webscraper.egg-info/requires.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       16 2023-05-23 14:28:36.000000 cazy_webscraper-2.3.0/cazy_webscraper.egg-info/top_level.txt
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-05-23 14:28:36.612437 cazy_webscraper-2.3.0/setup.cfg
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4414 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/setup.py
+drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-05-23 14:28:36.612437 cazy_webscraper-2.3.0/tests/
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5477 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/tests/test_add_cazymes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    19877 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_api.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     9717 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/tests/test_cazy_init.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     2944 2023-04-04 09:33:36.000000 cazy_webscraper-2.3.0/tests/test_crawler.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6180 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_cw_init.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1834 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_expand.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3540 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_extract_seqs.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    21513 2023-04-26 14:09:48.000000 cazy_webscraper-2.3.0/tests/test_get_ncbi_tax.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    13574 2023-04-26 14:09:30.000000 cazy_webscraper-2.3.0/tests/test_gtdb.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3460 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_ncbi.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11718 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_ncbi_genomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5398 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_orm.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7541 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_parse_config.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4397 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/tests/test_parsers.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5970 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_pdb.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3466 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/tests/test_sql_ad_genbank.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5648 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_sql_ad_genomes.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5298 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_sql_ad_gtdb.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5723 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_sql_ad_ncbi_tax.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     3406 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_sql_interf_gd_get_records.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    11054 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_sql_interf_gd_get_tax.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     5698 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_sql_interface.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)        0 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_sql_queries.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     4526 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_table_dicts.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     6575 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/tests/test_taxonomy.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     7805 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/tests/test_uniprot.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)     1827 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_utilities.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    18609 2023-03-30 07:15:44.000000 cazy_webscraper-2.3.0/tests/test_validation_data.py
+-rw-rw-r--   0 emmah     (1009) emmah     (1010)    23488 2023-05-23 14:27:41.000000 cazy_webscraper-2.3.0/tests/test_webscraper.py
```

### Comparing `cazy_webscraper-2.2.8/LICENSE` & `cazy_webscraper-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/PKG-INFO` & `cazy_webscraper-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,46 @@
-Metadata-Version: 2.1
-Name: cazy_webscraper
-Version: 2.2.8
-Summary: A tool to automate retrieving data from CAZy, build a local CAZyme SQL database, and throughly interrogating the data. Also, automate retrieving protein data, sequences, EC numbers and structure files for specific datasets in the CAZyme database from UniProt, GenBank and PDB.
-Home-page: https://github.com/HobnobMancer/cazy_webscraper
-Author: Emma E. M. Hobbs
-Author-email: eemh1@st-andrews.ac.uk
-License: MIT
-Keywords: bioinforamtics protein webscraper
-Platform: Posix
-Platform: MacOS X
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cazy_webscraper
 
 -------------------------------
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6343936.svg)](https://doi.org/10.5281/zenodo.6343936)
 [![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazy_webscraper/blob/master/LICENSE)  
 [![CircleCI](https://circleci.com/gh/HobnobMancer/cazy_webscraper.svg?style=shield)](https://circleci.com/gh/HobnobMancer/cazy_webscraper)
 [![codecov](https://codecov.io/gh/HobnobMancer/cazy_webscraper/branch/master/graph/badge.svg)](https://codecov.io/gh/HobnobMancer/cazy_webscraper)
 [![Documentation Status](https://readthedocs.org/projects/cazy-webscraper/badge/?version=latest)](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest)  
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/version.svg)](https://anaconda.org/bioconda/cazy_webscraper)
 [![Anaconda-Update Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/latest_release_date.svg)](https://anaconda.org/bioconda/cazy_webscraper)  
 [![pyani PyPi version](https://img.shields.io/pypi/v/cazy_webscraper "PyPI version")](https://pypi.python.org/pypi/cazy_webscraper)  
 [![Downloads](https://pepy.tech/badge/cazy-webscraper)](https://pepy.tech/project/cazy-webscraper)
 
--------------------------------
-
-> `cazy_webscraper` version 1 is depracted. Please ensure you are using version 2 or newer.  
-> `bioconda` installation is fixed for >= v2.1.3.1
+--------------------------------
 
 ## cazy_webscraper
 
 `cazy_webscraper` is an application and Python3 package for the automated retrieval of protein data from the [CAZy](http://wwww.cazy.org/) database. The code is distributed under the MIT license.
+The full documentation can be found at [Read the Docs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
 
 **`cazy_webscraper` retrieves protein data from the [CAZy database](https://www.cazy.org) and stores the data in a local SQLite3 database.** This enables users to integrate the dataset into analytical pipelines, and interrogate the data in a manner unachievable through the CAZy website.
 
 **Data can be retrieved for user defined datasets of interest.** `cazy_webscraper` can recover specified CAZy Classes and/or CAZy families. These queries can be filtered by taxonomy at Kingdoms, genus, species or strain level. Successive CAZy queries can be collated into a single local database. A log of each query is recorded in the database for transparency, reproducibility and shareablity.
 
 **Using the `expand` subcommand, a user can expand the core dataset.** Specifically, `cazy_webscraper` can be used to retrieve data from the following external databases for CAZymes in the local CAZyme database that meet user specified criteria, and adds the downloaded data to the local CAZyme database:
 
 **[GenBank](https://www.ncbi.nlm.nih.gov/genbank/):**  
 - Protein sequences 
 - Latest taxonomic classification - including complete lineage (including phylum, class, order and family) (version >=2.1.2)
 - Latest genomic assembly data (GenBank and RefSeq (when available) version accession and ID numbers) (version >=2.1.3)
 
-**[UniProt](https://www.uniprot.org/):**  
+**[UniProt](https://www.uniprot.org/):** 
+- UniProt ID/accession
 - Protein name
-- UniProt accession
 - EC numbers
 - PDB accessions
-- Protein sequences
+- Protein sequence (and date sequence was last updated)
+- Taxonomic classification (genus and species)
 
 **[Research Collaboratory for Structural Bioinformatics (RCSB) Protein Data Bank (PDB)](https://www.rcsb.org/):**
 - Protein structure files
 - *Structure files are written to disk, **not** stored in the local CAZyme database*
 
 **[Genome Taxonomy Database (GTDB)](https://gtdb.ecogenomic.org/):**
 Retrieve the latest archaeal and bacterial taxonomic classifications (including complete lineages from kingdom to species) - available in `cazy_webscraper` verion >= 2.2.0.
@@ -76,20 +52,64 @@
 - A FASTA file per extracted protein sequence
 - A local BLASTP database
 
 **The `cazy_webscraper` API facilitates interoggating the local CAZyme database.**
 
 Please see the [full documentation at ReadTheDocs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
 
+## Updates
+
+**New in version 2.3.0**
+* Downloading protein data from UniProt is several magnitudes faster than before - and should have fewer issues with using older version of `bioservices`
+    - Uses `bioservices` mapping to map directly from NCBI protein version accession to UniProt
+    - `cw_get_uniprot_data` not longer calls to NCBI and thus no longer requires an email address as a positional argument
+* Updated database schema: Changed `Genbanks 1--* Uniprots` to `Genbanks *--1 Uniprots`. `Uniprots.uniprot_id` is now listed in the `Genbanks` table, instead of listing `Genbanks.genbank_id` in the `Uniprots` table
+
+* Retrieve taxonomic classifications from UniProt
+    * Use the `--taxonomy`/`-t` flag to retrieve the scientific name (genus and species) for proteins of interest
+    * Adds downloaded taxonomic information to the `UniprotsTaxs` table
+
+* Improved clarrification of deleting old records when using `cw_get_uniprot_data`
+    - Separate arguments to delete Genbanks-EC number and Genbanks-PDB accession relationships that are no longer listed in UniProt for those proteins in the local CAZyme database for proteins whom data is downloaded from UniProt
+    - New args:
+        - `--delete_old_ec_relationships` = deletes Genbank(protein)-EC number relationships no longer in UniProt
+        - `--delete_old_ecs` = deletes EC numbers in the local db not linked to any proteins
+        - `--delete_old_pdb_relationships` = deletes Genbank(protein)-PDB relationships no longer in UniProt
+        - `--delete_old_pdbs` = deletes PDB accessions in the local db not linked to any proteins
+
+* Retrieve the local db schema
+    - New command `cw_get_db_schema` added.
+    - Retrieves the SQLite schema of a local CAZyme database and prints it to the terminal
+
+* Added option to skip retrieving the latest taxonomic classifications NCBI taxonomies
+    - By default, when retreiving data from CAZy, `cazy_webscraper` retrieves the latest taxonomic classifications for proteins listed under multiple tax
+    - To increase scrapping time, and to reduce burden on the NCBI-Entrez server, if this data is not needed (e.g. GTDB taxs will be use) this step can be skipped by using the new `--skip_ncbi_tax` flag.
+    - When skipping retrieval of the latest taxa classifications from NCBI, `cazy_webscraper` will add the first taxa retrieved from CAZy for those proteins listed under mutliple taxa
+
+
 ## Documentation
 
+The full documentation can be found at [Read the Docs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
+
+### Our paper: Implementation and demonstration of use
+
 For a full description of the operation and examples of use, please see our paper in (BioRxiv)[https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full].
 
 > Hobbs, E. E. M., Gloster, T. M., and Pritchard, L. (2022) 'cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets', _bioRxiv_, [https://doi.org/10.1101/2022.12.02.518825](https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full)
 
+### Database structure
+
+You can view the database schema [here](#database-schema) and find a PDF of the database schema [here](https://hobnobmancer.github.io/cazy_webscraper/database_schema.pdf).
+
+## Contributions
+
+We welcome contributions and suggestions. You can raise issues at this repository, or fork the repository and submit pull requests, at the links below:
+
+- [Issues](https://github.com/HobnobMancer/cazy_webscraper/issues)
+- [Pull Requests](https://github.com/HobnobMancer/cazy_webscraper/pulls)
 
 ## Table of Contents
 <!-- TOC -->
 - [`cazy_webscraper`](#cazy_webscraper)
 - [Citation](#citation)
 - [Best practice](#best-practice)
 - [Documentation](#documentation)
@@ -114,24 +134,24 @@
 - [Retrieving GTDB taxonomies](#retrieving-gtdb-taxonomies)
     - [Configuring retrieving GTDB taxonomies](#configuring-retrieving-gtdb-taxonomies)
 - [The `cazy_webscraper` API or Interrogating the local CAZyme database](#the_cazy_webscraper_api_or_interrogating_the_local_cazyme_database)
 - [Configuring `cazy_webscraper` using a YAML file](#configuring-using-a-yaml-file)
 - [CAZy coverage of GenBank](#cazy-coverage-of-genbank)
     - [Configure calculating CAZy coverage of GenBank](#configure-calculating-cazy-coverage-of-genbank)
 - [Integrating a local CAZyme database](#integrating-a-local-cazyme-database)
+- [Database schema](#database-schema)
 - [Contributions](#contributions)
 - [License and copyright](#license-and-copyright)
 <!-- /TOC -->
 
 
 ## Features in the pipeline:
 - Retrieve and stored PubMed IDs in the local CAZyme database
 - Fix any remaining bugs we can find (if you find a bug, please report it and provide as detailed bug report as possible!)
-- Update the unit tests to work with the new `cazy_webscraper` architecture
-- Update the documentation
+- Increase unit test coverage
 - Automate analysing the taxonomic distribution across CAZy and datasets of interest, including generating a final report
 
 ## Citation
 
 If you use `cazy_webscraper`, please cite the following publication:
 
 > Hobbs, E. E. M., Gloster, T. M., and Pritchard, L. (2022) 'cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets', _bioRxiv_, [https://doi.org/10.1101/2022.12.02.518825](https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1)
@@ -190,21 +210,29 @@
 ```
 
 ### Version and citation
 
 To retrieve the version, use the following command:
 
 ```bash
-cazy_webscraper <user_email> -V
+cazy_webscraper -V
+```
+or
+```bash
+cazy_webscraper --version
 ```
 
 To retrieve the citation to use:
 
 ```bash
-cazy_webscraper <user_email> -C
+cazy_webscraper -C
+```
+or
+```bash
+cazy_webscraper --citation
 ```
 
 ### Command summary
 
 Below are the list of commands (excluding required and optional arguments) included in `cazy_webscraper`.
 
 #### CAZy
@@ -236,19 +264,35 @@
 
 **Note:** PDB structure files are retrieved for the PDB accessions that are *in* a local CAZyme database created using `cazy_webscraper`. A freshly built CAZyme database only contains NCBI protein accessions, taxonomic kingdoms, source organisms, and CAZy family annotations. Therefore, the `cw_get_uniprot_data` command must be used to retrieve PDB accessions from the UniProt database **prior** to using the `cw_get_pdb_structures` command.
 
 #### Interrogate the database
 
 To interrogate the database, use the `cw_query_database` command.
 
+### Local CAZyme database schema
+
+The schema of a local CAZyme database can be retrieved using `cazy_webscraper`:
+
+```bash
+cw_get_db_schema <path to local CAZyme database>
+```
+
+Alternatively, `sqlite3` can be used to retrieve the schema:
+```bash
+sqlite3 <path to local CAZyme database> .schema
+```
+
+A visual representation of the db schema when using `cazy_webscraper` version >= 2.3.0 can be found [here](https://hobnobmancer.github.io/cazy_webscraper/database_schema.pdf).
+
 ## Creating a local CAZyme database
 Command line options for `cazy_webscraper`, which is used to scrape CAZy and compile a local SQLite database. 
 Options are written in alphabetical order.
 
 `email` - \[REQUIRED\] User email address. This is required by NCBI Entrez for querying the Entrez server.
+**Email address is not required when printing out the citation and version number information**
 
 `--cache_dir` - Path to cache dir to be used instead of default cache dir path.
 
 `--cazy_data` - Path to a txt file downloaded from CAZy containing a CAZy db data dump.
 
 `--cazy_synonyms` - Path to a JSON file containing accepted CAZy class synonsyms if the default are not sufficient.
 
@@ -278,20 +322,24 @@
 
 `--log`, `-l` - Target path to write out a log file. If not called, no log file is written. Default: None (no log file is written out).
 
 `--nodelete`, `-n` - When called content in an existing output directory is not deleted.
 
 __When the `--db_output` flag is used, `cazy_webscraper` will create any necessary parent directories. If the direct/immediate parent directory of the database exists, by default `cazy_webscraper` will delete the content in this parent directory._
 
+`--ncbi_batch_size` - The number of protein IDs submitted per batch to NCBI, when retrieving taxonomic classifications. Default 200.
+
 `--nodelete_cache` - When called, content in the existing cache dir will **not** be deleted. Default: False (existing content is deleted).
 
 `--nodelete_log` - When called, content in the existing log dir will **not** be deleted. Default: False (existing content is deleted).
 
 `--retries`, `-r` - Define the number of times to retry making a connection to CAZy if the connection should fail. Default: 10.
 
+`--skip-ncbi_tax` - Skip retrieving the latest taxonomic information for NCBI were multiple taxonomic classifications are retrieved from CAZy for a protein. The first taxonomy retrieved from CAZy will be added to the local CAZyme database. Default False - the first taxon listed for each protein is added to the local CAZyme database.
+
 `--sql_echo` - Set SQLite engine echo parameter to True, causing SQLite to print log messages. Default: False.
 
 `--subfamilies`, `-s` - Enable retrival of CAZy subfamilies, otherwise **only** CAZy family annotations will be retrieved. Default: False.
 
 `--species` - List of species written as Genus Species) to restrict the scraping of CAZymes to. CAZymes will be retrieved for **all** strains of each given species.
 
 `--strains` - List of specific species strains to restrict the scraping of CAZymes to.
@@ -337,41 +385,33 @@
 
 `cazy_webscraper` always retrieves the UniProt accession and protein name, but the retrieval of PDB accession, EC numbers and protein sequences is optional.
 
 Data can be retrieived for all proteins in the local CAZyme database, or a specific subset. CAZy class, CAZy family, genus, species, strains, kingdom and EC number filters can be defined in order to define a dataset to retrieve protein data for.
 
 To retrieve all UniProt data for all proteins in a local CAZyme datbase, using the following command:
 ```bash
-cw_get_uniprot_data <path_to_local_CAZyme_db> <user_email> --ec --pdb --sequence
+cw_get_uniprot_data <path_to_local_CAZyme_db> --ec --pdb --sequence
 ```
 
 ### Configuring UniProt data retrieval
 
 Below are listed the command-line flags for configuring the retrieval of UniProt data.
 
 `database` - \[REQUIRED\] Path to a local CAZyme database to add UniProt data to.
 
-`email` - \[REQUIRED\] User email address. This is required by NCBI Entrez for querying the Entrez server.
-
-`--ncbi_batch_size` - Size of batch query posted to NCBI Entrez. Default 150.
-
-`--uniprot_batch_size` - Change the query batch size submitted via [`bioservices`](https://bioservices.readthedocs.io/en/master/) to UniProt to retrieve protein data. Default is 150. `bioservices` recommands queries not larger than 200 objects.
+`--bioservices_batch_size` - Change the query batch size submitted via [`bioservices`](https://bioservices.readthedocs.io/en/master/) to UniProt to retrieve protein data. Default is 1000. See the [UniProt REST API documentation](https://www.uniprot.org/help/id_mapping) for batch size limits.
 
 `--cache_dir` - Path to cache dir to be used instead of default cache dir path.
 
 `--cazy_synonyms` - Path to a JSON file containing accepted CAZy class synonsyms if the default are not sufficient.
 
 `--classes` - List of classes to retrieve UniProt data for.
 
 `--config`, `-c` - Path to a configuration YAML file. Default: None.
 
-`--delete_old_ec` - Boolean, delete EC number - Protein relationships that are no longer listed in UniProt, i.e. an EC number annotation is no longer included in UniProt but is in the local database. If set to TRUE these relationships will be DELETED from the database.
-
-`--delete_old_pdbs` - Boolean, delete PDB accessions - Protein relationships that are no longer listed in UniProt, i.e. an PDB accessions that are no longer included in UniProt but is in the local database. If set to TRUE these relationships will be DELETED from the database.
-
 `--ec`, `-e` - Enable retrieval of EC number annotations from UniProt
 
 `--ec_filter` - Limist retrieval of protein data to proteins annotated with a provided list of EC numbers. Separate the EC numbers bu single commas without spaces. Recommend to wrap the entire str in quotation marks, for example:
 ```bash
 cw_get_uniprot_data my_cazyme_db/cazyme_db.db --ec_filter 'EC1.2.3.4,EC2.3.1.-'
 ```
 
@@ -393,36 +433,60 @@
 
 `--nodelete_log` - When called, content in the existing log dir will **not** be deleted. Default: False (existing content is deleted).
 
 `--pdb`, `-p` - Enable retrieval of PDB accessions. Default, PDB accessions not retrieved.
 
 `--retries`, `-r` - Define the number of times to retry making a connection to CAZy if the connection should fail. Default: 10.
 
+`--delete_old_ec_relationships` - Boolean, delete old Genbanks-EC number relationships - For those proteins in the local db for whom data is downloaded from UniProt, compare the current links between the proteins in the Genbanks table and EC numbers in the Ecs table. Delete Genbanks-Ecs relationships that are not longer listed in the respective protein records in UniProt.
+
+`--delete_old_ecs` - Boolean, delete EC number - Delete EC numbers that are not linked to any proteins listed in the Genbanks table. These can arise from multiple retrievals of data from the UniProt data over a period of time during UniProt records have been updated.
+
+`--delete_old_pdb_relationships` - Boolean, delete old Genbanks-PDB relationships - For those proteins in the local db for whom data is downloaded from UniProt, compare the current links between the proteins in the Genbanks table and PDB accessions in the Pdbs table. Delete Genbanks-Pdbs relationships that are not longer listed in the respective protein records in UniProt.
+
+`--delete_old_pdbs` - Boolean, delete PDB accessions - Protein relationships that are no longer listed in UniProt, i.e. an PDB accessions that are no longer included in UniProt but is in the local database. If set to TRUE these relationships will be DELETED from the database.
+
 `--use_uniprot_cache` - Path to a JSON file, keyed by UniProt accessions/IDs and valued by dicts containing `{'gbk_acc': str, 'db_id': int}`. This file part of the cache created by `cw_get_uniprot_data`. This is option to skip retrieving the UniProt IDs for a set of GenBank accessions, if retrieving data for the same dataset (this save a lot of time!)
 
 `skip_download` - Bool, default False. If set to True, only uses data from UniProt cache and will not download new data from UniProt.
 
 `--sequence`, `-s` - Retrieve protein amino acid sequences from UniProt
 
-`--seq_update` - If a newer version of the protein sequence is available, overwrite the existing sequence for the protein in the database. Default is false, the protein sequence is **not** overwritten and updated.
-
 `--sql_echo` - Set SQLite engine echo parameter to True, causing SQLite to print log messages. Default: False.
 
 `--species` - List of species written as Genus Species) to restrict the scraping of CAZymes to. CAZymes will be retrieved for **all** strains of each given species.
 
 `--strains` - List of specific species strains to restrict the scraping of CAZymes to.
 
-`--timeout`, `-t` - Connection timout limit (seconds). Default: 45.
+`--taxonomy`, `-t` - Retrieve taxonomic classifications (genus species) and add to the local CAZyme database
+
+`--timeout` - Connection timout limit (seconds). Default: 45.
+
+`--update_name` - If a newer version of the protein name is available, overwrite the existing name for the protein in the database. Default is false, the protein name is **not** overwritten and updated.
+
+`--update_seq` - If a newer version of the protein sequence is available, overwrite the existing sequence for the protein in the database. Default is false, the protein sequence is **not** overwritten and updated.
 
 `--use_uniprot_cache` - Path to JSON file containing data previosuly retrieved from UniProt by `cazy_webscraper`, use if an error occurred while adding the data to the local CAZyme database. This will skip the retrieval of data from UniProt, and the cached data will be added to the local CAZyme database. This can also be shared with others to add the same data to their local CAZyme database.
 
 `--uniprot_batch_size` - Size of an individual batch query submitted to the [UniProt REST API](https://www.uniprot.org/help/programmatic_access) to retrieve the UniProt accessions of proteins identified by the GenBank accession. Default is 150. The UniProt API documentation recommands batch sizes of less than 20,000 but batch sizes of 1,000 often result in HTTP 400 errors. It is recommend to keep batch sizes less than 1,000, and ideally less than 200.
 
 `--verbose`, `-v` - Enable verbose logging. This does not set the SQLite engine `echo` parameter to True. Default: False.
 
+**UniProt batch sizes:**
+Note that according to Uniprot (June 2022), there are various limits on ID Mapping Job Submission:
+
+========= =====================================================================================
+Limit	  Details
+========= =====================================================================================
+100,000	  Total number of ids allowed in comma separated param ids in /idmapping/run api
+500,000	  Total number of "mapped to" ids allowed
+100,000	  Total number of "mapped to" ids allowed to be enriched by UniProt data
+10,000	  Total number of "mapped to" ids allowed with filtering
+========= =====================================================================================
+
 ### UniProt data retrieval cache
 
 - The tables retrieved from UniProt are converted to dataframes, and written out as CSV files in the cache directory
 - The parsed UniProt data as a single JSON file
 
 ## Retrieveing protein seqences from GenBank
 
@@ -1020,15 +1084,15 @@
 
 For configuring the retrieval of data from UniProt, GenBank and PDB (_but not CAZy) the additional `ec` tag can be included to limit the retrieval of data to proteins annotated with specific EC numbers.
 
 When listing EC numbers, the 'EC' prefix can be included or excluded. For example, 'EC1.2.3.4' and '1.2.3.4' are accepted. Additionally, both dashes ('-') and astrixes ('*') can be used to represent missing digits, both '1.2.3.-' and '1.2.3.\*' are accepted.
 
 `cazy_webscraper` performs a direct EC number comparison. Therefore, supplying `cazy_webscraper` with the EC number EC1.2.3.- will only retrieve protein specifically annotated with EC1.2.3.-. `cazy_webscraper` will **not** retrieve proteins will all completed EC numbers under EC1.2.3.-, thus, `cazy_webscraper` will **not** retrieve data for proteins annotated with EC1.2.3.1, EC1.2.3.2, EC1.2.3.3, etc.
 
-Example configuration files, and an empty configuraiton file template are located in the [`config_files`]() directory of this repo.
+Example configuration files, and an empty configuraiton file template are located in the `configuration_files/` directory of this repo.
 
 
 ## Integrating a local CAZyme database
 
 `cazy_webscraper` compiles data downloaded from external databases into a local SQLite3 database.
 
 To facilitate integratting the local CAZyme database into third-party `Python` applications, use the `get_db_connection` function from `cazy_webscraper`, which will return an open connection to the CAZyme database from `sqlalchemy`.
@@ -1041,14 +1105,20 @@
 - Bool to reflect if a new database. Default is `False`, i.e. connecting to an existing local CAZyme database
 
 Import the function into the `Python` script using:
 ```python
 from cazy_webscraper.sql.sql_orm import get_db_connection
 ```
 
+## Database Schema
+
+This is the structure of the local SQLite3 database compiled by `cazy_webscraper` version >=2.3.0:
+
+![database schema](assets/cazy_webscraper_v2.3+.svg "database schema")
+
 
 ## Contributions
 
 We welcome contributions and suggestions. You can raise issues at this repository, or fork the repository and submit pull requests, at the links below:
 
 - [Issues](https://github.com/HobnobMancer/cazy_webscraper/issues)
 - [Pull Requests](https://github.com/HobnobMancer/cazy_webscraper/pulls)
```

### Comparing `cazy_webscraper-2.2.8/README.md` & `cazy_webscraper-2.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,69 @@
+Metadata-Version: 2.1
+Name: cazy_webscraper
+Version: 2.3.0
+Summary: A tool to automate retrieving data from CAZy, build a local CAZyme SQL database, and throughly interrogating the data. Also, automate retrieving protein data, sequences, EC numbers and structure files for specific datasets in the CAZyme database from UniProt, GenBank and PDB.
+Home-page: https://github.com/HobnobMancer/cazy_webscraper
+Author: Emma E. M. Hobbs
+Author-email: eemh1@st-andrews.ac.uk
+License: MIT
+Keywords: bioinforamtics protein webscraper
+Platform: Posix
+Platform: MacOS X
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # cazy_webscraper
 
 -------------------------------
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6343936.svg)](https://doi.org/10.5281/zenodo.6343936)
 [![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazy_webscraper/blob/master/LICENSE)  
 [![CircleCI](https://circleci.com/gh/HobnobMancer/cazy_webscraper.svg?style=shield)](https://circleci.com/gh/HobnobMancer/cazy_webscraper)
 [![codecov](https://codecov.io/gh/HobnobMancer/cazy_webscraper/branch/master/graph/badge.svg)](https://codecov.io/gh/HobnobMancer/cazy_webscraper)
 [![Documentation Status](https://readthedocs.org/projects/cazy-webscraper/badge/?version=latest)](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest)  
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/version.svg)](https://anaconda.org/bioconda/cazy_webscraper)
 [![Anaconda-Update Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/latest_release_date.svg)](https://anaconda.org/bioconda/cazy_webscraper)  
 [![pyani PyPi version](https://img.shields.io/pypi/v/cazy_webscraper "PyPI version")](https://pypi.python.org/pypi/cazy_webscraper)  
 [![Downloads](https://pepy.tech/badge/cazy-webscraper)](https://pepy.tech/project/cazy-webscraper)
 
--------------------------------
-
-> `cazy_webscraper` version 1 is depracted. Please ensure you are using version 2 or newer.  
-> `bioconda` installation is fixed for >= v2.1.3.1
+--------------------------------
 
 ## cazy_webscraper
 
 `cazy_webscraper` is an application and Python3 package for the automated retrieval of protein data from the [CAZy](http://wwww.cazy.org/) database. The code is distributed under the MIT license.
+The full documentation can be found at [Read the Docs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
 
 **`cazy_webscraper` retrieves protein data from the [CAZy database](https://www.cazy.org) and stores the data in a local SQLite3 database.** This enables users to integrate the dataset into analytical pipelines, and interrogate the data in a manner unachievable through the CAZy website.
 
 **Data can be retrieved for user defined datasets of interest.** `cazy_webscraper` can recover specified CAZy Classes and/or CAZy families. These queries can be filtered by taxonomy at Kingdoms, genus, species or strain level. Successive CAZy queries can be collated into a single local database. A log of each query is recorded in the database for transparency, reproducibility and shareablity.
 
 **Using the `expand` subcommand, a user can expand the core dataset.** Specifically, `cazy_webscraper` can be used to retrieve data from the following external databases for CAZymes in the local CAZyme database that meet user specified criteria, and adds the downloaded data to the local CAZyme database:
 
 **[GenBank](https://www.ncbi.nlm.nih.gov/genbank/):**  
 - Protein sequences 
 - Latest taxonomic classification - including complete lineage (including phylum, class, order and family) (version >=2.1.2)
 - Latest genomic assembly data (GenBank and RefSeq (when available) version accession and ID numbers) (version >=2.1.3)
 
-**[UniProt](https://www.uniprot.org/):**  
+**[UniProt](https://www.uniprot.org/):** 
+- UniProt ID/accession
 - Protein name
-- UniProt accession
 - EC numbers
 - PDB accessions
-- Protein sequences
+- Protein sequence (and date sequence was last updated)
+- Taxonomic classification (genus and species)
 
 **[Research Collaboratory for Structural Bioinformatics (RCSB) Protein Data Bank (PDB)](https://www.rcsb.org/):**
 - Protein structure files
 - *Structure files are written to disk, **not** stored in the local CAZyme database*
 
 **[Genome Taxonomy Database (GTDB)](https://gtdb.ecogenomic.org/):**
 Retrieve the latest archaeal and bacterial taxonomic classifications (including complete lineages from kingdom to species) - available in `cazy_webscraper` verion >= 2.2.0.
@@ -53,20 +75,64 @@
 - A FASTA file per extracted protein sequence
 - A local BLASTP database
 
 **The `cazy_webscraper` API facilitates interoggating the local CAZyme database.**
 
 Please see the [full documentation at ReadTheDocs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
 
+## Updates
+
+**New in version 2.3.0**
+* Downloading protein data from UniProt is several magnitudes faster than before - and should have fewer issues with using older version of `bioservices`
+    - Uses `bioservices` mapping to map directly from NCBI protein version accession to UniProt
+    - `cw_get_uniprot_data` not longer calls to NCBI and thus no longer requires an email address as a positional argument
+* Updated database schema: Changed `Genbanks 1--* Uniprots` to `Genbanks *--1 Uniprots`. `Uniprots.uniprot_id` is now listed in the `Genbanks` table, instead of listing `Genbanks.genbank_id` in the `Uniprots` table
+
+* Retrieve taxonomic classifications from UniProt
+    * Use the `--taxonomy`/`-t` flag to retrieve the scientific name (genus and species) for proteins of interest
+    * Adds downloaded taxonomic information to the `UniprotsTaxs` table
+
+* Improved clarrification of deleting old records when using `cw_get_uniprot_data`
+    - Separate arguments to delete Genbanks-EC number and Genbanks-PDB accession relationships that are no longer listed in UniProt for those proteins in the local CAZyme database for proteins whom data is downloaded from UniProt
+    - New args:
+        - `--delete_old_ec_relationships` = deletes Genbank(protein)-EC number relationships no longer in UniProt
+        - `--delete_old_ecs` = deletes EC numbers in the local db not linked to any proteins
+        - `--delete_old_pdb_relationships` = deletes Genbank(protein)-PDB relationships no longer in UniProt
+        - `--delete_old_pdbs` = deletes PDB accessions in the local db not linked to any proteins
+
+* Retrieve the local db schema
+    - New command `cw_get_db_schema` added.
+    - Retrieves the SQLite schema of a local CAZyme database and prints it to the terminal
+
+* Added option to skip retrieving the latest taxonomic classifications NCBI taxonomies
+    - By default, when retreiving data from CAZy, `cazy_webscraper` retrieves the latest taxonomic classifications for proteins listed under multiple tax
+    - To increase scrapping time, and to reduce burden on the NCBI-Entrez server, if this data is not needed (e.g. GTDB taxs will be use) this step can be skipped by using the new `--skip_ncbi_tax` flag.
+    - When skipping retrieval of the latest taxa classifications from NCBI, `cazy_webscraper` will add the first taxa retrieved from CAZy for those proteins listed under mutliple taxa
+
+
 ## Documentation
 
+The full documentation can be found at [Read the Docs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
+
+### Our paper: Implementation and demonstration of use
+
 For a full description of the operation and examples of use, please see our paper in (BioRxiv)[https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full].
 
 > Hobbs, E. E. M., Gloster, T. M., and Pritchard, L. (2022) 'cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets', _bioRxiv_, [https://doi.org/10.1101/2022.12.02.518825](https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full)
 
+### Database structure
+
+You can view the database schema [here](#database-schema) and find a PDF of the database schema [here](https://hobnobmancer.github.io/cazy_webscraper/database_schema.pdf).
+
+## Contributions
+
+We welcome contributions and suggestions. You can raise issues at this repository, or fork the repository and submit pull requests, at the links below:
+
+- [Issues](https://github.com/HobnobMancer/cazy_webscraper/issues)
+- [Pull Requests](https://github.com/HobnobMancer/cazy_webscraper/pulls)
 
 ## Table of Contents
 <!-- TOC -->
 - [`cazy_webscraper`](#cazy_webscraper)
 - [Citation](#citation)
 - [Best practice](#best-practice)
 - [Documentation](#documentation)
@@ -91,24 +157,24 @@
 - [Retrieving GTDB taxonomies](#retrieving-gtdb-taxonomies)
     - [Configuring retrieving GTDB taxonomies](#configuring-retrieving-gtdb-taxonomies)
 - [The `cazy_webscraper` API or Interrogating the local CAZyme database](#the_cazy_webscraper_api_or_interrogating_the_local_cazyme_database)
 - [Configuring `cazy_webscraper` using a YAML file](#configuring-using-a-yaml-file)
 - [CAZy coverage of GenBank](#cazy-coverage-of-genbank)
     - [Configure calculating CAZy coverage of GenBank](#configure-calculating-cazy-coverage-of-genbank)
 - [Integrating a local CAZyme database](#integrating-a-local-cazyme-database)
+- [Database schema](#database-schema)
 - [Contributions](#contributions)
 - [License and copyright](#license-and-copyright)
 <!-- /TOC -->
 
 
 ## Features in the pipeline:
 - Retrieve and stored PubMed IDs in the local CAZyme database
 - Fix any remaining bugs we can find (if you find a bug, please report it and provide as detailed bug report as possible!)
-- Update the unit tests to work with the new `cazy_webscraper` architecture
-- Update the documentation
+- Increase unit test coverage
 - Automate analysing the taxonomic distribution across CAZy and datasets of interest, including generating a final report
 
 ## Citation
 
 If you use `cazy_webscraper`, please cite the following publication:
 
 > Hobbs, E. E. M., Gloster, T. M., and Pritchard, L. (2022) 'cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets', _bioRxiv_, [https://doi.org/10.1101/2022.12.02.518825](https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1)
@@ -167,21 +233,29 @@
 ```
 
 ### Version and citation
 
 To retrieve the version, use the following command:
 
 ```bash
-cazy_webscraper <user_email> -V
+cazy_webscraper -V
+```
+or
+```bash
+cazy_webscraper --version
 ```
 
 To retrieve the citation to use:
 
 ```bash
-cazy_webscraper <user_email> -C
+cazy_webscraper -C
+```
+or
+```bash
+cazy_webscraper --citation
 ```
 
 ### Command summary
 
 Below are the list of commands (excluding required and optional arguments) included in `cazy_webscraper`.
 
 #### CAZy
@@ -213,19 +287,35 @@
 
 **Note:** PDB structure files are retrieved for the PDB accessions that are *in* a local CAZyme database created using `cazy_webscraper`. A freshly built CAZyme database only contains NCBI protein accessions, taxonomic kingdoms, source organisms, and CAZy family annotations. Therefore, the `cw_get_uniprot_data` command must be used to retrieve PDB accessions from the UniProt database **prior** to using the `cw_get_pdb_structures` command.
 
 #### Interrogate the database
 
 To interrogate the database, use the `cw_query_database` command.
 
+### Local CAZyme database schema
+
+The schema of a local CAZyme database can be retrieved using `cazy_webscraper`:
+
+```bash
+cw_get_db_schema <path to local CAZyme database>
+```
+
+Alternatively, `sqlite3` can be used to retrieve the schema:
+```bash
+sqlite3 <path to local CAZyme database> .schema
+```
+
+A visual representation of the db schema when using `cazy_webscraper` version >= 2.3.0 can be found [here](https://hobnobmancer.github.io/cazy_webscraper/database_schema.pdf).
+
 ## Creating a local CAZyme database
 Command line options for `cazy_webscraper`, which is used to scrape CAZy and compile a local SQLite database. 
 Options are written in alphabetical order.
 
 `email` - \[REQUIRED\] User email address. This is required by NCBI Entrez for querying the Entrez server.
+**Email address is not required when printing out the citation and version number information**
 
 `--cache_dir` - Path to cache dir to be used instead of default cache dir path.
 
 `--cazy_data` - Path to a txt file downloaded from CAZy containing a CAZy db data dump.
 
 `--cazy_synonyms` - Path to a JSON file containing accepted CAZy class synonsyms if the default are not sufficient.
 
@@ -255,20 +345,24 @@
 
 `--log`, `-l` - Target path to write out a log file. If not called, no log file is written. Default: None (no log file is written out).
 
 `--nodelete`, `-n` - When called content in an existing output directory is not deleted.
 
 __When the `--db_output` flag is used, `cazy_webscraper` will create any necessary parent directories. If the direct/immediate parent directory of the database exists, by default `cazy_webscraper` will delete the content in this parent directory._
 
+`--ncbi_batch_size` - The number of protein IDs submitted per batch to NCBI, when retrieving taxonomic classifications. Default 200.
+
 `--nodelete_cache` - When called, content in the existing cache dir will **not** be deleted. Default: False (existing content is deleted).
 
 `--nodelete_log` - When called, content in the existing log dir will **not** be deleted. Default: False (existing content is deleted).
 
 `--retries`, `-r` - Define the number of times to retry making a connection to CAZy if the connection should fail. Default: 10.
 
+`--skip-ncbi_tax` - Skip retrieving the latest taxonomic information for NCBI were multiple taxonomic classifications are retrieved from CAZy for a protein. The first taxonomy retrieved from CAZy will be added to the local CAZyme database. Default False - the first taxon listed for each protein is added to the local CAZyme database.
+
 `--sql_echo` - Set SQLite engine echo parameter to True, causing SQLite to print log messages. Default: False.
 
 `--subfamilies`, `-s` - Enable retrival of CAZy subfamilies, otherwise **only** CAZy family annotations will be retrieved. Default: False.
 
 `--species` - List of species written as Genus Species) to restrict the scraping of CAZymes to. CAZymes will be retrieved for **all** strains of each given species.
 
 `--strains` - List of specific species strains to restrict the scraping of CAZymes to.
@@ -314,41 +408,33 @@
 
 `cazy_webscraper` always retrieves the UniProt accession and protein name, but the retrieval of PDB accession, EC numbers and protein sequences is optional.
 
 Data can be retrieived for all proteins in the local CAZyme database, or a specific subset. CAZy class, CAZy family, genus, species, strains, kingdom and EC number filters can be defined in order to define a dataset to retrieve protein data for.
 
 To retrieve all UniProt data for all proteins in a local CAZyme datbase, using the following command:
 ```bash
-cw_get_uniprot_data <path_to_local_CAZyme_db> <user_email> --ec --pdb --sequence
+cw_get_uniprot_data <path_to_local_CAZyme_db> --ec --pdb --sequence
 ```
 
 ### Configuring UniProt data retrieval
 
 Below are listed the command-line flags for configuring the retrieval of UniProt data.
 
 `database` - \[REQUIRED\] Path to a local CAZyme database to add UniProt data to.
 
-`email` - \[REQUIRED\] User email address. This is required by NCBI Entrez for querying the Entrez server.
-
-`--ncbi_batch_size` - Size of batch query posted to NCBI Entrez. Default 150.
-
-`--uniprot_batch_size` - Change the query batch size submitted via [`bioservices`](https://bioservices.readthedocs.io/en/master/) to UniProt to retrieve protein data. Default is 150. `bioservices` recommands queries not larger than 200 objects.
+`--bioservices_batch_size` - Change the query batch size submitted via [`bioservices`](https://bioservices.readthedocs.io/en/master/) to UniProt to retrieve protein data. Default is 1000. See the [UniProt REST API documentation](https://www.uniprot.org/help/id_mapping) for batch size limits.
 
 `--cache_dir` - Path to cache dir to be used instead of default cache dir path.
 
 `--cazy_synonyms` - Path to a JSON file containing accepted CAZy class synonsyms if the default are not sufficient.
 
 `--classes` - List of classes to retrieve UniProt data for.
 
 `--config`, `-c` - Path to a configuration YAML file. Default: None.
 
-`--delete_old_ec` - Boolean, delete EC number - Protein relationships that are no longer listed in UniProt, i.e. an EC number annotation is no longer included in UniProt but is in the local database. If set to TRUE these relationships will be DELETED from the database.
-
-`--delete_old_pdbs` - Boolean, delete PDB accessions - Protein relationships that are no longer listed in UniProt, i.e. an PDB accessions that are no longer included in UniProt but is in the local database. If set to TRUE these relationships will be DELETED from the database.
-
 `--ec`, `-e` - Enable retrieval of EC number annotations from UniProt
 
 `--ec_filter` - Limist retrieval of protein data to proteins annotated with a provided list of EC numbers. Separate the EC numbers bu single commas without spaces. Recommend to wrap the entire str in quotation marks, for example:
 ```bash
 cw_get_uniprot_data my_cazyme_db/cazyme_db.db --ec_filter 'EC1.2.3.4,EC2.3.1.-'
 ```
 
@@ -370,36 +456,60 @@
 
 `--nodelete_log` - When called, content in the existing log dir will **not** be deleted. Default: False (existing content is deleted).
 
 `--pdb`, `-p` - Enable retrieval of PDB accessions. Default, PDB accessions not retrieved.
 
 `--retries`, `-r` - Define the number of times to retry making a connection to CAZy if the connection should fail. Default: 10.
 
+`--delete_old_ec_relationships` - Boolean, delete old Genbanks-EC number relationships - For those proteins in the local db for whom data is downloaded from UniProt, compare the current links between the proteins in the Genbanks table and EC numbers in the Ecs table. Delete Genbanks-Ecs relationships that are not longer listed in the respective protein records in UniProt.
+
+`--delete_old_ecs` - Boolean, delete EC number - Delete EC numbers that are not linked to any proteins listed in the Genbanks table. These can arise from multiple retrievals of data from the UniProt data over a period of time during UniProt records have been updated.
+
+`--delete_old_pdb_relationships` - Boolean, delete old Genbanks-PDB relationships - For those proteins in the local db for whom data is downloaded from UniProt, compare the current links between the proteins in the Genbanks table and PDB accessions in the Pdbs table. Delete Genbanks-Pdbs relationships that are not longer listed in the respective protein records in UniProt.
+
+`--delete_old_pdbs` - Boolean, delete PDB accessions - Protein relationships that are no longer listed in UniProt, i.e. an PDB accessions that are no longer included in UniProt but is in the local database. If set to TRUE these relationships will be DELETED from the database.
+
 `--use_uniprot_cache` - Path to a JSON file, keyed by UniProt accessions/IDs and valued by dicts containing `{'gbk_acc': str, 'db_id': int}`. This file part of the cache created by `cw_get_uniprot_data`. This is option to skip retrieving the UniProt IDs for a set of GenBank accessions, if retrieving data for the same dataset (this save a lot of time!)
 
 `skip_download` - Bool, default False. If set to True, only uses data from UniProt cache and will not download new data from UniProt.
 
 `--sequence`, `-s` - Retrieve protein amino acid sequences from UniProt
 
-`--seq_update` - If a newer version of the protein sequence is available, overwrite the existing sequence for the protein in the database. Default is false, the protein sequence is **not** overwritten and updated.
-
 `--sql_echo` - Set SQLite engine echo parameter to True, causing SQLite to print log messages. Default: False.
 
 `--species` - List of species written as Genus Species) to restrict the scraping of CAZymes to. CAZymes will be retrieved for **all** strains of each given species.
 
 `--strains` - List of specific species strains to restrict the scraping of CAZymes to.
 
-`--timeout`, `-t` - Connection timout limit (seconds). Default: 45.
+`--taxonomy`, `-t` - Retrieve taxonomic classifications (genus species) and add to the local CAZyme database
+
+`--timeout` - Connection timout limit (seconds). Default: 45.
+
+`--update_name` - If a newer version of the protein name is available, overwrite the existing name for the protein in the database. Default is false, the protein name is **not** overwritten and updated.
+
+`--update_seq` - If a newer version of the protein sequence is available, overwrite the existing sequence for the protein in the database. Default is false, the protein sequence is **not** overwritten and updated.
 
 `--use_uniprot_cache` - Path to JSON file containing data previosuly retrieved from UniProt by `cazy_webscraper`, use if an error occurred while adding the data to the local CAZyme database. This will skip the retrieval of data from UniProt, and the cached data will be added to the local CAZyme database. This can also be shared with others to add the same data to their local CAZyme database.
 
 `--uniprot_batch_size` - Size of an individual batch query submitted to the [UniProt REST API](https://www.uniprot.org/help/programmatic_access) to retrieve the UniProt accessions of proteins identified by the GenBank accession. Default is 150. The UniProt API documentation recommands batch sizes of less than 20,000 but batch sizes of 1,000 often result in HTTP 400 errors. It is recommend to keep batch sizes less than 1,000, and ideally less than 200.
 
 `--verbose`, `-v` - Enable verbose logging. This does not set the SQLite engine `echo` parameter to True. Default: False.
 
+**UniProt batch sizes:**
+Note that according to Uniprot (June 2022), there are various limits on ID Mapping Job Submission:
+
+========= =====================================================================================
+Limit	  Details
+========= =====================================================================================
+100,000	  Total number of ids allowed in comma separated param ids in /idmapping/run api
+500,000	  Total number of "mapped to" ids allowed
+100,000	  Total number of "mapped to" ids allowed to be enriched by UniProt data
+10,000	  Total number of "mapped to" ids allowed with filtering
+========= =====================================================================================
+
 ### UniProt data retrieval cache
 
 - The tables retrieved from UniProt are converted to dataframes, and written out as CSV files in the cache directory
 - The parsed UniProt data as a single JSON file
 
 ## Retrieveing protein seqences from GenBank
 
@@ -997,15 +1107,15 @@
 
 For configuring the retrieval of data from UniProt, GenBank and PDB (_but not CAZy) the additional `ec` tag can be included to limit the retrieval of data to proteins annotated with specific EC numbers.
 
 When listing EC numbers, the 'EC' prefix can be included or excluded. For example, 'EC1.2.3.4' and '1.2.3.4' are accepted. Additionally, both dashes ('-') and astrixes ('*') can be used to represent missing digits, both '1.2.3.-' and '1.2.3.\*' are accepted.
 
 `cazy_webscraper` performs a direct EC number comparison. Therefore, supplying `cazy_webscraper` with the EC number EC1.2.3.- will only retrieve protein specifically annotated with EC1.2.3.-. `cazy_webscraper` will **not** retrieve proteins will all completed EC numbers under EC1.2.3.-, thus, `cazy_webscraper` will **not** retrieve data for proteins annotated with EC1.2.3.1, EC1.2.3.2, EC1.2.3.3, etc.
 
-Example configuration files, and an empty configuraiton file template are located in the [`config_files`]() directory of this repo.
+Example configuration files, and an empty configuraiton file template are located in the `configuration_files/` directory of this repo.
 
 
 ## Integrating a local CAZyme database
 
 `cazy_webscraper` compiles data downloaded from external databases into a local SQLite3 database.
 
 To facilitate integratting the local CAZyme database into third-party `Python` applications, use the `get_db_connection` function from `cazy_webscraper`, which will return an open connection to the CAZyme database from `sqlalchemy`.
@@ -1018,14 +1128,20 @@
 - Bool to reflect if a new database. Default is `False`, i.e. connecting to an existing local CAZyme database
 
 Import the function into the `Python` script using:
 ```python
 from cazy_webscraper.sql.sql_orm import get_db_connection
 ```
 
+## Database Schema
+
+This is the structure of the local SQLite3 database compiled by `cazy_webscraper` version >=2.3.0:
+
+![database schema](assets/cazy_webscraper_v2.3+.svg "database schema")
+
 
 ## Contributions
 
 We welcome contributions and suggestions. You can raise issues at this repository, or fork the repository and submit pull requests, at the links below:
 
 - [Issues](https://github.com/HobnobMancer/cazy_webscraper/issues)
 - [Pull Requests](https://github.com/HobnobMancer/cazy_webscraper/pulls)
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,25 +40,37 @@
 """Web scraper to scrape the CAZy website."""
 
 
 import logging
 import os
 import sys
 
+import numpy as np
 import pandas as pd
 
 from datetime import datetime
 from pathlib import Path
 
+import Bio
+import bioservices
+import bs4
+import html5lib
+import lxml
+import mechanicalsoup
+import requests
+import saintBioutils
+import sqlalchemy
+import tqdm
+
 from saintBioutils.utilities.file_io import make_output_directory
 
 from cazy_webscraper.sql import sql_orm
 
 
-__version__ = "2.2.8"
+__version__ = "2.3.0"
 
 
 VERSION_INFO = f"cazy_webscraper version: {__version__}"
 
 
 CITATION_INFO = (
     "If you use cazy_webscraper in your work, please cite the following publication:\n"
@@ -130,15 +142,15 @@
     """Display citation inforamtion.
 
     Return nothing
     """
 
     message = f"""
     =====================cazy_webscraper Citation Information=====================
-    Version: {VERSION_INFO}
+    cazy_webscraper version: {VERSION_INFO}
 
     When publishing work that uses cazy_webscraper please cite:
     Citation: {CITATION_INFO}
 
     cazy_webscraper depends on a number of tools. To recognise the contributions that the 
     authors and developers have made, please also cite the following:
 
@@ -174,17 +186,36 @@
 
     print(message)
 
 
 def display_version_info():
     """Display package version number information"""
 
-    message = f""""
+    try:
+        saintbio_version = saintBioutils.__version__
+    except AttributeError:
+        saintbio_version = 'unknown'
+
+    message = f"""
     =====================cazy_webscraper Version Information=====================
-    Version: {VERSION_INFO}
+    cazy_webscraper version: {VERSION_INFO}
+
+    Third party tools used by cazy_webscraper:
+    beautifulsoup4: {bs4.__version__}
+    biopython: {Bio.__version__}
+    bioservices: {bioservices.version}
+    html5lib: {html5lib.__version__}
+    lxml: {lxml.__version__}
+    mechanicalsoup: {mechanicalsoup.__version__}
+    numpy: {np.__version__}
+    pandas: {pd.__version__}
+    requests: {requests.__version__}
+    saintBioutils: {saintbio_version}
+    sqlalchemy: {sqlalchemy.__version__}
+    tqdm: {tqdm.__version__}
     """
 
     print(message)
 
 
 def connect_existing_db(args, time_stamp, start_time):
     """Coordinate connecting to an existing local CAZyme database, define logger name and cache dir
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/api/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/api/cw_query_database.py` & `cazy_webscraper-2.3.0/cazy_webscraper/api/cw_query_database.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/cazy/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/cazy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,28 +40,28 @@
 """Parse data retrieved from CAZy and build a dict of data matching the user's criteria."""
 
 
 import logging
 import re
 import sys
 
+from collections import namedtuple
+
 from tqdm import tqdm
 from zipfile import ZipFile
 
 from cazy_webscraper import crawler
 from cazy_webscraper.crawler import get_cazy_file
 
 
 def get_cazy_txt_file_data(cache_dir, time_stamp, args):
     """Retrieve txt file of CAZy db dump from CAZy or the local disk.
-
     :param cache_dir: Path(), path to directory where cache is written to
     :param time_stamp: str, date and time cazy_webscraper was intiated
     :param args: cmd-line args parser
-
     Return list of lines from CAZy txt file, one line is one item in the list"""
     logger = logging.getLogger(__name__)
 
     if args.cazy_data is not None:   # retrieve lines from predownloaded CAZy txt file
         with open(args.cazy_data, 'r') as fh:
             cazy_txt_lines = fh.read().splitlines()
 
@@ -96,22 +96,23 @@
 
             with zip_handle.open(cazy_filepath) as fh:
                 cazy_txt_lines = fh.read().splitlines()
 
     return cazy_txt_lines
 
 
-def parse_all_cazy_data(lines, cazy_fam_populations):
+def parse_all_cazy_data(lines, cazy_fam_populations, args):
     """Extract ALL GenBank accession, taxonomy data and CAZy (sub)family annotations from CAZy txt file.
     
     This is when no filters are applied.
     
     :param lines: list of str, lines from CAZy txt file, one unqiue line is one item in the list
     :param cazy_fam_populations: None if args.validate is False, or dict of CAZy listed CAZy 
         (sub)fam population sizes if args.validate is True
+    :param args: CLI args parser
     
     Return cazy_data: dict, {gbk: {"organism": set(str), "families": {'fam': set (subfam)}}}
     """
 
     logger = logging.getLogger(__name__)
 
     # define dicts CAZy data will be stored in
@@ -130,18 +131,21 @@
             line_str = line   # used when parsing local CAZy file
         line_data = line_str.split('\t')
         
         gbk_accession = line_data[3]
 
         # retrieve CAZyme data
         cazy_fam = line_data[0]
-        if cazy_fam.find("_") != -1:
-            cazy_subfam = cazy_fam
-            cazy_fam = cazy_fam[:cazy_fam.find("_")]
-        else:
+        if cazy_fam.find("_") != -1: # is subfamily annotation present
+            if args.subfamilies:  # retrieve subfamily annotation if present
+                cazy_subfam = cazy_fam
+                cazy_fam = cazy_fam[:cazy_fam.find("_")]
+            else:  # no retrieving subfam annotations
+                cazy_subfam = None
+        else: # no sub fam annotation present
             cazy_subfam = None
         
         fam_annotations.add( (cazy_fam, cazy_subfam) )
        
         kingdom = line_data[1]
         kingdoms.add(kingdom)
         
@@ -170,24 +174,26 @@
 def parse_cazy_data_with_filters(
     lines,
     class_filter,
     fam_filter,
     kingdom_filter,
     tax_filter,
     cazy_fam_populations,
+    args,
 ):
     """Extract GenBank accession, taxonomy data and CAZy (sub)family annotations from CAZy txt file.
     
     :param lines: list of str, lines from CAZy txt file, one unqiue line is one item in the list
     :param class_filter: set of CAZy class to scrape
     :param fam_filter: set of CAZy families to scrape
     :param kingdom_filter: set of tax Kingdoms to limit scrape to
     :param tax_filter: set of tax (genus, species, strains) filters to limit scrape to
     :param cazy_fam_populations: None if args.validate is False, or dict of CAZy listed CAZy 
         (sub)fam population sizes if args.validate is True
+    :param args: CLI args parser
     
     Return cazy_data: dict, {gbk: {"organism": set(str), "families": {'fam': set (subfam)}}}
     """
 
     logger = logging.getLogger(__name__)
 
     # define dicts CAZy data will be stored in
@@ -212,18 +218,21 @@
         
         kingdom = line_data[1]
         organism = line_data[2]
         gbk_accession = line_data[3]
 
         # retrieve CAZyme data
         cazy_fam = line_data[0]
-        if cazy_fam.find("_") != -1:
-            cazy_subfam = cazy_fam
-            cazy_fam = cazy_fam[:cazy_fam.find("_")]
-        else:
+        if cazy_fam.find("_") != -1: # is subfamily annotation present
+            if args.subfamilies:  # retrieve subfamily annotation if present
+                cazy_subfam = cazy_fam
+                cazy_fam = cazy_fam[:cazy_fam.find("_")]
+            else:  # no retrieving subfam annotations
+                cazy_subfam = None
+        else: # no sub fam annotation present
             cazy_subfam = None
             
         # check if protein previously matched filter criteria, and additional CAZy (sub)fam annotations
         # are to be added to the db
         if gbk_accession in gbks_to_scrape:
             cazy_data, stored_gbk_accession = apply_kingdom_tax_filters(
                 cazy_data,
@@ -330,15 +339,14 @@
     :param cazy_data: dict of proteins to add to the local CAZyme database
     :param kingdom_filter: set of kingdoms to limit the addition of proteins to the db to
     :param tax_filter: set of genus, species and strains to limit the addition of protein to the db to
     :param gbk_accession: str, the GenBank accession of the protein
     :param cazy_fam: str, CAZy family annotation
     :param cazy_subfam: str, CAZy subfamily annotation, or None if protein is not a CAZy subfamily
     :param kingdom: str, taxonomy kingdom of the source organism of the protein
-
     Return
     - cazy_data ({gbk_acc: {kingdom: str, organism: str, families: {(fam, subfam, )}}})
     - boolean if data for the given protein was (True) or was not (False) added to the db
     """
     stored_gbk_accession = False
     
     if (len(kingdom_filter) == 0) and (len(tax_filter) == 0):  # kingdom and tax filters NOT enabled
@@ -384,30 +392,33 @@
     :param cazy_fam: str, name of the CAZy family
     :param cazy_subfam: str, name of the CAZy subfamily or None if not in a subfamily
     :param organism: str, scientific name of the source organism
     :param kingdom: str, taxonomy kingdom of the source organism of the protein
 
     Return dict of CAZy data
     """
+    TaxData = namedtuple('Tax', ['kingdom', 'organism'])
+    tax = TaxData(kingdom, organism)
+
     try:
         cazy_data[gbk_accession]
-        cazy_data[gbk_accession]["kingdom"].add(kingdom)
-        cazy_data[gbk_accession]["organism"].add(organism)
-        
+
+        cazy_data[gbk_accession]['taxonomy'].add(tax)
+
         try:
             cazy_data[gbk_accession]["families"][cazy_fam].add(cazy_subfam)
         except KeyError:
             cazy_data[gbk_accession]["families"][cazy_fam] = {cazy_subfam}
-        
+
     except KeyError:
         cazy_data[gbk_accession] = {
-            "kingdom": {kingdom},
-            "organism": {organism},
+            "taxonomy": {tax},
             "families": {cazy_fam: {cazy_subfam}},
         }
+        return cazy_data
     
     return cazy_data
 
 
 def validate_data_retrieval(cazy_data, cazy_fam_populations):
     """Extract GenBank accession, taxonomy data and CAZy (sub)family annotations from CAZy txt file.
 
@@ -498,19 +509,40 @@
 def build_taxa_dict(cazy_data):
     """Createa a dict of taxa data extracted from the CAZy plain text file.
     
     :param cazy_dict: dict of CAZy data
     
     Return taxa_dict, dict of taxonomy data {kingdom: set(organism)}
     """
+    logger = logging.getLogger(__name__)
+
+    cazy_data = add_tax_keys(cazy_data)
+
     taxa_dict = {}  # {kingdom: {organism,}}
     
     for genbank_accession in tqdm(cazy_data, "Compiling taxa data"):
-        kingdom = list(cazy_data[genbank_accession]['kingdom'])[0]
-        organism = list(cazy_data[genbank_accession]['organism'])[0]
+        kingdom = cazy_data[genbank_accession]['kingdom']
+        organism = cazy_data[genbank_accession]['organism']
         
         try:
             taxa_dict[kingdom].add(organism)
         except KeyError:
             taxa_dict[kingdom] = {organism}
+
+    return taxa_dict, cazy_data
+
+
+def add_tax_keys(cazy_data):
+    """Add kingdom and organism tax keys to proteins missing them in cazy_data
+
+    :param cazy_data: dict of data from CAZy
+
+    Return cazy_data
+    """
+    for gbk_acc in cazy_data:
+        try:
+            cazy_data[gbk_acc]['kingdom']
+        except KeyError:
+            cazy_data[gbk_acc]['kingdom'] = list(cazy_data[gbk_acc]['taxonomy'])[0].kingdom
+            cazy_data[gbk_acc]['organism'] = list(cazy_data[gbk_acc]['taxonomy'])[0].organism
     
-    return taxa_dict
+    return cazy_data
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/cazy_scraper.py` & `cazy_webscraper-2.3.0/cazy_webscraper/cazy_scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,19 +63,21 @@
 :cmd_args --timeout: specify the maximum time (in seconds) before determining connection timed out
 :cmd_args --validate: retrieve CAZy fam population sizes and check against
 :cmd_args --verbose: change logger level from warning to info, verbose logging
 :cmd_args --version: print version info
 """
 
 
+import logging
+import json
+import os
+
 from datetime import datetime
 from typing import List, Optional
 
-import logging
-import os
 import pandas as pd
 
 from Bio import Entrez
 from saintBioutils.utilities.file_io import make_output_directory
 from saintBioutils.utilities.logger import config_logger, build_logger
 
 from cazy_webscraper import (
@@ -83,14 +85,15 @@
     VERSION_INFO,
     closing_message,
     connect_to_new_db,
     connect_existing_db,
     display_citation_info,
     display_version_info,
 )
+from cazy_webscraper.cache.cazy import cache_cazy_data
 from cazy_webscraper.crawler.get_validation_data import get_validation_data
 from cazy_webscraper.cazy import (
     build_taxa_dict,
     get_cazy_txt_file_data,
     parse_all_cazy_data,
     parse_cazy_data_with_filters,
 )
@@ -132,14 +135,24 @@
         display_version_info()
         return
 
     if args.citation:
         display_citation_info()
         return
 
+    if args.email is None:
+        logger.error(
+            "No email address provided.\n"
+            "Email address required by NCBI - which is required to retrieve the latest taxonomic\n"
+            "classifications for proteins listed with multiple source organisms in the CAZy database\n"
+            "Please provide your email address.\n"
+            "Terminating program."
+        )
+        return
+
     # check correct output was provided, exit if not operable
     if args.database is not None and args.db_output is not None:
         warning_message = (
             "Target path for a NEW database (--db_output, -d) and\n"
             "a path to an EXISTING database (--database, -D) were provided.\n"
             "Please provide one OR the other.\n"
             "Terminating program."
@@ -162,14 +175,23 @@
                 "Force is False\n"
                 "Not ovewriting existing database\n"
                 "Termianting program"
             )
             closing_message("cazy_webscraper", start_time, args, early_term=True)
             return
 
+    if args.skip_ncbi_tax:
+        logger.warning(
+            "skip_ncbi_tax is True - not retrieving the latest taxa from NCBI for proteins with multipe tax. Will use the first taxa listed in CAZy\n"
+            "The latest taxonomic data can be retrieved using any of the three options:\n"
+            "(i) cw_get_ncbi_taxs\n"
+            "(ii) cw_get_genomics + cw_get_gtdb_taxs\n"
+            "(iii) cw_get_uniprot_data with --taxonomy/-t"
+        )
+
     Entrez.email = args.email
 
     logger.info("Parsing configuration")
     (
         excluded_classes,
         config_dict,
         cazy_class_synonym_dict,
@@ -326,24 +348,25 @@
 
     logger.info(f"Retrieved {len(cazy_txt_lines)} lines from the CAZy db txt file")
 
     if (len(class_filters) == 0) and \
         (len(fam_filters) == 0) and \
             (len(kingdom_filters) == 0) and \
                 (len(taxonomy_filters) == 0):
-        cazy_data = parse_all_cazy_data(cazy_txt_lines, cazy_fam_populations)
+        cazy_data = parse_all_cazy_data(cazy_txt_lines, cazy_fam_populations, args)
 
     else:
         cazy_data = parse_cazy_data_with_filters(
             cazy_txt_lines,
             class_filters,
             fam_filters,
             kingdom_filters,
             taxonomy_filters,
             cazy_fam_populations,
+            args,
         )
 
     logger.info(
         f"Retrieved {len((list(cazy_data.keys())))} proteins from the CAZy txt file "
         "matching the scraping criteria"
     )
 
@@ -356,15 +379,19 @@
             cazy_data,
             multiple_taxa_gbks,
             replaced_taxa_logger,
             args,
             invalid_ids=False,
         )
 
-    taxa_dict = build_taxa_dict(cazy_data)  # {kingdom: {organisms}}
+    # add separate kingdom and organism keys to cazy_data for all proteins
+    taxa_dict, cazy_data = build_taxa_dict(cazy_data)  # {kingdom: {organisms}}
+
+    # cache cazy_data dict
+    cache_cazy_data(cazy_data, cache_dir)
 
     add_cazyme_data.add_kingdoms(taxa_dict, connection)
 
     add_cazyme_data.add_source_organisms(taxa_dict, connection)
 
     add_cazyme_data.add_cazy_families(cazy_data, connection)
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/crawler/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/crawler/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/crawler/get_validation_data.py` & `cazy_webscraper-2.3.0/cazy_webscraper/crawler/get_validation_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/extract_seqs/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/extract_seqs/extract_db_seqs.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/extract_seqs/extract_db_seqs.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/entrez.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/genomes/entrez.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/genomes/get_genome_accs.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/genomes/get_genome_accs.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/sequences/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/sequences/get_genbank_sequences.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/sequences/get_genbank_sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 from saintBioutils.genbank import entrez_retry
 from saintBioutils.misc import get_chunks_list
 from saintBioutils.utilities.file_io import make_output_directory
 from saintBioutils.utilities.logger import config_logger
 from tqdm import tqdm
 
 from cazy_webscraper import closing_message, connect_existing_db
+from cazy_webscraper.cache.ncbi import get_cache_seqs
 from cazy_webscraper.ncbi.sequences import post_accessions_to_entrez, fetch_ncbi_seqs, get_protein_accession
 from cazy_webscraper.sql import sql_orm, sql_interface
 from cazy_webscraper.sql.sql_interface.get_data import get_selected_gbks
 from cazy_webscraper.sql.sql_interface.add_data import add_genbank_data
 from cazy_webscraper.utilities.parse_configuration import get_expansion_configuration
 from cazy_webscraper.utilities.parsers.gbk_seq_parser import build_parser
 
@@ -185,93 +186,14 @@
     # make subdir in cache dir for logging failed seqs
     make_output_directory(cache_dir, force=True, nodelete=True)
     add_genbank_data.add_gbk_seqs_to_db(seq_dict, date_today, gbk_dict, connection, cache_dir, args)
 
     closing_message("Get GenBank Sequences", start_time, args)
 
 
-def get_cache_seqs(start_time, args):
-    """Extract protein sequences from FASTA and/or JSON file, which will be added to the
-    local CAZyme database
-
-    :param seq_dict: dict, {genbank_acc: Bio.Seq}
-
-    Return update seq_dict and list of SeqRecords
-    """
-    logger = logging.getLogger(__name__)
-
-    seq_dict = {}
-    seq_records = []
-
-    if args.seq_dict:
-        logger.warning(f"Getting sequences from JSON cache:\n{args.seq_dict}")
-
-        try:
-            with open(args.seq_dict, "r") as fh:
-                cache_dict = json.load(fh)
-
-        except FileNotFoundError:
-            logger.error(
-                f"Could not find JSON file of protein sequences at:\n"
-                f"{args.seq_dict}\n"
-                "Check the path is correct"
-                "Terminating program"
-            )
-            closing_message("Get GenBank seqs", start_time, args, early_term=True)
-
-        # convert strs to SeqRecords
-        for key in cache_dict:
-            seq_dict[key] = Seq(cache_dict[key])
-
-    if args.seq_file:
-        logger.warning(f"Getting sequences from FASTA cache:\n{args.seq_file}")
-
-        try:
-            for record in SeqIO.parse(args.seq_file, "fasta"):
-                retrieved_accession = get_protein_accession(record)
-
-                if retrieved_accession is None:
-                    logger.error(
-                        "Could not retrieve a NCBI protein version accession from cache\n"
-                        f"from the record id '{record.id}'\n"
-                        "The sequence from this record will not be added to the db"
-                    )
-                    continue
-
-                try:
-                    seq_dict[retrieved_accession]
-                    if seq_dict[retrieved_accession] != record.seq:
-                        logger.warning(
-                            f"Retrieved seq for {retrieved_accession} from JSON file which does NOT match "
-                            "the seq in the FASTA file.\n"
-                            "Adding seq from the FASTA file to the local CAZyme database\n"
-                            f"JSON seq: {seq_dict[retrieved_accession]}\n"
-                            f"FASTA seq: {record.seq}"
-                        )
-                        seq_dict[retrieved_accession] = record.seq
-                except KeyError:
-                    seq_dict[retrieved_accession] = record.seq
-
-        except FileNotFoundError:
-            logger.error(
-                f"Could not find FASTA file of protein sequences at:\n"
-                f"{args.seq_file}\n"
-                "Check the path is correct"
-                "Terminating program"
-            )
-            closing_message("Get GenBank seqs", start_time, args, early_term=True)
-
-    for key in seq_dict:
-        seq_records.append(SeqRecord(id=key, seq=Seq(seq_dict[key])))
-
-    logger.warning(f"Retrieved {len(seq_records)} from cache")
-
-    return seq_dict, seq_records
-
-
 def get_records_to_retrieve(
     class_filters,
     family_filters,
     taxonomy_filter_dict,
     kingdom_filters,
     ec_filters,
     seq_dict,
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/genbank/taxonomy/get_ncbi_taxs.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/genbank/taxonomy/get_ncbi_taxs.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/gtdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/gtdb/get_gtdb_tax.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/gtdb/get_gtdb_tax.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/pdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/pdb/get_pdb_structures.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/pdb/get_pdb_structures.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/expand/uniprot/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/expand/uniprot/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/ncbi/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/gene_names/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/ncbi/gene_names/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,28 +72,27 @@
     ncbi_queries = get_chunks_list(
         list(gene_names.keys()),
         args.ncbi_batch_size,
     )
 
     invalid_gene_names = {'nan'}   # gene names no longer listed in NCBI
     failed_batches = []
+    failed_names = {}
 
     for batch in tqdm(ncbi_queries, desc="Batch quering NCBI to get protein accesions for gene names"):
         batch = list(set(batch).difference(set(invalid_gene_names)))
         uniprot_dict, invalid_gene_names, failed_batches = process_batch(
             batch,
             gene_names,
             uniprot_dict,
             invalid_gene_names,
             failed_batches,
         )
 
     if len(failed_batches) != 0:
-        failed_names = {}
-
         # remove invalid IDs
         for batch in tqdm(failed_batches, desc="Retrying failed batches"):
             batch = list(set(batch).difference(set(invalid_gene_names)))
 
             uniprot_dict, invalid_gene_names, processed_batch = process_batch(
                 batch,
                 gene_names,
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/genomes/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/ncbi/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/sequences/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/ncbi/sequences/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/ncbi/taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/lineage.py` & `cazy_webscraper-2.3.0/cazy_webscraper/ncbi/taxonomy/lineage.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/ncbi/taxonomy/multiple_taxa.py` & `cazy_webscraper-2.3.0/cazy_webscraper/ncbi/taxonomy/multiple_taxa.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 # SOFTWARE.
 """Parse taxonomy data from NCBI and CAZy to replace when multiple taxa are retrieved from CAZy"""
 
 
 import logging
 
 from saintBioutils.genbank import entrez_retry
+from saintBioutils.misc import get_chunks_list
 from tqdm import tqdm
 
 from Bio import Entrez
 
 
 def identify_multiple_taxa(cazy_data, multiple_taxa_logger):
     """Identify GenBank accessions in the CAZy data
@@ -61,25 +62,24 @@
     multiple_taxa_gbk = []
 
     for genbank_accession in tqdm(
         cazy_data,
         total=len(list(cazy_data.keys())), desc='Searching for multiple taxa annotations',
     ):
 
-        gbk_organisms = cazy_data[genbank_accession]["organism"]
-
-        if len(gbk_organisms) > 1:
+        if len(cazy_data[genbank_accession]['taxonomy']) > 1:
             multiple_taxa_gbk.append(genbank_accession)
 
-            kingdoms = ",".join(list(cazy_data[genbank_accession]["kingdom"]))
-            gbk_organisms = ",".join(list(gbk_organisms))
-
-            multiple_taxa_logger.warning(
-                f"{genbank_accession}\t{kingdoms}\t{gbk_organisms}"
-            )
+            for tax_tuple in cazy_data[genbank_accession]['taxonomy']:
+                multiple_taxa_logger.warning(
+                    f"{genbank_accession}\t{tax_tuple.kingdom}\t{tax_tuple.organism}"
+                )
+        
+        else:
+            cazy_data[genbank_accession]['organism'] = list(cazy_data[genbank_accession]['taxonomy'])[0]
 
     return multiple_taxa_gbk
 
 
 def replace_multiple_tax(cazy_data, genbank_accessions, replaced_taxa_logger, args, invalid_ids):
     """Identify GenBank accessions which have multiple source organisms listedi in CAZy.
     Replace with the latest source organism from NCBI.
@@ -92,69 +92,86 @@
     :param invalid_ids: boolean, potential presence of invalid GenBank accessions
         Set as true when func is called by replace_multiple_tax_with_invalid_ids()
 
     Return dict updated cazy_data dict and boolean, if multiple taxa were replaced by single taxa
     """
     logger = logging.getLogger(__name__)
 
-    id_post_list = str(",".join(genbank_accessions))
-
-    success = False
-
-    try:
-        epost_results = Entrez.read(
-            entrez_retry(
-                args.retries,
-                Entrez.epost,
-                "Protein",
-                id=id_post_list,
-            )
+    if args.skip_ncbi_tax:
+        logger.warning(
+            f"Skipping retrieving the latest taxonomy classification from the NCBI Taxonomy db\n"
+            "Adding the first tax listed for each protein in the CAZy db"
         )
-        success = True
-
-    except (TypeError, AttributeError):  # if no record is returned from call to Entrez
-        # error not due to the presence of invalid IDs
-        logger.error(
-            f"Entrez failed to post assembly IDs.\n"
-            "Not retrieving taxonomy classification from NCBI.\n"
-            "Selecting the first organism retrieved from CAZy as the source organism"
-        )
-        cazy_data = select_first_organism(cazy_data, genbank_accessions)
+        cazy_data = select_first_organism(cazy_data, genbank_accessions, replaced_taxa_logger)
         success = True
         return cazy_data, success
 
-    except RuntimeError:
-        logger.warning("Found GenBank accessions in CAZy data that are no longer in NCBI")
+    batches = get_chunks_list(genbank_accessions, args.ncbi_batch_size)
 
-        if invalid_ids:
-            # replace_multiple_tax was called by replace_multiple_tax_with_invalid_ids
-            # return results, don't use recursive programming
-            return cazy_data, success
+    for batch in tqdm(batches, desc=f"Batch retrieving tax info from NCBI. Batch size:{args.ncbi_batch_size}"):
 
-        else:
-            # first time replace_multiple_tax was called
-            cazy_data, success = replace_multiple_tax_with_invalid_ids(
-                cazy_data,
-                genbank_accessions,
-                replaced_taxa_logger,
-                args,
+        id_post_list = str(",".join(batch))
+
+        success = False
+
+        try:
+            epost_results = Entrez.read(
+                entrez_retry(
+                    args.retries,
+                    Entrez.epost,
+                    "Protein",
+                    id=id_post_list,
+                )
             )
+            success = True
 
-    if success is False:
-        logger.error(
-            "Could not retrieve taxonomy data from NCBI,\n"
-            "Using the first source organism retrieved from CAZy for each GenBank accession"
-        )
+        except (TypeError, AttributeError):  # if no record is returned from call to Entrez
+            # error not due to the presence of invalid IDs
+            logger.error(
+                f"Entrez failed to post assembly IDs for this batch.\n"
+                "Not retrieving tax data from NCBI for these proteins"
+                "Selecting the first organism retrieved from CAZy as the source organism\nProtein accessions:\n"
+                f"{batch}"
+            )
+            # cazy_data, gbk_accessions, replaced_taxa_logger
+            cazy_data = select_first_organism(cazy_data, batch, replaced_taxa_logger)
+            success = True
+            continue
+
+        except RuntimeError:
+            logger.warning("Found GenBank accessions in CAZy data that are no longer in NCBI")
+
+            if invalid_ids:
+                # replace_multiple_tax was called by replace_multiple_tax_with_invalid_ids
+                # return results, don't use recursive programming
+                continue
+
+            else:
+                # first time replace_multiple_tax was called
+                cazy_data, success = replace_multiple_tax_with_invalid_ids(
+                    cazy_data,
+                    genbank_accessions,
+                    replaced_taxa_logger,
+                    args,
+                )
 
-        cazy_data = select_first_organism(cazy_data, genbank_accessions, replaced_taxa_logger)
-        success = True
+        if success is False:
+            logger.error(
+                "Could not retrieve taxonomy data from NCBI for this batch,\n"
+                "Using the first source organism retrieved from CAZy for each GenBank accession\n"
+                "Protein accessions:\n"
+                f"{batch}"
+            )
 
-    else:
-        logger.info("Parsing data retrieved from NCBI")
-        cazy_data = get_ncbi_tax(epost_results, cazy_data, replaced_taxa_logger, args)
+            cazy_data = select_first_organism(cazy_data, genbank_accessions, replaced_taxa_logger)
+            success = True
+
+        else:
+            logger.info("Parsing data retrieved from NCBI")
+            cazy_data = get_ncbi_tax(epost_results, cazy_data, replaced_taxa_logger, args)
 
     return cazy_data, success
 
 
 def get_ncbi_tax(epost_results, cazy_data, replaced_taxa_logger, args):
     """Parse the ePost output from Entrez and add the NCBI tax classifications to the CAZy data
 
@@ -193,38 +210,30 @@
 
     for protein in tqdm(protein_records, desc="Retrieving organism from NCBI"):
         # retrieve NCBI taxonomy data
         accession = protein['GBSeq_accession-version']
         organism = protein['GBSeq_organism']
         kingdom = protein['GBSeq_taxonomy'].split(';')[0]
 
-        # retrieve CAZy taxonomy data
-        cazy_kingdom = cazy_data[accession]["kingdom"]
-        cazy_organisms = cazy_data[accession]["organism"]
-
-        cazy_kingdom_str = ",".join(cazy_kingdom)
-        cazy_organism_str = ','.join(cazy_organisms)
-
         try:
-            cazy_data[accession]['kingdom'] = {kingdom}
-            cazy_data[accession]['organism'] = {organism}
-
-            # log the difference
-            replaced_taxa_logger.warning(
-               f"{accession}\t{cazy_kingdom_str}: {cazy_organism_str}\t{kingdom}: {organism}"
-            )
+            cazy_data[accession]['kingdom'] = kingdom
+            cazy_data[accession]['organism'] = organism
 
         except KeyError:
             err = (
                 f'GenBank accession {accession} retrieved from NCBI, but it is not present in CAZy'
             )
             logger.error(err)
+            continue
 
+        for tax_tuple in list(cazy_data[accession]['taxonomy'])[1:]:
             replaced_taxa_logger.warning(
-               f"{accession}\t{cazy_kingdom_str}: {cazy_organism_str}\t{err}"
+                f"{accession}\t"
+                f"SELECTED: {kingdom} -- {organism}"
+                f"\tREPLACED: {tax_tuple.kingdom}: {tax_tuple.organism}"
             )
 
     return cazy_data
 
 
 def replace_multiple_tax_with_invalid_ids(cazy_data, gbk_accessions, replaced_taxa_logger, args):
     """Retrieve the latest taxonomy classification for proteins with multiple source organisms.
@@ -315,23 +324,21 @@
     :param gbk_accessions: list of GenBank accessions
     :param replaced_taxa_logger: logger, used for logging GenBank accessions with
         multiple taxa in CAZy
 
     Return cazy_data (dict)
     """
     for accession in tqdm(gbk_accessions, desc='Selecting the first retrieved organism'):
-        cazy_kingdoms_str = ",".join(list(cazy_data[accession]["kingdom"]))
-        cazy_organisms_str = ",".join(list(cazy_data[accession]["organism"]))
-
-        cazy_kingdom = list(cazy_data[accession]["kingdom"])[0]
-        cazy_organism = list(cazy_data[accession]["organism"])[0]
+        selected_kingdom = list(cazy_data[accession]['taxonomy'])[0].kingdom
+        selected_organism = list(cazy_data[accession]['taxonomy'])[0].organism
 
-        cazy_data[accession]["kingdom"] = {cazy_kingdom}
-        cazy_data[accession]["organism"] = {cazy_organism}
+        for tax_tuple in list(cazy_data[accession]['taxonomy'])[1:]:
+            replaced_taxa_logger.warning(
+                f"{accession}\t"
+                f"SELECTED: {selected_kingdom} -- {selected_organism}"
+                f"\tREPLACED: {tax_tuple.kingdom}: {tax_tuple.organism}"
+            )
 
-        # log the data that was replaced and the data it was replaced with
-        replaced_taxa_logger.warning(
-            f"{accession}\t{cazy_kingdoms_str}: "
-            f"{cazy_organisms_str}\t{cazy_kingdom}: {cazy_organism}"
-        )
+        cazy_data[accession]["kingdom"] = selected_kingdom
+        cazy_data[accession]["organism"] = selected_organism
 
     return cazy_data
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_cazyme_data.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_cazyme_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,17 @@
             except KeyError:  # organism not in the db, build new record
                 genus = organism.split(" ")[0]
                 species = ' '.join(organism.split(" ")[1:])
                 new_record = (genus, species, kingdom_id,)
                 taxonomy_db_insert_values.add( new_record )
     
     if len(taxonomy_db_insert_values) != 0:
+        with open("tax_sets", "w") as fh:
+            for tax in taxonomy_db_insert_values:
+                fh.write(f"{tax}\n")
         logger.info(
             f"Adding {len(taxonomy_db_insert_values)} new tax records to the db"
         )
         insert_data(
             connection,
             'Taxs',
             ['genus', 'species', 'kingdom_id'],
@@ -227,24 +230,24 @@
     # {genus species: {'tax_id': db_tax_id, 'kingdom_id': kingdom_id}
 
     gbk_record_updates = set()  # {gbk_accession: 'taxa_id': (new taxa_id) int, 'gbk_id': int}
     gbk_db_insert_values = set()
 
     for gbk_accession in tqdm(cazy_data, desc="Compiling Genbank records for insertion"):
         if gbk_accession not in existing_gbk_records:
-            organism = list(cazy_data[gbk_accession]['organism'])[0]
+            organism = cazy_data[gbk_accession]['organism']
             taxa_id = taxa_table_dict[organism]['tax_id']
             gbk_db_insert_values.add( (gbk_accession, taxa_id,) )
         
         else:  # check if need to update taxa_id
             # get the taxa_id for the existing record
             existing_record_id = gbk_table_dict[gbk_accession]['taxa_id']
             
             # get the taxa_id for the organism listed in the CAZy txt file
-            organism = list(cazy_data[gbk_accession]['organism'])[0]
+            organism = cazy_data[gbk_accession]['organism']
             cazy_data_taxa_id = taxa_table_dict[organism]['tax_id']
             
             if cazy_data_taxa_id != existing_record_id:
                 # need to update the record
                 gbk_record_updates.add( (cazy_data_taxa_id, gbk_table_dict[gbk_accession]['gbk_id']) )
 
     if len(gbk_db_insert_values) != 0:
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_genbank_data.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_genbank_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_genome_data.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_genome_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_gtdb_tax.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_gtdb_tax.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_ncbi_tax_data.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_ncbi_tax_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/add_data/add_uniprot_data.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/add_data/add_uniprot_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,252 +43,280 @@
 
 import logging
 from sqlalchemy import delete, text
 from tqdm import tqdm
 
 from cazy_webscraper.sql.sql_interface import insert_data
 from cazy_webscraper.sql.sql_interface.get_data import get_table_dicts
-from cazy_webscraper.sql.sql_orm import genbanks_ecs
+from cazy_webscraper.sql.sql_orm import genbanks_ecs, Ec, Pdb
 
 
-def add_uniprot_accessions(uniprot_dict, gbk_dict, connection, args):
+def add_uniprot_accessions(uniprot_dict, connection, args):
     """Add UniProt data to the local CAZyme database
     
     :param uniprot_dict: dict containing data retrieved from UniProt
-    :param gbk_dict: dict representing data from the Genbanks table
+        uniprot_dict[ncbi_acc] = {
+            'uniprot_acc': uniprot_acc, - str
+            'protein_name': protein_name, -str
+            'ec_numbers': ec_numbers, - set
+            'sequence': sequence, - str
+            'sequence_date': date seq was last updated yyyy-mm-dd
+            'pdbs': all_pdbs, - set
+        }
     :param connection: open sqlalchemy conenction to an SQLite db engine
     :param args: cmd-line args parser
 
     Return nothing.
     """
     logger = logging.getLogger(__name__)
 
     # load the current Uniprot records in the local CAZyme db
     # {acc: {name: str, gbk_id: int, seq: str, seq_date:str } }
     uniprot_table_dict = get_table_dicts.get_uniprot_table_dict(connection)
 
-    uniprot_insert_values = set()
+    uniprot_insert_values = set()   # new rows to add to the local CAZyme db Uniprots table
+    record_names_to_update = set()  # ((uniprot_accession, retrieved_name), )
+    record_seqs_to_update = set()   # ((uniprot_accession, retrieved_sequence), )
+
+    for ncbi_acc in tqdm(uniprot_dict, desc="Separating new and existing Uniprots Table records"):
+        # check if the uniprot accession is in the local CAZyme datbase
+        uniprot_acc = uniprot_dict[ncbi_acc]['uniprot_acc']
 
-    # the following variables containing objects in the local db that are to be updated
-    update_record_gbk_id = set()  # ((uniprot_accession, gbk_id),)
-    update_record_name = set()  # ((uniprot_accession, retrieved_name), )
-    update_record_seq = set()  # ((uniprot_accession, retrieved_seq), )
-
-    for uniprot_acc in tqdm(uniprot_dict, desc="Separating new and existing records"):
-        # check the genbank accession is in the local cazyme database
-        retrieved_gbk_acc = uniprot_dict[uniprot_acc]["genbank_accession"]
         try:
-            gbk_dict[retrieved_gbk_acc]
+            uniprot_table_dict[uniprot_acc]
         except KeyError:
-            logger.error(
-                f"Mapped the GenBank accession '{retrieved_gbk_acc}' to the UniProt accession\n"
-                f"'{uniprot_acc}' but the GenBank accession is not in the local CAZyme database\n"
-                f"therefore, not adding protein data for GBK:{retrieved_gbk_acc}/UniProt:{uniprot_acc}"
-                "to the local CAZyme database."
-            )
+            # uniprot acc not in Uniprots table, so will need to add
+            if args.sequence:  # add seq to local db
+                uniprot_insert_values.add(
+                    (
+                        uniprot_acc,
+                        uniprot_dict[ncbi_acc]['protein_name'],
+                        uniprot_dict[ncbi_acc]['sequence'],
+                        uniprot_dict[ncbi_acc]['sequence_date'],
+                    )
+                )
+            else:  # do not add sequence
+                uniprot_insert_values.add(
+                    (
+                        uniprot_acc,
+                        uniprot_dict[ncbi_acc]['protein_name'],
+                    )
+                )
             continue
-        # check if the UniProt accession is already in the local CAZyme db
-        try:
-            uniprot_table_dict[uniprot_acc]
-            # Uniprot accession is already in the local CAZyme db
 
-            # check if the GenBank id is the same
-            existing_gbk_id = uniprot_table_dict[uniprot_acc]['genbank_id']
-            retrieved_gbk_acc = uniprot_dict[uniprot_acc]["genbank_accession"]
-            retrieved_gbk_id = gbk_dict[retrieved_gbk_acc]
-            if existing_gbk_id != retrieved_gbk_id:
-                update_record_gbk_id.add( (uniprot_acc, retrieved_gbk_id) )
-                
-            if args.name_update:
-                # check if the name has changed
-                existing_name = uniprot_table_dict[uniprot_acc]["protein_name"]
-                retrieved_name = uniprot_dict[uniprot_acc]["protein_name"]
-                
-                if existing_name != retrieved_name:
-                    update_record_name.add( (uniprot_acc, retrieved_name) )
-            
-            if args.sequence:  # only add seq if sequence is not there
-                if uniprot_table_dict[uniprot_acc]['seq'] is None:
-                    update_record_seq.add( (uniprot_acc, uniprot_dict[uniprot_acc]["sequence"]) )
-                
-            if args.seq_update:  # update seq if a newer version is available or no seq present
-                if uniprot_table_dict[uniprot_acc]['seq'] is None:
-                        update_record_seq.add( (
-                            uniprot_acc,
-                            uniprot_dict[uniprot_acc]["sequence"],
-                            uniprot_dict[uniprot_acc]["seq_date"],
-                        ) )
-                else:
-                    existing_date = uniprot_table_dict[uniprot_acc]['seq_date']
-                    retrieved_date = uniprot_dict[uniprot_acc]['seq_date']
-                    
-                    if existing_date < retrieved_date:  # existing date is older, update seq
-                        update_record_seq.add( (
-                            uniprot_acc,
-                            uniprot_dict[uniprot_acc]["sequence"],
-                            uniprot_dict[uniprot_acc]["seq_date"],
-                        ) )
-        
-        except KeyError:  # new record to add to local CAZyme db
-            
-            if args.sequence or args.seq_update:
-                genbank_acc = uniprot_dict[uniprot_acc]["genbank_accession"]
-                gbk_id = gbk_dict[genbank_acc]
-                uniprot_name = uniprot_dict[uniprot_acc]["protein_name"]
-                seq = uniprot_dict[uniprot_acc]["sequence"]
-                date = uniprot_dict[uniprot_acc]["seq_date"]
-
-                uniprot_insert_values.add( (gbk_id, uniprot_acc, uniprot_name, seq, date) )
-
-            else:  # not retrieving protein sequences
-                genbank_acc = uniprot_dict[uniprot_acc]["genbank_accession"]
-                gbk_id = gbk_dict[genbank_acc]
-                uniprot_name = uniprot_dict[uniprot_acc]["protein_name"]
-                
-                uniprot_insert_values.add( (gbk_id, uniprot_acc, uniprot_name) )
+        # uniprot acc already in the db
+        # check if need to update name or sequence
+
+        if args.update_name:
+            if uniprot_table_dict[uniprot_acc]['name'] != uniprot_dict[ncbi_acc]['protein_name']:
+                logger.warning(
+                    f"Updating protein name for UniProt acc {uniprot_acc} from:\n"
+                    f"{uniprot_table_dict[uniprot_acc]['name']}\n"
+                    "to:\n"
+                    f"{uniprot_dict[ncbi_acc]['protein_name']}"
+                )
+                record_names_to_update.add(
+                    (
+                        uniprot_acc,
+                        uniprot_dict[ncbi_acc]['protein_name'],
+                    )
+                )
+
+        if args.update_seq:
+            if uniprot_table_dict[uniprot_acc]['seq'] != uniprot_dict[ncbi_acc]['sequence']:
+                logger.warning(
+                    f"Updating protein sequence for UniProt acc {uniprot_acc} from:\n"
+                    f"{uniprot_table_dict[uniprot_acc]['seq']}\n"
+                    "to:\n"
+                    f"{uniprot_dict[ncbi_acc]['sequence']}"
+                )
+                record_seqs_to_update.add(
+                    (
+                        uniprot_acc,
+                        uniprot_dict[ncbi_acc]['sequence'],
+                        uniprot_dict[ncbi_acc]['sequence_date'],
+                    )
+                )
     
     if len(uniprot_insert_values) != 0:
-        logger.warning(f"Inserting {len(uniprot_insert_values)} into the local CAZyme db")
-        if args.sequence or args.seq_update:
-            columns = ['genbank_id', 'uniprot_accession', 'uniprot_name', 'sequence', 'seq_update_date']
+        logger.warning(f"Inserting {len(uniprot_insert_values)} ew records into the Uniprots table")
+        if args.sequence:
+            columns = ['uniprot_accession', 'uniprot_name', 'sequence', 'seq_update_date']
         else:
-            columns = ['genbank_id', 'uniprot_accession', 'uniprot_name']
+            columns = ['uniprot_accession', 'uniprot_name']
     
         insert_data(connection, "Uniprots", columns, list(uniprot_insert_values))
 
-    if len(update_record_gbk_id) != 0:
-        logger.warning(f"Updating {len(update_record_gbk_id)} Gbk-UniProt relationships in the local CAZyme db")
-        with connection.begin():
-            for record in tqdm(update_record_gbk_id, desc="Updating UniProt-Gbk relationships"):
-                connection.execute(
-                    text(
-                        "UPDATE Uniprots "
-                        f"SET genbank_id = {record[1]} "
-                        f"WHERE uniprot_accession = '{record[0]}'"
-                    )
-                )
         
-    if len(update_record_name) != 0:
-        logger.warning(f"Updating {len(update_record_name)} UniProt protein names in the local CAZyme db")
+    if len(record_names_to_update) != 0:
+        logger.warning(f"Updating {len(record_names_to_update)} UniProt protein names in the local CAZyme db")
         with connection.begin():
-            for record in tqdm(update_record_name, desc="Updating UniProt protein names"):
+            for record in tqdm(record_names_to_update, desc="Updating UniProt protein names"):
                 connection.execute(
                     text(
                         "UPDATE Uniprots "
                         f"SET uniprot_name = {record[1]} "
                         f"WHERE uniprot_accession = '{record[0]}'"
                     )
                 )
 
-    if len(update_record_seq) != 0:
-        logger.warning(f"Updating {len(update_record_seq)} UniProt protein sequences in the local CAZyme db")
+    if len(record_seqs_to_update) != 0:
+        logger.warning(f"Updating {len(record_seqs_to_update)} UniProt protein sequences in the local CAZyme db")
         with connection.begin():
-            for record in tqdm(update_record_seq, desc="Updating UniProt protein seqs"):
+            for record in tqdm(record_seqs_to_update, desc="Updating UniProt protein seqs"):
                 connection.execute(
                     text(
                         "UPDATE Uniprots "
                         f"SET sequence = {record[1]}, seq_update_date = {record[2]} "
                         f"WHERE uniprot_accession = '{record[0]}'"
                     )
                 )
 
     return
 
 
-def add_ec_numbers(uniprot_dict, all_ecs, gbk_dict, connection, args):
+def add_uniprot_genbank_relationships(uniprot_dict, connection):
+    """Add Uniprots local db IDs to Genbanks table to link Genbanks and Uniprots records.
+
+    :param uniprot_dict: dict of data from uniprot
+        uniprot_dict[ncbi_acc] = {
+            'uniprot_acc': uniprot_acc,
+            'uniprot_entry_id': uniprot_entry_id,
+            'protein_name': protein_name,
+            'ec_numbers': ec_numbers,
+            'sequence': sequence,
+            'pdbs': all_pdbs,
+        }
+    :param connection: open sqlite3 engine connection
+
+    Return nothing.
+    """
+    logger = logging.getLogger(__name__)
+
+    uniprot_table_dict = get_table_dicts.get_uniprot_table_dict(connection)
+    # uniprot_table_dict = {acc: {db_id: int, name: str, seq: str, seq_date:str } }
+
+    logger.warning(
+        f"Linking {len(list(uniprot_dict.keys()))} Genbank records in the local CAZyme db"
+        "to records in the Uniprots table"
+    )
+    with connection.begin():
+        for ncbi_acc in tqdm(uniprot_dict, desc="Updating Genbanks records"):
+            uniprot_acc = uniprot_dict[ncbi_acc]['uniprot_acc']
+            try:
+                uniprot_db_id = uniprot_table_dict[uniprot_acc]['db_id']
+            except KeyError:
+                logger.error(
+                    f"Could not find a local db record for UniProt accession {uniprot_acc}\n"
+                    "Not linking the accession to a record in the Genbanks table"
+                )
+                continue
+
+            connection.execute(
+                text(
+                    "UPDATE Genbanks "
+                    f"SET uniprot_id = {uniprot_db_id} "
+                    f"WHERE genbank_accession = '{ncbi_acc}'"
+                )
+            )
+    
+
+def add_ec_numbers(uniprot_dict, connection, args):
     """Add EC numbers to the local CAZyme database
 
     :param uniprot_dict: dict containing data retrieved from UniProt
-    :param all_ecs: set of all EC numbers retrieved from UniProt
-    :param gbk_dict: dict representing data from the Genbanks table
+        uniprot_dict[ncbi_acc] = {
+            'uniprot_acc': uniprot_acc, - str
+            'protein_name': protein_name, -str
+            'ec_numbers': ec_numbers, - set
+            'sequence': sequence, - str
+            'sequence_date': date seq was last updated yyyy-mm-dd
+            'pdbs': all_pdbs, - set
+        }
     :param connection: open sqlalchemy conenction to an SQLite db engine
     :param args: cmd-line args parser
 
     Return nothing.
     """
+    logger = logging.getLogger(__name__)
+    
     # load EC records in the local CAZyme db
     ec_table_dict = get_table_dicts.get_ec_table_dict(connection)
 
     # identify new EC numbers to add to the EC table
     existing_ecs = list(ec_table_dict.keys())
     ec_insert_values = set()
 
-    for ec in all_ecs:
-        if ec[0] not in existing_ecs:
-            ec_insert_values.add( ec )
+    for ncbi_acc in tqdm(uniprot_dict, desc="Identifying EC numbers to add to the local CAZyme db"):
+        for ec_num in uniprot_dict[ncbi_acc]['ec_numbers']:
+            if ec_num not in existing_ecs:
+                ec_insert_values.add((ec_num,))
 
     if len(ec_insert_values) != 0:
         insert_data(connection, "Ecs", ["ec_number"], list(ec_insert_values))
 
-        # load in the newly updated EC table from the local CAZyme db
-        ec_table_dict = get_table_dicts.get_ec_table_dict(connection)
+
+def add_genbank_ec_relationships(uniprot_dict, gbk_dict, connection, args):
+    """Add and update relationships between the Genbanks and Ecs table.
+
+    :param uniprot_dict: dict containing data retrieved from UniProt
+        uniprot_dict[ncbi_acc] = {
+            'uniprot_acc': uniprot_acc, - str
+            'protein_name': protein_name, -str
+            'ec_numbers': ec_numbers, - set
+            'sequence': sequence, - str
+            'sequence_date': date seq was last updated yyyy-mm-dd
+            'pdbs': all_pdbs, - set
+        }
+    :param gbk_dict: {gbk_acc: gbk_id}
+    :param connection: open sqlalchemy conenction to an SQLite db engine
+    :param args: cmd-line args parser
+
+    Return nothing
+    """
+    # load in EC records in the local CAZyme db
+    # {ec_number: ec_id}
+    ec_table_dict = get_table_dicts.get_ec_table_dict(connection)
     
     # load in gbk_ec table, contains the gbk-ec number relationships
-    ec_gbk_table_dict = get_table_dicts.get_ec_gbk_table_dict(connection)  # {ec_id: {gbk ids}}
+    # {ec_id: {gbk ids}}
+    ec_gbk_table_dict = get_table_dicts.get_ec_gbk_table_dict(connection)  
 
-    if args.delete_old_ec:
-        gbk_ec_table_dict = get_table_dicts.get_gbk_ec_table_dict(connection)  # {gbk_id: {ec ids}}
-        ecs_rel_to_delete = set()  # set of tuples (gbk_id, ec_id)
-
-    # compile list of tuples to insert into the Genbanks_Ecs table
+    # compile list of tuples to insert or delete into the Genbanks_Ecs table
     gbk_ec_insert_values = set()
 
-    for uniprot_acc in tqdm(uniprot_dict, desc="Updating EC numbers"):
-        genbank_acc = uniprot_dict[uniprot_acc]["genbank_accession"]
-        try:
-            gbk_id = gbk_dict[genbank_acc]
-        except KeyError:
-            logger.error(
-                f"Mapped the GenBank accession '{genbank_acc}' to the UniProt accession\n"
-                f"'{uniprot_acc}' but the GenBank accession is not in the local CAZyme database\n"
-                f"therefore, not adding protein data for GBK:{genbank_acc}/UniProt:{uniprot_acc}"
-                "to the local CAZyme database."
-            )
-            continue
-        
-        retrieved_ec_numbers = uniprot_dict[uniprot_acc]["ec"]  # EC#s retrieved from UniProt
-        for ec in retrieved_ec_numbers:
-            ec_id = ec_table_dict[ec]
+    for ncbi_acc in tqdm(uniprot_dict, desc="Adding and updating EC-Genbanks relationships"):
+        for ec_number in uniprot_dict[ncbi_acc]['ec_numbers']:
+            gbk_db_id = gbk_dict[ncbi_acc]
+            ec_id = ec_table_dict[ec_number]
 
             try:
-                existing_gbk_relationships = ec_gbk_table_dict[ec_id]
-                # check if protein-ec# relationship is already in the db
-                if gbk_id not in existing_gbk_relationships:
-                    gbk_ec_insert_values.add( (gbk_id, ec_id) )
-            except KeyError:  # when adding relationship for the first time
-                gbk_ec_insert_values.add( (gbk_id, ec_id) )
-
-        if args.delete_old_ec:
-            existing_ec_relationships = gbk_ec_table_dict[gbk_id]
-            for ec in retrieved_ec_numbers:
-                ec_id = ec_table_dict[ec]
-                if ec_id not in existing_ec_relationships:
-                    ecs_rel_to_delete.add( (gbk_id, ec_id) )
+                existing_relationships = ec_gbk_table_dict[ec_id]
+                if gbk_db_id not in existing_relationships:
+                    gbk_ec_insert_values.add( (gbk_db_id, ec_id) )
+
+            except KeyError: # EC number is not linked to any gbk records so add new records
+                gbk_ec_insert_values.add( (gbk_db_id, ec_id) )
 
     if len(gbk_ec_insert_values) != 0:
         insert_data(connection, "Genbanks_Ecs", ["genbank_id", "ec_id"], list(gbk_ec_insert_values))
 
-    if args.delete_old_ec and len(ecs_rel_to_delete) != 0:
-        with connection.begin():
-            for record in tqdm(ecs_rel_to_delete, desc="Deleteing old GenBank-EC relationships"):
-                # record = (genbank_id, ec_id,)
-                stmt = (
-                    delete(genbanks_ecs).\
-                    where(genbanks_ecs.c.genbank_id == record[0]).\
-                    where(genbanks_ecs.c.ec_id == record[1])
-                )
-                connection.execute(stmt)
-
-    return
-
 
 def add_pdb_accessions(uniprot_dict, gbk_dict, connection, args):
     """Add PDB accessions to the local CAZyme database
 
     :param uniprot_dict: dict containing data retrieved from UniProt
+        uniprot_dict[ncbi_acc] = {
+            'uniprot_acc': uniprot_acc, - str
+            'protein_name': protein_name, -str
+            'ec_numbers': ec_numbers, - set
+            'sequence': sequence, - str
+            'sequence_date': date seq was last updated yyyy-mm-dd
+            'pdbs': all_pdbs, - set
+        }
     :param gbk_dict: dict representing data from the Genbanks table
     :param connection: open sqlalchemy conenction to an SQLite db engine
     :param args: cmd-line args parser
 
     Return nothing.
     """
     logger = logging.getLogger(__name__)
@@ -298,117 +326,176 @@
 
     # load in PDB objects in the local CAZyme db
     pdb_table_dict = get_table_dicts.get_pdb_table_dict(connection)
     # {pdb_accession: pdb_db_id}
 
     # First, identify new PDB accessions to add to the database
     pdb_insert_values = set()
-    for uniprot_acc in tqdm(uniprot_dict, desc="Identifying new PDBs to add to db"):
-        for pdb in uniprot_dict[uniprot_acc]["pdb"]:
+    for ncbi_acc in tqdm(uniprot_dict, desc="Identifying new PDBs to add to db"):
+        for pdb in uniprot_dict[ncbi_acc]["pdbs"]:
             try:
                 pdb_table_dict[pdb]
             except KeyError:
                 pdb_insert_values.add( (pdb,) )
     
     if len(pdb_insert_values) != 0:
         logger.warning(f"Adding {len(pdb_insert_values)} PDB accessions to the database")
         insert_data(connection, "Pdbs", ["pdb_accession"], list(pdb_insert_values))
-        # reload the updated pdb table
-        pdb_table_dict = get_table_dicts.get_pdb_table_dict(connection)
+
+
+def add_pdb_gbk_relationships(uniprot_dict, gbk_dict, connection, args):
+    """Add relationships between PDB accessions and proteins in the Genbanks table
+
+    :param uniprot_dict: dict containing data retrieved from UniProt
+        uniprot_dict[ncbi_acc] = {
+            'uniprot_acc': uniprot_acc, - str
+            'protein_name': protein_name, -str
+            'ec_numbers': ec_numbers, - set
+            'sequence': sequence, - str
+            'sequence_date': date seq was last updated yyyy-mm-dd
+            'pdbs': all_pdbs, - set
+        }
+    :param gbk_dict: dict representing data from the Genbanks table
+    :param connection: open sqlalchemy conenction to an SQLite db engine
+    :param args: cmd-line args parser
+
+    Return nothing.
+    """
+    # load the updated pdb table
+    # {pdb_acc: pdb_db_id}
+    pdb_table_dict = get_table_dicts.get_pdb_table_dict(connection)
     
     # load in Genbanks_Pdbs relationship table
     gbk_pdb_rel_table_dict = get_table_dicts.get_gbk_pdb_table_dict(connection)
-    # {gbk_db_id: {pdb_db_id} }
+    # {gbk_db_id: set(pdb_db_ids) }
 
     # convert the data from UniProt into a dict of {gbk_db_id: pdb_db_id} 
     # to identify pdb-protein relationships retrieved from UniProt
     gbk_pdb_insert_values = set()
-    for uniprot_acc in tqdm(uniprot_dict, desc="Identifying new protein-PDB relationships to add to db"):
-        genbank_acc = uniprot_dict[uniprot_acc]["genbank_accession"]
 
+    for ncbi_acc in tqdm(uniprot_dict, desc="Identifying new protein-PDB relationships to add to db"):
+
+        if len(uniprot_dict[ncbi_acc]['pdbs']) == 0:  # not relationships to add
+            continue
+
+        uniprot_acc = uniprot_dict[ncbi_acc]['uniprot_acc']
         try:
-            gbk_db_id = gbk_dict[genbank_acc]
+            gbk_db_id = gbk_dict[ncbi_acc]
         except KeyError:
             logger.error(
-                f"Mapped the GenBank accession '{genbank_acc}' to the UniProt accession\n"
+                f"Mapped the GenBank accession '{ncbi_acc}' to the UniProt accession\n"
                 f"'{uniprot_acc}' but the GenBank accession is not in the local CAZyme database\n"
-                f"therefore, not adding protein data for GBK:{genbank_acc}/UniProt:{uniprot_acc}"
+                f"therefore, not adding protein data for GBK:{ncbi_acc}/UniProt:{uniprot_acc}"
                 "to the local CAZyme database."
             )
             continue
 
-        # set of pdb_accessions retrieved from UniProt
-        retrieved_pdbs = uniprot_dict[uniprot_acc]["pdb"]
-        if len(retrieved_pdbs) == 0:
-            continue
-
-        # set of pdb_db_ids the protein (gbk_db_id) is already related to in the db
+        # check if there any existing relationships for the gbk record
         try:
             existing_pdb_relationships = gbk_pdb_rel_table_dict[gbk_db_id]  
         except KeyError:
             existing_pdb_relationships = set()
 
-        for pdb_acc in retrieved_pdbs:
-            pdb_db_id = pdb_table_dict[pdb_acc]
-
+        for pdb_acc in uniprot_dict[ncbi_acc]["pdbs"]:
             try:
-                if pdb_db_id not in existing_pdb_relationships:
-                    # genbank and pdb records not yet stored together in the relationship table
-                    gbk_pdb_insert_values.add( (gbk_db_id, pdb_db_id) )
+                pdb_db_id = pdb_table_dict[pdb_acc]
             except KeyError:
-                # genbank not listed in the Genbanks_Pdbs relationship table
+                logger.error(
+                    f"Retrieved PDB:{pdb_acc} from UniProt.\n"
+                    "Cannot link to Genbanks table records because PDB not listed in the Pdbs table"
+                )
+                continue
+            
+            if pdb_db_id not in gbk_pdb_rel_table_dict:
                 gbk_pdb_insert_values.add( (gbk_db_id, pdb_db_id) )
 
-        if args.delete_old_pdbs:
-            # convert gbk_pdb_rel_table_dict to be keyed by pdb_db_ids and valued by set of gbk_db_ids
-            pdb_gbk_relationships = {}
-            for existing_gbk_id in gbk_pdb_rel_table_dict:
-                existing_pdbs = gbk_pdb_rel_table_dict[existing_gbk_id]
-                for pdb in existing_pdbs:
-                    try:
-                        pdb_gbk_relationships[pdb].add(existing_gbk_id)
-                    except KeyError:
-                        pdb_gbk_relationships[pdb] = {existing_gbk_id}
-
-            # for each pdb_db_id related to the current protein in the db
-            # get the corresponding pdb_accession
-            all_existing_pdb_ids = list(set(pdb_table_dict.values()))
-            all_existing_pdb_accs = list(pdb_table_dict.keys())
-
-            for pdb_db_id in existing_pdb_relationships:
-                position = all_existing_pdb_ids.index(pdb_db_id)
-                pdb_acc = all_existing_pdb_accs[position]
-
-                if pdb_acc not in retrieved_pdbs:
-                    # delete genbank-pdb relationship
-                    relationships_to_delete.add( (gbk_db_id, pdb_db_id) )
-
-                    # check if can delete pdb accession because it is not linked to any other proteins
-                    if len(pdb_gbk_relationships[pdb_db_id]) != 1:  # deleting one pdb accession will not leave not related to any genbanks
-                        pdbs_to_delete.add( (pdb_acc) )
-
     if len(gbk_pdb_insert_values) != 0:
         insert_data(connection, "Genbanks_Pdbs", ["genbank_id", "pdb_id"], list(gbk_pdb_insert_values))
 
-    if args.delete_old_pdbs and len(pdbs_to_delete) != 0:
-        with connection.begin():
-            for record in tqdm(pdbs_to_delete, desc="Deleteing old PDB accessions"):
-            # record = (pdb_acc,)
-                connection.execute(
-                    text(
-                        "DELETE Pdbs "
-                        f"WHERE pdb_accession = '{record[0]}'"
-                    )
-                )
 
-    if args.delete_old_pdbs and len(relationships_to_delete) != 0:
-        with connection.begin():
-            for record in tqdm(relationships_to_delete, desc="Deleteing old Genbank-PDB relationships"):
-            # record = (pdb_acc,)
-                connection.execute(
-                    text(
-                        "DELETE Genbanks_Pdbs "
-                        f"WHERE genbank_id = '{record[0]}' AND pdb_id = '{record[1]}'"
-                    )
+def add_uniprot_taxs(uniprot_dict, connection, args):
+    """Add taxonomic classifications (genus, species) to the local CAZyme database UniprotTaxs table.
+
+    :param uniprot_dict: dict containing data retrieved from UniProt
+        uniprot_dict[ncbi_acc] = {
+            'uniprot_acc': uniprot_acc, - str
+            'protein_name': protein_name, -str
+            'ec_numbers': ec_numbers, - set
+            'sequence': sequence, - str
+            'sequence_date': date seq was last updated yyyy-mm-dd
+            'pdbs': all_pdbs, - set
+        }
+    :param connection: open sqlalchemy conenction to an SQLite db engine
+    :param args: cmd-line args parser
+
+    Return nothing.
+    """
+    # add tax data to the local db
+    # load the table
+    ut_table_dict, ut_tax_dict = get_table_dicts.get_uniprottax_table_dict(connection)
+    # {db id: {'genus': str, 'species': str}}
+    # {'genus species': db id}
+
+    taxs_to_add = set()
+
+    for ncbi_acc in tqdm(uniprot_dict, desc="Identifying taxs to add to db"):
+        genus = uniprot_dict[ncbi_acc]['genus']
+        species = uniprot_dict[ncbi_acc]['species']
+
+        try:
+            ut_tax_dict[f"{genus} {species}"]
+        except KeyError:
+            taxs_to_add.add( (genus, species) )
+
+    if len(taxs_to_add) > 0:
+        insert_data(connection, "UniprotTaxs", ["genus", "species"], list(taxs_to_add))
+
+    add_uniprot_tax_relationships(uniprot_dict, connection, args)
+
+    
+def add_uniprot_tax_relationships(uniprot_dict, connection, args):
+    """Link Uniprot records to UniprotTaxs table.
+
+    :param uniprot_dict: dict containing data retrieved from UniProt
+        uniprot_dict[ncbi_acc] = {
+            'uniprot_acc': uniprot_acc, - str
+            'protein_name': protein_name, -str
+            'ec_numbers': ec_numbers, - set
+            'sequence': sequence, - str
+            'sequence_date': date seq was last updated yyyy-mm-dd
+            'pdbs': all_pdbs, - set
+        }
+    :param connection: open sqlalchemy conenction to an SQLite db engine
+    :param args: cmd-line args parser
+
+    Return nothing.
+    """
+    ut_table_dict, ut_tax_dict = get_table_dicts.get_uniprottax_table_dict(connection)
+    # {db id: {'genus': str, 'species': str}}
+    # {'genus species': db id}
+    
+    uniprot_table_dict = get_table_dicts.get_uniprot_table_dict(connection)
+    # {acc: {name: str, gbk_id: int, seq: str, seq_date:str } }
+
+    print('ut_tax_dict:', ut_tax_dict)
+
+    relationships = {}  # {uniprot db id: uniprot tax db id}
+
+    for ncbi_acc in tqdm(uniprot_dict, desc="Identifying Uniprot-Tax relationships"):
+        genus = uniprot_dict[ncbi_acc]['genus']
+        species = uniprot_dict[ncbi_acc]['species']
+        uniprot_acc = uniprot_dict[ncbi_acc]['uniprot_acc']
+
+        uni_db_id = uniprot_table_dict[uniprot_acc]['db_id']
+        tax_db_id = ut_tax_dict[f"{genus} {species}"]
+
+        relationships[uni_db_id] = tax_db_id
+
+    with connection.begin():
+        for uni_db_id in tqdm(relationships, desc="Adding Uniprot-Tax relationships"):
+            connection.execute(
+                text(
+                    "UPDATE Uniprots "
+                    f"SET uniprot_tax_id = {relationships[uni_db_id]} "
+                    f"WHERE uniprot_id = '{uni_db_id}'"
                 )
-                
-    return
+            )
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_api_data.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_api_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_assemblies.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_assemblies.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_records.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_records.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_selected_gbks.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_selected_gbks.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_selected_pdbs.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_selected_pdbs.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_table_dicts.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_table_dicts.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     GtdbTax,
     Kingdom,
     NcbiTax,
     Pdb,
     Session,
     Taxonomy,
     Uniprot,
+    UniprotTax,
 )
 
 
 def get_ec_table_dict(connection):
     """Create dict of objects present in the CazyFamilies table.
     
     :param connection: open sqlalchemy db engine connection
@@ -319,15 +320,15 @@
 
 
 def get_gbk_pdb_table_dict(connection):
     """Create dict of objects present in the Genbanks_Pdbs table.
     
     :param connection: open sqlalchemy db engine connection
     
-    Return dict {gbk_db_id: {pdb_db_id} }
+    Return dict {gbk_db_id: set(pdb_db_ids) }
     """
     with Session(bind=connection) as session:
         all_gbk_pdb_records = session.query(Genbank, Pdb).\
             join(Pdb, Genbank.pdbs).\
             all()
 
     gbk_pdb_table_dict = {}  # {pdb_accession: pdb_db_id}
@@ -371,25 +372,25 @@
 
 
 def get_uniprot_table_dict(connection):
     """Create dict of objects present in the Uniprots table.
     
     :param connection: open sqlalchemy db engine connection
     
-    Return dict {acc: {name: str, gbk_id: int, seq: str, seq_date:str } }
+    Return dict {acc: {db_id: int, name: str, seq: str, seq_date:str } }
     """
     with Session(bind=connection) as session:
         db_uniprot_records = session.query(Uniprot).all()
 
     uniprot_table_dict = {}  # {acc: {name: str, gbk_id: int, seq: str, seq_date:str } }
 
     for record in tqdm(db_uniprot_records, desc="Retrieving existing UniProt records from db"):
         uniprot_table_dict[record.uniprot_accession] = {
+            "db_id": record.uniprot_id,
             "name": record.uniprot_name,
-            "genbank_id": record.genbank_id,
             "seq": record.sequence,
             "seq_date": record.seq_update_date,
         }
     
     return uniprot_table_dict
 
 
@@ -505,7 +506,31 @@
 
         if gbk_acc is not None:
             db_genome_dict[gbk_acc] = {'db_id': db_id, 'gtdb_id': gtdb_id}
         if ref_acc is not None:
             db_genome_dict[ref_acc] = {'db_id': db_id, 'gtdb_id': gtdb_id}
 
     return db_genome_dict
+
+
+def get_uniprottax_table_dict(connection):
+    """Load and parse the UniprotTaxs table from the db and compile a dict {db_id: {'genus': str, 'species': str}}
+    
+    :param connection:
+    
+    Return dict {db_id: {'genus': str, 'species': str}} AND {'genus species': db id}
+    """
+    with Session(bind=connection) as session:
+        ut_table = session.query(UniprotTax).all()
+    
+    ut_dict = {}  # {db_id: {'genus': str, 'species': str}}
+    ut_tax_dict = {}  # {'genus species': db id}
+    
+    for ut_obj in ut_table:
+        ut_dict[ut_obj.uniprot_tax_id] = {
+            'genus': ut_obj.genus,
+            'species': ut_obj.species,
+        }
+
+        ut_tax_dict[f"{ut_obj.genus} {ut_obj.species}"] = ut_obj.uniprot_tax_id
+        
+    return ut_dict, ut_tax_dict
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_interface/get_data/get_taxonomies.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_interface/get_data/get_taxonomies.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     :param connection: open connection to an SQLite3 database
 
     Return dict {genbank_accession: organism}
     """
     with Session(bind=connection) as session:
         uniprt_gbk_tax_records = session.query(Uniprot, Genbank, Taxonomy).\
             join(Genbank, (Taxonomy.taxonomy_id == Genbank.taxonomy_id)).\
-            join(Uniprot, (Genbank.genbank_id == Uniprot.genbank_id)).\
+            join(Uniprot, (Genbank.uniprot_id == Uniprot.uniprot_id)).\
             all()
 
     gbk_tax_dict = {}  # {genbank_accession: organism}
 
     uniprt_tax_dict = {}  # {uniprot acc: organism}
 
     for record in uniprt_gbk_tax_records:
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/sql/sql_orm.py` & `cazy_webscraper-2.3.0/cazy_webscraper/sql/sql_orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,20 @@
 
     genbank_id = Column(Integer, primary_key=True)
     genbank_accession = Column(String, index=True)
     sequence = Column(ReString)
     seq_update_date = Column(ReString)
     taxonomy_id = Column(Integer, ForeignKey("Taxs.taxonomy_id"))
     ncbi_tax_id = Column(Integer, ForeignKey("NcbiTaxs.ncbi_tax_id"))
+    uniprot_id = Column(Integer, ForeignKey("Uniprots.uniprot_id"))
+
+    uniprot = relationship(
+        "Uniprot",
+        back_populates="genbank",
+    )
 
     ncbi_taxs = relationship(
         "NcbiTax",
         back_populates="genbanks",
     )
 
     genomes = relationship(
@@ -240,20 +246,14 @@
     pdbs = relationship(
         "Pdb",
         secondary=genbanks_pdbs,
         back_populates="genbank",
         lazy="dynamic",
     )
 
-    uniprot = relationship(
-        "Uniprot",
-        back_populates="genbank",
-        # uselist=False,
-    )  # 1-1 relationship
-
     def __str__(self):
         return f"-Genbank accession={self.genbank_accession}-"
 
     def __repr__(self):
         return f"<Class GenBank acc={self.genbank_accession}>"
 
 
@@ -460,22 +460,23 @@
     __tablename__ = "Uniprots"
 
     __table_args__ = (
         UniqueConstraint("uniprot_accession",),
         Index("uniprot_option", "uniprot_id", "uniprot_accession")
     )
 
-    genbank_id = Column(Integer, ForeignKey('Genbanks.genbank_id'))
     uniprot_id = Column(Integer, primary_key=True)
     uniprot_accession = Column(String)
     uniprot_name = Column(ReString)
     sequence = Column(ReString)
     seq_update_date = Column(ReString)
+    uniprot_tax_id = Column(Integer, ForeignKey("UniprotTaxs.uniprot_tax_id"))
 
     genbank = relationship("Genbank", back_populates="uniprot")
+    taxs = relationship("UniprotTax", back_populates="uniprots")
 
     def __str__(self):
         return (
             f"-Uniprot, accession={self.uniprot_accession}, name={self.uniprot_name}, "
             f"id={self.uniprot_id}-"
         )
 
@@ -483,14 +484,43 @@
         """Return string representation of source organism."""
         return(
             f"<Uniprot, accession={self.uniprot_accession}, "
             f"name={self.uniprot_name}, id={self.uniprot_id}>"
         )
 
 
+class UniprotTax(Base):
+    """Describes a NCBI Taxonomy lineage."""
+    __tablename__ = "UniprotTaxs"
+
+    uniprot_tax_id = Column(Integer, primary_key=True)
+    genus = Column(ReString)
+    species = Column(ReString)
+
+    __table_args__ = (
+        UniqueConstraint("genus", "species"),
+        Index("uniprot_tax_index", "uniprot_tax_id", "genus", "species"),
+    )
+
+    uniprots = relationship(
+        "Uniprot",
+        back_populates="taxs",
+        lazy="dynamic",
+    )
+
+    def __str__(self):
+        return f"-UniProt Tax,  genus={self.genus}, species={self.species}-"
+
+    def __repr__(self):
+        """Return string representation of UniProt Tax record."""
+        return(
+            f"<Class UniProtTax, genus={self.genus}, species={self.species}>"
+        )
+
+
 class Ec(Base):
     """Describe EC numbers."""
     __tablename__ = "Ecs"
     __table_args__ = (
         UniqueConstraint("ec_number"),
     )
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parse_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parse_configuration/cazy_class_synonym_dict.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parse_configuration/cazy_class_synonym_dict.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/__init__.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/api_parser.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/api_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/cazy_webscraper_parser.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/cazy_webscraper_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         description="Scrapes the CAZy database",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     parser.add_argument(
         "email",
         type=str,
+        nargs='?',
         help="User email address. Requirement of Entrez, used to get source organsism data. Email is not stored be cazy_webscraper."
     )
 
     # Add optional arguments to parser
 
     # Add option to specify path to configuration file
     parser.add_argument(
@@ -192,14 +193,21 @@
         "--nodelete",
         dest="nodelete",
         action="store_true",
         default=False,
         help="When called, content in the existing out dir is NOT deleted",
     )
 
+    parser.add_argument(
+        "--ncbi_batch_size",
+        type=int,
+        default=200,
+        help="Number of genbank accessions in each NCBI Taxonomy db batch query"
+    )
+
     # Add option to not delete content in the existing cache dir
     parser.add_argument(
         "--nodelete_cache",
         dest="nodelete_cache",
         action="store_true",
         default=False,
         help="When called, content in the existing cache dir is NOT deleted",
@@ -218,14 +226,26 @@
         "-r",
         "--retries",
         type=int,
         default=10,
         help="Number of times to retry scraping a family or class page if error encountered",
     )
 
+    parser.add_argument(
+        "--skip_ncbi_tax",
+        dest="skip_ncbi_tax",
+        action="store_true",
+        default=False,
+        help=(
+            "Skip retrieving the latest tax classification from the NCBI Taxonomy db for proteins\n"
+            "listed with multiple taxs in CAZy.\n"
+            "For these proteins the first taxonomy listed in CAZy is added to the local CAZyme db"
+        ),
+    )
+
     # Add option to force file over writting
     parser.add_argument(
         "--sql_echo",
         dest="sql_echo",
         action="store_true",
         default=False,
         help="Set SQLite engine echo to True (SQLite will print its log messages)",
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/extract_seq_parser.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/extract_seq_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/gbk_seq_parser.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/gbk_seq_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/get_genomes_parser.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/get_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/get_gtdb_parser.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/get_gtdb_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/pdb_strctre_parser.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/pdb_strctre_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/tax_ncbi_parser.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/tax_ncbi_parser.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper/utilities/parsers/uniprot_parser.py` & `cazy_webscraper-2.3.0/cazy_webscraper/utilities/parsers/uniprot_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,27 +58,20 @@
 
     parser.add_argument(
         "database",
         type=Path,
         help="Path to local CAZyme database"
     )
 
-    parser.add_argument(
-        "email",
-        type=str,
-        metavar="user email address",
-        help="User email address, requirement of NCBI-Entrez",
-    )
-
     # Add optional arguments to parser
     parser.add_argument(
         "--bioservices_batch_size",
         type=int,
-        default=150,
-        help="Batch size for queries parsed by bioservices to UniProt to retrieve protein data"
+        default=1000,
+        help="Batch size for queries parsed by bioservices to the UniProt REST API to retrieve protein data"
     )
 
     parser.add_argument(
         "--cache_dir",
         type=Path,
         default=None,
         help="Target path for cache dir to be used instead of default path",
@@ -107,33 +100,14 @@
         type=Path,
         metavar="config file",
         default=None,
         help="Path to configuration file. Default: None, scrapes entire database",
     )
 
     parser.add_argument(
-        "--delete_old_ec",
-        dest="delete_old_ec",
-        action="store_true",
-        default=False,
-        help=(
-            "Delete EC number-GenBank relationships/annotations\n"
-            "that are not longer listed in UniProt for a given protein"
-        ),
-    )
-
-    parser.add_argument(
-        "--delete_old_pdbs",
-        dest="delete_old_pdbs",
-        action="store_true",
-        default=False,
-        help="Delete PDB accessions that are not longer listed in UniProt for a given protein",
-    )
-
-    parser.add_argument(
         "-e",
         "--ec",
         dest="ec",
         action="store_true",
         default=False,
         help="Retrieve EC numbers from UniProt",
     )
@@ -166,15 +140,14 @@
     parser.add_argument(
         "--genbank_accessions",
         type=Path,
         default=None,
         help="Path to a text file containing a list of GenBank accessions to retrieve data for",
     )
 
-
     # Add option to restrict scrape to specific genera
     parser.add_argument(
         "--genera",
         type=str,
         default=None,
         help="Genera to UniProt data for"
     )
@@ -244,26 +217,14 @@
         help=(
             "Retrieve protein Aa sequences from UniProt for records that do NOT\n"
             "have a sequence in the local CAZyme database"
         ),
     )
 
     parser.add_argument(
-        "--seq_update",
-        dest="seq_update",
-        action="store_true",
-        default=False,
-        help=(
-            "Retrieve protein Aa sequences from UniProt for records and overwrite the existing\n"
-            "sequence in the local CAZyme database if a newer sequence is retireved from UniProt"
-        ),
-    )
-
-
-    parser.add_argument(
         "--skip_download",
         dest="skip_download",
         action="store_true",
         default=False,
         help="Skip downloading data from UniProt. Use when only using data from cache",
     )
 
@@ -292,44 +253,100 @@
         default=None,
         help=(
             "Specific strains of organisms to UniProt data for "
             "(written as Genus Species Strain)"
         ),
     )
 
-    # Add option to define time out limit for trying to connect to CAZy
     parser.add_argument(
         "-t",
+        "--taxonomy",
+        dest="taxonomy",
+        action="store_true",
+        default=False,
+        help="Retrieve the taxonomic classifications (scientific name: 'genus speices')",
+    )
+
+    # Add option to define time out limit for trying to connect to CAZy
+    parser.add_argument(
         "--timeout",
         type=int,
         default=45,
         help="Connection timeout limit (seconds)"
     )
 
     parser.add_argument(
-        "--use_uniprot_cache",
-        type=Path,
-        default=None,
-        help="Path to a JSON file containing data previously retrieved from UniProt by cazy_webscraper",
-    )  
+        "--update_name",
+        dest="update_name",
+        action="store_true",
+        default=False,
+        help=(
+            "Update protein name in local CAZyme database Uniprots table.\n"
+            "Retrieve protein name from UniProt for records and overwrite the existing\n"
+            "protein name in the local CAZyme database if a new/different name is retireved from UniProt"
+        ),
+    )
 
     parser.add_argument(
-        "--uniprot_batch_size",
-        type=int,
-        default=150,
-        help="Batch size for queries sent to the UniProt REST API to retrieved UniProt accessions"
+        "--update_seq",
+        dest="update_seq",
+        action="store_true",
+        default=False,
+        help=(
+            "Update sequences in local CAZyme database Uniprots table\n"
+            "Retrieve protein Aa sequences from UniProt for records and overwrite the existing\n"
+            "sequence in the local CAZyme database if a newer sequence is retireved from UniProt"
+        ),
     )
 
     parser.add_argument(
-        "--ncbi_batch_size",
-        type=int,
-        default=150,
-        help="Batch size for queries sent to NCBI Entrez to retrieve protein accessions for gene names retrieved from UniProt"
+        "--delete_old_ec_relationships",
+        dest="delete_old_ec_relationships",
+        action="store_true",
+        default=False,
+        help=(
+            "Delete Genbank-EC number relationships for those proteins for whom data is downloaded from UniProt\n"
+            "and which are not included in the EC numbers listed for the respective protein reocrd in UniProt"
+        ),
+    )
+
+    parser.add_argument(
+        "--delete_old_ecs",
+        dest="delete_old_ecs",
+        action="store_true",
+        default=False,
+        help="Delete EC numbers that are not linked to any proteins listed in the Genbanks table.",
     )
 
+    parser.add_argument(
+        "--delete_old_pdb_relationships",
+        dest="delete_old_pdb_relationships",
+        action="store_true",
+        default=False,
+        help=(
+            "Delete Genbank-PDB relationships for those proteins for whom data is downloaded from UniProt\n"
+            "and which are not included in the PDB accessions listed for the respective protein reocrd in UniProt"
+        ),
+    )
+
+    parser.add_argument(
+        "--delete_old_pdbs",
+        dest="delete_old_pdbs",
+        action="store_true",
+        default=False,
+        help="Delete PDB accessions that are no longer linked to any records in the Genbanks table",
+    )
+
+    parser.add_argument(
+        "--use_uniprot_cache",
+        type=Path,
+        default=None,
+        help="Path to a JSON file containing data previously retrieved from UniProt by cazy_webscraper",
+    )  
+
     # Add option for more detail (verbose) logging
     parser.add_argument(
         "-v",
         "--verbose",
         dest="verbose",
         action="store_true",
         default=False,
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper.egg-info/PKG-INFO` & `cazy_webscraper-2.3.0/cazy_webscraper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazy-webscraper
-Version: 2.2.8
+Version: 2.3.0
 Summary: A tool to automate retrieving data from CAZy, build a local CAZyme SQL database, and throughly interrogating the data. Also, automate retrieving protein data, sequences, EC numbers and structure files for specific datasets in the CAZyme database from UniProt, GenBank and PDB.
 Home-page: https://github.com/HobnobMancer/cazy_webscraper
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein webscraper
 Platform: Posix
@@ -31,40 +31,39 @@
 [![codecov](https://codecov.io/gh/HobnobMancer/cazy_webscraper/branch/master/graph/badge.svg)](https://codecov.io/gh/HobnobMancer/cazy_webscraper)
 [![Documentation Status](https://readthedocs.org/projects/cazy-webscraper/badge/?version=latest)](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest)  
 [![Anaconda-Server Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/version.svg)](https://anaconda.org/bioconda/cazy_webscraper)
 [![Anaconda-Update Badge](https://anaconda.org/bioconda/cazy_webscraper/badges/latest_release_date.svg)](https://anaconda.org/bioconda/cazy_webscraper)  
 [![pyani PyPi version](https://img.shields.io/pypi/v/cazy_webscraper "PyPI version")](https://pypi.python.org/pypi/cazy_webscraper)  
 [![Downloads](https://pepy.tech/badge/cazy-webscraper)](https://pepy.tech/project/cazy-webscraper)
 
--------------------------------
-
-> `cazy_webscraper` version 1 is depracted. Please ensure you are using version 2 or newer.  
-> `bioconda` installation is fixed for >= v2.1.3.1
+--------------------------------
 
 ## cazy_webscraper
 
 `cazy_webscraper` is an application and Python3 package for the automated retrieval of protein data from the [CAZy](http://wwww.cazy.org/) database. The code is distributed under the MIT license.
+The full documentation can be found at [Read the Docs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
 
 **`cazy_webscraper` retrieves protein data from the [CAZy database](https://www.cazy.org) and stores the data in a local SQLite3 database.** This enables users to integrate the dataset into analytical pipelines, and interrogate the data in a manner unachievable through the CAZy website.
 
 **Data can be retrieved for user defined datasets of interest.** `cazy_webscraper` can recover specified CAZy Classes and/or CAZy families. These queries can be filtered by taxonomy at Kingdoms, genus, species or strain level. Successive CAZy queries can be collated into a single local database. A log of each query is recorded in the database for transparency, reproducibility and shareablity.
 
 **Using the `expand` subcommand, a user can expand the core dataset.** Specifically, `cazy_webscraper` can be used to retrieve data from the following external databases for CAZymes in the local CAZyme database that meet user specified criteria, and adds the downloaded data to the local CAZyme database:
 
 **[GenBank](https://www.ncbi.nlm.nih.gov/genbank/):**  
 - Protein sequences 
 - Latest taxonomic classification - including complete lineage (including phylum, class, order and family) (version >=2.1.2)
 - Latest genomic assembly data (GenBank and RefSeq (when available) version accession and ID numbers) (version >=2.1.3)
 
-**[UniProt](https://www.uniprot.org/):**  
+**[UniProt](https://www.uniprot.org/):** 
+- UniProt ID/accession
 - Protein name
-- UniProt accession
 - EC numbers
 - PDB accessions
-- Protein sequences
+- Protein sequence (and date sequence was last updated)
+- Taxonomic classification (genus and species)
 
 **[Research Collaboratory for Structural Bioinformatics (RCSB) Protein Data Bank (PDB)](https://www.rcsb.org/):**
 - Protein structure files
 - *Structure files are written to disk, **not** stored in the local CAZyme database*
 
 **[Genome Taxonomy Database (GTDB)](https://gtdb.ecogenomic.org/):**
 Retrieve the latest archaeal and bacterial taxonomic classifications (including complete lineages from kingdom to species) - available in `cazy_webscraper` verion >= 2.2.0.
@@ -76,20 +75,64 @@
 - A FASTA file per extracted protein sequence
 - A local BLASTP database
 
 **The `cazy_webscraper` API facilitates interoggating the local CAZyme database.**
 
 Please see the [full documentation at ReadTheDocs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
 
+## Updates
+
+**New in version 2.3.0**
+* Downloading protein data from UniProt is several magnitudes faster than before - and should have fewer issues with using older version of `bioservices`
+    - Uses `bioservices` mapping to map directly from NCBI protein version accession to UniProt
+    - `cw_get_uniprot_data` not longer calls to NCBI and thus no longer requires an email address as a positional argument
+* Updated database schema: Changed `Genbanks 1--* Uniprots` to `Genbanks *--1 Uniprots`. `Uniprots.uniprot_id` is now listed in the `Genbanks` table, instead of listing `Genbanks.genbank_id` in the `Uniprots` table
+
+* Retrieve taxonomic classifications from UniProt
+    * Use the `--taxonomy`/`-t` flag to retrieve the scientific name (genus and species) for proteins of interest
+    * Adds downloaded taxonomic information to the `UniprotsTaxs` table
+
+* Improved clarrification of deleting old records when using `cw_get_uniprot_data`
+    - Separate arguments to delete Genbanks-EC number and Genbanks-PDB accession relationships that are no longer listed in UniProt for those proteins in the local CAZyme database for proteins whom data is downloaded from UniProt
+    - New args:
+        - `--delete_old_ec_relationships` = deletes Genbank(protein)-EC number relationships no longer in UniProt
+        - `--delete_old_ecs` = deletes EC numbers in the local db not linked to any proteins
+        - `--delete_old_pdb_relationships` = deletes Genbank(protein)-PDB relationships no longer in UniProt
+        - `--delete_old_pdbs` = deletes PDB accessions in the local db not linked to any proteins
+
+* Retrieve the local db schema
+    - New command `cw_get_db_schema` added.
+    - Retrieves the SQLite schema of a local CAZyme database and prints it to the terminal
+
+* Added option to skip retrieving the latest taxonomic classifications NCBI taxonomies
+    - By default, when retreiving data from CAZy, `cazy_webscraper` retrieves the latest taxonomic classifications for proteins listed under multiple tax
+    - To increase scrapping time, and to reduce burden on the NCBI-Entrez server, if this data is not needed (e.g. GTDB taxs will be use) this step can be skipped by using the new `--skip_ncbi_tax` flag.
+    - When skipping retrieval of the latest taxa classifications from NCBI, `cazy_webscraper` will add the first taxa retrieved from CAZy for those proteins listed under mutliple taxa
+
+
 ## Documentation
 
+The full documentation can be found at [Read the Docs](https://cazy-webscraper.readthedocs.io/en/latest/?badge=latest).
+
+### Our paper: Implementation and demonstration of use
+
 For a full description of the operation and examples of use, please see our paper in (BioRxiv)[https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full].
 
 > Hobbs, E. E. M., Gloster, T. M., and Pritchard, L. (2022) 'cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets', _bioRxiv_, [https://doi.org/10.1101/2022.12.02.518825](https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1.full)
 
+### Database structure
+
+You can view the database schema [here](#database-schema) and find a PDF of the database schema [here](https://hobnobmancer.github.io/cazy_webscraper/database_schema.pdf).
+
+## Contributions
+
+We welcome contributions and suggestions. You can raise issues at this repository, or fork the repository and submit pull requests, at the links below:
+
+- [Issues](https://github.com/HobnobMancer/cazy_webscraper/issues)
+- [Pull Requests](https://github.com/HobnobMancer/cazy_webscraper/pulls)
 
 ## Table of Contents
 <!-- TOC -->
 - [`cazy_webscraper`](#cazy_webscraper)
 - [Citation](#citation)
 - [Best practice](#best-practice)
 - [Documentation](#documentation)
@@ -114,24 +157,24 @@
 - [Retrieving GTDB taxonomies](#retrieving-gtdb-taxonomies)
     - [Configuring retrieving GTDB taxonomies](#configuring-retrieving-gtdb-taxonomies)
 - [The `cazy_webscraper` API or Interrogating the local CAZyme database](#the_cazy_webscraper_api_or_interrogating_the_local_cazyme_database)
 - [Configuring `cazy_webscraper` using a YAML file](#configuring-using-a-yaml-file)
 - [CAZy coverage of GenBank](#cazy-coverage-of-genbank)
     - [Configure calculating CAZy coverage of GenBank](#configure-calculating-cazy-coverage-of-genbank)
 - [Integrating a local CAZyme database](#integrating-a-local-cazyme-database)
+- [Database schema](#database-schema)
 - [Contributions](#contributions)
 - [License and copyright](#license-and-copyright)
 <!-- /TOC -->
 
 
 ## Features in the pipeline:
 - Retrieve and stored PubMed IDs in the local CAZyme database
 - Fix any remaining bugs we can find (if you find a bug, please report it and provide as detailed bug report as possible!)
-- Update the unit tests to work with the new `cazy_webscraper` architecture
-- Update the documentation
+- Increase unit test coverage
 - Automate analysing the taxonomic distribution across CAZy and datasets of interest, including generating a final report
 
 ## Citation
 
 If you use `cazy_webscraper`, please cite the following publication:
 
 > Hobbs, E. E. M., Gloster, T. M., and Pritchard, L. (2022) 'cazy_webscraper: local compilation and interrogation of comprehensive CAZyme datasets', _bioRxiv_, [https://doi.org/10.1101/2022.12.02.518825](https://www.biorxiv.org/content/10.1101/2022.12.02.518825v1)
@@ -190,21 +233,29 @@
 ```
 
 ### Version and citation
 
 To retrieve the version, use the following command:
 
 ```bash
-cazy_webscraper <user_email> -V
+cazy_webscraper -V
+```
+or
+```bash
+cazy_webscraper --version
 ```
 
 To retrieve the citation to use:
 
 ```bash
-cazy_webscraper <user_email> -C
+cazy_webscraper -C
+```
+or
+```bash
+cazy_webscraper --citation
 ```
 
 ### Command summary
 
 Below are the list of commands (excluding required and optional arguments) included in `cazy_webscraper`.
 
 #### CAZy
@@ -236,19 +287,35 @@
 
 **Note:** PDB structure files are retrieved for the PDB accessions that are *in* a local CAZyme database created using `cazy_webscraper`. A freshly built CAZyme database only contains NCBI protein accessions, taxonomic kingdoms, source organisms, and CAZy family annotations. Therefore, the `cw_get_uniprot_data` command must be used to retrieve PDB accessions from the UniProt database **prior** to using the `cw_get_pdb_structures` command.
 
 #### Interrogate the database
 
 To interrogate the database, use the `cw_query_database` command.
 
+### Local CAZyme database schema
+
+The schema of a local CAZyme database can be retrieved using `cazy_webscraper`:
+
+```bash
+cw_get_db_schema <path to local CAZyme database>
+```
+
+Alternatively, `sqlite3` can be used to retrieve the schema:
+```bash
+sqlite3 <path to local CAZyme database> .schema
+```
+
+A visual representation of the db schema when using `cazy_webscraper` version >= 2.3.0 can be found [here](https://hobnobmancer.github.io/cazy_webscraper/database_schema.pdf).
+
 ## Creating a local CAZyme database
 Command line options for `cazy_webscraper`, which is used to scrape CAZy and compile a local SQLite database. 
 Options are written in alphabetical order.
 
 `email` - \[REQUIRED\] User email address. This is required by NCBI Entrez for querying the Entrez server.
+**Email address is not required when printing out the citation and version number information**
 
 `--cache_dir` - Path to cache dir to be used instead of default cache dir path.
 
 `--cazy_data` - Path to a txt file downloaded from CAZy containing a CAZy db data dump.
 
 `--cazy_synonyms` - Path to a JSON file containing accepted CAZy class synonsyms if the default are not sufficient.
 
@@ -278,20 +345,24 @@
 
 `--log`, `-l` - Target path to write out a log file. If not called, no log file is written. Default: None (no log file is written out).
 
 `--nodelete`, `-n` - When called content in an existing output directory is not deleted.
 
 __When the `--db_output` flag is used, `cazy_webscraper` will create any necessary parent directories. If the direct/immediate parent directory of the database exists, by default `cazy_webscraper` will delete the content in this parent directory._
 
+`--ncbi_batch_size` - The number of protein IDs submitted per batch to NCBI, when retrieving taxonomic classifications. Default 200.
+
 `--nodelete_cache` - When called, content in the existing cache dir will **not** be deleted. Default: False (existing content is deleted).
 
 `--nodelete_log` - When called, content in the existing log dir will **not** be deleted. Default: False (existing content is deleted).
 
 `--retries`, `-r` - Define the number of times to retry making a connection to CAZy if the connection should fail. Default: 10.
 
+`--skip-ncbi_tax` - Skip retrieving the latest taxonomic information for NCBI were multiple taxonomic classifications are retrieved from CAZy for a protein. The first taxonomy retrieved from CAZy will be added to the local CAZyme database. Default False - the first taxon listed for each protein is added to the local CAZyme database.
+
 `--sql_echo` - Set SQLite engine echo parameter to True, causing SQLite to print log messages. Default: False.
 
 `--subfamilies`, `-s` - Enable retrival of CAZy subfamilies, otherwise **only** CAZy family annotations will be retrieved. Default: False.
 
 `--species` - List of species written as Genus Species) to restrict the scraping of CAZymes to. CAZymes will be retrieved for **all** strains of each given species.
 
 `--strains` - List of specific species strains to restrict the scraping of CAZymes to.
@@ -337,41 +408,33 @@
 
 `cazy_webscraper` always retrieves the UniProt accession and protein name, but the retrieval of PDB accession, EC numbers and protein sequences is optional.
 
 Data can be retrieived for all proteins in the local CAZyme database, or a specific subset. CAZy class, CAZy family, genus, species, strains, kingdom and EC number filters can be defined in order to define a dataset to retrieve protein data for.
 
 To retrieve all UniProt data for all proteins in a local CAZyme datbase, using the following command:
 ```bash
-cw_get_uniprot_data <path_to_local_CAZyme_db> <user_email> --ec --pdb --sequence
+cw_get_uniprot_data <path_to_local_CAZyme_db> --ec --pdb --sequence
 ```
 
 ### Configuring UniProt data retrieval
 
 Below are listed the command-line flags for configuring the retrieval of UniProt data.
 
 `database` - \[REQUIRED\] Path to a local CAZyme database to add UniProt data to.
 
-`email` - \[REQUIRED\] User email address. This is required by NCBI Entrez for querying the Entrez server.
-
-`--ncbi_batch_size` - Size of batch query posted to NCBI Entrez. Default 150.
-
-`--uniprot_batch_size` - Change the query batch size submitted via [`bioservices`](https://bioservices.readthedocs.io/en/master/) to UniProt to retrieve protein data. Default is 150. `bioservices` recommands queries not larger than 200 objects.
+`--bioservices_batch_size` - Change the query batch size submitted via [`bioservices`](https://bioservices.readthedocs.io/en/master/) to UniProt to retrieve protein data. Default is 1000. See the [UniProt REST API documentation](https://www.uniprot.org/help/id_mapping) for batch size limits.
 
 `--cache_dir` - Path to cache dir to be used instead of default cache dir path.
 
 `--cazy_synonyms` - Path to a JSON file containing accepted CAZy class synonsyms if the default are not sufficient.
 
 `--classes` - List of classes to retrieve UniProt data for.
 
 `--config`, `-c` - Path to a configuration YAML file. Default: None.
 
-`--delete_old_ec` - Boolean, delete EC number - Protein relationships that are no longer listed in UniProt, i.e. an EC number annotation is no longer included in UniProt but is in the local database. If set to TRUE these relationships will be DELETED from the database.
-
-`--delete_old_pdbs` - Boolean, delete PDB accessions - Protein relationships that are no longer listed in UniProt, i.e. an PDB accessions that are no longer included in UniProt but is in the local database. If set to TRUE these relationships will be DELETED from the database.
-
 `--ec`, `-e` - Enable retrieval of EC number annotations from UniProt
 
 `--ec_filter` - Limist retrieval of protein data to proteins annotated with a provided list of EC numbers. Separate the EC numbers bu single commas without spaces. Recommend to wrap the entire str in quotation marks, for example:
 ```bash
 cw_get_uniprot_data my_cazyme_db/cazyme_db.db --ec_filter 'EC1.2.3.4,EC2.3.1.-'
 ```
 
@@ -393,36 +456,60 @@
 
 `--nodelete_log` - When called, content in the existing log dir will **not** be deleted. Default: False (existing content is deleted).
 
 `--pdb`, `-p` - Enable retrieval of PDB accessions. Default, PDB accessions not retrieved.
 
 `--retries`, `-r` - Define the number of times to retry making a connection to CAZy if the connection should fail. Default: 10.
 
+`--delete_old_ec_relationships` - Boolean, delete old Genbanks-EC number relationships - For those proteins in the local db for whom data is downloaded from UniProt, compare the current links between the proteins in the Genbanks table and EC numbers in the Ecs table. Delete Genbanks-Ecs relationships that are not longer listed in the respective protein records in UniProt.
+
+`--delete_old_ecs` - Boolean, delete EC number - Delete EC numbers that are not linked to any proteins listed in the Genbanks table. These can arise from multiple retrievals of data from the UniProt data over a period of time during UniProt records have been updated.
+
+`--delete_old_pdb_relationships` - Boolean, delete old Genbanks-PDB relationships - For those proteins in the local db for whom data is downloaded from UniProt, compare the current links between the proteins in the Genbanks table and PDB accessions in the Pdbs table. Delete Genbanks-Pdbs relationships that are not longer listed in the respective protein records in UniProt.
+
+`--delete_old_pdbs` - Boolean, delete PDB accessions - Protein relationships that are no longer listed in UniProt, i.e. an PDB accessions that are no longer included in UniProt but is in the local database. If set to TRUE these relationships will be DELETED from the database.
+
 `--use_uniprot_cache` - Path to a JSON file, keyed by UniProt accessions/IDs and valued by dicts containing `{'gbk_acc': str, 'db_id': int}`. This file part of the cache created by `cw_get_uniprot_data`. This is option to skip retrieving the UniProt IDs for a set of GenBank accessions, if retrieving data for the same dataset (this save a lot of time!)
 
 `skip_download` - Bool, default False. If set to True, only uses data from UniProt cache and will not download new data from UniProt.
 
 `--sequence`, `-s` - Retrieve protein amino acid sequences from UniProt
 
-`--seq_update` - If a newer version of the protein sequence is available, overwrite the existing sequence for the protein in the database. Default is false, the protein sequence is **not** overwritten and updated.
-
 `--sql_echo` - Set SQLite engine echo parameter to True, causing SQLite to print log messages. Default: False.
 
 `--species` - List of species written as Genus Species) to restrict the scraping of CAZymes to. CAZymes will be retrieved for **all** strains of each given species.
 
 `--strains` - List of specific species strains to restrict the scraping of CAZymes to.
 
-`--timeout`, `-t` - Connection timout limit (seconds). Default: 45.
+`--taxonomy`, `-t` - Retrieve taxonomic classifications (genus species) and add to the local CAZyme database
+
+`--timeout` - Connection timout limit (seconds). Default: 45.
+
+`--update_name` - If a newer version of the protein name is available, overwrite the existing name for the protein in the database. Default is false, the protein name is **not** overwritten and updated.
+
+`--update_seq` - If a newer version of the protein sequence is available, overwrite the existing sequence for the protein in the database. Default is false, the protein sequence is **not** overwritten and updated.
 
 `--use_uniprot_cache` - Path to JSON file containing data previosuly retrieved from UniProt by `cazy_webscraper`, use if an error occurred while adding the data to the local CAZyme database. This will skip the retrieval of data from UniProt, and the cached data will be added to the local CAZyme database. This can also be shared with others to add the same data to their local CAZyme database.
 
 `--uniprot_batch_size` - Size of an individual batch query submitted to the [UniProt REST API](https://www.uniprot.org/help/programmatic_access) to retrieve the UniProt accessions of proteins identified by the GenBank accession. Default is 150. The UniProt API documentation recommands batch sizes of less than 20,000 but batch sizes of 1,000 often result in HTTP 400 errors. It is recommend to keep batch sizes less than 1,000, and ideally less than 200.
 
 `--verbose`, `-v` - Enable verbose logging. This does not set the SQLite engine `echo` parameter to True. Default: False.
 
+**UniProt batch sizes:**
+Note that according to Uniprot (June 2022), there are various limits on ID Mapping Job Submission:
+
+========= =====================================================================================
+Limit	  Details
+========= =====================================================================================
+100,000	  Total number of ids allowed in comma separated param ids in /idmapping/run api
+500,000	  Total number of "mapped to" ids allowed
+100,000	  Total number of "mapped to" ids allowed to be enriched by UniProt data
+10,000	  Total number of "mapped to" ids allowed with filtering
+========= =====================================================================================
+
 ### UniProt data retrieval cache
 
 - The tables retrieved from UniProt are converted to dataframes, and written out as CSV files in the cache directory
 - The parsed UniProt data as a single JSON file
 
 ## Retrieveing protein seqences from GenBank
 
@@ -1020,15 +1107,15 @@
 
 For configuring the retrieval of data from UniProt, GenBank and PDB (_but not CAZy) the additional `ec` tag can be included to limit the retrieval of data to proteins annotated with specific EC numbers.
 
 When listing EC numbers, the 'EC' prefix can be included or excluded. For example, 'EC1.2.3.4' and '1.2.3.4' are accepted. Additionally, both dashes ('-') and astrixes ('*') can be used to represent missing digits, both '1.2.3.-' and '1.2.3.\*' are accepted.
 
 `cazy_webscraper` performs a direct EC number comparison. Therefore, supplying `cazy_webscraper` with the EC number EC1.2.3.- will only retrieve protein specifically annotated with EC1.2.3.-. `cazy_webscraper` will **not** retrieve proteins will all completed EC numbers under EC1.2.3.-, thus, `cazy_webscraper` will **not** retrieve data for proteins annotated with EC1.2.3.1, EC1.2.3.2, EC1.2.3.3, etc.
 
-Example configuration files, and an empty configuraiton file template are located in the [`config_files`]() directory of this repo.
+Example configuration files, and an empty configuraiton file template are located in the `configuration_files/` directory of this repo.
 
 
 ## Integrating a local CAZyme database
 
 `cazy_webscraper` compiles data downloaded from external databases into a local SQLite3 database.
 
 To facilitate integratting the local CAZyme database into third-party `Python` applications, use the `get_db_connection` function from `cazy_webscraper`, which will return an open connection to the CAZyme database from `sqlalchemy`.
@@ -1041,14 +1128,20 @@
 - Bool to reflect if a new database. Default is `False`, i.e. connecting to an existing local CAZyme database
 
 Import the function into the `Python` script using:
 ```python
 from cazy_webscraper.sql.sql_orm import get_db_connection
 ```
 
+## Database Schema
+
+This is the structure of the local SQLite3 database compiled by `cazy_webscraper` version >=2.3.0:
+
+![database schema](assets/cazy_webscraper_v2.3+.svg "database schema")
+
 
 ## Contributions
 
 We welcome contributions and suggestions. You can raise issues at this repository, or fork the repository and submit pull requests, at the links below:
 
 - [Issues](https://github.com/HobnobMancer/cazy_webscraper/issues)
 - [Pull Requests](https://github.com/HobnobMancer/cazy_webscraper/pulls)
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper.egg-info/SOURCES.txt` & `cazy_webscraper-2.3.0/cazy_webscraper.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 cazy_webscraper.egg-info/SOURCES.txt
 cazy_webscraper.egg-info/dependency_links.txt
 cazy_webscraper.egg-info/entry_points.txt
 cazy_webscraper.egg-info/requires.txt
 cazy_webscraper.egg-info/top_level.txt
 cazy_webscraper/api/__init__.py
 cazy_webscraper/api/cw_query_database.py
+cazy_webscraper/cache/__init__.py
+cazy_webscraper/cache/cazy.py
+cazy_webscraper/cache/ncbi.py
+cazy_webscraper/cache/uniprot.py
 cazy_webscraper/cazy/__init__.py
 cazy_webscraper/crawler/__init__.py
 cazy_webscraper/crawler/get_validation_data.py
 cazy_webscraper/expand/__init__.py
 cazy_webscraper/expand/extract_seqs/__init__.py
 cazy_webscraper/expand/extract_seqs/extract_db_seqs.py
 cazy_webscraper/expand/genbank/__init__.py
@@ -35,23 +39,25 @@
 cazy_webscraper/ncbi/gene_names/__init__.py
 cazy_webscraper/ncbi/genomes/__init__.py
 cazy_webscraper/ncbi/sequences/__init__.py
 cazy_webscraper/ncbi/taxonomy/__init__.py
 cazy_webscraper/ncbi/taxonomy/lineage.py
 cazy_webscraper/ncbi/taxonomy/multiple_taxa.py
 cazy_webscraper/sql/__init__.py
+cazy_webscraper/sql/get_schema.py
 cazy_webscraper/sql/sql_orm.py
 cazy_webscraper/sql/sql_interface/__init__.py
 cazy_webscraper/sql/sql_interface/add_data/__init__.py
 cazy_webscraper/sql/sql_interface/add_data/add_cazyme_data.py
 cazy_webscraper/sql/sql_interface/add_data/add_genbank_data.py
 cazy_webscraper/sql/sql_interface/add_data/add_genome_data.py
 cazy_webscraper/sql/sql_interface/add_data/add_gtdb_tax.py
 cazy_webscraper/sql/sql_interface/add_data/add_ncbi_tax_data.py
 cazy_webscraper/sql/sql_interface/add_data/add_uniprot_data.py
+cazy_webscraper/sql/sql_interface/delete_data/__init__.py
 cazy_webscraper/sql/sql_interface/get_data/__init__.py
 cazy_webscraper/sql/sql_interface/get_data/get_api_data.py
 cazy_webscraper/sql/sql_interface/get_data/get_assemblies.py
 cazy_webscraper/sql/sql_interface/get_data/get_records.py
 cazy_webscraper/sql/sql_interface/get_data/get_selected_gbks.py
 cazy_webscraper/sql/sql_interface/get_data/get_selected_pdbs.py
 cazy_webscraper/sql/sql_interface/get_data/get_table_dicts.py
@@ -62,14 +68,15 @@
 cazy_webscraper/utilities/parsers/__init__.py
 cazy_webscraper/utilities/parsers/api_parser.py
 cazy_webscraper/utilities/parsers/cazy_webscraper_parser.py
 cazy_webscraper/utilities/parsers/extract_seq_parser.py
 cazy_webscraper/utilities/parsers/gbk_seq_parser.py
 cazy_webscraper/utilities/parsers/get_genomes_parser.py
 cazy_webscraper/utilities/parsers/get_gtdb_parser.py
+cazy_webscraper/utilities/parsers/get_schema_parser.py
 cazy_webscraper/utilities/parsers/pdb_strctre_parser.py
 cazy_webscraper/utilities/parsers/tax_ncbi_parser.py
 cazy_webscraper/utilities/parsers/uniprot_parser.py
 tests/test_add_cazymes.py
 tests/test_api.py
 tests/test_cazy_init.py
 tests/test_crawler.py
```

### Comparing `cazy_webscraper-2.2.8/cazy_webscraper.egg-info/entry_points.txt` & `cazy_webscraper-2.3.0/cazy_webscraper.egg-info/entry_points.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [console_scripts]
 cazy_webscraper = cazy_webscraper.cazy_scraper:main
 cw_extract_db_seqs = cazy_webscraper.expand.extract_seqs.extract_db_seqs:main
+cw_get_db_schema = cazy_webscraper.sql.get_schema:main
 cw_get_genbank_seqs = cazy_webscraper.expand.genbank.sequences.get_genbank_sequences:main
 cw_get_genomics = cazy_webscraper.expand.genbank.genomes.get_genome_accs:main
 cw_get_gtdb_taxs = cazy_webscraper.expand.gtdb.get_gtdb_tax:main
 cw_get_ncbi_taxs = cazy_webscraper.expand.genbank.taxonomy.get_ncbi_taxs:main
 cw_get_pdb_structures = cazy_webscraper.expand.pdb.get_pdb_structures:main
 cw_get_uniprot_data = cazy_webscraper.expand.uniprot.get_uniprot_data:main
 cw_query_database = cazy_webscraper.api.cw_query_database:main
```

### Comparing `cazy_webscraper-2.2.8/setup.py` & `cazy_webscraper-2.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 # get long description from README.md
 with Path("README.md").open("r") as long_description_handle:
     long_description = long_description_handle.read()
 
 
 setuptools.setup(
     name="cazy_webscraper",
-    version="2.2.8",
+    version="2.3.0",
     # Metadata
     author="Emma E. M. Hobbs",
     author_email="eemh1@st-andrews.ac.uk",
     description="".join(
         [
             (
                 "A tool to automate retrieving data from CAZy, "
@@ -80,26 +80,28 @@
             "cw_get_ncbi_taxs = cazy_webscraper.expand.genbank.taxonomy.get_ncbi_taxs:main",
             "cw_get_genomics = cazy_webscraper.expand.genbank.genomes.get_genome_accs:main",
             "cw_get_gtdb_taxs = cazy_webscraper.expand.gtdb.get_gtdb_tax:main",
             "cw_get_uniprot_data = cazy_webscraper.expand.uniprot.get_uniprot_data:main",
             "cw_extract_db_seqs = cazy_webscraper.expand.extract_seqs.extract_db_seqs:main",
             "cw_get_pdb_structures = cazy_webscraper.expand.pdb.get_pdb_structures:main",
             "cw_query_database = cazy_webscraper.api.cw_query_database:main",
+            "cw_get_db_schema = cazy_webscraper.sql.get_schema:main",
         ]
     },
     install_requires=[
-        "biopython>=1.76",
-        "bioservices>=1.10.4",
+        "biopython",
+        "bioservices>=1.11.0",
         "mechanicalsoup",
-        "pandas>=1.0.3",
+        "pandas",
         "pyyaml",
         "requests",
-        "saintBioutils>=0.0.24",
+        "saintBioutils>=0.0.25",
         "sqlalchemy==1.4.20",
         "tqdm",
+        "html5lib",
     ],
     packages=setuptools.find_packages(),
     package_data={
         "Conda microenvironment": ["environment.yml"],
         "CAZy dictionary": ["cazy_dictionary.json"],
         "Configuration file": ["scraper_config.yaml"],
     },
```

### Comparing `cazy_webscraper-2.2.8/tests/test_add_cazymes.py` & `cazy_webscraper-2.3.0/tests/test_add_cazymes.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             'genus species': {'tax_id': 1, 'kingdom_id': 1},
         }
 
     def mock_return_none(*args, **kwards):
         return
 
     cazy_data = {
-        'gbk1': {'kingdom': 'k', 'organism': ('genus species',), 'families': {
+        'gbk1': {'kingdom': 'k', 'organism': 'genus species', 'families': {
                 'fam': {'subfam'},
                 'fam1': {None},
             }
         }
     }
     connection = None
```

### Comparing `cazy_webscraper-2.2.8/tests/test_api.py` & `cazy_webscraper-2.3.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_crawler.py` & `cazy_webscraper-2.3.0/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_cw_init.py` & `cazy_webscraper-2.3.0/tests/test_cw_init.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_expand.py` & `cazy_webscraper-2.3.0/tests/test_expand.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_extract_seqs.py` & `cazy_webscraper-2.3.0/tests/test_extract_seqs.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_get_ncbi_tax.py` & `cazy_webscraper-2.3.0/tests/test_get_ncbi_tax.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_gtdb.py` & `cazy_webscraper-2.3.0/tests/test_gtdb.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_ncbi.py` & `cazy_webscraper-2.3.0/tests/test_ncbi.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_ncbi_genomes.py` & `cazy_webscraper-2.3.0/tests/test_ncbi_genomes.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_orm.py` & `cazy_webscraper-2.3.0/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_parse_config.py` & `cazy_webscraper-2.3.0/tests/test_parse_config.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_parsers.py` & `cazy_webscraper-2.3.0/tests/test_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 def test_parser_uniprot():
     """Test building the parser when argsv is None"""
     uniprot_parser.build_parser()
 
 
 def test_parser_arsv_uniprot():
     """Test building the parser when argsv is not None"""
-    uniprot_parser.build_parser(["dbpath", "dummy_email"])
+    uniprot_parser.build_parser(["dbpath"])
 
 
 def test_parser_ncbi_tax():
     """Test building the parser when argsv is None"""
     tax_ncbi_parser.build_parser()
```

### Comparing `cazy_webscraper-2.2.8/tests/test_pdb.py` & `cazy_webscraper-2.3.0/tests/test_pdb.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_sql_ad_genbank.py` & `cazy_webscraper-2.3.0/tests/test_sql_ad_genbank.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     def mock_gbk_table_seq_dict(*args, **kwards):
         return {
             'gbk1': {'sequence': None, 'seq_date': None},
             'gbk2': {'sequence': 'AAAAAA', 'seq_date': '2022-11-01'},
         }
 
     monkeypatch.setattr(add_genbank_data, "get_gbk_table_seq_dict", mock_gbk_table_seq_dict)
-
+    Path("tests/test_outputs/test_outputs_sql").mkdir(exist_ok=True)
     cache_dir = Path("tests/test_outputs/test_outputs_sql/temp_dir")
     cache_dir.mkdir(exist_ok=True, parents=True)
 
     add_genbank_data.add_gbk_seqs_to_db(
         seq_dict,
         retrieval_data,
         gbk_dict,
```

### Comparing `cazy_webscraper-2.2.8/tests/test_sql_ad_genomes.py` & `cazy_webscraper-2.3.0/tests/test_sql_ad_genomes.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_sql_ad_gtdb.py` & `cazy_webscraper-2.3.0/tests/test_sql_ad_gtdb.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_sql_ad_ncbi_tax.py` & `cazy_webscraper-2.3.0/tests/test_sql_ad_ncbi_tax.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_sql_interf_gd_get_records.py` & `cazy_webscraper-2.3.0/tests/test_sql_interf_gd_get_records.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_sql_interf_gd_get_tax.py` & `cazy_webscraper-2.3.0/tests/test_sql_interf_gd_get_tax.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_sql_interface.py` & `cazy_webscraper-2.3.0/tests/test_sql_interface.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_table_dicts.py` & `cazy_webscraper-2.3.0/tests/test_table_dicts.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_taxonomy.py` & `cazy_webscraper-2.3.0/tests/test_taxonomy.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,36 +45,38 @@
 """
 
 
 import logging
 import pytest
 
 from argparse import Namespace
+from collections import namedtuple
 
 from cazy_webscraper.ncbi.taxonomy import multiple_taxa
 
 
 @pytest.fixture
 def cazy_data():
+    TaxData = namedtuple('Tax', ['kingdom', 'organism'])
     data = {
-        "gbk1": {"kingdom": {'Bacteria'}, "organism": {"sp 1", "sp 2"}, "families": {'GH1', 'GH2'}},
-        "gbk2": {"kingdom": {'Bacteria'}, "organism": {"sp 1", "sp 2"}, "families": {'GH1', 'GH2'}},
-        "gbk3": {"kingdom": {'Bacteria'}, "organism": {"sp 1", "sp 2"}, "families": {'GH1', 'GH2'}},
-        "gbk4": {"kingdom": {'Bacteria'}, "organism": {"sp 1", "sp 2"}, "families": {'GH1', 'GH2'}},
+        "gbk1": {"kingdom": {'Bacteria'}, "taxonomy": {TaxData('king1', 'sp2'), TaxData('king2', 'sp2')}, "families": {'GH1', 'GH2'}},
+        "gbk2": {"kingdom": {'Bacteria'}, "taxonomy": {TaxData('king2', 'sp2'), TaxData('king2', 'sp2')}, "families": {'GH1', 'GH2'}},
+        "gbk3": {"kingdom": {'Bacteria'}, "taxonomy": {TaxData('king3', 'sp2'), TaxData('king2', 'sp2')}, "families": {'GH1', 'GH2'}},
+        "gbk4": {"kingdom": {'Bacteria'}, "taxonomy": {TaxData('king1', 'sp2'), TaxData('king2', 'sp2')}, "families": {'GH1', 'GH2'}},
     }
     return data
 
 
 def test_id_multi_tax(cazy_data):
     """Test identify_multiplpe_taxa"""
     logger = logging.getLogger(__name__)
 
     returned_list = multiple_taxa.identify_multiple_taxa(cazy_data, logger)
 
-    assert len(returned_list) == 4
+    assert len(returned_list) == 3
 
 
 def test_select_first_organism(cazy_data):
     """Test select_first_organism()"""
     logger = logging.getLogger(__name__)
 
     multiple_taxa.select_first_organism(cazy_data, ['gbk1', 'gbk2', 'gbk3', 'gbk4'], logger)
@@ -105,14 +107,16 @@
 
     multiple_taxa.replace_multiple_tax_with_invalid_ids(cazy_data, gbk_accs, logger, "args")
 
 
 def test_get_ncbi_tax(monkeypatch):
     argsdict = {"args": Namespace(
         retries=10,
+        skip_ncbi_tax=True,
+        ncbi_batch_size=200,
     )}
 
     entrez_result = "tests/test_inputs/test_inputs_ncbi_tax/entrezProt.xml"
 
     with open(entrez_result, "rb") as fh:
         result = fh
 
@@ -120,24 +124,26 @@
             """Mocks call to Entrez."""
             return result
 
         monkeypatch.setattr(multiple_taxa, "entrez_retry", mock_entrez_tax_call)
 
         output = multiple_taxa.get_ncbi_tax(
             {"WebEnv": 1, "QueryKey": 2},
-            {'CAA35997.1': {'kingdom': {'kingdom'}, 'organism': {'organism'}}},
+            {'CAA35997.1': {'kingdom': {'kingdom'}, 'taxonomy': {'Bos taurus'}}},
             logging.getLogger(__name__),
             argsdict['args'],
         )
-        assert output == {'CAA35997.1': {'kingdom': {'Eukaryota'}, 'organism': {'Bos taurus'}}}
+        assert output == {'CAA35997.1': {'kingdom': 'Eukaryota', 'taxonomy': {'Bos taurus'}, 'organism': 'Bos taurus'}}
 
 
 def test_get_ncbi_tax_fails(monkeypatch):
     argsdict = {"args": Namespace(
         retries=10,
+        skip_ncbi_tax=True,
+        ncbi_batch_size=200,
     )}
 
     def mock_entrez_tax_call(*args, **kwargs):
         """Mocks call to Entrez."""
         return
 
     monkeypatch.setattr(multiple_taxa, "entrez_retry", mock_entrez_tax_call)
@@ -150,14 +156,16 @@
     )
 
 
 def test_failed_replace_tax(monkeypatch):
     """Test replace_multiple_tax when failes to conenct to NCBI.Entrez"""
     argsdict = {"args": Namespace(
         retries=10,
+        skip_ncbi_tax=True,
+        ncbi_batch_size=200,
     )}
 
     def mock_return_none(*args, **kwards):
         return None
 
     def mock_select_org(*args, **kwards):
         return {}
@@ -168,14 +176,16 @@
     multiple_taxa.replace_multiple_tax({}, "gk1", logging.getLogger(__name__), argsdict["args"], [])
 
 
 def test_failed_replace_tax_run_time(monkeypatch):
     """Test replace_multiple_tax when failes to conenct to NCBI.Entrez"""
     argsdict = {"args": Namespace(
         retries=10,
+        skip_ncbi_tax=True,
+        ncbi_batch_size=200,
     )}
 
     def mock_error(*args, **kwards):
         raise RuntimeError
 
     def mock_select_org(*args, **kwards):
         return {}
```

### Comparing `cazy_webscraper-2.2.8/tests/test_uniprot.py` & `cazy_webscraper-2.3.0/tests/test_uniprot.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 from cazy_webscraper import utilities
 from cazy_webscraper.cazy_scraper import connect_existing_db
 from cazy_webscraper.expand.uniprot import get_uniprot_data
 from cazy_webscraper.ncbi.gene_names import get_linked_ncbi_accessions
 from cazy_webscraper.sql import sql_interface
 from cazy_webscraper.sql.sql_interface.add_data import add_uniprot_data
-from cazy_webscraper.sql.sql_interface.get_data import get_selected_gbks
+from cazy_webscraper.sql.sql_interface.get_data import get_selected_gbks, get_table_dicts
 from cazy_webscraper.utilities.parsers import uniprot_parser
 
 
 
 @pytest.fixture
 def mock_building_parser(*args, **kwargs):
     parser_args = ArgumentParser(
@@ -104,29 +104,34 @@
             get_pages=True,
             kingdoms=None,
             log=None,
             nodelete=False,
             output=None,
             retries=10,
             sequence=True,
-            seq_update=True,
+            update_seq=True,
             subfamilies=True,
             species=None,
             strains=None,
             streamline=None,
             timeout=45,
             uniprot_accessions=None,
             uniprot_batch_size=150,
             uniprot_data=None,
             verbose=False,
             pdb=True,
             skip_uniprot_accessions=None,
             use_uniprot_cache=None,
             email="dummy_email",
+            taxonomy=True,
             skip_download=False,
+            delete_old_ec_relationships=True,
+            delete_old_ecs=True,
+            delete_old_pdb_relationships=True,
+            delete_old_pdbs=True,
         )
         return parser
 
     def mock_return_none(*args, **kwargs):
         return
 
     def mock_connect_existing_db(*args, **kwards):
@@ -135,21 +140,22 @@
     def mock_get_expansion_configuration(*args, **kwards):
         return config_dict, set(), set(), set(), dict(), set()
 
     def mock_get_genbank_accessions(*args, **kwards):
         return {1: 1, 2:2, 3:3}
     
     def mock_get_uniprot_data(*args, **kwards):
-        return (
-            {
-                1: {'genbank_accession': 1, 'gene_name': 1, 'ec': {1,2,3}, 'pdb': {1,2,3}},
-                2: {'gene_name': 'nan', 'ec': {1,2,3}, 'pdb': {1,2,3}}, 3: {'ec': {1,2,3}, 'pdb': {1,2,3}}
-            },
-            {1, 2, 3}
-        )
+        return  {'ncbi_acc': {
+            'uniprot_acc': 'uniprot_acc',
+            'uniprot_entry_id': 'uniprot_entry_id',
+            'protein_name': 'protein_name',
+            'ec_numbers': {'ec_numbers'},
+            'sequence': 'sequence',
+            'pdbs': {'all_pdbs'},
+        }}
 
     def mock_uniprot_data(*args, **kwards):
         return {
                 1: {'genbank_accession': 1, 'gene_name': 1, 'ec': {1,2,3}, 'pdb': {1,2,3}},
                 2: {'gene_name': 'nan', 'ec': {1,2,3}, 'pdb': {1,2,3}}, 3: {'ec': {1,2,3}, 'pdb': {1,2,3}}
             }
     
@@ -158,28 +164,31 @@
     monkeypatch.setattr(saint_logger, "config_logger", mock_return_logger)
     monkeypatch.setattr(get_uniprot_data, "connect_existing_db", mock_connect_existing_db)
     monkeypatch.setattr("cazy_webscraper.expand.uniprot.get_uniprot_data.make_output_directory", mock_return_none)
     monkeypatch.setattr(get_uniprot_data, "get_expansion_configuration", mock_get_expansion_configuration)
     monkeypatch.setattr(sql_interface, "log_scrape_in_db", mock_return_none)
     monkeypatch.setattr(get_selected_gbks, "get_genbank_accessions", mock_get_genbank_accessions)
     monkeypatch.setattr(get_uniprot_data, "get_uniprot_accessions", mock_get_genbank_accessions)
+    monkeypatch.setattr(get_uniprot_data, "add_uniprot_genbank_relationships", mock_return_none)
     monkeypatch.setattr(get_uniprot_data, "get_uniprot_data", mock_get_uniprot_data)
-    monkeypatch.setattr(get_uniprot_data, "get_gene_names", mock_get_uniprot_data)
-    monkeypatch.setattr(get_uniprot_data, "get_mapped_genbank_accessions", mock_uniprot_data)
-    monkeypatch.setattr(get_uniprot_data, "get_linked_ncbi_accessions", mock_get_uniprot_data)
     monkeypatch.setattr(get_uniprot_data, "add_uniprot_accessions", mock_return_none)
     monkeypatch.setattr(get_uniprot_data, "add_ec_numbers", mock_return_none)
+    monkeypatch.setattr(get_uniprot_data, "add_genbank_ec_relationships", mock_return_none)
+    monkeypatch.setattr(get_uniprot_data, "delete_old_relationships", mock_return_none)
+    monkeypatch.setattr(get_uniprot_data, "delete_old_annotations", mock_return_none)
     monkeypatch.setattr(get_uniprot_data, "add_pdb_accessions", mock_return_none)
+    monkeypatch.setattr(get_uniprot_data, "add_pdb_gbk_relationships", mock_return_none)
+    monkeypatch.setattr(get_uniprot_data, "delete_old_annotations", mock_return_none)
+    monkeypatch.setattr(get_uniprot_data, "delete_old_relationships", mock_return_none)
+    monkeypatch.setattr(get_uniprot_data, "add_uniprot_taxs", mock_return_none)
     monkeypatch.setattr(cazy_webscraper, "closing_message", mock_return_none)
 
+    monkeypatch.setattr(get_table_dicts, "get_ec_table_dict", mock_get_genbank_accessions)
+    monkeypatch.setattr(get_table_dicts, "get_ec_gbk_table_dict", mock_get_genbank_accessions)
+    monkeypatch.setattr(get_table_dicts, "get_pdb_table_dict", mock_get_genbank_accessions)
+    monkeypatch.setattr(get_table_dicts, "get_gbk_pdb_table_dict", mock_get_genbank_accessions)
+
     output = test_dir / "test_outputs" / "test_outputs_uniprot"
     output.mkdir(parents=True, exist_ok=True)
     get_uniprot_data.main()
     shutil.rmtree((test_dir / "test_outputs" / "test_outputs_uniprot"))
     output.mkdir(parents=True, exist_ok=True)
-
-
-def test_ec_num_cache():
-    """Test get_ecs_from_cache()"""
-    uniprot_dict = {'acc1': {'ec': []}, 'acc2': {'ec': ['1.2.3.4', '4.2.5.6']}, 'acc3': {1: 2}}
-
-    get_uniprot_data.get_ecs_from_cache(uniprot_dict)
```

### Comparing `cazy_webscraper-2.2.8/tests/test_utilities.py` & `cazy_webscraper-2.3.0/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_validation_data.py` & `cazy_webscraper-2.3.0/tests/test_validation_data.py`

 * *Files identical despite different names*

### Comparing `cazy_webscraper-2.2.8/tests/test_webscraper.py` & `cazy_webscraper-2.3.0/tests/test_webscraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,15 @@
 
 def test_main_citation(mock_building_parser, mock_config_logger, monkeypatch):
     """Test main() with args.citation"""
 
     def mock_parser(*args, **kwargs):
         parser = Namespace(
             email="dummy@domain.com",
+            skip_ncbi_tax=False,
             cache_dir=None,
             cazy_data=None,
             cazy_synonyms=None,
             classes=None,
             config=None,
             citation=True,
             db_output=None,
@@ -240,14 +241,15 @@
     """Test main() with args.version"""
 
     def mock_parser(*args, **kwargs):
         parser = Namespace(
             email="dummy@domain.com",
             cache_dir=None,
             cazy_data=None,
+            skip_ncbi_tax=False,
             cazy_synonyms=None,
             classes=None,
             config=None,
             citation=False,
             db_output=None,
             database=None,
             delete_old_relationships=False,
@@ -283,14 +285,15 @@
 
     def mock_parser(*args, **kwargs):
         parser = Namespace(
             email="dummy@domain.com",
             cache_dir=None,
             cazy_data=None,
             cazy_synonyms=None,
+            skip_ncbi_tax=False,
             classes=None,
             config=None,
             citation=False,
             db_output=None,
             database=None,
             delete_old_relationships=False,
             force=False,
@@ -325,14 +328,15 @@
 
     def mock_parser(*args, **kwargs):
         parser = Namespace(
             email="dummy@domain.com",
             cache_dir=None,
             cazy_data=None,
             cazy_synonyms=None,
+            skip_ncbi_tax=False,
             classes=None,
             config=None,
             citation=False,
             db_output=Path('database.db'),
             database=Path('database.db'),
             delete_old_relationships=False,
             force=False,
@@ -372,14 +376,15 @@
             email="dummy@domain.com",
             cache_dir=None,
             cazy_data=None,
             cazy_synonyms=None,
             classes=None,
             config=None,
             citation=False,
+            skip_ncbi_tax=False,
             db_output=Path(db_path),  ###
             database=None,
             delete_old_relationships=False,
             force=True,   ###
             families=None,
             genera=None,
             kingdoms=None,
@@ -428,14 +433,15 @@
     def mock_parser(*args, **kwargs):
         parser = Namespace(
             email="dummy@domain.com",
             cache_dir=None,
             cazy_data=Path('cazy_data.json'),
             cazy_synonyms=None,
             classes=None,
+            skip_ncbi_tax=False,
             config=None,
             citation=False,
             db_output=Path(db_path),  ###
             database=None,
             delete_old_relationships=False,
             force=False,   ###
             families=None,
@@ -492,14 +498,15 @@
     def mock_parser(*args, **kwargs):
         parser = Namespace(
             email="dummy@domain.com",
             cache_dir='cache',
             cazy_data=None,
             cazy_synonyms=None,
             classes=None,
+            skip_ncbi_tax=False,
             config=None,
             citation=False,
             db_output=None,
             database=Path(db_path),  ###
             delete_old_relationships=False,
             force=False,
             families=None,
@@ -574,14 +581,15 @@
             config=None,
             citation=False,
             db_output=Path(db_path),  ###
             database=None,
             delete_old_relationships=False,
             force=False,
             families=None,
+            skip_ncbi_tax=False,
             genera=None,
             kingdoms=None,
             log=None,
             nodelete=False,
             nodelete_cache=False,
             nodelete_log=False,
             retries=10,
@@ -703,14 +711,17 @@
 
     def mock_return_logger(*args, **kwards):
         return logging.getLogger('mock_logger')
 
     def mock_return_none(*args, **kwards):
         return
 
+    def mock_tax_dict(*args, **kwargs):
+        return {}, {}
+
     def mock_multiple_taxa(*args, **kwards):
         return [1,2,3,4]
 
     def mock_replace_taxa(*args, **kwards):
         return [], True
 
     def mock_cazy_data(*args, **kwargs):
@@ -718,15 +729,15 @@
 
     monkeypatch.setattr(cazy_scraper, "build_logger", mock_return_logger)
     monkeypatch.setattr(cazy_scraper, "get_validation_data", mock_return_none)
     monkeypatch.setattr(cazy_scraper, "get_cazy_txt_file_data", mock_multiple_taxa)
     monkeypatch.setattr(cazy_scraper, "parse_all_cazy_data", mock_cazy_data)
     monkeypatch.setattr(cazy_scraper, "identify_multiple_taxa", mock_multiple_taxa)
     monkeypatch.setattr(cazy_scraper, "replace_multiple_tax", mock_replace_taxa)
-    monkeypatch.setattr(cazy_scraper, "build_taxa_dict", mock_return_none)
+    monkeypatch.setattr(cazy_scraper, "build_taxa_dict", mock_tax_dict)
     monkeypatch.setattr(add_cazyme_data, "add_kingdoms", mock_return_none)
     monkeypatch.setattr(add_cazyme_data, "add_source_organisms", mock_return_none)
     monkeypatch.setattr(add_cazyme_data, "add_cazy_families", mock_return_none)
     monkeypatch.setattr(add_cazyme_data, "add_genbanks", mock_return_none)
     monkeypatch.setattr(add_cazyme_data, "add_genbank_fam_relationships", mock_return_none)
 
     cazy_scraper.get_cazy_data(
@@ -735,15 +746,15 @@
         cazy_synonym_dict,
         empty_config_dict,
         set(),
         set(),
         set(),
         set(),
         'connection',
-        Path('cache_dir'),
+        Path('tests/test_outputs/test_webscraper/test_logs'),
         'logger_name',
         'time_stamp',
         argsdict['args'],
     )
 
 
 def test_term_message():
```

