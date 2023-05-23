# Comparing `tmp/cognite_neat-0.11.4.tar.gz` & `tmp/cognite_neat-0.11.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.11.4.tar", max compression
+gzip compressed data, was "cognite_neat-0.11.5.tar", max compression
```

## Comparing `cognite_neat-0.11.4.tar` & `cognite_neat-0.11.5.tar`

### file list

```diff
@@ -1,80 +1,79 @@
--rw-r--r--   0        0        0    11351 2023-05-22 13:54:44.452487 cognite_neat-0.11.4/LICENSE
--rw-r--r--   0        0        0     8748 2023-05-22 13:54:44.452487 cognite_neat-0.11.4/README.md
--rw-r--r--   0        0        0       23 2023-05-22 13:54:44.452487 cognite_neat-0.11.4/cognite/neat/__init__.py
--rw-r--r--   0        0        0      616 2023-05-22 13:54:44.452487 cognite_neat-0.11.4/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-05-22 13:54:44.452487 cognite_neat-0.11.4/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-22 13:54:44.452487 cognite_neat-0.11.4/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-05-22 13:54:44.452487 cognite_neat-0.11.4/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-05-22 13:54:44.452487 cognite_neat-0.11.4/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4623 2023-05-22 13:54:44.452487 cognite_neat-0.11.4/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    28433 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     9436 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      470 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    34283 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    16987 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     6700 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      115 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0    10647 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    12025 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    10943 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     3621 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2558 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    15521 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17630 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6183 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     3201 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     5186 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      509 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/examples/config.yaml
--rw-r--r--   0        0        0    79580 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    52178 2023-05-22 13:54:44.456487 cognite_neat-0.11.4/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-05-22 13:54:44.460487 cognite_neat-0.11.4/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1155 2023-05-22 13:54:44.460487 cognite_neat-0.11.4/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1771 2023-05-22 13:54:44.460487 cognite_neat-0.11.4/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15541 2023-05-22 13:54:44.460487 cognite_neat-0.11.4/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6763 2023-05-22 13:54:44.460487 cognite_neat-0.11.4/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0    15552 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/examples/workflows/fast_graph/workflow.py
--rw-r--r--   0        0        0     6958 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/examples/workflows/fast_graph/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4781 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    13084 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6014 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0        0 2023-05-22 13:54:44.508488 cognite_neat-0.11.4/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 13:54:44.508488 cognite_neat-0.11.4/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-05-22 13:54:44.508488 cognite_neat-0.11.4/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    18989 2023-05-22 13:54:44.508488 cognite_neat-0.11.4/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-05-22 13:54:44.508488 cognite_neat-0.11.4/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-05-22 13:54:44.508488 cognite_neat-0.11.4/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-05-22 13:54:44.508488 cognite_neat-0.11.4/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css
--rw-r--r--   0        0        0    13320 2023-05-22 13:54:44.464487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map
--rw-r--r--   0        0        0  1318896 2023-05-22 13:54:44.472487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js
--rw-r--r--   0        0        0     2667 2023-05-22 13:54:44.472487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt
--rw-r--r--   0        0        0  5708777 2023-05-22 13:54:44.504487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map
--rw-r--r--   0        0        0     2633 2023-05-22 13:54:44.504487 cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-05-22 13:54:44.508488 cognite_neat-0.11.4/cognite/neat/main.py
--rw-r--r--   0        0        0     2005 2023-05-22 13:54:44.864493 cognite_neat-0.11.4/pyproject.toml
--rw-r--r--   0        0        0     9823 1970-01-01 00:00:00.000000 cognite_neat-0.11.4/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-05-23 06:21:22.335977 cognite_neat-0.11.5/LICENSE
+-rw-r--r--   0        0        0     8748 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/README.md
+-rw-r--r--   0        0        0       23 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      616 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4670 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    28433 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     9436 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      470 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     2250 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    34295 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    16995 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     6700 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      115 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0    10647 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    12025 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    10943 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     3621 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2558 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    15521 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17630 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6183 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     3201 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     5186 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0    79580 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    52178 2023-05-23 06:21:22.339977 cognite_neat-0.11.5/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1155 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1771 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15541 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6763 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0    15552 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/fast_graph/workflow.py
+-rw-r--r--   0        0        0     6958 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/fast_graph/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4781 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    13084 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6014 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-05-23 06:21:22.379977 cognite_neat-0.11.5/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:21:22.379977 cognite_neat-0.11.5/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-05-23 06:21:22.379977 cognite_neat-0.11.5/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    18989 2023-05-23 06:21:22.379977 cognite_neat-0.11.5/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-05-23 06:21:22.379977 cognite_neat-0.11.5/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-05-23 06:21:22.379977 cognite_neat-0.11.5/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-05-23 06:21:22.379977 cognite_neat-0.11.5/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css
+-rw-r--r--   0        0        0    13320 2023-05-23 06:21:22.343977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map
+-rw-r--r--   0        0        0  1318896 2023-05-23 06:21:22.351977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js
+-rw-r--r--   0        0        0     2667 2023-05-23 06:21:22.351977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt
+-rw-r--r--   0        0        0  5708777 2023-05-23 06:21:22.375977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map
+-rw-r--r--   0        0        0     2633 2023-05-23 06:21:22.375977 cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-05-23 06:21:22.379977 cognite_neat-0.11.5/cognite/neat/main.py
+-rw-r--r--   0        0        0     2005 2023-05-23 06:21:22.647980 cognite_neat-0.11.5/pyproject.toml
+-rw-r--r--   0        0        0     9823 1970-01-01 00:00:00.000000 cognite_neat-0.11.5/PKG-INFO
```

### Comparing `cognite_neat-0.11.4/LICENSE` & `cognite_neat-0.11.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/README.md` & `cognite_neat-0.11.5/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/constants.py` & `cognite_neat-0.11.5/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/app.py` & `cognite_neat-0.11.5/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/configuration.py` & `cognite_neat-0.11.5/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.11.5/cognite/neat/core/data_classes/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 from enum import StrEnum
 from pathlib import Path
 from typing import Literal, Self
 
