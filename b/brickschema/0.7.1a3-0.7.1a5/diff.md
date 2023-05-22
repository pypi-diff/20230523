# Comparing `tmp/brickschema-0.7.1a3.tar.gz` & `tmp/brickschema-0.7.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brickschema-0.7.1a3.tar", max compression
+gzip compressed data, was "brickschema-0.7.1a5.tar", max compression
```

## Comparing `brickschema-0.7.1a3.tar` & `brickschema-0.7.1a5.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1945 2021-07-23 15:38:20.787312 brickschema-0.7.1a3/LICENSE
--rw-r--r--   0        0        0     9176 2022-04-20 15:03:17.894671 brickschema-0.7.1a3/README.md
--rw-r--r--   0        0        0      530 2022-11-28 02:31:26.511103 brickschema-0.7.1a3/brickschema/__init__.py
--rw-r--r--   0        0        0      608 2020-11-10 06:11:23.496242 brickschema-0.7.1a3/brickschema/abbrmap.py
--rw-r--r--   0        0        0     2548 2022-11-20 19:44:54.915817 brickschema-0.7.1a3/brickschema/bacnet.py
--rw-r--r--   0        0        0     3572 2020-08-13 17:55:40.988282 brickschema-0.7.1a3/brickschema/bin/brick_validate.py
--rw-r--r--   0        0        0      145 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/__init__.py
--rw-r--r--   0        0        0       49 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/__main__.py
--rw-r--r--   0        0        0     4572 2022-02-24 17:03:40.701252 brickschema-0.7.1a3/brickschema/brickify/main.py
--rw-r--r--   0        0        0       45 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/__init__.py
--rw-r--r--   0        0        0     5890 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/Handler.py
--rw-r--r--   0        0        0     3755 2022-11-28 02:31:26.511103 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/HaystackHandler.py
--rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/__init__.py
--rw-r--r--   0        0        0     2511 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/analogy.ttl
--rw-r--r--   0        0        0     3952 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/haystack.json
--rw-r--r--   0        0        0     1577 2022-11-26 22:16:16.811116 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/HaystackRDFInferenceSession.py
--rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/__init__.py
--rw-r--r--   0        0        0     4339 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/RACHandler/RACHandler.py
--rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/RACHandler/__init__.py
--rw-r--r--   0        0        0     7715 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/RACHandler/conversions/rac.yml
--rw-r--r--   0        0        0     4557 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/TableHandler.py
--rw-r--r--   0        0        0       74 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/__init__.py
--rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/src/handlers/__init__.py
--rw-r--r--   0        0        0     6458 2021-06-10 16:16:30.295261 brickschema-0.7.1a3/brickschema/brickify/util.py
--rw-r--r--   0        0        0    23674 2023-03-29 17:17:46.145912 brickschema-0.7.1a3/brickschema/graph.py
--rw-r--r--   0        0        0    29028 2022-11-28 02:31:26.511103 brickschema-0.7.1a3/brickschema/inference.py
--rw-r--r--   0        0        0    14793 2022-11-28 02:31:26.511103 brickschema-0.7.1a3/brickschema/merge.py
--rw-r--r--   0        0        0     1949 2022-11-28 02:31:26.511103 brickschema-0.7.1a3/brickschema/namespaces.py
--rw-r--r--   0        0        0    33869 2021-03-03 20:58:32.139966 brickschema-0.7.1a3/brickschema/ontologies/1.1/Brick-VBIS-alignment.ttl
--rw-r--r--   0        0        0   540042 2021-08-06 17:41:07.025117 brickschema-0.7.1a3/brickschema/ontologies/1.1/Brick.ttl
--rw-r--r--   0        0        0     6480 2021-03-03 20:58:32.143966 brickschema-0.7.1a3/brickschema/ontologies/1.1/BrickShape.ttl
--rw-r--r--   0        0        0    72272 2021-03-03 20:58:32.143966 brickschema-0.7.1a3/brickschema/ontologies/1.1/taglookup.pickle
--rw-r--r--   0        0        0   334070 2021-03-03 20:58:32.143966 brickschema-0.7.1a3/brickschema/ontologies/1.1/vbis-masterlist.csv
--rw-r--r--   0        0        0    40592 2021-03-03 20:58:32.143966 brickschema-0.7.1a3/brickschema/ontologies/1.2/Brick-VBIS-alignment.ttl
--rw-r--r--   0        0        0   777615 2022-11-20 19:44:54.919817 brickschema-0.7.1a3/brickschema/ontologies/1.2/Brick.ttl
--rw-r--r--   0        0        0     5682 2021-03-03 20:58:32.151966 brickschema-0.7.1a3/brickschema/ontologies/1.2/BrickShape.ttl
--rw-r--r--   0        0        0     3799 2022-11-20 19:44:28.855622 brickschema-0.7.1a3/brickschema/ontologies/1.2/alignments/Brick-BOT-alignment.ttl
--rw-r--r--   0        0        0     4235 2022-11-20 19:44:28.851622 brickschema-0.7.1a3/brickschema/ontologies/1.2/alignments/Brick-REC-alignment.ttl
--rw-r--r--   0        0        0    25987 2022-11-20 19:44:28.851622 brickschema-0.7.1a3/brickschema/ontologies/1.2/alignments/Brick-VBIS-alignment.ttl
--rw-r--r--   0        0        0  1013502 2021-11-09 22:15:04.147911 brickschema-0.7.1a3/brickschema/ontologies/1.2/extensions/brick_extension_bacnet.ttl
--rw-r--r--   0        0        0   630955 2022-11-20 19:44:54.919817 brickschema-0.7.1a3/brickschema/ontologies/1.2/extensions/brick_extension_shacl_tag_inference.ttl
--rw-r--r--   0        0        0    72063 2022-11-21 22:27:04.539761 brickschema-0.7.1a3/brickschema/ontologies/1.2/taglookup.pickle
--rw-r--r--   0        0        0   334070 2021-03-03 20:58:32.155966 brickschema-0.7.1a3/brickschema/ontologies/1.2/vbis-masterlist.csv
--rw-r--r--   0        0        0  1601690 2022-11-28 02:31:26.515103 brickschema-0.7.1a3/brickschema/ontologies/1.3/Brick.ttl
--rw-r--r--   0        0        0     3799 2022-11-28 02:31:26.515103 brickschema-0.7.1a3/brickschema/ontologies/1.3/alignments/Brick-BOT-alignment.ttl
--rw-r--r--   0        0        0     4235 2022-11-28 02:31:26.515103 brickschema-0.7.1a3/brickschema/ontologies/1.3/alignments/Brick-REC-alignment.ttl
--rw-r--r--   0        0        0    25987 2022-11-28 02:31:26.515103 brickschema-0.7.1a3/brickschema/ontologies/1.3/alignments/Brick-VBIS-alignment.ttl
--rw-r--r--   0        0        0   695375 2022-11-28 02:31:26.519103 brickschema-0.7.1a3/brickschema/ontologies/1.3/extensions/brick_extension_shacl_tag_inference.ttl
--rw-r--r--   0        0        0    97692 2022-11-28 02:31:26.519103 brickschema-0.7.1a3/brickschema/ontologies/1.3/taglookup.pickle
--rw-r--r--   0        0        0   334070 2022-11-28 02:31:26.519103 brickschema-0.7.1a3/brickschema/ontologies/1.3/vbis-masterlist.csv
--rw-r--r--   0        0        0     8710 2022-02-24 17:03:40.705252 brickschema-0.7.1a3/brickschema/orm.py
--rw-r--r--   0        0        0    10514 2022-11-28 02:31:26.519103 brickschema-0.7.1a3/brickschema/persistent.py
--rw-r--r--   0        0        0     2852 2021-12-14 06:59:29.240496 brickschema-0.7.1a3/brickschema/tagmap.py
--rw-r--r--   0        0        0     2399 2021-08-13 03:43:10.682814 brickschema-0.7.1a3/brickschema/web/index.html
--rw-r--r--   0        0        0     2233 2022-02-24 17:03:40.705252 brickschema-0.7.1a3/brickschema/web.py
--rw-r--r--   0        0        0     2072 2023-04-28 15:27:35.311295 brickschema-0.7.1a3/pyproject.toml
--rw-r--r--   0        0        0     2807 2022-11-28 02:31:26.523104 brickschema-0.7.1a3/tests/data/badBuilding.ttl
--rw-r--r--   0        0        0      881 2022-11-28 02:31:26.523104 brickschema-0.7.1a3/tests/data/brick_inference_test.ttl
--rw-r--r--   0        0        0      318 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/RAC/README.md
--rw-r--r--   0        0        0    29696 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/RAC/rac.xls
--rw-r--r--   0        0        0     2400 2023-03-29 17:13:29.759256 brickschema-0.7.1a3/tests/data/brickify/RAC/rac.xls.brick.ttl
--rw-r--r--   0        0        0      139 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/haystack-v4/README.md
--rw-r--r--   0        0        0    49817 2023-02-06 17:25:43.296070 brickschema-0.7.1a3/tests/data/brickify/haystack-v4/charlie.ttl.brick.ttl
--rw-r--r--   0        0        0      819 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/jinja2/README.md
--rw-r--r--   0        0        0      277 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/jinja2/sheet.csv
--rw-r--r--   0        0        0     1158 2023-03-29 17:13:29.727255 brickschema-0.7.1a3/tests/data/brickify/jinja2/sheet.csv.brick.ttl
--rw-r--r--   0        0        0      902 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/jinja2/template.json
--rw-r--r--   0        0        0      846 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/jinja2/template.yml
--rw-r--r--   0        0        0      306 2021-08-13 03:43:10.686814 brickschema-0.7.1a3/tests/data/brickify/rdf/README.md
--rw-r--r--   0        0        0      339 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/rdf/input.ttl
--rw-r--r--   0        0        0      427 2023-03-29 17:13:29.719255 brickschema-0.7.1a3/tests/data/brickify/rdf/input.ttl.brick.ttl
--rw-r--r--   0        0        0      868 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/rdf/template.json
--rw-r--r--   0        0        0     1155 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/rdf/template.yml
--rw-r--r--   0        0        0      485 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/tsv/README.md
--rw-r--r--   0        0        0      103 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/tsv/sheet.tsv
--rw-r--r--   0        0        0      430 2023-03-29 17:13:29.667255 brickschema-0.7.1a3/tests/data/brickify/tsv/sheet.tsv.brick.ttl
--rw-r--r--   0        0        0      513 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/tsv/template.json
--rw-r--r--   0        0        0      527 2021-06-10 16:16:30.299261 brickschema-0.7.1a3/tests/data/brickify/tsv/template.yml
--rw-r--r--   0        0        0    23372 2019-12-11 19:58:37.625874 brickschema-0.7.1a3/tests/data/carytown.json
--rw-r--r--   0        0        0      657 2022-11-28 02:31:26.523104 brickschema-0.7.1a3/tests/data/extraOntology1.ttl
--rw-r--r--   0        0        0      657 2022-11-28 02:31:26.523104 brickschema-0.7.1a3/tests/data/extraOntology2.ttl
--rw-r--r--   0        0        0     1766 2022-11-28 02:31:26.523104 brickschema-0.7.1a3/tests/data/extraShapes.ttl
--rw-r--r--   0        0        0     1202 2021-08-06 17:41:07.033117 brickschema-0.7.1a3/tests/data/extraShapesWithExtraOnt.ttl
--rw-r--r--   0        0        0     1156 2022-11-28 02:31:26.523104 brickschema-0.7.1a3/tests/data/goodBuilding.ttl
--rw-r--r--   0        0        0      626 2021-03-03 20:58:32.159966 brickschema-0.7.1a3/tests/data/tags.ttl
--rw-r--r--   0        0        0     1236 2021-03-03 20:58:32.159966 brickschema-0.7.1a3/tests/data/test.ttl
--rw-r--r--   0        0        0      129 2021-03-03 20:58:32.159966 brickschema-0.7.1a3/tests/data/vbis_inference_test.ttl
--rw-r--r--   0        0        0    11445 1970-01-01 00:00:00.000000 brickschema-0.7.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1945 2021-07-23 15:38:20.787312 brickschema-0.7.1a5/LICENSE
+-rw-r--r--   0        0        0     9176 2023-04-28 16:26:09.527473 brickschema-0.7.1a5/README.md
+-rw-r--r--   0        0        0      530 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/__init__.py
+-rw-r--r--   0        0        0      608 2020-11-10 06:11:23.496242 brickschema-0.7.1a5/brickschema/abbrmap.py
+-rw-r--r--   0        0        0     2548 2022-11-20 19:44:54.915817 brickschema-0.7.1a5/brickschema/bacnet.py
+-rw-r--r--   0        0        0     3572 2020-08-13 17:55:40.988282 brickschema-0.7.1a5/brickschema/bin/brick_validate.py
+-rw-r--r--   0        0        0      145 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/__init__.py
+-rw-r--r--   0        0        0       49 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/__main__.py
+-rw-r--r--   0        0        0     4572 2022-02-24 17:03:40.701252 brickschema-0.7.1a5/brickschema/brickify/main.py
+-rw-r--r--   0        0        0       45 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/__init__.py
+-rw-r--r--   0        0        0     5890 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/Handler.py
+-rw-r--r--   0        0        0     3755 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/HaystackHandler.py
+-rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/__init__.py
+-rw-r--r--   0        0        0     2511 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/analogy.ttl
+-rw-r--r--   0        0        0     3952 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/haystack.json
+-rw-r--r--   0        0        0     1577 2022-11-26 22:16:16.811116 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/HaystackRDFInferenceSession.py
+-rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/__init__.py
+-rw-r--r--   0        0        0     4339 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/RACHandler.py
+-rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/__init__.py
+-rw-r--r--   0        0        0     7715 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/conversions/rac.yml
+-rw-r--r--   0        0        0     4557 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/TableHandler.py
+-rw-r--r--   0        0        0       74 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/__init__.py
+-rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/__init__.py
+-rw-r--r--   0        0        0     6458 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/util.py
+-rw-r--r--   0        0        0    23674 2023-03-29 17:17:46.145912 brickschema-0.7.1a5/brickschema/graph.py
+-rw-r--r--   0        0        0    29028 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/inference.py
+-rw-r--r--   0        0        0    14793 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/merge.py
+-rw-r--r--   0        0        0     1949 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/namespaces.py
+-rw-r--r--   0        0        0    33869 2021-03-03 20:58:32.139966 brickschema-0.7.1a5/brickschema/ontologies/1.1/Brick-VBIS-alignment.ttl
+-rw-r--r--   0        0        0   540042 2021-08-06 17:41:07.025117 brickschema-0.7.1a5/brickschema/ontologies/1.1/Brick.ttl
+-rw-r--r--   0        0        0     6480 2021-03-03 20:58:32.143966 brickschema-0.7.1a5/brickschema/ontologies/1.1/BrickShape.ttl
+-rw-r--r--   0        0        0    72272 2021-03-03 20:58:32.143966 brickschema-0.7.1a5/brickschema/ontologies/1.1/taglookup.pickle
+-rw-r--r--   0        0        0   334070 2021-03-03 20:58:32.143966 brickschema-0.7.1a5/brickschema/ontologies/1.1/vbis-masterlist.csv
+-rw-r--r--   0        0        0    40592 2021-03-03 20:58:32.143966 brickschema-0.7.1a5/brickschema/ontologies/1.2/Brick-VBIS-alignment.ttl
+-rw-r--r--   0        0        0   777615 2022-11-20 19:44:54.919817 brickschema-0.7.1a5/brickschema/ontologies/1.2/Brick.ttl
+-rw-r--r--   0        0        0     5682 2021-03-03 20:58:32.151966 brickschema-0.7.1a5/brickschema/ontologies/1.2/BrickShape.ttl
+-rw-r--r--   0        0        0     3799 2022-11-20 19:44:28.855622 brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-BOT-alignment.ttl
+-rw-r--r--   0        0        0     4235 2022-11-20 19:44:28.851622 brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-REC-alignment.ttl
+-rw-r--r--   0        0        0    25987 2022-11-20 19:44:28.851622 brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-VBIS-alignment.ttl
+-rw-r--r--   0        0        0  1013502 2021-11-09 22:15:04.147911 brickschema-0.7.1a5/brickschema/ontologies/1.2/extensions/brick_extension_bacnet.ttl
+-rw-r--r--   0        0        0   630955 2022-11-20 19:44:54.919817 brickschema-0.7.1a5/brickschema/ontologies/1.2/extensions/brick_extension_shacl_tag_inference.ttl
+-rw-r--r--   0        0        0    72063 2022-11-21 22:27:04.539761 brickschema-0.7.1a5/brickschema/ontologies/1.2/taglookup.pickle
+-rw-r--r--   0        0        0   334070 2021-03-03 20:58:32.155966 brickschema-0.7.1a5/brickschema/ontologies/1.2/vbis-masterlist.csv
+-rw-r--r--   0        0        0  1601690 2022-11-28 02:31:26.515103 brickschema-0.7.1a5/brickschema/ontologies/1.3/Brick.ttl
+-rw-r--r--   0        0        0     3799 2022-11-28 02:31:26.515103 brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-BOT-alignment.ttl
+-rw-r--r--   0        0        0     4235 2022-11-28 02:31:26.515103 brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-REC-alignment.ttl
+-rw-r--r--   0        0        0    25987 2022-11-28 02:31:26.515103 brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-VBIS-alignment.ttl
+-rw-r--r--   0        0        0   695375 2022-11-28 02:31:26.519103 brickschema-0.7.1a5/brickschema/ontologies/1.3/extensions/brick_extension_shacl_tag_inference.ttl
+-rw-r--r--   0        0        0    97692 2022-11-28 02:31:26.519103 brickschema-0.7.1a5/brickschema/ontologies/1.3/taglookup.pickle
+-rw-r--r--   0        0        0   334070 2022-11-28 02:31:26.519103 brickschema-0.7.1a5/brickschema/ontologies/1.3/vbis-masterlist.csv
+-rw-r--r--   0        0        0     8710 2022-02-24 17:03:40.705252 brickschema-0.7.1a5/brickschema/orm.py
+-rw-r--r--   0        0        0    11032 2023-05-22 23:54:32.421304 brickschema-0.7.1a5/brickschema/persistent.py
+-rw-r--r--   0        0        0     2852 2021-12-14 06:59:29.240496 brickschema-0.7.1a5/brickschema/tagmap.py
+-rw-r--r--   0        0        0     2399 2021-08-13 03:43:10.682814 brickschema-0.7.1a5/brickschema/web/index.html
+-rw-r--r--   0        0        0     2233 2022-02-24 17:03:40.705252 brickschema-0.7.1a5/brickschema/web.py
+-rw-r--r--   0        0        0     2068 2023-05-22 23:54:11.077119 brickschema-0.7.1a5/pyproject.toml
+-rw-r--r--   0        0        0     2807 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/badBuilding.ttl
+-rw-r--r--   0        0        0      881 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/brick_inference_test.ttl
+-rw-r--r--   0        0        0      318 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/RAC/README.md
+-rw-r--r--   0        0        0    29696 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/RAC/rac.xls
+-rw-r--r--   0        0        0     2400 2023-05-22 23:39:52.025722 brickschema-0.7.1a5/tests/data/brickify/RAC/rac.xls.brick.ttl
+-rw-r--r--   0        0        0      139 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/haystack-v4/README.md
+-rw-r--r--   0        0        0    49817 2023-02-06 17:25:43.296070 brickschema-0.7.1a5/tests/data/brickify/haystack-v4/charlie.ttl.brick.ttl
+-rw-r--r--   0        0        0      819 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/jinja2/README.md
+-rw-r--r--   0        0        0      277 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/jinja2/sheet.csv
+-rw-r--r--   0        0        0     1158 2023-05-22 23:39:51.989722 brickschema-0.7.1a5/tests/data/brickify/jinja2/sheet.csv.brick.ttl
+-rw-r--r--   0        0        0      902 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/jinja2/template.json
+-rw-r--r--   0        0        0      846 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/jinja2/template.yml
+-rw-r--r--   0        0        0      306 2021-08-13 03:43:10.686814 brickschema-0.7.1a5/tests/data/brickify/rdf/README.md
+-rw-r--r--   0        0        0      339 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/rdf/input.ttl
+-rw-r--r--   0        0        0      427 2023-05-22 23:39:51.921722 brickschema-0.7.1a5/tests/data/brickify/rdf/input.ttl.brick.ttl
+-rw-r--r--   0        0        0      868 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/rdf/template.json
+-rw-r--r--   0        0        0     1155 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/rdf/template.yml
+-rw-r--r--   0        0        0      485 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/tsv/README.md
+-rw-r--r--   0        0        0      103 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/tsv/sheet.tsv
+-rw-r--r--   0        0        0      430 2023-05-22 23:39:51.849721 brickschema-0.7.1a5/tests/data/brickify/tsv/sheet.tsv.brick.ttl
+-rw-r--r--   0        0        0      513 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/tsv/template.json
+-rw-r--r--   0        0        0      527 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/tsv/template.yml
+-rw-r--r--   0        0        0    23372 2019-12-11 19:58:37.625874 brickschema-0.7.1a5/tests/data/carytown.json
+-rw-r--r--   0        0        0      657 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/extraOntology1.ttl
+-rw-r--r--   0        0        0      657 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/extraOntology2.ttl
+-rw-r--r--   0        0        0     1766 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/extraShapes.ttl
+-rw-r--r--   0        0        0     1202 2021-08-06 17:41:07.033117 brickschema-0.7.1a5/tests/data/extraShapesWithExtraOnt.ttl
+-rw-r--r--   0        0        0     1156 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/goodBuilding.ttl
+-rw-r--r--   0        0        0      626 2021-03-03 20:58:32.159966 brickschema-0.7.1a5/tests/data/tags.ttl
+-rw-r--r--   0        0        0     1236 2021-03-03 20:58:32.159966 brickschema-0.7.1a5/tests/data/test.ttl
+-rw-r--r--   0        0        0      129 2021-03-03 20:58:32.159966 brickschema-0.7.1a5/tests/data/vbis_inference_test.ttl
+-rw-r--r--   0        0        0    11393 1970-01-01 00:00:00.000000 brickschema-0.7.1a5/PKG-INFO
```

### Comparing `brickschema-0.7.1a3/LICENSE` & `brickschema-0.7.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/README.md` & `brickschema-0.7.1a5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![Documentation Status](https://readthedocs.org/projects/brickschema/badge/?version=latest)](https://brickschema.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/brickschema.svg)](https://badge.fury.io/py/brickschema)
 
 Documentation available at [readthedocs](https://brickschema.readthedocs.io/en/latest/)
 
 ## Installation
 
-The `brickschema` package requires Python >= 3.6. It can be installed with `pip`:
+The `brickschema` package requires Python >= 3.8. It can be installed with `pip`:
 
 ```
 pip install brickschema
 ```
 
 The `brickschema` package offers several installation configuration options for reasoning.
 The default bundled [OWLRL](https://pypi.org/project/owlrl/) reasoner delivers correct results, but exhibits poor performance on large or complex ontologies (we have observed minutes to hours) due to its bruteforce implementation.
```

### Comparing `brickschema-0.7.1a3/brickschema/__init__.py` & `brickschema-0.7.1a5/brickschema/__init__.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/abbrmap.py` & `brickschema-0.7.1a5/brickschema/abbrmap.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/bacnet.py` & `brickschema-0.7.1a5/brickschema/bacnet.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/bin/brick_validate.py` & `brickschema-0.7.1a5/brickschema/bin/brick_validate.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/main.py` & `brickschema-0.7.1a5/brickschema/brickify/main.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/Handler.py` & `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/Handler.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/HaystackHandler.py` & `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/HaystackHandler.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/analogy.ttl` & `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/analogy.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/haystack.json` & `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/haystack.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/HaystackRDFInferenceSession.py` & `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/HaystackRDFInferenceSession.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/RACHandler/RACHandler.py` & `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/RACHandler.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/RACHandler/conversions/rac.yml` & `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/conversions/rac.yml`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/src/handlers/Handler/TableHandler.py` & `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/TableHandler.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/brickify/util.py` & `brickschema-0.7.1a5/brickschema/brickify/util.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/graph.py` & `brickschema-0.7.1a5/brickschema/graph.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/inference.py` & `brickschema-0.7.1a5/brickschema/inference.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/merge.py` & `brickschema-0.7.1a5/brickschema/merge.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/namespaces.py` & `brickschema-0.7.1a5/brickschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.1/Brick-VBIS-alignment.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.1/Brick-VBIS-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.1/Brick.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.1/Brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.1/BrickShape.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.1/BrickShape.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.1/taglookup.pickle` & `brickschema-0.7.1a5/brickschema/ontologies/1.1/taglookup.pickle`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.1/vbis-masterlist.csv` & `brickschema-0.7.1a5/brickschema/ontologies/1.1/vbis-masterlist.csv`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/Brick-VBIS-alignment.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/Brick-VBIS-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/Brick.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/Brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/BrickShape.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/BrickShape.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/alignments/Brick-BOT-alignment.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-BOT-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/alignments/Brick-REC-alignment.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-REC-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/alignments/Brick-VBIS-alignment.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-VBIS-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/extensions/brick_extension_bacnet.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/extensions/brick_extension_bacnet.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/extensions/brick_extension_shacl_tag_inference.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/extensions/brick_extension_shacl_tag_inference.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/taglookup.pickle` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/taglookup.pickle`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.2/vbis-masterlist.csv` & `brickschema-0.7.1a5/brickschema/ontologies/1.2/vbis-masterlist.csv`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.3/Brick.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.3/Brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.3/alignments/Brick-BOT-alignment.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-BOT-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.3/alignments/Brick-REC-alignment.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-REC-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.3/alignments/Brick-VBIS-alignment.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-VBIS-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.3/extensions/brick_extension_shacl_tag_inference.ttl` & `brickschema-0.7.1a5/brickschema/ontologies/1.3/extensions/brick_extension_shacl_tag_inference.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.3/taglookup.pickle` & `brickschema-0.7.1a5/brickschema/ontologies/1.3/taglookup.pickle`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/ontologies/1.3/vbis-masterlist.csv` & `brickschema-0.7.1a5/brickschema/ontologies/1.3/vbis-masterlist.csv`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/orm.py` & `brickschema-0.7.1a5/brickschema/orm.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/persistent.py` & `brickschema-0.7.1a5/brickschema/persistent.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,27 @@
             rows = conn.execute(
                 "SELECT id, timestamp from changesets "
                 "ORDER BY timestamp DESC LIMIT 1"
             )
             res = rows.fetchone()
             return res
 
+    def version_before(self, ts: str) -> str:
+        """Returns the version timestamp most immediately
+        *before* the given iso8601-formatted timestamp"""
+        with self.conn() as conn:
+            rows = conn.execute(
+                "SELECT timestamp from changesets "
+                "WHERE timestamp < ? "
+                "ORDER BY timestamp DESC LIMIT 1",
+                (ts,),
+            )
+            res = rows.fetchone()
+            return res[0]
+
     def __len__(self):
         # need to override __len__ because the rdflib-sqlalchemy
         # backend doesn't support .count() for recent versions of
         # SQLAlchemy
         return len(list(self.triples((None, None, None))))
 
     def undo(self):
@@ -121,15 +134,17 @@
         undoes the most recent changeset.
         """
         if self.latest_version is None:
             raise Exception("No changesets to undo")
         with self.conn() as conn:
             changeset_id = self.latest_version["id"]
             logger.info(f"Undoing changeset {changeset_id}")
-            self._graph_at(self, conn, self.latest_version["timestamp"])
+            self._graph_at(
+                self, conn, self.version_before(self.latest_version["timestamp"])
+            )
             conn.execute(
                 "INSERT INTO redos(id, timestamp, graph, is_insertion, triple) SELECT id, timestamp, graph, is_insertion, triple FROM changesets WHERE id = ?",
                 (changeset_id,),
             )
             conn.execute("DELETE FROM changesets WHERE id = ?", (changeset_id,))
 
     def redo(self):
@@ -271,20 +286,20 @@
         that is less than or equal to the given timestamp.
         """
         if timestamp is None:
             timestamp = datetime.now().isoformat()
 
         if graph is not None:
             rows = conn.execute(
-                "SELECT * FROM changesets WHERE graph = ? AND timestamp >= ? ORDER BY timestamp DESC",
+                "SELECT * FROM changesets WHERE graph = ? AND timestamp > ? ORDER BY timestamp DESC",
                 (graph, timestamp),
             )
         else:
             rows = conn.execute(
-                "SELECT * FROM changesets WHERE timestamp >= ? ORDER BY timestamp DESC",
+                "SELECT * FROM changesets WHERE timestamp > ? ORDER BY timestamp DESC",
                 (timestamp,),
             )
         for row in rows:
             triple = pickle.loads(row["triple"])
             if row["is_insertion"]:
                 alter_graph.add((triple[0], triple[1], triple[2]))
             else:
```

### Comparing `brickschema-0.7.1a3/brickschema/tagmap.py` & `brickschema-0.7.1a5/brickschema/tagmap.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/web/index.html` & `brickschema-0.7.1a5/brickschema/web/index.html`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/brickschema/web.py` & `brickschema-0.7.1a5/brickschema/web.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/pyproject.toml` & `brickschema-0.7.1a5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "brickschema"
-version = "0.7.1a3"
+version = "0.7.1a5"
 description = "A library for working with the Brick ontology for buildings (brickschema.org)"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 include = ["brickschema/ontologies", "tests/data", "brickschema/web"]
 homepage = "https://brickschema.org"
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 rdflib = "^6.2"
 owlrl = "^6.0"
-pytest = "^7.1"
+pytest = "^7.2"
 pyshacl = "^0.22"
 requests = "^2.25.0"
 importlib-resources = "^3.3.0"
 click-spinner = {optional = true, version="^0.1.10"}
 tabulate = {optional = true, version="^0.8.7"}
-Jinja2 = {optional = true, version="3.0.3"}
+Jinja2 = {optional = true, version="^3.1"}
 xlrd = {optional = true, version="^1.2.0"}
 PyYAML = {optional = true, version="^5.3.1"}
 typer = {optional = true, version = "^0.4.1"}
-Flask = {optional = true, version = "^2.0"}
+Flask = {optional = true, version = "^2.3"}
 colorama = {optional = true, version="^0.4.4"}
 dedupe = {optional = true, version = "^2.0"}
 reasonable = {optional = true, version="^0.2.2a4"}
 sqlalchemy = {optional = true, version="^1.4"}
 rdflib_sqlalchemy = {optional = true, version = "^0.5"}
-BAC0 = {optional = true, version = "^21.12.3"}
+BAC0 = {optional = true, version = "^22.9"}
 networkx = {optional = true, version="^2.6"}
 
 [tool.poetry.scripts]
 brick_validate = "brickschema.bin.brick_validate:main"
 brickify = "brickschema.brickify.main:app"
 
 [tool.poetry.extras]
```

### Comparing `brickschema-0.7.1a3/tests/data/badBuilding.ttl` & `brickschema-0.7.1a5/tests/data/badBuilding.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brick_inference_test.ttl` & `brickschema-0.7.1a5/tests/data/brick_inference_test.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/RAC/rac.xls` & `brickschema-0.7.1a5/tests/data/brickify/RAC/rac.xls`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/RAC/rac.xls.brick.ttl` & `brickschema-0.7.1a5/tests/data/brickify/RAC/rac.xls.brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/haystack-v4/charlie.ttl.brick.ttl` & `brickschema-0.7.1a5/tests/data/brickify/haystack-v4/charlie.ttl.brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/jinja2/README.md` & `brickschema-0.7.1a5/tests/data/brickify/jinja2/README.md`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/jinja2/sheet.csv.brick.ttl` & `brickschema-0.7.1a5/tests/data/brickify/jinja2/sheet.csv.brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/jinja2/template.json` & `brickschema-0.7.1a5/tests/data/brickify/jinja2/template.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/jinja2/template.yml` & `brickschema-0.7.1a5/tests/data/brickify/jinja2/template.yml`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/rdf/template.json` & `brickschema-0.7.1a5/tests/data/brickify/rdf/template.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/rdf/template.yml` & `brickschema-0.7.1a5/tests/data/brickify/rdf/template.yml`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/tsv/template.json` & `brickschema-0.7.1a5/tests/data/brickify/tsv/template.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/brickify/tsv/template.yml` & `brickschema-0.7.1a5/tests/data/brickify/tsv/template.yml`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/carytown.json` & `brickschema-0.7.1a5/tests/data/carytown.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/extraOntology1.ttl` & `brickschema-0.7.1a5/tests/data/extraOntology1.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/extraOntology2.ttl` & `brickschema-0.7.1a5/tests/data/extraOntology2.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/extraShapes.ttl` & `brickschema-0.7.1a5/tests/data/extraShapes.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/extraShapesWithExtraOnt.ttl` & `brickschema-0.7.1a5/tests/data/extraShapesWithExtraOnt.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/goodBuilding.ttl` & `brickschema-0.7.1a5/tests/data/goodBuilding.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/tags.ttl` & `brickschema-0.7.1a5/tests/data/tags.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/tests/data/test.ttl` & `brickschema-0.7.1a5/tests/data/test.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a3/PKG-INFO` & `brickschema-0.7.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: brickschema
-Version: 0.7.1a3
+Version: 0.7.1a5
 Summary: A library for working with the Brick ontology for buildings (brickschema.org)
 Home-page: https://brickschema.org
 License: BSD-3-Clause
 Author: Gabe Fierro
 Author-email: gtfierro@mines.edu
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: allegro
 Provides-Extra: bacnet
 Provides-Extra: brickify
 Provides-Extra: merge
 Provides-Extra: networkx
 Provides-Extra: orm
 Provides-Extra: persistence
 Provides-Extra: reasonable
 Provides-Extra: web
-Requires-Dist: BAC0 (>=21.12.3,<22.0.0) ; extra == "bacnet" or extra == "all"
-Requires-Dist: Flask (>=2.0,<3.0) ; extra == "web" or extra == "all"
-Requires-Dist: Jinja2 (==3.0.3) ; extra == "brickify" or extra == "all"
+Requires-Dist: BAC0 (>=22.9,<23.0) ; extra == "bacnet" or extra == "all"
+Requires-Dist: Flask (>=2.3,<3.0) ; extra == "web" or extra == "all"
+Requires-Dist: Jinja2 (>=3.1,<4.0) ; extra == "brickify" or extra == "all"
 Requires-Dist: PyYAML (>=5.3.1,<6.0.0) ; extra == "brickify" or extra == "all"
 Requires-Dist: click-spinner (>=0.1.10,<0.2.0) ; extra == "brickify" or extra == "all"
 Requires-Dist: colorama (>=0.4.4,<0.5.0) ; extra == "merge" or extra == "all"
 Requires-Dist: dedupe (>=2.0,<3.0) ; extra == "merge" or extra == "all"
 Requires-Dist: importlib-resources (>=3.3.0,<4.0.0)
 Requires-Dist: networkx (>=2.6,<3.0) ; extra == "networkx" or extra == "all"
 Requires-Dist: owlrl (>=6.0,<7.0)
 Requires-Dist: pyshacl (>=0.22,<0.23)
-Requires-Dist: pytest (>=7.1,<8.0)
+Requires-Dist: pytest (>=7.2,<8.0)
 Requires-Dist: rdflib (>=6.2,<7.0)
 Requires-Dist: rdflib_sqlalchemy (>=0.5,<0.6) ; extra == "persistence" or extra == "all"
 Requires-Dist: reasonable (>=0.2.2a4,<0.3.0) ; extra == "reasonable" or extra == "all"
 Requires-Dist: requests (>=2.25.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0) ; extra == "orm" or extra == "persistence" or extra == "all"
 Requires-Dist: tabulate (>=0.8.7,<0.9.0) ; extra == "brickify" or extra == "all"
 Requires-Dist: typer (>=0.4.1,<0.5.0) ; extra == "brickify" or extra == "all"
@@ -52,15 +51,15 @@
 [![Documentation Status](https://readthedocs.org/projects/brickschema/badge/?version=latest)](https://brickschema.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/brickschema.svg)](https://badge.fury.io/py/brickschema)
 
 Documentation available at [readthedocs](https://brickschema.readthedocs.io/en/latest/)
 
 ## Installation
 
-The `brickschema` package requires Python >= 3.6. It can be installed with `pip`:
+The `brickschema` package requires Python >= 3.8. It can be installed with `pip`:
 
 ```
 pip install brickschema
 ```
 
 The `brickschema` package offers several installation configuration options for reasoning.
 The default bundled [OWLRL](https://pypi.org/project/owlrl/) reasoner delivers correct results, but exhibits poor performance on large or complex ontologies (we have observed minutes to hours) due to its bruteforce implementation.
```

