# Comparing `tmp/rapidpro_flow_tools-1.0.1.tar.gz` & `tmp/rapidpro_flow_tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpro_flow_tools-1.0.1.tar", last modified: Fri May 19 21:15:17 2023, max compression
+gzip compressed data, was "rapidpro_flow_tools-1.0.2.tar", last modified: Fri May 19 21:56:04 2023, max compression
```

## Comparing `rapidpro_flow_tools-1.0.1.tar` & `rapidpro_flow_tools-1.0.2.tar`

### file list

```diff
@@ -1,70 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.544749 rapidpro_flow_tools-1.0.1/
--rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       89 2023-05-19 21:15:17.544749 rapidpro_flow_tools-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.455776 rapidpro_flow_tools-1.0.1/parsers/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.462942 rapidpro_flow_tools-1.0.1/parsers/common/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/__init__.py
--rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/cellparser.py
--rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/rowdatasheet.py
--rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/rowparser.py
--rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/sheetparser.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.480493 rapidpro_flow_tools-1.0.1/parsers/common/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/__init__.py
--rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/mock_cell_parser.py
--rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/mock_row_parser.py
--rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/mock_sheetparser.py
--rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/models.py
--rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/test_cellparser.py
--rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/test_differentways.py
--rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/test_full_rows.py
--rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/test_rowdatasheet.py
--rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/test_sheetparser.py
--rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/common/tests/test_unparse.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.491601 rapidpro_flow_tools-1.0.1/parsers/creation/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/__init__.py
--rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/constants.py
--rw-rw-rw-   0        0        0     7020 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/contentindexparser.py
--rw-rw-rw-   0        0        0      932 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/contentindexrowmodel.py
--rw-rw-rw-   0        0        0      102 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/datarowmodel.py
--rw-rw-rw-   0        0        0    26665 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/flowparser.py
--rw-rw-rw-   0        0        0     5242 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/flowrowmodel.py
--rw-rw-rw-   0        0        0     1016 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/template_sheet_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.502612 rapidpro_flow_tools-1.0.1/parsers/creation/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/tests/__init__.py
--rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/tests/mock_sheetreader.py
--rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/tests/row_data.py
--rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/tests/test_flowparser.py
--rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/tests/test_to_row_model.py
--rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/creation/tests/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.509157 rapidpro_flow_tools-1.0.1/parsers/sheets/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/sheets/__init__.py
--rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/sheets/csv_sheet_reader.py
--rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-1.0.1/parsers/sheets/google_sheet_reader.py
--rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/parsers/sheets/xlsx_sheet_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.511167 rapidpro_flow_tools-1.0.1/rapidpro/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/rapidpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.520168 rapidpro_flow_tools-1.0.1/rapidpro/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/rapidpro/tests/__init__.py
--rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/rapidpro/tests/test_actions.py
--rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/rapidpro/tests/test_containers.py
--rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/rapidpro/tests/test_import_export.py
--rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/rapidpro/tests/test_nodes.py
--rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/rapidpro/tests/test_routers.py
--rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/rapidpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.531705 rapidpro_flow_tools-1.0.1/rapidpro_flow_tools.egg-info/
--rw-rw-rw-   0        0        0       89 2023-05-19 21:15:17.000000 rapidpro_flow_tools-1.0.1/rapidpro_flow_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1874 2023-05-19 21:15:17.000000 rapidpro_flow_tools-1.0.1/rapidpro_flow_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 21:15:17.000000 rapidpro_flow_tools-1.0.1/rapidpro_flow_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-19 21:15:17.000000 rapidpro_flow_tools-1.0.1/rapidpro_flow_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-19 21:15:17.545759 rapidpro_flow_tools-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      146 2023-05-19 21:14:54.000000 rapidpro_flow_tools-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 21:15:17.542238 rapidpro_flow_tools-1.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/tests/test_contentindexparser.py
--rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/tests/test_flowparser.py
--rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/tests/test_flowparser_reverse.py
--rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/tests/test_template_sheet_parser.py
--rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.1/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.685563 rapidpro_flow_tools-1.0.2/
+-rw-rw-rw-   0        0        0    27030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3518 2023-05-19 21:56:04.684565 rapidpro_flow_tools-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/README.md
+-rw-rw-rw-   0        0        0      692 2023-05-19 21:45:01.000000 rapidpro_flow_tools-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 21:56:04.685563 rapidpro_flow_tools-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.509240 rapidpro_flow_tools-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.535817 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-05-17 15:46:39.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/flow_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.558896 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.566906 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/__init__.py
+-rw-rw-rw-   0        0        0     4152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/cellparser.py
+-rw-rw-rw-   0        0        0     3205 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py
+-rw-rw-rw-   0        0        0    15945 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/rowparser.py
+-rw-rw-rw-   0        0        0     1849 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/sheetparser.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.589434 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/__init__.py
+-rw-rw-rw-   0        0        0      163 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/mock_cell_parser.py
+-rw-rw-rw-   0        0        0      292 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/mock_row_parser.py
+-rw-rw-rw-   0        0        0      826 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py
+-rw-rw-rw-   0        0        0      600 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/models.py
+-rw-rw-rw-   0        0        0     6080 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py
+-rw-rw-rw-   0        0        0     3508 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py
+-rw-rw-rw-   0        0        0     5026 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py
+-rw-rw-rw-   0        0        0     3050 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py
+-rw-rw-rw-   0        0        0     2022 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py
+-rw-rw-rw-   0        0        0     4684 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.612554 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/constants.py
+-rw-rw-rw-   0        0        0     7020 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py
+-rw-rw-rw-   0        0        0      932 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py
+-rw-rw-rw-   0        0        0      102 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/datarowmodel.py
+-rw-rw-rw-   0        0        0    26665 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/flowparser.py
+-rw-rw-rw-   0        0        0     5242 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py
+-rw-rw-rw-   0        0        0     1016 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.625076 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.633098 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/
+-rw-rw-rw-   0        0        0      179 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/evalmodels.py
+-rw-rw-rw-   0        0        0      444 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/listmodel.py
+-rw-rw-rw-   0        0        0      557 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/nestedmodel.py
+-rw-rw-rw-   0        0        0      133 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/datarowmodels/simplemodel.py
+-rw-rw-rw-   0        0        0      478 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/mock_sheetreader.py
+-rw-rw-rw-   0        0        0     1030 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py
+-rw-rw-rw-   0        0        0    17043 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0    39668 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0    14789 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py
+-rw-rw-rw-   0        0        0      259 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.639094 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/sheets/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/sheets/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py
+-rw-rw-rw-   0        0        0     3199 2023-05-17 13:33:29.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py
+-rw-rw-rw-   0        0        0      711 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.642183 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.650186 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/models/
+-rw-rw-rw-   0        0        0    11728 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/models/actions.py
+-rw-rw-rw-   0        0        0     1004 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/models/common.py
+-rw-rw-rw-   0        0        0    10931 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/models/containers.py
+-rw-rw-rw-   0        0        0    20809 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/models/nodes.py
+-rw-rw-rw-   0        0        0    18753 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/models/routers.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.659253 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/__init__.py
+-rw-rw-rw-   0        0        0      542 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py
+-rw-rw-rw-   0        0        0     3453 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py
+-rw-rw-rw-   0        0        0     4525 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py
+-rw-rw-rw-   0        0        0     1304 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py
+-rw-rw-rw-   0        0        0     6368 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py
+-rw-rw-rw-   0        0        0       73 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.668942 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.526799 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.670937 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/epicsa_chatbot/
+-rw-rw-rw-   0        0        0      282 2023-05-09 00:55:58.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/epicsa_chatbot/epicsa_models.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.671938 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/example1/
+-rw-rw-rw-   0        0        0      557 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/example1/nestedmodel.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.675553 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/parenttext/
+-rw-rw-rw-   0        0        0     5926 2023-05-09 00:55:58.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/parenttext/parenttext_models.py
+-rw-rw-rw-   0        0        0     2231 2023-05-09 00:55:58.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/parenttext/parenttext_models_delivery.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.677565 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/srh_chatbot/
+-rw-rw-rw-   0        0        0     1818 2023-05-09 00:55:58.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/input/srh_chatbot/srh_models.py
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py
+-rw-rw-rw-   0        0        0    11693 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.557885 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools.egg-info/
+-rw-rw-rw-   0        0        0     3518 2023-05-19 21:56:04.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4192 2023-05-19 21:56:04.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 21:56:04.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-19 21:56:04.000000 rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 21:56:04.682563 rapidpro_flow_tools-1.0.2/tests/
+-rw-rw-rw-   0        0        0     2194 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/tests/test_contentindexparser.py
+-rw-rw-rw-   0        0        0     6373 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/tests/test_flowparser.py
+-rw-rw-rw-   0        0        0     2997 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/tests/test_flowparser_reverse.py
+-rw-rw-rw-   0        0        0     2437 2023-05-08 22:11:19.000000 rapidpro_flow_tools-1.0.2/tests/test_template_sheet_parser.py
```

### Comparing `rapidpro_flow_tools-1.0.1/LICENSE` & `rapidpro_flow_tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/README.md` & `rapidpro_flow_tools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/cellparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/rowdatasheet.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/rowparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/rowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/sheetparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/tests/mock_sheetparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/mock_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/tests/models.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/models.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/tests/test_cellparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_cellparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/tests/test_differentways.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_differentways.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/tests/test_full_rows.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_full_rows.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/tests/test_rowdatasheet.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_rowdatasheet.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/tests/test_sheetparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_sheetparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/common/tests/test_unparse.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/common/tests/test_unparse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/creation/contentindexparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/creation/contentindexrowmodel.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/contentindexrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/creation/flowparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/creation/flowrowmodel.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/flowrowmodel.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/creation/template_sheet_parser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/creation/tests/row_data.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/row_data.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/creation/tests/test_contentindexparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/creation/tests/test_flowparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/creation/tests/test_to_row_model.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/creation/tests/test_to_row_model.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/sheets/csv_sheet_reader.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/sheets/csv_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/sheets/google_sheet_reader.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/sheets/google_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/parsers/sheets/xlsx_sheet_reader.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/parsers/sheets/xlsx_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/rapidpro/tests/test_actions.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/rapidpro/tests/test_containers.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/rapidpro/tests/test_import_export.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_import_export.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/rapidpro/tests/test_nodes.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/rapidpro/tests/test_routers.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/rapidpro/tests/test_routers.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/tests/test_contentindexparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/test_contentindexparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/tests/test_flowparser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/test_flowparser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/tests/test_flowparser_reverse.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/test_flowparser_reverse.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/tests/test_template_sheet_parser.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/test_template_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `rapidpro_flow_tools-1.0.1/tests/utils.py` & `rapidpro_flow_tools-1.0.2/src/rapidpro_flow_tools/tests/utils.py`

 * *Files identical despite different names*