+import yaml
 from pydantic import BaseModel, Field, validator
 from yaml import safe_load
 
 LOG_FORMAT = "%(asctime)s.%(msecs)03d %(levelname)-8s %(message)s"
 LOG_DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
@@ -110,15 +111,16 @@
         return self.data_store_path / "source_graphs"
 
     @classmethod
     def from_yaml(cls, filepath: Path) -> Self:
         return cls(**safe_load(filepath.read_text()))
 
     def to_yaml(self, filepath: Path):
-        filepath.write_text(self.json())
+        with filepath.open("w") as f:
+            yaml.dump(self.dict(), f)
 
     @classmethod
     def from_env(cls) -> Self:
         cdf_config = ServiceClient(
             project=os.environ.get("NEAT_CDF_PROJECT"),
             client_name=os.environ.get("NEAT_CDF_CLIENT_NAME"),
             client_id=os.environ.get("NEAT_CDF_CLIENT_ID"),
```

### Comparing `cognite_neat-0.11.4/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.11.5/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.11.5/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.11.5/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.11.5/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.11.5/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -750,15 +750,15 @@
 
 def categorize_assets(
     client: CogniteClient,
     rdf_assets: dict,
     data_set_id: int,
     partitions: int = 40,
     stop_on_exception: bool = False,
-    reporting: bool = False,
+    return_report: bool = False,
 ) -> Union[tuple[dict, dict], dict]:
     """Categorize assets on those that are to be created, updated and decommissioned
 
     Parameters
     ----------
     client : CogniteClient
         Instance of CogniteClient
@@ -766,15 +766,15 @@
         Dictionary containing asset external_id - asset pairs
     data_set_id : int
         Dataset id to which assets are to be/are stored
     partitions : int, optional
         Number of partitions to use when fetching assets from CDF, by default 40
     stop_on_exception : bool, optional
         Whether to stop on exception or not, by default False
-    reporting : bool, optional
+    return_report : bool, optional
         Whether to report on the diffing results or not, by default False
 
     Returns
     -------
     Dict[str, list]
         dictionary containing asset category - list of asset pairs
     """
@@ -811,15 +811,15 @@
         "decommission": _assets_to_decommission(cdf_assets, decommission_ids),
     }
 
     categorized_assets["update"], report["update"] = _assets_to_update(
         rdf_assets, cdf_assets, update_ids, stop_on_exception=stop_on_exception
     )
 
-    return (categorized_assets, report) if reporting else categorized_assets
+    return (categorized_assets, report) if return_report else categorized_assets
 
 
 def _micro_batch_push(
     client: CogniteClient, assets: list, batch_size: int = 1000, push_type: str = "update", message: str = "Updated"
 ):
     """Updates assets in batches of 1000
```

### Comparing `cognite_neat-0.11.4/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.11.5/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
 
 
 def categorize_relationships(
     client: CogniteClient,
     rdf_relationships: pd.DataFrame,
     data_set_id: int,
     partitions: int = 40,
-    reporting: bool = False,
+    return_report: bool = False,
 ) -> Union[
     tuple[dict[str, list[Union[Relationship, RelationshipUpdate]]], dict[str, set]],
     dict[str, list[Union[Relationship, RelationshipUpdate]]],
 ]:
     """Categorize relationships on those that are to be created, decommissioned or resurrected"""
     # TODO also figure out which relationships to be deleted
 
@@ -321,15 +321,15 @@
     report = {"create": create_xids, "resurrect": resurrect_xids, "decommission": decommission_xids}
     categorized_relationships = {
         "create": _relationship_to_create(rdf_relationships[rdf_relationships.external_id.isin(create_xids)]),
         "resurrect": _relationships_to_resurrect(resurrect_xids),
         "decommission": _relationships_to_decommission(decommission_xids),
     }
 
-    return (categorized_relationships, report) if reporting else categorized_relationships
+    return (categorized_relationships, report) if return_report else categorized_relationships
 
 
 def _micro_batch_push(
     client: CogniteClient,
     relationships: list,
     batch_size: int = 1000,
     push_type: str = "update",
```

### Comparing `cognite_neat-0.11.4/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.11.5/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/loader/config.py` & `cognite_neat-0.11.5/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/loader/graph.py` & `cognite_neat-0.11.5/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.11.5/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/loader/rules.py` & `cognite_neat-0.11.5/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.11.5/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/modeler.py` & `cognite_neat-0.11.5/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.11.5/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.11.5/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/transformer.py` & `cognite_neat-0.11.5/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/utils.py` & `cognite_neat-0.11.5/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/validator.py` & `cognite_neat-0.11.5/cognite/neat/core/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/workflow/base.py` & `cognite_neat-0.11.5/cognite/neat/core/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.11.5/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.11.5/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/workflow/model.py` & `cognite_neat-0.11.5/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.11.5/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.11.5/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.11.5/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.11.5/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.11.5/cognite/neat/examples/source_graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/fast_graph/workflow.py` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/fast_graph/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/fast_graph/workflow.yaml` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/fast_graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.11.5/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.11.5/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer/explorer.py` & `cognite_neat-0.11.5/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.11.5/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/css/main.19f77ee7.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/js/main.0cd5fec2.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.11.5/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.11.4/pyproject.toml` & `cognite_neat-0.11.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.11.4"
+version = "0.11.5"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 packages = [
```

### Comparing `cognite_neat-0.11.4/PKG-INFO` & `cognite_neat-0.11.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.11.4
+Version: 0.11.5
 Summary: Knowledge graph transformation
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

